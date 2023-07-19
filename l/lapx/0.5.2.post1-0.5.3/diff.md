# Comparing `tmp/lapx-0.5.2.post1.tar.gz` & `tmp/lapx-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapx-0.5.2.post1.tar", last modified: Sun Jun 25 23:38:21 2023, max compression
+gzip compressed data, was "lapx-0.5.3.tar", last modified: Wed Jul 19 01:05:25 2023, max compression
```

## Comparing `lapx-0.5.2.post1.tar` & `lapx-0.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:21.900530 lapx-0.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-25 23:38:21.900530 lapx-0.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:21.896530 lapx-0.5.2.post1/_lapjv_src/
--rw-r--r--   0 runner    (1001) docker     (123)   398869 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/_lapjv_src/_lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/_lapjv_src/_lapjv.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/_lapjv_src/lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/_lapjv_src/lapjv.h
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/_lapjv_src/lapmod.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:21.896530 lapx-0.5.2.post1/lap/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/lapmod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:21.900530 lapx-0.5.2.post1/lap/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1415310 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/cost_eps.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/test_arr_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/test_lapjv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/test_lapmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/lap/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:38:21.900530 lapx-0.5.2.post1/lapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/lapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/lapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/lapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/lapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 23:38:21.000000 lapx-0.5.2.post1/lapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 23:38:21.900530 lapx-0.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-25 23:38:05.000000 lapx-0.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:25.676572 lapx-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-19 01:05:01.000000 lapx-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-19 01:05:01.000000 lapx-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-19 01:05:25.676572 lapx-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-19 01:05:01.000000 lapx-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:25.672572 lapx-0.5.3/_lapjv_src/
+-rw-r--r--   0 runner    (1001) docker     (123)   540872 2023-07-19 01:05:25.000000 lapx-0.5.3/_lapjv_src/_lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-19 01:05:01.000000 lapx-0.5.3/_lapjv_src/_lapjv.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-19 01:05:01.000000 lapx-0.5.3/_lapjv_src/lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-19 01:05:01.000000 lapx-0.5.3/_lapjv_src/lapjv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-19 01:05:01.000000 lapx-0.5.3/_lapjv_src/lapmod.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:25.672572 lapx-0.5.3/lap/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/lapmod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:25.676572 lapx-0.5.3/lap/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1415310 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/cost_eps.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/test_arr_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/test_lapjv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/test_lapmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-19 01:05:01.000000 lapx-0.5.3/lap/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:05:25.676572 lapx-0.5.3/lapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-19 01:05:25.000000 lapx-0.5.3/lapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-19 01:05:25.000000 lapx-0.5.3/lapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 01:05:25.000000 lapx-0.5.3/lapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 01:05:25.000000 lapx-0.5.3/lapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-19 01:05:25.000000 lapx-0.5.3/lapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-19 01:05:01.000000 lapx-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 01:05:01.000000 lapx-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 01:05:25.680572 lapx-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-19 01:05:01.000000 lapx-0.5.3/setup.py
```

### Comparing `lapx-0.5.2.post1/LICENSE` & `lapx-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/PKG-INFO` & `lapx-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.2.post1
-Summary: Customized Tomas Kazmar's lap, Linear Assignment Problem solver (LAPJV/LAPMOD).
+Version: 0.5.3
+Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap,lap05
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,71 +27,66 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Windows/Linux/macOS + Python [3.7-3.11] .](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml)
-[![Build `tar.gz` PyPI](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml)
+[![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test.yaml)
+[![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
+[![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-* `lapx` is a customized edition of Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap).
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE).
-* Source credit: Tomas Kazmar @[`gatagat`](https://github.com/gatagat).
-* `pypi.org` source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11.
 
+* License: BSD-2-Clause, see [`LICENSE`](LICENSE)
+* Based source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+* Credits: @[`gatagat`](https://github.com/gatagat) @[`remram44`](https://github.com/gatagat/lap/issues/34#issue-1114097201)
 
-## Windows ✅ | Linux ✅ | macOS ✅
+## Installation: Windows ✅ | Linux ✅ | macOS ✅
 
-* Build passed on all [Windows/Linux/macOS](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml) with Python 3.7/3.8/3.9/3.10/3.11 ✅
-
-* Install from PyPI:
+* Install from [PyPI](https://pypi.org/project/lapx/):
 
   ```
   pip install lapx
   ```
 
-* Or download [`tar.gz` or Wheels from releases](https://github.com/rathaROG/lapx/releases)
-
-* Or directly install from GitHub:
+* Or install `.tar.gz` or `.whl` from [GitHub releases](https://github.com/rathaROG/lapx/releases) or install from GitHub repo directly:
 
   ```
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
   pip install git+https://github.com/rathaROG/lapx.git
   ```
 
-* Or clone and build directly on your machine:
+* Or clone and build on your local machine:
 
   ```
   git clone https://github.com/rathaROG/lapx.git
   cd lapx
   python -m pip install --upgrade pip
   pip install "setuptools>=67.2.0"
   pip install wheel build
   python -m build --wheel
   cd dist
   ```
 
 ## Usage 🧪
 
-Note: Use `import lap` to import since `lapx` is just the name for package distribution. 
+* `lapx` is just the name for package distribution.
+* The same as `lap`, use `import lap` to import; for example:
 
-```
-import lap
-import numpy as np
-print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
-```
+  ```
+  import lap
+  import numpy as np
+  print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
+  ```
 
 <br />
 
-<details><summary><ins>Click here to show more ...</ins></summary>
+<details><summary>Click here to show more...</summary>
 
 <br />
 
 lap: Linear Assignment Problem solver
 =====================================
 
 **lap** is a [linear assignment
```

### Comparing `lapx-0.5.2.post1/README.md` & `lapx-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-[![Windows/Linux/macOS + Python [3.7-3.11] .](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml)
-[![Build `tar.gz` PyPI](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml)
+[![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test.yaml)
+[![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
+[![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-* `lapx` is a customized edition of Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap).
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE).
-* Source credit: Tomas Kazmar @[`gatagat`](https://github.com/gatagat).
-* `pypi.org` source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11.
 
+* License: BSD-2-Clause, see [`LICENSE`](LICENSE)
+* Based source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+* Credits: @[`gatagat`](https://github.com/gatagat) @[`remram44`](https://github.com/gatagat/lap/issues/34#issue-1114097201)
 
-## Windows ✅ | Linux ✅ | macOS ✅
+## Installation: Windows ✅ | Linux ✅ | macOS ✅
 
-* Build passed on all [Windows/Linux/macOS](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml) with Python 3.7/3.8/3.9/3.10/3.11 ✅
-
-* Install from PyPI:
+* Install from [PyPI](https://pypi.org/project/lapx/):
 
   ```
   pip install lapx
   ```
 
-* Or download [`tar.gz` or Wheels from releases](https://github.com/rathaROG/lapx/releases)
-
-* Or directly install from GitHub:
+* Or install `.tar.gz` or `.whl` from [GitHub releases](https://github.com/rathaROG/lapx/releases) or install from GitHub repo directly:
 
   ```
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
   pip install git+https://github.com/rathaROG/lapx.git
   ```
 
-* Or clone and build directly on your machine:
+* Or clone and build on your local machine:
 
   ```
   git clone https://github.com/rathaROG/lapx.git
   cd lapx
   python -m pip install --upgrade pip
   pip install "setuptools>=67.2.0"
   pip install wheel build
   python -m build --wheel
   cd dist
   ```
 
 ## Usage 🧪
 
-Note: Use `import lap` to import since `lapx` is just the name for package distribution. 
+* `lapx` is just the name for package distribution.
+* The same as `lap`, use `import lap` to import; for example:
 
-```
-import lap
-import numpy as np
-print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
-```
+  ```
+  import lap
+  import numpy as np
+  print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
+  ```
 
 <br />
 
-<details><summary><ins>Click here to show more ...</ins></summary>
+<details><summary>Click here to show more...</summary>
 
 <br />
 
 lap: Linear Assignment Problem solver
 =====================================
 
 **lap** is a [linear assignment
```

### Comparing `lapx-0.5.2.post1/_lapjv_src/_lapjv.cpp` & `lapx-0.5.3/_lapjv_src/_lapjv.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -31,31 +43,90 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -72,80 +143,102 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PYSTON_VERSION)
+#elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
   #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
   #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
@@ -181,37 +274,35 @@
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -226,45 +317,67 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -286,78 +399,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
+        #else
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -373,49 +536,48 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
         if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
         if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
         if (!(nlocals=PyLong_FromLong(l))) goto end;
         if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
         if (!(stacksize=PyLong_FromLong(s))) goto end;
         if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
@@ -427,104 +589,180 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -547,46 +785,120 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_READY(op)       (0)
   #else
     #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                                 0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -596,37 +908,43 @@
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -647,16 +965,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -667,25 +991,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -695,19 +1024,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -744,35 +1068,40 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE___lapjv
 #define __PYX_HAVE_API___lapjv
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
+
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
+    
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
-
-    /* NumPy API declarations from "numpy/__init__.pxd" */
-    
 #include <stdlib.h>
 #include "lapjv.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
@@ -835,29 +1164,40 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -875,15 +1215,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -897,15 +1282,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -962,31 +1347,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -996,22 +1377,23 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "_lapjv_src/_lapjv.pyx",
-  "__init__.pxd",
+  "__init__.cython-30.pxd",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -1038,368 +1420,378 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+struct __pyx_defaults;
+typedef struct __pyx_defaults __pyx_defaults;
+struct __pyx_defaults1;
+typedef struct __pyx_defaults1 __pyx_defaults1;
+struct __pyx_defaults {
+  double __pyx_arg_cost_limit;
+};
+struct __pyx_defaults1 {
+  enum fp_t __pyx_arg_fp_version;
+};
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
-
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
-
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1407,17 +1799,122 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
+    const char* function_name);
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1494,67 +1991,61 @@
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
+#endif
+#endif
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
+#define __Pyx_BufPtrCContig2d(type, buf, i0, s0, i1, s1) ((type)((char*)buf + i0 * s0) + i1)
+#define __Pyx_BufPtrCContig1d(type, buf, i0, s0) ((type)buf + i0)
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-#define __Pyx_BufPtrCContig2d(type, buf, i0, s0, i1, s1) ((type)((char*)buf + i0 * s0) + i1)
-#define __Pyx_BufPtrCContig1d(type, buf, i0, s0) ((type)buf + i0)
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1571,102 +2062,196 @@
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
+};
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
+#endif
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
-/* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
-#if __STDC_VERSION__ >= 201112L
-#include <stdalign.h>
-#endif
-#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+    PyCMethodObject func;
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
-};
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
 #endif
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1688,15 +2273,15 @@
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
@@ -1715,15 +2300,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1753,15 +2338,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1820,99 +2405,110 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int_t(int_t value);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cpython.buffer' */
-
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
+/* Module declarations from "cython" */
 
-/* Module declarations from 'cython' */
+/* Module declarations from "libc.stdlib" */
 
-/* Module declarations from 'libc.stdlib' */
-
-/* Module declarations from '_lapjv' */
+/* Module declarations from "_lapjv" */
+/* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_double_t = { "double_t", NULL, sizeof(__pyx_t_5numpy_double_t), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn_int_t = { "int_t", NULL, sizeof(int_t), { 0 }, 0, IS_UNSIGNED(int_t) ? 'U' : 'I', IS_UNSIGNED(int_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint_t = { "uint_t", NULL, sizeof(uint_t), { 0 }, 0, IS_UNSIGNED(uint_t) ? 'U' : 'I', IS_UNSIGNED(uint_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn_int_t = { "int_t", NULL, sizeof(int_t), { 0 }, 0, __PYX_IS_UNSIGNED(int_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint_t = { "uint_t", NULL, sizeof(uint_t), { 0 }, 0, __PYX_IS_UNSIGNED(uint_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(uint_t), 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "_lapjv"
 extern int __pyx_module_is_main__lapjv;
 int __pyx_module_is_main__lapjv = 0;
 
-/* Implementation of '_lapjv' */
+/* Implementation of "_lapjv" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_n[] = "n";
+static const char __pyx_k__7[] = "*";
 static const char __pyx_k_cc[] = "cc";
 static const char __pyx_k_ii[] = "ii";
 static const char __pyx_k_kk[] = "kk";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k__12[] = "?";
 static const char __pyx_k_inf[] = "inf";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_nan[] = "nan";
 static const char __pyx_k_opt[] = "opt";
 static const char __pyx_k_ret[] = "ret";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_x_c[] = "x_c";
@@ -1921,14 +2517,15 @@
 static const char __pyx_k_FP_2[] = "FP_2_";
 static const char __pyx_k_cc_c[] = "cc_c";
 static const char __pyx_k_cost[] = "cost";
 static const char __pyx_k_ii_c[] = "ii_c";
 static const char __pyx_k_kk_c[] = "kk_c";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_LARGE[] = "LARGE_";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_lapjv[] = "lapjv";
 static const char __pyx_k_numpy[] = "numpy";
@@ -1949,230 +2546,2077 @@
 static const char __pyx_k_cost_limit[] = "cost_limit";
 static const char __pyx_k_fp_version[] = "fp_version";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_extend_cost[] = "extend_cost";
 static const char __pyx_k_return_cost[] = "return_cost";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_Out_of_memory[] = "Out of memory.";
+static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_cost_c_extended[] = "cost_c_extended";
 static const char __pyx_k_ascontiguousarray[] = "ascontiguousarray";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_lapjv_src__lapjv_pyx[] = "_lapjv_src/_lapjv.pyx";
 static const char __pyx_k_2_dimensional_array_expected[] = "2-dimensional array expected";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Square_cost_array_expected_If_co[] = "Square cost array expected. If cost is intentionally non-square, pass extend_cost=True.";
 static const char __pyx_k_Unknown_error_lapjv_internal_ret[] = "Unknown error (lapjv_internal returned %d).";
 static const char __pyx_k_Unknown_error_lapmod_internal_re[] = "Unknown error (lapmod_internal returned %d).";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static PyObject *__pyx_kp_u_2_dimensional_array_expected;
-static PyObject *__pyx_n_s_FP_1;
-static PyObject *__pyx_n_s_FP_2;
-static PyObject *__pyx_n_s_FP_DYNAMIC;
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_LARGE;
-static PyObject *__pyx_n_s_MemoryError;
-static PyObject *__pyx_kp_u_Out_of_memory;
-static PyObject *__pyx_n_s_RuntimeError;
-static PyObject *__pyx_kp_u_Square_cost_array_expected_If_co;
-static PyObject *__pyx_kp_u_Unknown_error_lapjv_internal_ret;
-static PyObject *__pyx_kp_u_Unknown_error_lapmod_internal_re;
-static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_n_s_arange;
-static PyObject *__pyx_n_s_ascontiguousarray;
-static PyObject *__pyx_n_s_cc;
-static PyObject *__pyx_n_s_cc_c;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_cost;
-static PyObject *__pyx_n_s_cost_c;
-static PyObject *__pyx_n_s_cost_c_extended;
-static PyObject *__pyx_n_s_cost_limit;
-static PyObject *__pyx_n_s_cost_ptr;
-static PyObject *__pyx_n_s_double;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_empty;
-static PyObject *__pyx_n_s_extend_cost;
-static PyObject *__pyx_n_s_fp_version;
-static PyObject *__pyx_n_s_i;
-static PyObject *__pyx_n_s_ii;
-static PyObject *__pyx_n_s_ii_c;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_inf;
-static PyObject *__pyx_n_s_int32;
-static PyObject *__pyx_n_s_kk;
-static PyObject *__pyx_n_s_kk_c;
-static PyObject *__pyx_n_s_lapjv;
-static PyObject *__pyx_n_s_lapjv_2;
-static PyObject *__pyx_kp_s_lapjv_src__lapjv_pyx;
-static PyObject *__pyx_n_s_lapmod;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_max;
-static PyObject *__pyx_n_s_n;
-static PyObject *__pyx_n_s_n_cols;
-static PyObject *__pyx_n_s_n_rows;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_nan;
-static PyObject *__pyx_n_s_nonzero;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_opt;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_s_ret;
-static PyObject *__pyx_n_s_return_cost;
-static PyObject *__pyx_n_s_sum;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_uint32;
-static PyObject *__pyx_n_s_x_c;
-static PyObject *__pyx_n_s_y_c;
+/* #### Code section: decls ### */
+static PyObject *__pyx_pf_6_lapjv_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6_lapjv_lapjv(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_cost, char __pyx_v_extend_cost, double __pyx_v_cost_limit, char __pyx_v_return_cost); /* proto */
+static PyObject *__pyx_pf_6_lapjv_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6_lapjv_2_lapmod(CYTHON_UNUSED PyObject *__pyx_self, uint_t __pyx_v_n, PyArrayObject *__pyx_v_cc, PyArrayObject *__pyx_v_ii, PyArrayObject *__pyx_v_kk, enum fp_t __pyx_v_fp_version); /* proto */
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_1;
-static PyObject *__pyx_int_neg_1;
-static double __pyx_k_;
-static enum fp_t __pyx_k__6;
-static PyObject *__pyx_slice__4;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_codeobj__10;
-static PyObject *__pyx_codeobj__12;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_kp_u_2_dimensional_array_expected;
+  PyObject *__pyx_n_s_FP_1;
+  PyObject *__pyx_n_s_FP_2;
+  PyObject *__pyx_n_s_FP_DYNAMIC;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s_LARGE;
+  PyObject *__pyx_n_s_MemoryError;
+  PyObject *__pyx_kp_u_Out_of_memory;
+  PyObject *__pyx_n_s_RuntimeError;
+  PyObject *__pyx_kp_u_Square_cost_array_expected_If_co;
+  PyObject *__pyx_kp_u_Unknown_error_lapjv_internal_ret;
+  PyObject *__pyx_kp_u_Unknown_error_lapmod_internal_re;
+  PyObject *__pyx_n_s_ValueError;
+  PyObject *__pyx_n_s__12;
+  PyObject *__pyx_n_s__7;
+  PyObject *__pyx_n_s_arange;
+  PyObject *__pyx_n_s_ascontiguousarray;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_cc;
+  PyObject *__pyx_n_s_cc_c;
+  PyObject *__pyx_n_s_class_getitem;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_cost;
+  PyObject *__pyx_n_s_cost_c;
+  PyObject *__pyx_n_s_cost_c_extended;
+  PyObject *__pyx_n_s_cost_limit;
+  PyObject *__pyx_n_s_cost_ptr;
+  PyObject *__pyx_n_s_double;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_empty;
+  PyObject *__pyx_n_s_extend_cost;
+  PyObject *__pyx_n_s_fp_version;
+  PyObject *__pyx_n_s_i;
+  PyObject *__pyx_n_s_ii;
+  PyObject *__pyx_n_s_ii_c;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_inf;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_int32;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_n_s_kk;
+  PyObject *__pyx_n_s_kk_c;
+  PyObject *__pyx_n_s_lapjv;
+  PyObject *__pyx_n_s_lapjv_2;
+  PyObject *__pyx_kp_s_lapjv_src__lapjv_pyx;
+  PyObject *__pyx_n_s_lapmod;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_max;
+  PyObject *__pyx_n_s_n;
+  PyObject *__pyx_n_s_n_cols;
+  PyObject *__pyx_n_s_n_rows;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_nan;
+  PyObject *__pyx_n_s_nonzero;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_opt;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_ret;
+  PyObject *__pyx_n_s_return_cost;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_sum;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_uint32;
+  PyObject *__pyx_n_s_x_c;
+  PyObject *__pyx_n_s_y_c;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_int_1;
+  PyObject *__pyx_int_neg_1;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_slice__5;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_2_dimensional_array_expected);
+  Py_CLEAR(clear_module_state->__pyx_n_s_FP_1);
+  Py_CLEAR(clear_module_state->__pyx_n_s_FP_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_FP_DYNAMIC);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_LARGE);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Out_of_memory);
+  Py_CLEAR(clear_module_state->__pyx_n_s_RuntimeError);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Square_cost_array_expected_If_co);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_error_lapjv_internal_ret);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_error_lapmod_internal_re);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__7);
+  Py_CLEAR(clear_module_state->__pyx_n_s_arange);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ascontiguousarray);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cc_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cost);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cost_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cost_c_extended);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cost_limit);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cost_ptr);
+  Py_CLEAR(clear_module_state->__pyx_n_s_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_empty);
+  Py_CLEAR(clear_module_state->__pyx_n_s_extend_cost);
+  Py_CLEAR(clear_module_state->__pyx_n_s_fp_version);
+  Py_CLEAR(clear_module_state->__pyx_n_s_i);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ii);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ii_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_inf);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_n_s_kk);
+  Py_CLEAR(clear_module_state->__pyx_n_s_kk_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lapjv);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lapjv_2);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_lapjv_src__lapjv_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lapmod);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_max);
+  Py_CLEAR(clear_module_state->__pyx_n_s_n);
+  Py_CLEAR(clear_module_state->__pyx_n_s_n_cols);
+  Py_CLEAR(clear_module_state->__pyx_n_s_n_rows);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nan);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nonzero);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_opt);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ret);
+  Py_CLEAR(clear_module_state->__pyx_n_s_return_cost);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_uint32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_x_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_y_c);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_int_neg_1);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_slice__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_2_dimensional_array_expected);
+  Py_VISIT(traverse_module_state->__pyx_n_s_FP_1);
+  Py_VISIT(traverse_module_state->__pyx_n_s_FP_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_FP_DYNAMIC);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_LARGE);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Out_of_memory);
+  Py_VISIT(traverse_module_state->__pyx_n_s_RuntimeError);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Square_cost_array_expected_If_co);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_error_lapjv_internal_ret);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_error_lapmod_internal_re);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__7);
+  Py_VISIT(traverse_module_state->__pyx_n_s_arange);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ascontiguousarray);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cc_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cost);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cost_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cost_c_extended);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cost_limit);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cost_ptr);
+  Py_VISIT(traverse_module_state->__pyx_n_s_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_empty);
+  Py_VISIT(traverse_module_state->__pyx_n_s_extend_cost);
+  Py_VISIT(traverse_module_state->__pyx_n_s_fp_version);
+  Py_VISIT(traverse_module_state->__pyx_n_s_i);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ii);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ii_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_inf);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_n_s_kk);
+  Py_VISIT(traverse_module_state->__pyx_n_s_kk_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lapjv);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lapjv_2);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_lapjv_src__lapjv_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lapmod);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_max);
+  Py_VISIT(traverse_module_state->__pyx_n_s_n);
+  Py_VISIT(traverse_module_state->__pyx_n_s_n_cols);
+  Py_VISIT(traverse_module_state->__pyx_n_s_n_rows);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nan);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nonzero);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_opt);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ret);
+  Py_VISIT(traverse_module_state->__pyx_n_s_return_cost);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_uint32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_x_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_y_c);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_int_neg_1);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_slice__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_kp_u_2_dimensional_array_expected __pyx_mstate_global->__pyx_kp_u_2_dimensional_array_expected
+#define __pyx_n_s_FP_1 __pyx_mstate_global->__pyx_n_s_FP_1
+#define __pyx_n_s_FP_2 __pyx_mstate_global->__pyx_n_s_FP_2
+#define __pyx_n_s_FP_DYNAMIC __pyx_mstate_global->__pyx_n_s_FP_DYNAMIC
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s_LARGE __pyx_mstate_global->__pyx_n_s_LARGE
+#define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
+#define __pyx_kp_u_Out_of_memory __pyx_mstate_global->__pyx_kp_u_Out_of_memory
+#define __pyx_n_s_RuntimeError __pyx_mstate_global->__pyx_n_s_RuntimeError
+#define __pyx_kp_u_Square_cost_array_expected_If_co __pyx_mstate_global->__pyx_kp_u_Square_cost_array_expected_If_co
+#define __pyx_kp_u_Unknown_error_lapjv_internal_ret __pyx_mstate_global->__pyx_kp_u_Unknown_error_lapjv_internal_ret
+#define __pyx_kp_u_Unknown_error_lapmod_internal_re __pyx_mstate_global->__pyx_kp_u_Unknown_error_lapmod_internal_re
+#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
+#define __pyx_n_s__12 __pyx_mstate_global->__pyx_n_s__12
+#define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
+#define __pyx_n_s_arange __pyx_mstate_global->__pyx_n_s_arange
+#define __pyx_n_s_ascontiguousarray __pyx_mstate_global->__pyx_n_s_ascontiguousarray
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_cc __pyx_mstate_global->__pyx_n_s_cc
+#define __pyx_n_s_cc_c __pyx_mstate_global->__pyx_n_s_cc_c
+#define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_cost __pyx_mstate_global->__pyx_n_s_cost
+#define __pyx_n_s_cost_c __pyx_mstate_global->__pyx_n_s_cost_c
+#define __pyx_n_s_cost_c_extended __pyx_mstate_global->__pyx_n_s_cost_c_extended
+#define __pyx_n_s_cost_limit __pyx_mstate_global->__pyx_n_s_cost_limit
+#define __pyx_n_s_cost_ptr __pyx_mstate_global->__pyx_n_s_cost_ptr
+#define __pyx_n_s_double __pyx_mstate_global->__pyx_n_s_double
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_empty __pyx_mstate_global->__pyx_n_s_empty
+#define __pyx_n_s_extend_cost __pyx_mstate_global->__pyx_n_s_extend_cost
+#define __pyx_n_s_fp_version __pyx_mstate_global->__pyx_n_s_fp_version
+#define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
+#define __pyx_n_s_ii __pyx_mstate_global->__pyx_n_s_ii
+#define __pyx_n_s_ii_c __pyx_mstate_global->__pyx_n_s_ii_c
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_inf __pyx_mstate_global->__pyx_n_s_inf
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_int32 __pyx_mstate_global->__pyx_n_s_int32
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_n_s_kk __pyx_mstate_global->__pyx_n_s_kk
+#define __pyx_n_s_kk_c __pyx_mstate_global->__pyx_n_s_kk_c
+#define __pyx_n_s_lapjv __pyx_mstate_global->__pyx_n_s_lapjv
+#define __pyx_n_s_lapjv_2 __pyx_mstate_global->__pyx_n_s_lapjv_2
+#define __pyx_kp_s_lapjv_src__lapjv_pyx __pyx_mstate_global->__pyx_kp_s_lapjv_src__lapjv_pyx
+#define __pyx_n_s_lapmod __pyx_mstate_global->__pyx_n_s_lapmod
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_max __pyx_mstate_global->__pyx_n_s_max
+#define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
+#define __pyx_n_s_n_cols __pyx_mstate_global->__pyx_n_s_n_cols
+#define __pyx_n_s_n_rows __pyx_mstate_global->__pyx_n_s_n_rows
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_nan __pyx_mstate_global->__pyx_n_s_nan
+#define __pyx_n_s_nonzero __pyx_mstate_global->__pyx_n_s_nonzero
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
+#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_opt __pyx_mstate_global->__pyx_n_s_opt
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_ret __pyx_mstate_global->__pyx_n_s_ret
+#define __pyx_n_s_return_cost __pyx_mstate_global->__pyx_n_s_return_cost
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_sum __pyx_mstate_global->__pyx_n_s_sum
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_uint32 __pyx_mstate_global->__pyx_n_s_uint32
+#define __pyx_n_s_x_c __pyx_mstate_global->__pyx_n_s_x_c
+#define __pyx_n_s_y_c __pyx_mstate_global->__pyx_n_s_y_c
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_slice__5 __pyx_mstate_global->__pyx_slice__5
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+/* #### Code section: module_code ### */
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
+ * 
+ *     ctypedef unsigned char      npy_bool
+ */
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):
+ *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_array_base", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ */
+  Py_INCREF(__pyx_v_base);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ */
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 969, __pyx_L1_error)
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("get_array_base", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
+ *         return None
+ */
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = (__pyx_v_base == NULL);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ *         return None             # <<<<<<<<<<<<<<
+ *     return <object>base
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+ *     if base is NULL:
+ *         return None
+ *     return <object>base             # <<<<<<<<<<<<<<
+ * 
+ * # Versions of the import_* functions which are more suitable for
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_array", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+ * cdef inline int import_array() except -1:
+ *     try:
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ */
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 981, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+ *     try:
+ *         __pyx_import_array()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 982, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 983, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_umath", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+ * cdef inline int import_umath() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 987, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 989, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_ufunc", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+ * cdef inline int import_ufunc() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 993, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 995, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "_lapjv.pyx":41
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
+ */
 
-/* "_lapjv.pyx":43
+static PyObject *__pyx_pf_6_lapjv_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 0);
+  __Pyx_XDECREF(__pyx_r);
+
+  /* "_lapjv.pyx":43
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
  *           double cost_limit=np.inf, char return_cost=True):
  *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
  */
+  __pyx_t_1 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  /* "_lapjv.pyx":41
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
+ */
+  __pyx_t_2 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_cost_limit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "_lapjv.pyx":44
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
+ *           double cost_limit=np.inf, char return_cost=True):             # <<<<<<<<<<<<<<
+ *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  /* "_lapjv.pyx":41
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
+ */
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, Py_None);
+  __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("_lapjv.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6_lapjv_1lapjv(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6_lapjv_lapjv[] = "Solve linear assignment problem using Jonker-Volgenant algorithm.\n\n    Parameters\n    ----------\n    cost: (N,N) ndarray\n        Cost matrix. Entry `cost[i, j]` is the cost of assigning row `i` to\n        column `j`.\n    extend_cost: bool, optional\n        Whether or not extend a non-square matrix. Default: False.\n    cost_limit: double, optional\n        An upper limit for a cost of a single assignment. Default: `np.inf`.\n    return_cost: bool, optional\n        Whether or not to return the assignment cost.\n\n    Returns\n    -------\n    opt: double\n        Assignment cost. Not returned if `return_cost is False`.\n    x: (N,) ndarray\n        Assignment. `x[i]` specifies the column to which row `i` is assigned.\n    y: (N,) ndarray\n        Assignment. `y[j]` specifies the row to which column `j` is assigned.\n\n    Notes\n    -----\n    For non-square matrices (with `extend_cost is True`) or `cost_limit` set\n    low enough, there will be unmatched rows, columns in the solution `x`, `y`.\n    All such entries are set to -1.\n    ";
-static PyMethodDef __pyx_mdef_6_lapjv_1lapjv = {"lapjv", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6_lapjv_1lapjv, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6_lapjv_lapjv};
-static PyObject *__pyx_pw_6_lapjv_1lapjv(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6_lapjv_1lapjv(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6_lapjv_lapjv, "Solve linear assignment problem using Jonker-Volgenant algorithm.\n\n    Parameters\n    ----------\n    cost: (N,N) ndarray\n        Cost matrix. Entry `cost[i, j]` is the cost of assigning row `i` to\n        column `j`.\n    extend_cost: bool, optional\n        Whether or not extend a non-square matrix. Default: False.\n    cost_limit: double, optional\n        An upper limit for a cost of a single assignment. Default: `np.inf`.\n    return_cost: bool, optional\n        Whether or not to return the assignment cost.\n\n    Returns\n    -------\n    opt: double\n        Assignment cost. Not returned if `return_cost is False`.\n    x: (N,) ndarray\n        Assignment. `x[i]` specifies the column to which row `i` is assigned.\n    y: (N,) ndarray\n        Assignment. `y[j]` specifies the row to which column `j` is assigned.\n\n    Notes\n    -----\n    For non-square matrices (with `extend_cost is True`) or `cost_limit` set\n    low enough, there will be unmatched rows, columns in the solution `x`, `y`.\n    All such entries are set to -1.\n    ");
+static PyMethodDef __pyx_mdef_6_lapjv_1lapjv = {"lapjv", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6_lapjv_1lapjv, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6_lapjv_lapjv};
+static PyObject *__pyx_pw_6_lapjv_1lapjv(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_cost = 0;
   char __pyx_v_extend_cost;
   double __pyx_v_cost_limit;
   char __pyx_v_return_cost;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lapjv (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cost,&__pyx_n_s_extend_cost,&__pyx_n_s_cost_limit,&__pyx_n_s_return_cost,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cost,&__pyx_n_s_extend_cost,&__pyx_n_s_cost_limit,&__pyx_n_s_return_cost,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cost)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cost)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_extend_cost);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extend_cost);
           if (value) { values[1] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cost_limit);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cost_limit);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_cost);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_cost);
           if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "lapjv") < 0)) __PYX_ERR(0, 43, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lapjv") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_cost = ((PyArrayObject *)values[0]);
     if (values[1]) {
       __pyx_v_extend_cost = __Pyx_PyInt_As_char(values[1]); if (unlikely((__pyx_v_extend_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
     } else {
-      __pyx_v_extend_cost = ((char)0);
+      __pyx_v_extend_cost = ((char)((int)0));
     }
     if (values[2]) {
       __pyx_v_cost_limit = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_cost_limit == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
     } else {
-      __pyx_v_cost_limit = __pyx_k_;
+      __pyx_v_cost_limit = __pyx_dynamic_args->__pyx_arg_cost_limit;
     }
     if (values[3]) {
       __pyx_v_return_cost = __Pyx_PyInt_As_char(values[3]); if (unlikely((__pyx_v_return_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
     } else {
-
-      /* "_lapjv.pyx":44
- * @cython.wraparound(False)
- * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
- *           double cost_limit=np.inf, char return_cost=True):             # <<<<<<<<<<<<<<
- *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
- * 
- */
-      __pyx_v_return_cost = ((char)1);
+      __pyx_v_return_cost = ((char)((int)1));
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lapjv", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 43, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lapjv", 0, 1, 4, __pyx_nargs); __PYX_ERR(0, 41, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_lapjv.lapjv", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cost), __pyx_ptype_5numpy_ndarray, 0, "cost", 0))) __PYX_ERR(0, 43, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_lapjv_lapjv(__pyx_self, __pyx_v_cost, __pyx_v_extend_cost, __pyx_v_cost_limit, __pyx_v_return_cost);
 
-  /* "_lapjv.pyx":43
- * @cython.boundscheck(False)
- * @cython.wraparound(False)
- * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
- *           double cost_limit=np.inf, char return_cost=True):
- *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
- */
-
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -2197,33 +4641,34 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_x_c;
   __Pyx_Buffer __pyx_pybuffer_x_c;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_y_c;
   __Pyx_Buffer __pyx_pybuffer_y_c;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  PyArrayObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyArrayObject *__pyx_t_8 = NULL;
+  npy_intp *__pyx_t_9;
   int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
+  PyArrayObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  uint_t __pyx_t_14;
+  PyObject *__pyx_t_14 = NULL;
   uint_t __pyx_t_15;
-  Py_ssize_t __pyx_t_16;
+  uint_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
-  PyArrayObject *__pyx_t_18 = NULL;
+  Py_ssize_t __pyx_t_18;
   PyArrayObject *__pyx_t_19 = NULL;
-  double __pyx_t_20;
+  PyArrayObject *__pyx_t_20 = NULL;
+  double __pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lapjv", 0);
   __pyx_pybuffer_cost_c.pybuffer.buf = NULL;
   __pyx_pybuffer_cost_c.refcount = 0;
   __pyx_pybuffernd_cost_c.data = NULL;
@@ -2244,28 +4689,29 @@
   /* "_lapjv.pyx":74
  *     All such entries are set to -1.
  *     """
  *     if cost.ndim != 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('2-dimensional array expected')
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  */
-  __pyx_t_1 = ((__pyx_v_cost->nd != 2) != 0);
-  if (unlikely(__pyx_t_1)) {
+  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_cost); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 != 2);
+  if (unlikely(__pyx_t_2)) {
 
     /* "_lapjv.pyx":75
  *     """
  *     if cost.ndim != 2:
  *         raise ValueError('2-dimensional array expected')             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 75, __pyx_L1_error)
 
     /* "_lapjv.pyx":74
  *     All such entries are set to -1.
  *     """
  *     if cost.ndim != 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('2-dimensional array expected')
@@ -2276,69 +4722,71 @@
   /* "_lapjv.pyx":77
  *         raise ValueError('2-dimensional array expected')
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(((PyObject *)__pyx_v_cost));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_cost));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_cost));
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF((PyObject *)__pyx_v_cost);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_cost);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_cost));
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_double); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_8 = ((PyArrayObject *)__pyx_t_7);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_cost_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 76, __pyx_L1_error)
     } else {__pyx_pybuffernd_cost_c.diminfo[0].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c.diminfo[0].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c.diminfo[1].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c.diminfo[1].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[1];
     }
   }
+  __pyx_t_8 = 0;
+  __pyx_v_cost_c = ((PyArrayObject *)__pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_v_cost_c = ((PyArrayObject *)__pyx_t_6);
-  __pyx_t_6 = 0;
 
   /* "_lapjv.pyx":79
  *         np.ascontiguousarray(cost, dtype=np.double)
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]             # <<<<<<<<<<<<<<
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0
  */
-  __pyx_v_n_rows = (__pyx_v_cost_c->dimensions[0]);
+  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_v_n_rows = (__pyx_t_9[0]);
 
   /* "_lapjv.pyx":80
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]
  *     cdef uint_t n_cols = cost_c.shape[1]             # <<<<<<<<<<<<<<
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:
  */
-  __pyx_v_n_cols = (__pyx_v_cost_c->dimensions[1]);
+  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_v_n_cols = (__pyx_t_9[1]);
 
   /* "_lapjv.pyx":81
  *     cdef uint_t n_rows = cost_c.shape[0]
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0             # <<<<<<<<<<<<<<
  *     if n_rows == n_cols:
  *         n = n_rows
@@ -2348,16 +4796,16 @@
   /* "_lapjv.pyx":82
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:             # <<<<<<<<<<<<<<
  *         n = n_rows
  *     else:
  */
-  __pyx_t_1 = ((__pyx_v_n_rows == __pyx_v_n_cols) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_n_rows == __pyx_v_n_cols);
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":83
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:
  *         n = n_rows             # <<<<<<<<<<<<<<
  *     else:
  *         if not extend_cost:
@@ -2378,28 +4826,28 @@
  *         n = n_rows
  *     else:
  *         if not extend_cost:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                     'Square cost array expected. If cost is intentionally '
  */
   /*else*/ {
-    __pyx_t_1 = ((!(__pyx_v_extend_cost != 0)) != 0);
-    if (unlikely(__pyx_t_1)) {
+    __pyx_t_2 = (!(__pyx_v_extend_cost != 0));
+    if (unlikely(__pyx_t_2)) {
 
       /* "_lapjv.pyx":86
  *     else:
  *         if not extend_cost:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_Raise(__pyx_t_6, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_Raise(__pyx_t_7, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __PYX_ERR(0, 86, __pyx_L1_error)
 
       /* "_lapjv.pyx":85
  *         n = n_rows
  *     else:
  *         if not extend_cost:             # <<<<<<<<<<<<<<
  *             raise ValueError(
@@ -2412,35 +4860,35 @@
   /* "_lapjv.pyx":89
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  *     if extend_cost or cost_limit < np.inf:             # <<<<<<<<<<<<<<
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  */
-  __pyx_t_8 = (__pyx_v_extend_cost != 0);
-  if (!__pyx_t_8) {
+  __pyx_t_10 = (__pyx_v_extend_cost != 0);
+  if (!__pyx_t_10) {
   } else {
-    __pyx_t_1 = __pyx_t_8;
+    __pyx_t_2 = __pyx_t_10;
     goto __pyx_L7_bool_binop_done;
   }
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_1 = __pyx_t_8;
+  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_inf); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_7, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_2 = __pyx_t_10;
   __pyx_L7_bool_binop_done:;
-  if (__pyx_t_1) {
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":90
  *                     'non-square, pass extend_cost=True.')
  *     if extend_cost or cost_limit < np.inf:
  *         n = n_rows + n_cols             # <<<<<<<<<<<<<<
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  *         if cost_limit < np.inf:
@@ -2450,105 +4898,105 @@
     /* "_lapjv.pyx":91
  *     if extend_cost or cost_limit < np.inf:
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)             # <<<<<<<<<<<<<<
  *         if cost_limit < np.inf:
  *             cost_c_extended[:] = cost_limit / 2.
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
+    __pyx_t_5 = 0;
+    __pyx_t_7 = 0;
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 91, __pyx_L1_error)
-    __pyx_t_9 = ((PyArrayObject *)__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_11 = ((PyArrayObject *)__pyx_t_6);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer);
-      __pyx_t_10 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
-      if (unlikely(__pyx_t_10 < 0)) {
-        PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c_extended, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13);
+          Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
+          PyErr_Restore(__pyx_t_12, __pyx_t_13, __pyx_t_14);
         }
-        __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
+        __pyx_t_12 = __pyx_t_13 = __pyx_t_14 = 0;
       }
       __pyx_pybuffernd_cost_c_extended.diminfo[0].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c_extended.diminfo[0].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c_extended.diminfo[1].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c_extended.diminfo[1].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[1];
-      if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 91, __pyx_L1_error)
     }
-    __pyx_t_9 = 0;
-    __pyx_v_cost_c_extended = ((PyArrayObject *)__pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_11 = 0;
+    __pyx_v_cost_c_extended = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_6 = 0;
 
     /* "_lapjv.pyx":92
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  *         if cost_limit < np.inf:             # <<<<<<<<<<<<<<
  *             cost_c_extended[:] = cost_limit / 2.
  *         else:
  */
-    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_inf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_7, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__pyx_t_1) {
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (__pyx_t_2) {
 
       /* "_lapjv.pyx":93
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  *         if cost_limit < np.inf:
  *             cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
  *         else:
  *             cost_c_extended[:] = cost_c.max() + 1
  */
-      __pyx_t_3 = PyFloat_FromDouble((__pyx_v_cost_limit / 2.)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__4, __pyx_t_3) < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_4 = PyFloat_FromDouble((__pyx_v_cost_limit / 2.)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__5, __pyx_t_4) < 0))) __PYX_ERR(0, 93, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "_lapjv.pyx":92
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  *         if cost_limit < np.inf:             # <<<<<<<<<<<<<<
  *             cost_c_extended[:] = cost_limit / 2.
  *         else:
@@ -2560,120 +5008,125 @@
  *             cost_c_extended[:] = cost_limit / 2.
  *         else:
  *             cost_c_extended[:] = cost_c.max() + 1             # <<<<<<<<<<<<<<
  *         cost_c_extended[n_rows:, n_cols:] = 0
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
  */
     /*else*/ {
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cost_c), __pyx_n_s_max); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cost_c), __pyx_n_s_max); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_6 = NULL;
+      __pyx_t_1 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __Pyx_DECREF_SET(__pyx_t_7, function);
+          __pyx_t_1 = 1;
         }
       }
-      __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__4, __pyx_t_6) < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      {
+        PyObject *__pyx_callargs[1] = {__pyx_t_6, };
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      }
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__5, __pyx_t_7) < 0))) __PYX_ERR(0, 95, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __pyx_L9:;
 
     /* "_lapjv.pyx":96
  *         else:
  *             cost_c_extended[:] = cost_c.max() + 1
  *         cost_c_extended[n_rows:, n_cols:] = 0             # <<<<<<<<<<<<<<
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
  *         cost_c = cost_c_extended
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PySlice_New(__pyx_t_6, Py_None, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PySlice_New(__pyx_t_6, Py_None, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_4 = PySlice_New(__pyx_t_7, Py_None, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_6 = PySlice_New(__pyx_t_7, Py_None, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
-    __pyx_t_3 = 0;
-    __pyx_t_5 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_6, __pyx_int_0) < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6);
+    __pyx_t_4 = 0;
+    __pyx_t_6 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_7, __pyx_int_0) < 0))) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "_lapjv.pyx":97
  *             cost_c_extended[:] = cost_c.max() + 1
  *         cost_c_extended[n_rows:, n_cols:] = 0
  *         cost_c_extended[:n_rows, :n_cols] = cost_c             # <<<<<<<<<<<<<<
  *         cost_c = cost_c_extended
  * 
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
-    __pyx_t_5 = 0;
-    __pyx_t_3 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_6, ((PyObject *)__pyx_v_cost_c)) < 0)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_4 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4);
+    __pyx_t_6 = 0;
+    __pyx_t_4 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_7, ((PyObject *)__pyx_v_cost_c)) < 0))) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "_lapjv.pyx":98
  *         cost_c_extended[n_rows:, n_cols:] = 0
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
  *         cost_c = cost_c_extended             # <<<<<<<<<<<<<<
  * 
  *     cdef double **cost_ptr
  */
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer);
-      __pyx_t_10 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_v_cost_c_extended), &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
-      if (unlikely(__pyx_t_10 < 0)) {
-        PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_v_cost_c_extended), &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_14, &__pyx_t_13, &__pyx_t_12);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11);
+          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
+          PyErr_Restore(__pyx_t_14, __pyx_t_13, __pyx_t_12);
         }
