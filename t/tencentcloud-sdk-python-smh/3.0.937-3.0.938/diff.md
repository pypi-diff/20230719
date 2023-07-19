# Comparing `tmp/tencentcloud-sdk-python-smh-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-smh-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-smh-3.0.937.tar", last modified: Tue Jul 18 00:29:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-smh-3.0.938.tar", last modified: Wed Jul 19 00:44:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-smh-3.0.937.tar` & `tencentcloud-sdk-python-smh-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9872 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/smh_client.py
--rw-r--r--   0 root         (0) root         (0)    55893 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:41.000000 tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/smh_client.py
+-rw-r--r--   0 root         (0) root         (0)    55893 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:56.000000 tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-smh-3.0.937/setup.py` & `tencentcloud-sdk-python-smh-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/errorcodes.py` & `tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/smh_client.py` & `tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/smh_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLibrary(self, request):
         """删除 PaaS 服务媒体库
 
         :param request: Request instance for DeleteLibrary.
         :type request: :class:`tencentcloud.smh.v20210712.models.DeleteLibraryRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLibraries(self, request):
         """查询 PaaS 服务媒体库列表
 
         :param request: Request instance for DescribeLibraries.
         :type request: :class:`tencentcloud.smh.v20210712.models.DescribeLibrariesRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeLibrariesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLibrarySecret(self, request):
         """查询 PaaS 服务媒体库密钥
 
         :param request: Request instance for DescribeLibrarySecret.
         :type request: :class:`tencentcloud.smh.v20210712.models.DescribeLibrarySecretRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeLibrarySecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfficialInstances(self, request):
         """查询官方云盘实例
 
         :param request: Request instance for DescribeOfficialInstances.
         :type request: :class:`tencentcloud.smh.v20210712.models.DescribeOfficialInstancesRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeOfficialInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfficialOverview(self, request):
         """查询官方云盘实例概览数据
 
         :param request: Request instance for DescribeOfficialOverview.
         :type request: :class:`tencentcloud.smh.v20210712.models.DescribeOfficialOverviewRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeOfficialOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficPackages(self, request):
         """查询流量资源包
 
         :param request: Request instance for DescribeTrafficPackages.
         :type request: :class:`tencentcloud.smh.v20210712.models.DescribeTrafficPackagesRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLibrary(self, request):
         """修改 PaaS 服务媒体库配置项
 
         :param request: Request instance for ModifyLibrary.
         :type request: :class:`tencentcloud.smh.v20210712.models.ModifyLibraryRequest`
@@ -203,15 +203,15 @@
             model = models.ModifyLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSmsCode(self, request):
         """发送用于换绑官方云盘实例的超级管理员账号的短信验证码
 
         :param request: Request instance for SendSmsCode.
         :type request: :class:`tencentcloud.smh.v20210712.models.SendSmsCodeRequest`
@@ -226,15 +226,15 @@
             model = models.SendSmsCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifySmsCode(self, request):
         """验证短信验证码以换绑官方云盘实例的超级管理员账号
 
         :param request: Request instance for VerifySmsCode.
         :type request: :class:`tencentcloud.smh.v20210712.models.VerifySmsCodeRequest`
@@ -249,8 +249,8 @@
             model = models.VerifySmsCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-smh-3.0.937/tencentcloud/smh/v20210712/models.py` & `tencentcloud-sdk-python-smh-3.0.938/tencentcloud/smh/v20210712/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-smh-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-smh-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-smh-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smh
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Smh SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-smh-3.0.937/README.rst` & `tencentcloud-sdk-python-smh-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.937/tencentcloud_sdk_python_smh.egg-info/PKG-INFO` & `tencentcloud-sdk-python-smh-3.0.938/tencentcloud_sdk_python_smh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smh
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Smh SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

