# Comparing `tmp/tencentcloud-sdk-python-ic-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ic-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ic-3.0.937.tar", last modified: Tue Jul 18 00:25:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ic-3.0.938.tar", last modified: Wed Jul 19 00:40:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ic-3.0.937.tar` & `tencentcloud-sdk-python-ic-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/
--rw-r--r--   0 root         (0) root         (0)     8951 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/ic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46716 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:25:12.000000 tencentcloud-sdk-python-ic-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/
+-rw-r--r--   0 root         (0) root         (0)     8987 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/ic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46716 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:40:32.000000 tencentcloud-sdk-python-ic-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ic-3.0.937/setup.py` & `tencentcloud-sdk-python-ic-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.937/tencentcloud_sdk_python_ic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ic-3.0.938/tencentcloud_sdk_python_ic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/ic_client.py` & `tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/ic_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCard(self, request):
         """查询卡片详细信息
 
         :param request: Request instance for DescribeCard.
         :type request: :class:`tencentcloud.ic.v20190307.models.DescribeCardRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeCardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCards(self, request):
         """查询卡片列表信息
 
         :param request: Request instance for DescribeCards.
         :type request: :class:`tencentcloud.ic.v20190307.models.DescribeCardsRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeCardsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSms(self, request):
         """查询短信列表
 
         :param request: Request instance for DescribeSms.
         :type request: :class:`tencentcloud.ic.v20190307.models.DescribeSmsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeSmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserCardRemark(self, request):
         """编辑卡片备注
 
         :param request: Request instance for ModifyUserCardRemark.
         :type request: :class:`tencentcloud.ic.v20190307.models.ModifyUserCardRemarkRequest`
@@ -134,15 +134,15 @@
             model = models.ModifyUserCardRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PayForExtendData(self, request):
         """购买套外流量包
 
         :param request: Request instance for PayForExtendData.
         :type request: :class:`tencentcloud.ic.v20190307.models.PayForExtendDataRequest`
@@ -157,15 +157,15 @@
             model = models.PayForExtendDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewCards(self, request):
         """批量为卡片续费，此接口建议调用至少间隔10s,如果出现返回deal lock failed相关的错误，请过10s再重试。
         续费的必要条件：
         1、单次续费的卡片不可以超过 100张。
         2、接口只支持在控制台购买的卡片进行续费
@@ -185,15 +185,15 @@
             model = models.RenewCardsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendMultiSms(self, request):
         """群发短信
 
         :param request: Request instance for SendMultiSms.
         :type request: :class:`tencentcloud.ic.v20190307.models.SendMultiSmsRequest`
@@ -208,15 +208,15 @@
             model = models.SendMultiSmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSms(self, request):
         """发送短信息接口
 
         :param request: Request instance for SendSms.
         :type request: :class:`tencentcloud.ic.v20190307.models.SendSmsRequest`
@@ -231,8 +231,8 @@
             model = models.SendSmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/errorcodes.py` & `tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.937/tencentcloud/ic/v20190307/models.py` & `tencentcloud-sdk-python-ic-3.0.938/tencentcloud/ic/v20190307/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ic-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ic-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ic-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ic-3.0.937/README.rst` & `tencentcloud-sdk-python-ic-3.0.938/README.rst`

 * *Files identical despite different names*

