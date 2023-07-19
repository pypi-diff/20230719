# Comparing `tmp/tencentcloud-sdk-python-zj-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-zj-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-zj-3.0.937.tar", last modified: Tue Jul 18 00:36:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-zj-3.0.938.tar", last modified: Wed Jul 19 00:54:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-zj-3.0.937.tar` & `tencentcloud-sdk-python-zj-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19323 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/zj_client.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   114355 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:36:07.000000 tencentcloud-sdk-python-zj-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19407 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/zj_client.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   114355 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:54:35.000000 tencentcloud-sdk-python-zj-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-zj-3.0.937/setup.py` & `tencentcloud-sdk-python-zj-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-zj-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-zj-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/zj_client.py` & `tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/zj_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddCrowdPackInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddSmsSign(self, request):
         """创建普通短信签名信息
 
         :param request: Request instance for AddSmsSign.
         :type request: :class:`tencentcloud.zj.v20190121.models.AddSmsSignRequest`
@@ -65,15 +65,15 @@
             model = models.AddSmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddSmsTemplate(self, request):
         """根据短信标题、模板内容等创建短信模板
 
         :param request: Request instance for AddSmsTemplate.
         :type request: :class:`tencentcloud.zj.v20190121.models.AddSmsTemplateRequest`
@@ -88,15 +88,15 @@
             model = models.AddSmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelCampaign(self, request):
         """取消短信推送活动
 
         :param request: Request instance for CancelCampaign.
         :type request: :class:`tencentcloud.zj.v20190121.models.CancelCampaignRequest`
@@ -111,15 +111,15 @@
             model = models.CancelCampaignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCampaign(self, request):
         """创建短信推送活动
 
         :param request: Request instance for CreateCampaign.
         :type request: :class:`tencentcloud.zj.v20190121.models.CreateCampaignRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCampaignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMmsInstance(self, request):
         """创建超级短信的素材样例内容
 
         :param request: Request instance for CreateMmsInstance.
         :type request: :class:`tencentcloud.zj.v20190121.models.CreateMmsInstanceRequest`
@@ -157,15 +157,15 @@
             model = models.CreateMmsInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DelCrowdPack(self, request):
         """删除人群包
 
         :param request: Request instance for DelCrowdPack.
         :type request: :class:`tencentcloud.zj.v20190121.models.DelCrowdPackRequest`
@@ -180,15 +180,15 @@
             model = models.DelCrowdPackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DelTemplate(self, request):
         """删除短信模板
 
         :param request: Request instance for DelTemplate.
         :type request: :class:`tencentcloud.zj.v20190121.models.DelTemplateRequest`
@@ -203,15 +203,15 @@
             model = models.DelTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMmsInstance(self, request):
         """删除超级短信样例
 
         :param request: Request instance for DeleteMmsInstance.
         :type request: :class:`tencentcloud.zj.v20190121.models.DeleteMmsInstanceRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteMmsInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMmsInstanceInfo(self, request):
         """获取彩信实例信息
 
         :param request: Request instance for DescribeMmsInstanceInfo.
         :type request: :class:`tencentcloud.zj.v20190121.models.DescribeMmsInstanceInfoRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeMmsInstanceInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMmsInstanceList(self, request):
         """获取彩信实例列表
 
         :param request: Request instance for DescribeMmsInstanceList.
         :type request: :class:`tencentcloud.zj.v20190121.models.DescribeMmsInstanceListRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeMmsInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsCampaignStatistics(self, request):
         """获取短信超短活动统计数据
 
         :param request: Request instance for DescribeSmsCampaignStatistics.
         :type request: :class:`tencentcloud.zj.v20190121.models.DescribeSmsCampaignStatisticsRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeSmsCampaignStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsSignList(self, request):
         """获取普通短信签名信息
 
         :param request: Request instance for DescribeSmsSignList.
         :type request: :class:`tencentcloud.zj.v20190121.models.DescribeSmsSignListRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeSmsSignListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsTemplateList(self, request):
         """获取模板信息
 
         :param request: Request instance for DescribeSmsTemplateList.
         :type request: :class:`tencentcloud.zj.v20190121.models.DescribeSmsTemplateListRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeSmsTemplateListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCrowdPackList(self, request):
         """获取人群包列表接口
 
         :param request: Request instance for GetCrowdPackList.
         :type request: :class:`tencentcloud.zj.v20190121.models.GetCrowdPackListRequest`
@@ -364,15 +364,15 @@
             model = models.GetCrowdPackListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCrowdUploadInfo(self, request):
         """获取短信人群包cos上传需要的信息
 
         :param request: Request instance for GetCrowdUploadInfo.
         :type request: :class:`tencentcloud.zj.v20190121.models.GetCrowdUploadInfoRequest`
@@ -387,15 +387,15 @@
             model = models.GetCrowdUploadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSmsAmountInfo(self, request):
         """获取账号短信额度配置信息
 
         :param request: Request instance for GetSmsAmountInfo.
         :type request: :class:`tencentcloud.zj.v20190121.models.GetSmsAmountInfoRequest`
@@ -410,15 +410,15 @@
             model = models.GetSmsAmountInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSmsCampaignStatus(self, request):
         """获取短信活动状态信息
 
         :param request: Request instance for GetSmsCampaignStatus.
         :type request: :class:`tencentcloud.zj.v20190121.models.GetSmsCampaignStatusRequest`
@@ -433,15 +433,15 @@
             model = models.GetSmsCampaignStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySmsTemplate(self, request):
         """对未审核或者审核未通过的短信模板内容进行编辑修改
 
         :param request: Request instance for ModifySmsTemplate.
         :type request: :class:`tencentcloud.zj.v20190121.models.ModifySmsTemplateRequest`
@@ -456,15 +456,15 @@
             model = models.ModifySmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PushMmsContent(self, request):
         """推送超级短信
 
         :param request: Request instance for PushMmsContent.
         :type request: :class:`tencentcloud.zj.v20190121.models.PushMmsContentRequest`
@@ -479,15 +479,15 @@
             model = models.PushMmsContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSms(self, request):
         """发送短信
 
         :param request: Request instance for SendSms.
         :type request: :class:`tencentcloud.zj.v20190121.models.SendSmsRequest`
@@ -502,8 +502,8 @@
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

### Comparing `tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/errorcodes.py` & `tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-zj-3.0.937/tencentcloud/zj/v20190121/models.py` & `tencentcloud-sdk-python-zj-3.0.938/tencentcloud/zj/v20190121/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-zj-3.0.937/tencentcloud_sdk_python_zj.egg-info/PKG-INFO` & `tencentcloud-sdk-python-zj-3.0.938/tencentcloud_sdk_python_zj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-zj
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Zj SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-zj-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-zj-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-zj
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Zj SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-zj-3.0.937/README.rst` & `tencentcloud-sdk-python-zj-3.0.938/README.rst`

 * *Files identical despite different names*

