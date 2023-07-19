# Comparing `tmp/geohashr-1.0.0.tar.gz` & `tmp/geohashr-1.1.0.tar.gz`

## Comparing `geohashr-1.0.0.tar` & `geohashr-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 geohashr-1.0.0/Cargo.toml
--rw-r--r--   0     1001      123     1500 2023-07-13 09:55:02.000000 geohashr-1.0.0/LICENSE
--rw-r--r--   0     1001      123      778 2023-07-13 09:55:02.000000 geohashr-1.0.0/README.md
--rw-r--r--   0     1001      123       54 2023-07-13 09:55:02.000000 geohashr-1.0.0/build.rs
--rw-r--r--   0     1001      123      157 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/__init__.py
--rw-r--r--   0     1001      123       22 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/__version__.py
--rw-r--r--   0     1001      123      654 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/_geohashr.pyi
--rw-r--r--   0     1001      123        0 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/py.typed
--rw-r--r--   0     1001      123     1420 2023-07-13 09:55:02.000000 geohashr-1.0.0/pyproject.toml
--rw-r--r--   0     1001      123     4751 2023-07-13 09:55:02.000000 geohashr-1.0.0/src/lib.rs
--rw-r--r--   0     1001      123      786 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_bbox.py
--rw-r--r--   0     1001      123     1463 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_decode.py
--rw-r--r--   0     1001      123      203 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_encode.py
--rw-r--r--   0     1001      123     1338 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_neighbors.py
--rw-r--r--   0     1001      123    10216 2023-07-13 09:55:02.000000 geohashr-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 geohashr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 geohashr-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      123     1500 2023-07-19 10:37:10.000000 geohashr-1.1.0/LICENSE
+-rw-r--r--   0     1001      123      892 2023-07-19 10:37:10.000000 geohashr-1.1.0/README.md
+-rw-r--r--   0     1001      123       54 2023-07-19 10:37:10.000000 geohashr-1.1.0/build.rs
+-rw-r--r--   0     1001      123      157 2023-07-19 10:37:10.000000 geohashr-1.1.0/geohashr/__init__.py
+-rw-r--r--   0     1001      123       22 2023-07-19 10:37:10.000000 geohashr-1.1.0/geohashr/__version__.py
+-rw-r--r--   0     1001      123      654 2023-07-19 10:37:10.000000 geohashr-1.1.0/geohashr/_geohashr.pyi
+-rw-r--r--   0     1001      123        0 2023-07-19 10:37:10.000000 geohashr-1.1.0/geohashr/py.typed
+-rw-r--r--   0     1001      123     1420 2023-07-19 10:37:10.000000 geohashr-1.1.0/pyproject.toml
+-rw-r--r--   0     1001      123     4743 2023-07-19 10:37:10.000000 geohashr-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      123      786 2023-07-19 10:37:10.000000 geohashr-1.1.0/tests/test_bbox.py
+-rw-r--r--   0     1001      123     1596 2023-07-19 10:37:10.000000 geohashr-1.1.0/tests/test_decode.py
+-rw-r--r--   0     1001      123      286 2023-07-19 10:37:10.000000 geohashr-1.1.0/tests/test_encode.py
+-rw-r--r--   0     1001      123     1338 2023-07-19 10:37:10.000000 geohashr-1.1.0/tests/test_neighbors.py
+-rw-r--r--   0     1001      123    10216 2023-07-19 10:37:10.000000 geohashr-1.1.0/Cargo.lock
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 geohashr-1.1.0/PKG-INFO
```

### Comparing `geohashr-1.0.0/Cargo.toml` & `geohashr-1.1.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "geohashr"
-version = "1.0.0"
+version = "1.1.0"
 description = "Just another geohashing library"
 authors = [
     "Giovanni Barillari <g@baro.dev>",
     "Paolo Quadri <pquadri10@gmail.com>"
 ]
 license = "BSD-3-Clause"
 edition = "2021"
