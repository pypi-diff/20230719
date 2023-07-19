# Comparing `tmp/deciphon_snap-0.3.0.tar.gz` & `tmp/deciphon_snap-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.3.0.tar", max compression
+gzip compressed data, was "deciphon_snap-0.3.1.tar", max compression
```

## Comparing `deciphon_snap-0.3.0.tar` & `deciphon_snap-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/LICENSE
--rw-r--r--   0        0        0     2453 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/README.md
--rw-r--r--   0        0        0      355 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/amino.py
--rw-r--r--   0        0        0     2553 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/interval.py
--rw-r--r--   0        0        0     2980 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     1346 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-15 19:44:39.476582 deciphon_snap-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2453 2023-06-15 18:49:10.927152 deciphon_snap-0.3.1/README.md
+-rw-r--r--   0        0        0      355 2023-06-22 02:55:20.454640 deciphon_snap-0.3.1/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2601 2023-07-13 09:53:40.601153 deciphon_snap-0.3.1/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-06-23 10:26:33.750772 deciphon_snap-0.3.1/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-06-22 02:23:10.535862 deciphon_snap-0.3.1/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     2992 2023-07-13 09:53:28.028018 deciphon_snap-0.3.1/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-06-15 18:49:10.774824 deciphon_snap-0.3.1/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1358 2023-07-13 09:54:16.459105 deciphon_snap-0.3.1/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-06-22 02:40:28.801343 deciphon_snap-0.3.1/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-06-21 16:02:35.925904 deciphon_snap-0.3.1/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-06-21 21:22:12.179074 deciphon_snap-0.3.1/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-06-30 12:44:46.660388 deciphon_snap-0.3.1/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-06-15 18:49:10.775317 deciphon_snap-0.3.1/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-18 22:35:06.368714 deciphon_snap-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.1/PKG-INFO
```

### Comparing `deciphon_snap-0.3.0/LICENSE` & `deciphon_snap-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/README.md` & `deciphon_snap-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/deciphon_snap/hit.py` & `deciphon_snap-0.3.1/deciphon_snap/hit.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,34 @@
     id: int
     match_list_interval: MatchListInterval
     _interval: QueryInterval | None
     _match_list: MatchList | None
 
     @property
     def interval(self):
-        assert self._interval
+        assert self._interval is not None
         return self._interval
 
     @interval.setter
     def interval(self, x: QueryInterval):
         self._interval = x
 
     @property
     def match_list(self):
-        assert self._match_list
+        assert self._match_list is not None
         return self._match_list
 
     @match_list.setter
     def match_list(self, x: MatchList):
         self._match_list = x
 
     @property
     def matchs(self):
-        assert self._interval
-        assert self._match_list
+        assert self._interval is not None
+        assert self._match_list is not None
         matchs = []
         offset = self._interval.pyinterval.start
         for x in self._match_list[self.match_list_interval.slice]:
             x.position = offset
             if x.state.startswith("I"):
                 offset += len(x.query)
             if x.state.startswith("M"):
```

### Comparing `deciphon_snap-0.3.0/deciphon_snap/hmmer.py` & `deciphon_snap-0.3.1/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/deciphon_snap/interval.py` & `deciphon_snap-0.3.1/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/deciphon_snap/match.py` & `deciphon_snap-0.3.1/deciphon_snap/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @classmethod
     def from_string(cls, x: str):
         y = x.split(",", 3)
         return cls(query=y[0], state=y[1], codon=y[2], amino=y[3])
 
     @property
     def position(self):
-        assert self._position
+        assert self._position is not None
         return self._position
 
     @position.setter
     def position(self, x: int):
         self._position = x
 
     def __str__(self):
```

### Comparing `deciphon_snap-0.3.0/deciphon_snap/prod.py` & `deciphon_snap-0.3.1/deciphon_snap/prod.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             hit.interval = qibuilder.make(hit.match_list_interval)
             hit.match_list = self.match_list.evaluate()
             hits.append(hit)
         return hits
 
     @property
     def hmmer(self):
-        assert self.h3result
+        assert self.h3result is not None
         return self.h3result
 
     @property
     def query(self):
         return self.match_list.query
 
     @property
```

### Comparing `deciphon_snap-0.3.0/deciphon_snap/query_interval.py` & `deciphon_snap-0.3.1/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/deciphon_snap/shorten.py` & `deciphon_snap-0.3.1/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/deciphon_snap/snap_file.py` & `deciphon_snap-0.3.1/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.0/pyproject.toml` & `deciphon_snap-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.3.0"
+version = "0.3.1"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
 fsspec = { version = ">=2023.6.0" }
 prettytable = ">=3.8.0"
-pydantic = ">=2.0b3"
+pydantic = ">=2.0.3"
 python = "^3.9"
 h3result = ">=0.3.0"
 hmmer-tables = ">=0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
```

### Comparing `deciphon_snap-0.3.0/PKG-INFO` & `deciphon_snap-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.6.0)
 Requires-Dist: h3result (>=0.3.0)
 Requires-Dist: hmmer-tables (>=0.4.0)
 Requires-Dist: prettytable (>=3.8.0)
-Requires-Dist: pydantic (>=2.0b3)
+Requires-Dist: pydantic (>=2.0.3)
 Description-Content-Type: text/markdown
 
 # deciphon-snap
 
 ## Example
 
 ```python
```

