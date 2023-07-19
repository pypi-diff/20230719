# Comparing `tmp/tencentcloud-sdk-python-ds-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ds-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ds-3.0.937.tar", last modified: Tue Jul 18 00:22:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ds-3.0.938.tar", last modified: Wed Jul 19 00:38:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ds-3.0.937.tar` & `tencentcloud-sdk-python-ds-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/
--rw-r--r--   0 root         (0) root         (0)    13710 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/ds_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10034 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49948 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:22:55.000000 tencentcloud-sdk-python-ds-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:22:54.000000 tencentcloud-sdk-python-ds-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/
+-rw-r--r--   0 root         (0) root         (0)    13758 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/ds_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10034 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49948 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:38:07.000000 tencentcloud-sdk-python-ds-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ds-3.0.937/setup.py` & `tencentcloud-sdk-python-ds-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ds-3.0.937/tencentcloud_sdk_python_ds.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ds-3.0.938/tencentcloud_sdk_python_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ds
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/ds_client.py` & `tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/ds_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.CheckVcodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateContractByUpload(self, request):
         """此接口适用于：客户平台通过上传PDF文件作为合同，以备未来进行签署。接口返回任务号，可调用DescribeTaskStatus接口查看任务执行结果。
 
         :param request: Request instance for CreateContractByUpload.
         :type request: :class:`tencentcloud.ds.v20180523.models.CreateContractByUploadRequest`
@@ -67,15 +67,15 @@
             model = models.CreateContractByUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEnterpriseAccount(self, request):
         """为企业电子合同平台的最终企业用户进行开户。在企业电子合同平台进行操作的企业用户，企业电子合同平台向腾讯云发送企业用户的信息，提交开户命令。腾讯云接到请求后，自动为企业电子合同平台的企业用户生成一张数字证书。
 
         :param request: Request instance for CreateEnterpriseAccount.
         :type request: :class:`tencentcloud.ds.v20180523.models.CreateEnterpriseAccountRequest`
@@ -90,15 +90,15 @@
             model = models.CreateEnterpriseAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePersonalAccount(self, request):
         """为企业电子合同平台的最终个人用户进行开户。在企业电子合同平台进行操作的个人用户，企业电子合同平台向腾讯云发送个人用户的信息，提交开户命令。腾讯云接到请求后，自动为企业电子合同平台的个人用户生成一张数字证书。
 
         :param request: Request instance for CreatePersonalAccount.
         :type request: :class:`tencentcloud.ds.v20180523.models.CreatePersonalAccountRequest`
@@ -113,15 +113,15 @@
             model = models.CreatePersonalAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSeal(self, request):
         """此接口用于客户电子合同平台增加某用户的印章图片。客户平台可以调用此接口增加某用户的印章图片。
 
         :param request: Request instance for CreateSeal.
         :type request: :class:`tencentcloud.ds.v20180523.models.CreateSealRequest`
@@ -136,15 +136,15 @@
             model = models.CreateSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccount(self, request):
         """删除企业电子合同平台的最终用户。调用该接口后，腾讯云将删除该用户账号。删除账号后，已经签名的合同不受影响。
 
         :param request: Request instance for DeleteAccount.
         :type request: :class:`tencentcloud.ds.v20180523.models.DeleteAccountRequest`
@@ -159,15 +159,15 @@
             model = models.DeleteAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSeal(self, request):
         """删除印章接口，删除指定账号的某个印章
 
         :param request: Request instance for DeleteSeal.
         :type request: :class:`tencentcloud.ds.v20180523.models.DeleteSealRequest`
@@ -182,15 +182,15 @@
             model = models.DeleteSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStatus(self, request):
         """接口使用于：客户平台可使用该接口查询任务执行状态或者执行结果
 
         :param request: Request instance for DescribeTaskStatus.
         :type request: :class:`tencentcloud.ds.v20180523.models.DescribeTaskStatusRequest`
@@ -205,15 +205,15 @@
             model = models.DescribeTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadContract(self, request):
         """下载合同接口。调用该接口可以下载签署中和签署完成的合同。接口返回任务号，可调用DescribeTaskStatus接口查看任务执行结果。
 
         :param request: Request instance for DownloadContract.
         :type request: :class:`tencentcloud.ds.v20180523.models.DownloadContractRequest`
@@ -228,15 +228,15 @@
             model = models.DownloadContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendVcode(self, request):
         """发送验证码接口。此接口用于：企业电子合同平台需要腾讯云发送验证码对其用户进行验证时调用，腾讯云将向其用户联系手机(企业电子合同平台为用户开户时通过接口传入)发送验证码，以验证码授权方式签署合同。用户验证工作由企业电子合同平台自身完成。
 
         :param request: Request instance for SendVcode.
         :type request: :class:`tencentcloud.ds.v20180523.models.SendVcodeRequest`
@@ -251,15 +251,15 @@
             model = models.SendVcodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SignContractByCoordinate(self, request):
         """此接口适用于：客户平台在创建好合同后，由合同签署方对创建的合同内容进行确认，无误后再进行签署。客户平台使用该接口提供详细的PDF文档签名坐标进行签署。
 
         :param request: Request instance for SignContractByCoordinate.
         :type request: :class:`tencentcloud.ds.v20180523.models.SignContractByCoordinateRequest`
@@ -274,15 +274,15 @@
             model = models.SignContractByCoordinateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SignContractByKeyword(self, request):
         """此接口适用于：客户平台在创建好合同后，由合同签署方对创建的合同内容进行确认，无误后再进行签署。客户平台使用该接口对PDF合同文档按照关键字和坐标进行签署。
 
         :param request: Request instance for SignContractByKeyword.
         :type request: :class:`tencentcloud.ds.v20180523.models.SignContractByKeywordRequest`
@@ -297,8 +297,8 @@
             model = models.SignContractByKeywordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/errorcodes.py` & `tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ds-3.0.937/tencentcloud/ds/v20180523/models.py` & `tencentcloud-sdk-python-ds-3.0.938/tencentcloud/ds/v20180523/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ds-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ds-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ds-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ds-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ds
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ds-3.0.937/README.rst` & `tencentcloud-sdk-python-ds-3.0.938/README.rst`

 * *Files identical despite different names*