```

### Comparing `geohashr-1.0.0/LICENSE` & `geohashr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geohashr-1.0.0/geohashr/_geohashr.pyi` & `geohashr-1.1.0/geohashr/_geohashr.pyi`

 * *Files identical despite different names*

### Comparing `geohashr-1.0.0/pyproject.toml` & `geohashr-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geohashr-1.0.0/src/lib.rs` & `geohashr-1.1.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 use std::collections::HashMap;
 
 use geohash::{self, Direction};
 use lazy_static::lazy_static;
 use pyo3::{
     create_exception,
-    exceptions::{PyValueError, PySyntaxError},
+    exceptions::{PySyntaxError, PyValueError},
     prelude::*,
     types::PyDict,
 };
 
 create_exception!(_geohashr, DecodeError, PyValueError, "Geohash decode error");
 create_exception!(_geohashr, EncodeError, PyValueError, "Geohash encode error");
 create_exception!(_geohashr, ParamError, PySyntaxError, "Geohash parameter error");
@@ -19,47 +19,47 @@
 enum NeighborError {
     Hash(geohash::GeohashError),
     Direction
 }
 
 lazy_static! {
     static ref DIRECTION_MAP: HashMap<&'static str, Direction> = HashMap::from([
-        ("sw",  Direction::SW),
-        ("s",  Direction::S),
-        ("se",  Direction::SE),
-        ("w",  Direction::W),
-        ("e",  Direction::E),
-        ("nw",  Direction::NW),
-        ("n",  Direction::N),
-        ("ne",  Direction::NE)
+        ("sw", Direction::SW),
+        ("s", Direction::S),
+        ("se", Direction::SE),
+        ("w", Direction::W),
+        ("e", Direction::E),
+        ("nw", Direction::NW),
+        ("n", Direction::N),
+        ("ne", Direction::NE)
     ]);
 }
 
 #[pyfunction]
 #[pyo3(signature = (hash))]
 fn decode(py: Python, hash: &str) -> PyResult<(f64, f64)> {
     match py.allow_threads(|| geohash::decode(hash)) {
-        Ok((coords, _, _)) => Ok((coords.x, coords.y)),
+        Ok((coords, _, _)) => Ok((coords.y, coords.x)),
         Err(err) => Err(DecodeError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (hash))]
 fn decode_exact(py: Python, hash: &str) -> PyResult<(f64, f64, f64, f64)> {
     match py.allow_threads(|| geohash::decode(hash)) {
-        Ok((coords, dx, dy)) => Ok((coords.x, coords.y, dx, dy)),
+        Ok((coords, dx, dy)) => Ok((coords.y, coords.x, dy, dx)),
         Err(err) => Err(DecodeError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (lat, lon, len=12))]
 fn encode(py: Python, lat: f64, lon: f64, len: usize) -> PyResult<String> {
-    match py.allow_threads(|| geohash::encode(geohash::Coord { x: lat, y: lon }, len)) {
+    match py.allow_threads(|| geohash::encode(geohash::Coord { x: lon, y: lat }, len)) {
         Ok(hash) => Ok(hash),
         Err(err) => Err(EncodeError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (hash))]
@@ -71,15 +71,15 @@
         Ok((min, max)) => {
             let dict = PyDict::new(py);
             dict.set_item(pyo3::intern!(py, "e"), max.x)?;
             dict.set_item(pyo3::intern!(py, "s"), min.y)?;
             dict.set_item(pyo3::intern!(py, "w"), min.x)?;
             dict.set_item(pyo3::intern!(py, "n"), max.y)?;
             Ok(dict)
-        },
+        }
         Err(err) => Err(EncodeError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (hash))]
 fn neighbors<'p>(py: Python<'p>, hash: &str) -> PyResult<&'p PyDict> {
@@ -108,15 +108,15 @@
             geohash::neighbor(hash, *dir).map_err(|e| NeighborError::Hash(e))
         } else {
             Err(NeighborError::Direction)
         }
     }) {
         Ok(hash) => Ok(hash),
         Err(NeighborError::Hash(err)) => Err(EncodeError::new_err(err.to_string())),
-        Err(NeighborError::Direction) => Err(ParamError::new_err("Invalid direction"))
+        Err(NeighborError::Direction) => Err(ParamError::new_err("Invalid direction")),
     }
 }
 
 #[pymodule]
 fn _geohashr(py: Python, module: &PyModule) -> PyResult<()> {
     module.add_function(wrap_pyfunction!(decode, module)?)?;
     module.add_function(wrap_pyfunction!(decode_exact, module)?)?;
```

### Comparing `geohashr-1.0.0/tests/test_bbox.py` & `geohashr-1.1.0/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `geohashr-1.0.0/tests/test_decode.py` & `geohashr-1.1.0/tests/test_decode.py`

 * *Files 23% similar despite different names*

```diff
@@ -48,7 +48,12 @@
 )
 def test_hash_segment(params):
     segment, target = params
     ret = bbox(segment)
     assert (ret['s'], ret['w']) == target
     assert ret['n'] - ret['s'] == 45
     assert ret['e'] - ret['w'] == 45
+
+
+def test_simple_decode(): 
+    lat, lon =  decode('u4pruydqqvj8')
+    assert (57.64911,10.40744) == (round(lat, 6), round(lon, 6))
```

### Comparing `geohashr-1.0.0/tests/test_neighbors.py` & `geohashr-1.1.0/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `geohashr-1.0.0/Cargo.lock` & `geohashr-1.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 dependencies = [
  "geo-types",
  "libm",
 ]
 
 [[package]]
 name = "geohashr"