-        __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
+        __pyx_t_14 = __pyx_t_13 = __pyx_t_12 = 0;
       }
       __pyx_pybuffernd_cost_c.diminfo[0].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c.diminfo[0].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c.diminfo[1].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c.diminfo[1].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[1];
-      if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 98, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 98, __pyx_L1_error)
     }
-    __Pyx_INCREF(((PyObject *)__pyx_v_cost_c_extended));
+    __Pyx_INCREF((PyObject *)__pyx_v_cost_c_extended);
     __Pyx_DECREF_SET(__pyx_v_cost_c, ((PyArrayObject *)__pyx_v_cost_c_extended));
 
     /* "_lapjv.pyx":89
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  *     if extend_cost or cost_limit < np.inf:             # <<<<<<<<<<<<<<
  *         n = n_rows + n_cols
@@ -2693,145 +5146,145 @@
   /* "_lapjv.pyx":103
  *     cost_ptr = <double **> malloc(n * sizeof(double *))
  *     cdef int i
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         cost_ptr[i] = &cost_c[i, 0]
  * 
  */
-  __pyx_t_14 = __pyx_v_n;
-  __pyx_t_15 = __pyx_t_14;
-  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_15; __pyx_t_10+=1) {
-    __pyx_v_i = __pyx_t_10;
+  __pyx_t_15 = __pyx_v_n;
+  __pyx_t_16 = __pyx_t_15;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_16; __pyx_t_1+=1) {
+    __pyx_v_i = __pyx_t_1;
 
     /* "_lapjv.pyx":104
  *     cdef int i
  *     for i in range(n):
  *         cost_ptr[i] = &cost_c[i, 0]             # <<<<<<<<<<<<<<
  * 
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  */
-    __pyx_t_16 = __pyx_v_i;
-    __pyx_t_17 = 0;
-    (__pyx_v_cost_ptr[__pyx_v_i]) = (&(*__Pyx_BufPtrCContig2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_cost_c.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_cost_c.diminfo[1].strides)));
+    __pyx_t_17 = __pyx_v_i;
+    __pyx_t_18 = 0;
+    (__pyx_v_cost_ptr[__pyx_v_i]) = (&(*__Pyx_BufPtrCContig2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_cost_c.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_cost_c.diminfo[1].strides)));
   }
 
   /* "_lapjv.pyx":107
  * 
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_18 = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_19 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_x_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 106, __pyx_L1_error)
     } else {__pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_18 = 0;
-  __pyx_v_x_c = ((PyArrayObject *)__pyx_t_4);
-  __pyx_t_4 = 0;
+  __pyx_t_19 = 0;
+  __pyx_v_x_c = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_5 = 0;
 
   /* "_lapjv.pyx":109
  *         np.empty((n,), dtype=np.int32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
-  __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
-  __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_t_19 = ((PyArrayObject *)__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_20 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_y_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 108, __pyx_L1_error)
     } else {__pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_19 = 0;
-  __pyx_v_y_c = ((PyArrayObject *)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_t_20 = 0;
+  __pyx_v_y_c = ((PyArrayObject *)__pyx_t_3);
+  __pyx_t_3 = 0;
 
   /* "_lapjv.pyx":111
  *         np.empty((n,), dtype=np.int32)
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])             # <<<<<<<<<<<<<<
  *     free(cost_ptr)
  *     if ret != 0:
  */
