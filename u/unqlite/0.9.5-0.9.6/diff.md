# Comparing `tmp/unqlite-0.9.5.tar.gz` & `tmp/unqlite-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unqlite-0.9.5.tar", last modified: Sat Jul 15 17:52:29 2023, max compression
+gzip compressed data, was "dist/unqlite-0.9.6.tar", last modified: Tue Jul 18 22:20:44 2023, max compression
```

## Comparing `unqlite-0.9.5.tar` & `unqlite-0.9.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:48.000000 unqlite-0.9.5/LICENSE
--rw-rw-r--   0 charles   (1000) charles   (1000)      211 2018-08-16 18:40:48.000000 unqlite-0.9.5/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-15 17:52:29.000000 unqlite-0.9.5/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     7663 2020-12-07 15:43:34.000000 unqlite-0.9.5/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/docs/
--rw-rw-r--   0 charles   (1000) charles   (1000)     6794 2018-08-16 18:40:48.000000 unqlite-0.9.5/docs/Makefile
--rw-rw-r--   0 charles   (1000) charles   (1000)    29341 2020-11-26 04:00:08.000000 unqlite-0.9.5/docs/api.rst
--rw-r--r--   0 charles   (1000) charles   (1000)     8007 2021-11-25 17:03:21.000000 unqlite-0.9.5/docs/conf.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1837 2020-12-07 15:45:12.000000 unqlite-0.9.5/docs/index.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)      815 2018-08-16 18:40:48.000000 unqlite-0.9.5/docs/installation.rst
--rw-rw-r--   0 charles   (1000) charles   (1000)     6726 2020-03-06 23:33:53.000000 unqlite-0.9.5/docs/quickstart.rst
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-15 17:52:29.000000 unqlite-0.9.5/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     2183 2023-07-15 17:52:13.000000 unqlite-0.9.5/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/src/
--rw-r--r--   0 charles   (1000) charles   (1000)  1955368 2023-07-15 17:44:05.000000 unqlite-0.9.5/src/unqlite.c
--rw-r--r--   0 charles   (1000) charles   (1000)    48708 2021-11-25 17:03:21.000000 unqlite-0.9.5/src/unqlite.h
--rw-rw-r--   0 charles   (1000) charles   (1000)    24398 2022-04-26 15:29:11.000000 unqlite-0.9.5/tests.py
--rw-r--r--   0 charles   (1000) charles   (1000)  1353651 2023-07-15 17:51:37.000000 unqlite-0.9.5/unqlite.c
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      348 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        7 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        8 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)    45550 2023-07-15 17:51:34.000000 unqlite-0.9.5/unqlite.pyx
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:20:44.000000 unqlite-0.9.6/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:48.000000 unqlite-0.9.6/LICENSE
+-rw-r--r--   0 charles   (1000) charles   (1000)      211 2018-08-16 18:40:48.000000 unqlite-0.9.6/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-18 22:20:44.000000 unqlite-0.9.6/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     7663 2020-12-07 15:43:34.000000 unqlite-0.9.6/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:20:44.000000 unqlite-0.9.6/docs/
+-rw-r--r--   0 charles   (1000) charles   (1000)     6794 2018-08-16 18:40:48.000000 unqlite-0.9.6/docs/Makefile
+-rw-r--r--   0 charles   (1000) charles   (1000)    29341 2020-11-26 04:00:08.000000 unqlite-0.9.6/docs/api.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)     8007 2021-11-25 17:03:21.000000 unqlite-0.9.6/docs/conf.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     1837 2020-12-07 15:45:12.000000 unqlite-0.9.6/docs/index.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)      815 2018-08-16 18:40:48.000000 unqlite-0.9.6/docs/installation.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)     6726 2020-03-06 23:33:53.000000 unqlite-0.9.6/docs/quickstart.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-18 22:20:44.000000 unqlite-0.9.6/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     2183 2023-07-18 22:20:04.000000 unqlite-0.9.6/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:20:44.000000 unqlite-0.9.6/src/
+-rw-r--r--   0 charles   (1000) charles   (1000)  1955368 2023-07-13 03:08:42.000000 unqlite-0.9.6/src/unqlite.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    48708 2023-07-13 03:08:42.000000 unqlite-0.9.6/src/unqlite.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    24398 2022-04-27 16:51:36.000000 unqlite-0.9.6/tests.py
+-rw-r--r--   0 charles   (1000) charles   (1000)  1359880 2023-07-18 22:20:13.000000 unqlite-0.9.6/unqlite.c
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      348 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        7 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        8 2023-07-18 22:20:44.000000 unqlite-0.9.6/unqlite.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)    45655 2023-07-18 22:20:04.000000 unqlite-0.9.6/unqlite.pyx
```

### Comparing `unqlite-0.9.5/LICENSE` & `unqlite-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/PKG-INFO` & `unqlite-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unqlite
-Version: 0.9.5
+Version: 0.9.6
 Summary: Fast Python bindings for the UnQLite embedded NoSQL database.
 Home-page: https://github.com/coleifer/unqlite-python
 Author: Charles Leifer
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `unqlite-0.9.5/README.md` & `unqlite-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/Makefile` & `unqlite-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/api.rst` & `unqlite-0.9.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/conf.py` & `unqlite-0.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/index.rst` & `unqlite-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/installation.rst` & `unqlite-0.9.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/docs/quickstart.rst` & `unqlite-0.9.6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/setup.py` & `unqlite-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'unqlite',
     define_macros=[('UNQLITE_ENABLE_THREADS', '1')],
     libraries=libs,
     sources=[python_source] + library_source)
 
 setup(
     name='unqlite',
-    version='0.9.5',
+    version='0.9.6',
     description='Fast Python bindings for the UnQLite embedded NoSQL database.',
     author='Charles Leifer',
     author_email='',
     url='https://github.com/coleifer/unqlite-python',
     license='MIT',
     install_requires=['Cython'],
     setup_requires=['cython'],
```

### Comparing `unqlite-0.9.5/src/unqlite.c` & `unqlite-0.9.6/src/unqlite.c`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/src/unqlite.h` & `unqlite-0.9.6/src/unqlite.h`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/tests.py` & `unqlite-0.9.6/tests.py`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.5/unqlite.c` & `unqlite-0.9.6/unqlite.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "UNQLITE_ENABLE_THREADS",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -99,18 +99,22 @@
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
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -386,17 +390,14 @@
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
@@ -466,14 +467,19 @@
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
@@ -996,30 +1002,30 @@
 struct __pyx_obj_7unqlite___pyx_scope_struct_1_keys;
 struct __pyx_obj_7unqlite___pyx_scope_struct_2_values;
 struct __pyx_obj_7unqlite___pyx_scope_struct_3_items;
 struct __pyx_obj_7unqlite___pyx_scope_struct_4_range;
 struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until;
 struct __pyx_opt_args_7unqlite_6Cursor_seek;
 
-/* "unqlite.pyx":717
+/* "unqlite.pyx":720
  *         unqlite_kv_cursor_reset(self.cursor)
  * 
  *     cpdef seek(self, key, int flags=UNQLITE_CURSOR_MATCH_EXACT):             # <<<<<<<<<<<<<<
  *         """
  *         Seek to the given key. The flags specify how UnQLite will determine
  */
 struct __pyx_opt_args_7unqlite_6Cursor_seek {
   int __pyx_n;
   int flags;
 };
 
-/* "unqlite.pyx":845
+/* "unqlite.pyx":848
  * 
  * # Foreign function callback signature.
- * ctypedef int (*unqlite_filter_fn)(unqlite_context *, int, unqlite_value **)             # <<<<<<<<<<<<<<
+ * ctypedef int (*unqlite_filter_fn)(unqlite_context *, int, unqlite_value **) noexcept             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef int (*__pyx_t_7unqlite_unqlite_filter_fn)(unqlite_context *, int, unqlite_value **);
 
 /* "unqlite.pyx":325
  * 
@@ -1037,28 +1043,28 @@
   PyObject *filename;
   PyObject *encoded_filename;
   int flags;
   int open_database;
 };
 
 
-/* "unqlite.pyx":670
+/* "unqlite.pyx":673
  * 
  * 
  * cdef class Transaction(object):             # <<<<<<<<<<<<<<
  *     """Expose transaction as a context manager."""
  *     cdef UnQLite unqlite
  */
 struct __pyx_obj_7unqlite_Transaction {
   PyObject_HEAD
   struct __pyx_obj_7unqlite_UnQLite *unqlite;
 };
 
 
-/* "unqlite.pyx":692
+/* "unqlite.pyx":695
  * 
  * 
  * cdef class Cursor(object):             # <<<<<<<<<<<<<<
  *     """Cursor interface for efficiently iterating through database."""
  *     cdef UnQLite unqlite
  */
 struct __pyx_obj_7unqlite_Cursor {
@@ -1066,15 +1072,15 @@
   struct __pyx_vtabstruct_7unqlite_Cursor *__pyx_vtab;
   struct __pyx_obj_7unqlite_UnQLite *unqlite;
   struct unqlite_kv_cursor *cursor;
   int consumed;
 };
 
 
-/* "unqlite.pyx":848
+/* "unqlite.pyx":851
  * 
  * 
  * cdef class VM(object):             # <<<<<<<<<<<<<<
  *     """Jx9 virtual-machine interface."""
  *     cdef UnQLite unqlite
  */
 struct __pyx_obj_7unqlite_VM {
@@ -1085,44 +1091,44 @@
   int need_reset;
   PyObject *code;
   PyObject *encoded_code;
   PyObject *encoded_names;
 };
 
 
-/* "unqlite.pyx":977
+/* "unqlite.pyx":980
  * 
  * 
  * cdef class Context(object):             # <<<<<<<<<<<<<<
  *     cdef unqlite_context *context
  * 
  */
 struct __pyx_obj_7unqlite_Context {
   PyObject_HEAD
   struct __pyx_vtabstruct_7unqlite_Context *__pyx_vtab;
   unqlite_context *context;
 };
 
 
-/* "unqlite.pyx":1067
+/* "unqlite.pyx":1070
  * 
  * 
  * cdef class Collection(object):             # <<<<<<<<<<<<<<
  *     """
  *     Manage collections of UnQLite JSON documents.
  */
 struct __pyx_obj_7unqlite_Collection {
   PyObject_HEAD
   struct __pyx_vtabstruct_7unqlite_Collection *__pyx_vtab;
   struct __pyx_obj_7unqlite_UnQLite *unqlite;
   PyObject *name;
 };
 
 
-/* "unqlite.pyx":1225
+/* "unqlite.pyx":1228
  * 
  * 
  * cdef class CollectionIterator(object):             # <<<<<<<<<<<<<<
  *     cdef:
  *         VM vm
  */
 struct __pyx_obj_7unqlite_CollectionIterator {
@@ -1221,20 +1227,23 @@
   PyObject *__pyx_v_item;
   struct __pyx_obj_7unqlite_UnQLite *__pyx_v_self;
   PyObject *__pyx_v_start_key;
   PyObject *__pyx_t_0;
   PyObject *__pyx_t_1;
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  PyObject *(*__pyx_t_5)(PyObject *);
+  PyObject *__pyx_t_4;
+  PyObject *__pyx_t_5;
+  PyObject *__pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *(*__pyx_t_8)(PyObject *);
 };
 
 
-/* "unqlite.pyx":834
+/* "unqlite.pyx":837
  *         return (key, value)
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):             # <<<<<<<<<<<<<<
  *         for key, value in self:
  *             if key == stop_key:
  */
 struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until {
@@ -1275,15 +1284,15 @@
   PyObject *(*update)(struct __pyx_obj_7unqlite_UnQLite *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*random_string)(struct __pyx_obj_7unqlite_UnQLite *, int, int __pyx_skip_dispatch);
   int (*random_int)(struct __pyx_obj_7unqlite_UnQLite *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_7unqlite_UnQLite *__pyx_vtabptr_7unqlite_UnQLite;
 
 
-/* "unqlite.pyx":692
+/* "unqlite.pyx":695
  * 
  * 
  * cdef class Cursor(object):             # <<<<<<<<<<<<<<
  *     """Cursor interface for efficiently iterating through database."""
  *     cdef UnQLite unqlite
  */
 
@@ -1298,15 +1307,15 @@
   PyObject *(*key)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch);
   PyObject *(*value)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch);
   PyObject *(*delete)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_7unqlite_Cursor *__pyx_vtabptr_7unqlite_Cursor;
 
 
-/* "unqlite.pyx":848
+/* "unqlite.pyx":851
  * 
  * 
  * cdef class VM(object):             # <<<<<<<<<<<<<<
  *     """Jx9 virtual-machine interface."""
  *     cdef UnQLite unqlite
  */
 
@@ -1320,15 +1329,15 @@
   unqlite_value *(*create_array)(struct __pyx_obj_7unqlite_VM *);
   unqlite_value *(*create_scalar)(struct __pyx_obj_7unqlite_VM *);
   PyObject *(*set_values)(struct __pyx_obj_7unqlite_VM *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_7unqlite_VM *__pyx_vtabptr_7unqlite_VM;
 
 
-/* "unqlite.pyx":977
+/* "unqlite.pyx":980
  * 
  * 
  * cdef class Context(object):             # <<<<<<<<<<<<<<
  *     cdef unqlite_context *context
  * 
  */
 
@@ -1340,15 +1349,15 @@
   unqlite_value *(*create_scalar)(struct __pyx_obj_7unqlite_Context *);
   PyObject *(*push_result)(struct __pyx_obj_7unqlite_Context *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*python_to_unqlite_value)(struct __pyx_obj_7unqlite_Context *, unqlite_value *, PyObject *);
 };
 static struct __pyx_vtabstruct_7unqlite_Context *__pyx_vtabptr_7unqlite_Context;
 
 
-/* "unqlite.pyx":1067
+/* "unqlite.pyx":1070
  * 
  * 
  * cdef class Collection(object):             # <<<<<<<<<<<<<<
  *     """
  *     Manage collections of UnQLite JSON documents.
  */
 
@@ -1952,30 +1961,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
@@ -9432,26 +9441,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
+  PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
-  Py_ssize_t __pyx_t_10;
-  PyObject *(*__pyx_t_11)(PyObject *);
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  Py_ssize_t __pyx_t_13;
+  PyObject *(*__pyx_t_14)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("range", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
-    case 1: goto __pyx_L12_resume_from_yield;
+    case 1: goto __pyx_L18_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 612, __pyx_L1_error)
 
@@ -9517,166 +9529,267 @@
  *         except KeyError:
  */
     }
 
     /* "unqlite.pyx":620
  *             pass
  *         else:
- *             for item in cursor.fetch_until(end_key, include_end_key):             # <<<<<<<<<<<<<<
- *                 yield item
- * 
+ *             try:             # <<<<<<<<<<<<<<
+ *                 for item in cursor.fetch_until(end_key, include_end_key):
+ *                     yield item
  */
     /*else:*/ {
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_cursor), __pyx_n_s_fetch_until); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_cur_scope->__pyx_v_include_end_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = NULL;
-      __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_7)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_7);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
-          __pyx_t_8 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_end_key, __pyx_t_3};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_end_key, __pyx_t_3};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      } else
-      #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        if (__pyx_t_7) {
-          __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
-        }
-        __Pyx_INCREF(__pyx_cur_scope->__pyx_v_end_key);
-        __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_end_key);
-        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_cur_scope->__pyx_v_end_key);
-        __Pyx_GIVEREF(__pyx_t_3);
-        PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_3);
-        __pyx_t_3 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-        __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_10 = 0;
-        __pyx_t_11 = NULL;
-      } else {
-        __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_11 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-      }
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      for (;;) {
-        if (likely(!__pyx_t_11)) {
-          if (likely(PyList_CheckExact(__pyx_t_2))) {
-            if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_2)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-            #else
-            __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L6_except_error)
+        __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
+        __Pyx_XGOTREF(__pyx_t_7);
+        __Pyx_XGOTREF(__pyx_t_8);
+        __Pyx_XGOTREF(__pyx_t_9);
+        /*try:*/ {
+
+          /* "unqlite.pyx":621
+ *         else:
+ *             try:
+ *                 for item in cursor.fetch_until(end_key, include_end_key):             # <<<<<<<<<<<<<<
+ *                     yield item
+ *             except StopIteration:
+ */
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_cursor), __pyx_n_s_fetch_until); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L10_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_cur_scope->__pyx_v_include_end_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L10_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_10 = NULL;
+          __pyx_t_11 = 0;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
+            if (likely(__pyx_t_10)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+              __Pyx_INCREF(__pyx_t_10);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_2, function);
+              __pyx_t_11 = 1;
+            }
+          }
+          #if CYTHON_FAST_PYCALL
+          if (PyFunction_Check(__pyx_t_2)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_cur_scope->__pyx_v_end_key, __pyx_t_3};
+            __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L10_error)
+            __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
             __Pyx_GOTREF(__pyx_t_1);
-            #endif
-          } else {
-            if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 620, __pyx_L6_except_error)
-            #else
-            __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L6_except_error)
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          } else
+          #endif
+          #if CYTHON_FAST_PYCCALL
+          if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_cur_scope->__pyx_v_end_key, __pyx_t_3};
+            __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L10_error)
+            __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
             __Pyx_GOTREF(__pyx_t_1);
-            #endif
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          } else
+          #endif
+          {
+            __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 621, __pyx_L10_error)
+            __Pyx_GOTREF(__pyx_t_12);
+            if (__pyx_t_10) {
+              __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
+            }
+            __Pyx_INCREF(__pyx_cur_scope->__pyx_v_end_key);
+            __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_end_key);
+            PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_cur_scope->__pyx_v_end_key);
+            __Pyx_GIVEREF(__pyx_t_3);
+            PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_3);
+            __pyx_t_3 = 0;
+            __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L10_error)
+            __Pyx_GOTREF(__pyx_t_1);
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           }
-        } else {
-          __pyx_t_1 = __pyx_t_11(__pyx_t_2);
-          if (unlikely(!__pyx_t_1)) {
-            PyObject* exc_type = PyErr_Occurred();
-            if (exc_type) {
-              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 620, __pyx_L6_except_error)
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+            __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_13 = 0;
+            __pyx_t_14 = NULL;
+          } else {
+            __pyx_t_13 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L10_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __pyx_t_14 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 621, __pyx_L10_error)
+          }
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          for (;;) {
+            if (likely(!__pyx_t_14)) {
+              if (likely(PyList_CheckExact(__pyx_t_2))) {
+                if (__pyx_t_13 >= PyList_GET_SIZE(__pyx_t_2)) break;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L10_error)
+                #else
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L10_error)
+                __Pyx_GOTREF(__pyx_t_1);
+                #endif
+              } else {
+                if (__pyx_t_13 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L10_error)
+                #else
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L10_error)
+                __Pyx_GOTREF(__pyx_t_1);
+                #endif
+              }
+            } else {
+              __pyx_t_1 = __pyx_t_14(__pyx_t_2);
+              if (unlikely(!__pyx_t_1)) {
+                PyObject* exc_type = PyErr_Occurred();
+                if (exc_type) {
+                  if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+                  else __PYX_ERR(0, 621, __pyx_L10_error)
+                }
+                break;
+              }
+              __Pyx_GOTREF(__pyx_t_1);
             }
-            break;
+            __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_item);
+            __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_item, __pyx_t_1);
+            __Pyx_GIVEREF(__pyx_t_1);
+            __pyx_t_1 = 0;
+
+            /* "unqlite.pyx":622
+ *             try:
+ *                 for item in cursor.fetch_until(end_key, include_end_key):
+ *                     yield item             # <<<<<<<<<<<<<<
+ *             except StopIteration:
+ *                 return
+ */
+            __Pyx_INCREF(__pyx_cur_scope->__pyx_v_item);
+            __pyx_r = __pyx_cur_scope->__pyx_v_item;
+            __Pyx_XGIVEREF(__pyx_t_2);
+            __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
+            __Pyx_XGIVEREF(__pyx_t_4);
+            __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
+            __Pyx_XGIVEREF(__pyx_t_5);
+            __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
+            __Pyx_XGIVEREF(__pyx_t_6);
+            __pyx_cur_scope->__pyx_t_3 = __pyx_t_6;
+            __Pyx_XGIVEREF(__pyx_t_7);
+            __pyx_cur_scope->__pyx_t_4 = __pyx_t_7;
+            __Pyx_XGIVEREF(__pyx_t_8);
+            __pyx_cur_scope->__pyx_t_5 = __pyx_t_8;
+            __Pyx_XGIVEREF(__pyx_t_9);
+            __pyx_cur_scope->__pyx_t_6 = __pyx_t_9;
+            __pyx_cur_scope->__pyx_t_7 = __pyx_t_13;
+            __pyx_cur_scope->__pyx_t_8 = __pyx_t_14;
+            __Pyx_XGIVEREF(__pyx_r);
+            __Pyx_RefNannyFinishContext();
+            __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+            /* return from generator, yielding value */
+            __pyx_generator->resume_label = 1;
+            return __pyx_r;
+            __pyx_L18_resume_from_yield:;
+            __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
+            __pyx_cur_scope->__pyx_t_0 = 0;
+            __Pyx_XGOTREF(__pyx_t_2);
+            __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
+            __pyx_cur_scope->__pyx_t_1 = 0;
+            __Pyx_XGOTREF(__pyx_t_4);
+            __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
+            __pyx_cur_scope->__pyx_t_2 = 0;
+            __Pyx_XGOTREF(__pyx_t_5);
+            __pyx_t_6 = __pyx_cur_scope->__pyx_t_3;
+            __pyx_cur_scope->__pyx_t_3 = 0;
+            __Pyx_XGOTREF(__pyx_t_6);
+            __pyx_t_7 = __pyx_cur_scope->__pyx_t_4;
+            __pyx_cur_scope->__pyx_t_4 = 0;
+            __Pyx_XGOTREF(__pyx_t_7);
+            __pyx_t_8 = __pyx_cur_scope->__pyx_t_5;
+            __pyx_cur_scope->__pyx_t_5 = 0;
+            __Pyx_XGOTREF(__pyx_t_8);
+            __pyx_t_9 = __pyx_cur_scope->__pyx_t_6;
+            __pyx_cur_scope->__pyx_t_6 = 0;
+            __Pyx_XGOTREF(__pyx_t_9);
+            __pyx_t_13 = __pyx_cur_scope->__pyx_t_7;
+            __pyx_t_14 = __pyx_cur_scope->__pyx_t_8;
+            if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 622, __pyx_L10_error)
+
+            /* "unqlite.pyx":621
+ *         else:
+ *             try:
+ *                 for item in cursor.fetch_until(end_key, include_end_key):             # <<<<<<<<<<<<<<
+ *                     yield item
+ *             except StopIteration:
+ */
           }
-          __Pyx_GOTREF(__pyx_t_1);
-        }
-        __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_item);
-        __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_item, __pyx_t_1);
-        __Pyx_GIVEREF(__pyx_t_1);
-        __pyx_t_1 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "unqlite.pyx":621
+          /* "unqlite.pyx":620
+ *             pass
  *         else:
- *             for item in cursor.fetch_until(end_key, include_end_key):
- *                 yield item             # <<<<<<<<<<<<<<
+ *             try:             # <<<<<<<<<<<<<<
+ *                 for item in cursor.fetch_until(end_key, include_end_key):
+ *                     yield item
+ */
+        }
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+        goto __pyx_L15_try_end;
+        __pyx_L10_error:;
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+        /* "unqlite.pyx":623
+ *                 for item in cursor.fetch_until(end_key, include_end_key):
+ *                     yield item
+ *             except StopIteration:             # <<<<<<<<<<<<<<
+ *                 return
+ * 
+ */
+        __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
+        if (__pyx_t_11) {
+          __Pyx_AddTraceback("unqlite.UnQLite.range", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_12) < 0) __PYX_ERR(0, 623, __pyx_L12_except_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_GOTREF(__pyx_t_12);
+
+          /* "unqlite.pyx":624
+ *                     yield item
+ *             except StopIteration:
+ *                 return             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
-        __Pyx_INCREF(__pyx_cur_scope->__pyx_v_item);
-        __pyx_r = __pyx_cur_scope->__pyx_v_item;
-        __Pyx_XGIVEREF(__pyx_t_2);
-        __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
-        __Pyx_XGIVEREF(__pyx_t_4);
-        __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
-        __Pyx_XGIVEREF(__pyx_t_5);
-        __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
-        __Pyx_XGIVEREF(__pyx_t_6);
-        __pyx_cur_scope->__pyx_t_3 = __pyx_t_6;
-        __pyx_cur_scope->__pyx_t_4 = __pyx_t_10;
-        __pyx_cur_scope->__pyx_t_5 = __pyx_t_11;
-        __Pyx_XGIVEREF(__pyx_r);
-        __Pyx_RefNannyFinishContext();
-        __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-        /* return from generator, yielding value */
-        __pyx_generator->resume_label = 1;
-        return __pyx_r;
-        __pyx_L12_resume_from_yield:;
-        __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
-        __pyx_cur_scope->__pyx_t_0 = 0;
-        __Pyx_XGOTREF(__pyx_t_2);
-        __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
-        __pyx_cur_scope->__pyx_t_1 = 0;
-        __Pyx_XGOTREF(__pyx_t_4);
-        __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
-        __pyx_cur_scope->__pyx_t_2 = 0;
-        __Pyx_XGOTREF(__pyx_t_5);
-        __pyx_t_6 = __pyx_cur_scope->__pyx_t_3;
-        __pyx_cur_scope->__pyx_t_3 = 0;
-        __Pyx_XGOTREF(__pyx_t_6);
-        __pyx_t_10 = __pyx_cur_scope->__pyx_t_4;
-        __pyx_t_11 = __pyx_cur_scope->__pyx_t_5;
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 621, __pyx_L6_except_error)
+          __Pyx_XDECREF(__pyx_r);
+          __pyx_r = NULL;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          goto __pyx_L13_except_return;
+        }
+        goto __pyx_L12_except_error;
+        __pyx_L12_except_error:;
 
         /* "unqlite.pyx":620
  *             pass
  *         else:
- *             for item in cursor.fetch_until(end_key, include_end_key):             # <<<<<<<<<<<<<<
- *                 yield item
- * 
+ *             try:             # <<<<<<<<<<<<<<
+ *                 for item in cursor.fetch_until(end_key, include_end_key):
+ *                     yield item
  */
+        __Pyx_XGIVEREF(__pyx_t_7);
+        __Pyx_XGIVEREF(__pyx_t_8);
+        __Pyx_XGIVEREF(__pyx_t_9);
+        __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
+        goto __pyx_L6_except_error;
+        __pyx_L13_except_return:;
+        __Pyx_XGIVEREF(__pyx_t_7);
+        __Pyx_XGIVEREF(__pyx_t_8);
+        __Pyx_XGIVEREF(__pyx_t_9);
+        __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
+        goto __pyx_L7_except_return;
+        __pyx_L15_try_end:;
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -9686,16 +9799,16 @@
     /* "unqlite.pyx":617
  *         try:
  *             cursor.seek(start_key)
  *         except KeyError:             # <<<<<<<<<<<<<<
  *             pass
  *         else:
  */
-    __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
-    if (__pyx_t_8) {
+    __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
+    if (__pyx_t_11) {
       __Pyx_ErrRestore(0,0,0);
       goto __pyx_L5_exception_handled;
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
     /* "unqlite.pyx":615
@@ -9706,14 +9819,20 @@
  *         except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
     goto __pyx_L1_error;
+    __pyx_L7_except_return:;
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_XGIVEREF(__pyx_t_6);
+    __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
+    goto __pyx_L0;
     __pyx_L5_exception_handled:;
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
     __pyx_L9_try_end:;
   }
@@ -9730,30 +9849,30 @@
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("range", __pyx_clineno, __pyx_lineno, __pyx_filename);
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
 
-/* "unqlite.pyx":623
- *                 yield item
+/* "unqlite.pyx":626
+ *                 return
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return the total number of records in the database.
  */
 
 /* Python wrapper */
@@ -9793,152 +9912,152 @@
   int __pyx_t_12;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "unqlite.pyx":631
+  /* "unqlite.pyx":634
  *         """
  *         cdef Cursor cursor
  *         cdef long count = 0             # <<<<<<<<<<<<<<
  *         with self.cursor() as cursor:
  *             for item in cursor:
  */
   __pyx_v_count = 0;
 
-  /* "unqlite.pyx":632
+  /* "unqlite.pyx":635
  *         cdef Cursor cursor
  *         cdef long count = 0
  *         with self.cursor() as cursor:             # <<<<<<<<<<<<<<
  *             for item in cursor:
  *                 count += 1
  */
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 632, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 635, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
-          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_Cursor))))) __PYX_ERR(0, 632, __pyx_L7_error)
+          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_Cursor))))) __PYX_ERR(0, 635, __pyx_L7_error)
           __pyx_v_cursor = ((struct __pyx_obj_7unqlite_Cursor *)__pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":633
+          /* "unqlite.pyx":636
  *         cdef long count = 0
  *         with self.cursor() as cursor:
  *             for item in cursor:             # <<<<<<<<<<<<<<
  *                 count += 1
  *         return count
  */
           if (likely(PyList_CheckExact(((PyObject *)__pyx_v_cursor))) || PyTuple_CheckExact(((PyObject *)__pyx_v_cursor))) {
             __pyx_t_3 = ((PyObject *)__pyx_v_cursor); __Pyx_INCREF(__pyx_t_3); __pyx_t_9 = 0;
             __pyx_t_10 = NULL;
           } else {
-            __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_cursor)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 633, __pyx_L7_error)
+            __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_cursor)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 636, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 633, __pyx_L7_error)
+            __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 636, __pyx_L7_error)
           }
           for (;;) {
             if (likely(!__pyx_t_10)) {
               if (likely(PyList_CheckExact(__pyx_t_3))) {
                 if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L7_error)
+                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 636, __pyx_L7_error)
                 #else
-                __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L7_error)
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               } else {
                 if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L7_error)
+                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 636, __pyx_L7_error)
                 #else
-                __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L7_error)
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               }
             } else {
               __pyx_t_1 = __pyx_t_10(__pyx_t_3);
               if (unlikely(!__pyx_t_1)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 633, __pyx_L7_error)
+                  else __PYX_ERR(0, 636, __pyx_L7_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_1);
             }
             __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "unqlite.pyx":634
+            /* "unqlite.pyx":637
  *         with self.cursor() as cursor:
  *             for item in cursor:
  *                 count += 1             # <<<<<<<<<<<<<<
  *         return count
  * 
  */
             __pyx_v_count = (__pyx_v_count + 1);
 
-            /* "unqlite.pyx":633
+            /* "unqlite.pyx":636
  *         cdef long count = 0
  *         with self.cursor() as cursor:
  *             for item in cursor:             # <<<<<<<<<<<<<<
  *                 count += 1
  *         return count
  */
           }
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":632
+          /* "unqlite.pyx":635
  *         cdef Cursor cursor
  *         cdef long count = 0
  *         with self.cursor() as cursor:             # <<<<<<<<<<<<<<
  *             for item in cursor:
  *                 count += 1
  */
         }
@@ -9949,36 +10068,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("unqlite.UnQLite.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 632, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 635, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 632, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 635, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 632, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 635, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_12 < 0) __PYX_ERR(0, 632, __pyx_L9_except_error)
+          if (__pyx_t_12 < 0) __PYX_ERR(0, 635, __pyx_L9_except_error)
           __pyx_t_13 = ((!(__pyx_t_12 != 0)) != 0);
           if (__pyx_t_13) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_1, __pyx_t_2);
             __pyx_t_3 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 632, __pyx_L9_except_error)
+            __PYX_ERR(0, 635, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -9996,41 +10115,41 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 632, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 635, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L18;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L18:;
   }
 
-  /* "unqlite.pyx":635
+  /* "unqlite.pyx":638
  *             for item in cursor:
  *                 count += 1
  *         return count             # <<<<<<<<<<<<<<
  * 
  *     def flush(self):
  */
   __pyx_r = __pyx_v_count;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":623
- *                 yield item
+  /* "unqlite.pyx":626
+ *                 return
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return the total number of records in the database.
  */
 
   /* function exit code */
@@ -10044,15 +10163,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cursor);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":637
+/* "unqlite.pyx":640
  *         return count
  * 
  *     def flush(self):             # <<<<<<<<<<<<<<
  *         """
  *         Remove all records from the database.
  */
 
@@ -10087,116 +10206,116 @@
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("flush", 0);
 
-  /* "unqlite.pyx":645
+  /* "unqlite.pyx":648
  *         """
  *         cdef Cursor cursor
  *         cdef long i = 0             # <<<<<<<<<<<<<<
  *         with self.cursor() as cursor:
  *             while cursor.is_valid():
  */
   __pyx_v_i = 0;
 
