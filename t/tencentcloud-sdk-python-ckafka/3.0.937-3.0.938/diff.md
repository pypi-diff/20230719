# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.937.tar", last modified: Tue Jul 18 00:20:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.938.tar", last modified: Wed Jul 19 00:24:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.937.tar` & `tencentcloud-sdk-python-ckafka-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)   768834 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    71936 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)   768834 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:24:29.000000 tencentcloud-sdk-python-ckafka-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:24:28.000000 tencentcloud-sdk-python-ckafka-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AuthorizeTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchCreateAcl(self, request):
         """批量添加ACL策略
 
         :param request: Request instance for BatchCreateAcl.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.BatchCreateAclRequest`
@@ -65,15 +65,15 @@
             model = models.BatchCreateAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchModifyGroupOffsets(self, request):
         """批量修改消费组offset
 
         :param request: Request instance for BatchModifyGroupOffsets.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.BatchModifyGroupOffsetsRequest`
@@ -88,15 +88,15 @@
             model = models.BatchModifyGroupOffsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchModifyTopicAttributes(self, request):
         """批量设置主题属性
 
         :param request: Request instance for BatchModifyTopicAttributes.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.BatchModifyTopicAttributesRequest`
@@ -111,15 +111,15 @@
             model = models.BatchModifyTopicAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelAuthorizationToken(self, request):
         """取消授权token
 
         :param request: Request instance for CancelAuthorizationToken.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CancelAuthorizationTokenRequest`
@@ -134,15 +134,15 @@
             model = models.CancelAuthorizationTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckCdcCluster(self, request):
         """用于查询cdc-ckafka任务状态
 
         :param request: Request instance for CheckCdcCluster.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CheckCdcClusterRequest`
@@ -157,15 +157,15 @@
             model = models.CheckCdcClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAcl(self, request):
         """添加 ACL 策略
 
         :param request: Request instance for CreateAcl.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateAclRequest`
@@ -180,15 +180,15 @@
             model = models.CreateAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAclRule(self, request):
         """添加 ACL 规则
 
         :param request: Request instance for CreateAclRule.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateAclRuleRequest`
@@ -203,15 +203,15 @@
             model = models.CreateAclRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCdcCluster(self, request):
         """用于cdc的专用ckafka集群
 
         :param request: Request instance for CreateCdcCluster.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateCdcClusterRequest`
@@ -226,15 +226,15 @@
             model = models.CreateCdcClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConnectResource(self, request):
         """创建Datahub连接源
 
         :param request: Request instance for CreateConnectResource.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateConnectResourceRequest`
@@ -249,15 +249,15 @@
             model = models.CreateConnectResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConsumer(self, request):
         """创建消费者组
 
         :param request: Request instance for CreateConsumer.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateConsumerRequest`
@@ -272,15 +272,15 @@
             model = models.CreateConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDatahubTask(self, request):
         """创建DIP转储任务
 
         :param request: Request instance for CreateDatahubTask.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateDatahubTaskRequest`
@@ -295,15 +295,15 @@
             model = models.CreateDatahubTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDatahubTopic(self, request):
         """创建Datahub主题
 
         :param request: Request instance for CreateDatahubTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateDatahubTopicRequest`
@@ -318,15 +318,15 @@
             model = models.CreateDatahubTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstancePost(self, request):
         """由于出参需要更新，当前接口将会在未来版本中废弃，建议用户迁移使用 CreatePostPaidInstance 接口。创建按量计费实例。通常用于 SDK 或云 API 控制台调用接口，创建后付费 CKafka 实例。调用接口与在 CKafka 控制台购买按量付费实例效果相同。
 
         :param request: Request instance for CreateInstancePost.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePostRequest`
@@ -341,15 +341,15 @@
             model = models.CreateInstancePostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstancePre(self, request):
         """创建实例(预付费包年包月)
 
         :param request: Request instance for CreateInstancePre.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePreRequest`
@@ -364,15 +364,15 @@
             model = models.CreateInstancePreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePartition(self, request):
         """本接口用于增加主题中的分区
 
         :param request: Request instance for CreatePartition.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreatePartitionRequest`
