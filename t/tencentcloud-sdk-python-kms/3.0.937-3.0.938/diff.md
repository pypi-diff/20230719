# Comparing `tmp/tencentcloud-sdk-python-kms-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-kms-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.937.tar", last modified: Tue Jul 18 00:26:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.938.tar", last modified: Wed Jul 19 00:41:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-kms-3.0.937.tar` & `tencentcloud-sdk-python-kms-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/
--rw-r--r--   0 root         (0) root         (0)    50843 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/kms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   156339 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:26:24.000000 tencentcloud-sdk-python-kms-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/
+-rw-r--r--   0 root         (0) root         (0)    51055 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/kms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   156339 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:41:51.000000 tencentcloud-sdk-python-kms-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-kms-3.0.937/setup.py` & `tencentcloud-sdk-python-kms-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.937/tencentcloud_sdk_python_kms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.938/tencentcloud_sdk_python_kms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-kms-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/kms_client.py` & `tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/kms_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ArchiveKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AsymmetricRsaDecrypt(self, request):
         """使用指定的RSA非对称密钥的私钥进行数据解密，密文必须是使用对应公钥加密的。处于Enabled 状态的非对称密钥才能进行解密操作。
 
         :param request: Request instance for AsymmetricRsaDecrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.AsymmetricRsaDecryptRequest`
@@ -65,15 +65,15 @@
             model = models.AsymmetricRsaDecryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AsymmetricSm2Decrypt(self, request):
         """使用指定的SM2非对称密钥的私钥进行数据解密，密文必须是使用对应公钥加密的。处于Enabled 状态的非对称密钥才能进行解密操作。传入的密文的长度不能超过256字节。
 
         :param request: Request instance for AsymmetricSm2Decrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.AsymmetricSm2DecryptRequest`
@@ -88,15 +88,15 @@
             model = models.AsymmetricSm2DecryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindCloudResource(self, request):
         """记录当前key被哪个云产品的那个资源所使用。如果当前key设置了自动过期，则取消该设置，确保当前key不会自动失效。如果当前关联关系已经创建，也返回成功。
 
         :param request: Request instance for BindCloudResource.
         :type request: :class:`tencentcloud.kms.v20190118.models.BindCloudResourceRequest`
@@ -111,15 +111,15 @@
             model = models.BindCloudResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelKeyArchive(self, request):
         """取消密钥归档，取消后密钥的状态变为Enabled。
 
         :param request: Request instance for CancelKeyArchive.
         :type request: :class:`tencentcloud.kms.v20190118.models.CancelKeyArchiveRequest`
@@ -134,15 +134,15 @@
             model = models.CancelKeyArchiveResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelKeyDeletion(self, request):
         """取消CMK的计划删除操作
 
         :param request: Request instance for CancelKeyDeletion.
         :type request: :class:`tencentcloud.kms.v20190118.models.CancelKeyDeletionRequest`
@@ -157,15 +157,15 @@
             model = models.CancelKeyDeletionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKey(self, request):
         """创建用户管理数据密钥的主密钥CMK（Custom Master Key）。
 
         :param request: Request instance for CreateKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.CreateKeyRequest`
