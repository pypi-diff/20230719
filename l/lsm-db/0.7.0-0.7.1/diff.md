# Comparing `tmp/lsm-db-0.7.0.tar.gz` & `tmp/lsm-db-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lsm-db-0.7.0.tar", last modified: Thu Mar  2 14:41:03 2023, max compression
+gzip compressed data, was "dist/lsm-db-0.7.1.tar", last modified: Tue Jul 18 22:30:25 2023, max compression
```

## Comparing `lsm-db-0.7.0.tar` & `lsm-db-0.7.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-03-02 14:41:03.000000 lsm-db-0.7.0/
--rw-rw-r--   0 charles   (1000) charles   (1000)      218 2018-08-16 18:40:47.000000 lsm-db-0.7.0/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)      225 2023-03-02 14:41:03.000000 lsm-db-0.7.0/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     6604 2021-08-09 15:52:07.000000 lsm-db-0.7.0/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-03-02 14:41:03.000000 lsm-db-0.7.0/docs/
--rw-rw-r--   0 charles   (1000) charles   (1000)     7409 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/Makefile
--rw-rw-r--   0 charles   (1000) charles   (1000)     2459 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/api.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)     9179 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/conf.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1658 2019-01-22 16:06:09.000000 lsm-db-0.7.0/docs/index.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)      870 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/installation.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)     5850 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/quickstart.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)        7 2018-08-16 18:40:47.000000 lsm-db-0.7.0/docs/requirements.txt
--rw-r--r--   0 charles   (1000) charles   (1000)  1080370 2022-12-31 14:05:24.000000 lsm-db-0.7.0/lsm.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    60551 2019-08-11 20:06:32.000000 lsm-db-0.7.0/lsm.pyx
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-03-02 14:41:03.000000 lsm-db-0.7.0/lsm_db.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)      225 2023-03-02 14:41:03.000000 lsm-db-0.7.0/lsm_db.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      515 2023-03-02 14:41:03.000000 lsm-db-0.7.0/lsm_db.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-03-02 14:41:03.000000 lsm-db-0.7.0/lsm_db.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        4 2023-03-02 14:41:03.000000 lsm-db-0.7.0/lsm_db.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-03-02 14:41:03.000000 lsm-db-0.7.0/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)      771 2023-03-02 14:40:34.000000 lsm-db-0.7.0/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-03-02 14:41:03.000000 lsm-db-0.7.0/src/
--rw-rw-r--   0 charles   (1000) charles   (1000)    26725 2023-03-02 14:38:50.000000 lsm-db-0.7.0/src/lsm.h
--rw-rw-r--   0 charles   (1000) charles   (1000)    33728 2023-03-02 14:38:50.000000 lsm-db-0.7.0/src/lsmInt.h
--rw-rw-r--   0 charles   (1000) charles   (1000)    38996 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_ckpt.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    99726 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_file.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    39308 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_log.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    27168 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_main.c
--rw-rw-r--   0 charles   (1000) charles   (1000)     2383 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_mem.c
--rw-rw-r--   0 charles   (1000) charles   (1000)     2317 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_mutex.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    60532 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_shared.c
--rw-rw-r--   0 charles   (1000) charles   (1000)   184363 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_sorted.c
--rw-rw-r--   0 charles   (1000) charles   (1000)     3829 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_str.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    74206 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_tree.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    19398 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_unix.c
--rw-rw-r--   0 charles   (1000) charles   (1000)     4516 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_varint.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    29904 2023-03-02 14:38:47.000000 lsm-db-0.7.0/src/lsm_win32.c
--rw-rw-r--   0 charles   (1000) charles   (1000)    26688 2018-08-16 18:40:47.000000 lsm-db-0.7.0/tests.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:30:25.000000 lsm-db-0.7.1/
+-rw-r--r--   0 charles   (1000) charles   (1000)      241 2023-04-06 12:11:24.000000 lsm-db-0.7.1/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)      225 2023-07-18 22:30:25.000000 lsm-db-0.7.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     6604 2021-08-09 15:52:07.000000 lsm-db-0.7.1/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:30:25.000000 lsm-db-0.7.1/docs/
+-rw-r--r--   0 charles   (1000) charles   (1000)     7409 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/Makefile
+-rw-r--r--   0 charles   (1000) charles   (1000)     2459 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/api.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)     9179 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/conf.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     1658 2019-01-22 16:06:09.000000 lsm-db-0.7.1/docs/index.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)      870 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/installation.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)     5850 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/quickstart.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)        7 2018-08-16 18:40:47.000000 lsm-db-0.7.1/docs/requirements.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)  1088838 2023-07-18 22:29:38.000000 lsm-db-0.7.1/lsm.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    60716 2023-07-18 22:29:36.000000 lsm-db-0.7.1/lsm.pyx
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:30:25.000000 lsm-db-0.7.1/lsm_db.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)      225 2023-07-18 22:30:25.000000 lsm-db-0.7.1/lsm_db.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      530 2023-07-18 22:30:25.000000 lsm-db-0.7.1/lsm_db.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-07-18 22:30:25.000000 lsm-db-0.7.1/lsm_db.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        4 2023-07-18 22:30:25.000000 lsm-db-0.7.1/lsm_db.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       60 2023-03-02 18:58:33.000000 lsm-db-0.7.1/pyproject.toml
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-18 22:30:25.000000 lsm-db-0.7.1/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)      771 2023-07-18 22:30:05.000000 lsm-db-0.7.1/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:30:25.000000 lsm-db-0.7.1/src/
+-rw-r--r--   0 charles   (1000) charles   (1000)    26725 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    33728 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsmInt.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    38996 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_ckpt.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    99726 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_file.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    39308 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_log.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    27168 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_main.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2383 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_mem.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2317 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_mutex.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    60532 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_shared.c
+-rw-r--r--   0 charles   (1000) charles   (1000)   184363 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_sorted.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     3829 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_str.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    74206 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_tree.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    19398 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_unix.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     4516 2023-03-02 18:58:33.000000 lsm-db-0.7.1/src/lsm_varint.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    29904 2018-08-16 18:40:47.000000 lsm-db-0.7.1/src/lsm_win32.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    26688 2018-08-16 18:40:47.000000 lsm-db-0.7.1/tests.py
```

### Comparing `lsm-db-0.7.0/README.md` & `lsm-db-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/Makefile` & `lsm-db-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/api.rst` & `lsm-db-0.7.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/conf.py` & `lsm-db-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/index.rst` & `lsm-db-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/installation.rst` & `lsm-db-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/docs/quickstart.rst` & `lsm-db-0.7.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/lsm.c` & `lsm-db-0.7.1/lsm.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/lsm.h"
         ],
         "name": "lsm",
         "sources": [
             "lsm.pyx",
+            "src/lsm_varint.c",
+            "src/lsm_win32.c",
             "src/lsm_ckpt.c",
-            "src/lsm_sorted.c",
             "src/lsm_str.c",
+            "src/lsm_mutex.c",
             "src/lsm_mem.c",
             "src/lsm_file.c",
-            "src/lsm_unix.c",
             "src/lsm_tree.c",
-            "src/lsm_varint.c",
-            "src/lsm_log.c",
+            "src/lsm_shared.c",
+            "src/lsm_unix.c",
             "src/lsm_main.c",
-            "src/lsm_win32.c",
-            "src/lsm_mutex.c",
-            "src/lsm_shared.c"
+            "src/lsm_log.c",
+            "src/lsm_sorted.c"
         ]
     },
     "module_name": "lsm"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,24 +102,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -227,15 +231,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +270,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -389,17 +393,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -469,14 +470,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -576,35 +582,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1116,15 +1122,15 @@
   lsm_cursor *cursor;
   int is_open;
   int _consumed;
   int _reverse;
 };
 
 