@@ -387,15 +387,15 @@
             model = models.CreatePartitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePostPaidInstance(self, request):
         """当前接口用来替代 CreateInstancePost 接口。创建按量计费实例。通常用于 SDK 或云 API 控制台调用接口，创建后付费 CKafka 实例。调用接口与在 CKafka 控制台购买按量付费实例效果相同。
 
         :param request: Request instance for CreatePostPaidInstance.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreatePostPaidInstanceRequest`
@@ -410,15 +410,15 @@
             model = models.CreatePostPaidInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRoute(self, request):
         """添加实例路由
 
         :param request: Request instance for CreateRoute.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateRouteRequest`
@@ -433,15 +433,15 @@
             model = models.CreateRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateToken(self, request):
         """创建最高权限的token
 
         :param request: Request instance for CreateToken.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateTokenRequest`
@@ -456,15 +456,15 @@
             model = models.CreateTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopic(self, request):
         """创建ckafka主题
 
         :param request: Request instance for CreateTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateTopicRequest`
@@ -479,15 +479,15 @@
             model = models.CreateTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopicIpWhiteList(self, request):
         """创建主题ip白名单
 
         :param request: Request instance for CreateTopicIpWhiteList.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateTopicIpWhiteListRequest`
@@ -502,15 +502,15 @@
             model = models.CreateTopicIpWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """添加用户
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateUserRequest`
@@ -525,15 +525,15 @@
             model = models.CreateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAcl(self, request):
         """删除ACL
 
         :param request: Request instance for DeleteAcl.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteAclRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAclRule(self, request):
         """删除ACL规则
 
         :param request: Request instance for DeleteAclRule.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteAclRuleRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteAclRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConnectResource(self, request):
         """删除Datahub连接源
 
         :param request: Request instance for DeleteConnectResource.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteConnectResourceRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteConnectResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDatahubTask(self, request):
         """删除Datahub任务
 
         :param request: Request instance for DeleteDatahubTask.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteDatahubTaskRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteDatahubTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDatahubTopic(self, request):
         """删除Datahub主题
 
         :param request: Request instance for DeleteDatahubTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteDatahubTopicRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteDatahubTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGroup(self, request):
         """删除消费组
 
         :param request: Request instance for DeleteGroup.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteGroupRequest`
@@ -663,15 +663,15 @@
             model = models.DeleteGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstancePre(self, request):
         """删除预付费实例
 
         :param request: Request instance for DeleteInstancePre.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteInstancePreRequest`
@@ -686,15 +686,15 @@
             model = models.DeleteInstancePreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoute(self, request):
         """删除路由
 
         :param request: Request instance for DeleteRoute.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteRouteRequest`
@@ -709,15 +709,15 @@
             model = models.DeleteRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRouteTriggerTime(self, request):
         """修改删除路由延迟触发时间
 
         :param request: Request instance for DeleteRouteTriggerTime.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteRouteTriggerTimeRequest`
@@ -732,15 +732,15 @@
             model = models.DeleteRouteTriggerTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopic(self, request):
         """删除ckafka主题
 
         :param request: Request instance for DeleteTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteTopicRequest`