@@ -180,15 +180,15 @@
             model = models.CreateKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWhiteBoxKey(self, request):
         """创建白盒密钥。 密钥个数的上限为 50。
 
         :param request: Request instance for CreateWhiteBoxKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.CreateWhiteBoxKeyRequest`
@@ -203,15 +203,15 @@
             model = models.CreateWhiteBoxKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Decrypt(self, request):
         """本接口用于解密密文，得到明文数据。
 
         :param request: Request instance for Decrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.DecryptRequest`
@@ -226,15 +226,15 @@
             model = models.DecryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImportedKeyMaterial(self, request):
         """用于删除导入的密钥材料，仅对EXTERNAL类型的CMK有效，该接口将CMK设置为PendingImport 状态，并不会删除CMK，在重新进行密钥导入后可继续使用。彻底删除CMK请使用 ScheduleKeyDeletion 接口。
 
         :param request: Request instance for DeleteImportedKeyMaterial.
         :type request: :class:`tencentcloud.kms.v20190118.models.DeleteImportedKeyMaterialRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteImportedKeyMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWhiteBoxKey(self, request):
         """删除白盒密钥, 注意：必须先禁用后，才可以删除。
 
         :param request: Request instance for DeleteWhiteBoxKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DeleteWhiteBoxKeyRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteWhiteBoxKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKey(self, request):
         """用于获取指定KeyId的主密钥属性详情信息。
 
         :param request: Request instance for DescribeKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeKeyRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKeys(self, request):
         """该接口用于批量获取主密钥属性信息。
 
         :param request: Request instance for DescribeKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeKeysRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteBoxDecryptKey(self, request):
         """获取白盒解密密钥
 
         :param request: Request instance for DescribeWhiteBoxDecryptKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeWhiteBoxDecryptKeyRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeWhiteBoxDecryptKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteBoxDeviceFingerprints(self, request):
         """获取指定密钥的设备指纹列表
 
         :param request: Request instance for DescribeWhiteBoxDeviceFingerprints.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeWhiteBoxDeviceFingerprintsRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeWhiteBoxDeviceFingerprintsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteBoxKey(self, request):
         """展示白盒密钥的信息
 
         :param request: Request instance for DescribeWhiteBoxKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeWhiteBoxKeyRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeWhiteBoxKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteBoxKeyDetails(self, request):
         """获取白盒密钥列表
 
         :param request: Request instance for DescribeWhiteBoxKeyDetails.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeWhiteBoxKeyDetailsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeWhiteBoxKeyDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteBoxServiceStatus(self, request):
         """获取白盒密钥服务状态
 
         :param request: Request instance for DescribeWhiteBoxServiceStatus.
         :type request: :class:`tencentcloud.kms.v20190118.models.DescribeWhiteBoxServiceStatusRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeWhiteBoxServiceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableKey(self, request):
         """本接口用于禁用一个主密钥，处于禁用状态的Key无法用于加密、解密操作。
 
         :param request: Request instance for DisableKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DisableKeyRequest`
@@ -456,15 +456,15 @@
             model = models.DisableKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableKeyRotation(self, request):
         """对指定的CMK禁止密钥轮换功能。
 
         :param request: Request instance for DisableKeyRotation.
         :type request: :class:`tencentcloud.kms.v20190118.models.DisableKeyRotationRequest`
@@ -479,15 +479,15 @@
             model = models.DisableKeyRotationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableKeys(self, request):
         """该接口用于批量禁止CMK的使用。
 
         :param request: Request instance for DisableKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.DisableKeysRequest`
@@ -502,15 +502,15 @@
             model = models.DisableKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableWhiteBoxKey(self, request):
         """禁用白盒密钥
 
         :param request: Request instance for DisableWhiteBoxKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.DisableWhiteBoxKeyRequest`
@@ -525,15 +525,15 @@
             model = models.DisableWhiteBoxKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableWhiteBoxKeys(self, request):
         """批量禁用白盒密钥
 
         :param request: Request instance for DisableWhiteBoxKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.DisableWhiteBoxKeysRequest`
@@ -548,15 +548,15 @@
             model = models.DisableWhiteBoxKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableKey(self, request):
         """用于启用一个指定的CMK。
 
         :param request: Request instance for EnableKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.EnableKeyRequest`
@@ -571,15 +571,15 @@
             model = models.EnableKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableKeyRotation(self, request):
         """对指定的CMK开启密钥轮换功能。
 
         :param request: Request instance for EnableKeyRotation.
         :type request: :class:`tencentcloud.kms.v20190118.models.EnableKeyRotationRequest`
@@ -594,15 +594,15 @@
             model = models.EnableKeyRotationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableKeys(self, request):
         """该接口用于批量启用CMK。
 
         :param request: Request instance for EnableKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.EnableKeysRequest`
@@ -617,15 +617,15 @@
             model = models.EnableKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableWhiteBoxKey(self, request):
         """启用白盒密钥
 
         :param request: Request instance for EnableWhiteBoxKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.EnableWhiteBoxKeyRequest`
@@ -640,15 +640,15 @@
             model = models.EnableWhiteBoxKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableWhiteBoxKeys(self, request):
         """批量启用白盒密钥
 
         :param request: Request instance for EnableWhiteBoxKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.EnableWhiteBoxKeysRequest`
@@ -663,15 +663,15 @@
             model = models.EnableWhiteBoxKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Encrypt(self, request):
         """本接口用于加密最多为4KB任意数据，可用于加密数据库密码，RSA Key，或其它较小的敏感信息。对于应用的数据加密，使用GenerateDataKey生成的DataKey进行本地数据的加解密操作
 
         :param request: Request instance for Encrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.EncryptRequest`
