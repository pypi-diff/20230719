# Comparing `tmp/tencentcloud-sdk-python-ssm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ssm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.937.tar", last modified: Tue Jul 18 00:30:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.938.tar", last modified: Wed Jul 19 00:45:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssm-3.0.937.tar` & `tencentcloud-sdk-python-ssm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24513 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/ssm_client.py
--rw-r--r--   0 root         (0) root         (0)   100023 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:31.000000 tencentcloud-sdk-python-ssm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24609 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/ssm_client.py
+-rw-r--r--   0 root         (0) root         (0)   100023 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:45:43.000000 tencentcloud-sdk-python-ssm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/setup.py` & `tencentcloud-sdk-python-ssm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.938/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/errorcodes.py` & `tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/ssm_client.py` & `tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/ssm_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateProductSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSSHKeyPairSecret(self, request):
         """创建用于托管SSH密钥对的凭据
 
         :param request: Request instance for CreateSSHKeyPairSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.CreateSSHKeyPairSecretRequest`
@@ -65,15 +65,15 @@
             model = models.CreateSSHKeyPairSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecret(self, request):
         """创建新的凭据信息，通过KMS进行加密保护。每个Region最多可创建存储1000个凭据信息。
 
         :param request: Request instance for CreateSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.CreateSecretRequest`
@@ -88,15 +88,15 @@
             model = models.CreateSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecret(self, request):
         """删除指定的凭据信息，可以通过RecoveryWindowInDays参数设置立即删除或者计划删除。对于计划删除的凭据，在删除日期到达之前状态为 PendingDelete，并可以通过RestoreSecret 进行恢复，超出指定删除日期之后会被彻底删除。您必须先通过 DisableSecret 停用凭据后才可以进行（计划）删除操作。
 
         :param request: Request instance for DeleteSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.DeleteSecretRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecretVersion(self, request):
         """该接口用于直接删除指定凭据下的单个版本凭据，删除操作立即生效，对所有状态下的凭据版本都可以删除。
         本接口仅适用于用户自定义凭据，本接口不能对云产品凭据进行操作。
 
         :param request: Request instance for DeleteSecretVersion.
@@ -135,15 +135,15 @@
             model = models.DeleteSecretVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAsyncRequestInfo(self, request):
         """查询异步任务的执行结果
 
         :param request: Request instance for DescribeAsyncRequestInfo.
         :type request: :class:`tencentcloud.ssm.v20190923.models.DescribeAsyncRequestInfoRequest`
@@ -158,15 +158,15 @@
             model = models.DescribeAsyncRequestInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRotationDetail(self, request):
         """查询凭据轮转策略详情。
         本接口只适用于云产品凭据。
 
         :param request: Request instance for DescribeRotationDetail.
@@ -182,15 +182,15 @@
             model = models.DescribeRotationDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRotationHistory(self, request):
         """查询凭据轮转历史版本。
         本接口仅适用于云产品凭据。
 
         :param request: Request instance for DescribeRotationHistory.
@@ -206,15 +206,15 @@
             model = models.DescribeRotationHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecret(self, request):
         """获取凭据的详细属性信息。
 
         :param request: Request instance for DescribeSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.DescribeSecretRequest`
@@ -229,15 +229,15 @@
             model = models.DescribeSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSupportedProducts(self, request):
         """查询支持的云产品列表
 
         :param request: Request instance for DescribeSupportedProducts.
         :type request: :class:`tencentcloud.ssm.v20190923.models.DescribeSupportedProductsRequest`
@@ -252,15 +252,15 @@
             model = models.DescribeSupportedProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableSecret(self, request):
         """停用指定的凭据，停用后状态为 Disabled，无法通过接口获取该凭据的明文。
 
         :param request: Request instance for DisableSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.DisableSecretRequest`
@@ -275,15 +275,15 @@
             model = models.DisableSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableSecret(self, request):
         """该接口用于开启凭据，状态为Enabled。可以通过 GetSecretValue 接口获取凭据明文。处于PendingDelete状态的凭据不能直接开启，需要通过RestoreSecret 恢复后再开启使用。
 
         :param request: Request instance for EnableSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.EnableSecretRequest`
