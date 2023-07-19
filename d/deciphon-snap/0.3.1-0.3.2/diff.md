# Comparing `tmp/deciphon_snap-0.3.1.tar.gz` & `tmp/deciphon_snap-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.3.1.tar", max compression
+gzip compressed data, was "deciphon_snap-0.3.2.tar", max compression
```

## Comparing `deciphon_snap-0.3.1.tar` & `deciphon_snap-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-06-15 19:44:39.476582 deciphon_snap-0.3.1/LICENSE
--rw-r--r--   0        0        0     2453 2023-06-15 18:49:10.927152 deciphon_snap-0.3.1/README.md
--rw-r--r--   0        0        0      355 2023-06-22 02:55:20.454640 deciphon_snap-0.3.1/deciphon_snap/amino.py
--rw-r--r--   0        0        0     2601 2023-07-13 09:53:40.601153 deciphon_snap-0.3.1/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-06-23 10:26:33.750772 deciphon_snap-0.3.1/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-06-22 02:23:10.535862 deciphon_snap-0.3.1/deciphon_snap/interval.py
--rw-r--r--   0        0        0     2992 2023-07-13 09:53:28.028018 deciphon_snap-0.3.1/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-06-15 18:49:10.774824 deciphon_snap-0.3.1/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     1358 2023-07-13 09:54:16.459105 deciphon_snap-0.3.1/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-06-22 02:40:28.801343 deciphon_snap-0.3.1/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-06-21 16:02:35.925904 deciphon_snap-0.3.1/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-06-21 21:22:12.179074 deciphon_snap-0.3.1/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-06-30 12:44:46.660388 deciphon_snap-0.3.1/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-06-15 18:49:10.775317 deciphon_snap-0.3.1/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-18 22:35:06.368714 deciphon_snap-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/README.md
+-rw-r--r--   0        0        0      355 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2706 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     3054 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1377 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.2/PKG-INFO
```

### Comparing `deciphon_snap-0.3.1/LICENSE` & `deciphon_snap-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/README.md` & `deciphon_snap-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/deciphon_snap/hit.py` & `deciphon_snap-0.3.2/deciphon_snap/hit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List
+from __future__ import annotations
+
+from typing import List, Type, TypeVar
 
 from pydantic import BaseModel, RootModel
 
 from deciphon_snap.match import MatchList, MatchListInterval
 from deciphon_snap.query_interval import QueryInterval
 
 __all__ = ["Hit", "HitList"]
@@ -29,27 +31,30 @@
         return self._match_list
 
     @match_list.setter
     def match_list(self, x: MatchList):
         self._match_list = x
 
     @property
-    def matchs(self):
+    def matches(self):
         assert self._interval is not None
         assert self._match_list is not None
-        matchs = []
+        matches = []
         offset = self._interval.pyinterval.start
         for x in self._match_list[self.match_list_interval.slice]:
             x.position = offset
             if x.state.startswith("I"):
                 offset += len(x.query)
             if x.state.startswith("M"):
                 offset += len(x.query)
-            matchs.append(x)
-        return matchs
+            matches.append(x)
+        return matches
+
+
+T = TypeVar("T", bound="HitList")
 
 
 class HitList(RootModel):
     root: List[Hit]
 
     def __len__(self):
         return len(self.root)
@@ -60,15 +65,15 @@
     def __iter__(self):
         return iter(self.root)
 
     def __str__(self):
         return " ".join(str(i) for i in self.root)
 
     @classmethod
-    def make(cls, match_list: MatchList):
+    def make(cls: Type[T], match_list: MatchList) -> T:
         hits: List[Hit] = []
 
         offset = 0
         hit_start_found = False
         hit_end_found = False
         match_start = 0
         match_stop = 0
```

### Comparing `deciphon_snap-0.3.1/deciphon_snap/hmmer.py` & `deciphon_snap-0.3.2/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/deciphon_snap/interval.py` & `deciphon_snap-0.3.2/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/deciphon_snap/match.py` & `deciphon_snap-0.3.2/deciphon_snap/match.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 
     def __len__(self):
         return len(self.root)
 
     def __getitem__(self, i):
         if isinstance(i, slice):
             return MatchList.model_validate(self.root[i])
-        return self.root[i]
+        match = self.root[i]
+        assert isinstance(match, Match)
+        return match
 
     def __iter__(self):
         return iter(self.root)
 
     def __str__(self):
         return " ".join(str(i) for i in self.root)
```

### Comparing `deciphon_snap-0.3.1/deciphon_snap/prod.py` & `deciphon_snap-0.3.2/deciphon_snap/prod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from pydantic import BaseModel, RootModel
 from typing import List
 
+from pydantic import BaseModel, RootModel
+
+from deciphon_snap.hit import Hit, HitList
 from deciphon_snap.hmmer import H3Result
 from deciphon_snap.match import LazyMatchList
 from deciphon_snap.query_interval import QueryIntervalBuilder
-from deciphon_snap.hit import HitList
 
 __all__ = ["Prod"]
 
 
 class Prod(BaseModel):
     id: int
     seq_id: int
@@ -17,15 +18,15 @@
     alt: float
     null: float
     evalue: float
     match_list: LazyMatchList
     h3result: H3Result | None = None
 
     @property
-    def hits(self):
+    def hits(self) -> list[Hit]:
         qibuilder = QueryIntervalBuilder(self.match_list)
         hits = []
         for hit in HitList.make(self.match_list):
             hit.interval = qibuilder.make(hit.match_list_interval)
             hit.match_list = self.match_list.evaluate()
             hits.append(hit)
         return hits
```

### Comparing `deciphon_snap-0.3.1/deciphon_snap/query_interval.py` & `deciphon_snap-0.3.2/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/deciphon_snap/shorten.py` & `deciphon_snap-0.3.2/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/deciphon_snap/snap_file.py` & `deciphon_snap-0.3.2/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.1/pyproject.toml` & `deciphon_snap-0.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.3.1"
+version = "0.3.2"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphon_snap-0.3.1/PKG-INFO` & `deciphon_snap-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.3.1
+Version: 0.3.2
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