@@ -686,15 +686,15 @@
             model = models.EncryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EncryptByWhiteBox(self, request):
         """使用白盒密钥进行加密
 
         :param request: Request instance for EncryptByWhiteBox.
         :type request: :class:`tencentcloud.kms.v20190118.models.EncryptByWhiteBoxRequest`
@@ -709,15 +709,15 @@
             model = models.EncryptByWhiteBoxResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateDataKey(self, request):
         """本接口生成一个数据密钥，您可以用这个密钥进行本地数据的加密。
 
         :param request: Request instance for GenerateDataKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.GenerateDataKeyRequest`
@@ -732,15 +732,15 @@
             model = models.GenerateDataKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateRandom(self, request):
         """随机数生成接口。
 
         :param request: Request instance for GenerateRandom.
         :type request: :class:`tencentcloud.kms.v20190118.models.GenerateRandomRequest`
@@ -755,15 +755,15 @@
             model = models.GenerateRandomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetKeyRotationStatus(self, request):
         """查询指定的CMK是否开启了密钥轮换功能。
 
         :param request: Request instance for GetKeyRotationStatus.
         :type request: :class:`tencentcloud.kms.v20190118.models.GetKeyRotationStatusRequest`
@@ -778,15 +778,15 @@
             model = models.GetKeyRotationStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetParametersForImport(self, request):
         """获取导入主密钥（CMK）材料的参数，返回的Token作为执行ImportKeyMaterial的参数之一，返回的PublicKey用于对自主导入密钥材料进行加密。返回的Token和PublicKey 24小时后失效，失效后如需重新导入，需要再次调用该接口获取新的Token和PublicKey。
 
         :param request: Request instance for GetParametersForImport.
         :type request: :class:`tencentcloud.kms.v20190118.models.GetParametersForImportRequest`
@@ -801,15 +801,15 @@
             model = models.GetParametersForImportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPublicKey(self, request):
         """该接口用于获取非对称密钥的公钥信息，可用于本地数据加密或验签。只有处于Enabled状态的非对称密钥才可能获取公钥。
 
         :param request: Request instance for GetPublicKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.GetPublicKeyRequest`
@@ -824,15 +824,15 @@
             model = models.GetPublicKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRegions(self, request):
         """获取可以提供KMS服务的地域列表
 
         :param request: Request instance for GetRegions.
         :type request: :class:`tencentcloud.kms.v20190118.models.GetRegionsRequest`
@@ -847,15 +847,15 @@
             model = models.GetRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetServiceStatus(self, request):
         """用于查询该用户是否已开通KMS服务
 
         :param request: Request instance for GetServiceStatus.
         :type request: :class:`tencentcloud.kms.v20190118.models.GetServiceStatusRequest`
@@ -870,15 +870,15 @@
             model = models.GetServiceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportKeyMaterial(self, request):
         """用于导入密钥材料。只有类型为EXTERNAL 的CMK 才可以导入，导入的密钥材料使用 GetParametersForImport 获取的密钥进行加密。可以为指定的 CMK 重新导入密钥材料，并重新指定过期时间，但必须导入相同的密钥材料。CMK 密钥材料导入后不可以更换密钥材料。导入的密钥材料过期或者被删除后，指定的CMK将无法使用，需要再次导入相同的密钥材料才能正常使用。CMK是独立的，同样的密钥材料可导入不同的 CMK 中，但使用其中一个 CMK 加密的数据无法使用另一个 CMK解密。
         只有Enabled 和 PendingImport状态的CMK可以导入密钥材料。
 
         :param request: Request instance for ImportKeyMaterial.
@@ -894,15 +894,15 @@
             model = models.ImportKeyMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAlgorithms(self, request):
         """列出当前Region支持的加密方式
 
         :param request: Request instance for ListAlgorithms.
         :type request: :class:`tencentcloud.kms.v20190118.models.ListAlgorithmsRequest`
@@ -917,15 +917,15 @@
             model = models.ListAlgorithmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListKeyDetail(self, request):
         """根据指定Offset和Limit获取主密钥列表详情。
 
         :param request: Request instance for ListKeyDetail.
         :type request: :class:`tencentcloud.kms.v20190118.models.ListKeyDetailRequest`
@@ -940,15 +940,15 @@
             model = models.ListKeyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListKeys(self, request):
         """列出账号下面状态为Enabled， Disabled 和 PendingImport 的CMK KeyId 列表
 
         :param request: Request instance for ListKeys.
         :type request: :class:`tencentcloud.kms.v20190118.models.ListKeysRequest`
