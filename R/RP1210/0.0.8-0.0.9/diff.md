# Comparing `tmp/RP1210-0.0.8.tar.gz` & `tmp/RP1210-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RP1210-0.0.8.tar", last modified: Thu Feb 24 02:03:49 2022, max compression
+gzip compressed data, was "RP1210-0.0.9.tar", last modified: Tue Mar  1 16:15:22 2022, max compression
```

## Comparing `RP1210-0.0.8.tar` & `RP1210-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 02:03:49.582810 RP1210-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-02-24 02:03:39.000000 RP1210-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-02-24 02:03:49.582810 RP1210-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-02-24 02:03:39.000000 RP1210-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 02:03:49.582810 RP1210-0.0.8/RP1210/
--rw-r--r--   0 runner    (1001) docker     (121)    14111 2022-02-24 02:03:39.000000 RP1210-0.0.8/RP1210/Commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    19386 2022-02-24 02:03:39.000000 RP1210-0.0.8/RP1210/J1939.py
--rw-r--r--   0 runner    (1001) docker     (121)    60425 2022-02-24 02:03:39.000000 RP1210-0.0.8/RP1210/RP1210.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-02-24 02:03:39.000000 RP1210-0.0.8/RP1210/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 02:03:49.582810 RP1210-0.0.8/RP1210.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-02-24 02:03:49.000000 RP1210-0.0.8/RP1210.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-02-24 02:03:49.000000 RP1210-0.0.8/RP1210.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 02:03:49.000000 RP1210-0.0.8/RP1210.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-24 02:03:49.000000 RP1210-0.0.8/RP1210.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-24 02:03:49.582810 RP1210-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-02-24 02:03:39.000000 RP1210-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 16:15:22.404643 RP1210-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-03-01 16:15:08.000000 RP1210-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-03-01 16:15:22.404643 RP1210-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-03-01 16:15:08.000000 RP1210-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 16:15:22.400643 RP1210-0.0.9/RP1210/
+-rw-r--r--   0 runner    (1001) docker     (121)    14111 2022-03-01 16:15:08.000000 RP1210-0.0.9/RP1210/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19612 2022-03-01 16:15:08.000000 RP1210-0.0.9/RP1210/J1939.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60425 2022-03-01 16:15:08.000000 RP1210-0.0.9/RP1210/RP1210.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-03-01 16:15:08.000000 RP1210-0.0.9/RP1210/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 16:15:22.404643 RP1210-0.0.9/RP1210.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-03-01 16:15:22.000000 RP1210-0.0.9/RP1210.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-01 16:15:22.000000 RP1210-0.0.9/RP1210.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 16:15:22.000000 RP1210-0.0.9/RP1210.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-01 16:15:22.000000 RP1210-0.0.9/RP1210.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-01 16:15:22.404643 RP1210-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-03-01 16:15:08.000000 RP1210-0.0.9/setup.py
```

### Comparing `RP1210-0.0.8/LICENSE` & `RP1210-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RP1210-0.0.8/PKG-INFO` & `RP1210-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RP1210
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python32 implementation of the RP1210C standard.
 Home-page: https://github.com/dfieschko/RP1210
 Author: Darius Fieschko
 Author-email: dfieschko@gmail.com
 License: MIT
 Project-URL: Wiki, https://github.com/dfieschko/RP1210/wiki
 Project-URL: Issues, https://github.com/dfieschko/RP1210/issues
```

### Comparing `RP1210-0.0.8/README.md` & `RP1210-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `RP1210-0.0.8/RP1210/Commands.py` & `RP1210-0.0.9/RP1210/Commands.py`

 * *Files identical despite different names*

### Comparing `RP1210-0.0.8/RP1210/J1939.py` & `RP1210-0.0.9/RP1210/J1939.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,20 +232,25 @@
         """Returns timestamp (4 bytes) as int."""
         return int.from_bytes(self.msg[0:4], 'big')
 
     def getPGN(self) -> int:
         """Returns PGN (3 bytes) as int."""
         start = 4 + self.echo_offset
         end = 6 + self.echo_offset
-        return int.from_bytes(self.msg[start:end+1], 'little')
+        pgn = self.msg[start:(end+1)]
+        pgn_int = int.from_bytes(pgn, 'little')
+        # PDU1 (destination specific) - RP1210 adapters handle this in a dumb way
+        if pgn[1] < 0xF0 and pgn[0] == 0x00:
+            pgn_int += self.getDestination()
+        return pgn_int
 
     def getPriority(self) -> int:
         """Returns Priority (1 byte) as int."""
         loc = 7 + self.echo_offset
-        return int(self.msg[loc])
+        return int(self.msg[loc]) & 0b111
 
     def getSource(self) -> int:
         """Returns Source Address (1 byte) as int."""
         loc = 8 + self.echo_offset
         return int(self.msg[loc])
 
     def getSourceAddress(self) -> int:
```

### Comparing `RP1210-0.0.8/RP1210/RP1210.py` & `RP1210-0.0.9/RP1210/RP1210.py`

 * *Files identical despite different names*

### Comparing `RP1210-0.0.8/RP1210/__init__.py` & `RP1210-0.0.9/RP1210/__init__.py`

 * *Files identical despite different names*

### Comparing `RP1210-0.0.8/RP1210.egg-info/PKG-INFO` & `RP1210-0.0.9/RP1210.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RP1210
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python32 implementation of the RP1210C standard.
 Home-page: https://github.com/dfieschko/RP1210
 Author: Darius Fieschko
 Author-email: dfieschko@gmail.com
 License: MIT
 Project-URL: Wiki, https://github.com/dfieschko/RP1210/wiki
 Project-URL: Issues, https://github.com/dfieschko/RP1210/issues
```

### Comparing `RP1210-0.0.8/setup.cfg` & `RP1210-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = RP1210
-version = 0.0.8
+version = 0.0.9
 keywords = RP1210, CAN, J1939
 author = Darius Fieschko
 author_email = dfieschko@gmail.com
 description = A Python32 implementation of the RP1210C standard.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dfieschko/RP1210
```

### Comparing `RP1210-0.0.8/setup.py` & `RP1210-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name = 'RP1210',
   packages = ['RP1210'],
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'A Python32 implementation of the RP1210C standard.',
   long_description = open('README.md').read(),
   long_description_content_type = 'text/markdown',
   author = 'Darius Fieschko',
   author_email = 'dfieschko@gmail.com',
   url = 'https://github.com/dfieschko/RP1210',
```

