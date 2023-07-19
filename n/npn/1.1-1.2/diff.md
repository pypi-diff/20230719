# Comparing `tmp/npn-1.1.tar.gz` & `tmp/npn-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npn-1.1.tar", last modified: Fri Jul 14 01:21:45 2023, max compression
+gzip compressed data, was "npn-1.2.tar", last modified: Wed Jul 19 01:37:13 2023, max compression
```

## Comparing `npn-1.1.tar` & `npn-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.316379 npn-1.1/
--rw-rw-rw-   0        0        0      325 2023-07-14 01:21:45.316379 npn-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2023-07-13 12:16:12.000000 npn-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.312379 npn-1.1/npn/
--rw-rw-rw-   0        0        0      179 2023-07-13 18:02:13.000000 npn-1.1/npn/__init__.py
--rw-rw-rw-   0        0        0     4471 2023-07-14 01:20:34.000000 npn-1.1/npn/api.py
--rw-rw-rw-   0        0        0    16728 2023-07-14 00:26:42.000000 npn-1.1/npn/libnpn.so
--rw-rw-rw-   0        0        0    13312 2023-07-13 19:51:46.000000 npn-1.1/npn/npn.dll
-drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.315379 npn-1.1/npn.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 01:21:45.316379 npn-1.1/setup.cfg
--rw-rw-rw-   0        0        0      458 2023-07-14 01:21:36.000000 npn-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:37:13.208622 npn-1.2/
+-rw-rw-rw-   0        0        0      325 2023-07-19 01:37:13.208622 npn-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2441 2023-07-14 01:38:34.000000 npn-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 01:37:13.204655 npn-1.2/npn/
+-rw-rw-rw-   0        0        0      197 2023-07-16 23:15:51.000000 npn-1.2/npn/__init__.py
+-rw-rw-rw-   0        0        0     4826 2023-07-16 23:14:55.000000 npn-1.2/npn/api.py
+-rw-rw-rw-   0        0        0    16728 2023-07-14 00:26:42.000000 npn-1.2/npn/libnpn.so
+-rw-rw-rw-   0        0        0    13312 2023-07-13 19:51:46.000000 npn-1.2/npn/npn.dll
+drwxrwxrwx   0        0        0        0 2023-07-19 01:37:13.207621 npn-1.2/npn.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-07-19 01:37:13.000000 npn-1.2/npn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-19 01:37:13.000000 npn-1.2/npn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:37:13.000000 npn-1.2/npn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-19 01:37:13.000000 npn-1.2/npn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:37:13.208622 npn-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      458 2023-07-19 01:36:47.000000 npn-1.2/setup.py
```

### Comparing `npn-1.1/npn/api.py` & `npn-1.2/npn/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,19 +75,19 @@
         return r
 
 
 def transform_tt(tt, phase, perm, output_inv):
     res = [False] * len(tt)
     num_inputs = base_2_log(len(tt))
     for i, value in enumerate(itertools.product([False, True], repeat=num_inputs)):   # value = (x_2, x_1, x_0)
-        value = list(reversed(value))       # value = (x_0, x_1, x_2) so that x_i can be accessed by index i
+        value = list(reversed(value))       # reverse `value` to (x_0, x_1, x_2) so that x_i can be accessed by index i
         value_new = [0] * num_inputs
         for j in range(num_inputs):
             value_new[j] = value[perm[j]]   # permutate first, then change the phase of the input
-            if phase[j]:                    # x_i -> not(x_i)
+            if phase[j]:                    # x_i -> not(x_i), note that `phase` is already reversed
                 value_new[j] = not value_new[j]
         id = 0
         for j in range(num_inputs):
             if value_new[j]:
                 id += 2 ** j
         res[i] = not(tt[id]) if output_inv else tt[id]
     return res
@@ -98,14 +98,26 @@
     res = 0
     for i, b in enumerate(tt):
         if b:
             res += 2 ** (tt_size - 1 - i)
     return res
 
 
+def int_to_tt(n, num_inputs=None):
+    if num_inputs is None:
+        num_inputs = base_2_log(base_2_log(n + 1))
+    tt = [False] * (2 ** num_inputs)
+    for i in reversed(range(2 ** num_inputs)):
+        tt[i] = n % 2 == 1
+        n >>= 1
+        if n == 0:
+            break
+    return tt
+
+
 # num_inputs = 2
 # generate_permutation_table(num_inputs)
 # # p = [0] * num_inputs
 # # p_ctypes = (ctypes.c_uint8 * len(p))(*p)
 # tt = [False, True, False, True]
 # # tt = [False, False, False, True, False, False, False, False]
 # # tt = [True, True, True, False, True, True, True, True]  # f(x_2, x_1, x_0) = x_2 + not(x_1) + not(x_0)
```

### Comparing `npn-1.1/npn/libnpn.so` & `npn-1.2/npn/libnpn.so`

 * *Files identical despite different names*

### Comparing `npn-1.1/npn/npn.dll` & `npn-1.2/npn/npn.dll`

 * *Files identical despite different names*