+  __pyx_t_18 = 0;
   __pyx_t_17 = 0;
-  __pyx_t_16 = 0;
-  __pyx_v_ret = lapjv_internal(__pyx_v_n, __pyx_v_cost_ptr, (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_x_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_y_c.diminfo[0].strides))));
+  __pyx_v_ret = lapjv_internal(__pyx_v_n, __pyx_v_cost_ptr, (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_x_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_y_c.diminfo[0].strides))));
 
   /* "_lapjv.pyx":112
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)             # <<<<<<<<<<<<<<
  *     if ret != 0:
  *         if ret == -1:
@@ -2841,38 +5294,38 @@
   /* "_lapjv.pyx":113
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
-  __pyx_t_1 = ((__pyx_v_ret != 0) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_ret != 0);
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":114
  *     free(cost_ptr)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  */
-    __pyx_t_1 = ((__pyx_v_ret == -1L) != 0);
-    if (unlikely(__pyx_t_1)) {
+    __pyx_t_2 = (__pyx_v_ret == -1L);
+    if (unlikely(__pyx_t_2)) {
 
       /* "_lapjv.pyx":115
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  * 
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(0, 115, __pyx_L1_error)
 
       /* "_lapjv.pyx":114
  *     free(cost_ptr)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
@@ -2883,24 +5336,24 @@
     /* "_lapjv.pyx":116
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 116, __pyx_L1_error)
 
     /* "_lapjv.pyx":113
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
@@ -2911,215 +5364,225 @@
   /* "_lapjv.pyx":119
  * 
  * 
  *     cdef double opt = np.nan             # <<<<<<<<<<<<<<
  *     if n != n_rows:
  *         x_c[x_c >= n_cols] = -1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_nan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_20 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_20 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_opt = __pyx_t_20;
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_v_opt = __pyx_t_21;
 
   /* "_lapjv.pyx":120
  * 
  *     cdef double opt = np.nan
  *     if n != n_rows:             # <<<<<<<<<<<<<<
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  */
-  __pyx_t_1 = ((__pyx_v_n != __pyx_v_n_rows) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_n != __pyx_v_n_rows);
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":121
  *     cdef double opt = np.nan
  *     if n != n_rows:
  *         x_c[x_c >= n_cols] = -1             # <<<<<<<<<<<<<<
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_2, __pyx_int_neg_1) < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "_lapjv.pyx":122
  *     if n != n_rows:
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1             # <<<<<<<<<<<<<<
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  */
-    __pyx_t_2 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_6, __pyx_int_neg_1) < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_7, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "_lapjv.pyx":123
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]             # <<<<<<<<<<<<<<
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
-    __pyx_t_18 = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_19 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer);
-      __pyx_t_10 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_10 < 0)) {
-        PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_c, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13);
+          Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
+          PyErr_Restore(__pyx_t_12, __pyx_t_13, __pyx_t_14);
         }
