# Comparing `tmp/tencentcloud-sdk-python-mgobe-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mgobe-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.937.tar", last modified: Tue Jul 18 00:27:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.938.tar", last modified: Wed Jul 19 00:42:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mgobe-3.0.937.tar` & `tencentcloud-sdk-python-mgobe-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)    34005 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8244 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)    34111 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    32095 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:27:15.000000 tencentcloud-sdk-python-mgobe-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34005 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34111 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    32095 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:42:37.000000 tencentcloud-sdk-python-mgobe-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/setup.py` & `tencentcloud-sdk-python-mgobe-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/mgobe_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,8 +42,8 @@
             model = models.DismissRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20190929/models.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20190929/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/mgobe_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.ChangeRoomPlayerProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeRoomPlayerStatus(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         修改玩家自定义状态
 
@@ -69,15 +69,15 @@
             model = models.ChangeRoomPlayerStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayer(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         该接口用于查询玩家信息。支持两种用法，当OpenId不传的时候，PlayerId必传，传入PlayerId可以查询当前PlayerId的玩家信息，当OpenId传入的时候，PlayerId可不传，按照OpenId查询玩家信息。
 
@@ -94,15 +94,15 @@
             model = models.DescribePlayerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoom(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         该接口用于查询房间信息。支持两种用法，当房间Id不传的时候，玩家Id必传，传入玩家Id可以查询当前玩家所在的房间信息，当房间Id传入的时候，玩家Id可不传，按照房间Id查询房间信息。
 
@@ -119,15 +119,15 @@
             model = models.DescribeRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DismissRoom(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         通过game_id、room_id解散房间
 
@@ -144,15 +144,15 @@
             model = models.DismissRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRoom(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         修改房间
 
@@ -169,15 +169,15 @@
             model = models.ModifyRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveRoomPlayer(self, request):
         """此接口无法使用，游戏联机对战引擎MGOBE已于6.1正式下架，感谢您的支持
 
         踢出房间玩家
 
@@ -194,8 +194,8 @@
             model = models.RemoveRoomPlayerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/tencentcloud/mgobe/v20201014/models.py` & `tencentcloud-sdk-python-mgobe-3.0.938/tencentcloud/mgobe/v20201014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.937/README.rst` & `tencentcloud-sdk-python-mgobe-3.0.938/README.rst`

 * *Files identical despite different names*

