# Comparing `tmp/tencentcloud-sdk-python-ecdn-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ecdn-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.937.tar", last modified: Tue Jul 18 00:23:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.938.tar", last modified: Wed Jul 19 00:38:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecdn-3.0.937.tar` & `tencentcloud-sdk-python-ecdn-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/
--rw-r--r--   0 root         (0) root         (0)    20260 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/ecdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   120841 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:23:18.000000 tencentcloud-sdk-python-ecdn-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/
+-rw-r--r--   0 root         (0) root         (0)    20324 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/ecdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   120841 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:38:32.000000 tencentcloud-sdk-python-ecdn-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/setup.py` & `tencentcloud-sdk-python-ecdn-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/ecdn_client.py` & `tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/ecdn_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             model = models.AddEcdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVerifyRecord(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         生成一条子域名解析，提示客户添加到域名解析上，用于泛域名及域名取回校验归属权。
 
@@ -73,15 +73,15 @@
             model = models.CreateVerifyRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEcdnDomain(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         本接口（DeleteEcdnDomain）用于删除指定加速域名。待删除域名必须处于已停用状态。
 
@@ -100,15 +100,15 @@
             model = models.DeleteEcdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomains(self, request):
         """本接口（DescribeDomains）用于查询CDN域名基本信息，包括项目id，状态，业务类型，创建时间，更新时间等。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/41118"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -125,15 +125,15 @@
             model = models.DescribeDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainsConfig(self, request):
         """本接口（DescribeDomainsConfig）用于查询CDN加速域名详细配置信息。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/41117"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -150,15 +150,15 @@
             model = models.DescribeDomainsConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEcdnDomainLogs(self, request):
         """本接口（DescribeEcdnDomainLogs）用于查询域名的访问日志下载地址。
 
         :param request: Request instance for DescribeEcdnDomainLogs.
         :type request: :class:`tencentcloud.ecdn.v20191012.models.DescribeEcdnDomainLogsRequest`
@@ -173,15 +173,15 @@
             model = models.DescribeEcdnDomainLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEcdnDomainStatistics(self, request):
         """本接口（DescribeEcdnDomainStatistics）用于查询指定时间段内的域名访问统计指标。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/30986"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -198,15 +198,15 @@
             model = models.DescribeEcdnDomainStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEcdnStatistics(self, request):
         """DescribeEcdnStatistics用于查询 ECDN 实时访问监控数据，支持以下指标查询：
 
         + 流量（单位为 byte）
         + 带宽（单位为 bps）
@@ -229,15 +229,15 @@
             model = models.DescribeEcdnStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpStatus(self, request):
         """DescribeIpStatus 用于查询域名所在加速平台的所有节点信息, 如果您的源站有白名单设置,可以通过本接口获取ECDN服务的节点IP进行加白, 本接口为内测接口,请联系腾讯云工程师开白。
 
         由于产品服务节点常有更新，对于源站开白的使用场景，请定期调用接口获取最新节点信息，若新增服务节点发布7日后您尚未更新加白导致回源失败等问题，ECDN侧不对此承担责任。
 
@@ -254,15 +254,15 @@
             model = models.DescribeIpStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurgeQuota(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         查询刷新接口的用量配额。
 
@@ -281,15 +281,15 @@
             model = models.DescribePurgeQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurgeTasks(self, request):
         """DescribePurgeTasks 用于查询刷新任务提交历史记录及执行进度。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/37873"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -306,15 +306,15 @@
             model = models.DescribePurgeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PurgePathCache(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         PurgePathCache 用于批量刷新目录缓存，一次提交将返回一个刷新任务id。
 
@@ -333,15 +333,15 @@
             model = models.PurgePathCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PurgeUrlsCache(self, request):
         """PurgeUrlsCache 用于批量刷新Url，一次提交将返回一个刷新任务id。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/37870"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -358,15 +358,15 @@
             model = models.PurgeUrlsCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartEcdnDomain(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         本接口（StartEcdnDomain）用于启用加速域名，待启用域名必须处于已下线状态。
 
@@ -385,15 +385,15 @@
             model = models.StartEcdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopEcdnDomain(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         本接口（StopCdnDomain）用于停止加速域名，待停用加速域名必须处于已上线或部署中状态。
 
@@ -412,15 +412,15 @@
             model = models.StopEcdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDomainConfig(self, request):
         """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
 
         本接口（UpdateDomainConfig）用于更新ECDN加速域名配置信息。
         注意：如果需要更新复杂类型的配置项，必须传递整个对象的所有属性，未传递的属性将使用默认值。建议通过查询接口获取配置属性后，直接修改后传递给本接口。Https配置由于证书的特殊性，更新时不用传递证书和密钥字段。
@@ -440,8 +440,8 @@
             model = models.UpdateDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/errorcodes.py` & `tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/ecdn/v20191012/models.py` & `tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/ecdn/v20191012/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecdn-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.937/README.rst` & `tencentcloud-sdk-python-ecdn-3.0.938/README.rst`

 * *Files identical despite different names*

