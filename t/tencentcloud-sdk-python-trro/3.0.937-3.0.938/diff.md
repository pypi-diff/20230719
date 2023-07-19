# Comparing `tmp/tencentcloud-sdk-python-trro-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-trro-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.937.tar", last modified: Tue Jul 18 00:34:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.938.tar", last modified: Wed Jul 19 00:52:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trro-3.0.937.tar` & `tencentcloud-sdk-python-trro-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/
--rw-r--r--   0 root         (0) root         (0)    21281 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/trro_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   103053 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/
+-rw-r--r--   0 root         (0) root         (0)    21373 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/trro_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   103053 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:52:45.000000 tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trro-3.0.937/setup.py` & `tencentcloud-sdk-python-trro-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/trro_client.py` & `tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/trro_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchDeleteDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeletePolicy(self, request):
         """用于批量删除修改权限配置
 
         :param request: Request instance for BatchDeletePolicy.
         :type request: :class:`tencentcloud.trro.v20220325.models.BatchDeletePolicyRequest`
@@ -65,15 +65,15 @@
             model = models.BatchDeletePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BoundLicenses(self, request):
         """为推流设备绑定license，优先绑定到期时间最近的，到期时间相同优先绑定月包
 
         :param request: Request instance for BoundLicenses.
         :type request: :class:`tencentcloud.trro.v20220325.models.BoundLicensesRequest`
@@ -88,15 +88,15 @@
             model = models.BoundLicensesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDevice(self, request):
         """用于创建设备
 
         :param request: Request instance for CreateDevice.
         :type request: :class:`tencentcloud.trro.v20220325.models.CreateDeviceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """用于创建项目
 
         :param request: Request instance for CreateProject.
         :type request: :class:`tencentcloud.trro.v20220325.models.CreateProjectRequest`
@@ -134,15 +134,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProject(self, request):
         """用于删除项目
 
         :param request: Request instance for DeleteProject.
         :type request: :class:`tencentcloud.trro.v20220325.models.DeleteProjectRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceInfo(self, request):
         """用于获取指定设备信息
 
         :param request: Request instance for DescribeDeviceInfo.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeDeviceInfoRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeDeviceInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceList(self, request):
         """用于获取设备信息列表
 
         :param request: Request instance for DescribeDeviceList.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeDeviceListRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeDeviceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceSessionDetails(self, request):
         """获取设备会话数据详单
 
         :param request: Request instance for DescribeDeviceSessionDetails.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeDeviceSessionDetailsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeDeviceSessionDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceSessionList(self, request):
         """获取设备会话列表
 
         :param request: Request instance for DescribeDeviceSessionList.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeDeviceSessionListRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeDeviceSessionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicy(self, request):
         """用于查看权限配置
 
         :param request: Request instance for DescribePolicy.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribePolicyRequest`
@@ -272,15 +272,15 @@
             model = models.DescribePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectInfo(self, request):
         """用于获取项目信息
 
         :param request: Request instance for DescribeProjectInfo.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeProjectInfoRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeProjectInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectList(self, request):
         """用于获取项目列表
 
         :param request: Request instance for DescribeProjectList.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeProjectListRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeProjectListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecentSessionList(self, request):
         """获取最新设备会话列表
 
         :param request: Request instance for DescribeRecentSessionList.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeRecentSessionListRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeRecentSessionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSessionStatistics(self, request):
         """获取会话统计值
 
         :param request: Request instance for DescribeSessionStatistics.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeSessionStatisticsRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeSessionStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSessionStatisticsByInterval(self, request):
         """获取各时间段的会话统计值
 
         :param request: Request instance for DescribeSessionStatisticsByInterval.
         :type request: :class:`tencentcloud.trro.v20220325.models.DescribeSessionStatisticsByIntervalRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeSessionStatisticsByIntervalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceLicense(self, request):
         """获取设备已经绑定的可用授权数量
 
         :param request: Request instance for GetDeviceLicense.
         :type request: :class:`tencentcloud.trro.v20220325.models.GetDeviceLicenseRequest`
@@ -410,15 +410,15 @@
             model = models.GetDeviceLicenseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDevices(self, request):
         """查询用户设备的授权绑定情况
 
         :param request: Request instance for GetDevices.
         :type request: :class:`tencentcloud.trro.v20220325.models.GetDevicesRequest`
@@ -433,15 +433,15 @@
             model = models.GetDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLicenseStat(self, request):
         """统计license类型数量
 
         :param request: Request instance for GetLicenseStat.
         :type request: :class:`tencentcloud.trro.v20220325.models.GetLicenseStatRequest`
@@ -456,15 +456,15 @@
             model = models.GetLicenseStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLicenses(self, request):
         """按授权查看license列表
 
         :param request: Request instance for GetLicenses.
         :type request: :class:`tencentcloud.trro.v20220325.models.GetLicensesRequest`
@@ -479,15 +479,15 @@
             model = models.GetLicensesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDevice(self, request):
         """用于修改设备信息
 
         :param request: Request instance for ModifyDevice.
         :type request: :class:`tencentcloud.trro.v20220325.models.ModifyDeviceRequest`
@@ -502,15 +502,15 @@
             model = models.ModifyDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPolicy(self, request):
         """用于修改权限配置
 
         :param request: Request instance for ModifyPolicy.
         :type request: :class:`tencentcloud.trro.v20220325.models.ModifyPolicyRequest`
@@ -525,15 +525,15 @@
             model = models.ModifyPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProject(self, request):
         """用于修改项目信息
 
         :param request: Request instance for ModifyProject.
         :type request: :class:`tencentcloud.trro.v20220325.models.ModifyProjectRequest`
@@ -548,8 +548,8 @@
             model = models.ModifyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/errorcodes.py` & `tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/models.py` & `tencentcloud-sdk-python-trro-3.0.938/tencentcloud/trro/v20220325/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trro-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trro-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.938/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trro-3.0.937/README.rst` & `tencentcloud-sdk-python-trro-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.938/tencentcloud_sdk_python_trro.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