@@ -298,15 +298,15 @@
             model = models.EnableSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRegions(self, request):
         """获取控制台展示region列表
 
         :param request: Request instance for GetRegions.
         :type request: :class:`tencentcloud.ssm.v20190923.models.GetRegionsRequest`
@@ -321,15 +321,15 @@
             model = models.GetRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSSHKeyPairValue(self, request):
         """获取SSH密钥对凭据明文信息。
 
         :param request: Request instance for GetSSHKeyPairValue.
         :type request: :class:`tencentcloud.ssm.v20190923.models.GetSSHKeyPairValueRequest`
@@ -344,15 +344,15 @@
             model = models.GetSSHKeyPairValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSecretValue(self, request):
         """对于用户自定义凭据，通过指定凭据名称和版本来获取凭据的明文信息；
         对于云产品凭据如Mysql凭据，通过指定凭据名称和历史版本号来获取历史轮转凭据的明文信息，如果要获取当前正在使用的凭据版本的明文，需要将版本号指定为：SSM_Current。
 
         :param request: Request instance for GetSecretValue.
@@ -368,15 +368,15 @@
             model = models.GetSecretValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetServiceStatus(self, request):
         """该接口用户获取用户SecretsManager服务开通状态。
 
         :param request: Request instance for GetServiceStatus.
         :type request: :class:`tencentcloud.ssm.v20190923.models.GetServiceStatusRequest`
@@ -391,15 +391,15 @@
             model = models.GetServiceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListSecretVersionIds(self, request):
         """该接口用于获取指定凭据下的版本列表信息
 
         :param request: Request instance for ListSecretVersionIds.
         :type request: :class:`tencentcloud.ssm.v20190923.models.ListSecretVersionIdsRequest`
@@ -414,15 +414,15 @@
             model = models.ListSecretVersionIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListSecrets(self, request):
         """该接口用于获取所有凭据的详细列表，可以指定过滤字段、排序方式等。
 
         :param request: Request instance for ListSecrets.
         :type request: :class:`tencentcloud.ssm.v20190923.models.ListSecretsRequest`
@@ -437,15 +437,15 @@
             model = models.ListSecretsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutSecretValue(self, request):
         """该接口在指定名称的凭据下增加新版本的凭据内容，一个凭据下最多可以支持10个版本。只能对处于Enabled 和 Disabled 状态的凭据添加新的版本。
         本接口仅适用于用户自定义凭据，对云产品凭据不能操作。
 
         :param request: Request instance for PutSecretValue.
@@ -461,15 +461,15 @@
             model = models.PutSecretValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestoreSecret(self, request):
         """该接口用于恢复计划删除（PendingDelete状态）中的凭据，取消计划删除。取消计划删除的凭据将处于Disabled 状态，如需恢复使用，通过EnableSecret 接口开启凭据。
 
         :param request: Request instance for RestoreSecret.
         :type request: :class:`tencentcloud.ssm.v20190923.models.RestoreSecretRequest`
@@ -484,15 +484,15 @@
             model = models.RestoreSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RotateProductSecret(self, request):
         """轮转云产品凭据或云API密钥对凭据。
         该接口仅适用于处于Enabled状态的云产品凭据或处于Enable状态的云API密钥对凭据，对于其他状态的云产品凭据或云API密钥对凭据或用户自定义凭据不适用。
 
         :param request: Request instance for RotateProductSecret.
@@ -508,15 +508,15 @@
             model = models.RotateProductSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDescription(self, request):
         """该接口用于修改指定凭据的描述信息，仅能修改Enabled 和 Disabled 状态的凭据。
 
         :param request: Request instance for UpdateDescription.
         :type request: :class:`tencentcloud.ssm.v20190923.models.UpdateDescriptionRequest`
@@ -531,15 +531,15 @@
             model = models.UpdateDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRotationStatus(self, request):
         """设置云产品凭据轮转策略，可以设置：
         是否开启轮转
         轮转周期
         轮转开始时间
@@ -557,15 +557,15 @@
             model = models.UpdateRotationStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateSecret(self, request):
         """该接口用于更新指定凭据名称和版本号的内容，调用该接口会对新的凭据内容加密后覆盖旧的内容。仅允许更新Enabled 和 Disabled 状态的凭据。
         本接口仅适用于用户自定义凭据，不能对云产品凭据操作。
 
         :param request: Request instance for UpdateSecret.
@@ -581,8 +581,8 @@
             model = models.UpdateSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/ssm/v20190923/models.py` & `tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/ssm/v20190923/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.937/README.rst` & `tencentcloud-sdk-python-ssm-3.0.938/README.rst`

 * *Files identical despite different names*