-  /* "unqlite.pyx":646
+  /* "unqlite.pyx":649
  *         cdef Cursor cursor
  *         cdef long i = 0
  *         with self.cursor() as cursor:             # <<<<<<<<<<<<<<
  *             while cursor.is_valid():
  *                 cursor.delete()
  */
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 646, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 646, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 649, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 646, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
-          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_Cursor))))) __PYX_ERR(0, 646, __pyx_L7_error)
+          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_Cursor))))) __PYX_ERR(0, 649, __pyx_L7_error)
           __pyx_v_cursor = ((struct __pyx_obj_7unqlite_Cursor *)__pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":647
+          /* "unqlite.pyx":650
  *         cdef long i = 0
  *         with self.cursor() as cursor:
  *             while cursor.is_valid():             # <<<<<<<<<<<<<<
  *                 cursor.delete()
  *                 i += 1
  */
           while (1) {
             __pyx_t_9 = (((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_cursor->__pyx_vtab)->is_valid(__pyx_v_cursor, 0) != 0);
             if (!__pyx_t_9) break;
 
-            /* "unqlite.pyx":648
+            /* "unqlite.pyx":651
  *         with self.cursor() as cursor:
  *             while cursor.is_valid():
  *                 cursor.delete()             # <<<<<<<<<<<<<<
  *                 i += 1
  *         return i
  */
-            __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_cursor->__pyx_vtab)->delete(__pyx_v_cursor, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L7_error)
+            __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_cursor->__pyx_vtab)->delete(__pyx_v_cursor, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 651, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-            /* "unqlite.pyx":649
+            /* "unqlite.pyx":652
  *             while cursor.is_valid():
  *                 cursor.delete()
  *                 i += 1             # <<<<<<<<<<<<<<
  *         return i
  * 
  */
             __pyx_v_i = (__pyx_v_i + 1);
           }
 
-          /* "unqlite.pyx":646
+          /* "unqlite.pyx":649
  *         cdef Cursor cursor
  *         cdef long i = 0
  *         with self.cursor() as cursor:             # <<<<<<<<<<<<<<
  *             while cursor.is_valid():
  *                 cursor.delete()
  */
         }
@@ -10207,36 +10326,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("unqlite.UnQLite.flush", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 646, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 649, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 646, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 649, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 646, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 649, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (__pyx_t_9 < 0) __PYX_ERR(0, 646, __pyx_L9_except_error)
+          if (__pyx_t_9 < 0) __PYX_ERR(0, 649, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_9 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_1, __pyx_t_2);
             __pyx_t_3 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 646, __pyx_L9_except_error)
+            __PYX_ERR(0, 649, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -10254,44 +10373,44 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 646, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 649, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L18;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L18:;
   }
 
-  /* "unqlite.pyx":650
+  /* "unqlite.pyx":653
  *                 cursor.delete()
  *                 i += 1
  *         return i             # <<<<<<<<<<<<<<
  * 
  *     cpdef random_string(self, int nbytes):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":637
+  /* "unqlite.pyx":640
  *         return count
  * 
  *     def flush(self):             # <<<<<<<<<<<<<<
  *         """
  *         Remove all records from the database.
  */
 
@@ -10306,15 +10425,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cursor);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":652
+/* "unqlite.pyx":655
  *         return i
  * 
  *     cpdef random_string(self, int nbytes):             # <<<<<<<<<<<<<<
  *         """Generate a random string of given length."""
  *         cdef char *buf
  */
 
@@ -10346,19 +10465,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_random_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_random_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_7UnQLite_71random_string)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 652, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 655, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -10366,15 +10485,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 652, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 655, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -10387,60 +10506,60 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":655
+  /* "unqlite.pyx":658
  *         """Generate a random string of given length."""
  *         cdef char *buf
  *         buf = <char *>malloc(nbytes * sizeof(char))             # <<<<<<<<<<<<<<
  *         try:
  *             unqlite_util_random_string(self.database, buf, nbytes)
  */
   __pyx_v_buf = ((char *)malloc((__pyx_v_nbytes * (sizeof(char)))));
 
-  /* "unqlite.pyx":656
+  /* "unqlite.pyx":659
  *         cdef char *buf
  *         buf = <char *>malloc(nbytes * sizeof(char))
  *         try:             # <<<<<<<<<<<<<<
  *             unqlite_util_random_string(self.database, buf, nbytes)
  *             return bytes(buf[:nbytes])
  */
   /*try:*/ {
 
-    /* "unqlite.pyx":657
+    /* "unqlite.pyx":660
  *         buf = <char *>malloc(nbytes * sizeof(char))
  *         try:
  *             unqlite_util_random_string(self.database, buf, nbytes)             # <<<<<<<<<<<<<<
  *             return bytes(buf[:nbytes])
  *         finally:
  */
     (void)(unqlite_util_random_string(__pyx_v_self->database, __pyx_v_buf, __pyx_v_nbytes));
 
-    /* "unqlite.pyx":658
+    /* "unqlite.pyx":661
  *         try:
  *             unqlite_util_random_string(self.database, buf, nbytes)
  *             return bytes(buf[:nbytes])             # <<<<<<<<<<<<<<
  *         finally:
  *             free(buf)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_nbytes - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 658, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_nbytes - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 661, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 658, __pyx_L4_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 661, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "unqlite.pyx":660
+  /* "unqlite.pyx":663
  *             return bytes(buf[:nbytes])
  *         finally:
  *             free(buf)             # <<<<<<<<<<<<<<
  * 
  *     cpdef int random_int(self):
  */
   /*finally:*/ {
@@ -10486,15 +10605,15 @@
       free(__pyx_v_buf);
       __pyx_r = __pyx_t_14;
       __pyx_t_14 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "unqlite.pyx":652
+  /* "unqlite.pyx":655
  *         return i
  * 
  *     cpdef random_string(self, int nbytes):             # <<<<<<<<<<<<<<
  *         """Generate a random string of given length."""
  *         cdef char *buf
  */
 
@@ -10521,15 +10640,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_string (wrapper)", 0);
   assert(__pyx_arg_nbytes); {
-    __pyx_v_nbytes = __Pyx_PyInt_As_int(__pyx_arg_nbytes); if (unlikely((__pyx_v_nbytes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 652, __pyx_L3_error)
+    __pyx_v_nbytes = __Pyx_PyInt_As_int(__pyx_arg_nbytes); if (unlikely((__pyx_v_nbytes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 655, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.UnQLite.random_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -10545,15 +10664,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_string", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_7UnQLite_random_string(__pyx_v_self, __pyx_v_nbytes, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_7UnQLite_random_string(__pyx_v_self, __pyx_v_nbytes, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10562,15 +10681,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":662
+/* "unqlite.pyx":665
  *             free(buf)
  * 
  *     cpdef int random_int(self):             # <<<<<<<<<<<<<<
  *         """Generate a random integer."""
  *         return unqlite_util_random_num(self.database)
  */
 
@@ -10592,15 +10711,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_random_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_random_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_7UnQLite_73random_int)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -10608,18 +10727,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 662, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 665, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 662, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 665, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -10630,25 +10749,25 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":664
+  /* "unqlite.pyx":667
  *     cpdef int random_int(self):
  *         """Generate a random integer."""
  *         return unqlite_util_random_num(self.database)             # <<<<<<<<<<<<<<
  * 
  *     def lib_version(self):
  */
   __pyx_r = unqlite_util_random_num(__pyx_v_self->database);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":662
+  /* "unqlite.pyx":665
  *             free(buf)
  * 
  *     cpdef int random_int(self):             # <<<<<<<<<<<<<<
  *         """Generate a random integer."""
  *         return unqlite_util_random_num(self.database)
  */
 
@@ -10684,15 +10803,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_int", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_7unqlite_7UnQLite_random_int(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_7unqlite_7UnQLite_random_int(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10701,15 +10820,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":666
+/* "unqlite.pyx":669
  *         return unqlite_util_random_num(self.database)
  * 
  *     def lib_version(self):             # <<<<<<<<<<<<<<
  *         return unqlite_lib_version()
  * 
  */
 
@@ -10731,29 +10850,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lib_version", 0);
 
-  /* "unqlite.pyx":667
+  /* "unqlite.pyx":670
  * 
  *     def lib_version(self):
  *         return unqlite_lib_version()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromString(unqlite_lib_version()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString(unqlite_lib_version()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":666
+  /* "unqlite.pyx":669
  *         return unqlite_util_random_num(self.database)
  * 
  *     def lib_version(self):             # <<<<<<<<<<<<<<
  *         return unqlite_lib_version()
  * 
  */
 
@@ -11092,15 +11211,15 @@
   __Pyx_AddTraceback("unqlite.UnQLite.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":674
+/* "unqlite.pyx":677
  *     cdef UnQLite unqlite
  * 
  *     def __init__(self, unqlite):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  * 
  */
 
@@ -11129,26 +11248,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unqlite)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 674, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 677, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_unqlite = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 674, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 677, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Transaction.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_11Transaction___init__(((struct __pyx_obj_7unqlite_Transaction *)__pyx_v_self), __pyx_v_unqlite);
 
@@ -11162,31 +11281,31 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "unqlite.pyx":675
+  /* "unqlite.pyx":678
  * 
  *     def __init__(self, unqlite):
  *         self.unqlite = unqlite             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  if (!(likely(((__pyx_v_unqlite) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_unqlite, __pyx_ptype_7unqlite_UnQLite))))) __PYX_ERR(0, 675, __pyx_L1_error)
+  if (!(likely(((__pyx_v_unqlite) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_unqlite, __pyx_ptype_7unqlite_UnQLite))))) __PYX_ERR(0, 678, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_unqlite;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->unqlite);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->unqlite));
   __pyx_v_self->unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":674
+  /* "unqlite.pyx":677
  *     cdef UnQLite unqlite
  * 
  *     def __init__(self, unqlite):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  * 
  */
 
@@ -11198,15 +11317,15 @@
   __Pyx_AddTraceback("unqlite.Transaction.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":677
+/* "unqlite.pyx":680
  *         self.unqlite = unqlite
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.unqlite.begin()
  *         return self
  */
 
@@ -11228,38 +11347,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "unqlite.pyx":678
+  /* "unqlite.pyx":681
  * 
  *     def __enter__(self):
  *         self.unqlite.begin()             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->begin(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->begin(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":679
+  /* "unqlite.pyx":682
  *     def __enter__(self):
  *         self.unqlite.begin()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":677
+  /* "unqlite.pyx":680
  *         self.unqlite = unqlite
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.unqlite.begin()
  *         return self
  */
 
@@ -11270,15 +11389,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":681
+/* "unqlite.pyx":684
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         if exc_type:
  *             self.unqlite.rollback()
  */
 
@@ -11315,40 +11434,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 681, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 684, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_tb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 681, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 684, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 681, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 684, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 681, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 684, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Transaction.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_11Transaction_4__exit__(((struct __pyx_obj_7unqlite_Transaction *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_val, __pyx_v_exc_tb);
 
@@ -11370,46 +11489,46 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "unqlite.pyx":682
+  /* "unqlite.pyx":685
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:             # <<<<<<<<<<<<<<
  *             self.unqlite.rollback()
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_exc_type); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_exc_type); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 685, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":683
+    /* "unqlite.pyx":686
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:
  *             self.unqlite.rollback()             # <<<<<<<<<<<<<<
  *         else:
  *             try:
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->rollback(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->rollback(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 686, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unqlite.pyx":682
+    /* "unqlite.pyx":685
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         if exc_type:             # <<<<<<<<<<<<<<
  *             self.unqlite.rollback()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":685
+  /* "unqlite.pyx":688
  *             self.unqlite.rollback()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.unqlite.commit()
  *             except Exception:
  */
   /*else*/ {
@@ -11418,84 +11537,84 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "unqlite.pyx":686
+        /* "unqlite.pyx":689
  *         else:
  *             try:
  *                 self.unqlite.commit()             # <<<<<<<<<<<<<<
  *             except Exception:
  *                 self.unqlite.rollback()
  */
-        __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->commit(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 686, __pyx_L4_error)
+        __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->commit(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "unqlite.pyx":685
+        /* "unqlite.pyx":688
  *             self.unqlite.rollback()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.unqlite.commit()
  *             except Exception:
  */
       }
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "unqlite.pyx":687
+      /* "unqlite.pyx":690
  *             try:
  *                 self.unqlite.commit()
  *             except Exception:             # <<<<<<<<<<<<<<
  *                 self.unqlite.rollback()
  *                 raise
  */
       __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_6) {
         __Pyx_AddTraceback("unqlite.Transaction.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 687, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 690, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
 
-        /* "unqlite.pyx":688
+        /* "unqlite.pyx":691
  *                 self.unqlite.commit()
  *             except Exception:
  *                 self.unqlite.rollback()             # <<<<<<<<<<<<<<
  *                 raise
  * 
  */
-        __pyx_t_9 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->rollback(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 688, __pyx_L6_except_error)
+        __pyx_t_9 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->rollback(__pyx_v_self->unqlite, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 691, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "unqlite.pyx":689
+        /* "unqlite.pyx":692
  *             except Exception:
  *                 self.unqlite.rollback()
  *                 raise             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __Pyx_GIVEREF(__pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
         __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_7, __pyx_t_8);
         __pyx_t_2 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; 
-        __PYX_ERR(0, 689, __pyx_L6_except_error)
+        __PYX_ERR(0, 692, __pyx_L6_except_error)
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "unqlite.pyx":685
+      /* "unqlite.pyx":688
  *             self.unqlite.rollback()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.unqlite.commit()
  *             except Exception:
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -11504,15 +11623,15 @@
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L1_error;
       __pyx_L9_try_end:;
     }
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":681
+  /* "unqlite.pyx":684
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         if exc_type:
  *             self.unqlite.rollback()
  */
 
@@ -11821,15 +11940,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":698
+/* "unqlite.pyx":701
  *     cdef bint consumed
  * 
  *     def __cinit__(self, unqlite):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.cursor = <unqlite_kv_cursor *>0
  */
 
@@ -11858,26 +11977,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unqlite)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 698, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 701, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_unqlite = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 698, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 701, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Cursor.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_6Cursor___cinit__(((struct __pyx_obj_7unqlite_Cursor *)__pyx_v_self), __pyx_v_unqlite);
 
@@ -11891,49 +12010,49 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "unqlite.pyx":699
+  /* "unqlite.pyx":702
  * 
  *     def __cinit__(self, unqlite):
  *         self.unqlite = unqlite             # <<<<<<<<<<<<<<
  *         self.cursor = <unqlite_kv_cursor *>0
  *         unqlite_kv_cursor_init(self.unqlite.database, &self.cursor)
  */
-  if (!(likely(((__pyx_v_unqlite) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_unqlite, __pyx_ptype_7unqlite_UnQLite))))) __PYX_ERR(0, 699, __pyx_L1_error)
+  if (!(likely(((__pyx_v_unqlite) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_unqlite, __pyx_ptype_7unqlite_UnQLite))))) __PYX_ERR(0, 702, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_unqlite;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->unqlite);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->unqlite));
   __pyx_v_self->unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":700
+  /* "unqlite.pyx":703
  *     def __cinit__(self, unqlite):
  *         self.unqlite = unqlite
  *         self.cursor = <unqlite_kv_cursor *>0             # <<<<<<<<<<<<<<
  *         unqlite_kv_cursor_init(self.unqlite.database, &self.cursor)
  * 
  */
   __pyx_v_self->cursor = ((struct unqlite_kv_cursor *)0);
 
-  /* "unqlite.pyx":701
+  /* "unqlite.pyx":704
  *         self.unqlite = unqlite
  *         self.cursor = <unqlite_kv_cursor *>0
  *         unqlite_kv_cursor_init(self.unqlite.database, &self.cursor)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   (void)(unqlite_kv_cursor_init(__pyx_v_self->unqlite->database, (&__pyx_v_self->cursor)));
 
-  /* "unqlite.pyx":698
+  /* "unqlite.pyx":701
  *     cdef bint consumed
  * 
  *     def __cinit__(self, unqlite):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.cursor = <unqlite_kv_cursor *>0
  */
 
@@ -11945,15 +12064,15 @@
   __Pyx_AddTraceback("unqlite.Cursor.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":703
+/* "unqlite.pyx":706
  *         unqlite_kv_cursor_init(self.unqlite.database, &self.cursor)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         unqlite_kv_cursor_release(self.unqlite.database, self.cursor)
  * 
  */
 
@@ -11968,36 +12087,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_7unqlite_6Cursor_2__dealloc__(struct __pyx_obj_7unqlite_Cursor *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "unqlite.pyx":704
+  /* "unqlite.pyx":707
  * 
  *     def __dealloc__(self):
  *         unqlite_kv_cursor_release(self.unqlite.database, self.cursor)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
   (void)(unqlite_kv_cursor_release(__pyx_v_self->unqlite->database, __pyx_v_self->cursor));
 
-  /* "unqlite.pyx":703
+  /* "unqlite.pyx":706
  *         unqlite_kv_cursor_init(self.unqlite.database, &self.cursor)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         unqlite_kv_cursor_release(self.unqlite.database, self.cursor)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "unqlite.pyx":706
+/* "unqlite.pyx":709
  *         unqlite_kv_cursor_release(self.unqlite.database, self.cursor)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.reset()
  *         return self
  */
 
@@ -12019,38 +12138,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "unqlite.pyx":707
+  /* "unqlite.pyx":710
  * 
  *     def __enter__(self):
  *         self.reset()             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->reset(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->reset(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":708
+  /* "unqlite.pyx":711
  *     def __enter__(self):
  *         self.reset()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":706
+  /* "unqlite.pyx":709
  *         unqlite_kv_cursor_release(self.unqlite.database, self.cursor)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.reset()
  *         return self
  */
 
@@ -12061,15 +12180,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":710
+/* "unqlite.pyx":713
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
@@ -12106,40 +12225,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 710, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 713, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_tb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 710, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 713, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 710, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 713, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 710, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 713, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Cursor.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_6Cursor_6__exit__(((struct __pyx_obj_7unqlite_Cursor *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_val, __pyx_v_exc_tb);
 
@@ -12156,15 +12275,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":713
+/* "unqlite.pyx":716
  *         pass
  * 
  *     cpdef reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the cursor's position."""
  *         unqlite_kv_cursor_reset(self.cursor)
  */
 
@@ -12185,15 +12304,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_9reset)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -12202,15 +12321,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 713, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 716, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -12223,24 +12342,24 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":715
+  /* "unqlite.pyx":718
  *     cpdef reset(self):
  *         """Reset the cursor's position."""
  *         unqlite_kv_cursor_reset(self.cursor)             # <<<<<<<<<<<<<<
  * 
  *     cpdef seek(self, key, int flags=UNQLITE_CURSOR_MATCH_EXACT):
  */
   (void)(unqlite_kv_cursor_reset(__pyx_v_self->cursor));
 
-  /* "unqlite.pyx":713
+  /* "unqlite.pyx":716
  *         pass
  * 
  *     cpdef reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the cursor's position."""
  *         unqlite_kv_cursor_reset(self.cursor)
  */
 
@@ -12279,15 +12398,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reset", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_reset(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_reset(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12296,15 +12415,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":717
+/* "unqlite.pyx":720
  *         unqlite_kv_cursor_reset(self.cursor)
  * 
  *     cpdef seek(self, key, int flags=UNQLITE_CURSOR_MATCH_EXACT):             # <<<<<<<<<<<<<<
  *         """
  *         Seek to the given key. The flags specify how UnQLite will determine
  */
 
@@ -12336,19 +12455,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_seek); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_seek); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_11seek)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 717, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 720, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         __pyx_t_6 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
@@ -12358,42 +12477,42 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_6 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_key, __pyx_t_3};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_key, __pyx_t_3};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         {
-          __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 717, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 720, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           if (__pyx_t_5) {
             __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
           }
           __Pyx_INCREF(__pyx_v_key);
           __Pyx_GIVEREF(__pyx_v_key);
           PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_key);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_3);
           __pyx_t_3 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -12408,51 +12527,51 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":726
+  /* "unqlite.pyx":729
  *         * UNQLITE_CURSOR_MATCH_GE
  *         """
  *         cdef bytes encoded_key = encode(key)             # <<<<<<<<<<<<<<
  * 
  *         self.unqlite.check_call(unqlite_kv_cursor_seek(
  */
-  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_encoded_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":730
+  /* "unqlite.pyx":733
  *         self.unqlite.check_call(unqlite_kv_cursor_seek(
  *             self.cursor,
  *             <char *>encoded_key,             # <<<<<<<<<<<<<<
  *             -1,
  *             flags))
  */
   if (unlikely(__pyx_v_encoded_key == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 730, __pyx_L1_error)
+    __PYX_ERR(0, 733, __pyx_L1_error)
   }
-  __pyx_t_8 = __Pyx_PyBytes_AsWritableString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 730, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyBytes_AsWritableString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 733, __pyx_L1_error)
 
-  /* "unqlite.pyx":728
+  /* "unqlite.pyx":731
  *         cdef bytes encoded_key = encode(key)
  * 
  *         self.unqlite.check_call(unqlite_kv_cursor_seek(             # <<<<<<<<<<<<<<
  *             self.cursor,
  *             <char *>encoded_key,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_seek(__pyx_v_self->cursor, ((char *)__pyx_t_8), -1, __pyx_v_flags)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_seek(__pyx_v_self->cursor, ((char *)__pyx_t_8), -1, __pyx_v_flags)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":717
+  /* "unqlite.pyx":720
  *         unqlite_kv_cursor_reset(self.cursor)
  * 
  *     cpdef seek(self, key, int flags=UNQLITE_CURSOR_MATCH_EXACT):             # <<<<<<<<<<<<<<
  *         """
  *         Seek to the given key. The flags specify how UnQLite will determine
  */
 
@@ -12510,35 +12629,35 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "seek") < 0)) __PYX_ERR(0, 717, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "seek") < 0)) __PYX_ERR(0, 720, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = values[0];
     if (values[1]) {
-      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L3_error)
+      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
     } else {
       __pyx_v_flags = __pyx_k__10;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("seek", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 717, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("seek", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 720, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Cursor.seek", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_6Cursor_10seek(((struct __pyx_obj_7unqlite_Cursor *)__pyx_v_self), __pyx_v_key, __pyx_v_flags);
 
@@ -12555,15 +12674,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("seek", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.flags = __pyx_v_flags;
-  __pyx_t_1 = __pyx_vtabptr_7unqlite_Cursor->seek(__pyx_v_self, __pyx_v_key, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7unqlite_Cursor->seek(__pyx_v_self, __pyx_v_key, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12572,15 +12691,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":734
+/* "unqlite.pyx":737
  *             flags))
  * 
  *     cpdef first(self):             # <<<<<<<<<<<<<<
  *         """Set cursor to the first record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_first_entry(self.cursor))
  */
 
@@ -12601,15 +12720,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 734, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 737, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_13first)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -12618,15 +12737,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 734, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 737, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -12639,26 +12758,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":736
+  /* "unqlite.pyx":739
  *     cpdef first(self):
  *         """Set cursor to the first record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_first_entry(self.cursor))             # <<<<<<<<<<<<<<
  * 
  *     cpdef last(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_first_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_first_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":734
+  /* "unqlite.pyx":737
  *             flags))
  * 
  *     cpdef first(self):             # <<<<<<<<<<<<<<
  *         """Set cursor to the first record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_first_entry(self.cursor))
  */
 
@@ -12697,15 +12816,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("first", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_first(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 734, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_first(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 737, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12714,15 +12833,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":738
+/* "unqlite.pyx":741
  *         self.unqlite.check_call(unqlite_kv_cursor_first_entry(self.cursor))
  * 
  *     cpdef last(self):             # <<<<<<<<<<<<<<
  *         """Set cursor to the last record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_last_entry(self.cursor))
  */
 
@@ -12743,15 +12862,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_last); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_last); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 741, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_15last)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -12760,15 +12879,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 741, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -12781,26 +12900,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":740
+  /* "unqlite.pyx":743
  *     cpdef last(self):
  *         """Set cursor to the last record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_last_entry(self.cursor))             # <<<<<<<<<<<<<<
  * 
  *     cpdef next_entry(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_last_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_last_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 743, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":738
+  /* "unqlite.pyx":741
  *         self.unqlite.check_call(unqlite_kv_cursor_first_entry(self.cursor))
  * 
  *     cpdef last(self):             # <<<<<<<<<<<<<<
  *         """Set cursor to the last record in the database."""
  *         self.unqlite.check_call(unqlite_kv_cursor_last_entry(self.cursor))
  */
 
@@ -12839,15 +12958,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("last", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_last(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_last(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12856,15 +12975,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":742
+/* "unqlite.pyx":745
  *         self.unqlite.check_call(unqlite_kv_cursor_last_entry(self.cursor))
  * 
  *     cpdef next_entry(self):             # <<<<<<<<<<<<<<
  *         """Move cursor to the next entry."""
  *         cdef int ret
  */
 
@@ -12887,15 +13006,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_entry); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_entry); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 745, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_17next_entry)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -12904,15 +13023,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 742, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 745, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -12925,53 +13044,53 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":745
+  /* "unqlite.pyx":748
  *         """Move cursor to the next entry."""
  *         cdef int ret
  *         ret = unqlite_kv_cursor_next_entry(self.cursor)             # <<<<<<<<<<<<<<
  *         if ret != UNQLITE_OK:
  *             raise StopIteration
  */
   __pyx_v_ret = unqlite_kv_cursor_next_entry(__pyx_v_self->cursor);
 
-  /* "unqlite.pyx":746
+  /* "unqlite.pyx":749
  *         cdef int ret
  *         ret = unqlite_kv_cursor_next_entry(self.cursor)
  *         if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   __pyx_t_5 = ((__pyx_v_ret != UNQLITE_OK) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unqlite.pyx":747
+    /* "unqlite.pyx":750
  *         ret = unqlite_kv_cursor_next_entry(self.cursor)
  *         if ret != UNQLITE_OK:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *     cpdef previous_entry(self):
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 747, __pyx_L1_error)
+    __PYX_ERR(0, 750, __pyx_L1_error)
 
-    /* "unqlite.pyx":746
+    /* "unqlite.pyx":749
  *         cdef int ret
  *         ret = unqlite_kv_cursor_next_entry(self.cursor)
  *         if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   }
 
-  /* "unqlite.pyx":742
+  /* "unqlite.pyx":745
  *         self.unqlite.check_call(unqlite_kv_cursor_last_entry(self.cursor))
  * 
  *     cpdef next_entry(self):             # <<<<<<<<<<<<<<
  *         """Move cursor to the next entry."""
  *         cdef int ret
  */
 
@@ -13010,15 +13129,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_entry", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_next_entry(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_next_entry(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13027,15 +13146,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":749
+/* "unqlite.pyx":752
  *             raise StopIteration
  * 
  *     cpdef previous_entry(self):             # <<<<<<<<<<<<<<
  *         """Move cursor to the previous entry."""
  *         cdef int ret
  */
 
@@ -13058,15 +13177,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_previous_entry); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 749, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_previous_entry); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 752, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_19previous_entry)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -13075,15 +13194,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 749, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 752, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -13096,53 +13215,53 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":752
+  /* "unqlite.pyx":755
  *         """Move cursor to the previous entry."""
  *         cdef int ret
  *         ret = unqlite_kv_cursor_prev_entry(self.cursor)             # <<<<<<<<<<<<<<
  *         if ret != UNQLITE_OK:
  *             raise StopIteration
  */
   __pyx_v_ret = unqlite_kv_cursor_prev_entry(__pyx_v_self->cursor);
 
-  /* "unqlite.pyx":753
+  /* "unqlite.pyx":756
  *         cdef int ret
  *         ret = unqlite_kv_cursor_prev_entry(self.cursor)
  *         if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   __pyx_t_5 = ((__pyx_v_ret != UNQLITE_OK) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unqlite.pyx":754
+    /* "unqlite.pyx":757
  *         ret = unqlite_kv_cursor_prev_entry(self.cursor)
  *         if ret != UNQLITE_OK:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *     cpdef bint is_valid(self):
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 754, __pyx_L1_error)
+    __PYX_ERR(0, 757, __pyx_L1_error)
 
-    /* "unqlite.pyx":753
+    /* "unqlite.pyx":756
  *         cdef int ret
  *         ret = unqlite_kv_cursor_prev_entry(self.cursor)
  *         if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   }
 
-  /* "unqlite.pyx":749
+  /* "unqlite.pyx":752
  *             raise StopIteration
  * 
  *     cpdef previous_entry(self):             # <<<<<<<<<<<<<<
  *         """Move cursor to the previous entry."""
  *         cdef int ret
  */
 
@@ -13181,15 +13300,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("previous_entry", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_previous_entry(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 749, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_previous_entry(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 752, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13198,15 +13317,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":756
+/* "unqlite.pyx":759
  *             raise StopIteration
  * 
  *     cpdef bint is_valid(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return a boolean value indicating whether the cursor is currently
  */
 
@@ -13228,15 +13347,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_valid); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 756, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_valid); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_21is_valid)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -13244,18 +13363,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 756, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 759, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 759, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13266,54 +13385,54 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":761
+  /* "unqlite.pyx":764
  *         pointing to a valid record.
  *         """
  *         if unqlite_kv_cursor_valid_entry(self.cursor):             # <<<<<<<<<<<<<<
  *             return True
  *         return False
  */
   __pyx_t_5 = (unqlite_kv_cursor_valid_entry(__pyx_v_self->cursor) != 0);
   if (__pyx_t_5) {
 
-    /* "unqlite.pyx":762
+    /* "unqlite.pyx":765
  *         """
  *         if unqlite_kv_cursor_valid_entry(self.cursor):
  *             return True             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":761
+    /* "unqlite.pyx":764
  *         pointing to a valid record.
  *         """
  *         if unqlite_kv_cursor_valid_entry(self.cursor):             # <<<<<<<<<<<<<<
  *             return True
  *         return False
  */
   }
 
-  /* "unqlite.pyx":763
+  /* "unqlite.pyx":766
  *         if unqlite_kv_cursor_valid_entry(self.cursor):
  *             return True
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":756
+  /* "unqlite.pyx":759
  *             raise StopIteration
  * 
  *     cpdef bint is_valid(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return a boolean value indicating whether the cursor is currently
  */
 
@@ -13349,15 +13468,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_valid", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7unqlite_6Cursor_is_valid(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7unqlite_6Cursor_is_valid(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13366,15 +13485,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":765
+/* "unqlite.pyx":768
  *         return False
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self.consumed = False
  *         return self
  */
 
@@ -13392,51 +13511,51 @@
 }
 
 static PyObject *__pyx_pf_7unqlite_6Cursor_22__iter__(struct __pyx_obj_7unqlite_Cursor *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "unqlite.pyx":766
+  /* "unqlite.pyx":769
  * 
  *     def __iter__(self):
  *         self.consumed = False             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->consumed = 0;
 
-  /* "unqlite.pyx":767
+  /* "unqlite.pyx":770
  *     def __iter__(self):
  *         self.consumed = False
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     cpdef key(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":765
+  /* "unqlite.pyx":768
  *         return False
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self.consumed = False
  *         return self
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":769
+/* "unqlite.pyx":772
  *         return self
  * 
  *     cpdef key(self):             # <<<<<<<<<<<<<<
  *         """Retrieve the key at the cursor's current location."""
  *         cdef char *buf
  */
 
@@ -13469,15 +13588,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 769, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_25key)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -13486,15 +13605,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 769, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 772, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -13507,65 +13626,65 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":774
+  /* "unqlite.pyx":777
  *         cdef int buf_size
  * 
  *         self.unqlite.check_call(             # <<<<<<<<<<<<<<
  *             unqlite_kv_cursor_key(self.cursor, <void *>0, &buf_size))
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_key(__pyx_v_self->cursor, ((void *)0), (&__pyx_v_buf_size))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_key(__pyx_v_self->cursor, ((void *)0), (&__pyx_v_buf_size))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":777
+  /* "unqlite.pyx":780
  *             unqlite_kv_cursor_key(self.cursor, <void *>0, &buf_size))
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             buf = <char *>malloc(buf_size * sizeof(char))
  *             unqlite_kv_cursor_key(
  */
   /*try:*/ {
 
-    /* "unqlite.pyx":778
+    /* "unqlite.pyx":781
  * 
  *         try:
  *             buf = <char *>malloc(buf_size * sizeof(char))             # <<<<<<<<<<<<<<
  *             unqlite_kv_cursor_key(
  *                 self.cursor,
  */
     __pyx_v_buf = ((char *)malloc((__pyx_v_buf_size * (sizeof(char)))));
 
-    /* "unqlite.pyx":779
+    /* "unqlite.pyx":782
  *         try:
  *             buf = <char *>malloc(buf_size * sizeof(char))
  *             unqlite_kv_cursor_key(             # <<<<<<<<<<<<<<
  *                 self.cursor,
  *                 <char *>buf,
  */
     (void)(unqlite_kv_cursor_key(__pyx_v_self->cursor, ((char *)__pyx_v_buf), (&__pyx_v_buf_size)));
 
-    /* "unqlite.pyx":784
+    /* "unqlite.pyx":787
  *                 &buf_size)
  * 
  *             key = buf[:buf_size]             # <<<<<<<<<<<<<<
  *             try:
  *                 return key.decode('utf-8')
  */
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 784, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 787, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_key = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "unqlite.pyx":785
+    /* "unqlite.pyx":788
  * 
  *             key = buf[:buf_size]
  *             try:             # <<<<<<<<<<<<<<
  *                 return key.decode('utf-8')
  *             except UnicodeDecodeError:
  */
     {
@@ -13573,58 +13692,58 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       /*try:*/ {
 
-        /* "unqlite.pyx":786
+        /* "unqlite.pyx":789
  *             key = buf[:buf_size]
  *             try:
  *                 return key.decode('utf-8')             # <<<<<<<<<<<<<<
  *             except UnicodeDecodeError:
  *                 return key
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_key, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 786, __pyx_L6_error)
+        __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_key, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 789, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L10_try_return;
 
-        /* "unqlite.pyx":785
+        /* "unqlite.pyx":788
  * 
  *             key = buf[:buf_size]
  *             try:             # <<<<<<<<<<<<<<
  *                 return key.decode('utf-8')
  *             except UnicodeDecodeError:
  */
       }
       __pyx_L6_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "unqlite.pyx":787
+      /* "unqlite.pyx":790
  *             try:
  *                 return key.decode('utf-8')
  *             except UnicodeDecodeError:             # <<<<<<<<<<<<<<
  *                 return key
  *         finally:
  */
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_UnicodeDecodeError);
       if (__pyx_t_8) {
         __Pyx_AddTraceback("unqlite.Cursor.key", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 787, __pyx_L8_except_error)
+        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 790, __pyx_L8_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_3);
 
-        /* "unqlite.pyx":788
+        /* "unqlite.pyx":791
  *                 return key.decode('utf-8')
  *             except UnicodeDecodeError:
  *                 return key             # <<<<<<<<<<<<<<
  *         finally:
  *             free(buf)
  */
         __Pyx_XDECREF(__pyx_r);
@@ -13634,15 +13753,15 @@
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         goto __pyx_L9_except_return;
       }
       goto __pyx_L8_except_error;
       __pyx_L8_except_error:;
 
-      /* "unqlite.pyx":785
+      /* "unqlite.pyx":788
  * 
  *             key = buf[:buf_size]
  *             try:             # <<<<<<<<<<<<<<
  *                 return key.decode('utf-8')
  *             except UnicodeDecodeError:
  */
       __Pyx_XGIVEREF(__pyx_t_5);
@@ -13661,15 +13780,15 @@
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
       goto __pyx_L3_return;
     }
   }
 
