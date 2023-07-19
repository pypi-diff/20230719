# Comparing `tmp/tencentcloud-sdk-python-smpn-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-smpn-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-smpn-3.0.937.tar", last modified: Tue Jul 18 00:29:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-smpn-3.0.938.tar", last modified: Wed Jul 19 00:45:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-smpn-3.0.937.tar` & `tencentcloud-sdk-python-smpn-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24181 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/models.py
--rw-r--r--   0 root         (0) root         (0)     5294 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/smpn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:48.000000 tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24181 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/models.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/smpn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:45:04.000000 tencentcloud-sdk-python-smpn-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:05.000000 tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/setup.py` & `tencentcloud-sdk-python-smpn-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/errorcodes.py` & `tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/models.py` & `tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/smpn/v20190822/smpn_client.py` & `tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/smpn/v20190822/smpn_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateSmpnEpaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmpnChp(self, request):
         """查询号码的标记和标记次数
 
         :param request: Request instance for DescribeSmpnChp.
         :type request: :class:`tencentcloud.smpn.v20190822.models.DescribeSmpnChpRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeSmpnChpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmpnFnr(self, request):
         """虚假号码识别
 
         :param request: Request instance for DescribeSmpnFnr.
         :type request: :class:`tencentcloud.smpn.v20190822.models.DescribeSmpnFnrRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeSmpnFnrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmpnMhm(self, request):
         """号码营销监控
 
         :param request: Request instance for DescribeSmpnMhm.
         :type request: :class:`tencentcloud.smpn.v20190822.models.DescribeSmpnMhmRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeSmpnMhmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmpnMrl(self, request):
         """查询号码恶意标记等级
 
         :param request: Request instance for DescribeSmpnMrl.
         :type request: :class:`tencentcloud.smpn.v20190822.models.DescribeSmpnMrlRequest`
@@ -134,8 +134,8 @@
             model = models.DescribeSmpnMrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-smpn-3.0.938/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.937'
+__version__ = '3.0.938'
```

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-smpn-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smpn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Smpn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/README.rst` & `tencentcloud-sdk-python-smpn-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smpn-3.0.937/tencentcloud_sdk_python_smpn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-smpn-3.0.938/tencentcloud_sdk_python_smpn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smpn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Smpn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

