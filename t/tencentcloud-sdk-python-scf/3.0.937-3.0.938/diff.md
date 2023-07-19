# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.937.tar", last modified: Tue Jul 18 00:29:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.938.tar", last modified: Wed Jul 19 00:44:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.937.tar` & `tencentcloud-sdk-python-scf-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42711 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32217 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   309047 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:31.000000 tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42891 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32217 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   309047 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:46.000000 tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.937/setup.py` & `tencentcloud-sdk-python-scf-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/scf_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             model = models.CopyFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlias(self, request):
         """为某个函数版本创建一个别名，您可以使用别名来标记特定的函数版本，如DEV/RELEASE版本，也可以随时修改别名指向的版本。
         一个别名必须指向一个主版本，此外还可以同时指向一个附加版本。调用函数时指定特定的别名，则请求会被发送到别名指向的版本上，您可以配置请求发送到主版本和附加版本的比例。
 
         :param request: Request instance for CreateAlias.
@@ -72,15 +72,15 @@
             model = models.CreateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFunction(self, request):
         """该接口根据传入参数创建新的函数。
 
         :param request: Request instance for CreateFunction.
         :type request: :class:`tencentcloud.scf.v20180416.models.CreateFunctionRequest`
@@ -95,15 +95,15 @@
             model = models.CreateFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespace(self, request):
         """该接口根据传入的参数创建命名空间。
 
         :param request: Request instance for CreateNamespace.
         :type request: :class:`tencentcloud.scf.v20180416.models.CreateNamespaceRequest`
@@ -118,15 +118,15 @@
             model = models.CreateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrigger(self, request):
         """该接口根据参数输入设置新的触发方式。
 
         :param request: Request instance for CreateTrigger.
         :type request: :class:`tencentcloud.scf.v20180416.models.CreateTriggerRequest`
@@ -141,15 +141,15 @@
             model = models.CreateTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlias(self, request):
         """删除一个函数版本的别名
 
         :param request: Request instance for DeleteAlias.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteAliasRequest`
@@ -164,15 +164,15 @@
             model = models.DeleteAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFunction(self, request):
         """该接口根据传入参数删除函数。
 
         :param request: Request instance for DeleteFunction.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteFunctionRequest`
@@ -187,15 +187,15 @@
             model = models.DeleteFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLayerVersion(self, request):
         """删除指定层的指定版本，被删除的版本无法再关联到函数上，但不会影响正在引用这个层的函数。
 
         :param request: Request instance for DeleteLayerVersion.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteLayerVersionRequest`
@@ -210,15 +210,15 @@
             model = models.DeleteLayerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNamespace(self, request):
         """该接口根据传入的参数删除命名空间。
 
         :param request: Request instance for DeleteNamespace.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteNamespaceRequest`
@@ -233,15 +233,15 @@
             model = models.DeleteNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProvisionedConcurrencyConfig(self, request):
         """删除函数版本的预置并发配置。
 
         :param request: Request instance for DeleteProvisionedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteProvisionedConcurrencyConfigRequest`
@@ -256,15 +256,15 @@
             model = models.DeleteProvisionedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReservedConcurrencyConfig(self, request):
         """删除函数的最大独占配额配置。
 
         :param request: Request instance for DeleteReservedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteReservedConcurrencyConfigRequest`
@@ -279,15 +279,15 @@
             model = models.DeleteReservedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrigger(self, request):
         """该接口根据参数传入删除已有的触发方式。
 
         :param request: Request instance for DeleteTrigger.
         :type request: :class:`tencentcloud.scf.v20180416.models.DeleteTriggerRequest`
@@ -302,15 +302,15 @@
             model = models.DeleteTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAccount(self, request):
         """获取账户信息
 
         :param request: Request instance for GetAccount.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetAccountRequest`
@@ -325,15 +325,15 @@
             model = models.GetAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAlias(self, request):
         """获取别名的详细信息，包括名称、描述、版本、路由信息等。
 
         :param request: Request instance for GetAlias.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetAliasRequest`
