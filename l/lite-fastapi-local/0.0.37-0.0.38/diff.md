# Comparing `tmp/lite_fastapi_local-0.0.37.tar.gz` & `tmp/lite_fastapi_local-0.0.38.tar.gz`

## Comparing `lite_fastapi_local-0.0.37.tar` & `lite_fastapi_local-0.0.38.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/ledModel.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/ledModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.38/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
 @app.get('/QR_CHK/{scan_in}')   #int 자료형 차후 Modeling
 def QR_CHK(scan_in):
     print(scan_in)
 
     result = json.loads(CHKF.QR_CHK(scan_in=scan_in))
     return result
 
+@app.get('/test/test')   #int 자료형 차후 Modeling
+def QR_test():
+    print("test")
+    return "test"
+
 @app.get('/QR_END', response_class=PlainTextResponse)   #QR_READ 종료
 def QR_END():
     print(os.getcwd())
     subprocess.run(args=[sys.executable,'QR_END_dep.py'], capture_output=True, text=True)        
     return 'QR_END'
 
 @app.get('/update')
```

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.38/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/LICENSE` & `lite_fastapi_local-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.37/pyproject.toml` & `lite_fastapi_local-0.0.38/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.37"
+version = "0.0.38"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.37/PKG-INFO` & `lite_fastapi_local-0.0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.37
+Version: 0.0.38
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

