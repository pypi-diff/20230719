# Comparing `tmp/tencentcloud-sdk-python-sts-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-sts-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sts-3.0.937.tar", last modified: Tue Jul 18 00:30:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sts-3.0.938.tar", last modified: Wed Jul 19 00:47:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sts-3.0.937.tar` & `tencentcloud-sdk-python-sts-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3086 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7300 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/sts_client.py
--rw-r--r--   0 root         (0) root         (0)    28050 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:35.000000 tencentcloud-sdk-python-sts-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/sts_client.py
+-rw-r--r--   0 root         (0) root         (0)    28050 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:47:57.000000 tencentcloud-sdk-python-sts-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-sts-3.0.937/setup.py` & `tencentcloud-sdk-python-sts-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sts-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sts-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/errorcodes.py` & `tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/sts_client.py` & `tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/sts_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AssumeRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssumeRoleWithSAML(self, request):
         """本接口（AssumeRoleWithSAML）用于根据 SAML 断言申请角色临时访问凭证。
 
         注意：当使用签名方法 V3 调用本接口时，请求头无须传入 X-TC-Token, 但 Authorization 需要传入值 SKIP。
 
@@ -67,15 +67,15 @@
             model = models.AssumeRoleWithSAMLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssumeRoleWithWebIdentity(self, request):
         """申请OIDC角色临时访问凭证。
 
         注意：当使用签名方法 V3 调用本接口时，请求头无须传入 X-TC-Token, 但 Authorization 需要传入值 SKIP。
 
@@ -92,15 +92,15 @@
             model = models.AssumeRoleWithWebIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCallerIdentity(self, request):
         """获取当前调用者的身份信息。
 
         接口支持主账号，子账号长期密钥以及AssumeRole，GetFederationToken生成的临时访问凭证身份获取。
 
@@ -117,15 +117,15 @@
             model = models.GetCallerIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFederationToken(self, request):
         """**使用说明**
 
         返回一组临时访问凭证，典型的应用场景是代理应用程序集中申请临时访问凭证，下发给企业网络内其他分布式终端应用，比如终端应用上传文件到COS场景，本接口仅支持永久密钥调用。
 
@@ -148,15 +148,15 @@
             model = models.GetFederationTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryApiKey(self, request):
         """拉取API密钥列表
 
         :param request: Request instance for QueryApiKey.
         :type request: :class:`tencentcloud.sts.v20180813.models.QueryApiKeyRequest`
@@ -171,8 +171,8 @@
             model = models.QueryApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-sts-3.0.937/tencentcloud/sts/v20180813/models.py` & `tencentcloud-sdk-python-sts-3.0.938/tencentcloud/sts/v20180813/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sts-3.0.937/tencentcloud_sdk_python_sts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sts-3.0.938/tencentcloud_sdk_python_sts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sts-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-sts-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sts-3.0.937/README.rst` & `tencentcloud-sdk-python-sts-3.0.938/README.rst`

 * *Files identical despite different names*