-/* "lsm.pyx":1691
+/* "lsm.pyx":1695
  * 
  * 
  * cdef class Transaction(object):             # <<<<<<<<<<<<<<
  *     """
  *     Context manager and decorator to run the wrapped block in a transaction.
  */
 struct __pyx_obj_3lsm_Transaction {
@@ -1308,36 +1314,36 @@
 
 
 /* "lsm.pyx":1668
  *         return self._value()
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 struct __pyx_obj_3lsm___pyx_scope_struct_8_keys {
   PyObject_HEAD
   struct __pyx_obj_3lsm_Cursor *__pyx_v_self;
 };
 
 
-/* "lsm.pyx":1679
- *                 self.next()
+/* "lsm.pyx":1681
+ *                     break
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields values."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 struct __pyx_obj_3lsm___pyx_scope_struct_9_values {
   PyObject_HEAD
   struct __pyx_obj_3lsm_Cursor *__pyx_v_self;
 };
 
 
-/* "lsm.pyx":1732
+/* "lsm.pyx":1736
  *                 raise
  * 
  *     def __call__(self, fn):             # <<<<<<<<<<<<<<
  *         def inner(*args, **kwargs):
  *             with self:
  */
 struct __pyx_obj_3lsm___pyx_scope_struct_10___call__ {
@@ -1505,26 +1511,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1940,22 +1946,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3988,15 +4002,15 @@
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_filename);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 374, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->encoded_filename);
     __Pyx_DECREF(__pyx_v_self->encoded_filename);
     __pyx_v_self->encoded_filename = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "lsm.pyx":373
@@ -5253,15 +5267,15 @@
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 643, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 643, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -10312,15 +10326,15 @@
  *         try:
  *             value = self[key]             # <<<<<<<<<<<<<<
  *         except KeyError:
  *             ivalue = 0
  */
       __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1169, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 1169, __pyx_L3_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 1169, __pyx_L3_error)
       __pyx_v_value = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
       /* "lsm.pyx":1168
  *         cdef bytes value
  *         cdef int ivalue
  *         try:             # <<<<<<<<<<<<<<
@@ -15814,15 +15828,15 @@
       /*try:*/ {
 
         /* "lsm.pyx":1637
  *         else:
  *             try:
  *                 self.seek(start, seek_method)             # <<<<<<<<<<<<<<
  *             except KeyError:
- *                 raise StopIteration
+ *                 return
  */
         __pyx_t_9.__pyx_n = 1;
         __pyx_t_9.method = __pyx_cur_scope->__pyx_v_seek_method;
         __pyx_t_3 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->seek(__pyx_cur_scope->__pyx_v_self, __pyx_cur_scope->__pyx_v_start, 0, &__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1637, __pyx_L25_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
@@ -15842,34 +15856,38 @@
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "lsm.pyx":1638
  *             try:
  *                 self.seek(start, seek_method)
  *             except KeyError:             # <<<<<<<<<<<<<<
- *                 raise StopIteration
+ *                 return
  * 
  */
       __pyx_t_2 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
       if (__pyx_t_2) {
         __Pyx_AddTraceback("lsm.Cursor.fetch_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
         if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_10) < 0) __PYX_ERR(0, 1638, __pyx_L27_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_10);
 
         /* "lsm.pyx":1639
  *                 self.seek(start, seek_method)
  *             except KeyError:
- *                 raise StopIteration             # <<<<<<<<<<<<<<
+ *                 return             # <<<<<<<<<<<<<<
  * 
  *         for key, value in self.fetch_until(end):
  */
-        __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-        __PYX_ERR(0, 1639, __pyx_L27_except_error)
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_r = NULL;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        goto __pyx_L28_except_return;
       }
       goto __pyx_L27_except_error;
       __pyx_L27_except_error:;
 
       /* "lsm.pyx":1636
  *                 self.first()
  *         else:
@@ -15878,21 +15896,27 @@
  *             except KeyError:
  */
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_8);
       __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_6, __pyx_t_8);
       goto __pyx_L1_error;
+      __pyx_L28_except_return:;
+      __Pyx_XGIVEREF(__pyx_t_7);
+      __Pyx_XGIVEREF(__pyx_t_6);
+      __Pyx_XGIVEREF(__pyx_t_8);
+      __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_6, __pyx_t_8);
+      goto __pyx_L0;
       __pyx_L30_try_end:;
     }
   }
   __pyx_L23:;
 
   /* "lsm.pyx":1641
- *                 raise StopIteration
+ *                 return
  * 
  *         for key, value in self.fetch_until(end):             # <<<<<<<<<<<<<<
  *             yield (key, value)
  * 
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_fetch_until); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -16038,15 +16062,15 @@
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_4);
     __pyx_t_11 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_12 = __pyx_cur_scope->__pyx_t_2;
     if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1642, __pyx_L1_error)
 
     /* "lsm.pyx":1641
- *                 raise StopIteration
+ *                 return
  * 
  *         for key, value in self.fetch_until(end):             # <<<<<<<<<<<<<<
  *             yield (key, value)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -16331,15 +16355,15 @@
 static PyObject *__pyx_gb_3lsm_6Cursor_42generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "lsm.pyx":1668
  *         return self._value()
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3lsm_6Cursor_41keys(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static char __pyx_doc_3lsm_6Cursor_40keys[] = "Return a generator that successively yields keys.";
 static PyObject *__pyx_pw_3lsm_6Cursor_41keys(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
@@ -16390,14 +16414,20 @@
 
 static PyObject *__pyx_gb_3lsm_6Cursor_42generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_3lsm___pyx_scope_struct_8_keys *__pyx_cur_scope = ((struct __pyx_obj_3lsm___pyx_scope_struct_8_keys *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("keys", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
@@ -16408,148 +16438,223 @@
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1668, __pyx_L1_error)
 
   /* "lsm.pyx":1670
  *     def keys(self):
  *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():             # <<<<<<<<<<<<<<
- *             raise StopIteration
- *         while True:
+ *         if self.is_valid():             # <<<<<<<<<<<<<<
+ *             while True:
+ *                 yield self._key()
  */
