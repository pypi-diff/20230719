# Comparing `tmp/tencentcloud-sdk-python-dc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dc-3.0.937.tar", last modified: Tue Jul 18 00:22:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dc-3.0.938.tar", last modified: Wed Jul 19 00:37:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dc-3.0.937.tar` & `tencentcloud-sdk-python-dc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   148313 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/models.py
--rw-r--r--   0 root         (0) root         (0)    20922 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/dc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:22:19.000000 tencentcloud-sdk-python-dc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   148313 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/models.py
+-rw-r--r--   0 root         (0) root         (0)    21006 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/dc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:37:35.000000 tencentcloud-sdk-python-dc-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dc-3.0.937/setup.py` & `tencentcloud-sdk-python-dc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dc-3.0.937/tencentcloud_sdk_python_dc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dc-3.0.938/tencentcloud_sdk_python_dc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/errorcodes.py` & `tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/models.py` & `tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dc-3.0.937/tencentcloud/dc/v20180410/dc_client.py` & `tencentcloud-sdk-python-dc-3.0.938/tencentcloud/dc/v20180410/dc_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AcceptDirectConnectTunnelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyInternetAddress(self, request):
         """申请互联网CIDR地址
 
         :param request: Request instance for ApplyInternetAddress.
         :type request: :class:`tencentcloud.dc.v20180410.models.ApplyInternetAddressRequest`
@@ -65,15 +65,15 @@
             model = models.ApplyInternetAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDirectConnect(self, request):
         """申请物理专线接入。
         调用该接口时，请注意：
         账号要进行实名认证，否则不允许申请物理专线；
         若账户下存在欠费状态的物理专线，则不能申请更多的物理专线。
@@ -91,15 +91,15 @@
             model = models.CreateDirectConnectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDirectConnectTunnel(self, request):
         """用于创建专用通道的接口
 
         :param request: Request instance for CreateDirectConnectTunnel.
         :type request: :class:`tencentcloud.dc.v20180410.models.CreateDirectConnectTunnelRequest`
@@ -114,15 +114,15 @@
             model = models.CreateDirectConnectTunnelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDirectConnect(self, request):
         """删除物理专线。
         只能删除处于已连接状态的物理专线。
 
         :param request: Request instance for DeleteDirectConnect.
@@ -138,15 +138,15 @@
             model = models.DeleteDirectConnectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDirectConnectTunnel(self, request):
         """删除专用通道
 
         :param request: Request instance for DeleteDirectConnectTunnel.
         :type request: :class:`tencentcloud.dc.v20180410.models.DeleteDirectConnectTunnelRequest`
@@ -161,15 +161,15 @@
             model = models.DeleteDirectConnectTunnelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessPoints(self, request):
         """查询物理专线接入点
 
         :param request: Request instance for DescribeAccessPoints.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeAccessPointsRequest`
@@ -184,15 +184,15 @@
             model = models.DescribeAccessPointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDirectConnectTunnelExtra(self, request):
         """本接口（DescribeDirectConnectTunnelExtra）用于查询专用通道扩展信息
 
         :param request: Request instance for DescribeDirectConnectTunnelExtra.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeDirectConnectTunnelExtraRequest`
@@ -207,15 +207,15 @@
             model = models.DescribeDirectConnectTunnelExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDirectConnectTunnels(self, request):
         """用于查询专用通道列表。
 
         :param request: Request instance for DescribeDirectConnectTunnels.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeDirectConnectTunnelsRequest`
@@ -230,15 +230,15 @@
             model = models.DescribeDirectConnectTunnelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDirectConnects(self, request):
         """查询物理专线列表。
 
         :param request: Request instance for DescribeDirectConnects.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeDirectConnectsRequest`
@@ -253,15 +253,15 @@
             model = models.DescribeDirectConnectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternetAddress(self, request):
         """获取用户互联网公网地址信息
 
         :param request: Request instance for DescribeInternetAddress.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeInternetAddressRequest`
@@ -276,15 +276,15 @@
             model = models.DescribeInternetAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternetAddressQuota(self, request):
         """获取用户互联网公网地址配额
 
         :param request: Request instance for DescribeInternetAddressQuota.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeInternetAddressQuotaRequest`
@@ -299,15 +299,15 @@
             model = models.DescribeInternetAddressQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternetAddressStatistics(self, request):
         """获取用户互联网公网地址分配统计信息
 
         :param request: Request instance for DescribeInternetAddressStatistics.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribeInternetAddressStatisticsRequest`
@@ -322,15 +322,15 @@
             model = models.DescribeInternetAddressStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicDirectConnectTunnelRoutes(self, request):
         """本接口（DescribePublicDirectConnectTunnelRoutes）用于查询互联网通道路由列表
 
         :param request: Request instance for DescribePublicDirectConnectTunnelRoutes.
         :type request: :class:`tencentcloud.dc.v20180410.models.DescribePublicDirectConnectTunnelRoutesRequest`
@@ -345,15 +345,15 @@
             model = models.DescribePublicDirectConnectTunnelRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableInternetAddress(self, request):
         """停用用户申请的公网互联网地址
 
         :param request: Request instance for DisableInternetAddress.
         :type request: :class:`tencentcloud.dc.v20180410.models.DisableInternetAddressRequest`
@@ -368,15 +368,15 @@
             model = models.DisableInternetAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableInternetAddress(self, request):
         """启用已停用的互联网公网地址
 
         :param request: Request instance for EnableInternetAddress.
         :type request: :class:`tencentcloud.dc.v20180410.models.EnableInternetAddressRequest`
@@ -391,15 +391,15 @@
             model = models.EnableInternetAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDirectConnectAttribute(self, request):
         """修改物理专线的属性。
 
         :param request: Request instance for ModifyDirectConnectAttribute.
         :type request: :class:`tencentcloud.dc.v20180410.models.ModifyDirectConnectAttributeRequest`
@@ -414,15 +414,15 @@
             model = models.ModifyDirectConnectAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDirectConnectTunnelAttribute(self, request):
         """修改专用通道属性
 
         :param request: Request instance for ModifyDirectConnectTunnelAttribute.
         :type request: :class:`tencentcloud.dc.v20180410.models.ModifyDirectConnectTunnelAttributeRequest`
@@ -437,15 +437,15 @@
             model = models.ModifyDirectConnectTunnelAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDirectConnectTunnelExtra(self, request):
         """本接口（ModifyDirectConnectTunnelExtra）用于修改专用通道扩展信息
 
         :param request: Request instance for ModifyDirectConnectTunnelExtra.
         :type request: :class:`tencentcloud.dc.v20180410.models.ModifyDirectConnectTunnelExtraRequest`
@@ -460,15 +460,15 @@
             model = models.ModifyDirectConnectTunnelExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RejectDirectConnectTunnel(self, request):
         """拒绝专用通道申请
 
         :param request: Request instance for RejectDirectConnectTunnel.
         :type request: :class:`tencentcloud.dc.v20180410.models.RejectDirectConnectTunnelRequest`
@@ -483,15 +483,15 @@
             model = models.RejectDirectConnectTunnelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseInternetAddress(self, request):
         """释放已申请的互联网地址
 
         :param request: Request instance for ReleaseInternetAddress.
         :type request: :class:`tencentcloud.dc.v20180410.models.ReleaseInternetAddressRequest`
@@ -506,8 +506,8 @@
             model = models.ReleaseInternetAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dc-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dc-3.0.937/README.rst` & `tencentcloud-sdk-python-dc-3.0.938/README.rst`

 * *Files identical despite different names*

