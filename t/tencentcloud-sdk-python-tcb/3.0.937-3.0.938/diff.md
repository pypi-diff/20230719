# Comparing `tmp/tencentcloud-sdk-python-tcb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.937.tar", last modified: Tue Jul 18 00:31:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.938.tar", last modified: Wed Jul 19 00:48:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcb-3.0.937.tar` & `tencentcloud-sdk-python-tcb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    83901 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/tcb_client.py
--rw-r--r--   0 root         (0) root         (0)   549868 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:23.000000 tencentcloud-sdk-python-tcb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    84257 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/tcb_client.py
+-rw-r--r--   0 root         (0) root         (0)   549868 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:48.000000 tencentcloud-sdk-python-tcb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/setup.py` & `tencentcloud-sdk-python-tcb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/errorcodes.py` & `tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/tcb_client.py` & `tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/tcb_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindEnvGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckTcbService(self, request):
         """检查是否开通Tcb服务
 
         :param request: Request instance for CheckTcbService.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CheckTcbServiceRequest`
@@ -65,15 +65,15 @@
             model = models.CheckTcbServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommonServiceAPI(self, request):
         """TCB云API统一入口
 
         :param request: Request instance for CommonServiceAPI.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CommonServiceAPIRequest`
@@ -88,15 +88,15 @@
             model = models.CommonServiceAPIResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAndDeployCloudBaseProject(self, request):
         """创建云开发项目
 
         :param request: Request instance for CreateAndDeployCloudBaseProject.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateAndDeployCloudBaseProjectRequest`
@@ -111,15 +111,15 @@
             model = models.CreateAndDeployCloudBaseProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAuthDomain(self, request):
         """增加安全域名
 
         :param request: Request instance for CreateAuthDomain.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateAuthDomainRequest`
@@ -134,15 +134,15 @@
             model = models.CreateAuthDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudBaseRunResource(self, request):
         """开通容器托管的资源，包括集群创建，VPC配置，异步任务创建，镜像托管，Coding等，查看创建结果需要根据DescribeCloudBaseRunResource接口来查看
 
         :param request: Request instance for CreateCloudBaseRunResource.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateCloudBaseRunResourceRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCloudBaseRunResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudBaseRunServerVersion(self, request):
         """创建服务版本
 
         :param request: Request instance for CreateCloudBaseRunServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateCloudBaseRunServerVersionRequest`
@@ -180,15 +180,15 @@
             model = models.CreateCloudBaseRunServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHostingDomain(self, request):
         """创建托管域名
 
         :param request: Request instance for CreateHostingDomain.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateHostingDomainRequest`
@@ -203,15 +203,15 @@
             model = models.CreateHostingDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePostpayPackage(self, request):
         """开通后付费资源
 
         :param request: Request instance for CreatePostpayPackage.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreatePostpayPackageRequest`
@@ -226,15 +226,15 @@
             model = models.CreatePostpayPackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStandaloneGateway(self, request):
         """本接口（CreateStandaloneGateway）用于创建独立网关。
 
         :param request: Request instance for CreateStandaloneGateway.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateStandaloneGatewayRequest`
@@ -249,15 +249,15 @@
             model = models.CreateStandaloneGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStaticStore(self, request):
         """创建静态托管资源，包括COS和CDN，异步任务创建，查看创建结果需要根据DescribeStaticStore接口来查看
 
         :param request: Request instance for CreateStaticStore.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateStaticStoreRequest`
@@ -272,15 +272,15 @@
             model = models.CreateStaticStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWxCloudBaseRunEnv(self, request):
         """创建微信云托管
 
         :param request: Request instance for CreateWxCloudBaseRunEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateWxCloudBaseRunEnvRequest`
@@ -295,15 +295,15 @@
             model = models.CreateWxCloudBaseRunEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWxCloudBaseRunServerDBCluster(self, request):
         """开通微信云托管MySQL数据库服务
 
         :param request: Request instance for CreateWxCloudBaseRunServerDBCluster.
         :type request: :class:`tencentcloud.tcb.v20180608.models.CreateWxCloudBaseRunServerDBClusterRequest`
@@ -318,15 +318,15 @@
             model = models.CreateWxCloudBaseRunServerDBClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudBaseProjectLatestVersion(self, request):
         """删除云项目
 
         :param request: Request instance for DeleteCloudBaseProjectLatestVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteCloudBaseProjectLatestVersionRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteCloudBaseProjectLatestVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudBaseRunServerVersion(self, request):
         """删除服务版本
 
         :param request: Request instance for DeleteCloudBaseRunServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteCloudBaseRunServerVersionRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteCloudBaseRunServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEndUser(self, request):
         """删除终端用户
 
         :param request: Request instance for DeleteEndUser.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteEndUserRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteEndUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGatewayVersion(self, request):
         """删除网关某版本
 
         :param request: Request instance for DeleteGatewayVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteGatewayVersionRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteGatewayVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWxGatewayRoute(self, request):
         """删除安全网关路由
 
         :param request: Request instance for DeleteWxGatewayRoute.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteWxGatewayRouteRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteWxGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeActivityInfo(self, request):
         """查询活动信息
 
         :param request: Request instance for DescribeActivityInfo.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeActivityInfoRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeActivityInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeActivityRecord(self, request):
         """查询活动记录信息
 
         :param request: Request instance for DescribeActivityRecord.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeActivityRecordRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeActivityRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuthDomains(self, request):
         """获取安全域名列表
 
         :param request: Request instance for DescribeAuthDomains.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeAuthDomainsRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeAuthDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBaasPackageList(self, request):
         """获取新套餐列表，含详情，如果传了PackageId，则只获取指定套餐详情
 
         :param request: Request instance for DescribeBaasPackageList.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeBaasPackageListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeBaasPackageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillingInfo(self, request):
         """获取计费相关信息
 
         :param request: Request instance for DescribeBillingInfo.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeBillingInfoRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeBillingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCbrServerVersion(self, request):
         """查询服务版本的详情
 
         :param request: Request instance for DescribeCbrServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCbrServerVersionRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeCbrServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseBuildService(self, request):
         """获取云托管代码上传url
 
         :param request: Request instance for DescribeCloudBaseBuildService.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseBuildServiceRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeCloudBaseBuildServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseProjectLatestVersionList(self, request):
         """获取云开发项目列表
 
         :param request: Request instance for DescribeCloudBaseProjectLatestVersionList.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseProjectLatestVersionListRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeCloudBaseProjectLatestVersionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseProjectVersionList(self, request):
         """云项目部署列表
 
         :param request: Request instance for DescribeCloudBaseProjectVersionList.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseProjectVersionListRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeCloudBaseProjectVersionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunAllVpcs(self, request):
         """查询环境下所有的vpc列表
 
         :param request: Request instance for DescribeCloudBaseRunAllVpcs.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunAllVpcsRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeCloudBaseRunAllVpcsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunConfForGateWay(self, request):
         """独立网关中拉取云托管服务对应的配置信息
 
         :param request: Request instance for DescribeCloudBaseRunConfForGateWay.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunConfForGateWayRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeCloudBaseRunConfForGateWayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunOneClickTaskExternal(self, request):
         """查询一键部署任务 （特定接口：外部查询使用）
 
         :param request: Request instance for DescribeCloudBaseRunOneClickTaskExternal.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunOneClickTaskExternalRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeCloudBaseRunOneClickTaskExternalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunOperationTypes(self, request):
         """查询服务、版本和操作类型
 
         :param request: Request instance for DescribeCloudBaseRunOperationTypes.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunOperationTypesRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeCloudBaseRunOperationTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunPodList(self, request):
         """查询云应用服务版本容器列表
 
         :param request: Request instance for DescribeCloudBaseRunPodList.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunPodListRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeCloudBaseRunPodListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunResource(self, request):
         """查看容器托管的集群状态
 
         :param request: Request instance for DescribeCloudBaseRunResource.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunResourceRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeCloudBaseRunResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunResourceForExtend(self, request):
         """查看容器托管的集群状态扩展使用
 
         :param request: Request instance for DescribeCloudBaseRunResourceForExtend.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunResourceForExtendRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeCloudBaseRunResourceForExtendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunServer(self, request):
         """查询单个服务的详情，版本以及详情
 
         :param request: Request instance for DescribeCloudBaseRunServer.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunServerRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeCloudBaseRunServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunServerDomainName(self, request):
         """查询微信云托管服务域名
 
         :param request: Request instance for DescribeCloudBaseRunServerDomainName.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunServerDomainNameRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeCloudBaseRunServerDomainNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunServerVersion(self, request):
         """查询服务版本的详情，CPU和MEM  请使用CPUSize和MemSize
 
         :param request: Request instance for DescribeCloudBaseRunServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunServerVersionRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeCloudBaseRunServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunVersion(self, request):
         """查询服务版本详情(新)
 
         :param request: Request instance for DescribeCloudBaseRunVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunVersionRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeCloudBaseRunVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunVersionRsByCondition(self, request):
         """DescribeCloudBaseRunVersionRsByCondition 获取云托管详情
 
         :param request: Request instance for DescribeCloudBaseRunVersionRsByCondition.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunVersionRsByConditionRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeCloudBaseRunVersionRsByConditionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudBaseRunVersionSnapshot(self, request):
         """查询版本历史
 
         :param request: Request instance for DescribeCloudBaseRunVersionSnapshot.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseRunVersionSnapshotRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeCloudBaseRunVersionSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCurveData(self, request):
         """根据用户传入的指标, 拉取一段时间内的监控数据。
 
         :param request: Request instance for DescribeCurveData.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCurveDataRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeCurveDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabaseACL(self, request):
         """获取数据库权限
 
         :param request: Request instance for DescribeDatabaseACL.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeDatabaseACLRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDatabaseACLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDownloadFile(self, request):
         """获取下载文件信息
 
         :param request: Request instance for DescribeDownloadFile.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeDownloadFileRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDownloadFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEndUserLoginStatistic(self, request):
         """获取环境终端用户新增与登录信息
 
         :param request: Request instance for DescribeEndUserLoginStatistic.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEndUserLoginStatisticRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeEndUserLoginStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEndUserStatistic(self, request):
         """获取终端用户总量与平台分布情况
 
         :param request: Request instance for DescribeEndUserStatistic.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEndUserStatisticRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeEndUserStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEndUsers(self, request):
         """获取终端用户列表
 
         :param request: Request instance for DescribeEndUsers.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEndUsersRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeEndUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvDealRegion(self, request):
         """获取环境下单地域
 
         :param request: Request instance for DescribeEnvDealRegion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEnvDealRegionRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeEnvDealRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvFreeQuota(self, request):
         """查询后付费免费配额信息
 
         :param request: Request instance for DescribeEnvFreeQuota.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEnvFreeQuotaRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeEnvFreeQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvLimit(self, request):
         """查询环境个数上限
 
         :param request: Request instance for DescribeEnvLimit.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEnvLimitRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeEnvLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvPostpaidDeduct(self, request):
         """查询环境后付费计费详情
 
         :param request: Request instance for DescribeEnvPostpaidDeduct.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEnvPostpaidDeductRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeEnvPostpaidDeductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvs(self, request):
         """获取环境列表，含环境下的各个资源信息。尤其是各资源的唯一标识，是请求各资源的关键参数
 
         :param request: Request instance for DescribeEnvs.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeEnvsRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeEnvsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExtensionUploadInfo(self, request):
         """描述扩展上传文件信息
 
         :param request: Request instance for DescribeExtensionUploadInfo.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeExtensionUploadInfoRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeExtensionUploadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExtraPkgBillingInfo(self, request):
         """获取增值包计费相关信息
 
         :param request: Request instance for DescribeExtraPkgBillingInfo.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeExtraPkgBillingInfoRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeExtraPkgBillingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayCurveData(self, request):
         """查询网关监控数据
 
         :param request: Request instance for DescribeGatewayCurveData.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeGatewayCurveDataRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeGatewayCurveDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayVersions(self, request):
         """查询网关版本信息
         暂不鉴权
 
         :param request: Request instance for DescribeGatewayVersions.
@@ -1285,15 +1285,15 @@
             model = models.DescribeGatewayVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGraphData(self, request):
         """根据用户传入的指标, 拉取一段时间内的监控数据。
 
         :param request: Request instance for DescribeGraphData.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeGraphDataRequest`
@@ -1308,15 +1308,15 @@
             model = models.DescribeGraphDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostingDomainTask(self, request):
         """查询静态托管域名任务状态
 
         :param request: Request instance for DescribeHostingDomainTask.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeHostingDomainTaskRequest`
@@ -1331,15 +1331,15 @@
             model = models.DescribeHostingDomainTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePostpayFreeQuotas(self, request):
         """查询后付费资源免费量
 
         :param request: Request instance for DescribePostpayFreeQuotas.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribePostpayFreeQuotasRequest`
@@ -1354,15 +1354,15 @@
             model = models.DescribePostpayFreeQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePostpayPackageFreeQuotas(self, request):
         """获取后付费免费额度
 
         :param request: Request instance for DescribePostpayPackageFreeQuotas.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribePostpayPackageFreeQuotasRequest`
@@ -1377,15 +1377,15 @@
             model = models.DescribePostpayPackageFreeQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQuotaData(self, request):
         """查询指定指标的配额使用量
 
         :param request: Request instance for DescribeQuotaData.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeQuotaDataRequest`
@@ -1400,15 +1400,15 @@
             model = models.DescribeQuotaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsQuotas(self, request):
         """查询后付费短信资源量
         1 有免费包的返回SmsFreeQuota结构所有字段
         2 没有免费包，有付费包，付费返回复用SmsFreeQuota结构，其中只有 TodayUsedQuota 字段有效
         3 都没有返回为空数组
@@ -1426,15 +1426,15 @@
             model = models.DescribeSmsQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSpecialCostItems(self, request):
         """查询环境1分钱抵扣信息
 
         :param request: Request instance for DescribeSpecialCostItems.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeSpecialCostItemsRequest`
@@ -1449,15 +1449,15 @@
             model = models.DescribeSpecialCostItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStandaloneGateway(self, request):
         """本接口（DescribeStandaloneGateway）查询小租户网关套餐信息。
 
         :param request: Request instance for DescribeStandaloneGateway.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeStandaloneGatewayRequest`
