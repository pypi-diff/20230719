# Comparing `tmp/tencentcloud-sdk-python-af-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-af-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-af-3.0.937.tar", last modified: Tue Jul 18 00:15:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-af-3.0.938.tar", last modified: Wed Jul 19 00:20:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-af-3.0.937.tar` & `tencentcloud-sdk-python-af-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/af_client.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54195 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:15:54.000000 tencentcloud-sdk-python-af-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/af_client.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54195 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:20:12.000000 tencentcloud-sdk-python-af-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-af-3.0.937/setup.py` & `tencentcloud-sdk-python-af-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-af-3.0.937/tencentcloud_sdk_python_af.egg-info/PKG-INFO` & `tencentcloud-sdk-python-af-3.0.938/tencentcloud_sdk_python_af.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-af
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Af SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-af-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-af-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/af_client.py` & `tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/af_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.DescribeAntiFraudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAntiFraud(self, request):
         """反欺诈评分接口
 
         :param request: Request instance for GetAntiFraud.
         :type request: :class:`tencentcloud.af.v20200226.models.GetAntiFraudRequest`
@@ -67,15 +67,15 @@
             model = models.GetAntiFraudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAntiFraud(self, request):
         """天御反欺诈服务，主要应用于银行、证券、保险、消费金融等金融行业客户，通过腾讯的大数据风控能力，
         可以准确识别恶意用户信息，解决客户在支付、活动、理财，风控等业务环节遇到的欺诈威胁，降低企业
         的损失。
 
@@ -92,8 +92,8 @@
             model = models.QueryAntiFraudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/errorcodes.py` & `tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-af-3.0.937/tencentcloud/af/v20200226/models.py` & `tencentcloud-sdk-python-af-3.0.938/tencentcloud/af/v20200226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-af-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-af-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-af
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Af SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-af-3.0.937/README.rst` & `tencentcloud-sdk-python-af-3.0.938/README.rst`

 * *Files identical despite different names*