-  /* "unqlite.pyx":790
+  /* "unqlite.pyx":793
  *                 return key
  *         finally:
  *             free(buf)             # <<<<<<<<<<<<<<
  * 
  *     cpdef value(self):
  */
   /*finally:*/ {
@@ -13714,15 +13833,15 @@
       free(__pyx_v_buf);
       __pyx_r = __pyx_t_13;
       __pyx_t_13 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "unqlite.pyx":769
+  /* "unqlite.pyx":772
  *         return self
  * 
  *     cpdef key(self):             # <<<<<<<<<<<<<<
  *         """Retrieve the key at the cursor's current location."""
  *         cdef char *buf
  */
 
@@ -13760,15 +13879,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("key", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_key(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 769, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_key(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13777,15 +13896,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":792
+/* "unqlite.pyx":795
  *             free(buf)
  * 
  *     cpdef value(self):             # <<<<<<<<<<<<<<
  *         """Retrieve the value at the cursor's current location."""
  *         cdef char *buf
  */
 
@@ -13818,15 +13937,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_27value)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -13835,15 +13954,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 792, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 795, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -13856,78 +13975,78 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":797
+  /* "unqlite.pyx":800
  *         cdef unqlite_int64 buf_size
  * 
  *         self.unqlite.check_call(             # <<<<<<<<<<<<<<
  *             unqlite_kv_cursor_data(self.cursor, <void *>0, &buf_size))
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_data(__pyx_v_self->cursor, ((void *)0), (&__pyx_v_buf_size))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_data(__pyx_v_self->cursor, ((void *)0), (&__pyx_v_buf_size))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 800, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":800
+  /* "unqlite.pyx":803
  *             unqlite_kv_cursor_data(self.cursor, <void *>0, &buf_size))
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             buf = <char *>malloc(buf_size * sizeof(char))
  *             unqlite_kv_cursor_data(
  */
   /*try:*/ {
 
-    /* "unqlite.pyx":801
+    /* "unqlite.pyx":804
  * 
  *         try:
  *             buf = <char *>malloc(buf_size * sizeof(char))             # <<<<<<<<<<<<<<
  *             unqlite_kv_cursor_data(
  *                 self.cursor,
  */
     __pyx_v_buf = ((char *)malloc((__pyx_v_buf_size * (sizeof(char)))));
 
-    /* "unqlite.pyx":802
+    /* "unqlite.pyx":805
  *         try:
  *             buf = <char *>malloc(buf_size * sizeof(char))
  *             unqlite_kv_cursor_data(             # <<<<<<<<<<<<<<
  *                 self.cursor,
  *                 <char *>buf,
  */
     (void)(unqlite_kv_cursor_data(__pyx_v_self->cursor, ((char *)__pyx_v_buf), (&__pyx_v_buf_size)));
 
-    /* "unqlite.pyx":807
+    /* "unqlite.pyx":810
  *                 &buf_size)
  * 
  *             value = buf[:buf_size]             # <<<<<<<<<<<<<<
  *             return value
  *         finally:
  */
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 807, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buf + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 810, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_value = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "unqlite.pyx":808
+    /* "unqlite.pyx":811
  * 
  *             value = buf[:buf_size]
  *             return value             # <<<<<<<<<<<<<<
  *         finally:
  *             free(buf)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_value);
     __pyx_r = __pyx_v_value;
     goto __pyx_L3_return;
   }
 
-  /* "unqlite.pyx":810
+  /* "unqlite.pyx":813
  *             return value
  *         finally:
  *             free(buf)             # <<<<<<<<<<<<<<
  * 
  *     cpdef delete(self):
  */
   /*finally:*/ {
@@ -13972,15 +14091,15 @@
       free(__pyx_v_buf);
       __pyx_r = __pyx_t_13;
       __pyx_t_13 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "unqlite.pyx":792
+  /* "unqlite.pyx":795
  *             free(buf)
  * 
  *     cpdef value(self):             # <<<<<<<<<<<<<<
  *         """Retrieve the value at the cursor's current location."""
  *         cdef char *buf
  */
 
@@ -14018,15 +14137,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("value", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_value(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_value(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14035,15 +14154,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":812
+/* "unqlite.pyx":815
  *             free(buf)
  * 
  *     cpdef delete(self):             # <<<<<<<<<<<<<<
  *         """Delete the record at the cursor's current location."""
  *         self.unqlite.check_call(unqlite_kv_cursor_delete_entry(self.cursor))
  */
 
@@ -14064,15 +14183,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_delete); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 812, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_delete); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 815, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_6Cursor_29delete)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -14081,15 +14200,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 812, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 815, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -14102,26 +14221,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":814
+  /* "unqlite.pyx":817
  *     cpdef delete(self):
  *         """Delete the record at the cursor's current location."""
  *         self.unqlite.check_call(unqlite_kv_cursor_delete_entry(self.cursor))             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_delete_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_kv_cursor_delete_entry(__pyx_v_self->cursor)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":812
+  /* "unqlite.pyx":815
  *             free(buf)
  * 
  *     cpdef delete(self):             # <<<<<<<<<<<<<<
  *         """Delete the record at the cursor's current location."""
  *         self.unqlite.check_call(unqlite_kv_cursor_delete_entry(self.cursor))
  */
 
@@ -14160,15 +14279,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_delete(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 812, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_6Cursor_delete(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14177,15 +14296,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":816
+/* "unqlite.pyx":819
  *         self.unqlite.check_call(unqlite_kv_cursor_delete_entry(self.cursor))
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef int ret
  * 
  */
 
@@ -14217,44 +14336,44 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "unqlite.pyx":819
+  /* "unqlite.pyx":822
  *         cdef int ret
  * 
  *         if self.consumed:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   __pyx_t_1 = (__pyx_v_self->consumed != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unqlite.pyx":820
+    /* "unqlite.pyx":823
  * 
  *         if self.consumed:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 820, __pyx_L1_error)
+    __PYX_ERR(0, 823, __pyx_L1_error)
 
-    /* "unqlite.pyx":819
+    /* "unqlite.pyx":822
  *         cdef int ret
  * 
  *         if self.consumed:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   }
 
-  /* "unqlite.pyx":822
+  /* "unqlite.pyx":825
  *             raise StopIteration
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             key = self.key()
  *             value = self.value()
  */
   {
@@ -14262,77 +14381,77 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "unqlite.pyx":823
+      /* "unqlite.pyx":826
  * 
  *         try:
  *             key = self.key()             # <<<<<<<<<<<<<<
  *             value = self.value()
  *         except Exception:
  */
-      __pyx_t_5 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->key(__pyx_v_self, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 823, __pyx_L4_error)
+      __pyx_t_5 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->key(__pyx_v_self, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 826, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_v_key = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "unqlite.pyx":824
+      /* "unqlite.pyx":827
  *         try:
  *             key = self.key()
  *             value = self.value()             # <<<<<<<<<<<<<<
  *         except Exception:
  *             raise StopIteration
  */
-      __pyx_t_5 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->value(__pyx_v_self, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 824, __pyx_L4_error)
+      __pyx_t_5 = ((struct __pyx_vtabstruct_7unqlite_Cursor *)__pyx_v_self->__pyx_vtab)->value(__pyx_v_self, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 827, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_v_value = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "unqlite.pyx":822
+      /* "unqlite.pyx":825
  *             raise StopIteration
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             key = self.key()
  *             value = self.value()
  */
     }
 
-    /* "unqlite.pyx":828
+    /* "unqlite.pyx":831
  *             raise StopIteration
  *         else:
  *             ret = unqlite_kv_cursor_next_entry(self.cursor)             # <<<<<<<<<<<<<<
  *             if ret != UNQLITE_OK:
  *                 self.consumed = True
  */
     /*else:*/ {
       __pyx_v_ret = unqlite_kv_cursor_next_entry(__pyx_v_self->cursor);
 
-      /* "unqlite.pyx":829
+      /* "unqlite.pyx":832
  *         else:
  *             ret = unqlite_kv_cursor_next_entry(self.cursor)
  *             if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *                 self.consumed = True
  * 
  */
       __pyx_t_1 = ((__pyx_v_ret != UNQLITE_OK) != 0);
       if (__pyx_t_1) {
 
-        /* "unqlite.pyx":830
+        /* "unqlite.pyx":833
  *             ret = unqlite_kv_cursor_next_entry(self.cursor)
  *             if ret != UNQLITE_OK:
  *                 self.consumed = True             # <<<<<<<<<<<<<<
  * 
  *         return (key, value)
  */
         __pyx_v_self->consumed = 1;
 
-        /* "unqlite.pyx":829
+        /* "unqlite.pyx":832
  *         else:
  *             ret = unqlite_kv_cursor_next_entry(self.cursor)
  *             if ret != UNQLITE_OK:             # <<<<<<<<<<<<<<
  *                 self.consumed = True
  * 
  */
       }
@@ -14340,78 +14459,78 @@
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "unqlite.pyx":825
+    /* "unqlite.pyx":828
  *             key = self.key()
  *             value = self.value()
  *         except Exception:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  *         else:
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_6) {
       __Pyx_AddTraceback("unqlite.Cursor.__next__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 825, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 828, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_8);
 
-      /* "unqlite.pyx":826
+      /* "unqlite.pyx":829
  *             value = self.value()
  *         except Exception:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  *         else:
  *             ret = unqlite_kv_cursor_next_entry(self.cursor)
  */
       __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-      __PYX_ERR(0, 826, __pyx_L6_except_error)
+      __PYX_ERR(0, 829, __pyx_L6_except_error)
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "unqlite.pyx":822
+    /* "unqlite.pyx":825
  *             raise StopIteration
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             key = self.key()
  *             value = self.value()
  */
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "unqlite.pyx":832
+  /* "unqlite.pyx":835
  *                 self.consumed = True
  * 
  *         return (key, value)             # <<<<<<<<<<<<<<
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 832, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_v_key);
   __Pyx_GIVEREF(__pyx_v_key);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_key);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_value);
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":816
+  /* "unqlite.pyx":819
  *         self.unqlite.check_call(unqlite_kv_cursor_delete_entry(self.cursor))
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef int ret
  * 
  */
 
@@ -14427,15 +14546,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_7unqlite_6Cursor_34generator4(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "unqlite.pyx":834
+/* "unqlite.pyx":837
  *         return (key, value)
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):             # <<<<<<<<<<<<<<
  *         for key, value in self:
  *             if key == stop_key:
  */
 
@@ -14473,35 +14592,35 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_include_stop_key);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fetch_until") < 0)) __PYX_ERR(0, 834, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fetch_until") < 0)) __PYX_ERR(0, 837, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_stop_key = values[0];
     if (values[1]) {
-      __pyx_v_include_stop_key = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_include_stop_key == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 834, __pyx_L3_error)
+      __pyx_v_include_stop_key = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_include_stop_key == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 837, __pyx_L3_error)
     } else {
       __pyx_v_include_stop_key = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fetch_until", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 834, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fetch_until", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 837, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Cursor.fetch_until", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_6Cursor_32fetch_until(((struct __pyx_obj_7unqlite_Cursor *)__pyx_v_self), __pyx_v_stop_key, __pyx_v_include_stop_key);
 
@@ -14518,27 +14637,27 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fetch_until", 0);
   __pyx_cur_scope = (struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until *)__pyx_tp_new_7unqlite___pyx_scope_struct_5_fetch_until(__pyx_ptype_7unqlite___pyx_scope_struct_5_fetch_until, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 834, __pyx_L1_error)
+    __PYX_ERR(0, 837, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_stop_key = __pyx_v_stop_key;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_stop_key);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_stop_key);
   __pyx_cur_scope->__pyx_v_include_stop_key = __pyx_v_include_stop_key;
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7unqlite_6Cursor_34generator4, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_fetch_until, __pyx_n_s_Cursor_fetch_until, __pyx_n_s_unqlite); if (unlikely(!gen)) __PYX_ERR(0, 834, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7unqlite_6Cursor_34generator4, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_fetch_until, __pyx_n_s_Cursor_fetch_until, __pyx_n_s_unqlite); if (unlikely(!gen)) __PYX_ERR(0, 837, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14573,147 +14692,147 @@
     case 1: goto __pyx_L10_resume_from_yield;
     case 2: goto __pyx_L11_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 834, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 837, __pyx_L1_error)
 
-  /* "unqlite.pyx":835
+  /* "unqlite.pyx":838
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):
  *         for key, value in self:             # <<<<<<<<<<<<<<
  *             if key == stop_key:
  *                 if include_stop_key:
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_v_self))) {
     __pyx_t_1 = ((PyObject *)__pyx_cur_scope->__pyx_v_self); __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 835, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 838, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 835, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 838, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 835, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 835, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 838, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 835, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 835, __pyx_L1_error)
+          else __PYX_ERR(0, 838, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
       PyObject* sequence = __pyx_t_4;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 835, __pyx_L1_error)
+        __PYX_ERR(0, 838, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 835, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 838, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 835, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 838, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_7 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 835, __pyx_L1_error)
+      __pyx_t_7 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 838, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
       index = 0; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
       index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 835, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 838, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 835, __pyx_L1_error)
+      __PYX_ERR(0, 838, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_key);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_key, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_value);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_value, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "unqlite.pyx":836
+    /* "unqlite.pyx":839
  *     def fetch_until(self, stop_key, bint include_stop_key=True):
  *         for key, value in self:
  *             if key == stop_key:             # <<<<<<<<<<<<<<
  *                 if include_stop_key:
  *                     yield (key, value)
  */
-    __pyx_t_4 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_key, __pyx_cur_scope->__pyx_v_stop_key, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 836, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 836, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_key, __pyx_cur_scope->__pyx_v_stop_key, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 839, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 839, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_9) {
 
-      /* "unqlite.pyx":837
+      /* "unqlite.pyx":840
  *         for key, value in self:
  *             if key == stop_key:
  *                 if include_stop_key:             # <<<<<<<<<<<<<<
  *                     yield (key, value)
- *                 raise StopIteration
+ *                 return
  */
       __pyx_t_9 = (__pyx_cur_scope->__pyx_v_include_stop_key != 0);
       if (__pyx_t_9) {
 
-        /* "unqlite.pyx":838
+        /* "unqlite.pyx":841
  *             if key == stop_key:
  *                 if include_stop_key:
  *                     yield (key, value)             # <<<<<<<<<<<<<<
- *                 raise StopIteration
+ *                 return
  *             else:
  */
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_key);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_key);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_key);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_value);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_value);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_cur_scope->__pyx_v_value);
@@ -14731,53 +14850,55 @@
         return __pyx_r;
         __pyx_L10_resume_from_yield:;
         __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
         __pyx_cur_scope->__pyx_t_0 = 0;
         __Pyx_XGOTREF(__pyx_t_1);
         __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
         __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 838, __pyx_L1_error)
+        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 841, __pyx_L1_error)
 
-        /* "unqlite.pyx":837
+        /* "unqlite.pyx":840
  *         for key, value in self:
  *             if key == stop_key:
  *                 if include_stop_key:             # <<<<<<<<<<<<<<
  *                     yield (key, value)
- *                 raise StopIteration
+ *                 return
  */
       }
 
-      /* "unqlite.pyx":839
+      /* "unqlite.pyx":842
  *                 if include_stop_key:
  *                     yield (key, value)
- *                 raise StopIteration             # <<<<<<<<<<<<<<
+ *                 return             # <<<<<<<<<<<<<<
  *             else:
  *                 yield (key, value)
  */
-      __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-      __PYX_ERR(0, 839, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_r);
+      __pyx_r = NULL;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      goto __pyx_L0;
 
-      /* "unqlite.pyx":836
+      /* "unqlite.pyx":839
  *     def fetch_until(self, stop_key, bint include_stop_key=True):
  *         for key, value in self:
  *             if key == stop_key:             # <<<<<<<<<<<<<<
  *                 if include_stop_key:
  *                     yield (key, value)
  */
     }
 
-    /* "unqlite.pyx":841
- *                 raise StopIteration
+    /* "unqlite.pyx":844
+ *                 return
  *             else:
  *                 yield (key, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_key);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_key);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_key);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_value);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_cur_scope->__pyx_v_value);
@@ -14795,29 +14916,29 @@
       return __pyx_r;
       __pyx_L11_resume_from_yield:;
       __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
       __pyx_cur_scope->__pyx_t_0 = 0;
       __Pyx_XGOTREF(__pyx_t_1);
       __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 841, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 844, __pyx_L1_error)
     }
 
-    /* "unqlite.pyx":835
+    /* "unqlite.pyx":838
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):
  *         for key, value in self:             # <<<<<<<<<<<<<<
  *             if key == stop_key:
  *                 if include_stop_key:
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "unqlite.pyx":834
+  /* "unqlite.pyx":837
  *         return (key, value)
  * 
  *     def fetch_until(self, stop_key, bint include_stop_key=True):             # <<<<<<<<<<<<<<
  *         for key, value in self:
  *             if key == stop_key:
  */
 
@@ -14951,15 +15072,15 @@
   __Pyx_AddTraceback("unqlite.Cursor.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":857
+/* "unqlite.pyx":860
  *     cdef set encoded_names
  * 
  *     def __cinit__(self, UnQLite unqlite, code):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.vm = <unqlite_vm *>0
  */
 
@@ -14993,38 +15114,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unqlite)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 857, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 860, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 857, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 860, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)values[0]);
     __pyx_v_code = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 857, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 860, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.VM.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unqlite), __pyx_ptype_7unqlite_UnQLite, 1, "unqlite", 0))) __PYX_ERR(0, 857, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unqlite), __pyx_ptype_7unqlite_UnQLite, 1, "unqlite", 0))) __PYX_ERR(0, 860, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_2VM___cinit__(((struct __pyx_obj_7unqlite_VM *)__pyx_v_self), __pyx_v_unqlite, __pyx_v_code);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -15037,80 +15158,80 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "unqlite.pyx":858
+  /* "unqlite.pyx":861
  * 
  *     def __cinit__(self, UnQLite unqlite, code):
  *         self.unqlite = unqlite             # <<<<<<<<<<<<<<
  *         self.vm = <unqlite_vm *>0
  *         self.code = code
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_unqlite));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_unqlite));
   __Pyx_GOTREF(__pyx_v_self->unqlite);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->unqlite));
   __pyx_v_self->unqlite = __pyx_v_unqlite;
 
-  /* "unqlite.pyx":859
+  /* "unqlite.pyx":862
  *     def __cinit__(self, UnQLite unqlite, code):
  *         self.unqlite = unqlite
  *         self.vm = <unqlite_vm *>0             # <<<<<<<<<<<<<<
  *         self.code = code
  *         self.encoded_code = encode(code)
  */
   __pyx_v_self->vm = ((unqlite_vm *)0);
 
-  /* "unqlite.pyx":860
+  /* "unqlite.pyx":863
  *         self.unqlite = unqlite
  *         self.vm = <unqlite_vm *>0
  *         self.code = code             # <<<<<<<<<<<<<<
  *         self.encoded_code = encode(code)
  *         self.encoded_names = set()
  */
   __Pyx_INCREF(__pyx_v_code);
   __Pyx_GIVEREF(__pyx_v_code);
   __Pyx_GOTREF(__pyx_v_self->code);
   __Pyx_DECREF(__pyx_v_self->code);
   __pyx_v_self->code = __pyx_v_code;
 
-  /* "unqlite.pyx":861
+  /* "unqlite.pyx":864
  *         self.vm = <unqlite_vm *>0
  *         self.code = code
  *         self.encoded_code = encode(code)             # <<<<<<<<<<<<<<
  *         self.encoded_names = set()
  * 
  */
-  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 861, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->encoded_code);
   __Pyx_DECREF(__pyx_v_self->encoded_code);
   __pyx_v_self->encoded_code = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":862
+  /* "unqlite.pyx":865
  *         self.code = code
  *         self.encoded_code = encode(code)
  *         self.encoded_names = set()             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 862, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 865, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->encoded_names);
   __Pyx_DECREF(__pyx_v_self->encoded_names);
   __pyx_v_self->encoded_names = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":857
+  /* "unqlite.pyx":860
  *     cdef set encoded_names
  * 
  *     def __cinit__(self, UnQLite unqlite, code):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.vm = <unqlite_vm *>0
  */
 
@@ -15122,15 +15243,15 @@
   __Pyx_AddTraceback("unqlite.VM.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":864
+/* "unqlite.pyx":867
  *         self.encoded_names = set()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         # For some reason, calling unqlite_vm_release() here always causes a
  *         # segfault.
  */
 
@@ -15149,15 +15270,15 @@
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "unqlite.pyx":869
+/* "unqlite.pyx":872
  *         pass
  * 
  *     cpdef compile(self):             # <<<<<<<<<<<<<<
  *         """Compile the Jx9 script."""
  *         self.encoded_names.clear()
  */
 
@@ -15181,15 +15302,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_compile); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 869, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_compile); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_2VM_5compile)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15198,15 +15319,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 869, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 872, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -15219,53 +15340,53 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":871
+  /* "unqlite.pyx":874
  *     cpdef compile(self):
  *         """Compile the Jx9 script."""
  *         self.encoded_names.clear()             # <<<<<<<<<<<<<<
  *         cdef const char *code = <const char *>self.encoded_code
  *         self.unqlite.check_call(unqlite_compile(
  */
   if (unlikely(__pyx_v_self->encoded_names == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-    __PYX_ERR(0, 871, __pyx_L1_error)
+    __PYX_ERR(0, 874, __pyx_L1_error)
   }
-  __pyx_t_5 = PySet_Clear(__pyx_v_self->encoded_names); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 871, __pyx_L1_error)
+  __pyx_t_5 = PySet_Clear(__pyx_v_self->encoded_names); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 874, __pyx_L1_error)
 