-        __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
+        __pyx_t_12 = __pyx_t_13 = __pyx_t_14 = 0;
       }
       __pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
     }
-    __pyx_t_18 = 0;
-    __Pyx_DECREF_SET(__pyx_v_x_c, ((PyArrayObject *)__pyx_t_6));
-    __pyx_t_6 = 0;
+    __pyx_t_19 = 0;
+    __Pyx_DECREF_SET(__pyx_v_x_c, ((PyArrayObject *)__pyx_t_7));
+    __pyx_t_7 = 0;
 
     /* "_lapjv.pyx":124
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]             # <<<<<<<<<<<<<<
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 124, __pyx_L1_error)
-    __pyx_t_19 = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_20 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer);
-      __pyx_t_10 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_10 < 0)) {
-        PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_14, &__pyx_t_13, &__pyx_t_12);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_c, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11);
+          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
+          PyErr_Restore(__pyx_t_14, __pyx_t_13, __pyx_t_12);
         }
-        __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
+        __pyx_t_14 = __pyx_t_13 = __pyx_t_12 = 0;
       }
       __pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
     }
-    __pyx_t_19 = 0;
-    __Pyx_DECREF_SET(__pyx_v_y_c, ((PyArrayObject *)__pyx_t_6));
-    __pyx_t_6 = 0;
+    __pyx_t_20 = 0;
+    __Pyx_DECREF_SET(__pyx_v_y_c, ((PyArrayObject *)__pyx_t_7));
+    __pyx_t_7 = 0;
 
     /* "_lapjv.pyx":125
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  */
-    __pyx_t_1 = (__pyx_v_return_cost != 0);
-    if (__pyx_t_1) {
+    __pyx_t_2 = (__pyx_v_return_cost != 0);
+    if (__pyx_t_2) {
 
       /* "_lapjv.pyx":126
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()             # <<<<<<<<<<<<<<
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __pyx_t_3 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-        if (likely(__pyx_t_3)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-          __Pyx_INCREF(__pyx_t_3);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __pyx_t_4 = NULL;
+      __pyx_t_1 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_1 = 1;
         }
       }
-      __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_2, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
+        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_3, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_GIVEREF(__pyx_t_6);
+      PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5);
+      __pyx_t_6 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_4);
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_1 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_1 = 1;
         }
       }
-      __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_20 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_20 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_v_opt = __pyx_t_20;
+      {
+        PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 126, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
+      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_v_opt = __pyx_t_21;
 
       /* "_lapjv.pyx":125
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
@@ -3139,79 +5602,89 @@
   /* "_lapjv.pyx":127
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  */
-  __pyx_t_1 = (__pyx_v_return_cost != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_return_cost != 0);
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":128
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()             # <<<<<<<<<<<<<<
  * 
  *     if return_cost:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
-    __Pyx_INCREF(((PyObject *)__pyx_v_x_c));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_x_c));
-    PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_x_c));
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_4 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_1 = 1;
       }
     }
