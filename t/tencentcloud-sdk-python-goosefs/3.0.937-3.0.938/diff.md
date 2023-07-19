# Comparing `tmp/tencentcloud-sdk-python-goosefs-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-goosefs-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-goosefs-3.0.937.tar", last modified: Tue Jul 18 00:24:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-goosefs-3.0.938.tar", last modified: Wed Jul 19 00:39:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-goosefs-3.0.937.tar` & `tencentcloud-sdk-python-goosefs-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/__init__.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5810 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/goosefs_client.py
--rw-r--r--   0 root         (0) root         (0)    18278 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:28.000000 tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5830 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/goosefs_client.py
+-rw-r--r--   0 root         (0) root         (0)    19733 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:45.000000 tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/setup.py` & `tencentcloud-sdk-python-goosefs-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/errorcodes.py` & `tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/goosefs_client.py` & `tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/goosefs_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateDataRepositoryTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterClientToken(self, request):
         """查询GooseFS集群客户端凭证
 
         :param request: Request instance for DescribeClusterClientToken.
         :type request: :class:`tencentcloud.goosefs.v20220519.models.DescribeClusterClientTokenRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeClusterClientTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterRoleToken(self, request):
         """查询GooseFS集群角色凭证
 
         :param request: Request instance for DescribeClusterRoleToken.
         :type request: :class:`tencentcloud.goosefs.v20220519.models.DescribeClusterRoleTokenRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeClusterRoleTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterRoles(self, request):
         """查询GooseFS集群角色
 
         :param request: Request instance for DescribeClusterRoles.
         :type request: :class:`tencentcloud.goosefs.v20220519.models.DescribeClusterRolesRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeClusterRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataRepositoryTaskStatus(self, request):
         """获取数据流通任务实时状态，用作客户端控制
 
         :param request: Request instance for DescribeDataRepositoryTaskStatus.
         :type request: :class:`tencentcloud.goosefs.v20220519.models.DescribeDataRepositoryTaskStatusRequest`
@@ -134,8 +134,8 @@
             model = models.DescribeDataRepositoryTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/goosefs/v20220519/models.py` & `tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/goosefs/v20220519/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,70 @@
 class ClientToken(AbstractModel):
     """查询Client Token
 
     """
 
     def __init__(self):
         r"""
+        :param _NodeIp: 节点 IP
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeIp: str
         :param _LocalDirectory: 挂载点
 注意：此字段可能返回 null，表示取不到有效值。
         :type LocalDirectory: str
+        :param _GooseFSDirectory: 可以访问的 GooseFS 目录
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GooseFSDirectory: str
+        :param _Token: token
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Token: str
         """
+        self._NodeIp = None
         self._LocalDirectory = None
+        self._GooseFSDirectory = None
+        self._Token = None
+
+    @property
+    def NodeIp(self):
+        return self._NodeIp
+
+    @NodeIp.setter
+    def NodeIp(self, NodeIp):
+        self._NodeIp = NodeIp
 
     @property
     def LocalDirectory(self):
         return self._LocalDirectory
 
     @LocalDirectory.setter
     def LocalDirectory(self, LocalDirectory):
         self._LocalDirectory = LocalDirectory
 
+    @property
+    def GooseFSDirectory(self):
+        return self._GooseFSDirectory
+
+    @GooseFSDirectory.setter
+    def GooseFSDirectory(self, GooseFSDirectory):
+        self._GooseFSDirectory = GooseFSDirectory
+
+    @property
+    def Token(self):
+        return self._Token
+
+    @Token.setter
+    def Token(self, Token):
+        self._Token = Token
+
 
     def _deserialize(self, params):
+        self._NodeIp = params.get("NodeIp")
         self._LocalDirectory = params.get("LocalDirectory")
+        self._GooseFSDirectory = params.get("GooseFSDirectory")
+        self._Token = params.get("Token")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -430,28 +469,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _ClusterId: 集群ID
         :type ClusterId: str
+        :param _RoleName: 角色名
+        :type RoleName: str
         """
         self._ClusterId = None
+        self._RoleName = None
 
     @property
     def ClusterId(self):
         return self._ClusterId
 
     @ClusterId.setter
     def ClusterId(self, ClusterId):
         self._ClusterId = ClusterId
 
+    @property
+    def RoleName(self):
+        return self._RoleName
+
+    @RoleName.setter
+    def RoleName(self, RoleName):
+        self._RoleName = RoleName
+
 
     def _deserialize(self, params):
         self._ClusterId = params.get("ClusterId")
+        self._RoleName = params.get("RoleName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-goosefs-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-goosefs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Goosefs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/README.rst` & `tencentcloud-sdk-python-goosefs-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-goosefs-3.0.937/tencentcloud_sdk_python_goosefs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-goosefs-3.0.938/tencentcloud_sdk_python_goosefs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-goosefs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Goosefs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