-  /* "unqlite.pyx":872
+  /* "unqlite.pyx":875
  *         """Compile the Jx9 script."""
  *         self.encoded_names.clear()
  *         cdef const char *code = <const char *>self.encoded_code             # <<<<<<<<<<<<<<
  *         self.unqlite.check_call(unqlite_compile(
  *             self.unqlite.database,
  */
   if (unlikely(__pyx_v_self->encoded_code == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 872, __pyx_L1_error)
+    __PYX_ERR(0, 875, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyBytes_AsString(__pyx_v_self->encoded_code); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 872, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_AsString(__pyx_v_self->encoded_code); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 875, __pyx_L1_error)
   __pyx_v_code = ((char const *)__pyx_t_6);
 
-  /* "unqlite.pyx":873
+  /* "unqlite.pyx":876
  *         self.encoded_names.clear()
  *         cdef const char *code = <const char *>self.encoded_code
  *         self.unqlite.check_call(unqlite_compile(             # <<<<<<<<<<<<<<
  *             self.unqlite.database,
  *             code,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_compile(__pyx_v_self->unqlite->database, __pyx_v_code, -1, (&__pyx_v_self->vm))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 873, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_compile(__pyx_v_self->unqlite->database, __pyx_v_code, -1, (&__pyx_v_self->vm))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 876, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":869
+  /* "unqlite.pyx":872
  *         pass
  * 
  *     cpdef compile(self):             # <<<<<<<<<<<<<<
  *         """Compile the Jx9 script."""
  *         self.encoded_names.clear()
  */
 
@@ -15304,15 +15425,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_2VM_compile(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 869, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_2VM_compile(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15321,15 +15442,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":879
+/* "unqlite.pyx":882
  *             &self.vm))
  * 
  *     cpdef execute(self):             # <<<<<<<<<<<<<<
  *         """Execute the compiled Jx9 script."""
  *         if not self.vm:
  */
 
@@ -15351,15 +15472,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_2VM_7execute)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15368,15 +15489,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -15389,73 +15510,73 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":881
+  /* "unqlite.pyx":884
  *     cpdef execute(self):
  *         """Execute the compiled Jx9 script."""
  *         if not self.vm:             # <<<<<<<<<<<<<<
  *             raise UnQLiteError('Jx9 script must be compiled before executing.')
  * 
  */
   __pyx_t_5 = ((!(__pyx_v_self->vm != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unqlite.pyx":882
+    /* "unqlite.pyx":885
  *         """Execute the compiled Jx9 script."""
  *         if not self.vm:
  *             raise UnQLiteError('Jx9 script must be compiled before executing.')             # <<<<<<<<<<<<<<
  * 
  *         # Cannot release GIL here as the Jx9 script may invoke python-side code
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnQLiteError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnQLiteError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_Jx9_script_must_be_compiled_befo) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_Jx9_script_must_be_compiled_befo);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 882, __pyx_L1_error)
+    __PYX_ERR(0, 885, __pyx_L1_error)
 
-    /* "unqlite.pyx":881
+    /* "unqlite.pyx":884
  *     cpdef execute(self):
  *         """Execute the compiled Jx9 script."""
  *         if not self.vm:             # <<<<<<<<<<<<<<
  *             raise UnQLiteError('Jx9 script must be compiled before executing.')
  * 
  */
   }
 
-  /* "unqlite.pyx":886
+  /* "unqlite.pyx":889
  *         # Cannot release GIL here as the Jx9 script may invoke python-side code
  *         # like user-defined functions or filters.
  *         self.unqlite.check_call(unqlite_vm_exec(self.vm))             # <<<<<<<<<<<<<<
  * 
  *     cpdef reset(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_exec(__pyx_v_self->vm)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 886, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_exec(__pyx_v_self->vm)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 889, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":879
+  /* "unqlite.pyx":882
  *             &self.vm))
  * 
  *     cpdef execute(self):             # <<<<<<<<<<<<<<
  *         """Execute the compiled Jx9 script."""
  *         if not self.vm:
  */
 
@@ -15494,15 +15615,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("execute", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_2VM_execute(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_2VM_execute(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15511,15 +15632,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":888
+/* "unqlite.pyx":891
  *         self.unqlite.check_call(unqlite_vm_exec(self.vm))
  * 
  *     cpdef reset(self):             # <<<<<<<<<<<<<<
  *         if not self.vm:
  *             raise UnQLiteError('Jx9 script has not been compiled.')
  */
 
@@ -15541,15 +15662,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 888, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 891, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_2VM_9reset)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15558,15 +15679,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 888, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 891, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -15579,85 +15700,85 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":889
+  /* "unqlite.pyx":892
  * 
  *     cpdef reset(self):
  *         if not self.vm:             # <<<<<<<<<<<<<<
  *             raise UnQLiteError('Jx9 script has not been compiled.')
  * 
  */
   __pyx_t_5 = ((!(__pyx_v_self->vm != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unqlite.pyx":890
+    /* "unqlite.pyx":893
  *     cpdef reset(self):
  *         if not self.vm:
  *             raise UnQLiteError('Jx9 script has not been compiled.')             # <<<<<<<<<<<<<<
  * 
  *         self.unqlite.check_call(unqlite_vm_reset(self.vm))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnQLiteError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 890, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnQLiteError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 893, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_Jx9_script_has_not_been_compiled) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_Jx9_script_has_not_been_compiled);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 890, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 893, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 890, __pyx_L1_error)
+    __PYX_ERR(0, 893, __pyx_L1_error)
 
-    /* "unqlite.pyx":889
+    /* "unqlite.pyx":892
  * 
  *     cpdef reset(self):
  *         if not self.vm:             # <<<<<<<<<<<<<<
  *             raise UnQLiteError('Jx9 script has not been compiled.')
  * 
  */
   }
 
-  /* "unqlite.pyx":892
+  /* "unqlite.pyx":895
  *             raise UnQLiteError('Jx9 script has not been compiled.')
  * 
  *         self.unqlite.check_call(unqlite_vm_reset(self.vm))             # <<<<<<<<<<<<<<
  *         return True
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_reset(__pyx_v_self->vm)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 892, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_reset(__pyx_v_self->vm)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 895, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":893
+  /* "unqlite.pyx":896
  * 
  *         self.unqlite.check_call(unqlite_vm_reset(self.vm))
  *         return True             # <<<<<<<<<<<<<<
  * 
  *     cpdef close(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(Py_True);
   __pyx_r = Py_True;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":888
+  /* "unqlite.pyx":891
  *         self.unqlite.check_call(unqlite_vm_exec(self.vm))
  * 
  *     cpdef reset(self):             # <<<<<<<<<<<<<<
  *         if not self.vm:
  *             raise UnQLiteError('Jx9 script has not been compiled.')
  */
 
@@ -15693,15 +15814,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reset", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_2VM_reset(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 888, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_2VM_reset(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 891, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15710,15 +15831,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":895
+/* "unqlite.pyx":898
  *         return True
  * 
  *     cpdef close(self):             # <<<<<<<<<<<<<<
  *         """Close and release the virtual machine."""
  *         self.encoded_names.clear()
  */
 
@@ -15741,15 +15862,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 895, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 898, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_2VM_11close)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15758,15 +15879,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 895, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 898, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -15779,65 +15900,65 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":897
+  /* "unqlite.pyx":900
  *     cpdef close(self):
  *         """Close and release the virtual machine."""
  *         self.encoded_names.clear()             # <<<<<<<<<<<<<<
  *         if self.vm:
  *             unqlite_vm_release(self.vm)
  */
   if (unlikely(__pyx_v_self->encoded_names == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-    __PYX_ERR(0, 897, __pyx_L1_error)
+    __PYX_ERR(0, 900, __pyx_L1_error)
   }
-  __pyx_t_5 = PySet_Clear(__pyx_v_self->encoded_names); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 897, __pyx_L1_error)
+  __pyx_t_5 = PySet_Clear(__pyx_v_self->encoded_names); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 900, __pyx_L1_error)
 
-  /* "unqlite.pyx":898
+  /* "unqlite.pyx":901
  *         """Close and release the virtual machine."""
  *         self.encoded_names.clear()
  *         if self.vm:             # <<<<<<<<<<<<<<
  *             unqlite_vm_release(self.vm)
  *             self.vm = <unqlite_vm *>0
  */
   __pyx_t_6 = (__pyx_v_self->vm != 0);
   if (__pyx_t_6) {
 
-    /* "unqlite.pyx":899
+    /* "unqlite.pyx":902
  *         self.encoded_names.clear()
  *         if self.vm:
  *             unqlite_vm_release(self.vm)             # <<<<<<<<<<<<<<
  *             self.vm = <unqlite_vm *>0
  * 
  */
     (void)(unqlite_vm_release(__pyx_v_self->vm));
 
-    /* "unqlite.pyx":900
+    /* "unqlite.pyx":903
  *         if self.vm:
  *             unqlite_vm_release(self.vm)
  *             self.vm = <unqlite_vm *>0             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
     __pyx_v_self->vm = ((unqlite_vm *)0);
 
-    /* "unqlite.pyx":898
+    /* "unqlite.pyx":901
  *         """Close and release the virtual machine."""
  *         self.encoded_names.clear()
  *         if self.vm:             # <<<<<<<<<<<<<<
  *             unqlite_vm_release(self.vm)
  *             self.vm = <unqlite_vm *>0
  */
   }
 
-  /* "unqlite.pyx":895
+  /* "unqlite.pyx":898
  *         return True
  * 
  *     cpdef close(self):             # <<<<<<<<<<<<<<
  *         """Close and release the virtual machine."""
  *         self.encoded_names.clear()
  */
 
@@ -15876,15 +15997,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_2VM_close(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 895, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_2VM_close(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 898, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15893,15 +16014,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":902
+/* "unqlite.pyx":905
  *             self.vm = <unqlite_vm *>0
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.compile()
  *         return self
  */
 
@@ -15923,38 +16044,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "unqlite.pyx":903
+  /* "unqlite.pyx":906
  * 
  *     def __enter__(self):
  *         self.compile()             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->compile(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 903, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->compile(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":904
+  /* "unqlite.pyx":907
  *     def __enter__(self):
  *         self.compile()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":902
+  /* "unqlite.pyx":905
  *             self.vm = <unqlite_vm *>0
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         self.compile()
  *         return self
  */
 
@@ -15965,15 +16086,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":906
+/* "unqlite.pyx":909
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -16010,40 +16131,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 906, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 909, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_tb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 906, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 909, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 906, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 909, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 906, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 909, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.VM.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_2VM_14__exit__(((struct __pyx_obj_7unqlite_VM *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_val, __pyx_v_exc_tb);
 
@@ -16057,26 +16178,26 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "unqlite.pyx":907
+  /* "unqlite.pyx":910
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value* create_value(self, value):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 907, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 910, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":906
+  /* "unqlite.pyx":909
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -16089,15 +16210,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":909
+/* "unqlite.pyx":912
  *         self.close()
  * 
  *     cdef unqlite_value* create_value(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Create an `unqlite_value` corresponding to the given Python value.
  */
 
@@ -16110,15 +16231,15 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_value", 0);
 
-  /* "unqlite.pyx":914
+  /* "unqlite.pyx":917
  *         """
  *         cdef unqlite_value *ptr
  *         if isinstance(value, (list, tuple, dict)):             # <<<<<<<<<<<<<<
  *             ptr = self.create_array()
  *         else:
  */
   __pyx_t_2 = PyList_Check(__pyx_v_value); 
@@ -16138,67 +16259,67 @@
   __pyx_t_2 = PyDict_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __pyx_t_3 = (__pyx_t_1 != 0);
   if (__pyx_t_3) {
 
-    /* "unqlite.pyx":915
+    /* "unqlite.pyx":918
  *         cdef unqlite_value *ptr
  *         if isinstance(value, (list, tuple, dict)):
  *             ptr = self.create_array()             # <<<<<<<<<<<<<<
  *         else:
  *             ptr = self.create_scalar()
  */
     __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->create_array(__pyx_v_self);
 
-    /* "unqlite.pyx":914
+    /* "unqlite.pyx":917
  *         """
  *         cdef unqlite_value *ptr
  *         if isinstance(value, (list, tuple, dict)):             # <<<<<<<<<<<<<<
  *             ptr = self.create_array()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":917
+  /* "unqlite.pyx":920
  *             ptr = self.create_array()
  *         else:
  *             ptr = self.create_scalar()             # <<<<<<<<<<<<<<
  *         python_to_unqlite_value(self, ptr, value)
  *         return ptr
  */
   /*else*/ {
     __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->create_scalar(__pyx_v_self);
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":918
+  /* "unqlite.pyx":921
  *         else:
  *             ptr = self.create_scalar()
  *         python_to_unqlite_value(self, ptr, value)             # <<<<<<<<<<<<<<
  *         return ptr
  * 
  */
-  __pyx_t_4 = __pyx_f_7unqlite_python_to_unqlite_value(__pyx_v_self, __pyx_v_ptr, __pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 918, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_7unqlite_python_to_unqlite_value(__pyx_v_self, __pyx_v_ptr, __pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 921, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "unqlite.pyx":919
+  /* "unqlite.pyx":922
  *             ptr = self.create_scalar()
  *         python_to_unqlite_value(self, ptr, value)
  *         return ptr             # <<<<<<<<<<<<<<
  * 
  *     cdef release_value(self, unqlite_value *ptr):
  */
   __pyx_r = __pyx_v_ptr;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":909
+  /* "unqlite.pyx":912
  *         self.close()
  * 
  *     cdef unqlite_value* create_value(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Create an `unqlite_value` corresponding to the given Python value.
  */
 
@@ -16208,15 +16329,15 @@
   __Pyx_WriteUnraisable("unqlite.VM.create_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":921
+/* "unqlite.pyx":924
  *         return ptr
  * 
  *     cdef release_value(self, unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *         """Release the given `unqlite_value`."""
  *         self.unqlite.check_call(unqlite_vm_release_value(self.vm, ptr))
  */
 
@@ -16225,26 +16346,26 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("release_value", 0);
 
-  /* "unqlite.pyx":923
+  /* "unqlite.pyx":926
  *     cdef release_value(self, unqlite_value *ptr):
  *         """Release the given `unqlite_value`."""
  *         self.unqlite.check_call(unqlite_vm_release_value(self.vm, ptr))             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value* create_array(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_release_value(__pyx_v_self->vm, __pyx_v_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 923, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_release_value(__pyx_v_self->vm, __pyx_v_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":921
+  /* "unqlite.pyx":924
  *         return ptr
  * 
  *     cdef release_value(self, unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *         """Release the given `unqlite_value`."""
  *         self.unqlite.check_call(unqlite_vm_release_value(self.vm, ptr))
  */
 
@@ -16257,89 +16378,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":925
+/* "unqlite.pyx":928
  *         self.unqlite.check_call(unqlite_vm_release_value(self.vm, ptr))
  * 
  *     cdef unqlite_value* create_array(self):             # <<<<<<<<<<<<<<
  *         return unqlite_vm_new_array(self.vm)
  * 
  */
 
 static unqlite_value *__pyx_f_7unqlite_2VM_create_array(struct __pyx_obj_7unqlite_VM *__pyx_v_self) {
   unqlite_value *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_array", 0);
 
-  /* "unqlite.pyx":926
+  /* "unqlite.pyx":929
  * 
  *     cdef unqlite_value* create_array(self):
  *         return unqlite_vm_new_array(self.vm)             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value* create_scalar(self):
  */
   __pyx_r = unqlite_vm_new_array(__pyx_v_self->vm);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":925
+  /* "unqlite.pyx":928
  *         self.unqlite.check_call(unqlite_vm_release_value(self.vm, ptr))
  * 
  *     cdef unqlite_value* create_array(self):             # <<<<<<<<<<<<<<
  *         return unqlite_vm_new_array(self.vm)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":928
+/* "unqlite.pyx":931
  *         return unqlite_vm_new_array(self.vm)
  * 
  *     cdef unqlite_value* create_scalar(self):             # <<<<<<<<<<<<<<
  *         return unqlite_vm_new_scalar(self.vm)
  * 
  */
 
 static unqlite_value *__pyx_f_7unqlite_2VM_create_scalar(struct __pyx_obj_7unqlite_VM *__pyx_v_self) {
   unqlite_value *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_scalar", 0);
 
-  /* "unqlite.pyx":929
+  /* "unqlite.pyx":932
  * 
  *     cdef unqlite_value* create_scalar(self):
  *         return unqlite_vm_new_scalar(self.vm)             # <<<<<<<<<<<<<<
  * 
  *     def set_value(self, name, value):
  */
   __pyx_r = unqlite_vm_new_scalar(__pyx_v_self->vm);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":928
+  /* "unqlite.pyx":931
  *         return unqlite_vm_new_array(self.vm)
  * 
  *     cdef unqlite_value* create_scalar(self):             # <<<<<<<<<<<<<<
  *         return unqlite_vm_new_scalar(self.vm)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":931
+/* "unqlite.pyx":934
  *         return unqlite_vm_new_scalar(self.vm)
  * 
  *     def set_value(self, name, value):             # <<<<<<<<<<<<<<
  *         """Set the value of a variable in the Jx9 script."""
  *         cdef unqlite_value *ptr
  */
 
@@ -16374,32 +16495,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_value", 1, 2, 2, 1); __PYX_ERR(0, 931, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_value", 1, 2, 2, 1); __PYX_ERR(0, 934, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_value") < 0)) __PYX_ERR(0, 931, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_value") < 0)) __PYX_ERR(0, 934, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_value = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 931, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 934, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.VM.set_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_2VM_16set_value(((struct __pyx_obj_7unqlite_VM *)__pyx_v_self), __pyx_v_name, __pyx_v_value);
 
@@ -16417,84 +16538,84 @@
   int __pyx_t_2;
   char const *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_value", 0);
 
-  /* "unqlite.pyx":934
+  /* "unqlite.pyx":937
  *         """Set the value of a variable in the Jx9 script."""
  *         cdef unqlite_value *ptr
  *         cdef bytes encoded_name = encode(name)             # <<<<<<<<<<<<<<
  * 
  *         # since Jx9 does not make a private copy of the name,
  */
-  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 934, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_encoded_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":938
+  /* "unqlite.pyx":941
  *         # since Jx9 does not make a private copy of the name,
  *         # we need to keep it alive by adding it to a set
  *         self.encoded_names.add(encoded_name)             # <<<<<<<<<<<<<<
  * 
  *         ptr = self.create_value(value)
  */
   if (unlikely(__pyx_v_self->encoded_names == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "add");
-    __PYX_ERR(0, 938, __pyx_L1_error)
+    __PYX_ERR(0, 941, __pyx_L1_error)
   }
-  __pyx_t_2 = PySet_Add(__pyx_v_self->encoded_names, __pyx_v_encoded_name); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 938, __pyx_L1_error)
+  __pyx_t_2 = PySet_Add(__pyx_v_self->encoded_names, __pyx_v_encoded_name); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 941, __pyx_L1_error)
 
-  /* "unqlite.pyx":940
+  /* "unqlite.pyx":943
  *         self.encoded_names.add(encoded_name)
  * 
  *         ptr = self.create_value(value)             # <<<<<<<<<<<<<<
  *         self.unqlite.check_call(unqlite_vm_config(
  *             self.vm,
  */
   __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->create_value(__pyx_v_self, __pyx_v_value);
 
-  /* "unqlite.pyx":944
+  /* "unqlite.pyx":947
  *             self.vm,
  *             UNQLITE_VM_CONFIG_CREATE_VAR,
  *             <const char *>encoded_name,             # <<<<<<<<<<<<<<
  *             ptr))
  *         # since Jx9 makes a private copy of the value,
  */
   if (unlikely(__pyx_v_encoded_name == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 944, __pyx_L1_error)
+    __PYX_ERR(0, 947, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyBytes_AsString(__pyx_v_encoded_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsString(__pyx_v_encoded_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 947, __pyx_L1_error)
 
-  /* "unqlite.pyx":941
+  /* "unqlite.pyx":944
  * 
  *         ptr = self.create_value(value)
  *         self.unqlite.check_call(unqlite_vm_config(             # <<<<<<<<<<<<<<
  *             self.vm,
  *             UNQLITE_VM_CONFIG_CREATE_VAR,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_config(__pyx_v_self->vm, UNQLITE_VM_CONFIG_CREATE_VAR, ((char const *)__pyx_t_3), __pyx_v_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 941, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_UnQLite *)__pyx_v_self->unqlite->__pyx_vtab)->check_call(__pyx_v_self->unqlite, unqlite_vm_config(__pyx_v_self->vm, UNQLITE_VM_CONFIG_CREATE_VAR, ((char const *)__pyx_t_3), __pyx_v_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":948
+  /* "unqlite.pyx":951
  *         # since Jx9 makes a private copy of the value,
  *         # we do not need to keep the value alive
  *         self.release_value(ptr)             # <<<<<<<<<<<<<<
  * 
  *     def get_value(self, name):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 948, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":931
+  /* "unqlite.pyx":934
  *         return unqlite_vm_new_scalar(self.vm)
  * 
  *     def set_value(self, name, value):             # <<<<<<<<<<<<<<
  *         """Set the value of a variable in the Jx9 script."""
  *         cdef unqlite_value *ptr
  */
 
@@ -16508,15 +16629,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_encoded_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":950
+/* "unqlite.pyx":953
  *         self.release_value(ptr)
  * 
  *     def get_value(self, name):             # <<<<<<<<<<<<<<
  *         """
  *         Retrieve the value of a variable after the execution of the
  */
 
@@ -16552,97 +16673,97 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_value", 0);
 
-  /* "unqlite.pyx":956
+  /* "unqlite.pyx":959
  *         """
  *         cdef unqlite_value *ptr
  *         cdef bytes encoded_name = encode(name)             # <<<<<<<<<<<<<<
  * 
  *         ptr = unqlite_vm_extract_variable(self.vm, <const char *>encoded_name)
  */
-  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 956, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_encode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 959, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_encoded_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":958
+  /* "unqlite.pyx":961
  *         cdef bytes encoded_name = encode(name)
  * 
  *         ptr = unqlite_vm_extract_variable(self.vm, <const char *>encoded_name)             # <<<<<<<<<<<<<<
  *         if not ptr:
  *             raise KeyError(name)
  */
   if (unlikely(__pyx_v_encoded_name == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 958, __pyx_L1_error)
+    __PYX_ERR(0, 961, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_encoded_name); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 958, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_encoded_name); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 961, __pyx_L1_error)
   __pyx_v_ptr = unqlite_vm_extract_variable(__pyx_v_self->vm, ((char const *)__pyx_t_2));
 
-  /* "unqlite.pyx":959
+  /* "unqlite.pyx":962
  * 
  *         ptr = unqlite_vm_extract_variable(self.vm, <const char *>encoded_name)
  *         if not ptr:             # <<<<<<<<<<<<<<
  *             raise KeyError(name)
  *         try:
  */
   __pyx_t_3 = ((!(__pyx_v_ptr != 0)) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "unqlite.pyx":960
+    /* "unqlite.pyx":963
  *         ptr = unqlite_vm_extract_variable(self.vm, <const char *>encoded_name)
  *         if not ptr:
  *             raise KeyError(name)             # <<<<<<<<<<<<<<
  *         try:
  *             return unqlite_value_to_python(ptr)
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 960, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 960, __pyx_L1_error)
+    __PYX_ERR(0, 963, __pyx_L1_error)
 
-    /* "unqlite.pyx":959
+    /* "unqlite.pyx":962
  * 
  *         ptr = unqlite_vm_extract_variable(self.vm, <const char *>encoded_name)
  *         if not ptr:             # <<<<<<<<<<<<<<
  *             raise KeyError(name)
  *         try:
  */
   }
 
-  /* "unqlite.pyx":961
+  /* "unqlite.pyx":964
  *         if not ptr:
  *             raise KeyError(name)
  *         try:             # <<<<<<<<<<<<<<
  *             return unqlite_value_to_python(ptr)
  *         finally:
  */
   /*try:*/ {
 
-    /* "unqlite.pyx":962
+    /* "unqlite.pyx":965
  *             raise KeyError(name)
  *         try:
  *             return unqlite_value_to_python(ptr)             # <<<<<<<<<<<<<<
  *         finally:
  *             self.release_value(ptr)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 962, __pyx_L5_error)
+    __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 965, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L4_return;
   }
 
-  /* "unqlite.pyx":964
+  /* "unqlite.pyx":967
  *             return unqlite_value_to_python(ptr)
  *         finally:
  *             self.release_value(ptr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, name):
  */
   /*finally:*/ {
@@ -16658,15 +16779,15 @@
       __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       __pyx_t_4 = __pyx_lineno; __pyx_t_5 = __pyx_clineno; __pyx_t_6 = __pyx_filename;
       {
-        __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 964, __pyx_L8_error)
+        __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 967, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_XGIVEREF(__pyx_t_12);
@@ -16691,24 +16812,24 @@
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
       goto __pyx_L1_error;
     }
     __pyx_L4_return: {
       __pyx_t_12 = __pyx_r;
       __pyx_r = 0;
-      __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 964, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 967, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_r = __pyx_t_12;
       __pyx_t_12 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "unqlite.pyx":950
+  /* "unqlite.pyx":953
  *         self.release_value(ptr)
  * 
  *     def get_value(self, name):             # <<<<<<<<<<<<<<
  *         """
  *         Retrieve the value of a variable after the execution of the
  */
 
@@ -16720,15 +16841,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_encoded_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":966
+/* "unqlite.pyx":969
  *             self.release_value(ptr)
  * 
  *     def __getitem__(self, name):             # <<<<<<<<<<<<<<
  *         return self.get_value(name)
  * 
  */
 
@@ -16752,44 +16873,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "unqlite.pyx":967
+  /* "unqlite.pyx":970
  * 
  *     def __getitem__(self, name):
  *         return self.get_value(name)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, name, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 967, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 967, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":966
+  /* "unqlite.pyx":969
  *             self.release_value(ptr)
  * 
  *     def __getitem__(self, name):             # <<<<<<<<<<<<<<
  *         return self.get_value(name)
  * 
  */
 
@@ -16802,15 +16923,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":969
+/* "unqlite.pyx":972
  *         return self.get_value(name)
  * 
  *     def __setitem__(self, name, value):             # <<<<<<<<<<<<<<
  *         self.set_value(name, value)
  * 
  */
 
@@ -16836,22 +16957,22 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
-  /* "unqlite.pyx":970
+  /* "unqlite.pyx":973
  * 
  *     def __setitem__(self, name, value):
  *         self.set_value(name, value)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set_values(self, dict data):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -16860,47 +16981,47 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_name, __pyx_v_value};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_name, __pyx_v_value};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_name);
     __Pyx_GIVEREF(__pyx_v_name);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_name);
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_value);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":969
+  /* "unqlite.pyx":972
  *         return self.get_value(name)
  * 
  *     def __setitem__(self, name, value):             # <<<<<<<<<<<<<<
  *         self.set_value(name, value)
  * 
  */
 
@@ -16915,15 +17036,15 @@
   __Pyx_AddTraceback("unqlite.VM.__setitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":972
+/* "unqlite.pyx":975
  *         self.set_value(name, value)
  * 
  *     cpdef set_values(self, dict data):             # <<<<<<<<<<<<<<
  *         for key, value in data.items():
  *             self.set_value(key, value)
  */
 
@@ -16951,15 +17072,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 972, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 975, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_2VM_25set_values)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -16968,15 +17089,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_data);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 972, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -16989,50 +17110,50 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":973
+  /* "unqlite.pyx":976
  * 
  *     cpdef set_values(self, dict data):
  *         for key, value in data.items():             # <<<<<<<<<<<<<<
  *             self.set_value(key, value)
  * 
  */
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 973, __pyx_L1_error)
+    __PYX_ERR(0, 976, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_data, 1, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_data, 1, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 976, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_2;
   __pyx_t_2 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_6, &__pyx_t_5, &__pyx_t_2, &__pyx_t_3, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 973, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 976, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":974
+    /* "unqlite.pyx":977
  *     cpdef set_values(self, dict data):
  *         for key, value in data.items():
  *             self.set_value(key, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 974, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 977, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17041,49 +17162,49 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_key, __pyx_v_value};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 977, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_key, __pyx_v_value};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 977, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 974, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 977, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_key);
       __Pyx_GIVEREF(__pyx_v_key);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_key);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_value);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 977, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":972
+  /* "unqlite.pyx":975
  *         self.set_value(name, value)
  * 
  *     cpdef set_values(self, dict data):             # <<<<<<<<<<<<<<
  *         for key, value in data.items():
  *             self.set_value(key, value)
  */
 
@@ -17111,15 +17232,15 @@
 static PyObject *__pyx_pw_7unqlite_2VM_25set_values(PyObject *__pyx_v_self, PyObject *__pyx_v_data) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_values (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyDict_Type), 1, "data", 1))) __PYX_ERR(0, 972, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyDict_Type), 1, "data", 1))) __PYX_ERR(0, 975, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_2VM_24set_values(((struct __pyx_obj_7unqlite_VM *)__pyx_v_self), ((PyObject*)__pyx_v_data));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17132,15 +17253,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_values", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_2VM_set_values(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 972, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_2VM_set_values(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17149,15 +17270,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":852
+/* "unqlite.pyx":855
  *     cdef UnQLite unqlite
  *     cdef unqlite_vm *vm
  *     cdef readonly bint need_reset             # <<<<<<<<<<<<<<
  *     cdef readonly code
  *     cdef readonly bytes encoded_code
  */
 
@@ -17179,15 +17300,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->need_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 852, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->need_reset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17196,15 +17317,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":853
+/* "unqlite.pyx":856
  *     cdef unqlite_vm *vm
  *     cdef readonly bint need_reset
  *     cdef readonly code             # <<<<<<<<<<<<<<
  *     cdef readonly bytes encoded_code
  *     cdef set encoded_names
  */
 
@@ -17233,15 +17354,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":854
+/* "unqlite.pyx":857
  *     cdef readonly bint need_reset
  *     cdef readonly code
  *     cdef readonly bytes encoded_code             # <<<<<<<<<<<<<<
  *     cdef set encoded_names
  * 
  */
 
@@ -17383,15 +17504,15 @@
   __Pyx_AddTraceback("unqlite.VM.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":980
+/* "unqlite.pyx":983
  *     cdef unqlite_context *context
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.context = NULL
  * 
  */
 
@@ -17412,75 +17533,75 @@
 }
 
 static int __pyx_pf_7unqlite_7Context___cinit__(struct __pyx_obj_7unqlite_Context *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "unqlite.pyx":981
+  /* "unqlite.pyx":984
  * 
  *     def __cinit__(self):
  *         self.context = NULL             # <<<<<<<<<<<<<<
  * 
  *     cdef set_context(self, unqlite_context *context):
  */
   __pyx_v_self->context = NULL;
 
-  /* "unqlite.pyx":980
+  /* "unqlite.pyx":983
  *     cdef unqlite_context *context
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.context = NULL
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":983
+/* "unqlite.pyx":986
  *         self.context = NULL
  * 
  *     cdef set_context(self, unqlite_context *context):             # <<<<<<<<<<<<<<
  *         self.context = context
  * 
  */
 
 static PyObject *__pyx_f_7unqlite_7Context_set_context(struct __pyx_obj_7unqlite_Context *__pyx_v_self, unqlite_context *__pyx_v_context) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_context", 0);
 
-  /* "unqlite.pyx":984
+  /* "unqlite.pyx":987
  * 
  *     cdef set_context(self, unqlite_context *context):
  *         self.context = context             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value * create_value(self, value):
  */
   __pyx_v_self->context = __pyx_v_context;
 
-  /* "unqlite.pyx":983
+  /* "unqlite.pyx":986
  *         self.context = NULL
  * 
  *     cdef set_context(self, unqlite_context *context):             # <<<<<<<<<<<<<<
  *         self.context = context
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":986
+/* "unqlite.pyx":989
  *         self.context = context
  * 
  *     cdef unqlite_value * create_value(self, value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *ptr
  * 
  */
 
@@ -17493,15 +17614,15 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_value", 0);
 
-  /* "unqlite.pyx":989
+  /* "unqlite.pyx":992
  *         cdef unqlite_value *ptr
  * 
  *         if isinstance(value, (list, tuple, dict)):             # <<<<<<<<<<<<<<
  *             ptr = self.create_array()
  *         else:
  */
   __pyx_t_2 = PyList_Check(__pyx_v_value); 
@@ -17521,67 +17642,67 @@
   __pyx_t_2 = PyDict_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __pyx_t_3 = (__pyx_t_1 != 0);
   if (__pyx_t_3) {
 
-    /* "unqlite.pyx":990
+    /* "unqlite.pyx":993
  * 
  *         if isinstance(value, (list, tuple, dict)):
  *             ptr = self.create_array()             # <<<<<<<<<<<<<<
  *         else:
  *             ptr = self.create_scalar()
  */
     __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->create_array(__pyx_v_self);
 
-    /* "unqlite.pyx":989
+    /* "unqlite.pyx":992
  *         cdef unqlite_value *ptr
  * 
  *         if isinstance(value, (list, tuple, dict)):             # <<<<<<<<<<<<<<
  *             ptr = self.create_array()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":992
+  /* "unqlite.pyx":995
  *             ptr = self.create_array()
  *         else:
  *             ptr = self.create_scalar()             # <<<<<<<<<<<<<<
  * 
  *         self.python_to_unqlite_value(ptr, value)
  */
   /*else*/ {
     __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->create_scalar(__pyx_v_self);
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":994
+  /* "unqlite.pyx":997
  *             ptr = self.create_scalar()
  * 
  *         self.python_to_unqlite_value(ptr, value)             # <<<<<<<<<<<<<<
  *         return ptr
  * 
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->python_to_unqlite_value(__pyx_v_self, __pyx_v_ptr, __pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 994, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->python_to_unqlite_value(__pyx_v_self, __pyx_v_ptr, __pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "unqlite.pyx":995
+  /* "unqlite.pyx":998
  * 
  *         self.python_to_unqlite_value(ptr, value)
  *         return ptr             # <<<<<<<<<<<<<<
  * 
  *     cdef release_value(self, unqlite_value *ptr):
  */
   __pyx_r = __pyx_v_ptr;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":986
+  /* "unqlite.pyx":989
  *         self.context = context
  * 
  *     cdef unqlite_value * create_value(self, value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *ptr
  * 
  */
 
@@ -17591,126 +17712,126 @@
   __Pyx_WriteUnraisable("unqlite.Context.create_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":997
+/* "unqlite.pyx":1000
  *         return ptr
  * 
  *     cdef release_value(self, unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *         unqlite_context_release_value(self.context, ptr)
  * 
  */
 
 static PyObject *__pyx_f_7unqlite_7Context_release_value(struct __pyx_obj_7unqlite_Context *__pyx_v_self, unqlite_value *__pyx_v_ptr) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("release_value", 0);
 
-  /* "unqlite.pyx":998
+  /* "unqlite.pyx":1001
  * 
  *     cdef release_value(self, unqlite_value *ptr):
  *         unqlite_context_release_value(self.context, ptr)             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value* create_array(self):
  */
   unqlite_context_release_value(__pyx_v_self->context, __pyx_v_ptr);
 
-  /* "unqlite.pyx":997
+  /* "unqlite.pyx":1000
  *         return ptr
  * 
  *     cdef release_value(self, unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *         unqlite_context_release_value(self.context, ptr)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1000
+/* "unqlite.pyx":1003
  *         unqlite_context_release_value(self.context, ptr)
  * 
  *     cdef unqlite_value* create_array(self):             # <<<<<<<<<<<<<<
  *         return unqlite_context_new_array(self.context)
  * 
  */
 
 static unqlite_value *__pyx_f_7unqlite_7Context_create_array(struct __pyx_obj_7unqlite_Context *__pyx_v_self) {
   unqlite_value *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_array", 0);
 
-  /* "unqlite.pyx":1001
+  /* "unqlite.pyx":1004
  * 
  *     cdef unqlite_value* create_array(self):
  *         return unqlite_context_new_array(self.context)             # <<<<<<<<<<<<<<
  * 
  *     cdef unqlite_value* create_scalar(self):
  */
   __pyx_r = unqlite_context_new_array(__pyx_v_self->context);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1000
+  /* "unqlite.pyx":1003
  *         unqlite_context_release_value(self.context, ptr)
  * 
  *     cdef unqlite_value* create_array(self):             # <<<<<<<<<<<<<<
  *         return unqlite_context_new_array(self.context)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1003
+/* "unqlite.pyx":1006
  *         return unqlite_context_new_array(self.context)
  * 
  *     cdef unqlite_value* create_scalar(self):             # <<<<<<<<<<<<<<
  *         return unqlite_context_new_scalar(self.context)
  * 
  */
 
 static unqlite_value *__pyx_f_7unqlite_7Context_create_scalar(struct __pyx_obj_7unqlite_Context *__pyx_v_self) {
   unqlite_value *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_scalar", 0);
 
-  /* "unqlite.pyx":1004
+  /* "unqlite.pyx":1007
  * 
  *     cdef unqlite_value* create_scalar(self):
  *         return unqlite_context_new_scalar(self.context)             # <<<<<<<<<<<<<<
  * 
  *     cpdef push_result(self, value):
  */
   __pyx_r = unqlite_context_new_scalar(__pyx_v_self->context);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1003
+  /* "unqlite.pyx":1006
  *         return unqlite_context_new_array(self.context)
  * 
  *     cdef unqlite_value* create_scalar(self):             # <<<<<<<<<<<<<<
  *         return unqlite_context_new_scalar(self.context)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1006
+/* "unqlite.pyx":1009
  *         return unqlite_context_new_scalar(self.context)
  * 
  *     cpdef push_result(self, value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *ptr
  *         ptr = self.create_value(value)
  */
 
@@ -17732,15 +17853,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_push_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1006, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_push_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1009, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_7Context_3push_result)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -17749,15 +17870,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1006, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1009, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -17770,44 +17891,44 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":1008
+  /* "unqlite.pyx":1011
  *     cpdef push_result(self, value):
  *         cdef unqlite_value *ptr
  *         ptr = self.create_value(value)             # <<<<<<<<<<<<<<
  *         unqlite_result_value(self.context, ptr)
  *         self.release_value(ptr)
  */
   __pyx_v_ptr = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->create_value(__pyx_v_self, __pyx_v_value);
 
-  /* "unqlite.pyx":1009
+  /* "unqlite.pyx":1012
  *         cdef unqlite_value *ptr
  *         ptr = self.create_value(value)
  *         unqlite_result_value(self.context, ptr)             # <<<<<<<<<<<<<<
  *         self.release_value(ptr)
  * 
  */
   (void)(unqlite_result_value(__pyx_v_self->context, __pyx_v_ptr));
 
-  /* "unqlite.pyx":1010
+  /* "unqlite.pyx":1013
  *         ptr = self.create_value(value)
  *         unqlite_result_value(self.context, ptr)
  *         self.release_value(ptr)             # <<<<<<<<<<<<<<
  * 
  *     cdef python_to_unqlite_value(self, unqlite_value *ptr, python_value):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1010, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1006
+  /* "unqlite.pyx":1009
  *         return unqlite_context_new_scalar(self.context)
  * 
  *     cpdef push_result(self, value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *ptr
  *         ptr = self.create_value(value)
  */
 
@@ -17845,15 +17966,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push_result", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_7Context_push_result(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1006, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_7Context_push_result(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17862,15 +17983,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1012
+/* "unqlite.pyx":1015
  *         self.release_value(ptr)
  * 
  *     cdef python_to_unqlite_value(self, unqlite_value *ptr, python_value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *item_ptr = <unqlite_value *>0
  *         cdef bytes encoded_value
  */
 
@@ -17898,102 +18019,102 @@
   unqlite_int64 __pyx_t_14;
   double __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("python_to_unqlite_value", 0);
 
-  /* "unqlite.pyx":1013
+  /* "unqlite.pyx":1016
  * 
  *     cdef python_to_unqlite_value(self, unqlite_value *ptr, python_value):
  *         cdef unqlite_value *item_ptr = <unqlite_value *>0             # <<<<<<<<<<<<<<
  *         cdef bytes encoded_value
  * 
  */
   __pyx_v_item_ptr = ((unqlite_value *)0);
 
-  /* "unqlite.pyx":1016
+  /* "unqlite.pyx":1019
  *         cdef bytes encoded_value
  * 
  *         if isinstance(python_value, unicode):             # <<<<<<<<<<<<<<
  *             encoded_value = encode(python_value)
  *             unqlite_value_string(ptr, encoded_value, -1)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1017
+    /* "unqlite.pyx":1020
  * 
  *         if isinstance(python_value, unicode):
  *             encoded_value = encode(python_value)             # <<<<<<<<<<<<<<
  *             unqlite_value_string(ptr, encoded_value, -1)
  *         elif isinstance(python_value, bytes):
  */
-    __pyx_t_3 = __pyx_f_7unqlite_encode(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1017, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_7unqlite_encode(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1020, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_encoded_value = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1018
+    /* "unqlite.pyx":1021
  *         if isinstance(python_value, unicode):
  *             encoded_value = encode(python_value)
  *             unqlite_value_string(ptr, encoded_value, -1)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, bytes):
  *             unqlite_value_string(ptr, python_value, -1)
  */
     if (unlikely(__pyx_v_encoded_value == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 1018, __pyx_L1_error)
+      __PYX_ERR(0, 1021, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1018, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1021, __pyx_L1_error)
     (void)(unqlite_value_string(__pyx_v_ptr, __pyx_t_4, -1));
 
-    /* "unqlite.pyx":1016
+    /* "unqlite.pyx":1019
  *         cdef bytes encoded_value
  * 
  *         if isinstance(python_value, unicode):             # <<<<<<<<<<<<<<
  *             encoded_value = encode(python_value)
  *             unqlite_value_string(ptr, encoded_value, -1)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1019
+  /* "unqlite.pyx":1022
  *             encoded_value = encode(python_value)
  *             unqlite_value_string(ptr, encoded_value, -1)
  *         elif isinstance(python_value, bytes):             # <<<<<<<<<<<<<<
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1020
+    /* "unqlite.pyx":1023
  *             unqlite_value_string(ptr, encoded_value, -1)
  *         elif isinstance(python_value, bytes):
  *             unqlite_value_string(ptr, python_value, -1)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, (list, tuple)):
  *             for item in python_value:
  */
-    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_v_python_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1020, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_v_python_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1023, __pyx_L1_error)
     (void)(unqlite_value_string(__pyx_v_ptr, __pyx_t_4, -1));
 
-    /* "unqlite.pyx":1019
+    /* "unqlite.pyx":1022
  *             encoded_value = encode(python_value)
  *             unqlite_value_string(ptr, encoded_value, -1)
  *         elif isinstance(python_value, bytes):             # <<<<<<<<<<<<<<
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1021
+  /* "unqlite.pyx":1024
  *         elif isinstance(python_value, bytes):
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):             # <<<<<<<<<<<<<<
  *             for item in python_value:
  *                 item_ptr = self.create_value(item)
  */
   __pyx_t_2 = PyList_Check(__pyx_v_python_value); 
@@ -18006,252 +18127,252 @@
   __pyx_t_5 = PyTuple_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_5 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1022
+    /* "unqlite.pyx":1025
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):
  *             for item in python_value:             # <<<<<<<<<<<<<<
  *                 item_ptr = self.create_value(item)
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  */
     if (likely(PyList_CheckExact(__pyx_v_python_value)) || PyTuple_CheckExact(__pyx_v_python_value)) {
       __pyx_t_3 = __pyx_v_python_value; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1022, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1025, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1022, __pyx_L1_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1025, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1022, __pyx_L1_error)
+          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1025, __pyx_L1_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1022, __pyx_L1_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1025, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1022, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1025, __pyx_L1_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1022, __pyx_L1_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1025, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         }
       } else {
         __pyx_t_8 = __pyx_t_7(__pyx_t_3);
         if (unlikely(!__pyx_t_8)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 1022, __pyx_L1_error)
+            else __PYX_ERR(0, 1025, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_8);
       }
       __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_8);
       __pyx_t_8 = 0;
 
-      /* "unqlite.pyx":1023
+      /* "unqlite.pyx":1026
  *         elif isinstance(python_value, (list, tuple)):
  *             for item in python_value:
  *                 item_ptr = self.create_value(item)             # <<<<<<<<<<<<<<
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  *                 self.release_value(item_ptr)
  */
       __pyx_v_item_ptr = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->create_value(__pyx_v_self, __pyx_v_item);
 
-      /* "unqlite.pyx":1024
+      /* "unqlite.pyx":1027
  *             for item in python_value:
  *                 item_ptr = self.create_value(item)
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)             # <<<<<<<<<<<<<<
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, dict):
  */
       (void)(unqlite_array_add_elem(__pyx_v_ptr, NULL, __pyx_v_item_ptr));
 
-      /* "unqlite.pyx":1025
+      /* "unqlite.pyx":1028
  *                 item_ptr = self.create_value(item)
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  *                 self.release_value(item_ptr)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, dict):
  *             for key, value in python_value.items():
  */
-      __pyx_t_8 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_item_ptr); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1025, __pyx_L1_error)
+      __pyx_t_8 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_item_ptr); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1028, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "unqlite.pyx":1022
+      /* "unqlite.pyx":1025
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):
  *             for item in python_value:             # <<<<<<<<<<<<<<
  *                 item_ptr = self.create_value(item)
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1021
+    /* "unqlite.pyx":1024
  *         elif isinstance(python_value, bytes):
  *             unqlite_value_string(ptr, python_value, -1)
  *         elif isinstance(python_value, (list, tuple)):             # <<<<<<<<<<<<<<
  *             for item in python_value:
  *                 item_ptr = self.create_value(item)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1026
+  /* "unqlite.pyx":1029
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, dict):             # <<<<<<<<<<<<<<
  *             for key, value in python_value.items():
  *                 encoded_value = encode(key)
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1027
+    /* "unqlite.pyx":1030
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, dict):
  *             for key, value in python_value.items():             # <<<<<<<<<<<<<<
  *                 encoded_value = encode(key)
  *                 item_ptr = self.create_value(value)
  */
     __pyx_t_6 = 0;
     if (unlikely(__pyx_v_python_value == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 1027, __pyx_L1_error)
+      __PYX_ERR(0, 1030, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_python_value, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1027, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_python_value, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1030, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_8;
     __pyx_t_8 = 0;
     while (1) {
       __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_9, &__pyx_t_6, &__pyx_t_8, &__pyx_t_11, NULL, __pyx_t_10);
       if (unlikely(__pyx_t_12 == 0)) break;
-      if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1027, __pyx_L1_error)
+      if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1030, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "unqlite.pyx":1028
+      /* "unqlite.pyx":1031
  *         elif isinstance(python_value, dict):
  *             for key, value in python_value.items():
  *                 encoded_value = encode(key)             # <<<<<<<<<<<<<<
  *                 item_ptr = self.create_value(value)
  *                 unqlite_array_add_strkey_elem(
  */
-      __pyx_t_11 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1028, __pyx_L1_error)
+      __pyx_t_11 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1031, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_XDECREF_SET(__pyx_v_encoded_value, ((PyObject*)__pyx_t_11));
       __pyx_t_11 = 0;
 
-      /* "unqlite.pyx":1029
+      /* "unqlite.pyx":1032
  *             for key, value in python_value.items():
  *                 encoded_value = encode(key)
  *                 item_ptr = self.create_value(value)             # <<<<<<<<<<<<<<
  *                 unqlite_array_add_strkey_elem(
  *                     ptr,
  */
       __pyx_v_item_ptr = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->create_value(__pyx_v_self, __pyx_v_value);
 
-      /* "unqlite.pyx":1032
+      /* "unqlite.pyx":1035
  *                 unqlite_array_add_strkey_elem(
  *                     ptr,
  *                     <const char *>encoded_value,             # <<<<<<<<<<<<<<
  *                     item_ptr)
  *                 self.release_value(item_ptr)
  */
       if (unlikely(__pyx_v_encoded_value == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-        __PYX_ERR(0, 1032, __pyx_L1_error)
+        __PYX_ERR(0, 1035, __pyx_L1_error)
       }
-      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 1032, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 1035, __pyx_L1_error)
 
-      /* "unqlite.pyx":1030
+      /* "unqlite.pyx":1033
  *                 encoded_value = encode(key)
  *                 item_ptr = self.create_value(value)
  *                 unqlite_array_add_strkey_elem(             # <<<<<<<<<<<<<<
  *                     ptr,
  *                     <const char *>encoded_value,
  */
       (void)(unqlite_array_add_strkey_elem(__pyx_v_ptr, ((char const *)__pyx_t_13), __pyx_v_item_ptr));
 
-      /* "unqlite.pyx":1034
+      /* "unqlite.pyx":1037
  *                     <const char *>encoded_value,
  *                     item_ptr)
  *                 self.release_value(item_ptr)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, bool):
  *             unqlite_value_bool(ptr, python_value)
  */
-      __pyx_t_11 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_item_ptr); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1034, __pyx_L1_error)
+      __pyx_t_11 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_self->__pyx_vtab)->release_value(__pyx_v_self, __pyx_v_item_ptr); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1037, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1026
+    /* "unqlite.pyx":1029
  *                 unqlite_array_add_elem(ptr, NULL, item_ptr)
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, dict):             # <<<<<<<<<<<<<<
  *             for key, value in python_value.items():
  *                 encoded_value = encode(key)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1035
+  /* "unqlite.pyx":1038
  *                     item_ptr)
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, bool):             # <<<<<<<<<<<<<<
  *             unqlite_value_bool(ptr, python_value)
  *         elif isinstance(python_value, (int, long)):
  */
   __pyx_t_3 = ((PyObject*)&PyBool_Type);
   __Pyx_INCREF(__pyx_t_3);
-  __pyx_t_1 = PyObject_IsInstance(__pyx_v_python_value, __pyx_t_3); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1035, __pyx_L1_error)
+  __pyx_t_1 = PyObject_IsInstance(__pyx_v_python_value, __pyx_t_3); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1038, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1036
+    /* "unqlite.pyx":1039
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, bool):
  *             unqlite_value_bool(ptr, python_value)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, (int, long)):
  *             unqlite_value_int64(ptr, python_value)
  */
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_python_value); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1036, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_python_value); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1039, __pyx_L1_error)
     (void)(unqlite_value_bool(__pyx_v_ptr, __pyx_t_10));
 
-    /* "unqlite.pyx":1035
+    /* "unqlite.pyx":1038
  *                     item_ptr)
  *                 self.release_value(item_ptr)
  *         elif isinstance(python_value, bool):             # <<<<<<<<<<<<<<
  *             unqlite_value_bool(ptr, python_value)
  *         elif isinstance(python_value, (int, long)):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1037
+  /* "unqlite.pyx":1040
  *         elif isinstance(python_value, bool):
  *             unqlite_value_bool(ptr, python_value)
  *         elif isinstance(python_value, (int, long)):             # <<<<<<<<<<<<<<
  *             unqlite_value_int64(ptr, python_value)
  *         elif isinstance(python_value, float):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_python_value); 
@@ -18264,78 +18385,78 @@
   __pyx_t_5 = PyLong_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L10_bool_binop_done:;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1038
+    /* "unqlite.pyx":1041
  *             unqlite_value_bool(ptr, python_value)
  *         elif isinstance(python_value, (int, long)):
  *             unqlite_value_int64(ptr, python_value)             # <<<<<<<<<<<<<<
  *         elif isinstance(python_value, float):
  *             unqlite_value_double(ptr, python_value)
  */
-    __pyx_t_14 = __Pyx_PyInt_As_sxi64(__pyx_v_python_value); if (unlikely((__pyx_t_14 == ((unqlite_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1038, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_As_sxi64(__pyx_v_python_value); if (unlikely((__pyx_t_14 == ((unqlite_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1041, __pyx_L1_error)
     (void)(unqlite_value_int64(__pyx_v_ptr, __pyx_t_14));
 
-    /* "unqlite.pyx":1037
+    /* "unqlite.pyx":1040
  *         elif isinstance(python_value, bool):
  *             unqlite_value_bool(ptr, python_value)
  *         elif isinstance(python_value, (int, long)):             # <<<<<<<<<<<<<<
  *             unqlite_value_int64(ptr, python_value)
  *         elif isinstance(python_value, float):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1039
+  /* "unqlite.pyx":1042
  *         elif isinstance(python_value, (int, long)):
  *             unqlite_value_int64(ptr, python_value)
  *         elif isinstance(python_value, float):             # <<<<<<<<<<<<<<
  *             unqlite_value_double(ptr, python_value)
  *         else:
  */
   __pyx_t_1 = PyFloat_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1040
+    /* "unqlite.pyx":1043
  *             unqlite_value_int64(ptr, python_value)
  *         elif isinstance(python_value, float):
  *             unqlite_value_double(ptr, python_value)             # <<<<<<<<<<<<<<
  *         else:
  *             unqlite_value_null(ptr)
  */
-    __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_python_value); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1040, __pyx_L1_error)
+    __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_python_value); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1043, __pyx_L1_error)
     (void)(unqlite_value_double(__pyx_v_ptr, __pyx_t_15));
 
-    /* "unqlite.pyx":1039
+    /* "unqlite.pyx":1042
  *         elif isinstance(python_value, (int, long)):
  *             unqlite_value_int64(ptr, python_value)
  *         elif isinstance(python_value, float):             # <<<<<<<<<<<<<<
  *             unqlite_value_double(ptr, python_value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1042
+  /* "unqlite.pyx":1045
  *             unqlite_value_double(ptr, python_value)
  *         else:
  *             unqlite_value_null(ptr)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     (void)(unqlite_value_null(__pyx_v_ptr));
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":1012
+  /* "unqlite.pyx":1015
  *         self.release_value(ptr)
  * 
  *     cdef python_to_unqlite_value(self, unqlite_value *ptr, python_value):             # <<<<<<<<<<<<<<
  *         cdef unqlite_value *item_ptr = <unqlite_value *>0
  *         cdef bytes encoded_value
  */
 
@@ -18467,18 +18588,18 @@
   __Pyx_AddTraceback("unqlite.Context.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1045
+/* "unqlite.pyx":1048
  * 
  * 
- * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values):             # <<<<<<<<<<<<<<
+ * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef list converted = []
  */
 
 static int __pyx_f_7unqlite_py_filter_wrapper(unqlite_context *__pyx_v_context, int __pyx_v_nargs, unqlite_value **__pyx_v_values) {
   int __pyx_v_i;
   PyObject *__pyx_v_converted = 0;
@@ -18500,88 +18621,88 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_filter_wrapper", 0);
 
-  /* "unqlite.pyx":1047
- * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values):
+  /* "unqlite.pyx":1050
+ * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values) noexcept:
  *     cdef int i
  *     cdef list converted = []             # <<<<<<<<<<<<<<
  *     cdef object callback = <object>unqlite_context_user_data(context)
  *     cdef Context context_wrapper = Context()
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1047, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_converted = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1048
+  /* "unqlite.pyx":1051
  *     cdef int i
  *     cdef list converted = []
  *     cdef object callback = <object>unqlite_context_user_data(context)             # <<<<<<<<<<<<<<
  *     cdef Context context_wrapper = Context()
  * 
  */
   __pyx_t_2 = unqlite_context_user_data(__pyx_v_context);
   __pyx_t_1 = ((PyObject *)__pyx_t_2);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_callback = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1049
+  /* "unqlite.pyx":1052
  *     cdef list converted = []
  *     cdef object callback = <object>unqlite_context_user_data(context)
  *     cdef Context context_wrapper = Context()             # <<<<<<<<<<<<<<
  * 
  *     context_wrapper.set_context(context)
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7unqlite_Context)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1049, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7unqlite_Context)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1052, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_context_wrapper = ((struct __pyx_obj_7unqlite_Context *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1051
+  /* "unqlite.pyx":1054
  *     cdef Context context_wrapper = Context()
  * 
  *     context_wrapper.set_context(context)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(nargs):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->set_context(__pyx_v_context_wrapper, __pyx_v_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1051, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->set_context(__pyx_v_context_wrapper, __pyx_v_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1053
+  /* "unqlite.pyx":1056
  *     context_wrapper.set_context(context)
  * 
  *     for i in range(nargs):             # <<<<<<<<<<<<<<
  *         converted.append(unqlite_value_to_python(values[i]))
  * 
  */
   __pyx_t_3 = __pyx_v_nargs;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "unqlite.pyx":1054
+    /* "unqlite.pyx":1057
  * 
  *     for i in range(nargs):
  *         converted.append(unqlite_value_to_python(values[i]))             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python((__pyx_v_values[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1054, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python((__pyx_v_values[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1057, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_converted, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 1054, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_converted, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 1057, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "unqlite.pyx":1056
+  /* "unqlite.pyx":1059
  *         converted.append(unqlite_value_to_python(values[i]))
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         ret = callback(*converted)
  *     except KeyError:
  */
   {
@@ -18589,105 +18710,105 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
     __Pyx_XGOTREF(__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_9);
     /*try:*/ {
 
-      /* "unqlite.pyx":1057
+      /* "unqlite.pyx":1060
  * 
  *     try:
  *         ret = callback(*converted)             # <<<<<<<<<<<<<<
  *     except KeyError:
  *         context_wrapper.push_result(False)
  */
-      __pyx_t_1 = PySequence_Tuple(__pyx_v_converted); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1057, __pyx_L5_error)
+      __pyx_t_1 = PySequence_Tuple(__pyx_v_converted); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1060, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_v_callback, __pyx_t_1, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1057, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_v_callback, __pyx_t_1, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1060, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_ret = __pyx_t_10;
       __pyx_t_10 = 0;
 
-      /* "unqlite.pyx":1056
+      /* "unqlite.pyx":1059
  *         converted.append(unqlite_value_to_python(values[i]))
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         ret = callback(*converted)
  *     except KeyError:
  */
     }
 
-    /* "unqlite.pyx":1063
+    /* "unqlite.pyx":1066
  *         return UNQLITE_ABORT
  *     else:
  *         context_wrapper.push_result(ret)             # <<<<<<<<<<<<<<
  *     return UNQLITE_OK
  * 
  */
     /*else:*/ {
-      __pyx_t_10 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->push_result(__pyx_v_context_wrapper, __pyx_v_ret, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1063, __pyx_L7_except_error)
+      __pyx_t_10 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->push_result(__pyx_v_context_wrapper, __pyx_v_ret, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1066, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     goto __pyx_L10_try_end;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-    /* "unqlite.pyx":1058
+    /* "unqlite.pyx":1061
  *     try:
  *         ret = callback(*converted)
  *     except KeyError:             # <<<<<<<<<<<<<<
  *         context_wrapper.push_result(False)
  *     except Exception:
  */
     __pyx_t_3 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_3) {
       __Pyx_AddTraceback("unqlite.py_filter_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_10, &__pyx_t_1, &__pyx_t_11) < 0) __PYX_ERR(0, 1058, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_10, &__pyx_t_1, &__pyx_t_11) < 0) __PYX_ERR(0, 1061, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_11);
 
-      /* "unqlite.pyx":1059
+      /* "unqlite.pyx":1062
  *         ret = callback(*converted)
  *     except KeyError:
  *         context_wrapper.push_result(False)             # <<<<<<<<<<<<<<
  *     except Exception:
  *         return UNQLITE_ABORT
  */
-      __pyx_t_12 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->push_result(__pyx_v_context_wrapper, Py_False, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1059, __pyx_L7_except_error)
+      __pyx_t_12 = ((struct __pyx_vtabstruct_7unqlite_Context *)__pyx_v_context_wrapper->__pyx_vtab)->push_result(__pyx_v_context_wrapper, Py_False, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1062, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       goto __pyx_L6_exception_handled;
     }
 
-    /* "unqlite.pyx":1060
+    /* "unqlite.pyx":1063
  *     except KeyError:
  *         context_wrapper.push_result(False)
  *     except Exception:             # <<<<<<<<<<<<<<
  *         return UNQLITE_ABORT
  *     else:
  */
     __pyx_t_3 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_3) {
       __Pyx_AddTraceback("unqlite.py_filter_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_1, &__pyx_t_10) < 0) __PYX_ERR(0, 1060, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_1, &__pyx_t_10) < 0) __PYX_ERR(0, 1063, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "unqlite.pyx":1061
+      /* "unqlite.pyx":1064
  *         context_wrapper.push_result(False)
  *     except Exception:
  *         return UNQLITE_ABORT             # <<<<<<<<<<<<<<
  *     else:
  *         context_wrapper.push_result(ret)
  */
       __pyx_r = UNQLITE_ABORT;
@@ -18695,15 +18816,15 @@
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       goto __pyx_L8_except_return;
     }
     goto __pyx_L7_except_error;
     __pyx_L7_except_error:;
 
-    /* "unqlite.pyx":1056
+    /* "unqlite.pyx":1059
  *         converted.append(unqlite_value_to_python(values[i]))
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         ret = callback(*converted)
  *     except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_7);
@@ -18721,28 +18842,28 @@
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_XGIVEREF(__pyx_t_8);
     __Pyx_XGIVEREF(__pyx_t_9);
     __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
     __pyx_L10_try_end:;
   }
 
-  /* "unqlite.pyx":1064
+  /* "unqlite.pyx":1067
  *     else:
  *         context_wrapper.push_result(ret)
  *     return UNQLITE_OK             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = UNQLITE_OK;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1045
+  /* "unqlite.pyx":1048
  * 
  * 
- * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values):             # <<<<<<<<<<<<<<
+ * cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef list converted = []
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -18756,15 +18877,15 @@
   __Pyx_XDECREF(__pyx_v_callback);
   __Pyx_XDECREF((PyObject *)__pyx_v_context_wrapper);
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1074
+/* "unqlite.pyx":1077
  *     cdef basestring name
  * 
  *     def __init__(self, UnQLite unqlite, basestring name):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.name = decode(name)
  */
 
@@ -18798,39 +18919,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unqlite)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 1074, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 1077, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1074, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1077, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)values[0]);
     __pyx_v_name = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1074, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1077, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Collection.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unqlite), __pyx_ptype_7unqlite_UnQLite, 1, "unqlite", 0))) __PYX_ERR(0, 1074, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyBaseString_Type), 1, "name", 1))) __PYX_ERR(0, 1074, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unqlite), __pyx_ptype_7unqlite_UnQLite, 1, "unqlite", 0))) __PYX_ERR(0, 1077, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyBaseString_Type), 1, "name", 1))) __PYX_ERR(0, 1077, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_10Collection___init__(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v_unqlite, __pyx_v_name);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -18843,43 +18964,43 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "unqlite.pyx":1075
+  /* "unqlite.pyx":1078
  * 
  *     def __init__(self, UnQLite unqlite, basestring name):
  *         self.unqlite = unqlite             # <<<<<<<<<<<<<<
  *         self.name = decode(name)
  * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_unqlite));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_unqlite));
   __Pyx_GOTREF(__pyx_v_self->unqlite);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->unqlite));
   __pyx_v_self->unqlite = __pyx_v_unqlite;
 
-  /* "unqlite.pyx":1076
+  /* "unqlite.pyx":1079
  *     def __init__(self, UnQLite unqlite, basestring name):
  *         self.unqlite = unqlite
  *         self.name = decode(name)             # <<<<<<<<<<<<<<
  * 
  *     def _execute(self, basestring script, **kwargs):
  */
-  __pyx_t_1 = __pyx_f_7unqlite_decode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1076, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_decode(__pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1079, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1074
+  /* "unqlite.pyx":1077
  *     cdef basestring name
  * 
  *     def __init__(self, UnQLite unqlite, basestring name):             # <<<<<<<<<<<<<<
  *         self.unqlite = unqlite
  *         self.name = decode(name)
  */
 
@@ -18891,15 +19012,15 @@
   __Pyx_AddTraceback("unqlite.Collection.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1078
+/* "unqlite.pyx":1081
  *         self.name = decode(name)
  * 
  *     def _execute(self, basestring script, **kwargs):             # <<<<<<<<<<<<<<
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  */
 
@@ -18931,33 +19052,33 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_script)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_execute") < 0)) __PYX_ERR(0, 1078, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_execute") < 0)) __PYX_ERR(0, 1081, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_script = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_execute", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1078, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_execute", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1081, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("unqlite.Collection._execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_script), (&PyBaseString_Type), 1, "script", 1))) __PYX_ERR(0, 1078, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_script), (&PyBaseString_Type), 1, "script", 1))) __PYX_ERR(0, 1081, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_10Collection_2_execute(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v_script, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -18982,103 +19103,103 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_execute", 0);
 
-  /* "unqlite.pyx":1080
+  /* "unqlite.pyx":1083
  *     def _execute(self, basestring script, **kwargs):
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  */
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1080, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1083, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)__pyx_v_self->unqlite));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self->unqlite));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self->unqlite));
     __Pyx_INCREF(__pyx_v_script);
     __Pyx_GIVEREF(__pyx_v_script);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_script);
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1080, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1083, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1080, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1083, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1080, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1083, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1080, __pyx_L3_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1083, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
-          if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1080, __pyx_L7_error)
+          if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1083, __pyx_L7_error)
           __pyx_v_vm = ((struct __pyx_obj_7unqlite_VM *)__pyx_t_4);
           __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1081