-    __pyx_t_6 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_20 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_20 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
+    __Pyx_INCREF((PyObject *)__pyx_v_x_c);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_x_c));
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_opt = __pyx_t_20;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_3, };
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_v_opt = __pyx_t_21;
 
     /* "_lapjv.pyx":127
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
@@ -3222,40 +5695,40 @@
   /* "_lapjv.pyx":130
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
  *     else:
  */
-  __pyx_t_1 = (__pyx_v_return_cost != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_return_cost != 0);
+  if (__pyx_t_2) {
 
     /* "_lapjv.pyx":131
  * 
  *     if return_cost:
  *         return opt, x_c, y_c             # <<<<<<<<<<<<<<
  *     else:
  *         return x_c, y_c
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
-    __Pyx_INCREF(((PyObject *)__pyx_v_x_c));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_x_c));
-    PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_x_c));
-    __Pyx_INCREF(((PyObject *)__pyx_v_y_c));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_y_c));
-    PyTuple_SET_ITEM(__pyx_t_5, 2, ((PyObject *)__pyx_v_y_c));
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
+    __Pyx_INCREF((PyObject *)__pyx_v_x_c);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_x_c));
+    __Pyx_INCREF((PyObject *)__pyx_v_y_c);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
+    PyTuple_SET_ITEM(__pyx_t_6, 2, ((PyObject *)__pyx_v_y_c));
+    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
     goto __pyx_L0;
 
     /* "_lapjv.pyx":130
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
@@ -3268,42 +5741,42 @@
  *     else:
  *         return x_c, y_c             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_INCREF(((PyObject *)__pyx_v_x_c));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_x_c));
-    PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_x_c));
-    __Pyx_INCREF(((PyObject *)__pyx_v_y_c));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_y_c));
-    PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_y_c));
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_INCREF((PyObject *)__pyx_v_x_c);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_v_x_c));
+    __Pyx_INCREF((PyObject *)__pyx_v_y_c);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_y_c));
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
-  /* "_lapjv.pyx":43
- * @cython.boundscheck(False)
+  /* "_lapjv.pyx":41
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
- *           double cost_limit=np.inf, char return_cost=True):
- *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer);
@@ -3323,116 +5796,179 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_x_c);
   __Pyx_XDECREF((PyObject *)__pyx_v_y_c);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_lapjv.pyx":138
- * @cython.boundscheck(False)
+/* "_lapjv.pyx":136
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(             # <<<<<<<<<<<<<<
- *         const uint_t n,
- *         cnp.ndarray cc not None,
+ * def _lapmod(
  */
 
+static PyObject *__pyx_pf_6_lapjv_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_fp_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None);
+  __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("_lapjv.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* Python wrapper */
-static PyObject *__pyx_pw_6_lapjv_3_lapmod(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6_lapjv_2_lapmod[] = "Internal function called from lapmod(..., fast=True).";
-static PyMethodDef __pyx_mdef_6_lapjv_3_lapmod = {"_lapmod", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6_lapjv_3_lapmod, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6_lapjv_2_lapmod};
-static PyObject *__pyx_pw_6_lapjv_3_lapmod(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6_lapjv_3_lapmod(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6_lapjv_2_lapmod, "Internal function called from lapmod(..., fast=True).");
+static PyMethodDef __pyx_mdef_6_lapjv_3_lapmod = {"_lapmod", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6_lapjv_3_lapmod, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6_lapjv_2_lapmod};
+static PyObject *__pyx_pw_6_lapjv_3_lapmod(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   uint_t __pyx_v_n;
   PyArrayObject *__pyx_v_cc = 0;
   PyArrayObject *__pyx_v_ii = 0;
   PyArrayObject *__pyx_v_kk = 0;
   enum fp_t __pyx_v_fp_version;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_lapmod (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_n,&__pyx_n_s_cc,&__pyx_n_s_ii,&__pyx_n_s_kk,&__pyx_n_s_fp_version,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_n,&__pyx_n_s_cc,&__pyx_n_s_ii,&__pyx_n_s_kk,&__pyx_n_s_fp_version,0};
     PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cc)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cc)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 138, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 136, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ii)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ii)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 138, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 136, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kk)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kk)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 138, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 136, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fp_version);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fp_version);
           if (value) { values[4] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_lapmod") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lapmod") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_n = __Pyx_PyInt_As_uint_t(values[0]); if (unlikely((__pyx_v_n == ((uint_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_cc = ((PyArrayObject *)values[1]);
     __pyx_v_ii = ((PyArrayObject *)values[2]);
     __pyx_v_kk = ((PyArrayObject *)values[3]);
     if (values[4]) {
       __pyx_v_fp_version = ((enum fp_t)__Pyx_PyInt_As_enum__fp_t(values[4])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L3_error)
     } else {
-      __pyx_v_fp_version = __pyx_k__6;
+      __pyx_v_fp_version = __pyx_dynamic_args->__pyx_arg_fp_version;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 138, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 136, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_lapjv._lapmod", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cc), __pyx_ptype_5numpy_ndarray, 0, "cc", 0))) __PYX_ERR(0, 140, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ii), __pyx_ptype_5numpy_ndarray, 0, "ii", 0))) __PYX_ERR(0, 141, __pyx_L1_error)
@@ -3518,16 +6054,16 @@
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(((PyObject *)__pyx_v_cc));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_cc));
+  __Pyx_INCREF((PyObject *)__pyx_v_cc);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_cc);
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_cc));
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -3563,16 +6099,16 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_INCREF(((PyObject *)__pyx_v_ii));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_ii));
+  __Pyx_INCREF((PyObject *)__pyx_v_ii);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_ii);
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_ii));
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -3608,16 +6144,16 @@
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_INCREF(((PyObject *)__pyx_v_kk));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_kk));
+  __Pyx_INCREF((PyObject *)__pyx_v_kk);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_kk);
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_kk));
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -3780,35 +6316,35 @@
   /* "_lapjv.pyx":159
  *                 n, &cc_c[0], &ii_c[0], &kk_c[0],
  *                 &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
-  __pyx_t_16 = ((__pyx_v_ret != 0) != 0);
+  __pyx_t_16 = (__pyx_v_ret != 0);
   if (__pyx_t_16) {
 
     /* "_lapjv.pyx":160
  *                 &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  */
