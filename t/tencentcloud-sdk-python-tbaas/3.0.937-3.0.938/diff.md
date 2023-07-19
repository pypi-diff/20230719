# Comparing `tmp/tencentcloud-sdk-python-tbaas-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tbaas-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.937.tar", last modified: Tue Jul 18 00:31:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.938.tar", last modified: Wed Jul 19 00:48:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbaas-3.0.937.tar` & `tencentcloud-sdk-python-tbaas-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/
--rw-r--r--   0 root         (0) root         (0)    28041 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/tbaas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11697 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   156059 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:31:02.000000 tencentcloud-sdk-python-tbaas-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    28157 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/tbaas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   156059 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:48:28.000000 tencentcloud-sdk-python-tbaas-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/setup.py` & `tencentcloud-sdk-python-tbaas-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/tbaas_client.py` & `tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/tbaas_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyChainMakerBatchUserCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyUserCert(self, request):
         """申请用户证书
 
         :param request: Request instance for ApplyUserCert.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.ApplyUserCertRequest`
@@ -65,15 +65,15 @@
             model = models.ApplyUserCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateChaincodeAndInstallForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         创建并安装合约
 
@@ -90,15 +90,15 @@
             model = models.CreateChaincodeAndInstallForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadUserCert(self, request):
         """下载用户证书
 
         :param request: Request instance for DownloadUserCert.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.DownloadUserCertRequest`
@@ -113,15 +113,15 @@
             model = models.DownloadUserCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetBlockList(self, request):
         """查看当前网络下的所有区块列表，分页展示
 
         :param request: Request instance for GetBlockList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBlockListRequest`
@@ -136,15 +136,15 @@
             model = models.GetBlockListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetBlockTransactionListForUser(self, request):
         """获取区块内的交易列表
 
         :param request: Request instance for GetBlockTransactionListForUser.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBlockTransactionListForUserRequest`
@@ -159,15 +159,15 @@
             model = models.GetBlockTransactionListForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetChaincodeCompileLogForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         获取合约编译日志
 
@@ -184,15 +184,15 @@
             model = models.GetChaincodeCompileLogForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetChaincodeInitializeResultForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         实例化结果查询
 
@@ -209,15 +209,15 @@
             model = models.GetChaincodeInitializeResultForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetChaincodeLogForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         获取合约容器日志
 
@@ -234,15 +234,15 @@
             model = models.GetChaincodeLogForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetChannelListForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         获取通道列表
 
@@ -259,15 +259,15 @@
             model = models.GetChannelListForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetClusterListForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         获取该用户的网络列表。网络信息中包含组织信息，但仅包含该用户所在组织的信息。
 
@@ -284,15 +284,15 @@
             model = models.GetClusterListForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetClusterSummary(self, request):
         """获取区块链网络概要
 
         :param request: Request instance for GetClusterSummary.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetClusterSummaryRequest`
@@ -307,15 +307,15 @@
             model = models.GetClusterSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetInvokeTx(self, request):
         """Invoke异步调用结果查询
 
         :param request: Request instance for GetInvokeTx.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetInvokeTxRequest`
@@ -330,15 +330,15 @@
             model = models.GetInvokeTxResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLatesdTransactionList(self, request):
         """获取最新交易列表（已废弃）
 
         :param request: Request instance for GetLatesdTransactionList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetLatesdTransactionListRequest`
@@ -353,15 +353,15 @@
             model = models.GetLatesdTransactionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLatestTransactionList(self, request):
         """获取fabric最新交易列表
 
         :param request: Request instance for GetLatestTransactionList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetLatestTransactionListRequest`
@@ -376,15 +376,15 @@
             model = models.GetLatestTransactionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPeerLogForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         获取节点日志
 
@@ -401,15 +401,15 @@
             model = models.GetPeerLogForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTransactionDetailForUser(self, request):
         """获取交易详情
 
         :param request: Request instance for GetTransactionDetailForUser.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetTransactionDetailForUserRequest`
@@ -424,15 +424,15 @@
             model = models.GetTransactionDetailForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InitializeChaincodeForUser(self, request):
         """接口已废弃，请通过控制台查询或操作
 
         实例化合约
 
@@ -449,15 +449,15 @@
             model = models.InitializeChaincodeForUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Invoke(self, request):
         """新增交易
 
         :param request: Request instance for Invoke.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeRequest`
@@ -472,15 +472,15 @@
             model = models.InvokeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InvokeChainMakerContract(self, request):
         """调用长安链合约执行交易
 
         :param request: Request instance for InvokeChainMakerContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeChainMakerContractRequest`
@@ -495,15 +495,15 @@
             model = models.InvokeChainMakerContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InvokeChainMakerDemoContract(self, request):
         """调用长安链体验网络合约执行交易
 
         :param request: Request instance for InvokeChainMakerDemoContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeChainMakerDemoContractRequest`
@@ -518,15 +518,15 @@
             model = models.InvokeChainMakerDemoContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Query(self, request):
         """查询交易
 
         :param request: Request instance for Query.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryRequest`
@@ -541,15 +541,15 @@
             model = models.QueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerBlockTransaction(self, request):
         """查询长安链指定高度区块的交易
 
         :param request: Request instance for QueryChainMakerBlockTransaction.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerBlockTransactionRequest`
@@ -564,15 +564,15 @@
             model = models.QueryChainMakerBlockTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerContract(self, request):
         """调用长安链合约查询
 
         :param request: Request instance for QueryChainMakerContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerContractRequest`
@@ -587,15 +587,15 @@
             model = models.QueryChainMakerContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerDemoBlockTransaction(self, request):
         """查询长安链体验网络指定高度区块的交易
 
         :param request: Request instance for QueryChainMakerDemoBlockTransaction.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerDemoBlockTransactionRequest`
@@ -610,15 +610,15 @@
             model = models.QueryChainMakerDemoBlockTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerDemoContract(self, request):
         """调用长安链体验网络合约查询
 
         :param request: Request instance for QueryChainMakerDemoContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerDemoContractRequest`
@@ -633,15 +633,15 @@
             model = models.QueryChainMakerDemoContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerDemoTransaction(self, request):
         """通过交易ID查询长安链体验网络交易
 
         :param request: Request instance for QueryChainMakerDemoTransaction.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerDemoTransactionRequest`
@@ -656,15 +656,15 @@
             model = models.QueryChainMakerDemoTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChainMakerTransaction(self, request):
         """通过交易ID查询长安链交易
 
         :param request: Request instance for QueryChainMakerTransaction.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.QueryChainMakerTransactionRequest`
@@ -679,15 +679,15 @@
             model = models.QueryChainMakerTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SrvInvoke(self, request):
         """trustsql服务统一接口
 
         :param request: Request instance for SrvInvoke.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.SrvInvokeRequest`
@@ -702,8 +702,8 @@
             model = models.SrvInvokeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/errorcodes.py` & `tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/tbaas/v20180416/models.py` & `tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/tbaas/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.938/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.937/README.rst` & `tencentcloud-sdk-python-tbaas-3.0.938/README.rst`

 * *Files identical despite different names*

