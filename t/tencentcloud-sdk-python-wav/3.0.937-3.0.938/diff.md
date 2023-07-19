# Comparing `tmp/tencentcloud-sdk-python-wav-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-wav-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.937.tar", last modified: Tue Jul 18 00:35:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.938.tar", last modified: Wed Jul 19 00:53:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wav-3.0.937.tar` & `tencentcloud-sdk-python-wav-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229425 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/models.py
--rw-r--r--   0 root         (0) root         (0)    25908 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/wav_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229425 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/models.py
+-rw-r--r--   0 root         (0) root         (0)    26012 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/wav_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:56.000000 tencentcloud-sdk-python-wav-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-wav-3.0.937/setup.py` & `tencentcloud-sdk-python-wav-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wav-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/errorcodes.py` & `tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/models.py` & `tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/wav_client.py` & `tencentcloud-sdk-python-wav-3.0.938/tencentcloud/wav/v20210129/wav_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateChannelCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCorpTag(self, request):
         """该接口用户设置标签库, 每个企业最多可配置3000个企业标签。
 
         :param request: Request instance for CreateCorpTag.
         :type request: :class:`tencentcloud.wav.v20210129.models.CreateCorpTagRequest`
@@ -65,15 +65,15 @@
             model = models.CreateCorpTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLead(self, request):
         """线索回收接口
 
         :param request: Request instance for CreateLead.
         :type request: :class:`tencentcloud.wav.v20210129.models.CreateLeadRequest`
@@ -88,15 +88,15 @@
             model = models.CreateLeadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryActivityJoinList(self, request):
         """根据游标拉取活动参与列表信息
 
         :param request: Request instance for QueryActivityJoinList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryActivityJoinListRequest`
@@ -111,15 +111,15 @@
             model = models.QueryActivityJoinListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryActivityList(self, request):
         """根据游标拉取活动列表信息
 
         :param request: Request instance for QueryActivityList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryActivityListRequest`
@@ -134,15 +134,15 @@
             model = models.QueryActivityListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryActivityLiveCodeList(self, request):
         """根据游标拉取活动活码列表信息
 
         :param request: Request instance for QueryActivityLiveCodeList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryActivityLiveCodeListRequest`
@@ -157,15 +157,15 @@
             model = models.QueryActivityLiveCodeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryArrivalList(self, request):
         """查询指定时间范围内发生过到店的潜客到店信息
 
         :param request: Request instance for QueryArrivalList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryArrivalListRequest`
@@ -180,15 +180,15 @@
             model = models.QueryArrivalListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChannelCodeList(self, request):
         """根据游标拉取渠道活码列表信息
 
         :param request: Request instance for QueryChannelCodeList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryChannelCodeListRequest`
@@ -203,15 +203,15 @@
             model = models.QueryChannelCodeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryChatArchivingList(self, request):
         """根据游标拉取会话存档列表信息
 
         :param request: Request instance for QueryChatArchivingList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryChatArchivingListRequest`
@@ -226,15 +226,15 @@
             model = models.QueryChatArchivingListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryClueInfoList(self, request):
         """企业可通过此接口获取线索列表。
 
         :param request: Request instance for QueryClueInfoList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryClueInfoListRequest`
@@ -249,15 +249,15 @@
             model = models.QueryClueInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCrmStatistics(self, request):
         """通过接口拉取租户/指定成员/部门在指定日期范围内的CRM跟进统计数据
 
         :param request: Request instance for QueryCrmStatistics.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryCrmStatisticsRequest`
@@ -272,15 +272,15 @@
             model = models.QueryCrmStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCustomerEventDetailStatistics(self, request):
         """通过接口拉取SaaS内C端外部联系人在指定时间范围内的行为事件明细。此接口提供的数据以天为维度，查询的时间范围为[start_time,end_time]，即前后均为闭区间，支持的最大查询跨度为365天。
 
         :param request: Request instance for QueryCustomerEventDetailStatistics.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryCustomerEventDetailStatisticsRequest`
@@ -295,15 +295,15 @@
             model = models.QueryCustomerEventDetailStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCustomerProfileList(self, request):
         """通过接口拉取租户已有潜客客户档案列表信息
 
         :param request: Request instance for QueryCustomerProfileList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryCustomerProfileListRequest`
@@ -318,15 +318,15 @@
             model = models.QueryCustomerProfileListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryDealerInfoList(self, request):
         """企业可通过此接口获取录入在企微SaaS平台上的经销商信息。
 
         :param request: Request instance for QueryDealerInfoList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryDealerInfoListRequest`
@@ -341,15 +341,15 @@
             model = models.QueryDealerInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExternalContactDetail(self, request):
         """企业可通过此接口，根据外部联系人的userid，拉取外部联系人详情
 
         :param request: Request instance for QueryExternalContactDetail.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryExternalContactDetailRequest`
@@ -364,15 +364,15 @@
             model = models.QueryExternalContactDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExternalContactDetailByDate(self, request):
         """企业可通过传入起始和结束时间，获取该时间段的外部联系人详情列表
 
         :param request: Request instance for QueryExternalContactDetailByDate.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryExternalContactDetailByDateRequest`
@@ -387,15 +387,15 @@
             model = models.QueryExternalContactDetailByDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExternalContactList(self, request):
         """企业可通过此接口基于外部联系人获取指定成员添加的客户列表。客户是指配置了客户联系功能的成员所添加的外部联系人。没有配置客户联系功能的成员，所添加的外部联系人将不会作为客户返回。
 
         :param request: Request instance for QueryExternalContactList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryExternalContactListRequest`
@@ -410,15 +410,15 @@
             model = models.QueryExternalContactListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExternalUserEventList(self, request):
         """通过接口拉取租户在指定时间范围内的外部联系人添加/删除明细，此接口提供的数据以天为维度，查询的时间范围为[StarTime, EndTime]，即前后均为闭区间，支持的最大查询跨度为365天；
 
         :param request: Request instance for QueryExternalUserEventList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryExternalUserEventListRequest`
@@ -433,15 +433,15 @@
             model = models.QueryExternalUserEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExternalUserMappingInfo(self, request):
         """企业可通过此接口将企业主体对应的外部联系人id转换为乐销车应用主体对应的外部联系人。
 
         :param request: Request instance for QueryExternalUserMappingInfo.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryExternalUserMappingInfoRequest`
@@ -456,15 +456,15 @@
             model = models.QueryExternalUserMappingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFollowList(self, request):
         """查询指定时间范围内发生过跟进的潜客信息
 
         :param request: Request instance for QueryFollowList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryFollowListRequest`
@@ -479,15 +479,15 @@
             model = models.QueryFollowListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryLicenseInfo(self, request):
         """该接口获取license对应的详细信息
 
         :param request: Request instance for QueryLicenseInfo.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryLicenseInfoRequest`
@@ -502,15 +502,15 @@
             model = models.QueryLicenseInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMaterialList(self, request):
         """通过接口按类型拉取租户当前的素材列表及关键信息
 
         :param request: Request instance for QueryMaterialList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryMaterialListRequest`
@@ -525,15 +525,15 @@
             model = models.QueryMaterialListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMiniAppCodeList(self, request):
         """查询小程序码列表接口
 
         :param request: Request instance for QueryMiniAppCodeList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryMiniAppCodeListRequest`
@@ -548,15 +548,15 @@
             model = models.QueryMiniAppCodeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryStaffEventDetailStatistics(self, request):
         """通过接口拉取SaaS内企业成员在指定时间范围内的行为事件明细。此接口提供的数据以天为维度，查询的时间范围为[start_time,end_time]，即前后均为闭区间，支持的最大查询跨度为365天。
 
         :param request: Request instance for QueryStaffEventDetailStatistics.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryStaffEventDetailStatisticsRequest`
@@ -571,15 +571,15 @@
             model = models.QueryStaffEventDetailStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryUserInfoList(self, request):
         """查询企业成员信息列表接口
 
         :param request: Request instance for QueryUserInfoList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryUserInfoListRequest`
@@ -594,15 +594,15 @@
             model = models.QueryUserInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryVehicleInfoList(self, request):
         """企业可通过此接口获取企微SaaS平台上的车系车型信息。
 
         :param request: Request instance for QueryVehicleInfoList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryVehicleInfoListRequest`
@@ -617,8 +617,8 @@
             model = models.QueryVehicleInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.938/tencentcloud_sdk_python_wav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.937/README.rst` & `tencentcloud-sdk-python-wav-3.0.938/README.rst`

 * *Files identical despite different names*

