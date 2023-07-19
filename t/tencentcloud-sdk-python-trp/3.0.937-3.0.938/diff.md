# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.937.tar", last modified: Tue Jul 18 00:34:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.938.tar", last modified: Wed Jul 19 00:52:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.937.tar` & `tencentcloud-sdk-python-trp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)    45620 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   244909 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:00.000000 tencentcloud-sdk-python-trp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)    45820 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   244909 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:52:39.000000 tencentcloud-sdk-python-trp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-trp-3.0.937/setup.py` & `tencentcloud-sdk-python-trp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.937/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.938/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/trp_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AuthorizedTransferResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCodeBatch(self, request):
         """新增批次
 
         :param request: Request instance for CreateCodeBatch.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCodeBatchRequest`
@@ -65,15 +65,15 @@
             model = models.CreateCodeBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCodePack(self, request):
         """生成普通码包
 
         :param request: Request instance for CreateCodePack.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCodePackRequest`
@@ -88,15 +88,15 @@
             model = models.CreateCodePackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCorporationOrder(self, request):
         """以订单方式新建企业信息/配额信息
 
         :param request: Request instance for CreateCorporationOrder.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCorporationOrderRequest`
@@ -111,15 +111,15 @@
             model = models.CreateCorporationOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomPack(self, request):
         """生成自定义码包
 
         :param request: Request instance for CreateCustomPack.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCustomPackRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCustomPackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomRule(self, request):
         """新建自定义码规则
 
         :param request: Request instance for CreateCustomRule.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCustomRuleRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCustomRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMerchant(self, request):
         """新建商户
 
         :param request: Request instance for CreateMerchant.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateMerchantRequest`
@@ -180,15 +180,15 @@
             model = models.CreateMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
         """新建商品
 
         :param request: Request instance for CreateProduct.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateProductRequest`
@@ -203,15 +203,15 @@
             model = models.CreateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTraceChain(self, request):
         """上链溯源信息
 
         :param request: Request instance for CreateTraceChain.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateTraceChainRequest`
@@ -226,15 +226,15 @@
             model = models.CreateTraceChainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTraceCodes(self, request):
         """批量绑定指定批次并激活二维码，只支持平台发的码，且只会激活没有使用过的码
 
         :param request: Request instance for CreateTraceCodes.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateTraceCodesRequest`
@@ -249,15 +249,15 @@
             model = models.CreateTraceCodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTraceCodesAsync(self, request):
         """异步导入激活码包，如果是第三方码包，需要域名跟配置的匹配
 
         :param request: Request instance for CreateTraceCodesAsync.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateTraceCodesAsyncRequest`
@@ -272,15 +272,15 @@
             model = models.CreateTraceCodesAsyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTraceData(self, request):
         """新增溯源信息
 
         :param request: Request instance for CreateTraceData.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateTraceDataRequest`
@@ -295,15 +295,15 @@
             model = models.CreateTraceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCodeBatch(self, request):
         """删除批次
 
         :param request: Request instance for DeleteCodeBatch.
         :type request: :class:`tencentcloud.trp.v20210515.models.DeleteCodeBatchRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteCodeBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMerchant(self, request):
         """删除商户
 
         :param request: Request instance for DeleteMerchant.
         :type request: :class:`tencentcloud.trp.v20210515.models.DeleteMerchantRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProduct(self, request):
         """删除商品，如果商品被使用，则不可删除
 
         :param request: Request instance for DeleteProduct.
         :type request: :class:`tencentcloud.trp.v20210515.models.DeleteProductRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTraceData(self, request):
         """删除溯源信息，如果已经上链则不可删除
 
         :param request: Request instance for DeleteTraceData.
         :type request: :class:`tencentcloud.trp.v20210515.models.DeleteTraceDataRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteTraceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentCorps(self, request):
         """查询渠道企业列表
 
         :param request: Request instance for DescribeAgentCorps.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeAgentCorpsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeAgentCorpsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodeBatchById(self, request):
         """查询批次信息
 
         :param request: Request instance for DescribeCodeBatchById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodeBatchByIdRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeCodeBatchByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodeBatchs(self, request):
         """查询批次列表
 
         :param request: Request instance for DescribeCodeBatchs.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodeBatchsRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeCodeBatchsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodePackStatus(self, request):
         """查询码包状态
 
         :param request: Request instance for DescribeCodePackStatus.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodePackStatusRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeCodePackStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodePackUrl(self, request):
         """查询码包地址
 
         :param request: Request instance for DescribeCodePackUrl.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodePackUrlRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeCodePackUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodePacks(self, request):
         """查询码包列表
 
         :param request: Request instance for DescribeCodePacks.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodePacksRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeCodePacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodesByPack(self, request):
         """查询码包的二维码列表，上限 3 万
 
         :param request: Request instance for DescribeCodesByPack.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCodesByPackRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeCodesByPackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCorpQuotas(self, request):
         """查询渠道商下属企业额度使用情况
 
         :param request: Request instance for DescribeCorpQuotas.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCorpQuotasRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeCorpQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomRuleById(self, request):
         """查自定义码规则
 
         :param request: Request instance for DescribeCustomRuleById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCustomRuleByIdRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeCustomRuleByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomRules(self, request):
         """查自定义码规则列表
 
         :param request: Request instance for DescribeCustomRules.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeCustomRulesRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeCustomRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobFileUrl(self, request):
         """获取异步任务的输出地址
 
         :param request: Request instance for DescribeJobFileUrl.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeJobFileUrlRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeJobFileUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMerchantById(self, request):
         """查询商户信息
 
         :param request: Request instance for DescribeMerchantById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeMerchantByIdRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeMerchantByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMerchants(self, request):
         """查询商户列表
 
         :param request: Request instance for DescribeMerchants.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeMerchantsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeMerchantsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductById(self, request):
         """查询商品信息
 
         :param request: Request instance for DescribeProductById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeProductByIdRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeProductByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProducts(self, request):
         """查询商品列表
 
         :param request: Request instance for DescribeProducts.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeProductsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRawScanLogs(self, request):
         """支持增量查询扫码日志，通常提供给数据同步使用，调用时需要指定从哪一行开始查询数据
 
         :param request: Request instance for DescribeRawScanLogs.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeRawScanLogsRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeRawScanLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanLogs(self, request):
         """查询扫码日志明细
 
         :param request: Request instance for DescribeScanLogs.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeScanLogsRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeScanLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanStats(self, request):
         """查询扫码的统计信息列表，支持按照商户ID，产品ID，批次ID，安心码筛选，筛选条件至少有一个
         没有被扫过的不会返回
 
         :param request: Request instance for DescribeScanStats.
@@ -802,15 +802,15 @@
             model = models.DescribeScanStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTmpToken(self, request):
         """查询临时Token，主要用于上传接口
 
         :param request: Request instance for DescribeTmpToken.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTmpTokenRequest`
@@ -825,15 +825,15 @@
             model = models.DescribeTmpTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTraceCodeById(self, request):
         """查询二维码信息
 
         :param request: Request instance for DescribeTraceCodeById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceCodeByIdRequest`