-    __pyx_t_16 = ((__pyx_v_ret == -1L) != 0);
+    __pyx_t_16 = (__pyx_v_ret == -1L);
     if (unlikely(__pyx_t_16)) {
 
       /* "_lapjv.pyx":161
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __PYX_ERR(0, 161, __pyx_L1_error)
 
       /* "_lapjv.pyx":160
  *                 &x_c[0], &y_c[0], fp_version)
@@ -3851,30 +6387,30 @@
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  *     return x_c, y_c             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(((PyObject *)__pyx_v_x_c));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_x_c));
+  __Pyx_INCREF((PyObject *)__pyx_v_x_c);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_x_c));
-  __Pyx_INCREF(((PyObject *)__pyx_v_y_c));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_y_c));
+  __Pyx_INCREF((PyObject *)__pyx_v_y_c);
+  __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
   PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_y_c));
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_lapjv.pyx":138
- * @cython.boundscheck(False)
+  /* "_lapjv.pyx":136
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(             # <<<<<<<<<<<<<<
- *         const uint_t n,
- *         cnp.ndarray cc not None,
+ * def _lapmod(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -3906,1268 +6442,252 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_x_c);
   __Pyx_XDECREF((PyObject *)__pyx_v_y_c);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":731
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":732
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":731
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":734
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":735
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":734
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":738
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":741
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":744
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":747
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":748
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
- *     else:
- *         return ()
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":747
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":750
- *         return <tuple>d.subarray.shape
- *     else:
- *         return ()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
-    goto __pyx_L0;
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":925
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":926
- * 
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
- *     PyArray_SetBaseObject(arr, base)
- * 
- */
-  Py_INCREF(__pyx_v_base);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":927
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object get_array_base(ndarray arr):
- */
-  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":925
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":929
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
-  PyObject *__pyx_v_base;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":930
- * 
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
- *     if base is NULL:
- *         return None
- */
-  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":931
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":932
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- *         return None             # <<<<<<<<<<<<<<
- *     return <object>base
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":931
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":933
- *     if base is NULL:
- *         return None
- *     return <object>base             # <<<<<<<<<<<<<<
- * 
- * # Versions of the import_* functions which are more suitable for
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_base));
-  __pyx_r = ((PyObject *)__pyx_v_base);
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":929
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":937
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":938
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":939
- * cdef inline int import_array() except -1:
- *     try:
- *         __pyx_import_array()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
- */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":938
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":940
- *     try:
- *         __pyx_import_array()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":941
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_umath() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 941, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":938
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":937
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":943
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":944
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":945
- * cdef inline int import_umath() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":944
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":946
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":947
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_ufunc() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 947, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":944
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":943
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":949
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":950
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":951
- * cdef inline int import_ufunc() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":950
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":952
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":953
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef extern from *:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 953, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":950
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":949
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":963
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":975
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":963
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":978
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":990
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":978
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":993
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1000
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":993
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1003
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1007
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1003
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1010
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1014
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1010
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__lapjv(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__lapjv},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "_lapjv",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_2_dimensional_array_expected, __pyx_k_2_dimensional_array_expected, sizeof(__pyx_k_2_dimensional_array_expected), 0, 1, 0, 0},
-  {&__pyx_n_s_FP_1, __pyx_k_FP_1, sizeof(__pyx_k_FP_1), 0, 0, 1, 1},
-  {&__pyx_n_s_FP_2, __pyx_k_FP_2, sizeof(__pyx_k_FP_2), 0, 0, 1, 1},
-  {&__pyx_n_s_FP_DYNAMIC, __pyx_k_FP_DYNAMIC, sizeof(__pyx_k_FP_DYNAMIC), 0, 0, 1, 1},
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_LARGE, __pyx_k_LARGE, sizeof(__pyx_k_LARGE), 0, 0, 1, 1},
-  {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Out_of_memory, __pyx_k_Out_of_memory, sizeof(__pyx_k_Out_of_memory), 0, 1, 0, 0},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Square_cost_array_expected_If_co, __pyx_k_Square_cost_array_expected_If_co, sizeof(__pyx_k_Square_cost_array_expected_If_co), 0, 1, 0, 0},
-  {&__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_k_Unknown_error_lapjv_internal_ret, sizeof(__pyx_k_Unknown_error_lapjv_internal_ret), 0, 1, 0, 0},
-  {&__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_k_Unknown_error_lapmod_internal_re, sizeof(__pyx_k_Unknown_error_lapmod_internal_re), 0, 1, 0, 0},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
-  {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
-  {&__pyx_n_s_cc, __pyx_k_cc, sizeof(__pyx_k_cc), 0, 0, 1, 1},
-  {&__pyx_n_s_cc_c, __pyx_k_cc_c, sizeof(__pyx_k_cc_c), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_cost, __pyx_k_cost, sizeof(__pyx_k_cost), 0, 0, 1, 1},
-  {&__pyx_n_s_cost_c, __pyx_k_cost_c, sizeof(__pyx_k_cost_c), 0, 0, 1, 1},
-  {&__pyx_n_s_cost_c_extended, __pyx_k_cost_c_extended, sizeof(__pyx_k_cost_c_extended), 0, 0, 1, 1},
-  {&__pyx_n_s_cost_limit, __pyx_k_cost_limit, sizeof(__pyx_k_cost_limit), 0, 0, 1, 1},
-  {&__pyx_n_s_cost_ptr, __pyx_k_cost_ptr, sizeof(__pyx_k_cost_ptr), 0, 0, 1, 1},
-  {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
-  {&__pyx_n_s_extend_cost, __pyx_k_extend_cost, sizeof(__pyx_k_extend_cost), 0, 0, 1, 1},
-  {&__pyx_n_s_fp_version, __pyx_k_fp_version, sizeof(__pyx_k_fp_version), 0, 0, 1, 1},
-  {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
-  {&__pyx_n_s_ii, __pyx_k_ii, sizeof(__pyx_k_ii), 0, 0, 1, 1},
-  {&__pyx_n_s_ii_c, __pyx_k_ii_c, sizeof(__pyx_k_ii_c), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
-  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
-  {&__pyx_n_s_kk, __pyx_k_kk, sizeof(__pyx_k_kk), 0, 0, 1, 1},
-  {&__pyx_n_s_kk_c, __pyx_k_kk_c, sizeof(__pyx_k_kk_c), 0, 0, 1, 1},
-  {&__pyx_n_s_lapjv, __pyx_k_lapjv, sizeof(__pyx_k_lapjv), 0, 0, 1, 1},
-  {&__pyx_n_s_lapjv_2, __pyx_k_lapjv_2, sizeof(__pyx_k_lapjv_2), 0, 0, 1, 1},
-  {&__pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_k_lapjv_src__lapjv_pyx, sizeof(__pyx_k_lapjv_src__lapjv_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_lapmod, __pyx_k_lapmod, sizeof(__pyx_k_lapmod), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
-  {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
-  {&__pyx_n_s_n_cols, __pyx_k_n_cols, sizeof(__pyx_k_n_cols), 0, 0, 1, 1},
-  {&__pyx_n_s_n_rows, __pyx_k_n_rows, sizeof(__pyx_k_n_rows), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
-  {&__pyx_n_s_nonzero, __pyx_k_nonzero, sizeof(__pyx_k_nonzero), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
-  {&__pyx_n_s_opt, __pyx_k_opt, sizeof(__pyx_k_opt), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_s_ret, __pyx_k_ret, sizeof(__pyx_k_ret), 0, 0, 1, 1},
-  {&__pyx_n_s_return_cost, __pyx_k_return_cost, sizeof(__pyx_k_return_cost), 0, 0, 1, 1},
-  {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
-  {&__pyx_n_s_x_c, __pyx_k_x_c, sizeof(__pyx_k_x_c), 0, 0, 1, 1},
-  {&__pyx_n_s_y_c, __pyx_k_y_c, sizeof(__pyx_k_y_c), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_u_2_dimensional_array_expected, __pyx_k_2_dimensional_array_expected, sizeof(__pyx_k_2_dimensional_array_expected), 0, 1, 0, 0},
+    {&__pyx_n_s_FP_1, __pyx_k_FP_1, sizeof(__pyx_k_FP_1), 0, 0, 1, 1},
+    {&__pyx_n_s_FP_2, __pyx_k_FP_2, sizeof(__pyx_k_FP_2), 0, 0, 1, 1},
+    {&__pyx_n_s_FP_DYNAMIC, __pyx_k_FP_DYNAMIC, sizeof(__pyx_k_FP_DYNAMIC), 0, 0, 1, 1},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_LARGE, __pyx_k_LARGE, sizeof(__pyx_k_LARGE), 0, 0, 1, 1},
+    {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_kp_u_Out_of_memory, __pyx_k_Out_of_memory, sizeof(__pyx_k_Out_of_memory), 0, 1, 0, 0},
+    {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+    {&__pyx_kp_u_Square_cost_array_expected_If_co, __pyx_k_Square_cost_array_expected_If_co, sizeof(__pyx_k_Square_cost_array_expected_If_co), 0, 1, 0, 0},
+    {&__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_k_Unknown_error_lapjv_internal_ret, sizeof(__pyx_k_Unknown_error_lapjv_internal_ret), 0, 1, 0, 0},
+    {&__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_k_Unknown_error_lapmod_internal_re, sizeof(__pyx_k_Unknown_error_lapmod_internal_re), 0, 1, 0, 0},
+    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 1, 1},
+    {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
+    {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
+    {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_cc, __pyx_k_cc, sizeof(__pyx_k_cc), 0, 0, 1, 1},
+    {&__pyx_n_s_cc_c, __pyx_k_cc_c, sizeof(__pyx_k_cc_c), 0, 0, 1, 1},
+    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_cost, __pyx_k_cost, sizeof(__pyx_k_cost), 0, 0, 1, 1},
+    {&__pyx_n_s_cost_c, __pyx_k_cost_c, sizeof(__pyx_k_cost_c), 0, 0, 1, 1},
+    {&__pyx_n_s_cost_c_extended, __pyx_k_cost_c_extended, sizeof(__pyx_k_cost_c_extended), 0, 0, 1, 1},
+    {&__pyx_n_s_cost_limit, __pyx_k_cost_limit, sizeof(__pyx_k_cost_limit), 0, 0, 1, 1},
+    {&__pyx_n_s_cost_ptr, __pyx_k_cost_ptr, sizeof(__pyx_k_cost_ptr), 0, 0, 1, 1},
+    {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
+    {&__pyx_n_s_extend_cost, __pyx_k_extend_cost, sizeof(__pyx_k_extend_cost), 0, 0, 1, 1},
+    {&__pyx_n_s_fp_version, __pyx_k_fp_version, sizeof(__pyx_k_fp_version), 0, 0, 1, 1},
+    {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
+    {&__pyx_n_s_ii, __pyx_k_ii, sizeof(__pyx_k_ii), 0, 0, 1, 1},
+    {&__pyx_n_s_ii_c, __pyx_k_ii_c, sizeof(__pyx_k_ii_c), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_n_s_kk, __pyx_k_kk, sizeof(__pyx_k_kk), 0, 0, 1, 1},
+    {&__pyx_n_s_kk_c, __pyx_k_kk_c, sizeof(__pyx_k_kk_c), 0, 0, 1, 1},
+    {&__pyx_n_s_lapjv, __pyx_k_lapjv, sizeof(__pyx_k_lapjv), 0, 0, 1, 1},
+    {&__pyx_n_s_lapjv_2, __pyx_k_lapjv_2, sizeof(__pyx_k_lapjv_2), 0, 0, 1, 1},
+    {&__pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_k_lapjv_src__lapjv_pyx, sizeof(__pyx_k_lapjv_src__lapjv_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_lapmod, __pyx_k_lapmod, sizeof(__pyx_k_lapmod), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
+    {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
+    {&__pyx_n_s_n_cols, __pyx_k_n_cols, sizeof(__pyx_k_n_cols), 0, 0, 1, 1},
+    {&__pyx_n_s_n_rows, __pyx_k_n_rows, sizeof(__pyx_k_n_rows), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
+    {&__pyx_n_s_nonzero, __pyx_k_nonzero, sizeof(__pyx_k_nonzero), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_n_s_opt, __pyx_k_opt, sizeof(__pyx_k_opt), 0, 0, 1, 1},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_ret, __pyx_k_ret, sizeof(__pyx_k_ret), 0, 0, 1, 1},
+    {&__pyx_n_s_return_cost, __pyx_k_return_cost, sizeof(__pyx_k_return_cost), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
+    {&__pyx_n_s_x_c, __pyx_k_x_c, sizeof(__pyx_k_x_c), 0, 0, 1, 1},
+    {&__pyx_n_s_y_c, __pyx_k_y_c, sizeof(__pyx_k_y_c), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 103, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 115, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 116, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 983, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 983, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+
+  /* "../../../../../tmp/build-env-w2y1er_9/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
   /* "_lapjv.pyx":75
  *     """
  *     if cost.ndim != 2:
  *         raise ValueError('2-dimensional array expected')             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_2_dimensional_array_expected); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_2_dimensional_array_expected); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "_lapjv.pyx":86
  *     else:
  *         if not extend_cost:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Square_cost_array_expected_If_co); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Square_cost_array_expected_If_co); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "_lapjv.pyx":93
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  *         if cost_limit < np.inf:
  *             cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
  *         else:
  *             cost_c_extended[:] = cost_c.max() + 1
  */
-  __pyx_slice__4 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__4)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__4);
-  __Pyx_GIVEREF(__pyx_slice__4);
+  __pyx_slice__5 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__5);
+  __Pyx_GIVEREF(__pyx_slice__5);
 
   /* "_lapjv.pyx":115
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Out_of_memory); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Out_of_memory); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":941
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+  /* "_lapjv.pyx":41
  * 
- * cdef inline int import_umath() except -1:
- */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 941, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":947
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
- * cdef inline int import_ufunc() except -1:
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 947, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(15, __pyx_n_s_cost, __pyx_n_s_extend_cost, __pyx_n_s_cost_limit, __pyx_n_s_return_cost, __pyx_n_s_cost_c, __pyx_n_s_cost_c_extended, __pyx_n_s_n_rows, __pyx_n_s_n_cols, __pyx_n_s_n, __pyx_n_s_cost_ptr, __pyx_n_s_i, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapjv, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 41, __pyx_L1_error)
 
-  /* "_lapjv.pyx":43
- * @cython.boundscheck(False)
+  /* "_lapjv.pyx":136
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
- *           double cost_limit=np.inf, char return_cost=True):
- *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
+ * def _lapmod(
  */
-  __pyx_tuple__9 = PyTuple_Pack(15, __pyx_n_s_cost, __pyx_n_s_extend_cost, __pyx_n_s_cost_limit, __pyx_n_s_return_cost, __pyx_n_s_cost_c, __pyx_n_s_cost_c_extended, __pyx_n_s_n_rows, __pyx_n_s_n_cols, __pyx_n_s_n, __pyx_n_s_cost_ptr, __pyx_n_s_i, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 43, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapjv, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 43, __pyx_L1_error)
-
-  /* "_lapjv.pyx":138
- * @cython.boundscheck(False)
- * @cython.wraparound(False)
- * def _lapmod(             # <<<<<<<<<<<<<<
- *         const uint_t n,
- *         cnp.ndarray cc not None,
- */
-  __pyx_tuple__11 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(5, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#if !NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -5211,39 +6731,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 865, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5262,14 +6784,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec__lapjv(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__lapjv},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "_lapjv",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -5312,42 +6883,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -5355,30 +6940,65 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__lapjv(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  double __pyx_t_3;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module '_lapjv' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("_lapjv", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _lapjv pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -5389,239 +7009,245 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_lapjv", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main__lapjv) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "_lapjv")) {
-      if (unlikely(PyDict_SetItemString(modules, "_lapjv", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "_lapjv", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "_lapjv.pyx":7
  * # cython: language_level=3
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as cnp
  * cimport cython
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":35
  *             fp_t fp_version)
  * 
  * LARGE_ = LARGE             # <<<<<<<<<<<<<<
  * FP_1_ = FP_1
  * FP_2_ = FP_2
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LARGE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LARGE, __pyx_t_1) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyInt_From_int(LARGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LARGE, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":36
  * 
  * LARGE_ = LARGE
  * FP_1_ = FP_1             # <<<<<<<<<<<<<<
  * FP_2_ = FP_2
  * FP_DYNAMIC_ = FP_DYNAMIC
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(FP_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_1, __pyx_t_1) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_1, __pyx_t_2) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":37
  * LARGE_ = LARGE
  * FP_1_ = FP_1
  * FP_2_ = FP_2             # <<<<<<<<<<<<<<
  * FP_DYNAMIC_ = FP_DYNAMIC
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(FP_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_2, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_2, __pyx_t_2) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":38
  * FP_1_ = FP_1
  * FP_2_ = FP_2
  * FP_DYNAMIC_ = FP_DYNAMIC             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(FP_DYNAMIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_DYNAMIC, __pyx_t_1) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_DYNAMIC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_DYNAMIC, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "_lapjv.pyx":41
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
+ * @cython.wraparound(False)
+ * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_1lapjv, 0, __pyx_n_s_lapjv, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 0)) __PYX_ERR(0, 41, __pyx_L1_error)
 
   /* "_lapjv.pyx":44
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  *           double cost_limit=np.inf, char return_cost=True):             # <<<<<<<<<<<<<<
  *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_inf); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_inf); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_cost_limit = __pyx_t_5;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_4__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapjv, __pyx_t_2) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_k_ = __pyx_t_3;
 
-  /* "_lapjv.pyx":43
- * @cython.boundscheck(False)
+  /* "_lapjv.pyx":136
+ * 
+ * 
+ * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
- *           double cost_limit=np.inf, char return_cost=True):
- *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
+ * def _lapmod(
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6_lapjv_1lapjv, NULL, __pyx_n_s_lapjv_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_3_lapmod, 0, __pyx_n_s_lapmod, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapjv, __pyx_t_2) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 136, __pyx_L1_error)
 
   /* "_lapjv.pyx":143
  *         cnp.ndarray ii not None,
  *         cnp.ndarray kk not None,
  *         fp_t fp_version=FP_DYNAMIC):             # <<<<<<<<<<<<<<
  *     """Internal function called from lapmod(..., fast=True)."""
  *     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
  */
-  __pyx_k__6 = FP_DYNAMIC;
-
-  /* "_lapjv.pyx":138
- * @cython.boundscheck(False)
- * @cython.wraparound(False)
- * def _lapmod(             # <<<<<<<<<<<<<<
- *         const uint_t n,
- *         cnp.ndarray cc not None,
- */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6_lapjv_3_lapmod, NULL, __pyx_n_s_lapjv_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_fp_version = FP_DYNAMIC;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_6__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":1
  * # Tomas Kazmar, 2012-2017, BSD 2-clause license, see LICENSE.             # <<<<<<<<<<<<<<
  * 
  * # Updated 2023/06/22 by rathaROG
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../tmp/build-env-9ltlyl_d/lib/python3.11/site-packages/numpy/__init__.pxd":1010
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init _lapjv", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init _lapjv");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -5633,203 +7259,339 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* RaiseDoubleKeywords */
-static void __Pyx_RaiseDoubleKeywordsError(
-    const char* func_name,
-    PyObject* kw_name)
-{
-    PyErr_Format(PyExc_TypeError,
-        #if PY_MAJOR_VERSION >= 3
-        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
-        #else
-        "%s() got multiple values for keyword argument '%s'", func_name,
-        PyString_AsString(kw_name));
-        #endif
-}
-
-/* ParseKeywords */
-static int __Pyx_ParseOptionalKeywords(
-    PyObject *kwds,
-    PyObject **argnames[],
-    PyObject *kwds2,
-    PyObject *values[],
-    Py_ssize_t num_pos_args,
-    const char* function_name)
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
-    PyObject *key = 0, *value = 0;
-    Py_ssize_t pos = 0;
-    PyObject*** name;
-    PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
-        name = first_kw_arg;
-        while (*name && (**name != key)) name++;
-        if (*name) {
-            values[name-argnames] = value;
-            continue;
-        }
-        name = first_kw_arg;
-        #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_Check(key))) {
-            while (*name) {
-                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
-                        && _PyString_Eq(**name, key)) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    if ((**argname == key) || (
-                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
-                             && _PyString_Eq(**argname, key))) {
-                        goto arg_passed_twice;
-                    }
-                    argname++;
-                }
-            }
-        } else
-        #endif
-        if (likely(PyUnicode_Check(key))) {
-            while (*name) {
-                int cmp = (**name == key) ? 0 :
-                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                #endif
-                    PyUnicode_Compare(**name, key);
-                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                if (cmp == 0) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    int cmp = (**argname == key) ? 0 :
-                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                    #endif
-                        PyUnicode_Compare(**argname, key);
-                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                    if (cmp == 0) goto arg_passed_twice;
-                    argname++;
-                }
-            }
-        } else
-            goto invalid_keyword_type;
-        if (kwds2) {
-            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
-        } else {
-            goto invalid_keyword;
-        }
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
     }
-    return 0;
-arg_passed_twice:
-    __Pyx_RaiseDoubleKeywordsError(function_name, key);
-    goto bad;
-invalid_keyword_type:
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() keywords must be strings", function_name);
-    goto bad;
-invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
-    #if PY_MAJOR_VERSION < 3
-        "%.200s() got an unexpected keyword argument '%.200s'",
-        function_name, PyString_AsString(key));
-    #else
-        "%s() got an unexpected keyword argument '%U'",
-        function_name, key);
-    #endif
-bad:
-    return -1;
+    return exc_info;
 }
+#endif
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
     } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
     }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
 }
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
 {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
     }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
     }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
     }
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
     return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
 }
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
@@ -5844,43 +7606,19 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -6005,15 +7743,17 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_FAST_THREAD_STATE
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
@@ -6027,14 +7767,404 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
+/* RaiseDoubleKeywords */
+static void __Pyx_RaiseDoubleKeywordsError(
+    const char* func_name,
+    PyObject* kw_name)
+{
+    PyErr_Format(PyExc_TypeError,
+        #if PY_MAJOR_VERSION >= 3
+        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
+        #else
+        "%s() got multiple values for keyword argument '%s'", func_name,
+        PyString_AsString(kw_name));
+        #endif
+}
+
+/* ParseKeywords */
+static int __Pyx_ParseOptionalKeywords(
+    PyObject *kwds,
+    PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2,
+    PyObject *values[],
+    Py_ssize_t num_pos_args,
+    const char* function_name)
+{
+    PyObject *key = 0, *value = 0;
+    Py_ssize_t pos = 0;
+    PyObject*** name;
+    PyObject*** first_kw_arg = argnames + num_pos_args;
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
+        name = first_kw_arg;
+        while (*name && (**name != key)) name++;
+        if (*name) {
+            values[name-argnames] = value;
+            continue;
+        }
+        name = first_kw_arg;
+        #if PY_MAJOR_VERSION < 3
+        if (likely(PyString_Check(key))) {
+            while (*name) {
+                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
+                        && _PyString_Eq(**name, key)) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    if ((**argname == key) || (
+                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
+                             && _PyString_Eq(**argname, key))) {
+                        goto arg_passed_twice;
+                    }
+                    argname++;
+                }
+            }
+        } else
+        #endif
+        if (likely(PyUnicode_Check(key))) {
+            while (*name) {
+                int cmp = (
+                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                #endif
+                    PyUnicode_Compare(**name, key)
+                );
+                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                if (cmp == 0) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    int cmp = (**argname == key) ? 0 :
+                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                    #endif
+                        PyUnicode_Compare(**argname, key);
+                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                    if (cmp == 0) goto arg_passed_twice;
+                    argname++;
+                }
+            }
+        } else
+            goto invalid_keyword_type;
+        if (kwds2) {
+            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
+        } else {
+            goto invalid_keyword;
+        }
+    }
+    return 0;
+arg_passed_twice:
+    __Pyx_RaiseDoubleKeywordsError(function_name, key);
+    goto bad;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    goto bad;
+invalid_keyword:
+    #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+    PyErr_Format(PyExc_TypeError,
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+bad:
+    return -1;
+}
+
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
+}
+
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -6070,14 +8200,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -6090,22 +8228,29 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
@@ -6188,15 +8333,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -6238,15 +8383,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -6270,15 +8416,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -6669,107 +8816,111 @@
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
 /* PyIntBinop */
   #if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
         long a = PyInt_AS_LONG(op1);