@@ -755,15 +755,15 @@
             model = models.DeleteTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopicIpWhiteList(self, request):
         """删除主题IP白名单
 
         :param request: Request instance for DeleteTopicIpWhiteList.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteTopicIpWhiteListRequest`
@@ -778,15 +778,15 @@
             model = models.DeleteTopicIpWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUser(self, request):
         """删除用户
 
         :param request: Request instance for DeleteUser.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DeleteUserRequest`
@@ -801,15 +801,15 @@
             model = models.DeleteUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeACL(self, request):
         """枚举ACL
 
         :param request: Request instance for DescribeACL.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeACLRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeACLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAclRule(self, request):
         """查询ACL规则列表
 
         :param request: Request instance for DescribeAclRule.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeAclRuleRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeAclRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppInfo(self, request):
         """查询用户列表
 
         :param request: Request instance for DescribeAppInfo.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeAppInfoRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeAppInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCkafkaZone(self, request):
         """用于查看ckafka的可用区列表
 
         :param request: Request instance for DescribeCkafkaZone.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeCkafkaZoneRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeCkafkaZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConnectResource(self, request):
         """查询Datahub连接源
 
         :param request: Request instance for DescribeConnectResource.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeConnectResourceRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeConnectResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConnectResources(self, request):
         """查询Datahub连接源列表
 
         :param request: Request instance for DescribeConnectResources.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeConnectResourcesRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeConnectResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConsumerGroup(self, request):
         """查询消费分组信息
 
         :param request: Request instance for DescribeConsumerGroup.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeConsumerGroupRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeConsumerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatahubGroupOffsets(self, request):
         """获取Datahub消费分组offset
 
         :param request: Request instance for DescribeDatahubGroupOffsets.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeDatahubGroupOffsetsRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDatahubGroupOffsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatahubTask(self, request):
         """查询Datahub任务信息
 
         :param request: Request instance for DescribeDatahubTask.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeDatahubTaskRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDatahubTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatahubTasks(self, request):
         """查询Datahub任务列表
 
         :param request: Request instance for DescribeDatahubTasks.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeDatahubTasksRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeDatahubTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatahubTopic(self, request):
         """获取Datahub主题属性
 
         :param request: Request instance for DescribeDatahubTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeDatahubTopicRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeDatahubTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatahubTopics(self, request):
         """查询DIP主题列表
 
         :param request: Request instance for DescribeDatahubTopics.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeDatahubTopicsRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeDatahubTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroup(self, request):
         """枚举消费分组(精简版)
 
         :param request: Request instance for DescribeGroup.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeGroupRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupInfo(self, request):
         """获取消费分组信息
 
         :param request: Request instance for DescribeGroupInfo.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeGroupInfoRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeGroupInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupOffsets(self, request):
         """获取消费分组offset
 
         :param request: Request instance for DescribeGroupOffsets.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeGroupOffsetsRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeGroupOffsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceAttributes(self, request):
         """获取实例属性
 
         :param request: Request instance for DescribeInstanceAttributes.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeInstanceAttributesRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeInstanceAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口（DescribeInstance）用于在用户账户下获取消息队列 CKafka 实例列表
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeInstancesRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesDetail(self, request):
         """用户账户下获取实例列表详情
 
         :param request: Request instance for DescribeInstancesDetail.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeInstancesDetailRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeInstancesDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegion(self, request):
         """枚举地域,只支持广州地域
 
         :param request: Request instance for DescribeRegion.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeRegionRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoute(self, request):
         """查看路由信息
 
         :param request: Request instance for DescribeRoute.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeRouteRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStatus(self, request):
         """查询任务状态
 
         :param request: Request instance for DescribeTaskStatus.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTaskStatusRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopic(self, request):
         """接口请求域名：https://ckafka.tencentcloudapi.com
         本接口（DescribeTopic）用于在用户获取消息队列 CKafka 实例的主题列表
 
         :param request: Request instance for DescribeTopic.
@@ -1308,15 +1308,15 @@
             model = models.DescribeTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicAttributes(self, request):
         """获取主题属性
 
         :param request: Request instance for DescribeTopicAttributes.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicAttributesRequest`
@@ -1331,15 +1331,15 @@
             model = models.DescribeTopicAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicDetail(self, request):
         """获取主题列表详情（仅控制台调用）
 
         :param request: Request instance for DescribeTopicDetail.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicDetailRequest`
@@ -1354,15 +1354,15 @@
             model = models.DescribeTopicDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicFlowRanking(self, request):
         """获取Topic流量排行，消费者流量排行
 
         :param request: Request instance for DescribeTopicFlowRanking.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicFlowRankingRequest`
@@ -1377,15 +1377,15 @@
             model = models.DescribeTopicFlowRankingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicProduceConnection(self, request):
         """查询topic 生产端连接信息
 
         :param request: Request instance for DescribeTopicProduceConnection.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicProduceConnectionRequest`
@@ -1400,15 +1400,15 @@
             model = models.DescribeTopicProduceConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicSubscribeGroup(self, request):
         """查询订阅某主题消息分组信息
 
         :param request: Request instance for DescribeTopicSubscribeGroup.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicSubscribeGroupRequest`
@@ -1423,15 +1423,15 @@
             model = models.DescribeTopicSubscribeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicSyncReplica(self, request):
         """获取Topic 副本详情信息
 
         :param request: Request instance for DescribeTopicSyncReplica.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicSyncReplicaRequest`
@@ -1446,15 +1446,15 @@
             model = models.DescribeTopicSyncReplicaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUser(self, request):
         """查询用户信息
 
         :param request: Request instance for DescribeUser.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeUserRequest`
