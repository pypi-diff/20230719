# Comparing `tmp/tencentcloud-sdk-python-cws-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cws-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cws-3.0.937.tar", last modified: Tue Jul 18 00:21:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cws-3.0.938.tar", last modified: Wed Jul 19 00:36:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cws-3.0.937.tar` & `tencentcloud-sdk-python-cws-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/
--rw-r--r--   0 root         (0) root         (0)    18517 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/cws_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92049 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:21:44.000000 tencentcloud-sdk-python-cws-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/
+-rw-r--r--   0 root         (0) root         (0)    18593 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/cws_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92049 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:36:55.000000 tencentcloud-sdk-python-cws-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cws-3.0.937/setup.py` & `tencentcloud-sdk-python-cws-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.937/tencentcloud_sdk_python_cws.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cws-3.0.938/tencentcloud_sdk_python_cws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cws
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cws SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/cws_client.py` & `tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/cws_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateMonitorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSites(self, request):
         """本接口（CreateSites）用于新增一个或多个站点。
 
         :param request: Request instance for CreateSites.
         :type request: :class:`tencentcloud.cws.v20180312.models.CreateSitesRequest`
@@ -65,15 +65,15 @@
             model = models.CreateSitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSitesScans(self, request):
         """本接口（CreateSitesScans）用于新增一个或多个站点的单次扫描任务。
 
         :param request: Request instance for CreateSitesScans.
         :type request: :class:`tencentcloud.cws.v20180312.models.CreateSitesScansRequest`
@@ -88,15 +88,15 @@
             model = models.CreateSitesScansResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulsMisinformation(self, request):
         """本接口（CreateVulsMisinformation）可以用于新增一个或多个漏洞误报信息。
 
         :param request: Request instance for CreateVulsMisinformation.
         :type request: :class:`tencentcloud.cws.v20180312.models.CreateVulsMisinformationRequest`
@@ -111,15 +111,15 @@
             model = models.CreateVulsMisinformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulsReport(self, request):
         """本接口 (CreateVulsReport) 用于生成漏洞报告并返回下载链接。
 
         :param request: Request instance for CreateVulsReport.
         :type request: :class:`tencentcloud.cws.v20180312.models.CreateVulsReportRequest`
@@ -134,15 +134,15 @@
             model = models.CreateVulsReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMonitors(self, request):
         """本接口 (DeleteMonitors) 用于删除用户监控任务。
 
         :param request: Request instance for DeleteMonitors.
         :type request: :class:`tencentcloud.cws.v20180312.models.DeleteMonitorsRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteMonitorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSites(self, request):
         """本接口 (DeleteSites) 用于删除站点。
 
         :param request: Request instance for DeleteSites.
         :type request: :class:`tencentcloud.cws.v20180312.models.DeleteSitesRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteSitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfig(self, request):
         """本接口 (DescribeConfig) 用于查询用户配置的详细信息。
 
         :param request: Request instance for DescribeConfig.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeConfigRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonitors(self, request):
         """本接口 (DescribeMonitors) 用于查询一个或多个监控任务的详细信息。
 
         :param request: Request instance for DescribeMonitors.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeMonitorsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeMonitorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSiteQuota(self, request):
         """本接口 (DescribeSiteQuota) 用于查询用户购买的扫描次数总数和已使用数。
 
         :param request: Request instance for DescribeSiteQuota.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeSiteQuotaRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeSiteQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSites(self, request):
         """本接口 (DescribeSites) 用于查询一个或多个站点的详细信息。
 
         :param request: Request instance for DescribeSites.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeSitesRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeSitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSitesVerification(self, request):
         """本接口 (DescribeSitesVerification) 用于查询一个或多个待验证站点的验证信息。
 
         :param request: Request instance for DescribeSitesVerification.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeSitesVerificationRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeSitesVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVuls(self, request):
         """本接口 (DescribeVuls) 用于查询一个或多个漏洞的详细信息。
 
         :param request: Request instance for DescribeVuls.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeVulsRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeVulsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulsNumber(self, request):
         """本接口 (DescribeVulsNumber) 用于查询用户网站的漏洞总计数量。
 
         :param request: Request instance for DescribeVulsNumber.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeVulsNumberRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeVulsNumberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulsNumberTimeline(self, request):
         """本接口 (DescribeVulsNumberTimeline) 用于查询漏洞数随时间变化统计信息。
 
         :param request: Request instance for DescribeVulsNumberTimeline.
         :type request: :class:`tencentcloud.cws.v20180312.models.DescribeVulsNumberTimelineRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeVulsNumberTimelineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConfigAttribute(self, request):
         """本接口 (ModifyConfigAttribute) 用于修改用户配置的属性。
 
         :param request: Request instance for ModifyConfigAttribute.
         :type request: :class:`tencentcloud.cws.v20180312.models.ModifyConfigAttributeRequest`
@@ -387,15 +387,15 @@
             model = models.ModifyConfigAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMonitorAttribute(self, request):
         """本接口 (ModifyMonitorAttribute) 用于修改监测任务的属性。
 
         :param request: Request instance for ModifyMonitorAttribute.
         :type request: :class:`tencentcloud.cws.v20180312.models.ModifyMonitorAttributeRequest`
@@ -410,15 +410,15 @@
             model = models.ModifyMonitorAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySiteAttribute(self, request):
         """本接口 (ModifySiteAttribute) 用于修改站点的属性。
 
         :param request: Request instance for ModifySiteAttribute.
         :type request: :class:`tencentcloud.cws.v20180312.models.ModifySiteAttributeRequest`
@@ -433,15 +433,15 @@
             model = models.ModifySiteAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifySites(self, request):
         """本接口 (VerifySites) 用于验证一个或多个待验证站点。
 
         :param request: Request instance for VerifySites.
         :type request: :class:`tencentcloud.cws.v20180312.models.VerifySitesRequest`
@@ -456,8 +456,8 @@
             model = models.VerifySitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/errorcodes.py` & `tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.937/tencentcloud/cws/v20180312/models.py` & `tencentcloud-sdk-python-cws-3.0.938/tencentcloud/cws/v20180312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cws-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cws-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cws-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cws
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cws SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cws-3.0.937/README.rst` & `tencentcloud-sdk-python-cws-3.0.938/README.rst`

 * *Files identical despite different names*

