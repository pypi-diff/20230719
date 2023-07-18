# Comparing `tmp/universal_pathlib-0.0.8.tar.gz` & `tmp/universal_pathlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_pathlib-0.0.8.tar", last modified: Tue May 11 16:00:54 2021, max compression
+gzip compressed data, was "universal_pathlib-0.0.9.tar", last modified: Wed May 12 16:34:52 2021, max compression
```

## Comparing `universal_pathlib-0.0.8.tar` & `universal_pathlib-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      195 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/.flake8
--rw-r--r--   0        0        0     1006 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/.github/workflows/python.yml
--rw-r--r--   0        0        0       38 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/.gitignore
--rw-r--r--   0        0        0     1065 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/LICENSE
--rw-r--r--   0        0        0      843 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/README.md
--rw-r--r--   0        0        0      308 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/environment.yml
--rw-r--r--   0        0        0    12505 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/notebooks/examples.ipynb
--rw-r--r--   0        0        0      962 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/noxfile.py
--rw-r--r--   0        0        0      859 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      540 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/setup.py
--rw-r--r--   0        0        0      102 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/__init__.py
--rw-r--r--   0        0        0     1535 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/core.py
--rw-r--r--   0        0        0       45 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/errors.py
--rw-r--r--   0        0        0        0 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/implementations/__init__.py
--rw-r--r--   0        0        0      893 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/implementations/hdfs.py
--rw-r--r--   0        0        0     1189 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/implementations/http.py
--rw-r--r--   0        0        0     1228 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/implementations/memory.py
--rw-r--r--   0        0        0      711 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/implementations/s3.py
--rw-r--r--   0        0        0      742 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/registry.py
--rw-r--r--   0        0        0        0 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/__init__.py
--rw-r--r--   0        0        0     6174 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/cases.py
--rw-r--r--   0        0        0     4796 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/implementations/__init__.py
--rw-r--r--   0        0        0      635 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/implementations/test_hdfs.py
--rw-r--r--   0        0        0      226 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/implementations/test_http.py
--rw-r--r--   0        0        0      897 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/implementations/test_memory.py
--rw-r--r--   0        0        0     2638 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/implementations/test_s3.py
--rw-r--r--   0        0        0     1476 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/tests/test_core.py
--rw-r--r--   0        0        0     8582 2021-05-11 16:00:39.697418 universal_pathlib-0.0.8/upath/universal_path.py
--rw-r--r--   0        0        0      232 1970-01-01 00:00:00.000000 universal_pathlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      195 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.flake8
+-rw-r--r--   0        0        0     1006 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.github/workflows/python.yml
+-rw-r--r--   0        0        0       38 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1065 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/LICENSE
+-rw-r--r--   0        0        0      843 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/README.md
+-rw-r--r--   0        0        0      308 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/environment.yml
+-rw-r--r--   0        0        0    12505 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/notebooks/examples.ipynb
+-rw-r--r--   0        0        0      962 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/noxfile.py
+-rw-r--r--   0        0        0      859 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      540 2021-05-12 16:34:37.748629 universal_pathlib-0.0.9/setup.py
+-rw-r--r--   0        0        0      102 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/__init__.py
+-rw-r--r--   0        0        0     1535 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/core.py
+-rw-r--r--   0        0        0       45 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/errors.py
+-rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/__init__.py
+-rw-r--r--   0        0        0      893 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/hdfs.py
+-rw-r--r--   0        0        0     1189 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/http.py
+-rw-r--r--   0        0        0     1228 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/memory.py
+-rw-r--r--   0        0        0      734 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/implementations/s3.py
+-rw-r--r--   0        0        0      742 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/registry.py
+-rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/__init__.py
+-rw-r--r--   0        0        0     6263 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/cases.py
+-rw-r--r--   0        0        0     4796 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/conftest.py
+-rw-r--r--   0        0        0        0 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/__init__.py
+-rw-r--r--   0        0        0      635 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_hdfs.py
+-rw-r--r--   0        0        0      226 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_http.py
+-rw-r--r--   0        0        0      897 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_memory.py
+-rw-r--r--   0        0        0     2638 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/implementations/test_s3.py
+-rw-r--r--   0        0        0     1476 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/tests/test_core.py
+-rw-r--r--   0        0        0     8582 2021-05-12 16:34:37.752629 universal_pathlib-0.0.9/upath/universal_path.py
+-rw-r--r--   0        0        0      232 1970-01-01 00:00:00.000000 universal_pathlib-0.0.9/PKG-INFO
```

### Comparing `universal_pathlib-0.0.8/.github/workflows/python.yml` & `universal_pathlib-0.0.9/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/LICENSE` & `universal_pathlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/README.md` & `universal_pathlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/notebooks/examples.ipynb` & `universal_pathlib-0.0.9/notebooks/examples.ipynb`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/noxfile.py` & `universal_pathlib-0.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/pyproject.toml` & `universal_pathlib-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/setup.py` & `universal_pathlib-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/core.py` & `universal_pathlib-0.0.9/upath/core.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/implementations/hdfs.py` & `universal_pathlib-0.0.9/upath/implementations/hdfs.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/implementations/http.py` & `universal_pathlib-0.0.9/upath/implementations/http.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/implementations/memory.py` & `universal_pathlib-0.0.9/upath/implementations/memory.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/implementations/s3.py` & `universal_pathlib-0.0.9/upath/implementations/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 
     def _sub_path(self, name):
         """s3fs returns path as `{bucket}/<path>` with listdir
         and glob, so here we can add the netloc to the sub string
         so it gets subbed out as well
         """
         sp = self.path
-        return re.sub(f"^{self._url.netloc}/({sp}|{sp[1:]})/", "", name)
+        subed = re.sub(f"^{self._url.netloc}/({sp}|{sp[1:]})/?", "", name)
+        return subed
```