+          /* "unqlite.pyx":1084
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  *             vm['collection'] = self.name             # <<<<<<<<<<<<<<
  *             vm.set_values(kwargs)
  *             vm.execute()
  */
           __pyx_t_4 = __pyx_v_self->name;
           __Pyx_INCREF(__pyx_t_4);
-          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1081, __pyx_L7_error)
+          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1084, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1082
+          /* "unqlite.pyx":1085
  *         with VM(self.unqlite, script) as vm:
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)             # <<<<<<<<<<<<<<
  *             vm.execute()
  * 
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->set_values(__pyx_v_vm, __pyx_v_kwargs, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L7_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->set_values(__pyx_v_vm, __pyx_v_kwargs, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1085, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1083
+          /* "unqlite.pyx":1086
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  *             vm.execute()             # <<<<<<<<<<<<<<
  * 
  *     def _simple_execute(self, basestring script, **kwargs):
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1083, __pyx_L7_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1086, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1080
+          /* "unqlite.pyx":1083
  *     def _execute(self, basestring script, **kwargs):
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  */
         }
@@ -19089,36 +19210,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("unqlite.Collection._execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1080, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1083, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1080, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1083, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1080, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1083, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 1080, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 1083, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_2, __pyx_t_1);
             __pyx_t_4 = 0; __pyx_t_2 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 1080, __pyx_L9_except_error)
+            __PYX_ERR(0, 1083, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -19136,30 +19257,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1080, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1083, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "unqlite.pyx":1078
+  /* "unqlite.pyx":1081
  *         self.name = decode(name)
  * 
  *     def _execute(self, basestring script, **kwargs):             # <<<<<<<<<<<<<<
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  */
 
@@ -19176,15 +19297,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_vm);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1085
+/* "unqlite.pyx":1088
  *             vm.execute()
  * 
  *     def _simple_execute(self, basestring script, **kwargs):             # <<<<<<<<<<<<<<
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  */
 
@@ -19216,33 +19337,33 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_script)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_simple_execute") < 0)) __PYX_ERR(0, 1085, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_simple_execute") < 0)) __PYX_ERR(0, 1088, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_script = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_simple_execute", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1085, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_simple_execute", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1088, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("unqlite.Collection._simple_execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_script), (&PyBaseString_Type), 1, "script", 1))) __PYX_ERR(0, 1085, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_script), (&PyBaseString_Type), 1, "script", 1))) __PYX_ERR(0, 1088, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_10Collection_4_simple_execute(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v_script, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -19270,103 +19391,103 @@
   int __pyx_t_13;
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_simple_execute", 0);
 
-  /* "unqlite.pyx":1087
+  /* "unqlite.pyx":1090
  *     def _simple_execute(self, basestring script, **kwargs):
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  */
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1087, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)__pyx_v_self->unqlite));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self->unqlite));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self->unqlite));
     __Pyx_INCREF(__pyx_v_script);
     __Pyx_GIVEREF(__pyx_v_script);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_script);
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1087, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1087, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1087, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1087, __pyx_L3_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
-          if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1087, __pyx_L7_error)
+          if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1090, __pyx_L7_error)
           __pyx_v_vm = ((struct __pyx_obj_7unqlite_VM *)__pyx_t_4);
           __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1088
+          /* "unqlite.pyx":1091
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  *             vm['collection'] = self.name             # <<<<<<<<<<<<<<
  *             vm.set_values(kwargs)
  *             vm.execute()
  */
           __pyx_t_4 = __pyx_v_self->name;
           __Pyx_INCREF(__pyx_t_4);
-          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1088, __pyx_L7_error)
+          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1091, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1089
+          /* "unqlite.pyx":1092
  *         with VM(self.unqlite, script) as vm:
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)             # <<<<<<<<<<<<<<
  *             vm.execute()
  *             try:
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->set_values(__pyx_v_vm, __pyx_v_kwargs, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1089, __pyx_L7_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->set_values(__pyx_v_vm, __pyx_v_kwargs, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1092, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1090
+          /* "unqlite.pyx":1093
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  *             vm.execute()             # <<<<<<<<<<<<<<
  *             try:
  *                 return vm['ret']
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L7_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1093, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "unqlite.pyx":1091
+          /* "unqlite.pyx":1094
  *             vm.set_values(kwargs)
  *             vm.execute()
  *             try:             # <<<<<<<<<<<<<<
  *                 return vm['ret']
  *             except KeyError:
  */
           {
@@ -19374,74 +19495,74 @@
             __Pyx_PyThreadState_assign
             __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
             __Pyx_XGOTREF(__pyx_t_9);
             __Pyx_XGOTREF(__pyx_t_10);
             __Pyx_XGOTREF(__pyx_t_11);
             /*try:*/ {
 
-              /* "unqlite.pyx":1092
+              /* "unqlite.pyx":1095
  *             vm.execute()
  *             try:
  *                 return vm['ret']             # <<<<<<<<<<<<<<
  *             except KeyError:
  *                 raise ValueError('Error fetching return value from script.')
  */
               __Pyx_XDECREF(__pyx_r);
-              __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1092, __pyx_L13_error)
+              __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1095, __pyx_L13_error)
               __Pyx_GOTREF(__pyx_t_4);
               __pyx_r = __pyx_t_4;
               __pyx_t_4 = 0;
               goto __pyx_L17_try_return;
 
-              /* "unqlite.pyx":1091
+              /* "unqlite.pyx":1094
  *             vm.set_values(kwargs)
  *             vm.execute()
  *             try:             # <<<<<<<<<<<<<<
  *                 return vm['ret']
  *             except KeyError:
  */
             }
             __pyx_L13_error:;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "unqlite.pyx":1093
+            /* "unqlite.pyx":1096
  *             try:
  *                 return vm['ret']
  *             except KeyError:             # <<<<<<<<<<<<<<
  *                 raise ValueError('Error fetching return value from script.')
  * 
  */
             __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
             if (__pyx_t_12) {
               __Pyx_AddTraceback("unqlite.Collection._simple_execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
-              if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1093, __pyx_L15_except_error)
+              if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1096, __pyx_L15_except_error)
               __Pyx_GOTREF(__pyx_t_4);
               __Pyx_GOTREF(__pyx_t_2);
               __Pyx_GOTREF(__pyx_t_1);
 
-              /* "unqlite.pyx":1094
+              /* "unqlite.pyx":1097
  *                 return vm['ret']
  *             except KeyError:
  *                 raise ValueError('Error fetching return value from script.')             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
-              __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1094, __pyx_L15_except_error)
+              __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1097, __pyx_L15_except_error)
               __Pyx_GOTREF(__pyx_t_5);
               __Pyx_Raise(__pyx_t_5, 0, 0, 0);
               __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-              __PYX_ERR(0, 1094, __pyx_L15_except_error)
+              __PYX_ERR(0, 1097, __pyx_L15_except_error)
             }
             goto __pyx_L15_except_error;
             __pyx_L15_except_error:;
 
-            /* "unqlite.pyx":1091
+            /* "unqlite.pyx":1094
  *             vm.set_values(kwargs)
  *             vm.execute()
  *             try:             # <<<<<<<<<<<<<<
  *                 return vm['ret']
  *             except KeyError:
  */
             __Pyx_XGIVEREF(__pyx_t_9);
@@ -19453,51 +19574,51 @@
             __Pyx_XGIVEREF(__pyx_t_9);
             __Pyx_XGIVEREF(__pyx_t_10);
             __Pyx_XGIVEREF(__pyx_t_11);
             __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
             goto __pyx_L11_try_return;
           }
 
