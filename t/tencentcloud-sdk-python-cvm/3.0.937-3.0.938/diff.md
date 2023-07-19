# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.937.tar", last modified: Tue Jul 18 00:21:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.938.tar", last modified: Wed Jul 19 00:25:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.937.tar` & `tencentcloud-sdk-python-cvm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44021 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   119300 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   624883 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:21:32.000000 tencentcloud-sdk-python-cvm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44021 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   119676 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)   624916 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:25:37.000000 tencentcloud-sdk-python-cvm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/setup.py` & `tencentcloud-sdk-python-cvm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.938/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.AllocateHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateInstancesKeyPairs(self, request):
         """本接口 (AssociateInstancesKeyPairs) 用于将密钥绑定到实例上。
 
         * 将密钥的公钥写入到实例的`SSH`配置当中，用户就可以通过该密钥的私钥来登录实例。
         * 如果实例原来绑定过密钥，那么原来的密钥将失效。
@@ -71,15 +71,15 @@
             model = models.AssociateInstancesKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSecurityGroups(self, request):
         """本接口 (AssociateSecurityGroups) 用于绑定安全组到指定实例。
         * 实例操作结果可以通过调用 [DescribeInstances](https://cloud.tencent.com/document/api/213/15728#.E7.A4.BA.E4.BE.8B3-.E6.9F.A5.E8.AF.A2.E5.AE.9E.E4.BE.8B.E7.9A.84.E6.9C.80.E6.96.B0.E6.93.8D.E4.BD.9C.E6.83.85.E5.86.B5) 接口查询，如果实例的最新操作状态(LatestOperationState)为“SUCCESS”，则代表操作成功。
 
         :param request: Request instance for AssociateSecurityGroups.
@@ -95,15 +95,15 @@
             model = models.AssociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfigureChcAssistVpc(self, request):
         """配置CHC物理服务器的带外和部署网络。传入带外网络和部署网络信息
 
         :param request: Request instance for ConfigureChcAssistVpc.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ConfigureChcAssistVpcRequest`
@@ -118,15 +118,15 @@
             model = models.ConfigureChcAssistVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfigureChcDeployVpc(self, request):
         """配置CHC物理服务器部署网络
 
         :param request: Request instance for ConfigureChcDeployVpc.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ConfigureChcDeployVpcRequest`
@@ -141,15 +141,15 @@
             model = models.ConfigureChcDeployVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDisasterRecoverGroup(self, request):
         """本接口 (CreateDisasterRecoverGroup)用于创建[分散置放群组](https://cloud.tencent.com/document/product/213/15486)。创建好的置放群组，可在[创建实例](https://cloud.tencent.com/document/api/213/15730)时指定。
 
         :param request: Request instance for CreateDisasterRecoverGroup.
         :type request: :class:`tencentcloud.cvm.v20170312.models.CreateDisasterRecoverGroupRequest`
@@ -164,15 +164,15 @@
             model = models.CreateDisasterRecoverGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHpcCluster(self, request):
         """创建高性能计算集群
 
         :param request: Request instance for CreateHpcCluster.
         :type request: :class:`tencentcloud.cvm.v20170312.models.CreateHpcClusterRequest`
@@ -187,15 +187,15 @@
             model = models.CreateHpcClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImage(self, request):
         """本接口(CreateImage)用于将实例的系统盘制作为新镜像，创建后的镜像可以用于创建实例。
 
         :param request: Request instance for CreateImage.
         :type request: :class:`tencentcloud.cvm.v20170312.models.CreateImageRequest`
@@ -210,15 +210,15 @@
             model = models.CreateImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKeyPair(self, request):
         """本接口 (CreateKeyPair) 用于创建一个 `OpenSSH RSA` 密钥对，可以用于登录 `Linux` 实例。
 
         * 开发者只需指定密钥对名称，即可由系统自动创建密钥对，并返回所生成的密钥对的 `ID` 及其公钥、私钥的内容。
         * 密钥对名称不能和已经存在的密钥对的名称重复。
@@ -238,15 +238,15 @@
             model = models.CreateKeyPairResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLaunchTemplate(self, request):
         """本接口（CreateLaunchTemplate）用于创建实例启动模板。
 
         实例启动模板是一种配置数据并可用于创建实例，其内容包含创建实例所需的配置，比如实例类型，数据盘和系统盘的类型和大小，以及安全组等信息。
 
@@ -265,15 +265,15 @@
             model = models.CreateLaunchTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLaunchTemplateVersion(self, request):
         """本接口（CreateLaunchTemplateVersion）根据指定的实例模板ID以及对应的模板版本号创建新的实例启动模板，若未指定模板版本号则使用默认版本号。每个实例启动模板最多创建30个版本。
 
         :param request: Request instance for CreateLaunchTemplateVersion.
         :type request: :class:`tencentcloud.cvm.v20170312.models.CreateLaunchTemplateVersionRequest`
@@ -288,15 +288,15 @@
             model = models.CreateLaunchTemplateVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDisasterRecoverGroups(self, request):
         """本接口 (DeleteDisasterRecoverGroups)用于删除[分散置放群组](https://cloud.tencent.com/document/product/213/15486)。只有空的置放群组才能被删除，非空的群组需要先销毁组内所有云服务器，才能执行删除操作，不然会产生删除置放群组失败的错误。
 
         :param request: Request instance for DeleteDisasterRecoverGroups.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DeleteDisasterRecoverGroupsRequest`
@@ -311,15 +311,15 @@
             model = models.DeleteDisasterRecoverGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteHpcClusters(self, request):
         """当高性能计算集群为空, 即集群内没有任何设备时候, 可以删除该集群。
 
         :param request: Request instance for DeleteHpcClusters.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DeleteHpcClustersRequest`
@@ -334,15 +334,15 @@
             model = models.DeleteHpcClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImages(self, request):
         """本接口（DeleteImages）用于删除一个或多个镜像。
 
         * 当[镜像状态](https://cloud.tencent.com/document/product/213/15753#Image)为`创建中`和`使用中`时, 不允许删除。镜像状态可以通过[DescribeImages](https://cloud.tencent.com/document/api/213/9418)获取。
         * 每个地域最多只支持创建10个自定义镜像，删除镜像可以释放账户的配额。
@@ -361,15 +361,15 @@
             model = models.DeleteImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteKeyPairs(self, request):
         """本接口 (DeleteKeyPairs) 用于删除已在腾讯云托管的密钥对。
 
         * 可以同时删除多个密钥对。
         * 不能删除已被实例或镜像引用的密钥对，所以需要独立判断是否所有密钥对都被成功删除。
@@ -387,15 +387,15 @@
             model = models.DeleteKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLaunchTemplate(self, request):
         """本接口（DeleteLaunchTemplate）用于删除一个实例启动模板。
 
         :param request: Request instance for DeleteLaunchTemplate.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DeleteLaunchTemplateRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteLaunchTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLaunchTemplateVersions(self, request):
         """本接口（DeleteLaunchTemplateVersions）用于删除一个或者多个实例启动模板版本。
 
         :param request: Request instance for DeleteLaunchTemplateVersions.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DeleteLaunchTemplateVersionsRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteLaunchTemplateVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountQuota(self, request):
         """本接口(DescribeAccountQuota)用于查询用户配额详情。
 
         :param request: Request instance for DescribeAccountQuota.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeAccountQuotaRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeAccountQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChcDeniedActions(self, request):
         """查询CHC物理服务器禁止做的操作，返回给用户
 
         :param request: Request instance for DescribeChcDeniedActions.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeChcDeniedActionsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeChcDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChcHosts(self, request):
         """本接口 (DescribeChcHosts) 用于查询一个或多个CHC物理服务器详细信息。
 
         * 可以根据实例`ID`、实例名称或者设备类型等信息来查询实例的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的实例。
@@ -505,15 +505,15 @@
             model = models.DescribeChcHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisasterRecoverGroupQuota(self, request):
         """本接口 (DescribeDisasterRecoverGroupQuota)用于查询[分散置放群组](https://cloud.tencent.com/document/product/213/15486)配额。
 
         :param request: Request instance for DescribeDisasterRecoverGroupQuota.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeDisasterRecoverGroupQuotaRequest`
@@ -528,15 +528,15 @@
             model = models.DescribeDisasterRecoverGroupQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisasterRecoverGroups(self, request):
         """本接口 (DescribeDisasterRecoverGroups)用于查询[分散置放群组](https://cloud.tencent.com/document/product/213/15486)信息。
 
         :param request: Request instance for DescribeDisasterRecoverGroups.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeDisasterRecoverGroupsRequest`
@@ -551,15 +551,15 @@
             model = models.DescribeDisasterRecoverGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHosts(self, request):
         """本接口 (DescribeHosts) 用于获取一个或多个CDH实例的详细信息。
 
         :param request: Request instance for DescribeHosts.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeHostsRequest`
@@ -574,15 +574,15 @@
             model = models.DescribeHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHpcClusters(self, request):
         """查询高性能集群信息
 
         :param request: Request instance for DescribeHpcClusters.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeHpcClustersRequest`
@@ -597,15 +597,15 @@
             model = models.DescribeHpcClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageQuota(self, request):
         """本接口(DescribeImageQuota)用于查询用户帐号的镜像配额。
 
         :param request: Request instance for DescribeImageQuota.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeImageQuotaRequest`
@@ -620,15 +620,15 @@
             model = models.DescribeImageQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageSharePermission(self, request):
         """本接口（DescribeImageSharePermission）用于查询镜像分享信息。
 
         :param request: Request instance for DescribeImageSharePermission.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeImageSharePermissionRequest`
@@ -643,15 +643,15 @@
             model = models.DescribeImageSharePermissionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """本接口(DescribeImages) 用于查看镜像列表。
 
         * 可以通过指定镜像ID来查询指定镜像的详细信息，或通过设定过滤器来查询满足过滤条件的镜像的详细信息。
         * 指定偏移(Offset)和限制(Limit)来选择结果中的一部分，默认返回满足条件的前20个镜像信息。
@@ -669,15 +669,15 @@
             model = models.DescribeImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImportImageOs(self, request):
         """查看可以导入的镜像操作系统信息。
 
         :param request: Request instance for DescribeImportImageOs.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeImportImageOsRequest`
@@ -692,15 +692,15 @@
             model = models.DescribeImportImageOsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceFamilyConfigs(self, request):
         """本接口（DescribeInstanceFamilyConfigs）查询当前用户和地域所支持的机型族列表信息。
 
         :param request: Request instance for DescribeInstanceFamilyConfigs.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeInstanceFamilyConfigsRequest`
@@ -715,15 +715,15 @@
             model = models.DescribeInstanceFamilyConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceInternetBandwidthConfigs(self, request):
         """本接口 (DescribeInstanceInternetBandwidthConfigs) 用于查询实例带宽配置。
 
         * 只支持查询`BANDWIDTH_PREPAID`（ 预付费按带宽结算 ）计费模式的带宽配置。
         * 接口返回实例的所有带宽配置信息（包含历史的带宽配置信息）。
@@ -741,15 +741,15 @@
             model = models.DescribeInstanceInternetBandwidthConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceTypeConfigs(self, request):
         """本接口 (DescribeInstanceTypeConfigs) 用于查询实例机型配置。
 
         * 可以根据`zone`、`instance-family`、`instance-type`来查询实例机型配置。过滤条件详见过滤器[`Filter`](https://cloud.tencent.com/document/api/213/15753#Filter)。
         * 如果参数为空，返回指定地域的所有实例机型配置。
@@ -767,15 +767,15 @@
             model = models.DescribeInstanceTypeConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceVncUrl(self, request):
         """本接口 ( DescribeInstanceVncUrl ) 用于查询实例管理终端地址，获取的地址可用于实例的 VNC 登录。
 
         * 处于 `STOPPED` 状态的机器无法使用此功能。
         * 管理终端地址的有效期为 15 秒，调用接口成功后如果 15 秒内不使用该链接进行访问，管理终端地址自动失效，您需要重新查询。
@@ -804,15 +804,15 @@
             model = models.DescribeInstanceVncUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口 (DescribeInstances) 用于查询一个或多个实例的详细信息。
 
         * 可以根据实例`ID`、实例名称或者实例计费模式等信息来查询实例的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的实例。
@@ -831,15 +831,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesModification(self, request):
         """本接口 (DescribeInstancesModification) 用于查询指定实例支持调整的机型配置。
 
         :param request: Request instance for DescribeInstancesModification.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeInstancesModificationRequest`
@@ -854,15 +854,15 @@
             model = models.DescribeInstancesModificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesOperationLimit(self, request):
         """本接口（DescribeInstancesOperationLimit）用于查询实例操作限制。
 
         * 目前支持调整配置操作限制次数查询。
 
@@ -879,15 +879,15 @@
             model = models.DescribeInstancesOperationLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesStatus(self, request):
         """本接口 (DescribeInstancesStatus) 用于查询一个或多个实例的状态。
 
         * 可以根据实例`ID`来查询实例的状态。
         * 如果参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的实例状态。
@@ -905,15 +905,15 @@
             model = models.DescribeInstancesStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternetChargeTypeConfigs(self, request):
         """本接口（DescribeInternetChargeTypeConfigs）用于查询网络的计费类型。
 
         :param request: Request instance for DescribeInternetChargeTypeConfigs.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeInternetChargeTypeConfigsRequest`
@@ -928,15 +928,15 @@
             model = models.DescribeInternetChargeTypeConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKeyPairs(self, request):
         """本接口 (DescribeKeyPairs) 用于查询密钥对信息。
 
         * 密钥对是通过一种算法生成的一对密钥，在生成的密钥对中，一个向外界公开，称为公钥；另一个用户自己保留，称为私钥。密钥对的公钥内容可以通过这个接口查询，但私钥内容系统不保留。
 
@@ -953,15 +953,15 @@
             model = models.DescribeKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLaunchTemplateVersions(self, request):
         """本接口（DescribeLaunchTemplateVersions）用于查询实例模板版本信息。
 
         :param request: Request instance for DescribeLaunchTemplateVersions.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeLaunchTemplateVersionsRequest`
@@ -976,15 +976,15 @@
             model = models.DescribeLaunchTemplateVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLaunchTemplates(self, request):
         """本接口（DescribeLaunchTemplates）用于查询一个或者多个实例启动模板。
 
         :param request: Request instance for DescribeLaunchTemplates.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeLaunchTemplatesRequest`
@@ -999,15 +999,15 @@
             model = models.DescribeLaunchTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """本接口(DescribeRegions)用于查询地域信息。因平台策略原因，该接口暂时停止更新，为确保您正常调用，可切换至新链接：https://cloud.tencent.com/document/product/1596/77930。
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeRegionsRequest`
@@ -1022,15 +1022,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReservedInstances(self, request):
         """本接口(DescribeReservedInstances)可提供列出用户已购买的预留实例
 
         :param request: Request instance for DescribeReservedInstances.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeReservedInstancesRequest`
@@ -1045,15 +1045,15 @@
             model = models.DescribeReservedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReservedInstancesConfigInfos(self, request):
         """本接口(DescribeReservedInstancesConfigInfos)供用户列出可购买预留实例机型配置。预留实例当前只针对国际站白名单用户开放。
 
         :param request: Request instance for DescribeReservedInstancesConfigInfos.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeReservedInstancesConfigInfosRequest`
@@ -1068,15 +1068,15 @@
             model = models.DescribeReservedInstancesConfigInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReservedInstancesOfferings(self, request):
         """本接口(DescribeReservedInstancesOfferings)供用户列出可购买的预留实例配置
 
         :param request: Request instance for DescribeReservedInstancesOfferings.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeReservedInstancesOfferingsRequest`
@@ -1091,15 +1091,15 @@
             model = models.DescribeReservedInstancesOfferingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInfo(self, request):
         """本接口 (DescribeTaskInfo) 用于查询云服务器维修任务列表及详细信息。
 
         - 可以根据实例ID、实例名称或任务状态等信息来查询维修任务列表。过滤信息详情可参考入参说明。
         - 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的维修任务列表。
@@ -1117,15 +1117,15 @@
             model = models.DescribeTaskInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneInstanceConfigInfos(self, request):
         """本接口(DescribeZoneInstanceConfigInfos) 获取可用区的机型信息。
 
         :param request: Request instance for DescribeZoneInstanceConfigInfos.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeZoneInstanceConfigInfosRequest`
@@ -1140,15 +1140,15 @@
             model = models.DescribeZoneInstanceConfigInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """本接口(DescribeZones)用于查询可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeZonesRequest`
@@ -1163,15 +1163,15 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateInstancesKeyPairs(self, request):
         """本接口 (DisassociateInstancesKeyPairs) 用于解除实例的密钥绑定关系。
 
         * 只支持[`STOPPED`](https://cloud.tencent.com/document/product/213/15753#InstanceStatus)状态的`Linux`操作系统的实例。
         * 解绑密钥后，实例可以通过原来设置的密码登录。
@@ -1191,15 +1191,15 @@
             model = models.DisassociateInstancesKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateSecurityGroups(self, request):
         """本接口 (DisassociateSecurityGroups) 用于解绑实例的指定安全组。
         * 实例操作结果可以通过调用 [DescribeInstances](https://cloud.tencent.com/document/api/213/15728#.E7.A4.BA.E4.BE.8B3-.E6.9F.A5.E8.AF.A2.E5.AE.9E.E4.BE.8B.E7.9A.84.E6.9C.80.E6.96.B0.E6.93.8D.E4.BD.9C.E6.83.85.E5.86.B5) 接口查询，如果实例的最新操作状态(LatestOperationState)为“SUCCESS”，则代表操作成功。
 
         :param request: Request instance for DisassociateSecurityGroups.
@@ -1215,15 +1215,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportImages(self, request):
         """提供导出自定义镜像到指定COS存储桶的能力
 
         :param request: Request instance for ExportImages.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ExportImagesRequest`
@@ -1238,15 +1238,15 @@
             model = models.ExportImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportImage(self, request):
         """本接口(ImportImage)用于导入镜像，导入后的镜像可用于创建实例。目前支持 RAW、VHD、QCOW2、VMDK 镜像格式。
 
         :param request: Request instance for ImportImage.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ImportImageRequest`
@@ -1261,15 +1261,15 @@
             model = models.ImportImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportKeyPair(self, request):
         """本接口 (ImportKeyPair) 用于导入密钥对。
 
         * 本接口的功能是将密钥对导入到用户账户，并不会自动绑定到实例。如需绑定可以使用[AssociasteInstancesKeyPair](https://cloud.tencent.com/document/api/213/9404)接口。
         * 需指定密钥对名称以及该密钥对的公钥文本。
@@ -1288,15 +1288,15 @@
             model = models.ImportKeyPairResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePricePurchaseReservedInstancesOffering(self, request):
         """本接口(InquirePricePurchaseReservedInstancesOffering)用于创建预留实例询价。本接口仅允许针对购买限制范围内的预留实例配置进行询价。预留实例当前只针对国际站白名单用户开放。
 
         :param request: Request instance for InquirePricePurchaseReservedInstancesOffering.
         :type request: :class:`tencentcloud.cvm.v20170312.models.InquirePricePurchaseReservedInstancesOfferingRequest`
@@ -1311,15 +1311,15 @@
             model = models.InquirePricePurchaseReservedInstancesOfferingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceModifyInstancesChargeType(self, request):
         """本接口 (InquiryPriceModifyInstancesChargeType) 用于切换实例的计费模式询价。
 
         * 只支持从 `POSTPAID_BY_HOUR` 计费模式切换为`PREPAID`计费模式。
         * 关机不收费的实例、`BC1`和`BS1`机型族的实例、设置定时销毁的实例、竞价实例不支持该操作。
@@ -1337,15 +1337,15 @@
             model = models.InquiryPriceModifyInstancesChargeTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRenewHosts(self, request):
         """本接口 (InquiryPriceRenewHosts) 用于续费包年包月`CDH`实例询价。
         * 只支持查询包年包月`CDH`实例的续费价格。
 
         :param request: Request instance for InquiryPriceRenewHosts.
@@ -1361,15 +1361,15 @@
             model = models.InquiryPriceRenewHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRenewInstances(self, request):
         """本接口 (InquiryPriceRenewInstances) 用于续费包年包月实例询价。
 
         * 只支持查询包年包月实例的续费价格。
 
@@ -1386,15 +1386,15 @@
             model = models.InquiryPriceRenewInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceResetInstance(self, request):
         """本接口 (InquiryPriceResetInstance) 用于重装实例询价。
 
         * 如果指定了`ImageId`参数，则使用指定的镜像进行重装询价；否则按照当前实例使用的镜像进行重装询价。
         * 目前只支持[系统盘类型](https://cloud.tencent.com/document/api/213/15753#SystemDisk)是`CLOUD_BASIC`、`CLOUD_PREMIUM`、`CLOUD_SSD`类型的实例使用该接口实现`Linux`和`Windows`操作系统切换的重装询价。
@@ -1413,15 +1413,15 @@
             model = models.InquiryPriceResetInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceResetInstancesInternetMaxBandwidth(self, request):
         """本接口 (InquiryPriceResetInstancesInternetMaxBandwidth) 用于调整实例公网带宽上限询价。
 
         * 不同机型带宽上限范围不一致，具体限制详见[公网带宽上限](https://cloud.tencent.com/document/product/213/12523)。
         * 对于`BANDWIDTH_PREPAID`计费方式的带宽，目前不支持调小带宽，且需要输入参数`StartTime`和`EndTime`，指定调整后的带宽的生效时间段。在这种场景下会涉及扣费，请确保账户余额充足。可通过[`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253)接口查询账户余额。
@@ -1443,15 +1443,15 @@
             model = models.InquiryPriceResetInstancesInternetMaxBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceResetInstancesType(self, request):
         """本接口 (InquiryPriceResetInstancesType) 用于调整实例的机型询价。
 
         * 目前只支持[系统盘类型](https://cloud.tencent.com/document/product/213/15753#SystemDisk)是`CLOUD_BASIC`、`CLOUD_PREMIUM`、`CLOUD_SSD`类型的实例使用该接口进行调整机型询价。
         * 目前不支持[CDH](https://cloud.tencent.com/document/product/416)实例使用该接口调整机型询价。
@@ -1469,15 +1469,15 @@
             model = models.InquiryPriceResetInstancesTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceResizeInstanceDisks(self, request):
         """本接口 (InquiryPriceResizeInstanceDisks) 用于扩容实例的数据盘询价。
 
         * 目前只支持扩容非弹性数据盘（[`DescribeDisks`](https://cloud.tencent.com/document/api/362/16315)接口返回值中的`Portable`为`false`表示非弹性）询价，且[数据盘类型](https://cloud.tencent.com/document/product/213/15753#DataDisk)为：`CLOUD_BASIC`、`CLOUD_PREMIUM`、`CLOUD_SSD`。
         * 目前不支持[CDH](https://cloud.tencent.com/document/product/416)实例使用该接口扩容数据盘询价。* 仅支持包年包月实例随机器购买的数据盘。* 目前只支持扩容一块数据盘询价。
@@ -1495,15 +1495,15 @@
             model = models.InquiryPriceResizeInstanceDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRunInstances(self, request):
         """本接口(InquiryPriceRunInstances)用于创建实例询价。本接口仅允许针对购买限制范围内的实例配置进行询价, 详见：[创建实例](https://cloud.tencent.com/document/api/213/15730)。
 
         :param request: Request instance for InquiryPriceRunInstances.
         :type request: :class:`tencentcloud.cvm.v20170312.models.InquiryPriceRunInstancesRequest`
@@ -1518,15 +1518,15 @@
             model = models.InquiryPriceRunInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceTerminateInstances(self, request):
         """本接口 (InquiryPriceTerminateInstances) 用于退还实例询价。
 
         * 查询退还实例可以返还的费用。
         * 在退还包年包月实例时，使用ReleasePrepaidDataDisks参数，会在返回值中包含退还挂载的包年包月数据盘返还的费用。
@@ -1545,15 +1545,15 @@
             model = models.InquiryPriceTerminateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyChcAttribute(self, request):
         """修改CHC物理服务器的属性
 
         :param request: Request instance for ModifyChcAttribute.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ModifyChcAttributeRequest`
@@ -1568,15 +1568,15 @@
             model = models.ModifyChcAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDisasterRecoverGroupAttribute(self, request):
         """本接口 (ModifyDisasterRecoverGroupAttribute)用于修改[分散置放群组](https://cloud.tencent.com/document/product/213/15486)属性。
 
         :param request: Request instance for ModifyDisasterRecoverGroupAttribute.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ModifyDisasterRecoverGroupAttributeRequest`
@@ -1591,15 +1591,15 @@
             model = models.ModifyDisasterRecoverGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHostsAttribute(self, request):
         """本接口（ModifyHostsAttribute）用于修改CDH实例的属性，如实例名称和续费标记等。参数HostName和RenewFlag必须设置其中一个，但不能同时设置。
 
         :param request: Request instance for ModifyHostsAttribute.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ModifyHostsAttributeRequest`
@@ -1614,15 +1614,15 @@
             model = models.ModifyHostsAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHpcClusterAttribute(self, request):
         """修改高性能计算集群属性。
 
         :param request: Request instance for ModifyHpcClusterAttribute.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ModifyHpcClusterAttributeRequest`
@@ -1637,15 +1637,15 @@
             model = models.ModifyHpcClusterAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImageAttribute(self, request):
         """本接口（ModifyImageAttribute）用于修改镜像属性。
 
         * 已分享的镜像无法修改属性。
 
@@ -1662,15 +1662,15 @@
             model = models.ModifyImageAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImageSharePermission(self, request):
         """本接口（ModifyImageSharePermission）用于修改镜像分享信息。
 
         * 分享镜像后，被分享账户可以通过该镜像创建实例。
         * 每个自定义镜像最多可共享给50个账户。
@@ -1690,15 +1690,15 @@
             model = models.ModifyImageSharePermissionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceDiskType(self, request):
         """本接口 (ModifyInstanceDiskType) 用于修改实例硬盘介质类型。
 
         * 只支持实例的本地系统盘、本地数据盘转化成指定云硬盘介质。
         * 只支持实例在关机状态下转换成指定云硬盘介质。
@@ -1719,15 +1719,15 @@
             model = models.ModifyInstanceDiskTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesAttribute(self, request):
         """本接口 (ModifyInstancesAttribute) 用于修改实例的属性（目前只支持修改实例的名称和关联的安全组）。
 
         * 每次请求必须指定实例的一种属性用于修改。
         * “实例名称”仅为方便用户自己管理之用，腾讯云并不以此名称作为在线支持或是进行实例管理操作的依据。
@@ -1748,15 +1748,15 @@
             model = models.ModifyInstancesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesChargeType(self, request):
         """本接口 (ModifyInstancesChargeType) 用于切换实例的计费模式。
 
         * 关机不收费的实例、`BC1`和`BS1`机型族的实例、设置定时销毁的实例不支持该操作。
         * 实例操作结果可以通过调用 [DescribeInstances](https://cloud.tencent.com/document/api/213/15728#.E7.A4.BA.E4.BE.8B3-.E6.9F.A5.E8.AF.A2.E5.AE.9E.E4.BE.8B.E7.9A.84.E6.9C.80.E6.96.B0.E6.93.8D.E4.BD.9C.E6.83.85.E5.86.B5) 接口查询，如果实例的最新操作状态(LatestOperationState)为“SUCCESS”，则代表操作成功。
@@ -1774,15 +1774,15 @@
             model = models.ModifyInstancesChargeTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesProject(self, request):
         """本接口 (ModifyInstancesProject) 用于修改实例所属项目。
 
         * 项目为一个虚拟概念，用户可以在一个账户下面建立多个项目，每个项目中管理不同的资源；将多个不同实例分属到不同项目中，后续使用 [`DescribeInstances`](https://cloud.tencent.com/document/api/213/15728)接口查询实例，项目ID可用于过滤结果。
         * 绑定负载均衡的实例不支持修改实例所属项目，请先使用[`DeregisterInstancesFromLoadBalancer`](https://cloud.tencent.com/document/api/214/1258)接口解绑负载均衡。
@@ -1802,15 +1802,15 @@
             model = models.ModifyInstancesProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesRenewFlag(self, request):
         """本接口 (ModifyInstancesRenewFlag) 用于修改包年包月实例续费标识。
 
         * 实例被标识为自动续费后，每次在实例到期时，会自动续费一个月。
         * 支持批量操作。每次请求批量实例的上限为100。
@@ -1829,15 +1829,15 @@
             model = models.ModifyInstancesRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesVpcAttribute(self, request):
         """本接口(ModifyInstancesVpcAttribute)用于修改实例vpc属性，如私有网络IP。
         * 此操作默认会关闭实例，完成后再启动。
         * 当指定私有网络ID和子网ID（子网必须在实例所在的可用区）与指定实例所在私有网络不一致时，会将实例迁移至指定的私有网络的子网下。执行此操作前请确保指定的实例上没有绑定[弹性网卡](https://cloud.tencent.com/document/product/576)和[负载均衡](https://cloud.tencent.com/document/product/214)。
         * 实例操作结果可以通过调用 [DescribeInstances](https://cloud.tencent.com/document/api/213/15728#.E7.A4.BA.E4.BE.8B3-.E6.9F.A5.E8.AF.A2.E5.AE.9E.E4.BE.8B.E7.9A.84.E6.9C.80.E6.96.B0.E6.93.8D.E4.BD.9C.E6.83.85.E5.86.B5) 接口查询，如果实例的最新操作状态(LatestOperationState)为“SUCCESS”，则代表操作成功。
@@ -1855,15 +1855,15 @@
             model = models.ModifyInstancesVpcAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyKeyPairAttribute(self, request):
         """本接口 (ModifyKeyPairAttribute) 用于修改密钥对属性。
 
         * 修改密钥对ID所指定的密钥对的名称和描述信息。
         * 密钥对名称不能和已经存在的密钥对的名称重复。
@@ -1882,15 +1882,15 @@
             model = models.ModifyKeyPairAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLaunchTemplateDefaultVersion(self, request):
         """本接口（ModifyLaunchTemplateDefaultVersion）用于修改实例启动模板默认版本。
 
         :param request: Request instance for ModifyLaunchTemplateDefaultVersion.
         :type request: :class:`tencentcloud.cvm.v20170312.models.ModifyLaunchTemplateDefaultVersionRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifyLaunchTemplateDefaultVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProgramFpgaImage(self, request):
         """本接口(ProgramFpgaImage)用于在线烧录由客户提供的FPGA镜像文件到指定实例的指定FPGA卡上。
         * 只支持对单个实例发起在线烧录FPGA镜像的操作。
         * 支持对单个实例的多块FPGA卡同时烧录FPGA镜像，DBDFs参数为空时，默认对指定实例的所有FPGA卡进行烧录。
 
@@ -1930,15 +1930,15 @@
             model = models.ProgramFpgaImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PurchaseReservedInstancesOffering(self, request):
         """本接口(PurchaseReservedInstancesOffering)用于用户购买一个或者多个指定配置的预留实例
 
         :param request: Request instance for PurchaseReservedInstancesOffering.
         :type request: :class:`tencentcloud.cvm.v20170312.models.PurchaseReservedInstancesOfferingRequest`
@@ -1953,15 +1953,15 @@
             model = models.PurchaseReservedInstancesOfferingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebootInstances(self, request):
         """本接口 (RebootInstances) 用于重启实例。
 
         * 只有状态为`RUNNING`的实例才可以进行此操作。
         * 接口调用成功时，实例会进入`REBOOTING`状态；重启实例成功时，实例会进入`RUNNING`状态。
@@ -1982,15 +1982,15 @@
             model = models.RebootInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveChcAssistVpc(self, request):
         """清理CHC物理服务器的带外网络和部署网络
 
         :param request: Request instance for RemoveChcAssistVpc.
         :type request: :class:`tencentcloud.cvm.v20170312.models.RemoveChcAssistVpcRequest`
@@ -2005,15 +2005,15 @@
             model = models.RemoveChcAssistVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveChcDeployVpc(self, request):
         """清理CHC物理服务器的部署网络
 
         :param request: Request instance for RemoveChcDeployVpc.
         :type request: :class:`tencentcloud.cvm.v20170312.models.RemoveChcDeployVpcRequest`
@@ -2028,15 +2028,15 @@
             model = models.RemoveChcDeployVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewHosts(self, request):
         """本接口 (RenewHosts) 用于续费包年包月CDH实例。
 
         * 只支持操作包年包月实例，否则操作会以特定[错误码](#6.-.E9.94.99.E8.AF.AF.E7.A0.81)返回。
         * 续费时请确保账户余额充足。可通过[`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253)接口查询账户余额。
@@ -2054,15 +2054,15 @@
             model = models.RenewHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstances(self, request):
         """本接口 (RenewInstances) 用于续费包年包月实例。
 
         * 只支持操作包年包月实例。
         * 续费时请确保账户余额充足。可通过[`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253)接口查询账户余额。
@@ -2081,15 +2081,15 @@
             model = models.RenewInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RepairTaskControl(self, request):
         """本接口（RepairTaskControl）用于对待授权状态的维修任务进行授权操作。
 
         - 仅当任务状态处于`待授权`状态时，可通过此接口对待授权的维修任务进行授权。
         - 调用时需指定产品类型、实例ID、维修任务ID、操作类型。
@@ -2109,15 +2109,15 @@
             model = models.RepairTaskControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstance(self, request):
         """本接口 (ResetInstance) 用于重装指定实例上的操作系统。
 
         * 如果指定了`ImageId`参数，则使用指定的镜像重装；否则按照当前实例使用的镜像进行重装。
         * 系统盘将会被格式化，并重置；请确保系统盘中无重要文件。
@@ -2140,15 +2140,15 @@
             model = models.ResetInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesInternetMaxBandwidth(self, request):
         """本接口 (ResetInstancesInternetMaxBandwidth) 用于调整实例公网带宽上限。
 
         * 不同机型带宽上限范围不一致，具体限制详见[公网带宽上限](https://cloud.tencent.com/document/product/213/12523)。
         * 对于 `BANDWIDTH_PREPAID` 计费方式的带宽，需要输入参数 `StartTime` 和 `EndTime` ，指定调整后的带宽的生效时间段。在这种场景下目前不支持调小带宽，会涉及扣费，请确保账户余额充足。可通过 [`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253) 接口查询账户余额。
@@ -2171,15 +2171,15 @@
             model = models.ResetInstancesInternetMaxBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesPassword(self, request):
         """本接口 (ResetInstancesPassword) 用于将实例操作系统的密码重置为用户指定的密码。
 
         *如果是修改系统管理云密码：实例的操作系统不同，管理员帐号也会不一样(`Windows`为`Administrator`，`Ubuntu`为`ubuntu`，其它系统为`root`)。
         * 重置处于运行中状态的实例密码，需要设置关机参数`ForceStop`为`TRUE`。如果没有显式指定强制关机参数，则只有处于关机状态的实例才允许执行重置密码操作。
@@ -2199,15 +2199,15 @@
             model = models.ResetInstancesPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesType(self, request):
         """本接口 (ResetInstancesType) 用于调整实例的机型。
 
         * 目前只支持[系统盘类型](/document/api/213/9452#block_device)是CLOUD_BASIC、CLOUD_PREMIUM、CLOUD_SSD类型的实例使用该接口进行机型调整。
         * 目前不支持[CDH](https://cloud.tencent.com/document/product/416)实例使用该接口调整机型。对于包年包月实例，使用该接口会涉及扣费，请确保账户余额充足。可通过[`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253)接口查询账户余额。
@@ -2226,15 +2226,15 @@
             model = models.ResetInstancesTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResizeInstanceDisks(self, request):
         """本接口 (ResizeInstanceDisks) 用于扩容实例的数据盘。
 
         * 目前只支持扩容非弹性盘（[`DescribeDisks`](https://cloud.tencent.com/document/api/362/16315)接口返回值中的`Portable`为`false`表示非弹性），且[数据盘类型](https://cloud.tencent.com/document/api/213/15753#DataDisk)为：`CLOUD_BASIC`、`CLOUD_PREMIUM`、`CLOUD_SSD`和[CDH](https://cloud.tencent.com/document/product/416)实例的`LOCAL_BASIC`、`LOCAL_SSD`类型数据盘。
         * 对于包年包月实例，使用该接口会涉及扣费，请确保账户余额充足。可通过[`DescribeAccountBalance`](https://cloud.tencent.com/document/product/555/20253)接口查询账户余额。
@@ -2255,15 +2255,15 @@
             model = models.ResizeInstanceDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunInstances(self, request):
         """本接口 (RunInstances) 用于创建一个或多个指定配置的实例。
 
         * 实例创建成功后将自动开机启动，[实例状态](https://cloud.tencent.com/document/product/213/15753#InstanceStatus)变为“运行中”。
         * 预付费实例的购买会预先扣除本次实例购买所需金额，按小时后付费实例购买会预先冻结本次实例购买一小时内所需金额，在调用本接口前请确保账户余额充足。
@@ -2284,15 +2284,15 @@
             model = models.RunInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartInstances(self, request):
         """本接口 (StartInstances) 用于启动一个或多个实例。
 
         * 只有状态为`STOPPED`的实例才可以进行此操作。
         * 接口调用成功时，实例会进入`STARTING`状态；启动实例成功时，实例会进入`RUNNING`状态。
@@ -2312,15 +2312,15 @@
             model = models.StartInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopInstances(self, request):
         """本接口 (StopInstances) 用于关闭一个或多个实例。
 
         * 只有状态为`RUNNING`的实例才可以进行此操作。
         * 接口调用成功时，实例会进入`STOPPING`状态；关闭实例成功时，实例会进入`STOPPED`状态。
@@ -2341,15 +2341,15 @@
             model = models.StopInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncImages(self, request):
         """本接口（SyncImages）用于将自定义镜像同步到其它地区。
 
         * 该接口每次调用只支持同步一个镜像。
         * 该接口支持多个同步地域。
@@ -2368,15 +2368,15 @@
             model = models.SyncImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateInstances(self, request):
         """本接口 (TerminateInstances) 用于主动退还实例。
 
         * 不再使用的实例，可通过本接口主动退还。
         * 按量计费的实例通过本接口可直接退还；包年包月实例如符合[退还规则](https://cloud.tencent.com/document/product/213/9711)，也可通过本接口主动退还。
@@ -2398,8 +2398,8 @@
             model = models.TerminateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.938/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8979,15 +8979,15 @@
         :type LoginSettings: :class:`tencentcloud.cvm.v20170312.models.LoginSettings`
         :param _SecurityGroupIds: 实例所属安全组。该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的sgId字段来获取。若不指定该参数，则默认不绑定安全组。
         :type SecurityGroupIds: list of str
         :param _EnhancedService: 增强服务。通过该参数可以指定是否开启云安全、云监控等服务。若不指定该参数，则默认开启云监控、云安全服务。
         :type EnhancedService: :class:`tencentcloud.cvm.v20170312.models.EnhancedService`
         :param _ClientToken: 用于保证请求幂等性的字符串。该字符串由客户生成，需保证不同请求之间唯一，最大值不超过64个ASCII字符。若不指定该参数，则无法保证请求的幂等性。<br>更多详细信息请参阅：如何保证幂等性。
         :type ClientToken: str
-        :param _HostName: 云服务器的主机名。<br><li>点号（.）和短横线（-）不能作为 HostName 的首尾字符，不能连续使用。<br><li>Windows 实例：名字符长度为[2, 15]，允许字母（不限制大小写）、数字和短横线（-）组成，不支持点号（.），不能全是数字。<br><li>其他类型（Linux 等）实例：字符长度为[2, 30]，允许支持多个点号，点之间为一段，每段允许字母（不限制大小写）、数字和短横线（-）组成。
+        :param _HostName: 云服务器的主机名。<br><li>点号（.）和短横线（-）不能作为 HostName 的首尾字符，不能连续使用。<br><li>Windows 实例：主机名字符长度为[2, 15]，允许字母（不限制大小写）、数字和短横线（-）组成，不支持点号（.），不能全是数字。<br><li>其他类型（Linux 等）实例：主机名字符长度为[2, 30]，允许支持多个点号，点之间为一段，每段允许字母（不限制大小写）、数字和短横线（-）组成。
         :type HostName: str
         :param _TagSpecification: 标签描述列表。通过指定该参数可以同时绑定标签到相应的资源实例，当前仅支持绑定标签到云服务器实例。
         :type TagSpecification: list of TagSpecification
         :param _InstanceMarketOptions: 实例的市场相关选项，如竞价实例相关参数
         :type InstanceMarketOptions: :class:`tencentcloud.cvm.v20170312.models.InstanceMarketOptionsRequest`
         :param _HpcClusterId: 高性能计算集群ID。
         :type HpcClusterId: str
@@ -16162,15 +16162,15 @@
         :type LoginSettings: :class:`tencentcloud.cvm.v20170312.models.LoginSettings`
         :param _SecurityGroupIds: 实例所属安全组。该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的sgId字段来获取。若不指定该参数，则绑定默认安全组。
         :type SecurityGroupIds: list of str
         :param _EnhancedService: 增强服务。通过该参数可以指定是否开启云安全、云监控等服务。若不指定该参数，则默认公共镜像开启云监控、云安全服务；自定义镜像与镜像市场镜像默认不开启云监控，云安全服务，而使用镜像里保留的服务。
         :type EnhancedService: :class:`tencentcloud.cvm.v20170312.models.EnhancedService`
         :param _ClientToken: 用于保证请求幂等性的字符串。该字符串由客户生成，需保证不同请求之间唯一，最大值不超过64个ASCII字符。若不指定该参数，则无法保证请求的幂等性。
         :type ClientToken: str
-        :param _HostName: 实例主机名。<br><li>点号（.）和短横线（-）不能作为 HostName 的首尾字符，不能连续使用。<br><li>Windows 实例：名字符长度为[2, 15]，允许字母（不限制大小写）、数字和短横线（-）组成，不支持点号（.），不能全是数字。<br><li>其他类型（Linux 等）实例：字符长度为[2, 60]，允许支持多个点号，点之间为一段，每段允许字母（不限制大小写）、数字和短横线（-）组成。<br><li>购买多台实例，如果指定模式串`{R:x}`，表示生成数字`[x, x+n-1]`，其中`n`表示购买实例的数量，例如`server{R:3}`，购买1台时，实例主机名为`server3`；购买2台时，实例主机名分别为`server3`，`server4`。支持指定多个模式串`{R:x}`。</li><br><li>购买多台实例，如果不指定模式串，则在实例主机名添加后缀`1、2...n`，其中`n`表示购买实例的数量，例如`server`，购买2台时，实例主机名分别为`server1`，`server2`。
+        :param _HostName: 实例主机名。<br><li>点号（.）和短横线（-）不能作为 HostName 的首尾字符，不能连续使用。<br><li>Windows 实例：主机名名字符长度为[2, 15]，允许字母（不限制大小写）、数字和短横线（-）组成，不支持点号（.），不能全是数字。<br><li>其他类型（Linux 等）实例：主机名字符长度为[2, 60]，允许支持多个点号，点之间为一段，每段允许字母（不限制大小写）、数字和短横线（-）组成。<br><li>购买多台实例，如果指定模式串`{R:x}`，表示生成数字`[x, x+n-1]`，其中`n`表示购买实例的数量，例如`server{R:3}`，购买1台时，实例主机名为`server3`；购买2台时，实例主机名分别为`server3`，`server4`。支持指定多个模式串`{R:x}`。</li><br><li>购买多台实例，如果不指定模式串，则在实例主机名添加后缀`1、2...n`，其中`n`表示购买实例的数量，例如`server`，购买2台时，实例主机名分别为`server1`，`server2`。
         :type HostName: str
         :param _ActionTimer: 定时任务。通过该参数可以为实例指定定时任务，目前仅支持定时销毁。
         :type ActionTimer: :class:`tencentcloud.cvm.v20170312.models.ActionTimer`
         :param _DisasterRecoverGroupIds: 置放群组id，仅支持指定一个。
         :type DisasterRecoverGroupIds: list of str
         :param _TagSpecification: 标签描述列表。通过指定该参数可以同时绑定标签到相应的云服务器、云硬盘实例。
         :type TagSpecification: list of TagSpecification
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.937/README.rst` & `tencentcloud-sdk-python-cvm-3.0.938/README.rst`

 * *Files identical despite different names*