-version = "1.0.0"
+version = "1.1.0"
 dependencies = [
  "geohash",
  "lazy_static",
  "mimalloc",
  "pyo3",
  "pyo3-build-config",
 ]
```

### Comparing `geohashr-1.0.0/PKG-INFO` & `geohashr-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohashr
-Version: 1.0.0
+Version: 1.1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -38,40 +38,43 @@
 
 ## In a nutshell
 
 ```python
 import geohashr
 
 geohashr.encode(45.464664, 9.188540)
-# 't18k68dr5kn8'
+# 'u0nd9hdfue8h'
 
-geohashr.decode('t18k68dr5kn8')
-# (45.46466404572129, 9.188540065661073)
+geohashr.decode('u0nd9hdfue8h')
+# (45.46466396190226, 9.188540149480104)
 
-geohashr.bbox('t18k68dr5kn8')
+geohashr.decode_exact('u0nd9hd')
+# (45.46485900878906, 9.188003540039062, 0.0006866455078125, 0.0006866455078125)
+
+geohashr.bbox('u0nd9hdfue8h')
 # {
-#     'e': 45.464664213359356, 
-#     's': 9.188539981842041, 
-#     'w': 45.46466387808323, 
-#     'n': 9.188540149480104
+#     'e': 9.188540317118168, 
+#     's': 45.46466387808323, 
+#     'w': 9.188539981842041, 
+#     'n': 45.46466404572129
 # }
 
-geohashr.neighbors('t18k68dr5kn8')
+geohashr.neighbors('u0nd9hdfue8h')
 # {
-#     'e': 't18k68dr5knb', 
-#     'n': 't18k68dr5kn9', 
-#     'ne': 't18k68dr5knc', 
-#     'nw': 't18k68dr5kn3', 
-#     's': 't18k68dr57yx', 
-#     'se': 't18k68dr57yz', 
-#     'sw': 't18k68dr57yr', 
-#     'w': 't18k68dr5kn2'
+#     'e': 'u0nd9hdfue8k', 
+#     'n': 'u0nd9hdfue8j', 
+#     'ne': 'u0nd9hdfue8m', 
+#     'nw': 'u0nd9hdfu7xv', 
+#     's': 'u0nd9hdfue85', 
+#     'se': 'u0nd9hdfue87', 
+#     'sw': 'u0nd9hdfu7xg', 
+#     'w': 'u0nd9hdfu7xu'
 # }
 
-geohashr.neighbor('t18k68dr5kn8', 'e')
-# 't18k68dr5knb'
+geohashr.neighbor('u0nd9hdfue8h', 'e')
+# 'u0nd9hdfue8k'
 ```
 
 ## License
 
 Geohashr is released under the BSD License.
```