-          /* "unqlite.pyx":1087
+          /* "unqlite.pyx":1090
  *     def _simple_execute(self, basestring script, **kwargs):
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             vm['collection'] = self.name
  *             vm.set_values(kwargs)
  */
         }
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("unqlite.Collection._simple_execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 1087, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 1090, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1087, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1090, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1087, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1090, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_13 < 0) __PYX_ERR(0, 1087, __pyx_L9_except_error)
+          if (__pyx_t_13 < 0) __PYX_ERR(0, 1090, __pyx_L9_except_error)
           __pyx_t_14 = ((!(__pyx_t_13 != 0)) != 0);
           if (__pyx_t_14) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_4);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_2, __pyx_t_4);
             __pyx_t_1 = 0; __pyx_t_2 = 0; __pyx_t_4 = 0; 
-            __PYX_ERR(0, 1087, __pyx_L9_except_error)
+            __PYX_ERR(0, 1090, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -19520,27 +19641,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1087, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1090, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_8 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1087, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1090, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __pyx_r = __pyx_t_8;
         __pyx_t_8 = 0;
         goto __pyx_L0;
       }
@@ -19549,15 +19670,15 @@
     goto __pyx_L24;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L24:;
   }
 
-  /* "unqlite.pyx":1085
+  /* "unqlite.pyx":1088
  *             vm.execute()
  * 
  *     def _simple_execute(self, basestring script, **kwargs):             # <<<<<<<<<<<<<<
  *         cdef VM vm
  *         with VM(self.unqlite, script) as vm:
  */
 
@@ -19574,15 +19695,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_vm);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1096
+/* "unqlite.pyx":1099
  *                 raise ValueError('Error fetching return value from script.')
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         """Retrieve all records in the given collection."""
  *         return self._simple_execute('$ret = db_fetch_all($collection);')
  */
 
@@ -19607,44 +19728,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all", 0);
 
-  /* "unqlite.pyx":1098
+  /* "unqlite.pyx":1101
  *     def all(self):
  *         """Retrieve all records in the given collection."""
  *         return self._simple_execute('$ret = db_fetch_all($collection);')             # <<<<<<<<<<<<<<
  * 
  *     cpdef filter(self, filter_fn):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1098, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_fetch_all_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_fetch_all_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1098, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1096
+  /* "unqlite.pyx":1099
  *                 raise ValueError('Error fetching return value from script.')
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         """Retrieve all records in the given collection."""
  *         return self._simple_execute('$ret = db_fetch_all($collection);')
  */
 
@@ -19657,15 +19778,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1100
+/* "unqlite.pyx":1103
  *         return self._simple_execute('$ret = db_fetch_all($collection);')
  * 
  *     cpdef filter(self, filter_fn):             # <<<<<<<<<<<<<<
  *         """
  *         Filter the records in the collection using the provided Python
  */
 
@@ -19698,15 +19819,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_filter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1100, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_filter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1103, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7unqlite_10Collection_9filter)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -19715,15 +19836,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_filter_fn) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_filter_fn);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1100, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1103, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -19736,150 +19857,150 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "unqlite.pyx":1105
+  /* "unqlite.pyx":1108
  *         callback.
  *         """
  *         cdef unqlite_filter_fn filter_callback = py_filter_wrapper             # <<<<<<<<<<<<<<
  *         cdef VM vm
  *         cdef void *cb_pointer = <void *>filter_fn
  */
   __pyx_v_filter_callback = __pyx_f_7unqlite_py_filter_wrapper;
 
-  /* "unqlite.pyx":1107
+  /* "unqlite.pyx":1110
  *         cdef unqlite_filter_fn filter_callback = py_filter_wrapper
  *         cdef VM vm
  *         cdef void *cb_pointer = <void *>filter_fn             # <<<<<<<<<<<<<<
  * 
  *         script = '$ret = db_fetch_all($collection, _filter_fn)'
  */
   __pyx_v_cb_pointer = ((void *)__pyx_v_filter_fn);
 
-  /* "unqlite.pyx":1109
+  /* "unqlite.pyx":1112
  *         cdef void *cb_pointer = <void *>filter_fn
  * 
  *         script = '$ret = db_fetch_all($collection, _filter_fn)'             # <<<<<<<<<<<<<<
  *         with VM(self.unqlite, script) as vm:
  *             unqlite_create_function(
  */
   __Pyx_INCREF(__pyx_kp_u_ret_db_fetch_all_collection__fi);
   __pyx_v_script = __pyx_kp_u_ret_db_fetch_all_collection__fi;
 
-  /* "unqlite.pyx":1110
+  /* "unqlite.pyx":1113
  * 
  *         script = '$ret = db_fetch_all($collection, _filter_fn)'
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             unqlite_create_function(
  *                 vm.vm,
  */
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)__pyx_v_self->unqlite));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self->unqlite));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self->unqlite));
     __Pyx_INCREF(__pyx_v_script);
     __Pyx_GIVEREF(__pyx_v_script);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_script);
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1110, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1113, __pyx_L3_error)
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
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1110, __pyx_L3_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1113, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
-          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1110, __pyx_L7_error)
+          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7unqlite_VM))))) __PYX_ERR(0, 1113, __pyx_L7_error)
           __pyx_v_vm = ((struct __pyx_obj_7unqlite_VM *)__pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":1111
+          /* "unqlite.pyx":1114
  *         script = '$ret = db_fetch_all($collection, _filter_fn)'
  *         with VM(self.unqlite, script) as vm:
  *             unqlite_create_function(             # <<<<<<<<<<<<<<
  *                 vm.vm,
  *                 '_filter_fn',
  */
           (void)(unqlite_create_function(__pyx_v_vm->vm, ((char const *)"_filter_fn"), __pyx_v_filter_callback, __pyx_v_cb_pointer));
 
-          /* "unqlite.pyx":1116
+          /* "unqlite.pyx":1119
  *                 filter_callback,
  *                 cb_pointer)
  *             vm['collection'] = self.name             # <<<<<<<<<<<<<<
  *             vm.execute()
  *             ret = vm['ret']
  */
           __pyx_t_3 = __pyx_v_self->name;
           __Pyx_INCREF(__pyx_t_3);
-          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_3) < 0)) __PYX_ERR(0, 1116, __pyx_L7_error)
+          if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_collection, __pyx_t_3) < 0)) __PYX_ERR(0, 1119, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":1117
+          /* "unqlite.pyx":1120
  *                 cb_pointer)
  *             vm['collection'] = self.name
  *             vm.execute()             # <<<<<<<<<<<<<<
  *             ret = vm['ret']
  *             unqlite_delete_function(
  */
-          __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1117, __pyx_L7_error)
+          __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->execute(__pyx_v_vm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1120, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":1118
+          /* "unqlite.pyx":1121
  *             vm['collection'] = self.name
  *             vm.execute()
  *             ret = vm['ret']             # <<<<<<<<<<<<<<
  *             unqlite_delete_function(
  *                 vm.vm,
  */
-          __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1118, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_vm), __pyx_n_u_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1121, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_v_ret = __pyx_t_3;
           __pyx_t_3 = 0;
 
-          /* "unqlite.pyx":1119
+          /* "unqlite.pyx":1122
  *             vm.execute()
  *             ret = vm['ret']
  *             unqlite_delete_function(             # <<<<<<<<<<<<<<
  *                 vm.vm,
  *                 '_filter_fn')
  */
           (void)(unqlite_delete_function(__pyx_v_vm->vm, ((char const *)"_filter_fn")));
 
-          /* "unqlite.pyx":1110
+          /* "unqlite.pyx":1113
  * 
  *         script = '$ret = db_fetch_all($collection, _filter_fn)'
  *         with VM(self.unqlite, script) as vm:             # <<<<<<<<<<<<<<
  *             unqlite_create_function(
  *                 vm.vm,
  */
         }
@@ -19890,36 +20011,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("unqlite.Collection.filter", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1110, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 1113, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_4 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1110, __pyx_L9_except_error)
+          __pyx_t_4 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1113, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, NULL);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1110, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1113, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 1110, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 1113, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_2, __pyx_t_1);
             __pyx_t_3 = 0; __pyx_t_2 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 1110, __pyx_L9_except_error)
+            __PYX_ERR(0, 1113, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -19937,43 +20058,43 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_5) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__5, NULL);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1110, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1113, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "unqlite.pyx":1123
+  /* "unqlite.pyx":1126
  *                 '_filter_fn')
  * 
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     def create(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_ret)) { __Pyx_RaiseUnboundLocalError("ret"); __PYX_ERR(0, 1123, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_ret)) { __Pyx_RaiseUnboundLocalError("ret"); __PYX_ERR(0, 1126, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1100
+  /* "unqlite.pyx":1103
  *         return self._simple_execute('$ret = db_fetch_all($collection);')
  * 
  *     cpdef filter(self, filter_fn):             # <<<<<<<<<<<<<<
  *         """
  *         Filter the records in the collection using the provided Python
  */
 
@@ -20013,15 +20134,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("filter", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7unqlite_10Collection_filter(__pyx_v_self, __pyx_v_filter_fn, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1100, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_10Collection_filter(__pyx_v_self, __pyx_v_filter_fn, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -20030,15 +20151,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1125
+/* "unqlite.pyx":1128
  *         return ret
  * 
  *     def create(self):             # <<<<<<<<<<<<<<
  *         """
  *         Create the named collection.
  */
 
@@ -20063,44 +20184,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create", 0);
 
-  /* "unqlite.pyx":1132
+  /* "unqlite.pyx":1135
  *         used to create the collection itself.
  *         """
  *         return self._simple_execute('if (!db_exists($collection)) { '             # <<<<<<<<<<<<<<
  *                                     '$ret = db_create($collection); } '
  *                                     'else { $ret = false; }')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1132, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_if_db_exists_collection_ret_db_c) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_if_db_exists_collection_ret_db_c);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1132, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1125
+  /* "unqlite.pyx":1128
  *         return ret
  * 
  *     def create(self):             # <<<<<<<<<<<<<<
  *         """
  *         Create the named collection.
  */
 
@@ -20113,15 +20234,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1136
+/* "unqlite.pyx":1139
  *                                     'else { $ret = false; }')
  * 
  *     def drop(self):             # <<<<<<<<<<<<<<
  *         """Drop the collection and all associated records."""
  *         return self._simple_execute('if (db_exists($collection)) { '
  */
 
@@ -20146,44 +20267,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("drop", 0);
 
-  /* "unqlite.pyx":1138
+  /* "unqlite.pyx":1141
  *     def drop(self):
  *         """Drop the collection and all associated records."""
  *         return self._simple_execute('if (db_exists($collection)) { '             # <<<<<<<<<<<<<<
  *                                     '$ret = db_drop_collection($collection); }'
  *                                     'else { $ret = false; }')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1138, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_if_db_exists_collection_ret_db_d) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_if_db_exists_collection_ret_db_d);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1138, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1136
+  /* "unqlite.pyx":1139
  *                                     'else { $ret = false; }')
  * 
  *     def drop(self):             # <<<<<<<<<<<<<<
  *         """Drop the collection and all associated records."""
  *         return self._simple_execute('if (db_exists($collection)) { '
  */
 
@@ -20196,15 +20317,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1142
+/* "unqlite.pyx":1145
  *                                     'else { $ret = false; }')
  * 
  *     def exists(self):             # <<<<<<<<<<<<<<
  *         """Return boolean indicating whether the collection exists."""
  *         return self._simple_execute('$ret = db_exists($collection);')
  */
 
@@ -20229,44 +20350,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exists", 0);
 
-  /* "unqlite.pyx":1144
+  /* "unqlite.pyx":1147
  *     def exists(self):
  *         """Return boolean indicating whether the collection exists."""
  *         return self._simple_execute('$ret = db_exists($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def last_record_id(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1144, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_exists_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_exists_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1144, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1142
+  /* "unqlite.pyx":1145
  *                                     'else { $ret = false; }')
  * 
  *     def exists(self):             # <<<<<<<<<<<<<<
  *         """Return boolean indicating whether the collection exists."""
  *         return self._simple_execute('$ret = db_exists($collection);')
  */
 
@@ -20279,15 +20400,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1146
+/* "unqlite.pyx":1149
  *         return self._simple_execute('$ret = db_exists($collection);')
  * 
  *     def last_record_id(self):             # <<<<<<<<<<<<<<
  *         """Return the ID of the last document to be stored."""
  *         return self._simple_execute('$ret = db_last_record_id($collection);')
  */
 
@@ -20312,44 +20433,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("last_record_id", 0);
 
-  /* "unqlite.pyx":1148
+  /* "unqlite.pyx":1151
  *     def last_record_id(self):
  *         """Return the ID of the last document to be stored."""
  *         return self._simple_execute('$ret = db_last_record_id($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def current_record_id(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_last_record_id_collectio) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_last_record_id_collectio);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1148, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1146
+  /* "unqlite.pyx":1149
  *         return self._simple_execute('$ret = db_exists($collection);')
  * 
  *     def last_record_id(self):             # <<<<<<<<<<<<<<
  *         """Return the ID of the last document to be stored."""
  *         return self._simple_execute('$ret = db_last_record_id($collection);')
  */
 
@@ -20362,15 +20483,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1150
+/* "unqlite.pyx":1153
  *         return self._simple_execute('$ret = db_last_record_id($collection);')
  * 
  *     def current_record_id(self):             # <<<<<<<<<<<<<<
  *         """Return the ID of the current JSON document."""
  *         return self._simple_execute(
  */
 
@@ -20395,44 +20516,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("current_record_id", 0);
 
-  /* "unqlite.pyx":1152
+  /* "unqlite.pyx":1155
  *     def current_record_id(self):
  *         """Return the ID of the current JSON document."""
  *         return self._simple_execute(             # <<<<<<<<<<<<<<
  *             '$ret = db_current_record_id($collection);')
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_current_record_id_collec) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_current_record_id_collec);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1152, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1150
+  /* "unqlite.pyx":1153
  *         return self._simple_execute('$ret = db_last_record_id($collection);')
  * 
  *     def current_record_id(self):             # <<<<<<<<<<<<<<
  *         """Return the ID of the current JSON document."""
  *         return self._simple_execute(
  */
 
@@ -20445,15 +20566,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1155
+/* "unqlite.pyx":1158
  *             '$ret = db_current_record_id($collection);')
  * 
  *     def reset_cursor(self):             # <<<<<<<<<<<<<<
  *         self._execute('db_reset_record_cursor($collection);')
  * 
  */
 
@@ -20477,41 +20598,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reset_cursor", 0);
 
-  /* "unqlite.pyx":1156
+  /* "unqlite.pyx":1159
  * 
  *     def reset_cursor(self):
  *         self._execute('db_reset_record_cursor($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def creation_date(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_execute_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_execute_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_db_reset_record_cursor_collectio) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_db_reset_record_cursor_collectio);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1156, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1155
+  /* "unqlite.pyx":1158
  *             '$ret = db_current_record_id($collection);')
  * 
  *     def reset_cursor(self):             # <<<<<<<<<<<<<<
  *         self._execute('db_reset_record_cursor($collection);')
  * 
  */
 
@@ -20526,15 +20647,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1158
+/* "unqlite.pyx":1161
  *         self._execute('db_reset_record_cursor($collection);')
  * 
  *     def creation_date(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_creation_date($collection);')
  * 
  */
 
@@ -20558,44 +20679,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("creation_date", 0);
 
-  /* "unqlite.pyx":1159
+  /* "unqlite.pyx":1162
  * 
  *     def creation_date(self):
  *         return self._simple_execute('$ret = db_creation_date($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def set_schema(self, _schema=None, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_creation_date_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_creation_date_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1159, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1158
+  /* "unqlite.pyx":1161
  *         self._execute('db_reset_record_cursor($collection);')
  * 
  *     def creation_date(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_creation_date($collection);')
  * 
  */
 
@@ -20608,15 +20729,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1161
+/* "unqlite.pyx":1164
  *         return self._simple_execute('$ret = db_creation_date($collection);')
  * 
  *     def set_schema(self, _schema=None, **kwargs):             # <<<<<<<<<<<<<<
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)
  */
 
@@ -20651,29 +20772,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "set_schema") < 0)) __PYX_ERR(0, 1161, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "set_schema") < 0)) __PYX_ERR(0, 1164, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v__schema = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_schema", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_schema", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1164, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("unqlite.Collection.set_schema", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_10Collection_24set_schema(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v__schema, __pyx_v_kwargs);
@@ -20693,104 +20814,104 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_schema", 0);
 
-  /* "unqlite.pyx":1162
+  /* "unqlite.pyx":1165
  * 
  *     def set_schema(self, _schema=None, **kwargs):
  *         schema = _schema or {}             # <<<<<<<<<<<<<<
  *         if kwargs: schema.update(kwargs)
  *         return self._simple_execute(
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v__schema); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1162, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v__schema); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1165, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __Pyx_INCREF(__pyx_v__schema);
     __pyx_t_1 = __pyx_v__schema;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1162, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_v_schema = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1163
+  /* "unqlite.pyx":1166
  *     def set_schema(self, _schema=None, **kwargs):
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)             # <<<<<<<<<<<<<<
  *         return self._simple_execute(
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1166, __pyx_L1_error)
   if (__pyx_t_2) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1163, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1166, __pyx_L1_error)
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
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_kwargs) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_kwargs);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1163, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "unqlite.pyx":1164
+  /* "unqlite.pyx":1167
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)
  *         return self._simple_execute(             # <<<<<<<<<<<<<<
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1164, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "unqlite.pyx":1165
+  /* "unqlite.pyx":1168
  *         if kwargs: schema.update(kwargs)
  *         return self._simple_execute(
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)             # <<<<<<<<<<<<<<
  * 
  *     def get_schema(self):
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1165, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_schema_2, __pyx_v_schema) < 0) __PYX_ERR(0, 1165, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_schema_2, __pyx_v_schema) < 0) __PYX_ERR(0, 1168, __pyx_L1_error)
 
-  /* "unqlite.pyx":1164
+  /* "unqlite.pyx":1167
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)
  *         return self._simple_execute(             # <<<<<<<<<<<<<<
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__18, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1164, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__18, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1161
+  /* "unqlite.pyx":1164
  *         return self._simple_execute('$ret = db_creation_date($collection);')
  * 
  *     def set_schema(self, _schema=None, **kwargs):             # <<<<<<<<<<<<<<
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)
  */
 
@@ -20804,15 +20925,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_schema);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1167
+/* "unqlite.pyx":1170
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  * 
  *     def get_schema(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_get_schema($collection);')
  * 
  */
 
@@ -20836,44 +20957,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_schema", 0);
 
-  /* "unqlite.pyx":1168
+  /* "unqlite.pyx":1171
  * 
  *     def get_schema(self):
  *         return self._simple_execute('$ret = db_get_schema($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_get_schema_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_get_schema_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1167
+  /* "unqlite.pyx":1170
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  * 
  *     def get_schema(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_get_schema($collection);')
  * 
  */
 
@@ -20886,15 +21007,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1170
+/* "unqlite.pyx":1173
  *         return self._simple_execute('$ret = db_get_schema($collection);')
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """Return the number of records in the document collection."""
  *         return self._simple_execute('$ret = db_total_records($collection);')
  */
 
@@ -20923,44 +21044,44 @@
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "unqlite.pyx":1172
+  /* "unqlite.pyx":1175
  *     def __len__(self):
  *         """Return the number of records in the document collection."""
  *         return self._simple_execute('$ret = db_total_records($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def delete(self, record_id):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1172, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_total_records_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_total_records_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1172, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1172, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1170
+  /* "unqlite.pyx":1173
  *         return self._simple_execute('$ret = db_get_schema($collection);')
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """Return the number of records in the document collection."""
  *         return self._simple_execute('$ret = db_total_records($collection);')
  */
 
@@ -20972,15 +21093,15 @@
   __Pyx_AddTraceback("unqlite.Collection.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1174
+/* "unqlite.pyx":1177
  *         return self._simple_execute('$ret = db_total_records($collection);')
  * 
  *     def delete(self, record_id):             # <<<<<<<<<<<<<<
  *         """Delete the document associated with the given ID."""
  *         script = '$ret = db_drop_record($collection, $record_id);'
  */
 
@@ -21007,52 +21128,52 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
 
-  /* "unqlite.pyx":1176
+  /* "unqlite.pyx":1179
  *     def delete(self, record_id):
  *         """Delete the document associated with the given ID."""
  *         script = '$ret = db_drop_record($collection, $record_id);'             # <<<<<<<<<<<<<<
  *         return self._simple_execute(script, record_id=record_id)
  * 
  */
   __Pyx_INCREF(__pyx_kp_u_ret_db_drop_record_collection_r);
   __pyx_v_script = __pyx_kp_u_ret_db_drop_record_collection_r;
 
-  /* "unqlite.pyx":1177
+  /* "unqlite.pyx":1180
  *         """Delete the document associated with the given ID."""
  *         script = '$ret = db_drop_record($collection, $record_id);'
  *         return self._simple_execute(script, record_id=record_id)             # <<<<<<<<<<<<<<
  * 
  *     def fetch(self, record_id):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1177, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_script);
   __Pyx_GIVEREF(__pyx_v_script);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_script);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1177, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1177, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1180, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1174
+  /* "unqlite.pyx":1177
  *         return self._simple_execute('$ret = db_total_records($collection);')
  * 
  *     def delete(self, record_id):             # <<<<<<<<<<<<<<
  *         """Delete the document associated with the given ID."""
  *         script = '$ret = db_drop_record($collection, $record_id);'
  */
 
@@ -21067,15 +21188,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_script);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1179
+/* "unqlite.pyx":1182
  *         return self._simple_execute(script, record_id=record_id)
  * 
  *     def fetch(self, record_id):             # <<<<<<<<<<<<<<
  *         """Fetch the document associated with the given ID."""
  *         script = '$ret = db_fetch_by_id($collection, $record_id);'
  */
 
@@ -21102,52 +21223,52 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fetch", 0);
 
-  /* "unqlite.pyx":1181
+  /* "unqlite.pyx":1184
  *     def fetch(self, record_id):
  *         """Fetch the document associated with the given ID."""
  *         script = '$ret = db_fetch_by_id($collection, $record_id);'             # <<<<<<<<<<<<<<
  *         return self._simple_execute(script, record_id=record_id)
  * 
  */
   __Pyx_INCREF(__pyx_kp_u_ret_db_fetch_by_id_collection_r);
   __pyx_v_script = __pyx_kp_u_ret_db_fetch_by_id_collection_r;
 
-  /* "unqlite.pyx":1182
+  /* "unqlite.pyx":1185
  *         """Fetch the document associated with the given ID."""
  *         script = '$ret = db_fetch_by_id($collection, $record_id);'
  *         return self._simple_execute(script, record_id=record_id)             # <<<<<<<<<<<<<<
  * 
  *     def store(self, record, return_id=True):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1182, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1182, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_script);
   __Pyx_GIVEREF(__pyx_v_script);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_script);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1182, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1182, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1182, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1185, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1179
+  /* "unqlite.pyx":1182
  *         return self._simple_execute(script, record_id=record_id)
  * 
  *     def fetch(self, record_id):             # <<<<<<<<<<<<<<
  *         """Fetch the document associated with the given ID."""
  *         script = '$ret = db_fetch_by_id($collection, $record_id);'
  */
 
@@ -21162,15 +21283,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_script);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1184
+/* "unqlite.pyx":1187
  *         return self._simple_execute(script, record_id=record_id)
  * 
  *     def store(self, record, return_id=True):             # <<<<<<<<<<<<<<
  *         """
  *         Create a new JSON document in the collection, optionally returning
  */
 
@@ -21210,15 +21331,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_id);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "store") < 0)) __PYX_ERR(0, 1184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "store") < 0)) __PYX_ERR(0, 1187, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -21226,15 +21347,15 @@
       }
     }
     __pyx_v_record = values[0];
     __pyx_v_return_id = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("store", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("store", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Collection.store", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_10Collection_34store(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v_record, __pyx_v_return_id);
 
@@ -21253,85 +21374,85 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("store", 0);
 
-  /* "unqlite.pyx":1189
+  /* "unqlite.pyx":1192
  *         the new record's ID.
  *         """
  *         if return_id:             # <<<<<<<<<<<<<<
  *             script = ('if (db_store($collection, $record)) { '
  *                       '$ret = db_last_record_id($collection); }')
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_return_id); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_return_id); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1192, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1190
+    /* "unqlite.pyx":1193
  *         """
  *         if return_id:
  *             script = ('if (db_store($collection, $record)) { '             # <<<<<<<<<<<<<<
  *                       '$ret = db_last_record_id($collection); }')
  *         else:
  */
     __Pyx_INCREF(__pyx_kp_u_if_db_store_collection_record_re);
     __pyx_v_script = __pyx_kp_u_if_db_store_collection_record_re;
 
-    /* "unqlite.pyx":1189
+    /* "unqlite.pyx":1192
  *         the new record's ID.
  *         """
  *         if return_id:             # <<<<<<<<<<<<<<
  *             script = ('if (db_store($collection, $record)) { '
  *                       '$ret = db_last_record_id($collection); }')
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1193
+  /* "unqlite.pyx":1196
  *                       '$ret = db_last_record_id($collection); }')
  *         else:
  *             script = '$ret = db_store($collection, $record);'             # <<<<<<<<<<<<<<
  *         return self._simple_execute(script, record=record)
  * 
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_kp_u_ret_db_store_collection_record);
     __pyx_v_script = __pyx_kp_u_ret_db_store_collection_record;
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":1194
+  /* "unqlite.pyx":1197
  *         else:
  *             script = '$ret = db_store($collection, $record);'
  *         return self._simple_execute(script, record=record)             # <<<<<<<<<<<<<<
  * 
  *     def update(self, record_id, record):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1194, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1194, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_script);
   __Pyx_GIVEREF(__pyx_v_script);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_script);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1194, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_record, __pyx_v_record) < 0) __PYX_ERR(0, 1194, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1194, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_record, __pyx_v_record) < 0) __PYX_ERR(0, 1197, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1184
+  /* "unqlite.pyx":1187
  *         return self._simple_execute(script, record_id=record_id)
  * 
  *     def store(self, record, return_id=True):             # <<<<<<<<<<<<<<
  *         """
  *         Create a new JSON document in the collection, optionally returning
  */
 
@@ -21346,15 +21467,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_script);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1196
+/* "unqlite.pyx":1199
  *         return self._simple_execute(script, record=record)
  * 
  *     def update(self, record_id, record):             # <<<<<<<<<<<<<<
  *         """
  *         Update the record identified by the given ID.
  */
 
@@ -21389,32 +21510,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_record_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_record)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("update", 1, 2, 2, 1); __PYX_ERR(0, 1196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("update", 1, 2, 2, 1); __PYX_ERR(0, 1199, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update") < 0)) __PYX_ERR(0, 1196, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update") < 0)) __PYX_ERR(0, 1199, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_record_id = values[0];
     __pyx_v_record = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("update", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1196, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("update", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1199, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.Collection.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7unqlite_10Collection_36update(((struct __pyx_obj_7unqlite_Collection *)__pyx_v_self), __pyx_v_record_id, __pyx_v_record);
 
@@ -21432,53 +21553,53 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 0);
 
-  /* "unqlite.pyx":1200
+  /* "unqlite.pyx":1203
  *         Update the record identified by the given ID.
  *         """
  *         script = '$ret = db_update_record($collection, $record_id, $record);'             # <<<<<<<<<<<<<<
  *         return self._simple_execute(script, record_id=record_id, record=record)
  * 
  */
   __Pyx_INCREF(__pyx_kp_u_ret_db_update_record_collection);
   __pyx_v_script = __pyx_kp_u_ret_db_update_record_collection;
 
-  /* "unqlite.pyx":1201
+  /* "unqlite.pyx":1204
  *         """
  *         script = '$ret = db_update_record($collection, $record_id, $record);'
  *         return self._simple_execute(script, record_id=record_id, record=record)             # <<<<<<<<<<<<<<
  * 
  *     def fetch_current(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_script);
   __Pyx_GIVEREF(__pyx_v_script);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_script);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1201, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record, __pyx_v_record) < 0) __PYX_ERR(0, 1201, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record_id, __pyx_v_record_id) < 0) __PYX_ERR(0, 1204, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_record, __pyx_v_record) < 0) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1196
+  /* "unqlite.pyx":1199
  *         return self._simple_execute(script, record=record)
  * 
  *     def update(self, record_id, record):             # <<<<<<<<<<<<<<
  *         """
  *         Update the record identified by the given ID.
  */
 
@@ -21493,15 +21614,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_script);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1203
+/* "unqlite.pyx":1206
  *         return self._simple_execute(script, record_id=record_id, record=record)
  * 
  *     def fetch_current(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_fetch($collection);')
  * 
  */
 
@@ -21525,44 +21646,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fetch_current", 0);
 
-  /* "unqlite.pyx":1204
+  /* "unqlite.pyx":1207
  * 
  *     def fetch_current(self):
  *         return self._simple_execute('$ret = db_fetch($collection);')             # <<<<<<<<<<<<<<
  * 
  *     def __delitem__(self, record_id):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_fetch_collection) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_fetch_collection);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1203
+  /* "unqlite.pyx":1206
  *         return self._simple_execute(script, record_id=record_id, record=record)
  * 
  *     def fetch_current(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_fetch($collection);')
  * 
  */
 
@@ -21575,15 +21696,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1206
+/* "unqlite.pyx":1209
  *         return self._simple_execute('$ret = db_fetch($collection);')
  * 
  *     def __delitem__(self, record_id):             # <<<<<<<<<<<<<<
  *         self.delete(record_id)
  * 
  */
 
@@ -21607,41 +21728,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__delitem__", 0);
 
-  /* "unqlite.pyx":1207
+  /* "unqlite.pyx":1210
  * 
  *     def __delitem__(self, record_id):
  *         self.delete(record_id)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, record_id):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_delete); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1207, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_delete); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_record_id) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_record_id);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1207, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1206
+  /* "unqlite.pyx":1209
  *         return self._simple_execute('$ret = db_fetch($collection);')
  * 
  *     def __delitem__(self, record_id):             # <<<<<<<<<<<<<<
  *         self.delete(record_id)
  * 
  */
 
@@ -21655,15 +21776,15 @@
   __Pyx_AddTraceback("unqlite.Collection.__delitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1209
+/* "unqlite.pyx":1212
  *         self.delete(record_id)
  * 
  *     def __getitem__(self, record_id):             # <<<<<<<<<<<<<<
  *         return self.fetch(record_id)
  * 
  */
 
@@ -21687,44 +21808,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "unqlite.pyx":1210
+  /* "unqlite.pyx":1213
  * 
  *     def __getitem__(self, record_id):
  *         return self.fetch(record_id)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, record_id, record):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_record_id) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_record_id);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1209
+  /* "unqlite.pyx":1212
  *         self.delete(record_id)
  * 
  *     def __getitem__(self, record_id):             # <<<<<<<<<<<<<<
  *         return self.fetch(record_id)
  * 
  */
 
@@ -21737,15 +21858,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1212
+/* "unqlite.pyx":1215
  *         return self.fetch(record_id)
  * 
  *     def __setitem__(self, record_id, record):             # <<<<<<<<<<<<<<
  *         self.update(record_id, record)
  * 
  */
 
@@ -21771,22 +21892,22 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
-  /* "unqlite.pyx":1213
+  /* "unqlite.pyx":1216
  * 
  *     def __setitem__(self, record_id, record):
  *         self.update(record_id, record)             # <<<<<<<<<<<<<<
  * 
  *     def error_log(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -21795,47 +21916,47 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_record_id, __pyx_v_record};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_record_id, __pyx_v_record};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1213, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_record_id);
     __Pyx_GIVEREF(__pyx_v_record_id);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_record_id);
     __Pyx_INCREF(__pyx_v_record);
     __Pyx_GIVEREF(__pyx_v_record);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_record);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1212
+  /* "unqlite.pyx":1215
  *         return self.fetch(record_id)
  * 
  *     def __setitem__(self, record_id, record):             # <<<<<<<<<<<<<<
  *         self.update(record_id, record)
  * 
  */
 
@@ -21850,15 +21971,15 @@
   __Pyx_AddTraceback("unqlite.Collection.__setitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1215
+/* "unqlite.pyx":1218
  *         self.update(record_id, record)
  * 
  *     def error_log(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_errlog();')
  * 
  */
 
@@ -21882,44 +22003,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error_log", 0);
 
-  /* "unqlite.pyx":1216
+  /* "unqlite.pyx":1219
  * 
  *     def error_log(self):
  *         return self._simple_execute('$ret = db_errlog();')             # <<<<<<<<<<<<<<
  * 
  *     def iterator(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1216, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simple_execute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_ret_db_errlog) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_ret_db_errlog);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1215
+  /* "unqlite.pyx":1218
  *         self.update(record_id, record)
  * 
  *     def error_log(self):             # <<<<<<<<<<<<<<
  *         return self._simple_execute('$ret = db_errlog();')
  * 
  */
 
@@ -21932,15 +22053,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1218
+/* "unqlite.pyx":1221
  *         return self._simple_execute('$ret = db_errlog();')
  * 
  *     def iterator(self):             # <<<<<<<<<<<<<<
  *         return CollectionIterator(self)
  * 
  */
 
@@ -21962,29 +22083,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("iterator", 0);
 
-  /* "unqlite.pyx":1219
+  /* "unqlite.pyx":1222
  * 
  *     def iterator(self):
  *         return CollectionIterator(self)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7unqlite_CollectionIterator), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1219, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7unqlite_CollectionIterator), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1218
+  /* "unqlite.pyx":1221
  *         return self._simple_execute('$ret = db_errlog();')
  * 
  *     def iterator(self):             # <<<<<<<<<<<<<<
  *         return CollectionIterator(self)
  * 
  */
 
@@ -21995,15 +22116,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1221
+/* "unqlite.pyx":1224
  *         return CollectionIterator(self)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(CollectionIterator(self))
  * 
  */
 
@@ -22026,32 +22147,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "unqlite.pyx":1222
+  /* "unqlite.pyx":1225
  * 
  *     def __iter__(self):
  *         return iter(CollectionIterator(self))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7unqlite_CollectionIterator), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1222, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7unqlite_CollectionIterator), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1222, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1221
+  /* "unqlite.pyx":1224
  *         return CollectionIterator(self)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(CollectionIterator(self))
  * 
  */
 
@@ -22370,15 +22491,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1232
+/* "unqlite.pyx":1235
  *         public Collection collection
  * 
  *     def __init__(self, Collection collection):             # <<<<<<<<<<<<<<
  *         self.collection = collection
  *         self.unqlite = self.collection.unqlite
  */
 
@@ -22407,32 +22528,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_collection)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1232, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1235, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_collection = ((struct __pyx_obj_7unqlite_Collection *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1232, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1235, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unqlite.CollectionIterator.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), __pyx_ptype_7unqlite_Collection, 1, "collection", 0))) __PYX_ERR(0, 1232, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), __pyx_ptype_7unqlite_Collection, 1, "collection", 0))) __PYX_ERR(0, 1235, __pyx_L1_error)
   __pyx_r = __pyx_pf_7unqlite_18CollectionIterator___init__(((struct __pyx_obj_7unqlite_CollectionIterator *)__pyx_v_self), __pyx_v_collection);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -22442,79 +22563,79 @@
 
 static int __pyx_pf_7unqlite_18CollectionIterator___init__(struct __pyx_obj_7unqlite_CollectionIterator *__pyx_v_self, struct __pyx_obj_7unqlite_Collection *__pyx_v_collection) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "unqlite.pyx":1233