-            x = (long)((unsigned long)a + b);
+        
+            x = (long)((unsigned long)a + (unsigned long)b);
             if (likely((x^a) >= 0 || (x^b) >= 0))
                 return PyInt_FromLong(x);
             return PyLong_Type.tp_as_number->nb_add(op1, op2);
     }
     #endif
     #if CYTHON_USE_PYLONG_INTERNALS
     if (likely(PyLong_CheckExact(op1))) {
         const long b = intval;
         long a, x;
 #ifdef HAVE_LONG_LONG
         const PY_LONG_LONG llb = intval;
         PY_LONG_LONG lla, llx;
 #endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
+        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
+            return __Pyx_NewRef(op2);
+        }
+        if (likely(__Pyx_PyLong_IsCompact(op1))) {
+            a = __Pyx_PyLong_CompactValue(op1);
         } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
             switch (size) {
                 case -2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
             }
         }
                 x = a + b;
             return PyLong_FromLong(x);
@@ -6780,27 +8931,32 @@
 #endif
         
         
     }
     #endif
     if (PyFloat_CheckExact(op1)) {
         const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
         double a = PyFloat_AS_DOUBLE(op1);
+#endif
             double result;
+            
             PyFPE_START_PROTECT("add", return NULL)
             result = ((double)a) + (double)b;
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* PyFunctionFastCall */
-  #if CYTHON_FAST_PYCALL
+  #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -6821,15 +8977,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -6837,15 +8992,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -6908,15 +9063,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
 
 /* PyObjectCallMethO */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -6930,103 +9084,101 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+/* PyObjectFastCall */
+  static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
     }
-#endif
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
 #if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+        if (__Pyx_IsCyOrPyCFunction(func))
 #else
-    if (likely(PyCFunction_Check(func)))
+        if (PyCFunction_Check(func))
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
-/* PyCFunctionFastCall */
-  #if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
     }
-}
 #endif
-
-/* PyObjectCallOneArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+
+/* PyObjectCallOneArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
-#endif
 
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (!j) return NULL;
+    if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -7079,314 +9231,117 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return m->sq_item(o, i);
+            return sm->sq_item(o, i);
         }
     }
 #else
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
         return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
     }
     if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
         PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+        PyErr_Format(PyExc_IndexError,
+            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
+        __Pyx_DECREF_TypeName(index_type_name);
     }
     return NULL;
 }
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
-/* PyObjectCall2Args */
-  static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
-/* WriteUnraisableException */
-  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-    else state = (PyGILState_STATE)0;
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
-    }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
-    }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
-#endif
-}
-
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
+static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
+    __Pyx_TypeName obj_type_name;
+    if (likely(PyType_Check(obj))) {
+        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
+        if (meth) {
+            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
+            Py_DECREF(meth);
+            return result;
+        }
     }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return NULL;
 }
-#endif
-
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyMappingMethods *mm = tp->tp_as_mapping;
+    PySequenceMethods *sm = tp->tp_as_sequence;
+    if (likely(mm && mm->mp_subscript)) {
+        return mm->mp_subscript(obj, key);
     }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    if (likely(sm && sm->sq_item)) {
+        return __Pyx_PyObject_GetIndex(obj, key);
     }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    return __Pyx_PyObject_GetItem_Slow(obj, key);
 }
 #endif
 
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
-#ifdef Py_LIMITED_API
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
     PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
     itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