@@ -1469,15 +1469,15 @@
             model = models.DescribeUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FetchDatahubMessageByOffset(self, request):
         """根据指定offset位置的消息
 
         :param request: Request instance for FetchDatahubMessageByOffset.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.FetchDatahubMessageByOffsetRequest`
@@ -1492,15 +1492,15 @@
             model = models.FetchDatahubMessageByOffsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FetchLatestDatahubMessageList(self, request):
         """查询最新消息列表
 
         :param request: Request instance for FetchLatestDatahubMessageList.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.FetchLatestDatahubMessageListRequest`
@@ -1515,15 +1515,15 @@
             model = models.FetchLatestDatahubMessageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FetchMessageByOffset(self, request):
         """根据指定offset位置的消息
 
         :param request: Request instance for FetchMessageByOffset.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.FetchMessageByOffsetRequest`
@@ -1538,15 +1538,15 @@
             model = models.FetchMessageByOffsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FetchMessageListByOffset(self, request):
         """根据位点查询消息列表
 
         :param request: Request instance for FetchMessageListByOffset.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.FetchMessageListByOffsetRequest`
@@ -1561,15 +1561,15 @@
             model = models.FetchMessageListByOffsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquireCkafkaPrice(self, request):
         """Ckafka实例购买/续费询价
 
         :param request: Request instance for InquireCkafkaPrice.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.InquireCkafkaPriceRequest`
@@ -1584,15 +1584,15 @@
             model = models.InquireCkafkaPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAclRule(self, request):
         """修改AC策略，目前只支持预设规则的是否应用到新增topic这一项的修改
 
         :param request: Request instance for ModifyAclRule.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyAclRuleRequest`
@@ -1607,15 +1607,15 @@
             model = models.ModifyAclRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConnectResource(self, request):
         """编辑Datahub连接源
 
         :param request: Request instance for ModifyConnectResource.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyConnectResourceRequest`
@@ -1630,15 +1630,15 @@
             model = models.ModifyConnectResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatahubTask(self, request):
         """修改Datahub任务
 
         :param request: Request instance for ModifyDatahubTask.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyDatahubTaskRequest`
@@ -1653,15 +1653,15 @@
             model = models.ModifyDatahubTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatahubTopic(self, request):
         """修改Datahub主题属性
 
         :param request: Request instance for ModifyDatahubTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyDatahubTopicRequest`
@@ -1676,15 +1676,15 @@
             model = models.ModifyDatahubTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGroupOffsets(self, request):
         """设置Groups 消费分组offset
 
         :param request: Request instance for ModifyGroupOffsets.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyGroupOffsetsRequest`
@@ -1699,15 +1699,15 @@
             model = models.ModifyGroupOffsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceAttributes(self, request):
         """设置实例属性
 
         :param request: Request instance for ModifyInstanceAttributes.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyInstanceAttributesRequest`
@@ -1722,15 +1722,15 @@
             model = models.ModifyInstanceAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancePre(self, request):
         """预付费实例变配接口，调整磁盘，带宽
 
         :param request: Request instance for ModifyInstancePre.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyInstancePreRequest`
@@ -1745,15 +1745,15 @@
             model = models.ModifyInstancePreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPassword(self, request):
         """修改密码
 
         :param request: Request instance for ModifyPassword.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyPasswordRequest`
@@ -1768,15 +1768,15 @@
             model = models.ModifyPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopicAttributes(self, request):
         """本接口用于修改主题属性。
 
         :param request: Request instance for ModifyTopicAttributes.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.ModifyTopicAttributesRequest`
@@ -1791,15 +1791,15 @@
             model = models.ModifyTopicAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewCkafkaInstance(self, request):
         """续费Ckafka实例, 目前只支持国内站包年包月实例续费
 
         :param request: Request instance for RenewCkafkaInstance.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.RenewCkafkaInstanceRequest`
@@ -1814,15 +1814,15 @@
             model = models.RenewCkafkaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendMessage(self, request):
         """通过HTTP接入层发送消息
 
         :param request: Request instance for SendMessage.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.SendMessageRequest`
@@ -1837,8 +1837,8 @@
             model = models.SendMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.938/tencentcloud/ckafka/v20190819/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.937/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.938/README.rst`

 * *Files identical despite different names*