+  /* "unqlite.pyx":1236
  * 
  *     def __init__(self, Collection collection):
  *         self.collection = collection             # <<<<<<<<<<<<<<
  *         self.unqlite = self.collection.unqlite
  *         self.vm = None
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_collection));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_collection));
   __Pyx_GOTREF(__pyx_v_self->collection);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->collection));
   __pyx_v_self->collection = __pyx_v_collection;
 
-  /* "unqlite.pyx":1234
+  /* "unqlite.pyx":1237
  *     def __init__(self, Collection collection):
  *         self.collection = collection
  *         self.unqlite = self.collection.unqlite             # <<<<<<<<<<<<<<
  *         self.vm = None
  *         self.done = True
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->collection->unqlite);
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->unqlite);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->unqlite));
   __pyx_v_self->unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1235
+  /* "unqlite.pyx":1238
  *         self.collection = collection
  *         self.unqlite = self.collection.unqlite
  *         self.vm = None             # <<<<<<<<<<<<<<
  *         self.done = True
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->vm);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->vm));
   __pyx_v_self->vm = ((struct __pyx_obj_7unqlite_VM *)Py_None);
 
-  /* "unqlite.pyx":1236
+  /* "unqlite.pyx":1239
  *         self.unqlite = self.collection.unqlite
  *         self.vm = None
  *         self.done = True             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_v_self->done = 1;
 
-  /* "unqlite.pyx":1232
+  /* "unqlite.pyx":1235
  *         public Collection collection
  * 
  *     def __init__(self, Collection collection):             # <<<<<<<<<<<<<<
  *         self.collection = collection
  *         self.unqlite = self.collection.unqlite
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1238
+/* "unqlite.pyx":1241
  *         self.done = True
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if self.vm is not None:
  *             self.vm.close()
  */
 
@@ -22540,124 +22661,124 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "unqlite.pyx":1239
+  /* "unqlite.pyx":1242
  * 
  *     def __iter__(self):
  *         if self.vm is not None:             # <<<<<<<<<<<<<<
  *             self.vm.close()
  * 
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_self->vm) != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1240
+    /* "unqlite.pyx":1243
  *     def __iter__(self):
  *         if self.vm is not None:
  *             self.vm.close()             # <<<<<<<<<<<<<<
  * 
  *         script = '$row = db_fetch($collection)'
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->close(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1240, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->close(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1243, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1239
+    /* "unqlite.pyx":1242
  * 
  *     def __iter__(self):
  *         if self.vm is not None:             # <<<<<<<<<<<<<<
  *             self.vm.close()
  * 
  */
   }
 
-  /* "unqlite.pyx":1242
+  /* "unqlite.pyx":1245
  *             self.vm.close()
  * 
  *         script = '$row = db_fetch($collection)'             # <<<<<<<<<<<<<<
  *         self.vm = VM(self.unqlite, script)
  *         self.vm.compile()
  */
   __Pyx_INCREF(__pyx_kp_u_row_db_fetch_collection);
   __pyx_v_script = __pyx_kp_u_row_db_fetch_collection;
 
-  /* "unqlite.pyx":1243
+  /* "unqlite.pyx":1246
  * 
  *         script = '$row = db_fetch($collection)'
  *         self.vm = VM(self.unqlite, script)             # <<<<<<<<<<<<<<
  *         self.vm.compile()
  *         self.vm['collection'] = self.collection.name
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1243, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->unqlite));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self->unqlite));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self->unqlite));
   __Pyx_INCREF(__pyx_v_script);
   __Pyx_GIVEREF(__pyx_v_script);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_script);
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7unqlite_VM), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->vm);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->vm));
   __pyx_v_self->vm = ((struct __pyx_obj_7unqlite_VM *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "unqlite.pyx":1244
+  /* "unqlite.pyx":1247
  *         script = '$row = db_fetch($collection)'
  *         self.vm = VM(self.unqlite, script)
  *         self.vm.compile()             # <<<<<<<<<<<<<<
  *         self.vm['collection'] = self.collection.name
  *         self.done = False
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->compile(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1244, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->compile(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "unqlite.pyx":1245
+  /* "unqlite.pyx":1248
  *         self.vm = VM(self.unqlite, script)
  *         self.vm.compile()
  *         self.vm['collection'] = self.collection.name             # <<<<<<<<<<<<<<
  *         self.done = False
  *         return self
  */
   __pyx_t_4 = __pyx_v_self->collection->name;
   __Pyx_INCREF(__pyx_t_4);
-  if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self->vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1245, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self->vm), __pyx_n_u_collection, __pyx_t_4) < 0)) __PYX_ERR(0, 1248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "unqlite.pyx":1246
+  /* "unqlite.pyx":1249
  *         self.vm.compile()
  *         self.vm['collection'] = self.collection.name
  *         self.done = False             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->done = 0;
 
-  /* "unqlite.pyx":1247
+  /* "unqlite.pyx":1250
  *         self.vm['collection'] = self.collection.name
  *         self.done = False
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1238
+  /* "unqlite.pyx":1241
  *         self.done = True
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if self.vm is not None:
  *             self.vm.close()
  */
 
@@ -22670,15 +22791,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_script);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1249
+/* "unqlite.pyx":1252
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.done:
  *             raise StopIteration
  */
 
@@ -22703,153 +22824,153 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "unqlite.pyx":1250
+  /* "unqlite.pyx":1253
  * 
  *     def __next__(self):
  *         if self.done:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   __pyx_t_1 = (__pyx_v_self->done != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unqlite.pyx":1251
+    /* "unqlite.pyx":1254
  *     def __next__(self):
  *         if self.done:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *         self.vm.execute()
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 1251, __pyx_L1_error)
+    __PYX_ERR(0, 1254, __pyx_L1_error)
 
-    /* "unqlite.pyx":1250
+    /* "unqlite.pyx":1253
  * 
  *     def __next__(self):
  *         if self.done:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
   }
 
-  /* "unqlite.pyx":1253
+  /* "unqlite.pyx":1256
  *             raise StopIteration
  * 
  *         self.vm.execute()             # <<<<<<<<<<<<<<
  *         row = self.vm['row']
  *         if row is None:
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->execute(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1253, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->execute(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unqlite.pyx":1254
+  /* "unqlite.pyx":1257
  * 
  *         self.vm.execute()
  *         row = self.vm['row']             # <<<<<<<<<<<<<<
  *         if row is None:
  *             self.done = True
  */
-  __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->vm), __pyx_n_u_row); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1254, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->vm), __pyx_n_u_row); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_row = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "unqlite.pyx":1255
+  /* "unqlite.pyx":1258
  *         self.vm.execute()
  *         row = self.vm['row']
  *         if row is None:             # <<<<<<<<<<<<<<
  *             self.done = True
  *             self.vm.close()
  */
   __pyx_t_1 = (__pyx_v_row == Py_None);
   __pyx_t_3 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "unqlite.pyx":1256
+    /* "unqlite.pyx":1259
  *         row = self.vm['row']
  *         if row is None:
  *             self.done = True             # <<<<<<<<<<<<<<
  *             self.vm.close()
  *             self.vm = None
  */
     __pyx_v_self->done = 1;
 
-    /* "unqlite.pyx":1257
+    /* "unqlite.pyx":1260
  *         if row is None:
  *             self.done = True
  *             self.vm.close()             # <<<<<<<<<<<<<<
  *             self.vm = None
  *             raise StopIteration
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->close(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1257, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->close(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unqlite.pyx":1258
+    /* "unqlite.pyx":1261
  *             self.done = True
  *             self.vm.close()
  *             self.vm = None             # <<<<<<<<<<<<<<
  *             raise StopIteration
  * 
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->vm);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->vm));
     __pyx_v_self->vm = ((struct __pyx_obj_7unqlite_VM *)Py_None);
 
-    /* "unqlite.pyx":1259
+    /* "unqlite.pyx":1262
  *             self.vm.close()
  *             self.vm = None
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *         self.vm.reset()
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 1259, __pyx_L1_error)
+    __PYX_ERR(0, 1262, __pyx_L1_error)
 
-    /* "unqlite.pyx":1255
+    /* "unqlite.pyx":1258
  *         self.vm.execute()
  *         row = self.vm['row']
  *         if row is None:             # <<<<<<<<<<<<<<
  *             self.done = True
  *             self.vm.close()
  */
   }
 
-  /* "unqlite.pyx":1261
+  /* "unqlite.pyx":1264
  *             raise StopIteration
  * 
  *         self.vm.reset()             # <<<<<<<<<<<<<<
  *         return row
  * 
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->reset(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1261, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_self->vm->__pyx_vtab)->reset(__pyx_v_self->vm, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unqlite.pyx":1262
+  /* "unqlite.pyx":1265
  * 
  *         self.vm.reset()
  *         return row             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_row);
   __pyx_r = __pyx_v_row;
   goto __pyx_L0;
 
-  /* "unqlite.pyx":1249
+  /* "unqlite.pyx":1252
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.done:
  *             raise StopIteration
  */
 
@@ -22861,15 +22982,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_row);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1230
+/* "unqlite.pyx":1233
  *         UnQLite unqlite
  *         bint done
  *         public Collection collection             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, Collection collection):
  */
 
@@ -22919,15 +23040,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_7unqlite_Collection))))) __PYX_ERR(0, 1230, __pyx_L1_error)
+  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_7unqlite_Collection))))) __PYX_ERR(0, 1233, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->collection);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->collection));
   __pyx_v_self->collection = ((struct __pyx_obj_7unqlite_Collection *)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -23291,15 +23412,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1265
+/* "unqlite.pyx":1268
  * 
  * 
  * cdef unqlite_value_to_python(unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *     cdef list json_array
  *     cdef dict json_object
  */
 
@@ -23319,138 +23440,138 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unqlite_value_to_python", 0);
 
-  /* "unqlite.pyx":1269
+  /* "unqlite.pyx":1272
  *     cdef dict json_object
  * 
  *     if unqlite_value_is_json_object(ptr):             # <<<<<<<<<<<<<<
  *         json_object = {}
  *         unqlite_array_walk(
  */
   __pyx_t_1 = (unqlite_value_is_json_object(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1270
+    /* "unqlite.pyx":1273
  * 
  *     if unqlite_value_is_json_object(ptr):
  *         json_object = {}             # <<<<<<<<<<<<<<
  *         unqlite_array_walk(
  *             ptr,
  */
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_json_object = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "unqlite.pyx":1271
+    /* "unqlite.pyx":1274
  *     if unqlite_value_is_json_object(ptr):
  *         json_object = {}
  *         unqlite_array_walk(             # <<<<<<<<<<<<<<
  *             ptr,
  *             unqlite_value_to_dict,
  */
     (void)(unqlite_array_walk(__pyx_v_ptr, __pyx_f_7unqlite_unqlite_value_to_dict, ((void *)__pyx_v_json_object)));
 
-    /* "unqlite.pyx":1275
+    /* "unqlite.pyx":1278
  *             unqlite_value_to_dict,
  *             <void *>json_object)
  *         return json_object             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_json_array(ptr):
  *         json_array = []
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_json_object);
     __pyx_r = __pyx_v_json_object;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1269
+    /* "unqlite.pyx":1272
  *     cdef dict json_object
  * 
  *     if unqlite_value_is_json_object(ptr):             # <<<<<<<<<<<<<<
  *         json_object = {}
  *         unqlite_array_walk(
  */
   }
 
-  /* "unqlite.pyx":1276
+  /* "unqlite.pyx":1279
  *             <void *>json_object)
  *         return json_object
  *     elif unqlite_value_is_json_array(ptr):             # <<<<<<<<<<<<<<
  *         json_array = []
  *         unqlite_array_walk(
  */
   __pyx_t_1 = (unqlite_value_is_json_array(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1277
+    /* "unqlite.pyx":1280
  *         return json_object
  *     elif unqlite_value_is_json_array(ptr):
  *         json_array = []             # <<<<<<<<<<<<<<
  *         unqlite_array_walk(
  *             ptr,
  */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1277, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1280, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_json_array = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "unqlite.pyx":1278
+    /* "unqlite.pyx":1281
  *     elif unqlite_value_is_json_array(ptr):
  *         json_array = []
  *         unqlite_array_walk(             # <<<<<<<<<<<<<<
  *             ptr,
  *             unqlite_value_to_list,
  */
     (void)(unqlite_array_walk(__pyx_v_ptr, __pyx_f_7unqlite_unqlite_value_to_list, ((void *)__pyx_v_json_array)));
 
-    /* "unqlite.pyx":1282
+    /* "unqlite.pyx":1285
  *             unqlite_value_to_list,
  *             <void *>json_array)
  *         return json_array             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_string(ptr):
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_json_array);
     __pyx_r = __pyx_v_json_array;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1276
+    /* "unqlite.pyx":1279
  *             <void *>json_object)
  *         return json_object
  *     elif unqlite_value_is_json_array(ptr):             # <<<<<<<<<<<<<<
  *         json_array = []
  *         unqlite_array_walk(
  */
   }
 
-  /* "unqlite.pyx":1283
+  /* "unqlite.pyx":1286
  *             <void *>json_array)
  *         return json_array
  *     elif unqlite_value_is_string(ptr):             # <<<<<<<<<<<<<<
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:
  */
   __pyx_t_1 = (unqlite_value_is_string(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1284
+    /* "unqlite.pyx":1287
  *         return json_array
  *     elif unqlite_value_is_string(ptr):
  *         bytestring = unqlite_value_to_string(ptr, NULL)             # <<<<<<<<<<<<<<
  *         try:
  *             return decode(bytestring)
  */
     __pyx_v_bytestring = unqlite_value_to_string(__pyx_v_ptr, NULL);
 
-    /* "unqlite.pyx":1285
+    /* "unqlite.pyx":1288
  *     elif unqlite_value_is_string(ptr):
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:             # <<<<<<<<<<<<<<
  *             return decode(bytestring)
  *         except UnicodeDecodeError:
  */
     {
@@ -23458,79 +23579,79 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "unqlite.pyx":1286
+        /* "unqlite.pyx":1289
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:
  *             return decode(bytestring)             # <<<<<<<<<<<<<<
  *         except UnicodeDecodeError:
  *             return bytestring
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_bytestring); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1286, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_bytestring); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1289, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_6 = __pyx_f_7unqlite_decode(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1286, __pyx_L4_error)
+        __pyx_t_6 = __pyx_f_7unqlite_decode(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1289, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L8_try_return;
 
-        /* "unqlite.pyx":1285
+        /* "unqlite.pyx":1288
  *     elif unqlite_value_is_string(ptr):
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:             # <<<<<<<<<<<<<<
  *             return decode(bytestring)
  *         except UnicodeDecodeError:
  */
       }
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "unqlite.pyx":1287
+      /* "unqlite.pyx":1290
  *         try:
  *             return decode(bytestring)
  *         except UnicodeDecodeError:             # <<<<<<<<<<<<<<
  *             return bytestring
  *     elif unqlite_value_is_int(ptr):
  */
       __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_UnicodeDecodeError);
       if (__pyx_t_7) {
         __Pyx_AddTraceback("unqlite.unqlite_value_to_python", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_2, &__pyx_t_8) < 0) __PYX_ERR(0, 1287, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_2, &__pyx_t_8) < 0) __PYX_ERR(0, 1290, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_8);
 
-        /* "unqlite.pyx":1288
+        /* "unqlite.pyx":1291
  *             return decode(bytestring)
  *         except UnicodeDecodeError:
  *             return bytestring             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_int(ptr):
  *         return unqlite_value_to_int64(ptr)
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_9 = __Pyx_PyBytes_FromString(__pyx_v_bytestring); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1288, __pyx_L6_except_error)
+        __pyx_t_9 = __Pyx_PyBytes_FromString(__pyx_v_bytestring); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1291, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_r = __pyx_t_9;
         __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "unqlite.pyx":1285
+      /* "unqlite.pyx":1288
  *     elif unqlite_value_is_string(ptr):
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:             # <<<<<<<<<<<<<<
  *             return decode(bytestring)
  *         except UnicodeDecodeError:
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -23548,170 +23669,170 @@
       __Pyx_XGIVEREF(__pyx_t_3);
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
     }
 
-    /* "unqlite.pyx":1283
+    /* "unqlite.pyx":1286
  *             <void *>json_array)
  *         return json_array
  *     elif unqlite_value_is_string(ptr):             # <<<<<<<<<<<<<<
  *         bytestring = unqlite_value_to_string(ptr, NULL)
  *         try:
  */
   }
 
-  /* "unqlite.pyx":1289
+  /* "unqlite.pyx":1292
  *         except UnicodeDecodeError:
  *             return bytestring
  *     elif unqlite_value_is_int(ptr):             # <<<<<<<<<<<<<<
  *         return unqlite_value_to_int64(ptr)
  *     elif unqlite_value_is_float(ptr):
  */
   __pyx_t_1 = (unqlite_value_is_int(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1290
+    /* "unqlite.pyx":1293
  *             return bytestring
  *     elif unqlite_value_is_int(ptr):
  *         return unqlite_value_to_int64(ptr)             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_float(ptr):
  *         return unqlite_value_to_double(ptr)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_sxi64(unqlite_value_to_int64(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1290, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_sxi64(unqlite_value_to_int64(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1289
+    /* "unqlite.pyx":1292
  *         except UnicodeDecodeError:
  *             return bytestring
  *     elif unqlite_value_is_int(ptr):             # <<<<<<<<<<<<<<
  *         return unqlite_value_to_int64(ptr)
  *     elif unqlite_value_is_float(ptr):
  */
   }
 
-  /* "unqlite.pyx":1291
+  /* "unqlite.pyx":1294
  *     elif unqlite_value_is_int(ptr):
  *         return unqlite_value_to_int64(ptr)
  *     elif unqlite_value_is_float(ptr):             # <<<<<<<<<<<<<<
  *         return unqlite_value_to_double(ptr)
  *     elif unqlite_value_is_bool(ptr):
  */
   __pyx_t_1 = (unqlite_value_is_float(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1292
+    /* "unqlite.pyx":1295
  *         return unqlite_value_to_int64(ptr)
  *     elif unqlite_value_is_float(ptr):
  *         return unqlite_value_to_double(ptr)             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_bool(ptr):
  *         return bool(unqlite_value_to_bool(ptr))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = PyFloat_FromDouble(unqlite_value_to_double(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1292, __pyx_L1_error)
+    __pyx_t_8 = PyFloat_FromDouble(unqlite_value_to_double(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1291
+    /* "unqlite.pyx":1294
  *     elif unqlite_value_is_int(ptr):
  *         return unqlite_value_to_int64(ptr)
  *     elif unqlite_value_is_float(ptr):             # <<<<<<<<<<<<<<
  *         return unqlite_value_to_double(ptr)
  *     elif unqlite_value_is_bool(ptr):
  */
   }
 
-  /* "unqlite.pyx":1293
+  /* "unqlite.pyx":1296
  *     elif unqlite_value_is_float(ptr):
  *         return unqlite_value_to_double(ptr)
  *     elif unqlite_value_is_bool(ptr):             # <<<<<<<<<<<<<<
  *         return bool(unqlite_value_to_bool(ptr))
  *     elif unqlite_value_is_null(ptr):
  */
   __pyx_t_1 = (unqlite_value_is_bool(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1294
+    /* "unqlite.pyx":1297
  *         return unqlite_value_to_double(ptr)
  *     elif unqlite_value_is_bool(ptr):
  *         return bool(unqlite_value_to_bool(ptr))             # <<<<<<<<<<<<<<
  *     elif unqlite_value_is_null(ptr):
  *         return None
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_int(unqlite_value_to_bool(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1294, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int(unqlite_value_to_bool(__pyx_v_ptr)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1294, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1297, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyBool_FromLong((!(!__pyx_t_1))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1294, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyBool_FromLong((!(!__pyx_t_1))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1293
+    /* "unqlite.pyx":1296
  *     elif unqlite_value_is_float(ptr):
  *         return unqlite_value_to_double(ptr)
  *     elif unqlite_value_is_bool(ptr):             # <<<<<<<<<<<<<<
  *         return bool(unqlite_value_to_bool(ptr))
  *     elif unqlite_value_is_null(ptr):
  */
   }
 
-  /* "unqlite.pyx":1295
+  /* "unqlite.pyx":1298
  *     elif unqlite_value_is_bool(ptr):
  *         return bool(unqlite_value_to_bool(ptr))
  *     elif unqlite_value_is_null(ptr):             # <<<<<<<<<<<<<<
  *         return None
  *     raise TypeError('Unrecognized type.')
  */
   __pyx_t_1 = (unqlite_value_is_null(__pyx_v_ptr) != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1296
+    /* "unqlite.pyx":1299
  *         return bool(unqlite_value_to_bool(ptr))
  *     elif unqlite_value_is_null(ptr):
  *         return None             # <<<<<<<<<<<<<<
  *     raise TypeError('Unrecognized type.')
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "unqlite.pyx":1295
+    /* "unqlite.pyx":1298
  *     elif unqlite_value_is_bool(ptr):
  *         return bool(unqlite_value_to_bool(ptr))
  *     elif unqlite_value_is_null(ptr):             # <<<<<<<<<<<<<<
  *         return None
  *     raise TypeError('Unrecognized type.')
  */
   }
 
-  /* "unqlite.pyx":1297
+  /* "unqlite.pyx":1300
  *     elif unqlite_value_is_null(ptr):
  *         return None
  *     raise TypeError('Unrecognized type.')             # <<<<<<<<<<<<<<
  * 
  * cdef python_to_unqlite_value(VM vm, unqlite_value *ptr, python_value):
  */
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1297, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_Raise(__pyx_t_8, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __PYX_ERR(0, 1297, __pyx_L1_error)
+  __PYX_ERR(0, 1300, __pyx_L1_error)
 
-  /* "unqlite.pyx":1265
+  /* "unqlite.pyx":1268
  * 
  * 
  * cdef unqlite_value_to_python(unqlite_value *ptr):             # <<<<<<<<<<<<<<
  *     cdef list json_array
  *     cdef dict json_object
  */
 
@@ -23727,15 +23848,15 @@
   __Pyx_XDECREF(__pyx_v_json_array);
   __Pyx_XDECREF(__pyx_v_json_object);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1299
+/* "unqlite.pyx":1302
  *     raise TypeError('Unrecognized type.')
  * 
  * cdef python_to_unqlite_value(VM vm, unqlite_value *ptr, python_value):             # <<<<<<<<<<<<<<
  *     cdef unqlite_value *item_ptr = <unqlite_value *>0
  *     cdef bytes encoded_value
  */
 
@@ -23763,102 +23884,102 @@
   unqlite_int64 __pyx_t_14;
   double __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("python_to_unqlite_value", 0);
 
-  /* "unqlite.pyx":1300
+  /* "unqlite.pyx":1303
  * 
  * cdef python_to_unqlite_value(VM vm, unqlite_value *ptr, python_value):
  *     cdef unqlite_value *item_ptr = <unqlite_value *>0             # <<<<<<<<<<<<<<
  *     cdef bytes encoded_value
  * 
  */
   __pyx_v_item_ptr = ((unqlite_value *)0);
 
-  /* "unqlite.pyx":1303
+  /* "unqlite.pyx":1306
  *     cdef bytes encoded_value
  * 
  *     if isinstance(python_value, unicode):             # <<<<<<<<<<<<<<
  *         encoded_value = encode(python_value)
  *         unqlite_value_string(ptr, encoded_value, -1)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1304
+    /* "unqlite.pyx":1307
  * 
  *     if isinstance(python_value, unicode):
  *         encoded_value = encode(python_value)             # <<<<<<<<<<<<<<
  *         unqlite_value_string(ptr, encoded_value, -1)
  *     elif isinstance(python_value, bytes):
  */
-    __pyx_t_3 = __pyx_f_7unqlite_encode(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1304, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_7unqlite_encode(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_encoded_value = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1305
+    /* "unqlite.pyx":1308
  *     if isinstance(python_value, unicode):
  *         encoded_value = encode(python_value)
  *         unqlite_value_string(ptr, encoded_value, -1)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, bytes):
  *         unqlite_value_string(ptr, python_value, -1)
  */
     if (unlikely(__pyx_v_encoded_value == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 1305, __pyx_L1_error)
+      __PYX_ERR(0, 1308, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1305, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1308, __pyx_L1_error)
     (void)(unqlite_value_string(__pyx_v_ptr, __pyx_t_4, -1));
 
-    /* "unqlite.pyx":1303
+    /* "unqlite.pyx":1306
  *     cdef bytes encoded_value
  * 
  *     if isinstance(python_value, unicode):             # <<<<<<<<<<<<<<
  *         encoded_value = encode(python_value)
  *         unqlite_value_string(ptr, encoded_value, -1)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1306
+  /* "unqlite.pyx":1309
  *         encoded_value = encode(python_value)
  *         unqlite_value_string(ptr, encoded_value, -1)
  *     elif isinstance(python_value, bytes):             # <<<<<<<<<<<<<<
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1307
+    /* "unqlite.pyx":1310
  *         unqlite_value_string(ptr, encoded_value, -1)
  *     elif isinstance(python_value, bytes):
  *         unqlite_value_string(ptr, python_value, -1)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, (list, tuple)):
  *         for item in python_value:
  */
-    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_v_python_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1307, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_v_python_value); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 1310, __pyx_L1_error)
     (void)(unqlite_value_string(__pyx_v_ptr, __pyx_t_4, -1));
 
-    /* "unqlite.pyx":1306
+    /* "unqlite.pyx":1309
  *         encoded_value = encode(python_value)
  *         unqlite_value_string(ptr, encoded_value, -1)
  *     elif isinstance(python_value, bytes):             # <<<<<<<<<<<<<<
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1308
+  /* "unqlite.pyx":1311
  *     elif isinstance(python_value, bytes):
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):             # <<<<<<<<<<<<<<
  *         for item in python_value:
  *             item_ptr = vm.create_value(item)
  */
   __pyx_t_2 = PyList_Check(__pyx_v_python_value); 
@@ -23871,252 +23992,252 @@
   __pyx_t_5 = PyTuple_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_5 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1309
+    /* "unqlite.pyx":1312
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):
  *         for item in python_value:             # <<<<<<<<<<<<<<
  *             item_ptr = vm.create_value(item)
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  */
     if (likely(PyList_CheckExact(__pyx_v_python_value)) || PyTuple_CheckExact(__pyx_v_python_value)) {
       __pyx_t_3 = __pyx_v_python_value; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1309, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_python_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1309, __pyx_L1_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1312, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1309, __pyx_L1_error)
+          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1312, __pyx_L1_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1309, __pyx_L1_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1312, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1309, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1312, __pyx_L1_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1309, __pyx_L1_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1312, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         }
       } else {
         __pyx_t_8 = __pyx_t_7(__pyx_t_3);
         if (unlikely(!__pyx_t_8)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 1309, __pyx_L1_error)
+            else __PYX_ERR(0, 1312, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_8);
       }
       __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_8);
       __pyx_t_8 = 0;
 
-      /* "unqlite.pyx":1310
+      /* "unqlite.pyx":1313
  *     elif isinstance(python_value, (list, tuple)):
  *         for item in python_value:
  *             item_ptr = vm.create_value(item)             # <<<<<<<<<<<<<<
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  *             vm.release_value(item_ptr)
  */
       __pyx_v_item_ptr = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->create_value(__pyx_v_vm, __pyx_v_item);
 
-      /* "unqlite.pyx":1311
+      /* "unqlite.pyx":1314
  *         for item in python_value:
  *             item_ptr = vm.create_value(item)
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)             # <<<<<<<<<<<<<<
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, dict):
  */
       (void)(unqlite_array_add_elem(__pyx_v_ptr, NULL, __pyx_v_item_ptr));
 
-      /* "unqlite.pyx":1312
+      /* "unqlite.pyx":1315
  *             item_ptr = vm.create_value(item)
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  *             vm.release_value(item_ptr)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, dict):
  *         for key, value in python_value.items():
  */
-      __pyx_t_8 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->release_value(__pyx_v_vm, __pyx_v_item_ptr); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1312, __pyx_L1_error)
+      __pyx_t_8 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->release_value(__pyx_v_vm, __pyx_v_item_ptr); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1315, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "unqlite.pyx":1309
+      /* "unqlite.pyx":1312
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):
  *         for item in python_value:             # <<<<<<<<<<<<<<
  *             item_ptr = vm.create_value(item)
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1308
+    /* "unqlite.pyx":1311
  *     elif isinstance(python_value, bytes):
  *         unqlite_value_string(ptr, python_value, -1)
  *     elif isinstance(python_value, (list, tuple)):             # <<<<<<<<<<<<<<
  *         for item in python_value:
  *             item_ptr = vm.create_value(item)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1313
+  /* "unqlite.pyx":1316
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, dict):             # <<<<<<<<<<<<<<
  *         for key, value in python_value.items():
  *             encoded_value = encode(key)
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1314
+    /* "unqlite.pyx":1317
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, dict):
  *         for key, value in python_value.items():             # <<<<<<<<<<<<<<
  *             encoded_value = encode(key)
  *             item_ptr = vm.create_value(value)
  */
     __pyx_t_6 = 0;
     if (unlikely(__pyx_v_python_value == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 1314, __pyx_L1_error)
+      __PYX_ERR(0, 1317, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_python_value, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1314, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_python_value, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1317, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_8;
     __pyx_t_8 = 0;
     while (1) {
       __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_9, &__pyx_t_6, &__pyx_t_8, &__pyx_t_11, NULL, __pyx_t_10);
       if (unlikely(__pyx_t_12 == 0)) break;
-      if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1314, __pyx_L1_error)
+      if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1317, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "unqlite.pyx":1315
+      /* "unqlite.pyx":1318
  *     elif isinstance(python_value, dict):
  *         for key, value in python_value.items():
  *             encoded_value = encode(key)             # <<<<<<<<<<<<<<
  *             item_ptr = vm.create_value(value)
  *             unqlite_array_add_strkey_elem(
  */
-      __pyx_t_11 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1315, __pyx_L1_error)
+      __pyx_t_11 = __pyx_f_7unqlite_encode(__pyx_v_key); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1318, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_XDECREF_SET(__pyx_v_encoded_value, ((PyObject*)__pyx_t_11));
       __pyx_t_11 = 0;
 
-      /* "unqlite.pyx":1316
+      /* "unqlite.pyx":1319
  *         for key, value in python_value.items():
  *             encoded_value = encode(key)
  *             item_ptr = vm.create_value(value)             # <<<<<<<<<<<<<<
  *             unqlite_array_add_strkey_elem(
  *                 ptr,
  */
       __pyx_v_item_ptr = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->create_value(__pyx_v_vm, __pyx_v_value);
 
-      /* "unqlite.pyx":1319
+      /* "unqlite.pyx":1322
  *             unqlite_array_add_strkey_elem(
  *                 ptr,
  *                 <const char *>encoded_value,             # <<<<<<<<<<<<<<
  *                 item_ptr)
  *             vm.release_value(item_ptr)
  */
       if (unlikely(__pyx_v_encoded_value == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-        __PYX_ERR(0, 1319, __pyx_L1_error)
+        __PYX_ERR(0, 1322, __pyx_L1_error)
       }
-      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 1319, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_v_encoded_value); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 1322, __pyx_L1_error)
 
-      /* "unqlite.pyx":1317
+      /* "unqlite.pyx":1320
  *             encoded_value = encode(key)
  *             item_ptr = vm.create_value(value)
  *             unqlite_array_add_strkey_elem(             # <<<<<<<<<<<<<<
  *                 ptr,
  *                 <const char *>encoded_value,
  */
       (void)(unqlite_array_add_strkey_elem(__pyx_v_ptr, ((char const *)__pyx_t_13), __pyx_v_item_ptr));
 
-      /* "unqlite.pyx":1321
+      /* "unqlite.pyx":1324
  *                 <const char *>encoded_value,
  *                 item_ptr)
  *             vm.release_value(item_ptr)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, bool):
  *         unqlite_value_bool(ptr, python_value)
  */
-      __pyx_t_11 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->release_value(__pyx_v_vm, __pyx_v_item_ptr); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1321, __pyx_L1_error)
+      __pyx_t_11 = ((struct __pyx_vtabstruct_7unqlite_VM *)__pyx_v_vm->__pyx_vtab)->release_value(__pyx_v_vm, __pyx_v_item_ptr); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1324, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "unqlite.pyx":1313
+    /* "unqlite.pyx":1316
  *             unqlite_array_add_elem(ptr, NULL, item_ptr)
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, dict):             # <<<<<<<<<<<<<<
  *         for key, value in python_value.items():
  *             encoded_value = encode(key)
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1322
+  /* "unqlite.pyx":1325
  *                 item_ptr)
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, bool):             # <<<<<<<<<<<<<<
  *         unqlite_value_bool(ptr, python_value)
  *     elif isinstance(python_value, (int, long)):
  */
   __pyx_t_3 = ((PyObject*)&PyBool_Type);
   __Pyx_INCREF(__pyx_t_3);
-  __pyx_t_1 = PyObject_IsInstance(__pyx_v_python_value, __pyx_t_3); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1322, __pyx_L1_error)
+  __pyx_t_1 = PyObject_IsInstance(__pyx_v_python_value, __pyx_t_3); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1325, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1323
+    /* "unqlite.pyx":1326
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, bool):
  *         unqlite_value_bool(ptr, python_value)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, (int, long)):
  *         unqlite_value_int64(ptr, python_value)
  */
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_python_value); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1323, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_python_value); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1326, __pyx_L1_error)
     (void)(unqlite_value_bool(__pyx_v_ptr, __pyx_t_10));
 