### Comparing `universal_pathlib-0.0.8/upath/registry.py` & `universal_pathlib-0.0.9/upath/registry.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/tests/cases.py` & `universal_pathlib-0.0.9/upath/tests/cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         with pytest.raises(NotImplementedError):
             self.path.joinpath("file1.txt").chmod(777)
 
     @pytest.mark.parametrize(
         "url, expected", [("file1.txt", True), ("fakefile.txt", False)]
     )
     def test_exists(self, url, expected):
-        print(self.path)
         path = self.path.joinpath(url)
         assert path.exists() == expected
 
     def test_expanduser(self):
         with pytest.raises(NotImplementedError):
             self.path.expanduser()
 
@@ -88,17 +87,21 @@
 
     def test_iterdir(self, local_testdir):
         pl_path = Path(local_testdir)
 
         up_iter = list(self.path.iterdir())
         pl_iter = list(pl_path.iterdir())
 
+        for x in up_iter:
+            assert x.exists()
+
         assert len(up_iter) == len(pl_iter)
         pnames = [p.name for p in pl_iter]
         assert all(map(lambda x: x.name in pnames, up_iter))
+        assert next(self.path.parent.iterdir()).exists()
 
     def test_lchmod(self):
         with pytest.raises(NotImplementedError):
             self.path.lchmod(mode=77)
 
     def test_lstat(self):
         with pytest.raises(NotImplementedError):
```

### Comparing `universal_pathlib-0.0.8/upath/tests/conftest.py` & `universal_pathlib-0.0.9/upath/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/tests/implementations/test_hdfs.py` & `universal_pathlib-0.0.9/upath/tests/implementations/test_hdfs.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/tests/implementations/test_memory.py` & `universal_pathlib-0.0.9/upath/tests/implementations/test_memory.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/tests/implementations/test_s3.py` & `universal_pathlib-0.0.9/upath/tests/implementations/test_s3.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/tests/test_core.py` & `universal_pathlib-0.0.9/upath/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.0.8/upath/universal_path.py` & `universal_pathlib-0.0.9/upath/universal_path.py`

 * *Files identical despite different names*