@@ -348,15 +348,15 @@
             model = models.GetAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAsyncEventStatus(self, request):
         """获取函数异步执行事件状态，事件状态保留 3 * 24 小时（从事件完成开始计时）。
 
         :param request: Request instance for GetAsyncEventStatus.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetAsyncEventStatusRequest`
@@ -371,15 +371,15 @@
             model = models.GetAsyncEventStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFunction(self, request):
         """该接口获取某个函数的详细信息，包括名称、代码、处理方法、关联触发器和超时时间等字段。
 
         :param request: Request instance for GetFunction.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetFunctionRequest`
@@ -394,15 +394,15 @@
             model = models.GetFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFunctionAddress(self, request):
         """该接口用于获取函数代码包的下载地址。
 
         :param request: Request instance for GetFunctionAddress.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetFunctionAddressRequest`
@@ -417,15 +417,15 @@
             model = models.GetFunctionAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFunctionEventInvokeConfig(self, request):
         """获取函数异步重试配置，包括重试次数和消息保留时间
 
         :param request: Request instance for GetFunctionEventInvokeConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetFunctionEventInvokeConfigRequest`
@@ -440,15 +440,15 @@
             model = models.GetFunctionEventInvokeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFunctionLogs(self, request):
         """该接口根据指定的日志查询条件返回函数运行日志。该接口已下线，查询函数请求运行的返回信息，请使用 [GetRequestStatus](https://cloud.tencent.com/document/product/583/65348)。查询函数运行日志，请参考[日志检索教程](https://cloud.tencent.com/document/product/583/52637)。
 
         :param request: Request instance for GetFunctionLogs.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetFunctionLogsRequest`
@@ -463,15 +463,15 @@
             model = models.GetFunctionLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLayerVersion(self, request):
         """获取层版本详细信息，包括用于下载层中文件的链接。
 
         :param request: Request instance for GetLayerVersion.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetLayerVersionRequest`
@@ -486,15 +486,15 @@
             model = models.GetLayerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetProvisionedConcurrencyConfig(self, request):
         """获取函数或函数某一版本的预置并发详情。
 
         :param request: Request instance for GetProvisionedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetProvisionedConcurrencyConfigRequest`
@@ -509,15 +509,15 @@
             model = models.GetProvisionedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRequestStatus(self, request):
         """该接口根据指定的查询条件返回函数单个请求运行状态。
 
         :param request: Request instance for GetRequestStatus.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetRequestStatusRequest`
@@ -532,15 +532,15 @@
             model = models.GetRequestStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetReservedConcurrencyConfig(self, request):
         """获取函数的最大独占配额详情。
 
         :param request: Request instance for GetReservedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.GetReservedConcurrencyConfigRequest`
@@ -555,15 +555,15 @@
             model = models.GetReservedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Invoke(self, request):
         """该接口用于运行函数。
 
         :param request: Request instance for Invoke.
         :type request: :class:`tencentcloud.scf.v20180416.models.InvokeRequest`
@@ -578,15 +578,15 @@
             model = models.InvokeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InvokeFunction(self, request):
         """SCF同步调用函数接口
 
         :param request: Request instance for InvokeFunction.
         :type request: :class:`tencentcloud.scf.v20180416.models.InvokeFunctionRequest`
@@ -601,15 +601,15 @@
             model = models.InvokeFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAliases(self, request):
         """返回一个函数下的全部别名，可以根据特定函数版本过滤。
 
         :param request: Request instance for ListAliases.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListAliasesRequest`
@@ -624,15 +624,15 @@
             model = models.ListAliasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAsyncEvents(self, request):
         """拉取函数异步事件列表
 
         :param request: Request instance for ListAsyncEvents.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListAsyncEventsRequest`
@@ -647,15 +647,15 @@
             model = models.ListAsyncEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListFunctions(self, request):
         """该接口根据传入的查询参数返回相关函数信息。
 
         :param request: Request instance for ListFunctions.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListFunctionsRequest`
@@ -670,15 +670,15 @@
             model = models.ListFunctionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLayerVersions(self, request):
         """返回指定层的全部版本的信息
 
         :param request: Request instance for ListLayerVersions.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListLayerVersionsRequest`
@@ -693,15 +693,15 @@
             model = models.ListLayerVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLayers(self, request):
         """返回全部层的列表，其中包含了每个层最新版本的信息，可以通过适配运行时进行过滤。
 
         :param request: Request instance for ListLayers.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListLayersRequest`
@@ -716,15 +716,15 @@
             model = models.ListLayersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListNamespaces(self, request):
         """列出命名空间列表
 
         :param request: Request instance for ListNamespaces.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListNamespacesRequest`
@@ -739,15 +739,15 @@
             model = models.ListNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTriggers(self, request):
         """获取函数触发器列表
 
         :param request: Request instance for ListTriggers.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListTriggersRequest`
@@ -762,15 +762,15 @@
             model = models.ListTriggersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListVersionByFunction(self, request):
         """该接口根据传入的参数查询函数的版本。
 
         :param request: Request instance for ListVersionByFunction.
         :type request: :class:`tencentcloud.scf.v20180416.models.ListVersionByFunctionRequest`
@@ -785,15 +785,15 @@
             model = models.ListVersionByFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishLayerVersion(self, request):
         """使用给定的zip文件或cos对象创建一个层的新版本，每次使用相同的层的名称调用本接口，都会生成一个新版本。
 
         :param request: Request instance for PublishLayerVersion.
         :type request: :class:`tencentcloud.scf.v20180416.models.PublishLayerVersionRequest`
@@ -808,15 +808,15 @@
             model = models.PublishLayerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishVersion(self, request):
         """该接口用于用户发布新版本函数。
 
         :param request: Request instance for PublishVersion.
         :type request: :class:`tencentcloud.scf.v20180416.models.PublishVersionRequest`
@@ -831,15 +831,15 @@
             model = models.PublishVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutProvisionedConcurrencyConfig(self, request):
         """设置函数某一非$LATEST版本的预置并发。
 
         :param request: Request instance for PutProvisionedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.PutProvisionedConcurrencyConfigRequest`
@@ -854,15 +854,15 @@
             model = models.PutProvisionedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutReservedConcurrencyConfig(self, request):
         """设置函数最大独占配额
 
         :param request: Request instance for PutReservedConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.PutReservedConcurrencyConfigRequest`
@@ -877,15 +877,15 @@
             model = models.PutReservedConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutTotalConcurrencyConfig(self, request):
         """修改账号并发限制配额
 
         :param request: Request instance for PutTotalConcurrencyConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.PutTotalConcurrencyConfigRequest`
@@ -900,15 +900,15 @@
             model = models.PutTotalConcurrencyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateAsyncEvent(self, request):
         """终止正在运行中的函数异步事件
 
         :param request: Request instance for TerminateAsyncEvent.
         :type request: :class:`tencentcloud.scf.v20180416.models.TerminateAsyncEventRequest`
@@ -923,15 +923,15 @@
             model = models.TerminateAsyncEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAlias(self, request):
         """更新别名的配置
 
         :param request: Request instance for UpdateAlias.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateAliasRequest`
@@ -946,15 +946,15 @@
             model = models.UpdateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFunctionCode(self, request):
         """该接口根据传入参数更新函数代码。
 
         :param request: Request instance for UpdateFunctionCode.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateFunctionCodeRequest`
@@ -969,15 +969,15 @@
             model = models.UpdateFunctionCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFunctionConfiguration(self, request):
         """该接口根据传入参数更新函数配置。
 
         :param request: Request instance for UpdateFunctionConfiguration.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateFunctionConfigurationRequest`
@@ -992,15 +992,15 @@
             model = models.UpdateFunctionConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFunctionEventInvokeConfig(self, request):
         """更新函数的异步重试配置，包括重试次数和消息保留时间
 
         :param request: Request instance for UpdateFunctionEventInvokeConfig.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateFunctionEventInvokeConfigRequest`
@@ -1015,15 +1015,15 @@
             model = models.UpdateFunctionEventInvokeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateNamespace(self, request):
         """更新命名空间
 
         :param request: Request instance for UpdateNamespace.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateNamespaceRequest`
@@ -1038,15 +1038,15 @@
             model = models.UpdateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTriggerStatus(self, request):
         """更新触发器状态的值
 
         :param request: Request instance for UpdateTriggerStatus.
         :type request: :class:`tencentcloud.scf.v20180416.models.UpdateTriggerStatusRequest`
@@ -1061,8 +1061,8 @@
             model = models.UpdateTriggerStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.937/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.938/tencentcloud/scf/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.937/README.rst` & `tencentcloud-sdk-python-scf-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.937/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.938/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