@@ -1472,15 +1472,15 @@
             model = models.DescribeStandaloneGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStandaloneGatewayPackage(self, request):
         """本接口（DescribeStandaloneGatewayPackage）用于查询小租户网关套餐信息。
 
         :param request: Request instance for DescribeStandaloneGatewayPackage.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeStandaloneGatewayPackageRequest`
@@ -1495,15 +1495,15 @@
             model = models.DescribeStandaloneGatewayPackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserActivityInfo(self, request):
         """查询用户活动信息
 
         :param request: Request instance for DescribeUserActivityInfo.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeUserActivityInfoRequest`
@@ -1518,15 +1518,15 @@
             model = models.DescribeUserActivityInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWxCloudBaseRunEnvs(self, request):
         """查询微信云托管环境信息
 
         :param request: Request instance for DescribeWxCloudBaseRunEnvs.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxCloudBaseRunEnvsRequest`
@@ -1541,15 +1541,15 @@
             model = models.DescribeWxCloudBaseRunEnvsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWxCloudBaseRunSubNets(self, request):
         """查询微信云托管子网
 
         :param request: Request instance for DescribeWxCloudBaseRunSubNets.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxCloudBaseRunSubNetsRequest`
@@ -1564,15 +1564,15 @@
             model = models.DescribeWxCloudBaseRunSubNetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWxGatewayRoutes(self, request):
         """查看安全网关路由
 
         :param request: Request instance for DescribeWxGatewayRoutes.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewayRoutesRequest`
@@ -1587,15 +1587,15 @@
             model = models.DescribeWxGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWxGateways(self, request):
         """查看安全网关
 
         :param request: Request instance for DescribeWxGateways.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewaysRequest`
@@ -1610,15 +1610,15 @@
             model = models.DescribeWxGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyEnv(self, request):
         """销毁环境
 
         :param request: Request instance for DestroyEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DestroyEnvRequest`
@@ -1633,15 +1633,15 @@
             model = models.DestroyEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyStandaloneGateway(self, request):
         """本接口（DestroyStandaloneGateway）用于销毁小租户网关。
 
         :param request: Request instance for DestroyStandaloneGateway.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DestroyStandaloneGatewayRequest`
@@ -1656,15 +1656,15 @@
             model = models.DestroyStandaloneGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyStaticStore(self, request):
         """销毁静态托管资源，该接口创建异步销毁任务，资源最终状态可从DestroyStaticStore接口查看
 
         :param request: Request instance for DestroyStaticStore.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DestroyStaticStoreRequest`
@@ -1679,15 +1679,15 @@
             model = models.DestroyStaticStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EstablishCloudBaseRunServer(self, request):
         """创建云应用服务
 
         :param request: Request instance for EstablishCloudBaseRunServer.
         :type request: :class:`tencentcloud.tcb.v20180608.models.EstablishCloudBaseRunServerRequest`
@@ -1702,15 +1702,15 @@
             model = models.EstablishCloudBaseRunServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EstablishWxGatewayRoute(self, request):
         """创建或修改安全网关路由
 
         :param request: Request instance for EstablishWxGatewayRoute.
         :type request: :class:`tencentcloud.tcb.v20180608.models.EstablishWxGatewayRouteRequest`
