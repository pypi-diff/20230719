# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.937.tar", last modified: Tue Jul 18 00:17:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.938.tar", last modified: Wed Jul 19 00:21:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.937.tar` & `tencentcloud-sdk-python-billing-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)    21124 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   276129 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:17:47.000000 tencentcloud-sdk-python-billing-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)    21208 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   276129 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:21:50.000000 tencentcloud-sdk-python-billing-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-billing-3.0.937/setup.py` & `tencentcloud-sdk-python-billing-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/billing_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillDetail(self, request):
         """查询账单明细数据。
         注意事项：
         1.在请求接口时，由于网络不稳定或其它异常，可能会导致请求失败。如果您遇到这种情况，我们建议您在接口请求失败时，手动发起重试操作，这样可以更好地确保您的接口请求能够成功执行。
         2.对于账单明细数据量级很大（例如每月账单明细量级超过20w）的客户，通过 API 调用账单数据效率较低，建议您开通账单数据存储功能，通过存储桶中获取账单文件进行分析。[账单存储至COS桶](https://cloud.tencent.com/document/product/555/61275)
@@ -68,15 +68,15 @@
             model = models.DescribeBillDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillList(self, request):
         """获取收支明细列表，支持翻页和参数过滤
 
         :param request: Request instance for DescribeBillList.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillListRequest`
@@ -91,15 +91,15 @@
             model = models.DescribeBillListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillResourceSummary(self, request):
         """查询账单资源汇总数据
 
         :param request: Request instance for DescribeBillResourceSummary.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillResourceSummaryRequest`
@@ -114,15 +114,15 @@
             model = models.DescribeBillResourceSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummary(self, request):
         """该接口支持通过传参，按照产品、项目、地域、计费模式和标签五个维度获取账单费用明细。
 
         :param request: Request instance for DescribeBillSummary.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryRequest`
@@ -137,15 +137,15 @@
             model = models.DescribeBillSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummaryByPayMode(self, request):
         """获取按计费模式汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByPayMode.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByPayModeRequest`
@@ -160,15 +160,15 @@
             model = models.DescribeBillSummaryByPayModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummaryByProduct(self, request):
         """获取产品汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByProduct.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByProductRequest`
@@ -183,15 +183,15 @@
             model = models.DescribeBillSummaryByProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummaryByProject(self, request):
         """获取按项目汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByProject.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByProjectRequest`
@@ -206,15 +206,15 @@
             model = models.DescribeBillSummaryByProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummaryByRegion(self, request):
         """获取按地域汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByRegion.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByRegionRequest`
@@ -229,15 +229,15 @@
             model = models.DescribeBillSummaryByRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillSummaryByTag(self, request):
         """获取按标签汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByTag.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByTagRequest`
@@ -252,15 +252,15 @@
             model = models.DescribeBillSummaryByTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCostDetail(self, request):
         """查询消耗明细
 
         :param request: Request instance for DescribeCostDetail.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeCostDetailRequest`
@@ -275,15 +275,15 @@
             model = models.DescribeCostDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCostSummaryByProduct(self, request):
         """获取按产品汇总消耗详情
 
         :param request: Request instance for DescribeCostSummaryByProduct.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeCostSummaryByProductRequest`
@@ -298,15 +298,15 @@
             model = models.DescribeCostSummaryByProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCostSummaryByProject(self, request):
         """获取按项目汇总消耗详情
 
         :param request: Request instance for DescribeCostSummaryByProject.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeCostSummaryByProjectRequest`
@@ -321,15 +321,15 @@
             model = models.DescribeCostSummaryByProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCostSummaryByRegion(self, request):
         """获取按地域汇总消耗详情
 
         :param request: Request instance for DescribeCostSummaryByRegion.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeCostSummaryByRegionRequest`
@@ -344,15 +344,15 @@
             model = models.DescribeCostSummaryByRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCostSummaryByResource(self, request):
         """获取按资源汇总消耗详情
 
         :param request: Request instance for DescribeCostSummaryByResource.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeCostSummaryByResourceRequest`
@@ -367,15 +367,15 @@
             model = models.DescribeCostSummaryByResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDealsByCond(self, request):
         """查询订单
 
         :param request: Request instance for DescribeDealsByCond.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeDealsByCondRequest`
@@ -390,15 +390,15 @@
             model = models.DescribeDealsByCondResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDosageCosDetailByDate(self, request):
         """获取COS产品用量明细
 
         :param request: Request instance for DescribeDosageCosDetailByDate.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeDosageCosDetailByDateRequest`
@@ -413,15 +413,15 @@
             model = models.DescribeDosageCosDetailByDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDosageDetailByDate(self, request):
         """按日期获取产品用量明细
 
         :param request: Request instance for DescribeDosageDetailByDate.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeDosageDetailByDateRequest`
@@ -436,15 +436,15 @@
             model = models.DescribeDosageDetailByDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVoucherInfo(self, request):
         """获取代金券相关信息
 
         :param request: Request instance for DescribeVoucherInfo.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeVoucherInfoRequest`
@@ -459,15 +459,15 @@
             model = models.DescribeVoucherInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVoucherUsageDetails(self, request):
         """获取代金券使用记录
 
         :param request: Request instance for DescribeVoucherUsageDetails.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeVoucherUsageDetailsRequest`
@@ -482,15 +482,15 @@
             model = models.DescribeVoucherUsageDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PayDeals(self, request):
         """支付订单
 
         :param request: Request instance for PayDeals.
         :type request: :class:`tencentcloud.billing.v20180709.models.PayDealsRequest`
@@ -505,8 +505,8 @@
             model = models.PayDealsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.937/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.938/tencentcloud/billing/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.937/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.938/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.937/README.rst` & `tencentcloud-sdk-python-billing-3.0.938/README.rst`

 * *Files identical despite different names*

