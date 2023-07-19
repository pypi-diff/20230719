# Comparing `tmp/tencentcloud-sdk-python-drm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-drm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-drm-3.0.937.tar", last modified: Tue Jul 18 00:22:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-drm-3.0.938.tar", last modified: Wed Jul 19 00:38:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-drm-3.0.937.tar` & `tencentcloud-sdk-python-drm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45281 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/models.py
--rw-r--r--   0 root         (0) root         (0)     9908 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/drm_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:50.000000 tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    45281 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/models.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/drm_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:03.000000 tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-drm-3.0.937/setup.py` & `tencentcloud-sdk-python-drm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-drm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-drm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/errorcodes.py` & `tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/models.py` & `tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-drm-3.0.937/tencentcloud/drm/v20181115/drm_client.py` & `tencentcloud-sdk-python-drm-3.0.938/tencentcloud/drm/v20181115/drm_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.AddFairPlayPemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEncryptKeys(self, request):
         """该接口用来设置加密的密钥。注意，同一个content id，只能设置一次！
 
         :param request: Request instance for CreateEncryptKeys.
         :type request: :class:`tencentcloud.drm.v20181115.models.CreateEncryptKeysRequest`
@@ -66,15 +66,15 @@
             model = models.CreateEncryptKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLicense(self, request):
         """本接口用来生成DRM方案对应的播放许可证，开发者需提供DRM方案类型、内容类型参数，后台将生成许可证后返回许可证数据
         开发者需要转发终端设备发出的许可证请求信息。
 
         :param request: Request instance for CreateLicense.
@@ -90,15 +90,15 @@
             model = models.CreateLicenseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFairPlayPem(self, request):
         """本接口用来删除fairplay方案的私钥、ask等信息
         注：高风险操作，删除后，您将无法使用腾讯云DRM提供的fairplay服务。
         由于缓存，删除操作需要约半小时生效
 
@@ -115,15 +115,15 @@
             model = models.DeleteFairPlayPemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllKeys(self, request):
         """本接口用来查询指定DRM类型、ContentType的所有加密密钥
 
         :param request: Request instance for DescribeAllKeys.
         :type request: :class:`tencentcloud.drm.v20181115.models.DescribeAllKeysRequest`
@@ -138,15 +138,15 @@
             model = models.DescribeAllKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFairPlayPem(self, request):
         """该接口用来查询设置的FairPlay私钥校验信息。可用该接口校验设置的私钥与本身的私钥是否一致。
 
         :param request: Request instance for DescribeFairPlayPem.
         :type request: :class:`tencentcloud.drm.v20181115.models.DescribeFairPlayPemRequest`
@@ -161,15 +161,15 @@
             model = models.DescribeFairPlayPemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKeys(self, request):
         """开发者需要指定使用的DRM类型、和需要加密的Track类型，后台返回加密使用的密钥
         如果加密使用的ContentID没有关联的密钥信息，后台会自动生成新的密钥返回
 
         :param request: Request instance for DescribeKeys.
@@ -185,15 +185,15 @@
             model = models.DescribeKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFairPlayPem(self, request):
         """本接口用来设置fairplay方案所需的私钥、私钥密钥、ask等信息。
         如需使用fairplay方案，请务必先设置私钥。
 
         :param request: Request instance for ModifyFairPlayPem.
@@ -209,15 +209,15 @@
             model = models.ModifyFairPlayPemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartEncryption(self, request):
         """开发者调用该接口，启动一次内容文件的DRM加密工作流。
         注意：该接口已下线。
 
         :param request: Request instance for StartEncryption.
@@ -233,8 +233,8 @@
             model = models.StartEncryptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-drm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-drm-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-drm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Drm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-drm-3.0.937/README.rst` & `tencentcloud-sdk-python-drm-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-drm-3.0.937/tencentcloud_sdk_python_drm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-drm-3.0.938/tencentcloud_sdk_python_drm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-drm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Drm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