@@ -963,15 +963,15 @@
             model = models.ListKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OverwriteWhiteBoxDeviceFingerprints(self, request):
         """覆盖指定密钥的设备指纹信息
 
         :param request: Request instance for OverwriteWhiteBoxDeviceFingerprints.
         :type request: :class:`tencentcloud.kms.v20190118.models.OverwriteWhiteBoxDeviceFingerprintsRequest`
@@ -986,15 +986,15 @@
             model = models.OverwriteWhiteBoxDeviceFingerprintsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PostQuantumCryptoDecrypt(self, request):
         """本接口使用后量子密码算法密钥，解密密文，并得到明文数据。
 
         :param request: Request instance for PostQuantumCryptoDecrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoDecryptRequest`
@@ -1009,15 +1009,15 @@
             model = models.PostQuantumCryptoDecryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PostQuantumCryptoEncrypt(self, request):
         """本接口使用后量子密码算法密钥，可加密最多为4KB任意数据，可用于加密数据库密码，RSA Key，或其它较小的敏感信息。对于应用的数据加密，使用GenerateDataKey生成的DataKey进行本地数据的加解密操作。
 
         :param request: Request instance for PostQuantumCryptoEncrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoEncryptRequest`
@@ -1032,15 +1032,15 @@
             model = models.PostQuantumCryptoEncryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PostQuantumCryptoSign(self, request):
         """使用后量子密码算法签名验签密钥进行签名。
 
         :param request: Request instance for PostQuantumCryptoSign.
         :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoSignRequest`
@@ -1055,15 +1055,15 @@
             model = models.PostQuantumCryptoSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PostQuantumCryptoVerify(self, request):
         """使用后量子密码算法密钥对签名进行验证。
 
         :param request: Request instance for PostQuantumCryptoVerify.
         :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoVerifyRequest`
@@ -1078,15 +1078,15 @@
             model = models.PostQuantumCryptoVerifyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReEncrypt(self, request):
         """使用指定CMK对密文重新加密。
 
         :param request: Request instance for ReEncrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.ReEncryptRequest`
@@ -1101,15 +1101,15 @@
             model = models.ReEncryptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScheduleKeyDeletion(self, request):
         """CMK计划删除接口，用于指定CMK删除的时间，可选时间区间为[7,30]天
 
         :param request: Request instance for ScheduleKeyDeletion.
         :type request: :class:`tencentcloud.kms.v20190118.models.ScheduleKeyDeletionRequest`
@@ -1124,15 +1124,15 @@
             model = models.ScheduleKeyDeletionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SignByAsymmetricKey(self, request):
         """非对称密钥签名。
         注意：只有 KeyUsage 为 ASYMMETRIC_SIGN_VERIFY_SM2、ASYMMETRIC_SIGN_VERIFY_ECC 或其他支持的 ASYMMETRIC_SIGN_VERIFY_${ALGORITHM} 的密钥才可以使用签名功能。
 
         :param request: Request instance for SignByAsymmetricKey.
@@ -1148,15 +1148,15 @@
             model = models.SignByAsymmetricKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindCloudResource(self, request):
         """删除指定（key, 资源，云产品）的记录，以表明：指定的云产品的资源已不再使用当前的key。
 
         :param request: Request instance for UnbindCloudResource.
         :type request: :class:`tencentcloud.kms.v20190118.models.UnbindCloudResourceRequest`
@@ -1171,15 +1171,15 @@
             model = models.UnbindCloudResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAlias(self, request):
         """用于修改CMK的别名。对于处于PendingDelete状态的CMK禁止修改。
 
         :param request: Request instance for UpdateAlias.
         :type request: :class:`tencentcloud.kms.v20190118.models.UpdateAliasRequest`
@@ -1194,15 +1194,15 @@
             model = models.UpdateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateKeyDescription(self, request):
         """该接口用于对指定的cmk修改描述信息。对于处于PendingDelete状态的CMK禁止修改。
 
         :param request: Request instance for UpdateKeyDescription.
         :type request: :class:`tencentcloud.kms.v20190118.models.UpdateKeyDescriptionRequest`
@@ -1217,15 +1217,15 @@
             model = models.UpdateKeyDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyByAsymmetricKey(self, request):
         """使用非对称密钥验签
 
         :param request: Request instance for VerifyByAsymmetricKey.
         :type request: :class:`tencentcloud.kms.v20190118.models.VerifyByAsymmetricKeyRequest`
@@ -1240,8 +1240,8 @@
             model = models.VerifyByAsymmetricKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/errorcodes.py` & `tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.937/tencentcloud/kms/v20190118/models.py` & `tencentcloud-sdk-python-kms-3.0.938/tencentcloud/kms/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.937/README.rst` & `tencentcloud-sdk-python-kms-3.0.938/README.rst`

 * *Files identical despite different names*