-  __pyx_t_1 = ((!(((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->is_valid(__pyx_cur_scope->__pyx_v_self, 0) != 0)) != 0);
-  if (unlikely(__pyx_t_1)) {
+  __pyx_t_1 = (((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->is_valid(__pyx_cur_scope->__pyx_v_self, 0) != 0);
+  if (__pyx_t_1) {
 
     /* "lsm.pyx":1671
  *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():
- *             raise StopIteration             # <<<<<<<<<<<<<<
- *         while True:
- *             yield self._key()
+ *         if self.is_valid():
+ *             while True:             # <<<<<<<<<<<<<<
+ *                 yield self._key()
+ *                 try:
+ */
+    while (1) {
+
+      /* "lsm.pyx":1672
+ *         if self.is_valid():
+ *             while True:
+ *                 yield self._key()             # <<<<<<<<<<<<<<
+ *                 try:
+ *                     if self._reverse:
  */
-    __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 1671, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_3lsm_6Cursor__key(__pyx_cur_scope->__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1672, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_r = __pyx_t_2;
+      __pyx_t_2 = 0;
+      __Pyx_XGIVEREF(__pyx_r);
+      __Pyx_RefNannyFinishContext();
+      __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+      /* return from generator, yielding value */
+      __pyx_generator->resume_label = 1;
+      return __pyx_r;
+      __pyx_L7_resume_from_yield:;
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1672, __pyx_L1_error)
 
-    /* "lsm.pyx":1670
- *     def keys(self):
- *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():             # <<<<<<<<<<<<<<
- *             raise StopIteration
- *         while True:
+      /* "lsm.pyx":1673
+ *             while True:
+ *                 yield self._key()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
  */
-  }
+      {
+        __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
+        __Pyx_XGOTREF(__pyx_t_3);
+        __Pyx_XGOTREF(__pyx_t_4);
+        __Pyx_XGOTREF(__pyx_t_5);
+        /*try:*/ {
 
-  /* "lsm.pyx":1672
- *         if not self.is_valid():
- *             raise StopIteration
- *         while True:             # <<<<<<<<<<<<<<
- *             yield self._key()
- *             if self._reverse:
+          /* "lsm.pyx":1674
+ *                 yield self._key()
+ *                 try:
+ *                     if self._reverse:             # <<<<<<<<<<<<<<
+ *                         self.previous()
+ *                     else:
+ */
+          __pyx_t_1 = (__pyx_cur_scope->__pyx_v_self->_reverse != 0);
+          if (__pyx_t_1) {
+
+            /* "lsm.pyx":1675
+ *                 try:
+ *                     if self._reverse:
+ *                         self.previous()             # <<<<<<<<<<<<<<
+ *                     else:
+ *                         self.next()
  */
-  while (1) {
+            __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->previous(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1675, __pyx_L8_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "lsm.pyx":1673
- *             raise StopIteration
- *         while True:
- *             yield self._key()             # <<<<<<<<<<<<<<
- *             if self._reverse:
- *                 self.previous()
+            /* "lsm.pyx":1674
+ *                 yield self._key()
+ *                 try:
+ *                     if self._reverse:             # <<<<<<<<<<<<<<
+ *                         self.previous()
+ *                     else:
  */
-    __pyx_t_2 = __pyx_f_3lsm_6Cursor__key(__pyx_cur_scope->__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1673, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
-    __Pyx_XGIVEREF(__pyx_r);
-    __Pyx_RefNannyFinishContext();
-    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-    /* return from generator, yielding value */
-    __pyx_generator->resume_label = 1;
-    return __pyx_r;
-    __pyx_L7_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1673, __pyx_L1_error)
+            goto __pyx_L16;
+          }
 
-    /* "lsm.pyx":1674
- *         while True:
- *             yield self._key()
- *             if self._reverse:             # <<<<<<<<<<<<<<
- *                 self.previous()
- *             else:
+          /* "lsm.pyx":1677
+ *                         self.previous()
+ *                     else:
+ *                         self.next()             # <<<<<<<<<<<<<<
+ *                 except StopIteration:
+ *                     break
  */
-    __pyx_t_1 = (__pyx_cur_scope->__pyx_v_self->_reverse != 0);
-    if (__pyx_t_1) {
+          /*else*/ {
+            __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->next(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1677, __pyx_L8_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          }
+          __pyx_L16:;
 
-      /* "lsm.pyx":1675
- *             yield self._key()
- *             if self._reverse:
- *                 self.previous()             # <<<<<<<<<<<<<<
- *             else:
- *                 self.next()
+          /* "lsm.pyx":1673
+ *             while True:
+ *                 yield self._key()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
  */
-      __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->previous(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1675, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        }
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        goto __pyx_L15_try_end;
+        __pyx_L8_error:;
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "lsm.pyx":1674
- *         while True:
- *             yield self._key()
- *             if self._reverse:             # <<<<<<<<<<<<<<
- *                 self.previous()
- *             else:
+        /* "lsm.pyx":1678
+ *                     else:
+ *                         self.next()
+ *                 except StopIteration:             # <<<<<<<<<<<<<<
+ *                     break
+ * 
  */
-      goto __pyx_L8;
-    }
+        __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
+        if (__pyx_t_6) {
+          __Pyx_AddTraceback("lsm.Cursor.keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1678, __pyx_L10_except_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_GOTREF(__pyx_t_8);
 
-    /* "lsm.pyx":1677
- *                 self.previous()
- *             else:
- *                 self.next()             # <<<<<<<<<<<<<<
+          /* "lsm.pyx":1679
+ *                         self.next()
+ *                 except StopIteration:
+ *                     break             # <<<<<<<<<<<<<<
  * 
  *     def values(self):
  */
-    /*else*/ {
-      __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->next(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1677, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          goto __pyx_L17_except_break;
+          __pyx_L17_except_break:;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          goto __pyx_L13_try_break;
+        }
+        goto __pyx_L10_except_error;
+        __pyx_L10_except_error:;
+
+        /* "lsm.pyx":1673
+ *             while True:
+ *                 yield self._key()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
+ */
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_XGIVEREF(__pyx_t_5);
+        __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+        goto __pyx_L1_error;
+        __pyx_L13_try_break:;
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_XGIVEREF(__pyx_t_5);
+        __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+        goto __pyx_L6_break;
+        __pyx_L15_try_end:;
+      }
     }
-    __pyx_L8:;
+    __pyx_L6_break:;
+
+    /* "lsm.pyx":1670
+ *     def keys(self):
+ *         """Return a generator that successively yields keys."""
+ *         if self.is_valid():             # <<<<<<<<<<<<<<
+ *             while True:
+ *                 yield self._key()
+ */
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* "lsm.pyx":1668
  *         return self._value()
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields keys."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_3lsm_6Cursor_45generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "lsm.pyx":1679
- *                 self.next()
+/* "lsm.pyx":1681
+ *                     break
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields values."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3lsm_6Cursor_44values(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static char __pyx_doc_3lsm_6Cursor_43values[] = "Return a generator that successively yields values.";
 static PyObject *__pyx_pw_3lsm_6Cursor_44values(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
@@ -16570,23 +16675,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("values", 0);
   __pyx_cur_scope = (struct __pyx_obj_3lsm___pyx_scope_struct_9_values *)__pyx_tp_new_3lsm___pyx_scope_struct_9_values(__pyx_ptype_3lsm___pyx_scope_struct_9_values, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_3lsm___pyx_scope_struct_9_values *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 1679, __pyx_L1_error)
+    __PYX_ERR(0, 1681, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3lsm_6Cursor_45generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_values, __pyx_n_s_Cursor_values, __pyx_n_s_lsm); if (unlikely(!gen)) __PYX_ERR(0, 1679, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3lsm_6Cursor_45generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_values, __pyx_n_s_Cursor_values, __pyx_n_s_lsm); if (unlikely(!gen)) __PYX_ERR(0, 1681, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16600,147 +16705,228 @@
 
 static PyObject *__pyx_gb_3lsm_6Cursor_45generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_3lsm___pyx_scope_struct_9_values *__pyx_cur_scope = ((struct __pyx_obj_3lsm___pyx_scope_struct_9_values *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("values", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L7_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1679, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1681, __pyx_L1_error)
 
-  /* "lsm.pyx":1681
+  /* "lsm.pyx":1683
  *     def values(self):
  *         """Return a generator that successively yields values."""
- *         if not self.is_valid():             # <<<<<<<<<<<<<<
- *             raise StopIteration
- *         while True:
+ *         if self.is_valid():             # <<<<<<<<<<<<<<
+ *             while True:
+ *                 yield self._value()
  */
-  __pyx_t_1 = ((!(((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->is_valid(__pyx_cur_scope->__pyx_v_self, 0) != 0)) != 0);
-  if (unlikely(__pyx_t_1)) {
+  __pyx_t_1 = (((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->is_valid(__pyx_cur_scope->__pyx_v_self, 0) != 0);
+  if (__pyx_t_1) {
 
-    /* "lsm.pyx":1682
+    /* "lsm.pyx":1684
  *         """Return a generator that successively yields values."""
- *         if not self.is_valid():
- *             raise StopIteration             # <<<<<<<<<<<<<<
- *         while True:
- *             yield self._value()
+ *         if self.is_valid():
+ *             while True:             # <<<<<<<<<<<<<<
+ *                 yield self._value()
+ *                 try:
  */
-    __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 1682, __pyx_L1_error)
+    while (1) {
 
-    /* "lsm.pyx":1681
- *     def values(self):
- *         """Return a generator that successively yields values."""
- *         if not self.is_valid():             # <<<<<<<<<<<<<<
- *             raise StopIteration
- *         while True:
+      /* "lsm.pyx":1685
+ *         if self.is_valid():
+ *             while True:
+ *                 yield self._value()             # <<<<<<<<<<<<<<
+ *                 try:
+ *                     if self._reverse:
  */
-  }
+      __pyx_t_2 = __pyx_f_3lsm_6Cursor__value(__pyx_cur_scope->__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1685, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_r = __pyx_t_2;
+      __pyx_t_2 = 0;
+      __Pyx_XGIVEREF(__pyx_r);
+      __Pyx_RefNannyFinishContext();
+      __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+      /* return from generator, yielding value */
+      __pyx_generator->resume_label = 1;
+      return __pyx_r;
+      __pyx_L7_resume_from_yield:;
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1685, __pyx_L1_error)
 
-  /* "lsm.pyx":1683
- *         if not self.is_valid():
- *             raise StopIteration
- *         while True:             # <<<<<<<<<<<<<<
- *             yield self._value()
- *             if self._reverse:
+      /* "lsm.pyx":1686
+ *             while True:
+ *                 yield self._value()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
  */
-  while (1) {
+      {
+        __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
+        __Pyx_XGOTREF(__pyx_t_3);
+        __Pyx_XGOTREF(__pyx_t_4);
+        __Pyx_XGOTREF(__pyx_t_5);
+        /*try:*/ {
 
-    /* "lsm.pyx":1684
- *             raise StopIteration
- *         while True:
- *             yield self._value()             # <<<<<<<<<<<<<<
- *             if self._reverse:
- *                 self.previous()
+          /* "lsm.pyx":1687
+ *                 yield self._value()
+ *                 try:
+ *                     if self._reverse:             # <<<<<<<<<<<<<<
+ *                         self.previous()
+ *                     else:
+ */
+          __pyx_t_1 = (__pyx_cur_scope->__pyx_v_self->_reverse != 0);
+          if (__pyx_t_1) {
+
+            /* "lsm.pyx":1688
+ *                 try:
+ *                     if self._reverse:
+ *                         self.previous()             # <<<<<<<<<<<<<<
+ *                     else:
+ *                         self.next()
  */
-    __pyx_t_2 = __pyx_f_3lsm_6Cursor__value(__pyx_cur_scope->__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1684, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
-    __Pyx_XGIVEREF(__pyx_r);
-    __Pyx_RefNannyFinishContext();
-    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-    /* return from generator, yielding value */
-    __pyx_generator->resume_label = 1;
-    return __pyx_r;
-    __pyx_L7_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1684, __pyx_L1_error)
+            __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->previous(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1688, __pyx_L8_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "lsm.pyx":1685
- *         while True:
- *             yield self._value()
- *             if self._reverse:             # <<<<<<<<<<<<<<
- *                 self.previous()
- *             else:
+            /* "lsm.pyx":1687
+ *                 yield self._value()
+ *                 try:
+ *                     if self._reverse:             # <<<<<<<<<<<<<<
+ *                         self.previous()
+ *                     else:
  */
-    __pyx_t_1 = (__pyx_cur_scope->__pyx_v_self->_reverse != 0);
-    if (__pyx_t_1) {
+            goto __pyx_L16;
+          }
 
-      /* "lsm.pyx":1686
- *             yield self._value()
- *             if self._reverse:
- *                 self.previous()             # <<<<<<<<<<<<<<
- *             else:
- *                 self.next()
+          /* "lsm.pyx":1690
+ *                         self.previous()
+ *                     else:
+ *                         self.next()             # <<<<<<<<<<<<<<
+ *                 except StopIteration:
+ *                     break
  */
-      __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->previous(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1686, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          /*else*/ {
+            __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->next(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1690, __pyx_L8_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          }
+          __pyx_L16:;
 
-      /* "lsm.pyx":1685
- *         while True:
- *             yield self._value()
- *             if self._reverse:             # <<<<<<<<<<<<<<
- *                 self.previous()
- *             else:
+          /* "lsm.pyx":1686
+ *             while True:
+ *                 yield self._value()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
  */
-      goto __pyx_L8;
-    }
+        }
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        goto __pyx_L15_try_end;
+        __pyx_L8_error:;
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "lsm.pyx":1688
- *                 self.previous()
- *             else:
- *                 self.next()             # <<<<<<<<<<<<<<
+        /* "lsm.pyx":1691
+ *                     else:
+ *                         self.next()
+ *                 except StopIteration:             # <<<<<<<<<<<<<<
+ *                     break
+ * 
+ */
+        __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
+        if (__pyx_t_6) {
+          __Pyx_AddTraceback("lsm.Cursor.values", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1691, __pyx_L10_except_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_GOTREF(__pyx_t_8);
+
+          /* "lsm.pyx":1692
+ *                         self.next()
+ *                 except StopIteration:
+ *                     break             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    /*else*/ {
-      __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_Cursor *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->next(__pyx_cur_scope->__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1688, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          goto __pyx_L17_except_break;
+          __pyx_L17_except_break:;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          goto __pyx_L13_try_break;
+        }
+        goto __pyx_L10_except_error;
+        __pyx_L10_except_error:;
+
+        /* "lsm.pyx":1686
+ *             while True:
+ *                 yield self._value()
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     if self._reverse:
+ *                         self.previous()
+ */
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_XGIVEREF(__pyx_t_5);
+        __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+        goto __pyx_L1_error;
+        __pyx_L13_try_break:;
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_XGIVEREF(__pyx_t_5);
+        __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+        goto __pyx_L6_break;
+        __pyx_L15_try_end:;
+      }
     }
-    __pyx_L8:;
+    __pyx_L6_break:;
+
+    /* "lsm.pyx":1683
+ *     def values(self):
+ *         """Return a generator that successively yields values."""
+ *         if self.is_valid():             # <<<<<<<<<<<<<<
+ *             while True:
+ *                 yield self._value()
+ */
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "lsm.pyx":1679
- *                 self.next()
+  /* "lsm.pyx":1681
+ *                     break
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         """Return a generator that successively yields values."""
- *         if not self.is_valid():
+ *         if self.is_valid():
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("values", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
@@ -16905,15 +17091,15 @@
   __Pyx_AddTraceback("lsm.Cursor.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1715
+/* "lsm.pyx":1719
  *     cdef LSM lsm
  * 
  *     def __cinit__(self, lsm):             # <<<<<<<<<<<<<<
  *         self.lsm = lsm
  * 
  */
 
@@ -16942,26 +17128,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lsm)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1715, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1719, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_lsm = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1715, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1719, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lsm.Transaction.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3lsm_11Transaction___cinit__(((struct __pyx_obj_3lsm_Transaction *)__pyx_v_self), __pyx_v_lsm);
 
@@ -16975,31 +17161,31 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "lsm.pyx":1716
+  /* "lsm.pyx":1720
  * 
  *     def __cinit__(self, lsm):
  *         self.lsm = lsm             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  if (!(likely(((__pyx_v_lsm) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_lsm, __pyx_ptype_3lsm_LSM))))) __PYX_ERR(0, 1716, __pyx_L1_error)
+  if (!(likely(((__pyx_v_lsm) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_lsm, __pyx_ptype_3lsm_LSM))))) __PYX_ERR(0, 1720, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_lsm;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->lsm);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->lsm));
   __pyx_v_self->lsm = ((struct __pyx_obj_3lsm_LSM *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1715
+  /* "lsm.pyx":1719
  *     cdef LSM lsm
  * 
  *     def __cinit__(self, lsm):             # <<<<<<<<<<<<<<
  *         self.lsm = lsm
  * 
  */
 
@@ -17011,15 +17197,15 @@
   __Pyx_AddTraceback("lsm.Transaction.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1718
+/* "lsm.pyx":1722
  *         self.lsm = lsm
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.lsm.begin()
  *         return self
  */
 
@@ -17041,38 +17227,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "lsm.pyx":1719
+  /* "lsm.pyx":1723
  * 
  *     def __enter__(self):
  *         self.lsm.begin()             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->begin(__pyx_v_self->lsm, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1719, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->begin(__pyx_v_self->lsm, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1720
+  /* "lsm.pyx":1724
  *     def __enter__(self):
  *         self.lsm.begin()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "lsm.pyx":1718
+  /* "lsm.pyx":1722
  *         self.lsm = lsm
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.lsm.begin()
  *         return self
  */
 
@@ -17083,15 +17269,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1722
+/* "lsm.pyx":1726
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         if exc_type:
  *             self.rollback(False)
  */
 
@@ -17128,40 +17314,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 1722, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 1726, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_tb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 1722, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 1726, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 1722, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 1726, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_exc_type = values[0];
     __pyx_v_exc_val = values[1];
     __pyx_v_exc_tb = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1722, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1726, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lsm.Transaction.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3lsm_11Transaction_4__exit__(((struct __pyx_obj_3lsm_Transaction *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_val, __pyx_v_exc_tb);
 
@@ -17182,61 +17368,61 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "lsm.pyx":1723
+  /* "lsm.pyx":1727
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:             # <<<<<<<<<<<<<<
  *             self.rollback(False)
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_exc_type); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1723, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_exc_type); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1727, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "lsm.pyx":1724
+    /* "lsm.pyx":1728
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:
  *             self.rollback(False)             # <<<<<<<<<<<<<<
  *         else:
  *             try:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_rollback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1724, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_rollback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1728, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, Py_False) : __Pyx_PyObject_CallOneArg(__pyx_t_3, Py_False);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1724, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1728, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "lsm.pyx":1723
+    /* "lsm.pyx":1727
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:             # <<<<<<<<<<<<<<
  *             self.rollback(False)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "lsm.pyx":1726
+  /* "lsm.pyx":1730
  *             self.rollback(False)
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.commit(False)
  *             except:
  */
   /*else*/ {
@@ -17245,41 +17431,41 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       /*try:*/ {
 
-        /* "lsm.pyx":1727
+        /* "lsm.pyx":1731
  *         else:
  *             try:
  *                 self.commit(False)             # <<<<<<<<<<<<<<
  *             except:
  *                 self.lsm._rollback(False)
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_commit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1727, __pyx_L4_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_commit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1731, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, Py_False) : __Pyx_PyObject_CallOneArg(__pyx_t_3, Py_False);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1727, __pyx_L4_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1731, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "lsm.pyx":1726
+        /* "lsm.pyx":1730
  *             self.rollback(False)
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.commit(False)
  *             except:
  */
       }
@@ -17288,54 +17474,54 @@
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "lsm.pyx":1728
+      /* "lsm.pyx":1732
  *             try:
  *                 self.commit(False)
  *             except:             # <<<<<<<<<<<<<<
  *                 self.lsm._rollback(False)
  *                 raise
  */
       /*except:*/ {
         __Pyx_AddTraceback("lsm.Transaction.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 1728, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 1732, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_4);
 
-        /* "lsm.pyx":1729
+        /* "lsm.pyx":1733
  *                 self.commit(False)
  *             except:
  *                 self.lsm._rollback(False)             # <<<<<<<<<<<<<<
  *                 raise
  * 
  */
-        __pyx_t_8 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_rollback(__pyx_v_self->lsm, 0); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 1729, __pyx_L6_except_error)
+        __pyx_t_8 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_rollback(__pyx_v_self->lsm, 0); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 1733, __pyx_L6_except_error)
 
-        /* "lsm.pyx":1730
+        /* "lsm.pyx":1734
  *             except:
  *                 self.lsm._rollback(False)
  *                 raise             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, fn):
  */
         __Pyx_GIVEREF(__pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_XGIVEREF(__pyx_t_4);
         __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_3, __pyx_t_4);
         __pyx_t_2 = 0; __pyx_t_3 = 0; __pyx_t_4 = 0; 
-        __PYX_ERR(0, 1730, __pyx_L6_except_error)
+        __PYX_ERR(0, 1734, __pyx_L6_except_error)
       }
       __pyx_L6_except_error:;
 
-      /* "lsm.pyx":1726
+      /* "lsm.pyx":1730
  *             self.rollback(False)
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.commit(False)
  *             except:
  */
       __Pyx_XGIVEREF(__pyx_t_5);
@@ -17344,15 +17530,15 @@
       __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
       goto __pyx_L1_error;
       __pyx_L9_try_end:;
     }
   }
   __pyx_L3:;
 
-  /* "lsm.pyx":1722
+  /* "lsm.pyx":1726
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         if exc_type:
  *             self.rollback(False)
  */
 
@@ -17367,15 +17553,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1732
+/* "lsm.pyx":1736
  *                 raise
  * 
  *     def __call__(self, fn):             # <<<<<<<<<<<<<<
  *         def inner(*args, **kwargs):
  *             with self:
  */
 
@@ -17404,39 +17590,39 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 1732, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 1736, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_fn = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1732, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1736, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lsm.Transaction.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3lsm_11Transaction_6__call__(((struct __pyx_obj_3lsm_Transaction *)__pyx_v_self), __pyx_v_fn);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1733
+/* "lsm.pyx":1737
  * 
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):             # <<<<<<<<<<<<<<
  *             with self:
  *                 return fn(*args, **kwargs)
  */
 
@@ -17482,107 +17668,107 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inner", 0);
   __pyx_outer_scope = (struct __pyx_obj_3lsm___pyx_scope_struct_10___call__ *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
-  /* "lsm.pyx":1734
+  /* "lsm.pyx":1738
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):
  *             with self:             # <<<<<<<<<<<<<<
  *                 return fn(*args, **kwargs)
  *         return inner
  */
   /*with:*/ {
-    if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 1734, __pyx_L1_error) }
-    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1734, __pyx_L1_error)
+    if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 1738, __pyx_L1_error) }
+    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1738, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1734, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1738, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1734, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1738, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         /*try:*/ {
 
-          /* "lsm.pyx":1735
+          /* "lsm.pyx":1739
  *         def inner(*args, **kwargs):
  *             with self:
  *                 return fn(*args, **kwargs)             # <<<<<<<<<<<<<<
  *         return inner
  * 
  */
           __Pyx_XDECREF(__pyx_r);
-          if (unlikely(!__pyx_cur_scope->__pyx_v_fn)) { __Pyx_RaiseClosureNameError("fn"); __PYX_ERR(0, 1735, __pyx_L7_error) }
-          __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1735, __pyx_L7_error)
+          if (unlikely(!__pyx_cur_scope->__pyx_v_fn)) { __Pyx_RaiseClosureNameError("fn"); __PYX_ERR(0, 1739, __pyx_L7_error) }
+          __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1739, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_cur_scope->__pyx_v_fn, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1735, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_cur_scope->__pyx_v_fn, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1739, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_r = __pyx_t_3;
           __pyx_t_3 = 0;
           goto __pyx_L11_try_return;
 
-          /* "lsm.pyx":1734
+          /* "lsm.pyx":1738
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):
  *             with self:             # <<<<<<<<<<<<<<
  *                 return fn(*args, **kwargs)
  *         return inner
  */
         }
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("lsm.Transaction.__call__.inner", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 1734, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 1738, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_8 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1734, __pyx_L9_except_error)
+          __pyx_t_8 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1738, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_8);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1734, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1738, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 1734, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 1738, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_4);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_2, __pyx_t_4);
             __pyx_t_3 = 0; __pyx_t_2 = 0; __pyx_t_4 = 0; 
-            __PYX_ERR(0, 1734, __pyx_L9_except_error)
+            __PYX_ERR(0, 1738, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -17605,27 +17791,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_1) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1734, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1738, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_7 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_1) {
           __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1734, __pyx_L1_error)
+          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1738, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __pyx_r = __pyx_t_7;
         __pyx_t_7 = 0;
         goto __pyx_L0;
       }
@@ -17634,15 +17820,15 @@
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "lsm.pyx":1733
+  /* "lsm.pyx":1737
  * 
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):             # <<<<<<<<<<<<<<
  *             with self:
  *                 return fn(*args, **kwargs)
  */
 
@@ -17658,15 +17844,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1732
+/* "lsm.pyx":1736
  *                 raise
  * 
  *     def __call__(self, fn):             # <<<<<<<<<<<<<<
  *         def inner(*args, **kwargs):
  *             with self:
  */
 
@@ -17680,50 +17866,50 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
   __pyx_cur_scope = (struct __pyx_obj_3lsm___pyx_scope_struct_10___call__ *)__pyx_tp_new_3lsm___pyx_scope_struct_10___call__(__pyx_ptype_3lsm___pyx_scope_struct_10___call__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_3lsm___pyx_scope_struct_10___call__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 1732, __pyx_L1_error)
+    __PYX_ERR(0, 1736, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_fn = __pyx_v_fn;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_fn);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_fn);
 
-  /* "lsm.pyx":1733
+  /* "lsm.pyx":1737
  * 
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):             # <<<<<<<<<<<<<<
  *             with self:
  *                 return fn(*args, **kwargs)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_3lsm_11Transaction_8__call___1inner, 0, __pyx_n_s_call___locals_inner, ((PyObject*)__pyx_cur_scope), __pyx_n_s_lsm, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1733, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_3lsm_11Transaction_8__call___1inner, 0, __pyx_n_s_call___locals_inner, ((PyObject*)__pyx_cur_scope), __pyx_n_s_lsm, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1737, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_inner = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1736
+  /* "lsm.pyx":1740
  *             with self:
  *                 return fn(*args, **kwargs)
  *         return inner             # <<<<<<<<<<<<<<
  * 
  *     def commit(self, begin=True):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_inner);
   __pyx_r = __pyx_v_inner;
   goto __pyx_L0;
 
-  /* "lsm.pyx":1732
+  /* "lsm.pyx":1736
  *                 raise
  * 
  *     def __call__(self, fn):             # <<<<<<<<<<<<<<
  *         def inner(*args, **kwargs):
  *             with self:
  */
 
@@ -17736,15 +17922,15 @@
   __Pyx_XDECREF(__pyx_v_inner);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1738
+/* "lsm.pyx":1742
  *         return inner
  * 
  *     def commit(self, begin=True):             # <<<<<<<<<<<<<<
  *         """
  *         Commit the transaction and optionally open a new transaction.
  */
 
@@ -17777,29 +17963,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_begin);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "commit") < 0)) __PYX_ERR(0, 1738, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "commit") < 0)) __PYX_ERR(0, 1742, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_begin = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("commit", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1738, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("commit", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1742, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lsm.Transaction.commit", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3lsm_11Transaction_8commit(((struct __pyx_obj_3lsm_Transaction *)__pyx_v_self), __pyx_v_begin);
 
@@ -17816,69 +18002,69 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("commit", 0);
 
-  /* "lsm.pyx":1746
+  /* "lsm.pyx":1750
  *         """
  *         cdef int rc
  *         rc = self.lsm._commit()             # <<<<<<<<<<<<<<
  *         if begin:
  *             self.lsm.begin()
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_commit(__pyx_v_self->lsm); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1746, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_commit(__pyx_v_self->lsm); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1750, __pyx_L1_error)
   __pyx_v_rc = __pyx_t_1;
 
-  /* "lsm.pyx":1747
+  /* "lsm.pyx":1751
  *         cdef int rc
  *         rc = self.lsm._commit()
  *         if begin:             # <<<<<<<<<<<<<<
  *             self.lsm.begin()
  *         return rc
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_begin); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1747, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_begin); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1751, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "lsm.pyx":1748
+    /* "lsm.pyx":1752
  *         rc = self.lsm._commit()
  *         if begin:
  *             self.lsm.begin()             # <<<<<<<<<<<<<<
  *         return rc
  * 
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->begin(__pyx_v_self->lsm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1748, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->begin(__pyx_v_self->lsm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1752, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "lsm.pyx":1747
+    /* "lsm.pyx":1751
  *         cdef int rc
  *         rc = self.lsm._commit()
  *         if begin:             # <<<<<<<<<<<<<<
  *             self.lsm.begin()
  *         return rc
  */
   }
 
-  /* "lsm.pyx":1749
+  /* "lsm.pyx":1753
  *         if begin:
  *             self.lsm.begin()
  *         return rc             # <<<<<<<<<<<<<<
  * 
  *     def rollback(self, begin=True):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1749, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "lsm.pyx":1738
+  /* "lsm.pyx":1742
  *         return inner
  * 
  *     def commit(self, begin=True):             # <<<<<<<<<<<<<<
  *         """
  *         Commit the transaction and optionally open a new transaction.
  */
 
@@ -17889,15 +18075,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "lsm.pyx":1751
+/* "lsm.pyx":1755
  *         return rc
  * 
  *     def rollback(self, begin=True):             # <<<<<<<<<<<<<<
  *         """
  *         Rollback the transaction and optionally retain the open transaction.
  */
 
@@ -17930,29 +18116,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_begin);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "rollback") < 0)) __PYX_ERR(0, 1751, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "rollback") < 0)) __PYX_ERR(0, 1755, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_begin = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("rollback", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1751, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("rollback", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1755, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lsm.Transaction.rollback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3lsm_11Transaction_10rollback(((struct __pyx_obj_3lsm_Transaction *)__pyx_v_self), __pyx_v_begin);
 
@@ -17968,31 +18154,31 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("rollback", 0);
 
-  /* "lsm.pyx":1758
+  /* "lsm.pyx":1762
  *         transactional behavior for the rest of the block.
  *         """
  *         return self.lsm._rollback(keep_transaction=begin)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_begin); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1758, __pyx_L1_error)
-  __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_rollback(__pyx_v_self->lsm, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 1758, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1758, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_begin); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1762, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_3lsm_LSM *)__pyx_v_self->lsm->__pyx_vtab)->_rollback(__pyx_v_self->lsm, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 1762, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1762, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "lsm.pyx":1751
+  /* "lsm.pyx":1755
  *         return rc
  * 
  *     def rollback(self, begin=True):             # <<<<<<<<<<<<<<
  *         """
  *         Rollback the transaction and optionally retain the open transaction.
  */
 
@@ -18141,15 +18327,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3lsm_LSM(PyObject *o) {
   struct __pyx_obj_3lsm_LSM *p = (struct __pyx_obj_3lsm_LSM *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18338,15 +18524,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_3lsm_Cursor __pyx_vtable_3lsm_Cursor;
 
 static PyObject *__pyx_tp_new_3lsm_Cursor(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_3lsm_Cursor *p;
@@ -18366,15 +18552,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3lsm_Cursor(PyObject *o) {
   struct __pyx_obj_3lsm_Cursor *p = (struct __pyx_obj_3lsm_Cursor *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18503,15 +18689,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_3lsm_Transaction(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_3lsm_Transaction *p;
   PyObject *o;
@@ -18529,15 +18715,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3lsm_Transaction(PyObject *o) {
   struct __pyx_obj_3lsm_Transaction *p = (struct __pyx_obj_3lsm_Transaction *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->lsm);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18633,15 +18819,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct__option *__pyx_freelist_3lsm___pyx_scope_struct__option[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct__option = 0;
 
@@ -18772,15 +18958,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_1_fetch_range *__pyx_freelist_3lsm___pyx_scope_struct_1_fetch_range[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_1_fetch_range = 0;
 
@@ -18905,15 +19091,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_2___iter__ *__pyx_freelist_3lsm___pyx_scope_struct_2___iter__[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_2___iter__ = 0;
 
@@ -19042,15 +19228,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_3___reversed__ *__pyx_freelist_3lsm___pyx_scope_struct_3___reversed__[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_3___reversed__ = 0;
 
@@ -19179,15 +19365,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_4_keys *__pyx_freelist_3lsm___pyx_scope_struct_4_keys[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_4_keys = 0;
 
@@ -19320,15 +19506,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_5_values *__pyx_freelist_3lsm___pyx_scope_struct_5_values[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_5_values = 0;
 
@@ -19461,15 +19647,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_6_fetch_until *__pyx_freelist_3lsm___pyx_scope_struct_6_fetch_until[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_6_fetch_until = 0;
 
@@ -19574,15 +19760,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_7_fetch_range *__pyx_freelist_3lsm___pyx_scope_struct_7_fetch_range[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_7_fetch_range = 0;
 
@@ -19711,15 +19897,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_8_keys *__pyx_freelist_3lsm___pyx_scope_struct_8_keys[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_8_keys = 0;
 
@@ -19820,15 +20006,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_9_values *__pyx_freelist_3lsm___pyx_scope_struct_9_values[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_9_values = 0;
 
@@ -19929,15 +20115,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3lsm___pyx_scope_struct_10___call__ *__pyx_freelist_3lsm___pyx_scope_struct_10___call__[8];
 static int __pyx_freecount_3lsm___pyx_scope_struct_10___call__ = 0;
 
@@ -20054,15 +20240,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -20409,25 +20595,25 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "lsm.pyx":1733
+  /* "lsm.pyx":1737
  * 
  *     def __call__(self, fn):
  *         def inner(*args, **kwargs):             # <<<<<<<<<<<<<<
  *             with self:
  *                 return fn(*args, **kwargs)
  */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1733, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1737, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lsm_pyx, __pyx_n_s_inner, 1733, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1733, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lsm_pyx, __pyx_n_s_inner, 1737, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1737, __pyx_L1_error)
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -20460,15 +20646,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -20635,23 +20821,23 @@
     }
   }
   #endif
   if (__Pyx_SetVtable(__pyx_type_3lsm_Cursor.tp_dict, __pyx_vtabptr_3lsm_Cursor) < 0) __PYX_ERR(0, 1355, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Cursor, (PyObject *)&__pyx_type_3lsm_Cursor) < 0) __PYX_ERR(0, 1355, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_3lsm_Cursor) < 0) __PYX_ERR(0, 1355, __pyx_L1_error)
   __pyx_ptype_3lsm_Cursor = &__pyx_type_3lsm_Cursor;
-  if (PyType_Ready(&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1691, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1695, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3lsm_Transaction.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3lsm_Transaction.tp_dictoffset && __pyx_type_3lsm_Transaction.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3lsm_Transaction.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Transaction, (PyObject *)&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1691, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1691, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Transaction, (PyObject *)&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1695, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_3lsm_Transaction) < 0) __PYX_ERR(0, 1695, __pyx_L1_error)
   __pyx_ptype_3lsm_Transaction = &__pyx_type_3lsm_Transaction;
   if (PyType_Ready(&__pyx_type_3lsm___pyx_scope_struct__option) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3lsm___pyx_scope_struct__option.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3lsm___pyx_scope_struct__option.tp_dictoffset && __pyx_type_3lsm___pyx_scope_struct__option.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3lsm___pyx_scope_struct__option.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -20717,23 +20903,23 @@
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3lsm___pyx_scope_struct_8_keys.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3lsm___pyx_scope_struct_8_keys.tp_dictoffset && __pyx_type_3lsm___pyx_scope_struct_8_keys.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3lsm___pyx_scope_struct_8_keys.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_3lsm___pyx_scope_struct_8_keys = &__pyx_type_3lsm___pyx_scope_struct_8_keys;
-  if (PyType_Ready(&__pyx_type_3lsm___pyx_scope_struct_9_values) < 0) __PYX_ERR(0, 1679, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3lsm___pyx_scope_struct_9_values) < 0) __PYX_ERR(0, 1681, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3lsm___pyx_scope_struct_9_values.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3lsm___pyx_scope_struct_9_values.tp_dictoffset && __pyx_type_3lsm___pyx_scope_struct_9_values.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3lsm___pyx_scope_struct_9_values.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_3lsm___pyx_scope_struct_9_values = &__pyx_type_3lsm___pyx_scope_struct_9_values;
-  if (PyType_Ready(&__pyx_type_3lsm___pyx_scope_struct_10___call__) < 0) __PYX_ERR(0, 1732, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3lsm___pyx_scope_struct_10___call__) < 0) __PYX_ERR(0, 1736, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3lsm___pyx_scope_struct_10___call__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3lsm___pyx_scope_struct_10___call__.tp_dictoffset && __pyx_type_3lsm___pyx_scope_struct_10___call__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3lsm___pyx_scope_struct_10___call__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_3lsm___pyx_scope_struct_10___call__ = &__pyx_type_3lsm___pyx_scope_struct_10___call__;
@@ -20750,22 +20936,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20962,15 +21147,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_lsm) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22112,95 +22297,95 @@
  *     cpdef seek(self, key, int method=LSM_SEEK_EQ):             # <<<<<<<<<<<<<<
  *         """
  *         Seek to the given key using the specified matching method. If the
  */
   __pyx_k__15 = LSM_SEEK_EQ;
   __pyx_k__15 = LSM_SEEK_EQ;
 
-  /* "lsm.pyx":1761
+  /* "lsm.pyx":1765
  * 
  * 
  * SAFETY_OFF = LSM_SAFETY_OFF             # <<<<<<<<<<<<<<
  * SAFETY_NORMAL = LSM_SAFETY_NORMAL
  * SAFETY_FULL = LSM_SAFETY_FULL
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_OFF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1761, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_OFF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1765, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_OFF, __pyx_t_1) < 0) __PYX_ERR(0, 1761, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_OFF, __pyx_t_1) < 0) __PYX_ERR(0, 1765, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1762
+  /* "lsm.pyx":1766
  * 
  * SAFETY_OFF = LSM_SAFETY_OFF
  * SAFETY_NORMAL = LSM_SAFETY_NORMAL             # <<<<<<<<<<<<<<
  * SAFETY_FULL = LSM_SAFETY_FULL
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_NORMAL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1762, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_NORMAL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1766, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_NORMAL, __pyx_t_1) < 0) __PYX_ERR(0, 1762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_NORMAL, __pyx_t_1) < 0) __PYX_ERR(0, 1766, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1763
+  /* "lsm.pyx":1767
  * SAFETY_OFF = LSM_SAFETY_OFF
  * SAFETY_NORMAL = LSM_SAFETY_NORMAL
  * SAFETY_FULL = LSM_SAFETY_FULL             # <<<<<<<<<<<<<<
  * 
  * SEEK_LEFAST = LSM_SEEK_LEFAST
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_FULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1763, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SAFETY_FULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_FULL, __pyx_t_1) < 0) __PYX_ERR(0, 1763, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SAFETY_FULL, __pyx_t_1) < 0) __PYX_ERR(0, 1767, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1765
+  /* "lsm.pyx":1769
  * SAFETY_FULL = LSM_SAFETY_FULL
  * 
  * SEEK_LEFAST = LSM_SEEK_LEFAST             # <<<<<<<<<<<<<<
  * SEEK_LE = LSM_SEEK_LE
  * SEEK_EQ = LSM_SEEK_EQ
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_LEFAST); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1765, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_LEFAST); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_LEFAST, __pyx_t_1) < 0) __PYX_ERR(0, 1765, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_LEFAST, __pyx_t_1) < 0) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1766
+  /* "lsm.pyx":1770
  * 
  * SEEK_LEFAST = LSM_SEEK_LEFAST
  * SEEK_LE = LSM_SEEK_LE             # <<<<<<<<<<<<<<
  * SEEK_EQ = LSM_SEEK_EQ
  * SEEK_GE = LSM_SEEK_GE
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_LE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1766, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_LE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1770, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_LE, __pyx_t_1) < 0) __PYX_ERR(0, 1766, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_LE, __pyx_t_1) < 0) __PYX_ERR(0, 1770, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1767
+  /* "lsm.pyx":1771
  * SEEK_LEFAST = LSM_SEEK_LEFAST
  * SEEK_LE = LSM_SEEK_LE
  * SEEK_EQ = LSM_SEEK_EQ             # <<<<<<<<<<<<<<
  * SEEK_GE = LSM_SEEK_GE
  * """ADD: # cython: profile=True to top of file to use with cProfile."""
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_EQ); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1767, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_EQ); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1771, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_EQ, __pyx_t_1) < 0) __PYX_ERR(0, 1767, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_EQ, __pyx_t_1) < 0) __PYX_ERR(0, 1771, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "lsm.pyx":1768
+  /* "lsm.pyx":1772
  * SEEK_LE = LSM_SEEK_LE
  * SEEK_EQ = LSM_SEEK_EQ
  * SEEK_GE = LSM_SEEK_GE             # <<<<<<<<<<<<<<
  * """ADD: # cython: profile=True to top of file to use with cProfile."""
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_GE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1768, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LSM_SEEK_GE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_GE, __pyx_t_1) < 0) __PYX_ERR(0, 1768, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SEEK_GE, __pyx_t_1) < 0) __PYX_ERR(0, 1772, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "lsm.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * from cpython.bytes cimport PyBytes_AsStringAndSize
  * from cpython.bytes cimport PyBytes_Check
  */
@@ -22755,28 +22940,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22805,19 +22990,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -23639,17 +23824,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -23716,15 +23906,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -23876,15 +24069,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -24056,18 +24249,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
@@ -24254,17 +24445,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -24594,15 +24783,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -24828,61 +25017,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
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
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -25036,15 +25243,15 @@
     }
     return (
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -25421,15 +25628,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25617,15 +25824,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26851,15 +27058,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `lsm-db-0.7.0/lsm.pyx` & `lsm-db-0.7.1/lsm.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1632,15 +1632,15 @@
                 self.last()
             else:
                 self.first()
         else:
             try:
                 self.seek(start, seek_method)
             except KeyError:
-                raise StopIteration
+                return
 
         for key, value in self.fetch_until(end):
             yield (key, value)
 
     cdef inline _key(self):
         """Return the key at the cursor's current position."""
         cdef:
@@ -1663,33 +1663,37 @@
         return self._key()
 
     def value(self):
         return self._value()
 
     def keys(self):
         """Return a generator that successively yields keys."""
-        if not self.is_valid():
-            raise StopIteration
-        while True:
-            yield self._key()
-            if self._reverse:
-                self.previous()
-            else:
-                self.next()
+        if self.is_valid():
+            while True:
+                yield self._key()
+                try:
+                    if self._reverse:
+                        self.previous()
+                    else:
+                        self.next()
+                except StopIteration:
+                    break
 
     def values(self):
         """Return a generator that successively yields values."""
-        if not self.is_valid():
-            raise StopIteration
-        while True:
-            yield self._value()
-            if self._reverse:
-                self.previous()
-            else:
-                self.next()
+        if self.is_valid():
+            while True:
+                yield self._value()
+                try:
+                    if self._reverse:
+                        self.previous()
+                    else:
+                        self.next()
+                except StopIteration:
+                    break
 
 
 cdef class Transaction(object):
     """
     Context manager and decorator to run the wrapped block in a transaction.
     LSM supports nested transactions, so the context manager/decorator can be
     mixed and matched and nested arbitrarily.
```

### Comparing `lsm-db-0.7.0/lsm_db.egg-info/SOURCES.txt` & `lsm-db-0.7.1/lsm_db.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 lsm.c
 lsm.pyx
+pyproject.toml
 setup.py
 tests.py
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/installation.rst
```

### Comparing `lsm-db-0.7.0/setup.py` & `lsm-db-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 library_source = glob.glob('src/*.c')
 lsm_extension = Extension(
     'lsm',
     sources=[python_source] + library_source)
 
 setup(
     name='lsm-db',
-    version='0.7.0',
+    version='0.7.1',
     description='Python bindings for the SQLite4 LSM database.',
     author='Charles Leifer',
     author_email='',
     ext_modules=cythonize([lsm_extension]),
 )
```

### Comparing `lsm-db-0.7.0/src/lsm.h` & `lsm-db-0.7.1/src/lsm.h`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsmInt.h` & `lsm-db-0.7.1/src/lsmInt.h`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_ckpt.c` & `lsm-db-0.7.1/src/lsm_ckpt.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_file.c` & `lsm-db-0.7.1/src/lsm_file.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_log.c` & `lsm-db-0.7.1/src/lsm_log.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_main.c` & `lsm-db-0.7.1/src/lsm_main.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_mem.c` & `lsm-db-0.7.1/src/lsm_mem.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_mutex.c` & `lsm-db-0.7.1/src/lsm_mutex.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_shared.c` & `lsm-db-0.7.1/src/lsm_shared.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_sorted.c` & `lsm-db-0.7.1/src/lsm_sorted.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_str.c` & `lsm-db-0.7.1/src/lsm_str.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_tree.c` & `lsm-db-0.7.1/src/lsm_tree.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_unix.c` & `lsm-db-0.7.1/src/lsm_unix.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_varint.c` & `lsm-db-0.7.1/src/lsm_varint.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/src/lsm_win32.c` & `lsm-db-0.7.1/src/lsm_win32.c`

 * *Files identical despite different names*

### Comparing `lsm-db-0.7.0/tests.py` & `lsm-db-0.7.1/tests.py`

 * *Files identical despite different names*