@@ -7410,25 +9365,26 @@
         if (itemsize < (Py_ssize_t)alignment)
             itemsize = (Py_ssize_t)alignment;
     }
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -7436,99 +9392,1353 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__7;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -7542,15 +10752,16 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -7620,25 +10831,36 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -7665,14 +10887,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -7727,19 +10950,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -7771,15 +11000,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -7791,15 +11020,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -7925,15 +11154,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -7945,15 +11174,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -8167,59 +11396,64 @@
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(char) < sizeof(long)) {
+        if ((sizeof(char) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(char, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (char) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (char) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(char, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(char) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) >= 2 * PyLong_SHIFT) {
-                            return (char) (((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 2 * PyLong_SHIFT)) {
+                                return (char) (((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(char) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) >= 3 * PyLong_SHIFT) {
-                            return (char) (((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 3 * PyLong_SHIFT)) {
+                                return (char) (((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(char) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
-                            return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 4 * PyLong_SHIFT)) {
+                                return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
@@ -8227,117 +11461,189 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (char) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(char) <= sizeof(unsigned long)) {
+            if ((sizeof(char) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(char, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(char) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(char, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (char) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(char, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(char,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(char) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 2 * PyLong_SHIFT) {
-                            return (char) (((char)-1)*(((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(char) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(char) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 2 * PyLong_SHIFT) {
-                            return (char) ((((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                                return (char) ((((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(char) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 3 * PyLong_SHIFT) {
-                            return (char) (((char)-1)*(((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(char) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 3 * PyLong_SHIFT) {
-                            return (char) ((((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                                return (char) ((((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(char) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 4 * PyLong_SHIFT) {
-                            return (char) (((char)-1)*(((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(char) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(char) - 1 > 4 * PyLong_SHIFT) {
-                            return (char) ((((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
+                                return (char) ((((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(char) <= sizeof(long)) {
+            if ((sizeof(char) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(char, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(char) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(char, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             char val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (char) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (char) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (char) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (char) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (char) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(char) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((char) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(char) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((char) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((char) 1) << (sizeof(char) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (char) -1;
         }
     } else {
         char val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (char) -1;
         val = __Pyx_PyInt_As_char(tmp);
@@ -8363,59 +11669,64 @@
     const uint_t neg_one = (uint_t) -1, const_zero = (uint_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(uint_t) < sizeof(long)) {
+        if ((sizeof(uint_t) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(uint_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (uint_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (uint_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(uint_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(uint_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) >= 2 * PyLong_SHIFT) {
-                            return (uint_t) (((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(uint_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(uint_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) >= 2 * PyLong_SHIFT)) {
+                                return (uint_t) (((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(uint_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) >= 3 * PyLong_SHIFT) {
-                            return (uint_t) (((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(uint_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) >= 3 * PyLong_SHIFT)) {
+                                return (uint_t) (((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(uint_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) >= 4 * PyLong_SHIFT) {
-                            return (uint_t) (((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(uint_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) >= 4 * PyLong_SHIFT)) {
+                                return (uint_t) (((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
@@ -8423,117 +11734,189 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (uint_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(uint_t) <= sizeof(unsigned long)) {
+            if ((sizeof(uint_t) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(uint_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (uint_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(uint_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(uint_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(uint_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint_t) (((uint_t)-1)*(((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(uint_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(uint_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (uint_t) (((uint_t)-1)*(((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(uint_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint_t) ((((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(uint_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (uint_t) ((((((uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint_t) (((uint_t)-1)*(((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(uint_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (uint_t) (((uint_t)-1)*(((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(uint_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint_t) ((((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(uint_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (uint_t) ((((((((uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint_t) (((uint_t)-1)*(((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(uint_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (uint_t) (((uint_t)-1)*(((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(uint_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint_t) ((((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(uint_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(uint_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(uint_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (uint_t) ((((((((((uint_t)digits[3]) << PyLong_SHIFT) | (uint_t)digits[2]) << PyLong_SHIFT) | (uint_t)digits[1]) << PyLong_SHIFT) | (uint_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(uint_t) <= sizeof(long)) {
+            if ((sizeof(uint_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint_t) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(uint_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(uint_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             uint_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (uint_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (uint_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (uint_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (uint_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (uint_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(uint_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((uint_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(uint_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((uint_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((uint_t) 1) << (sizeof(uint_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (uint_t) -1;
         }
     } else {
         uint_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (uint_t) -1;
         val = __Pyx_PyInt_As_uint_t(tmp);
@@ -8559,59 +11942,64 @@
     const enum fp_t neg_one = (enum fp_t) -1, const_zero = (enum fp_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(enum fp_t) < sizeof(long)) {
+        if ((sizeof(enum fp_t) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(enum fp_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (enum fp_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (enum fp_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(enum fp_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(enum fp_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) >= 2 * PyLong_SHIFT) {
-                            return (enum fp_t) (((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(enum fp_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(enum fp_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) >= 2 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(enum fp_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) >= 3 * PyLong_SHIFT) {
-                            return (enum fp_t) (((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(enum fp_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) >= 3 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(enum fp_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) >= 4 * PyLong_SHIFT) {
-                            return (enum fp_t) (((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(enum fp_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) >= 4 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
@@ -8619,119 +12007,97 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (enum fp_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(enum fp_t) <= sizeof(unsigned long)) {
+            if ((sizeof(enum fp_t) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(enum fp_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(enum fp_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(enum fp_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(enum fp_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (enum fp_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(enum fp_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(enum fp_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(enum fp_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (enum fp_t) (((enum fp_t)-1)*(((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(enum fp_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(enum fp_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((enum fp_t)-1)*(((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(enum fp_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (enum fp_t) ((((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(enum fp_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (enum fp_t) ((((((enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (enum fp_t) (((enum fp_t)-1)*(((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(enum fp_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((enum fp_t)-1)*(((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(enum fp_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (enum fp_t) ((((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(enum fp_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (enum fp_t) ((((((((enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (enum fp_t) (((enum fp_t)-1)*(((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(enum fp_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (enum fp_t) (((enum fp_t)-1)*(((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(enum fp_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(enum fp_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (enum fp_t) ((((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(enum fp_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(enum fp_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(enum fp_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (enum fp_t) ((((((((((enum fp_t)digits[3]) << PyLong_SHIFT) | (enum fp_t)digits[2]) << PyLong_SHIFT) | (enum fp_t)digits[1]) << PyLong_SHIFT) | (enum fp_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(enum fp_t) <= sizeof(long)) {
+            if ((sizeof(enum fp_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(enum fp_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(enum fp_t) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(enum fp_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(enum fp_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            enum fp_t val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (enum fp_t) -1;
-        }
+        PyErr_SetString(PyExc_RuntimeError,
+                        "_PyLong_AsByteArray() not available, cannot convert large enums");
+        return (enum fp_t) -1;
     } else {
         enum fp_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (enum fp_t) -1;
         val = __Pyx_PyInt_As_enum__fp_t(tmp);
         Py_DECREF(tmp);
         return val;
@@ -8831,59 +12197,64 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
@@ -8891,117 +12262,189 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9090,72 +12533,92 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int_t),
                                      little, !is_unsigned);
     }
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__12));
+    }
+    return name;
+}
+#endif
+
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
@@ -9163,117 +12626,189 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -9290,15 +12825,15 @@
     return (long) -1;
 }
 
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -9311,14 +12846,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -9335,19 +12886,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -9416,50 +12967,60 @@
                 found_dot = 1;
             } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
                 break;
             }
             rtversion[i] = rt_from_call[i];
         }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -9513,15 +13074,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -9542,30 +13103,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -9623,21 +13188,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -9697,8 +13260,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `lapx-0.5.2.post1/_lapjv_src/_lapjv.pyx` & `lapx-0.5.3/_lapjv_src/_lapjv.pyx`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/_lapjv_src/lapjv.cpp` & `lapx-0.5.3/_lapjv_src/lapjv.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/_lapjv_src/lapjv.h` & `lapx-0.5.3/_lapjv_src/lapjv.h`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/_lapjv_src/lapmod.cpp` & `lapx-0.5.3/_lapjv_src/lapmod.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/__init__.py` & `lapx-0.5.3/lap/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Find optimal (minimum-cost) assignment for a dense cost matrix.
 lapmod
     Find optimal (minimum-cost) assignment for a sparse cost matrix.
 """
 
 import sys
 
-__version__ = '0.5.2.post1'
+__version__ = '0.5.3'
 
 try:
     __LAP_SETUP__
 except NameError:
     __LAP_SETUP__ = False
 if __LAP_SETUP__:
     sys.stderr.write('Partial import of lap during the build process.\n')
```

### Comparing `lapx-0.5.2.post1/lap/lapmod.py` & `lapx-0.5.3/lap/lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/tests/cost_eps.csv.gz` & `lapx-0.5.3/lap/tests/cost_eps.csv.gz`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/tests/test_arr_loop.py` & `lapx-0.5.3/lap/tests/test_arr_loop.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/tests/test_lapjv.py` & `lapx-0.5.3/lap/tests/test_lapjv.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/tests/test_lapmod.py` & `lapx-0.5.3/lap/tests/test_lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lap/tests/test_utils.py` & `lapx-0.5.3/lap/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.2.post1/lapx.egg-info/PKG-INFO` & `lapx-0.5.3/lapx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.2.post1
-Summary: Customized Tomas Kazmar's lap, Linear Assignment Problem solver (LAPJV/LAPMOD).
+Version: 0.5.3
+Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap,lap05
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,71 +27,66 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Windows/Linux/macOS + Python [3.7-3.11] .](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml)
-[![Build `tar.gz` PyPI](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/build_pypi.yaml)
+[![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test.yaml)
+[![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
+[![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-* `lapx` is a customized edition of Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap).
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE).
-* Source credit: Tomas Kazmar @[`gatagat`](https://github.com/gatagat).
-* `pypi.org` source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11.
 
+* License: BSD-2-Clause, see [`LICENSE`](LICENSE)
+* Based source code: [lap05-0.5.1.tar.gz](https://files.pythonhosted.org/packages/05/71/5531017a60f5028c87ce34514f2b55d35a2999f6c6e587d1f56e6ee78b10/lap05-0.5.1.tar.gz)
+* Credits: @[`gatagat`](https://github.com/gatagat) @[`remram44`](https://github.com/gatagat/lap/issues/34#issue-1114097201)
 
-## Windows ✅ | Linux ✅ | macOS ✅
+## Installation: Windows ✅ | Linux ✅ | macOS ✅
 
-* Build passed on all [Windows/Linux/macOS](https://github.com/rathaROG/lapx/actions/workflows/build_all.yaml) with Python 3.7/3.8/3.9/3.10/3.11 ✅
-
-* Install from PyPI:
+* Install from [PyPI](https://pypi.org/project/lapx/):
 
   ```
   pip install lapx
   ```
 
-* Or download [`tar.gz` or Wheels from releases](https://github.com/rathaROG/lapx/releases)
-
-* Or directly install from GitHub:
+* Or install `.tar.gz` or `.whl` from [GitHub releases](https://github.com/rathaROG/lapx/releases) or install from GitHub repo directly:
 
   ```
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
   pip install git+https://github.com/rathaROG/lapx.git
   ```
 
-* Or clone and build directly on your machine:
+* Or clone and build on your local machine:
 
   ```
   git clone https://github.com/rathaROG/lapx.git
   cd lapx
   python -m pip install --upgrade pip
   pip install "setuptools>=67.2.0"
   pip install wheel build
   python -m build --wheel
   cd dist
   ```
 
 ## Usage 🧪
 
-Note: Use `import lap` to import since `lapx` is just the name for package distribution. 
+* `lapx` is just the name for package distribution.
+* The same as `lap`, use `import lap` to import; for example:
 
-```
-import lap
-import numpy as np
-print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
-```
+  ```
+  import lap
+  import numpy as np
+  print(lap.lapjv(np.random.rand(2, 1), extend_cost=True))
+  ```
 
 <br />
 
-<details><summary><ins>Click here to show more ...</ins></summary>
+<details><summary>Click here to show more...</summary>
 
 <br />
 
 lap: Linear Assignment Problem solver
 =====================================
 
 **lap** is a [linear assignment
```

### Comparing `lapx-0.5.2.post1/setup.py` & `lapx-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # # # # # # # # # # # # # # # # # # # # # #
-#    Rewrite on 2023/06/24 by rathaROG    #
+#    Rewrote on 2023/06/24 by rathaROG    #
+#    Updated on 2023/07/19 by rathaROG    #
 # # # # # # # # # # # # # # # # # # # # # #
 
 
 import distutils.cmd
 from setuptools import setup
 from setuptools.extension import Extension
 
 ###################################################################
 
-DESCRIPTION = "Customized Tomas Kazmar's lap, Linear Assignment Problem solver (LAPJV/LAPMOD)."
+DESCRIPTION = "Linear Assignment Problem solver (LAPJV/LAPMOD)."
 LICENSE = 'BSD-2-Clause'
 LONG_DESCRIPTION = open("README.md", encoding="utf-8").read()
 
 ###################################################################
 
 package_name = 'lapx'
 package_path = 'lap'
@@ -62,15 +63,14 @@
             if file[-2:].lower() in "soyd":
                 shutil.copy2(os.path.join(_lapjv, file), lap)
                 break
 
 def main_setup():
     """Use modern setup() 
     """
-
     import os
     from Cython.Build import cythonize
     _lapjvpyx = os.path.join(_lapjv, '_lapjv.pyx')
     _lapjvcpp = compile_cpp(_lapjvpyx)
     lapjvcpp = os.path.join(_lapjv, 'lapjv.cpp')
     lapmodcpp = os.path.join(_lapjv, 'lapmod.cpp')
 
@@ -81,15 +81,15 @@
             include_dirs=[numpy_include(), package_path],
         )
     ]
 
     package_data = {}
     tests_package = package_path + ".tests"
     packages = [package_path, tests_package]
-    for p in packages: package_data = {p: ["*"]}
+    for p in packages: package_data.update({p: ["*"]})
 
     setup(
         name=package_name,
         version=get_version_string(),
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
@@ -120,15 +120,15 @@
                      'Topic :: Software Development',
                      'Topic :: Software Development :: Libraries',
                      'Operating System :: Microsoft :: Windows',                                  
                      'Operating System :: POSIX',
                      'Operating System :: Unix',
                      'Operating System :: MacOS',],
         ext_modules=cythonize(ext_modules),
-        cmdclass={'ccythonize': ExportCythonCommand,},
+        cmdclass={'cmdexport': ExportCythonCommand,},
     )
 
 def read_requirments():
     with open(requirments_txt) as input_tmp_file:
         return [line for line in input_tmp_file.read().splitlines()]
 
 if __name__ == "__main__":
```