@@ -848,15 +848,15 @@
             model = models.DescribeTraceCodeByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTraceCodes(self, request):
         """查询二维码列表
 
         :param request: Request instance for DescribeTraceCodes.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceCodesRequest`
@@ -871,15 +871,15 @@
             model = models.DescribeTraceCodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTraceDataById(self, request):
         """查询溯源ID查溯源信息，通常溯源信息跟生产批次绑定，即一个批次的所有溯源信息都是一样的
 
         :param request: Request instance for DescribeTraceDataById.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataByIdRequest`
@@ -894,15 +894,15 @@
             model = models.DescribeTraceDataByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTraceDataList(self, request):
         """查询溯源信息，通常溯源信息跟生产批次绑定，即一个批次的所有溯源信息都是一样的
 
         :param request: Request instance for DescribeTraceDataList.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataListRequest`
@@ -917,15 +917,15 @@
             model = models.DescribeTraceDataListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EffectFeedback(self, request):
         """接收客户反馈的各环节数据
 
         :param request: Request instance for EffectFeedback.
         :type request: :class:`tencentcloud.trp.v20210515.models.EffectFeedbackRequest`
@@ -940,15 +940,15 @@
             model = models.EffectFeedbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCodeBatch(self, request):
         """修改批次
 
         :param request: Request instance for ModifyCodeBatch.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyCodeBatchRequest`
@@ -963,15 +963,15 @@
             model = models.ModifyCodeBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomRule(self, request):
         """修改自定义码规则
 
         :param request: Request instance for ModifyCustomRule.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyCustomRuleRequest`
@@ -986,15 +986,15 @@
             model = models.ModifyCustomRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomRuleStatus(self, request):
         """更新自定义码规则状态
 
         :param request: Request instance for ModifyCustomRuleStatus.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyCustomRuleStatusRequest`
@@ -1009,15 +1009,15 @@
             model = models.ModifyCustomRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMerchant(self, request):
         """编辑商户
 
         :param request: Request instance for ModifyMerchant.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyMerchantRequest`
@@ -1032,15 +1032,15 @@
             model = models.ModifyMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProduct(self, request):
         """编辑商品
 
         :param request: Request instance for ModifyProduct.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyProductRequest`
@@ -1055,15 +1055,15 @@
             model = models.ModifyProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTraceCode(self, request):
         """冻结或者激活二维码，所属的批次的冻结状态优先级大于单个二维码的状态，即如果批次是冻结的，那么该批次下二维码的状态都是冻结的
 
         :param request: Request instance for ModifyTraceCode.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyTraceCodeRequest`
@@ -1078,15 +1078,15 @@
             model = models.ModifyTraceCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTraceCodeUnlink(self, request):
         """解绑溯源码和批次的关系，让溯源码重置为未关联的状态，以便关联其他批次
         注意：溯源码必须属于指定的批次才会解绑
 
         :param request: Request instance for ModifyTraceCodeUnlink.
@@ -1102,15 +1102,15 @@
             model = models.ModifyTraceCodeUnlinkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTraceData(self, request):
         """修改溯源信息
 
         :param request: Request instance for ModifyTraceData.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyTraceDataRequest`
@@ -1125,15 +1125,15 @@
             model = models.ModifyTraceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTraceDataRanks(self, request):
         """修改溯源信息的排序
 
         :param request: Request instance for ModifyTraceDataRanks.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyTraceDataRanksRequest`
@@ -1148,15 +1148,15 @@
             model = models.ModifyTraceDataRanksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportBatchCallbackStatus(self, request):
         """接收离线筛选包回执，用于效果统计和分析。
 
         :param request: Request instance for ReportBatchCallbackStatus.
         :type request: :class:`tencentcloud.trp.v20210515.models.ReportBatchCallbackStatusRequest`
@@ -1171,8 +1171,8 @@
             model = models.ReportBatchCallbackStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.937/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.938/tencentcloud/trp/v20210515/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.937/README.rst` & `tencentcloud-sdk-python-trp-3.0.938/README.rst`

 * *Files identical despite different names*

