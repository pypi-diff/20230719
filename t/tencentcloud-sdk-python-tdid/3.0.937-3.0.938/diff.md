# Comparing `tmp/tencentcloud-sdk-python-tdid-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tdid-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.937.tar", last modified: Tue Jul 18 00:32:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.938.tar", last modified: Wed Jul 19 00:49:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdid-3.0.937.tar` & `tencentcloud-sdk-python-tdid-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17289 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    63817 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:32:10.000000 tencentcloud-sdk-python-tdid-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17361 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    63817 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:49:49.000000 tencentcloud-sdk-python-tdid-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/setup.py` & `tencentcloud-sdk-python-tdid-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/tdid_client.py` & `tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/tdid_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.AddLabelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckChain(self, request):
         """该接口不再使用
 
         检查区块链信息
 
@@ -69,15 +69,15 @@
             model = models.CheckChainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCredential(self, request):
         """该接口不再使用
 
         创建凭证
 
@@ -94,15 +94,15 @@
             model = models.CreateCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSelectiveCredential(self, request):
         """该接口不再使用
 
         创建选择性批露凭证
 
@@ -119,15 +119,15 @@
             model = models.CreateSelectiveCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTDid(self, request):
         """该接口不再使用
 
         创建机构DID
 
@@ -144,15 +144,15 @@
             model = models.CreateTDidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTDidByPrivateKey(self, request):
         """该接口不再使用
 
         新建DID根据私钥生成Tdid
 
@@ -169,15 +169,15 @@
             model = models.CreateTDidByPrivateKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTDidByPublicKey(self, request):
         """该接口不再使用
 
          新建DID根据公钥生成Tdid
 
@@ -194,15 +194,15 @@
             model = models.CreateTDidByPublicKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAgencyTDid(self, request):
         """该接口已废弃
 
         本机构DID详情
 
@@ -219,15 +219,15 @@
             model = models.GetAgencyTDidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAuthorityIssuer(self, request):
         """该接口不再使用
 
         获取权威机构信息
 
@@ -244,15 +244,15 @@
             model = models.GetAuthorityIssuerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetConsortiumClusterList(self, request):
         """下线已有内测接口，待上线正式版本的接口
 
         获取联盟bcos网络列表
 
@@ -269,15 +269,15 @@
             model = models.GetConsortiumClusterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetConsortiumList(self, request):
         """下线已有内测接口，待上线正式版本的接口
 
         获取联盟列表
 
@@ -294,15 +294,15 @@
             model = models.GetConsortiumListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCptInfo(self, request):
         """该接口不再使用
 
         凭证模版详情
 
@@ -319,15 +319,15 @@
             model = models.GetCptInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCredentialCptRank(self, request):
         """下线已有内测接口，待上线正式版本的接口
 
         凭证颁发按机构排行
 
@@ -344,15 +344,15 @@
             model = models.GetCredentialCptRankResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCredentialStatus(self, request):
         """该接口不再使用
 
         获取凭证链上状态信息
 
@@ -369,15 +369,15 @@
             model = models.GetCredentialStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDidDocument(self, request):
         """该接口不再使用
 
         查看DID文档
 
@@ -394,15 +394,15 @@
             model = models.GetDidDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterCpt(self, request):
         """该接口不再使用
 
         凭证模版新建
 
@@ -419,15 +419,15 @@
             model = models.RegisterCptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetCredentialStatus(self, request):
         """该接口不再使用
 
         设置凭证链上状态
 
@@ -444,15 +444,15 @@
             model = models.SetCredentialStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyCredential(self, request):
         """该接口不再使用
 
         验证凭证
 
@@ -469,8 +469,8 @@
             model = models.VerifyCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/tencentcloud/tdid/v20210519/models.py` & `tencentcloud-sdk-python-tdid-3.0.938/tencentcloud/tdid/v20210519/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.938/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.937/README.rst` & `tencentcloud-sdk-python-tdid-3.0.938/README.rst`

 * *Files identical despite different names*