-    /* "unqlite.pyx":1322
+    /* "unqlite.pyx":1325
  *                 item_ptr)
  *             vm.release_value(item_ptr)
  *     elif isinstance(python_value, bool):             # <<<<<<<<<<<<<<
  *         unqlite_value_bool(ptr, python_value)
  *     elif isinstance(python_value, (int, long)):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1324
+  /* "unqlite.pyx":1327
  *     elif isinstance(python_value, bool):
  *         unqlite_value_bool(ptr, python_value)
  *     elif isinstance(python_value, (int, long)):             # <<<<<<<<<<<<<<
  *         unqlite_value_int64(ptr, python_value)
  *     elif isinstance(python_value, float):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_python_value); 
@@ -24129,78 +24250,78 @@
   __pyx_t_5 = PyLong_Check(__pyx_v_python_value); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L10_bool_binop_done:;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "unqlite.pyx":1325
+    /* "unqlite.pyx":1328
  *         unqlite_value_bool(ptr, python_value)
  *     elif isinstance(python_value, (int, long)):
  *         unqlite_value_int64(ptr, python_value)             # <<<<<<<<<<<<<<
  *     elif isinstance(python_value, float):
  *         unqlite_value_double(ptr, python_value)
  */
-    __pyx_t_14 = __Pyx_PyInt_As_sxi64(__pyx_v_python_value); if (unlikely((__pyx_t_14 == ((unqlite_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1325, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_As_sxi64(__pyx_v_python_value); if (unlikely((__pyx_t_14 == ((unqlite_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1328, __pyx_L1_error)
     (void)(unqlite_value_int64(__pyx_v_ptr, __pyx_t_14));
 
-    /* "unqlite.pyx":1324
+    /* "unqlite.pyx":1327
  *     elif isinstance(python_value, bool):
  *         unqlite_value_bool(ptr, python_value)
  *     elif isinstance(python_value, (int, long)):             # <<<<<<<<<<<<<<
  *         unqlite_value_int64(ptr, python_value)
  *     elif isinstance(python_value, float):
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1326
+  /* "unqlite.pyx":1329
  *     elif isinstance(python_value, (int, long)):
  *         unqlite_value_int64(ptr, python_value)
  *     elif isinstance(python_value, float):             # <<<<<<<<<<<<<<
  *         unqlite_value_double(ptr, python_value)
  *     else:
  */
   __pyx_t_1 = PyFloat_Check(__pyx_v_python_value); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "unqlite.pyx":1327
+    /* "unqlite.pyx":1330
  *         unqlite_value_int64(ptr, python_value)
  *     elif isinstance(python_value, float):
  *         unqlite_value_double(ptr, python_value)             # <<<<<<<<<<<<<<
  *     else:
  *         unqlite_value_null(ptr)
  */
-    __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_python_value); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1327, __pyx_L1_error)
+    __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_python_value); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1330, __pyx_L1_error)
     (void)(unqlite_value_double(__pyx_v_ptr, __pyx_t_15));
 
-    /* "unqlite.pyx":1326
+    /* "unqlite.pyx":1329
  *     elif isinstance(python_value, (int, long)):
  *         unqlite_value_int64(ptr, python_value)
  *     elif isinstance(python_value, float):             # <<<<<<<<<<<<<<
  *         unqlite_value_double(ptr, python_value)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "unqlite.pyx":1329
+  /* "unqlite.pyx":1332
  *         unqlite_value_double(ptr, python_value)
  *     else:
  *         unqlite_value_null(ptr)             # <<<<<<<<<<<<<<
  * 
- * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data):
+ * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
  */
   /*else*/ {
     (void)(unqlite_value_null(__pyx_v_ptr));
   }
   __pyx_L3:;
 
-  /* "unqlite.pyx":1299
+  /* "unqlite.pyx":1302
  *     raise TypeError('Unrecognized type.')
  * 
  * cdef python_to_unqlite_value(VM vm, unqlite_value *ptr, python_value):             # <<<<<<<<<<<<<<
  *     cdef unqlite_value *item_ptr = <unqlite_value *>0
  *     cdef bytes encoded_value
  */
 
@@ -24219,18 +24340,18 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1331
+/* "unqlite.pyx":1334
  *         unqlite_value_null(ptr)
  * 
- * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data):             # <<<<<<<<<<<<<<
+ * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:             # <<<<<<<<<<<<<<
  *     cdef list accum
  *     accum = <list>user_data
  */
 
 static int __pyx_f_7unqlite_unqlite_value_to_list(CYTHON_UNUSED unqlite_value *__pyx_v_key, unqlite_value *__pyx_v_value, void *__pyx_v_user_data) {
   PyObject *__pyx_v_accum = 0;
   int __pyx_r;
@@ -24238,46 +24359,46 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unqlite_value_to_list", 0);
 
-  /* "unqlite.pyx":1333
- * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data):
+  /* "unqlite.pyx":1336
+ * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
  *     cdef list accum
  *     accum = <list>user_data             # <<<<<<<<<<<<<<
  *     accum.append(unqlite_value_to_python(value))
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_accum = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1334
+  /* "unqlite.pyx":1337
  *     cdef list accum
  *     accum = <list>user_data
  *     accum.append(unqlite_value_to_python(value))             # <<<<<<<<<<<<<<
  * 
- * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data):
+ * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
  */
   if (unlikely(__pyx_v_accum == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-    __PYX_ERR(0, 1334, __pyx_L1_error)
+    __PYX_ERR(0, 1337, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1334, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyList_Append(__pyx_v_accum, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 1334, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyList_Append(__pyx_v_accum, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 1337, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1331
+  /* "unqlite.pyx":1334
  *         unqlite_value_null(ptr)
  * 
- * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data):             # <<<<<<<<<<<<<<
+ * cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:             # <<<<<<<<<<<<<<
  *     cdef list accum
  *     accum = <list>user_data
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -24287,18 +24408,18 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_accum);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unqlite.pyx":1336
+/* "unqlite.pyx":1339
  *     accum.append(unqlite_value_to_python(value))
  * 
- * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data):             # <<<<<<<<<<<<<<
+ * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:             # <<<<<<<<<<<<<<
  *     cdef dict accum
  *     accum = <dict>user_data
  */
 
 static int __pyx_f_7unqlite_unqlite_value_to_dict(unqlite_value *__pyx_v_key, unqlite_value *__pyx_v_value, void *__pyx_v_user_data) {
   PyObject *__pyx_v_accum = 0;
   PyObject *__pyx_v_pkey = NULL;
@@ -24306,55 +24427,55 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unqlite_value_to_dict", 0);
 
-  /* "unqlite.pyx":1338
- * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data):
+  /* "unqlite.pyx":1341
+ * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
  *     cdef dict accum
  *     accum = <dict>user_data             # <<<<<<<<<<<<<<
  *     pkey = unqlite_value_to_python(key)
  *     accum[pkey] = unqlite_value_to_python(value)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_accum = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1339
+  /* "unqlite.pyx":1342
  *     cdef dict accum
  *     accum = <dict>user_data
  *     pkey = unqlite_value_to_python(key)             # <<<<<<<<<<<<<<
  *     accum[pkey] = unqlite_value_to_python(value)
  */
-  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1339, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pkey = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1340
+  /* "unqlite.pyx":1343
  *     accum = <dict>user_data
  *     pkey = unqlite_value_to_python(key)
  *     accum[pkey] = unqlite_value_to_python(value)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1340, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7unqlite_unqlite_value_to_python(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_v_accum == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 1340, __pyx_L1_error)
+    __PYX_ERR(0, 1343, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_accum, __pyx_v_pkey, __pyx_t_1) < 0)) __PYX_ERR(0, 1340, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_accum, __pyx_v_pkey, __pyx_t_1) < 0)) __PYX_ERR(0, 1343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unqlite.pyx":1336
+  /* "unqlite.pyx":1339
  *     accum.append(unqlite_value_to_python(value))
  * 
- * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data):             # <<<<<<<<<<<<<<
+ * cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:             # <<<<<<<<<<<<<<
  *     cdef dict accum
  *     accum = <dict>user_data
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -25640,15 +25761,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_UnQLite(PyObject *o) {
   struct __pyx_obj_7unqlite_UnQLite *p = (struct __pyx_obj_7unqlite_UnQLite *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -25821,15 +25942,15 @@
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
 
 static PyObject *__pyx_tp_new_7unqlite_Transaction(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Transaction *p;
   PyObject *o;
@@ -25843,15 +25964,15 @@
   p->unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Transaction(PyObject *o) {
   struct __pyx_obj_7unqlite_Transaction *p = (struct __pyx_obj_7unqlite_Transaction *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->unqlite);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -25945,15 +26066,15 @@
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
 static struct __pyx_vtabstruct_7unqlite_Cursor __pyx_vtable_7unqlite_Cursor;
 
 static PyObject *__pyx_tp_new_7unqlite_Cursor(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7unqlite_Cursor *p;
@@ -25973,15 +26094,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Cursor(PyObject *o) {
   struct __pyx_obj_7unqlite_Cursor *p = (struct __pyx_obj_7unqlite_Cursor *)o;
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
@@ -26097,15 +26218,15 @@
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
 static struct __pyx_vtabstruct_7unqlite_VM __pyx_vtable_7unqlite_VM;
 
 static PyObject *__pyx_tp_new_7unqlite_VM(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7unqlite_VM *p;
@@ -26128,15 +26249,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_VM(PyObject *o) {
   struct __pyx_obj_7unqlite_VM *p = (struct __pyx_obj_7unqlite_VM *)o;
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
@@ -26316,15 +26437,15 @@
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
 static struct __pyx_vtabstruct_7unqlite_Context __pyx_vtable_7unqlite_Context;
 
 static PyObject *__pyx_tp_new_7unqlite_Context(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Context *p;
@@ -26342,15 +26463,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Context(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_7unqlite_Context[] = {
@@ -26423,15 +26544,15 @@
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
 static struct __pyx_vtabstruct_7unqlite_Collection __pyx_vtable_7unqlite_Collection;
 
 static PyObject *__pyx_tp_new_7unqlite_Collection(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Collection *p;
@@ -26448,15 +26569,15 @@
   p->name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Collection(PyObject *o) {
   struct __pyx_obj_7unqlite_Collection *p = (struct __pyx_obj_7unqlite_Collection *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->unqlite);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
@@ -26604,15 +26725,15 @@
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
 
 static PyObject *__pyx_tp_new_7unqlite_CollectionIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_CollectionIterator *p;
   PyObject *o;
@@ -26628,15 +26749,15 @@
   p->collection = ((struct __pyx_obj_7unqlite_Collection *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_CollectionIterator(PyObject *o) {
   struct __pyx_obj_7unqlite_CollectionIterator *p = (struct __pyx_obj_7unqlite_CollectionIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->vm);
   Py_CLEAR(p->unqlite);
   Py_CLEAR(p->collection);
@@ -26763,15 +26884,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct__commit_on_success *__pyx_freelist_7unqlite___pyx_scope_struct__commit_on_success[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct__commit_on_success = 0;
 
@@ -26888,15 +27009,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_1_keys *__pyx_freelist_7unqlite___pyx_scope_struct_1_keys[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_1_keys = 0;
 
@@ -27017,15 +27138,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_2_values *__pyx_freelist_7unqlite___pyx_scope_struct_2_values[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_2_values = 0;
 
@@ -27146,15 +27267,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_3_items *__pyx_freelist_7unqlite___pyx_scope_struct_3_items[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_3_items = 0;
 
@@ -27283,15 +27404,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_4_range *__pyx_freelist_7unqlite___pyx_scope_struct_4_range[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_4_range = 0;
 
@@ -27317,14 +27438,17 @@
   Py_CLEAR(p->__pyx_v_item);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_start_key);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
   Py_CLEAR(p->__pyx_t_3);
+  Py_CLEAR(p->__pyx_t_4);
+  Py_CLEAR(p->__pyx_t_5);
+  Py_CLEAR(p->__pyx_t_6);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_7unqlite___pyx_scope_struct_4_range < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7unqlite___pyx_scope_struct_4_range)))) {
     __pyx_freelist_7unqlite___pyx_scope_struct_4_range[__pyx_freecount_7unqlite___pyx_scope_struct_4_range++] = ((struct __pyx_obj_7unqlite___pyx_scope_struct_4_range *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
@@ -27354,14 +27478,23 @@
   }
   if (p->__pyx_t_2) {
     e = (*v)(p->__pyx_t_2, a); if (e) return e;
   }
   if (p->__pyx_t_3) {
     e = (*v)(p->__pyx_t_3, a); if (e) return e;
   }
+  if (p->__pyx_t_4) {
+    e = (*v)(p->__pyx_t_4, a); if (e) return e;
+  }
+  if (p->__pyx_t_5) {
+    e = (*v)(p->__pyx_t_5, a); if (e) return e;
+  }
+  if (p->__pyx_t_6) {
+    e = (*v)(p->__pyx_t_6, a); if (e) return e;
+  }
   return 0;
 }
 
 static PyTypeObject __pyx_type_7unqlite___pyx_scope_struct_4_range = {
   PyVarObject_HEAD_INIT(0, 0)
   "unqlite.__pyx_scope_struct_4_range", /*tp_name*/
   sizeof(struct __pyx_obj_7unqlite___pyx_scope_struct_4_range), /*tp_basicsize*/
@@ -27424,15 +27557,15 @@
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
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until *__pyx_freelist_7unqlite___pyx_scope_struct_5_fetch_until[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_5_fetch_until = 0;
 
@@ -27549,15 +27682,15 @@
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
@@ -27788,17 +27921,17 @@
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 308, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 309, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 310, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 584, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 787, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 1053, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 1094, __pyx_L1_error)
+  __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 1056, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 1097, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -27910,44 +28043,44 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "unqlite.pyx":1094
+  /* "unqlite.pyx":1097
  *                 return vm['ret']
  *             except KeyError:
  *                 raise ValueError('Error fetching return value from script.')             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_Error_fetching_return_value_from); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 1094, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_Error_fetching_return_value_from); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "unqlite.pyx":1164
+  /* "unqlite.pyx":1167
  *         schema = _schema or {}
  *         if kwargs: schema.update(kwargs)
  *         return self._simple_execute(             # <<<<<<<<<<<<<<
  *             '$ret = db_set_schema($collection, $schema);', schema=schema)
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_ret_db_set_schema_collection_sc); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1164, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_ret_db_set_schema_collection_sc); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 1167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "unqlite.pyx":1297
+  /* "unqlite.pyx":1300
  *     elif unqlite_value_is_null(ptr):
  *         return None
  *     raise TypeError('Unrecognized type.')             # <<<<<<<<<<<<<<
  * 
  * cdef python_to_unqlite_value(VM vm, unqlite_value *ptr, python_value):
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_Unrecognized_type); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 1297, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_Unrecognized_type); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 1300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf669416, 0xf694ab9, 0x0b46877):             # <<<<<<<<<<<<<<
@@ -28101,118 +28234,118 @@
     }
   }
   #endif
   if (__Pyx_SetVtable(__pyx_type_7unqlite_UnQLite.tp_dict, __pyx_vtabptr_7unqlite_UnQLite) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_UnQLite, (PyObject *)&__pyx_type_7unqlite_UnQLite) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_UnQLite) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
   __pyx_ptype_7unqlite_UnQLite = &__pyx_type_7unqlite_UnQLite;
-  if (PyType_Ready(&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_Transaction.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_Transaction.tp_dictoffset && __pyx_type_7unqlite_Transaction.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_Transaction.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Transaction, (PyObject *)&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Transaction, (PyObject *)&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Transaction) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
   __pyx_ptype_7unqlite_Transaction = &__pyx_type_7unqlite_Transaction;
   __pyx_vtabptr_7unqlite_Cursor = &__pyx_vtable_7unqlite_Cursor;
   __pyx_vtable_7unqlite_Cursor.reset = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_reset;
   __pyx_vtable_7unqlite_Cursor.seek = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7unqlite_6Cursor_seek *__pyx_optional_args))__pyx_f_7unqlite_6Cursor_seek;
   __pyx_vtable_7unqlite_Cursor.first = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_first;
   __pyx_vtable_7unqlite_Cursor.last = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_last;
   __pyx_vtable_7unqlite_Cursor.next_entry = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_next_entry;
   __pyx_vtable_7unqlite_Cursor.previous_entry = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_previous_entry;
   __pyx_vtable_7unqlite_Cursor.is_valid = (int (*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_is_valid;
   __pyx_vtable_7unqlite_Cursor.key = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_key;
   __pyx_vtable_7unqlite_Cursor.value = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_value;
   __pyx_vtable_7unqlite_Cursor.delete = (PyObject *(*)(struct __pyx_obj_7unqlite_Cursor *, int __pyx_skip_dispatch))__pyx_f_7unqlite_6Cursor_delete;
-  if (PyType_Ready(&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_Cursor.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_Cursor.tp_dictoffset && __pyx_type_7unqlite_Cursor.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_Cursor.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7unqlite_Cursor.tp_dict, __pyx_vtabptr_7unqlite_Cursor) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Cursor, (PyObject *)&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7unqlite_Cursor.tp_dict, __pyx_vtabptr_7unqlite_Cursor) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Cursor, (PyObject *)&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Cursor) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
   __pyx_ptype_7unqlite_Cursor = &__pyx_type_7unqlite_Cursor;
   __pyx_vtabptr_7unqlite_VM = &__pyx_vtable_7unqlite_VM;
   __pyx_vtable_7unqlite_VM.compile = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, int __pyx_skip_dispatch))__pyx_f_7unqlite_2VM_compile;
   __pyx_vtable_7unqlite_VM.execute = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, int __pyx_skip_dispatch))__pyx_f_7unqlite_2VM_execute;
   __pyx_vtable_7unqlite_VM.reset = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, int __pyx_skip_dispatch))__pyx_f_7unqlite_2VM_reset;
   __pyx_vtable_7unqlite_VM.close = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, int __pyx_skip_dispatch))__pyx_f_7unqlite_2VM_close;
   __pyx_vtable_7unqlite_VM.create_value = (unqlite_value *(*)(struct __pyx_obj_7unqlite_VM *, PyObject *))__pyx_f_7unqlite_2VM_create_value;
   __pyx_vtable_7unqlite_VM.release_value = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, unqlite_value *))__pyx_f_7unqlite_2VM_release_value;
   __pyx_vtable_7unqlite_VM.create_array = (unqlite_value *(*)(struct __pyx_obj_7unqlite_VM *))__pyx_f_7unqlite_2VM_create_array;
   __pyx_vtable_7unqlite_VM.create_scalar = (unqlite_value *(*)(struct __pyx_obj_7unqlite_VM *))__pyx_f_7unqlite_2VM_create_scalar;
   __pyx_vtable_7unqlite_VM.set_values = (PyObject *(*)(struct __pyx_obj_7unqlite_VM *, PyObject *, int __pyx_skip_dispatch))__pyx_f_7unqlite_2VM_set_values;
-  if (PyType_Ready(&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_VM.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_VM.tp_dictoffset && __pyx_type_7unqlite_VM.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_VM.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7unqlite_VM.tp_dict, __pyx_vtabptr_7unqlite_VM) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_VM, (PyObject *)&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7unqlite_VM.tp_dict, __pyx_vtabptr_7unqlite_VM) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_VM, (PyObject *)&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_VM) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
   __pyx_ptype_7unqlite_VM = &__pyx_type_7unqlite_VM;
   __pyx_vtabptr_7unqlite_Context = &__pyx_vtable_7unqlite_Context;
   __pyx_vtable_7unqlite_Context.set_context = (PyObject *(*)(struct __pyx_obj_7unqlite_Context *, unqlite_context *))__pyx_f_7unqlite_7Context_set_context;
   __pyx_vtable_7unqlite_Context.create_value = (unqlite_value *(*)(struct __pyx_obj_7unqlite_Context *, PyObject *))__pyx_f_7unqlite_7Context_create_value;
   __pyx_vtable_7unqlite_Context.release_value = (PyObject *(*)(struct __pyx_obj_7unqlite_Context *, unqlite_value *))__pyx_f_7unqlite_7Context_release_value;
   __pyx_vtable_7unqlite_Context.create_array = (unqlite_value *(*)(struct __pyx_obj_7unqlite_Context *))__pyx_f_7unqlite_7Context_create_array;
   __pyx_vtable_7unqlite_Context.create_scalar = (unqlite_value *(*)(struct __pyx_obj_7unqlite_Context *))__pyx_f_7unqlite_7Context_create_scalar;
   __pyx_vtable_7unqlite_Context.push_result = (PyObject *(*)(struct __pyx_obj_7unqlite_Context *, PyObject *, int __pyx_skip_dispatch))__pyx_f_7unqlite_7Context_push_result;
   __pyx_vtable_7unqlite_Context.python_to_unqlite_value = (PyObject *(*)(struct __pyx_obj_7unqlite_Context *, unqlite_value *, PyObject *))__pyx_f_7unqlite_7Context_python_to_unqlite_value;
-  if (PyType_Ready(&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 980, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_Context.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_Context.tp_dictoffset && __pyx_type_7unqlite_Context.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_Context.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7unqlite_Context.tp_dict, __pyx_vtabptr_7unqlite_Context) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Context, (PyObject *)&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7unqlite_Context.tp_dict, __pyx_vtabptr_7unqlite_Context) < 0) __PYX_ERR(0, 980, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Context, (PyObject *)&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 980, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Context) < 0) __PYX_ERR(0, 980, __pyx_L1_error)
   __pyx_ptype_7unqlite_Context = &__pyx_type_7unqlite_Context;
   __pyx_vtabptr_7unqlite_Collection = &__pyx_vtable_7unqlite_Collection;
   __pyx_vtable_7unqlite_Collection.filter = (PyObject *(*)(struct __pyx_obj_7unqlite_Collection *, PyObject *, int __pyx_skip_dispatch))__pyx_f_7unqlite_10Collection_filter;
-  if (PyType_Ready(&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1067, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_Collection.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_Collection.tp_dictoffset && __pyx_type_7unqlite_Collection.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_Collection.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_7unqlite_Collection, "__len__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1067, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_7unqlite_Collection, "__len__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1070, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_7unqlite_10Collection_28__len__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_7unqlite_10Collection_28__len__.doc = __pyx_doc_7unqlite_10Collection_28__len__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_7unqlite_10Collection_28__len__;
     }
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_type_7unqlite_Collection.tp_dict, __pyx_vtabptr_7unqlite_Collection) < 0) __PYX_ERR(0, 1067, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Collection, (PyObject *)&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1067, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1067, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7unqlite_Collection.tp_dict, __pyx_vtabptr_7unqlite_Collection) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Collection, (PyObject *)&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_Collection) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
   __pyx_ptype_7unqlite_Collection = &__pyx_type_7unqlite_Collection;
-  if (PyType_Ready(&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1225, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1228, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite_CollectionIterator.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite_CollectionIterator.tp_dictoffset && __pyx_type_7unqlite_CollectionIterator.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite_CollectionIterator.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CollectionIterator, (PyObject *)&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1225, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1225, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CollectionIterator, (PyObject *)&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1228, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7unqlite_CollectionIterator) < 0) __PYX_ERR(0, 1228, __pyx_L1_error)
   __pyx_ptype_7unqlite_CollectionIterator = &__pyx_type_7unqlite_CollectionIterator;
   if (PyType_Ready(&__pyx_type_7unqlite___pyx_scope_struct__commit_on_success) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite___pyx_scope_struct__commit_on_success.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite___pyx_scope_struct__commit_on_success.tp_dictoffset && __pyx_type_7unqlite___pyx_scope_struct__commit_on_success.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite___pyx_scope_struct__commit_on_success.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -28246,15 +28379,15 @@
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite___pyx_scope_struct_4_range.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite___pyx_scope_struct_4_range.tp_dictoffset && __pyx_type_7unqlite___pyx_scope_struct_4_range.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite___pyx_scope_struct_4_range.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_7unqlite___pyx_scope_struct_4_range = &__pyx_type_7unqlite___pyx_scope_struct_4_range;
-  if (PyType_Ready(&__pyx_type_7unqlite___pyx_scope_struct_5_fetch_until) < 0) __PYX_ERR(0, 834, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7unqlite___pyx_scope_struct_5_fetch_until) < 0) __PYX_ERR(0, 837, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7unqlite___pyx_scope_struct_5_fetch_until.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7unqlite___pyx_scope_struct_5_fetch_until.tp_dictoffset && __pyx_type_7unqlite___pyx_scope_struct_5_fetch_until.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7unqlite___pyx_scope_struct_5_fetch_until.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_7unqlite___pyx_scope_struct_5_fetch_until = &__pyx_type_7unqlite___pyx_scope_struct_5_fetch_until;
@@ -28271,22 +28404,21 @@
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
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
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
@@ -28879,15 +29011,15 @@
  */
   __pyx_t_7 = __Pyx_PyInt_From_int(UNQLITE_OPEN_CREATE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_k__3 = __pyx_t_7;
   __Pyx_GIVEREF(__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "unqlite.pyx":717
+  /* "unqlite.pyx":720
  *         unqlite_kv_cursor_reset(self.cursor)
  * 
  *     cpdef seek(self, key, int flags=UNQLITE_CURSOR_MATCH_EXACT):             # <<<<<<<<<<<<<<
  *         """
  *         Seek to the given key. The flags specify how UnQLite will determine
  */
   __pyx_k__10 = UNQLITE_CURSOR_MATCH_EXACT;
@@ -30686,15 +30818,18 @@
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
@@ -31627,18 +31762,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -31684,22 +31819,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
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
@@ -32160,15 +32295,15 @@
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
@@ -32356,15 +32491,15 @@
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
@@ -32590,15 +32725,15 @@
                         } else if (8 * sizeof(sxi64) >= 4 * PyLong_SHIFT) {
                             return (sxi64) (((((((((sxi64)digits[3]) << PyLong_SHIFT) | (sxi64)digits[2]) << PyLong_SHIFT) | (sxi64)digits[1]) << PyLong_SHIFT) | (sxi64)digits[0]));
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
@@ -33862,15 +33997,18 @@
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

### Comparing `unqlite-0.9.5/unqlite.egg-info/PKG-INFO` & `unqlite-0.9.6/unqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unqlite
-Version: 0.9.5
+Version: 0.9.6
 Summary: Fast Python bindings for the UnQLite embedded NoSQL database.
 Home-page: https://github.com/coleifer/unqlite-python
 Author: Charles Leifer
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `unqlite-0.9.5/unqlite.pyx` & `unqlite-0.9.6/unqlite.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -613,16 +613,19 @@
                 bint include_end_key=True):
         cdef Cursor cursor = self.cursor()
         try:
             cursor.seek(start_key)
         except KeyError:
             pass
         else:
-            for item in cursor.fetch_until(end_key, include_end_key):
-                yield item
+            try:
+                for item in cursor.fetch_until(end_key, include_end_key):
+                    yield item
+            except StopIteration:
+                return
 
     def __len__(self):
         """
         Return the total number of records in the database.
 
         Note: this operation is O(n) and requires iterating through the
         entire key-space.
@@ -832,21 +835,21 @@
         return (key, value)
 
     def fetch_until(self, stop_key, bint include_stop_key=True):
         for key, value in self:
             if key == stop_key:
                 if include_stop_key:
                     yield (key, value)
-                raise StopIteration
+                return
             else:
                 yield (key, value)
 
 
 # Foreign function callback signature.
-ctypedef int (*unqlite_filter_fn)(unqlite_context *, int, unqlite_value **)
+ctypedef int (*unqlite_filter_fn)(unqlite_context *, int, unqlite_value **) noexcept
 
 
 cdef class VM(object):
     """Jx9 virtual-machine interface."""
     cdef UnQLite unqlite
     cdef unqlite_vm *vm
     cdef readonly bint need_reset
@@ -1038,15 +1041,15 @@
             unqlite_value_int64(ptr, python_value)
         elif isinstance(python_value, float):
             unqlite_value_double(ptr, python_value)
         else:
             unqlite_value_null(ptr)
 
 
-cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values):
+cdef int py_filter_wrapper(unqlite_context *context, int nargs, unqlite_value **values) noexcept:
     cdef int i
     cdef list converted = []
     cdef object callback = <object>unqlite_context_user_data(context)
     cdef Context context_wrapper = Context()
 
     context_wrapper.set_context(context)
 
@@ -1324,17 +1327,17 @@
     elif isinstance(python_value, (int, long)):
         unqlite_value_int64(ptr, python_value)
     elif isinstance(python_value, float):
         unqlite_value_double(ptr, python_value)
     else:
         unqlite_value_null(ptr)
 
-cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data):
+cdef int unqlite_value_to_list(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
     cdef list accum
     accum = <list>user_data
     accum.append(unqlite_value_to_python(value))
 
-cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data):
+cdef int unqlite_value_to_dict(unqlite_value *key, unqlite_value *value, void *user_data) noexcept:
     cdef dict accum
     accum = <dict>user_data
     pkey = unqlite_value_to_python(key)
     accum[pkey] = unqlite_value_to_python(value)
```

