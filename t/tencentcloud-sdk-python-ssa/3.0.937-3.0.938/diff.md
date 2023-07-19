# Comparing `tmp/tencentcloud-sdk-python-ssa-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ssa-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.937.tar", last modified: Tue Jul 18 00:30:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.938.tar", last modified: Wed Jul 19 00:45:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssa-3.0.937.tar` & `tencentcloud-sdk-python-ssa-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    22638 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/ssa_client.py
--rw-r--r--   0 root         (0) root         (0)   280205 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:15.000000 tencentcloud-sdk-python-ssa-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/ssa_client.py
+-rw-r--r--   0 root         (0) root         (0)   280205 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:45:28.000000 tencentcloud-sdk-python-ssa-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/setup.py` & `tencentcloud-sdk-python-ssa-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/errorcodes.py` & `tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/ssa_client.py` & `tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/ssa_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeAssetDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetDetailList(self, request):
         """资产条件查询
 
         :param request: Request instance for DescribeAssetDetailList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeAssetDetailListRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeAssetDetailListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetList(self, request):
         """资产安全资产列表
 
         :param request: Request instance for DescribeAssetList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeAssetListRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetsMappingList(self, request):
         """资产测绘-测绘列表
 
         :param request: Request instance for DescribeAssetsMappingList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeAssetsMappingListRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeAssetsMappingListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCheckConfigAssetList(self, request):
         """云安全配置管理资产组列表
 
         :param request: Request instance for DescribeCheckConfigAssetList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeCheckConfigAssetListRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeCheckConfigAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCheckConfigDetail(self, request):
         """云安全配置检查项详情
 
         :param request: Request instance for DescribeCheckConfigDetail.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeCheckConfigDetailRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeCheckConfigDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceAssetList(self, request):
         """合规管理-资产列表
 
         :param request: Request instance for DescribeComplianceAssetList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeComplianceAssetListRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeComplianceAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceDetail(self, request):
         """合规管理检查项详情
 
         :param request: Request instance for DescribeComplianceDetail.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeComplianceDetailRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeComplianceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceList(self, request):
         """合规管理总览页检查项列表
 
         :param request: Request instance for DescribeComplianceList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeComplianceListRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeComplianceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigList(self, request):
         """云配置检查项总览页检查项列表
 
         :param request: Request instance for DescribeConfigList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeConfigListRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeConfigListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainList(self, request):
         """域名列表信息
 
         :param request: Request instance for DescribeDomainList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeDomainListRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeDomainListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEventDetail(self, request):
         """获取安全事件详情
 
         :param request: Request instance for DescribeEventDetail.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeEventDetailRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeEventDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLeakDetectionList(self, request):
         """获取泄露列表
 
         :param request: Request instance for DescribeLeakDetectionList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeLeakDetectionListRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeLeakDetectionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMappingResults(self, request):
         """获取测绘列表
 
         :param request: Request instance for DescribeMappingResults.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeMappingResultsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeMappingResultsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSafetyEventList(self, request):
         """获取安全事件列表
 
         :param request: Request instance for DescribeSafetyEventList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSafetyEventListRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeSafetyEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSocAlertDetails(self, request):
         """返回告警详情
 
         :param request: Request instance for DescribeSocAlertDetails.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSocAlertDetailsRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeSocAlertDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSocAlertList(self, request):
         """拉取告警列表
 
         :param request: Request instance for DescribeSocAlertList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSocAlertListRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeSocAlertListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSocCheckItemList(self, request):
         """云安全配置检查项列表
 
         :param request: Request instance for DescribeSocCheckItemList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSocCheckItemListRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeSocCheckItemListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSocCheckResultList(self, request):
         """云安全配置检查项结果列表
 
         :param request: Request instance for DescribeSocCheckResultList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSocCheckResultListRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeSocCheckResultListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSocCspmCompliance(self, request):
         """合规详情项
 
         :param request: Request instance for DescribeSocCspmCompliance.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeSocCspmComplianceRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeSocCspmComplianceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDetail(self, request):
         """漏洞列表页，获取漏洞详情信息
 
         :param request: Request instance for DescribeVulDetail.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeVulDetailRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeVulDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulList(self, request):
         """漏洞管理页，获取漏洞列表
 
         :param request: Request instance for DescribeVulList.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeVulListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SaDivulgeDataQueryPub(self, request):
         """查询【通用字段】【泄露监测数据列表】
 
         :param request: Request instance for SaDivulgeDataQueryPub.
         :type request: :class:`tencentcloud.ssa.v20180608.models.SaDivulgeDataQueryPubRequest`
@@ -548,15 +548,15 @@
             model = models.SaDivulgeDataQueryPubResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SaEventPub(self, request):
         """安全事件通用字段
 
         :param request: Request instance for SaEventPub.
         :type request: :class:`tencentcloud.ssa.v20180608.models.SaEventPubRequest`
@@ -571,8 +571,8 @@
             model = models.SaEventPubResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/tencentcloud/ssa/v20180608/models.py` & `tencentcloud-sdk-python-ssa-3.0.938/tencentcloud/ssa/v20180608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.938/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.937/README.rst` & `tencentcloud-sdk-python-ssa-3.0.938/README.rst`

 * *Files identical despite different names*

