# Comparing `tmp/tencentcloud-sdk-python-rkp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-rkp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rkp-3.0.937.tar", last modified: Tue Jul 18 00:29:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rkp-3.0.938.tar", last modified: Wed Jul 19 00:44:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rkp-3.0.937.tar` & `tencentcloud-sdk-python-rkp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/rkp_client.py
--rw-r--r--   0 root         (0) root         (0)    21607 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:17.000000 tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3783 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/rkp_client.py
+-rw-r--r--   0 root         (0) root         (0)    21607 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:34.000000 tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/setup.py` & `tencentcloud-sdk-python-rkp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/errorcodes.py` & `tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/rkp_client.py` & `tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/rkp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.GetOpenIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetToken(self, request):
         """获取token接口。
 
         :param request: Request instance for GetToken.
         :type request: :class:`tencentcloud.rkp.v20191209.models.GetTokenRequest`
@@ -65,15 +65,15 @@
             model = models.GetTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryDevAndRisk(self, request):
         """腾讯天御设备风险查询接口，输入由客户应用自主采集的设备信息， 通过腾讯大数据风控能力，可以准确根据输入设备信息，还原设备库中的设备ID，并且识别设备的风险，解决客户业务过程中的设备风险，降低企业损失。
 
         :param request: Request instance for QueryDevAndRisk.
         :type request: :class:`tencentcloud.rkp.v20191209.models.QueryDevAndRiskRequest`
@@ -88,8 +88,8 @@
             model = models.QueryDevAndRiskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/rkp/v20191209/models.py` & `tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/rkp/v20191209/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rkp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-rkp-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rkp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rkp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/README.rst` & `tencentcloud-sdk-python-rkp-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rkp-3.0.937/tencentcloud_sdk_python_rkp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rkp-3.0.938/tencentcloud_sdk_python_rkp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rkp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rkp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