@@ -1725,15 +1725,15 @@
             model = models.EstablishWxGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FreezeCloudBaseRunServers(self, request):
         """批量冻结
 
         :param request: Request instance for FreezeCloudBaseRunServers.
         :type request: :class:`tencentcloud.tcb.v20180608.models.FreezeCloudBaseRunServersRequest`
@@ -1748,15 +1748,15 @@
             model = models.FreezeCloudBaseRunServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudBaseRunServerFlowConf(self, request):
         """修改容器内的版本流量配置
 
         :param request: Request instance for ModifyCloudBaseRunServerFlowConf.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyCloudBaseRunServerFlowConfRequest`
@@ -1771,15 +1771,15 @@
             model = models.ModifyCloudBaseRunServerFlowConfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudBaseRunServerVersion(self, request):
         """修改服务版本的副本数，环境变量
 
         :param request: Request instance for ModifyCloudBaseRunServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyCloudBaseRunServerVersionRequest`
@@ -1794,15 +1794,15 @@
             model = models.ModifyCloudBaseRunServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClsTopic(self, request):
         """修改日志主题
 
         :param request: Request instance for ModifyClsTopic.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyClsTopicRequest`
@@ -1817,15 +1817,15 @@
             model = models.ModifyClsTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatabaseACL(self, request):
         """修改数据库权限
 
         :param request: Request instance for ModifyDatabaseACL.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyDatabaseACLRequest`
@@ -1840,15 +1840,15 @@
             model = models.ModifyDatabaseACLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEndUser(self, request):
         """管理终端用户
 
         :param request: Request instance for ModifyEndUser.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyEndUserRequest`
@@ -1863,15 +1863,15 @@
             model = models.ModifyEndUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEnv(self, request):
         """更新环境信息
 
         :param request: Request instance for ModifyEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyEnvRequest`
@@ -1886,15 +1886,15 @@
             model = models.ModifyEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGatewayVersionTraffic(self, request):
         """设置网关版本的流量比例
 
         :param request: Request instance for ModifyGatewayVersionTraffic.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyGatewayVersionTrafficRequest`
@@ -1909,15 +1909,15 @@
             model = models.ModifyGatewayVersionTrafficResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReinstateEnv(self, request):
         """针对已隔离的免费环境，可以通过本接口将其恢复访问。
 
         :param request: Request instance for ReinstateEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ReinstateEnvRequest`
@@ -1932,15 +1932,15 @@
             model = models.ReinstateEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceActivityRecord(self, request):
         """更新活动详情
 
         :param request: Request instance for ReplaceActivityRecord.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ReplaceActivityRecordRequest`
@@ -1955,15 +1955,15 @@
             model = models.ReplaceActivityRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollUpdateCloudBaseRunServerVersion(self, request):
         """针对特定的版本，进行滚动更新
 
         :param request: Request instance for RollUpdateCloudBaseRunServerVersion.
         :type request: :class:`tencentcloud.tcb.v20180608.models.RollUpdateCloudBaseRunServerVersionRequest`
@@ -1978,15 +1978,15 @@
             model = models.RollUpdateCloudBaseRunServerVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchClsLog(self, request):
         """搜索CLS日志，TCB角色密钥访问
 
         :param request: Request instance for SearchClsLog.
         :type request: :class:`tencentcloud.tcb.v20180608.models.SearchClsLogRequest`
@@ -2001,15 +2001,15 @@
             model = models.SearchClsLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TurnOffStandaloneGateway(self, request):
         """本接口（TurnOffStandaloneGateway）用于关闭小租户网关。
 
         :param request: Request instance for TurnOffStandaloneGateway.
         :type request: :class:`tencentcloud.tcb.v20180608.models.TurnOffStandaloneGatewayRequest`
@@ -2024,15 +2024,15 @@
             model = models.TurnOffStandaloneGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TurnOnStandaloneGateway(self, request):
         """本接口（TurnOnStandaloneGateway）用于开启小租户网关。
 
         :param request: Request instance for TurnOnStandaloneGateway.
         :type request: :class:`tencentcloud.tcb.v20180608.models.TurnOnStandaloneGatewayRequest`
@@ -2047,15 +2047,15 @@
             model = models.TurnOnStandaloneGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnfreezeCloudBaseRunServers(self, request):
         """批量解冻服务
 
         :param request: Request instance for UnfreezeCloudBaseRunServers.
         :type request: :class:`tencentcloud.tcb.v20180608.models.UnfreezeCloudBaseRunServersRequest`
@@ -2070,8 +2070,8 @@
             model = models.UnfreezeCloudBaseRunServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/tencentcloud/tcb/v20180608/models.py` & `tencentcloud-sdk-python-tcb-3.0.938/tencentcloud/tcb/v20180608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.938/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.938/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.937/README.rst` & `tencentcloud-sdk-python-tcb-3.0.938/README.rst`

 * *Files identical despite different names*

