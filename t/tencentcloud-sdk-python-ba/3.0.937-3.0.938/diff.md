# Comparing `tmp/tencentcloud-sdk-python-ba-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ba-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ba-3.0.937.tar", last modified: Tue Jul 18 00:17:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ba-3.0.938.tar", last modified: Wed Jul 19 00:21:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ba-3.0.937.tar` & `tencentcloud-sdk-python-ba-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3792 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/ba_client.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:17:28.000000 tencentcloud-sdk-python-ba-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/ba_client.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:21:31.000000 tencentcloud-sdk-python-ba-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ba-3.0.937/setup.py` & `tencentcloud-sdk-python-ba-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ba-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ba-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/ba_client.py` & `tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/ba_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateWeappQRUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGetAuthInfo(self, request):
         """获取实名认证信息
 
         :param request: Request instance for DescribeGetAuthInfo.
         :type request: :class:`tencentcloud.ba.v20200720.models.DescribeGetAuthInfoRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeGetAuthInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncIcpOrderWebInfo(self, request):
         """将备案ICP订单下的一个网站信息 同步给订单下其他网站，需要被同步的网站被检查通过(isCheck:true)；
         只有指定的网站信息字段能被同步
 
         :param request: Request instance for SyncIcpOrderWebInfo.
@@ -89,8 +89,8 @@
             model = models.SyncIcpOrderWebInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/errorcodes.py` & `tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ba-3.0.937/tencentcloud/ba/v20200720/models.py` & `tencentcloud-sdk-python-ba-3.0.938/tencentcloud/ba/v20200720/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ba-3.0.937/tencentcloud_sdk_python_ba.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ba-3.0.938/tencentcloud_sdk_python_ba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ba
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ba SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ba-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ba-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ba
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ba SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ba-3.0.937/README.rst` & `tencentcloud-sdk-python-ba-3.0.938/README.rst`

 * *Files identical despite different names*

