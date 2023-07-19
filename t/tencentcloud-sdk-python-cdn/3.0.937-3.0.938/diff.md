# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.937.tar", last modified: Tue Jul 18 00:19:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.938.tar", last modified: Wed Jul 19 00:23:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.937.tar` & `tencentcloud-sdk-python-cdn-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82139 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)    22160 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   854003 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82463 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)    22160 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   854003 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:23:34.000000 tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/setup.py` & `tencentcloud-sdk-python-cdn-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddCLSTopicDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddCdnDomain(self, request):
         """AddCdnDomain 用于新增内容分发网络加速域名。1分钟内最多可新增100个域名。
 
         :param request: Request instance for AddCdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.AddCdnDomainRequest`
@@ -65,15 +65,15 @@
             model = models.AddCdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClsLogTopic(self, request):
         """CreateClsLogTopic 用于创建日志主题。注意：一个日志集下至多可创建10个日志主题。
 
         :param request: Request instance for CreateClsLogTopic.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateClsLogTopicRequest`
@@ -88,15 +88,15 @@
             model = models.CreateClsLogTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDiagnoseUrl(self, request):
         """CreateDiagnoseUrl 用于添加域名诊断任务URL， <font color=red>将于 **2023年5月31日** 下线</font><br>
 
         :param request: Request instance for CreateDiagnoseUrl.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateDiagnoseUrlRequest`
@@ -111,15 +111,15 @@
             model = models.CreateDiagnoseUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgePackTask(self, request):
         """动态打包任务提交接口
 
         :param request: Request instance for CreateEdgePackTask.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateEdgePackTaskRequest`
@@ -134,15 +134,15 @@
             model = models.CreateEdgePackTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScdnDomain(self, request):
         """CreateScdnDomain 用于创建 SCDN 加速域名
 
         :param request: Request instance for CreateScdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateScdnDomainRequest`
@@ -157,15 +157,15 @@
             model = models.CreateScdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScdnFailedLogTask(self, request):
         """CreateScdnFailedLogTask 用于重试创建失败的事件日志任务
 
         :param request: Request instance for CreateScdnFailedLogTask.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateScdnFailedLogTaskRequest`
@@ -180,15 +180,15 @@
             model = models.CreateScdnFailedLogTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScdnLogTask(self, request):
         """CreateScdnLogTask 用于创建事件日志任务
 
         :param request: Request instance for CreateScdnLogTask.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateScdnLogTaskRequest`
@@ -203,15 +203,15 @@
             model = models.CreateScdnLogTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVerifyRecord(self, request):
         """CreateVerifyRecord 用于生成一条子域名解析，提示客户添加到域名解析上，用于泛域名及域名取回校验归属权。
         生成的解析记录可通过 [VerifyDomainRecord](https://cloud.tencent.com/document/product/228/48117) 完成归属权校验。
         注意：生成的解析记录有效期为24小时，超过24小时后，需重新生成。
         具体流程可参考：[使用API接口进行域名归属校验](https://cloud.tencent.com/document/product/228/61702#.E6.96.B9.E6.B3.95.E4.B8.89.EF.BC.9Aapi-.E6.8E.A5.E5.8F.A3.E6.93.8D.E4.BD.9C)
@@ -229,15 +229,15 @@
             model = models.CreateVerifyRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCdnDomain(self, request):
         """DeleteCdnDomain 用于删除指定加速域名
 
         :param request: Request instance for DeleteCdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DeleteCdnDomainRequest`
@@ -252,15 +252,15 @@
             model = models.DeleteCdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClsLogTopic(self, request):
         """DeleteClsLogTopic 用于删除日志主题。注意：删除后，所有该日志主题下绑定域名的日志将不再继续投递至该主题，已经投递的日志将会被全部清空。生效时间约为 5~15 分钟。
 
         :param request: Request instance for DeleteClsLogTopic.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DeleteClsLogTopicRequest`
@@ -275,15 +275,15 @@
             model = models.DeleteClsLogTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScdnDomain(self, request):
         """删除SCDN域名
 
         :param request: Request instance for DeleteScdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DeleteScdnDomainRequest`
@@ -298,15 +298,15 @@
             model = models.DeleteScdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillingData(self, request):
         """DescribeBillingData 用于查询实际计费数据明细。
 
         :param request: Request instance for DescribeBillingData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeBillingDataRequest`
@@ -321,15 +321,15 @@
             model = models.DescribeBillingDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcData(self, request):
         """CC统计数据查询
 
         :param request: Request instance for DescribeCcData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeCcDataRequest`
@@ -344,15 +344,15 @@
             model = models.DescribeCcDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCdnData(self, request):
         """DescribeCdnData 用于查询 CDN 实时访问监控数据，支持以下指标查询：
 
         + 流量（单位为 byte）
         + 带宽（单位为 bps）
@@ -379,15 +379,15 @@
             model = models.DescribeCdnDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCdnDomainLogs(self, request):
         """DescribeCdnDomainLogs 用于查询访问日志下载地址，仅支持 30 天以内的境内、境外访问日志下载链接查询。
 
         :param request: Request instance for DescribeCdnDomainLogs.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeCdnDomainLogsRequest`
@@ -402,15 +402,15 @@
             model = models.DescribeCdnDomainLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCdnIp(self, request):
         """DescribeCdnIp 用于查询 CDN IP 归属。
         （注意：此接口请求频率限制以 CDN 侧限制为准：200次/10分钟）
 
         :param request: Request instance for DescribeCdnIp.
@@ -426,15 +426,15 @@
             model = models.DescribeCdnIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCdnOriginIp(self, request):
         """本接口（DescribeCdnOriginIp）用于查询 CDN 回源节点的IP信息。（注：此接口即将下线，不再进行维护，请通过DescribeIpStatus 接口进行查询）
 
         :param request: Request instance for DescribeCdnOriginIp.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeCdnOriginIpRequest`
@@ -449,15 +449,15 @@
             model = models.DescribeCdnOriginIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertDomains(self, request):
         """DescribeCertDomains 用于校验SSL证书并提取证书中包含的域名。
 
         :param request: Request instance for DescribeCertDomains.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeCertDomainsRequest`
@@ -472,15 +472,15 @@
             model = models.DescribeCertDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSData(self, request):
         """DDoS统计数据查询
 
         :param request: Request instance for DescribeDDoSData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeDDoSDataRequest`
@@ -495,15 +495,15 @@
             model = models.DescribeDDoSDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiagnoseReport(self, request):
         """DescribeDiagnoseReport 用于获取指定报告id的内容， <font color=red>将于 **2023年5月31日** 下线</font><br>
 
         :param request: Request instance for DescribeDiagnoseReport.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeDiagnoseReportRequest`
@@ -518,15 +518,15 @@
             model = models.DescribeDiagnoseReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDistrictIspData(self, request):
         """查询指定域名的区域、运营商明细数据
         注意事项：接口尚未全面开放，未在内测名单中的账号不支持调用
 
         :param request: Request instance for DescribeDistrictIspData.
@@ -542,15 +542,15 @@
             model = models.DescribeDistrictIspDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomains(self, request):
         """DescribeDomains 用于查询内容分发网络加速域名（含境内、境外）基本配置信息，包括项目ID、服务状态，业务类型、创建时间、更新时间等信息。
 
         :param request: Request instance for DescribeDomains.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeDomainsRequest`
@@ -565,15 +565,15 @@
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
         """DescribeDomainsConfig 用于查询内容分发网络加速域名（含境内、境外）的所有配置信息。
 
         :param request: Request instance for DescribeDomainsConfig.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeDomainsConfigRequest`
@@ -588,15 +588,15 @@
             model = models.DescribeDomainsConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgePackTaskStatus(self, request):
         """DescribeEdgePackTaskStatus 用于查询动态打包任务状态列表
 
         :param request: Request instance for DescribeEdgePackTaskStatus.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeEdgePackTaskStatusRequest`
@@ -611,15 +611,15 @@
             model = models.DescribeEdgePackTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEventLogData(self, request):
         """DescribeEventLogData 用于查询事件日志统计曲线
 
         :param request: Request instance for DescribeEventLogData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeEventLogDataRequest`
@@ -634,15 +634,15 @@
             model = models.DescribeEventLogDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHttpsPackages(self, request):
         """DescribeHttpsPackages 用于查询 CDN HTTPS请求包详情。
 
         :param request: Request instance for DescribeHttpsPackages.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeHttpsPackagesRequest`
@@ -657,15 +657,15 @@
             model = models.DescribeHttpsPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageConfig(self, request):
         """DescribeImageConfig 用于获取域名图片优化的当前配置，支持Webp、TPG、 Guetzli 和 Avif。
 
         :param request: Request instance for DescribeImageConfig.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeImageConfigRequest`
@@ -680,15 +680,15 @@
             model = models.DescribeImageConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpStatus(self, request):
         """DescribeIpStatus 用于查询域名所在加速平台的边缘节点、回源节点明细。注意事项：暂不支持查询边缘节点信息并且数据会存在一定延迟。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/41954"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
@@ -705,15 +705,15 @@
             model = models.DescribeIpStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpVisit(self, request):
         """DescribeIpVisit 用于查询 5 分钟活跃用户数，及日活跃用户数明细
 
         + 5 分钟活跃用户数：根据日志中客户端 IP，5 分钟粒度去重统计
         + 日活跃用户数：根据日志中客户端 IP，按天粒度去重统计
@@ -731,15 +731,15 @@
             model = models.DescribeIpVisitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMapInfo(self, request):
         """DescribeMapInfo 用于查询省份对应的 ID，运营商对应的 ID 信息。
 
         :param request: Request instance for DescribeMapInfo.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeMapInfoRequest`
@@ -754,15 +754,15 @@
             model = models.DescribeMapInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOriginData(self, request):
         """DescribeOriginData 用于查询 CDN 实时回源监控数据，支持以下指标查询：
 
         + 回源流量（单位为 byte）
         + 回源带宽（单位为 bps）
@@ -787,15 +787,15 @@
             model = models.DescribeOriginDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePayType(self, request):
         """DescribePayType 用于查询用户的计费类型，计费周期等信息。
 
         :param request: Request instance for DescribePayType.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribePayTypeRequest`
@@ -810,15 +810,15 @@
             model = models.DescribePayTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurgeQuota(self, request):
         """DescribePurgeQuota 用于查询账户刷新配额和每日可用量。
 
         :param request: Request instance for DescribePurgeQuota.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribePurgeQuotaRequest`
@@ -833,15 +833,15 @@
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
         """DescribePurgeTasks 用于查询提交的 URL 刷新、目录刷新记录及执行进度，通过 PurgePathCache 与 PurgeUrlsCache 接口提交的任务均可通过此接口进行查询。
 
         :param request: Request instance for DescribePurgeTasks.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribePurgeTasksRequest`
@@ -856,15 +856,15 @@
             model = models.DescribePurgeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushQuota(self, request):
         """DescribePushQuota  用于查询预热配额和每日可用量。
 
         :param request: Request instance for DescribePushQuota.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribePushQuotaRequest`
@@ -879,15 +879,15 @@
             model = models.DescribePushQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushTasks(self, request):
         """DescribePushTasks  用于查询预热任务提交历史记录及执行进度。
 
         :param request: Request instance for DescribePushTasks.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribePushTasksRequest`
@@ -902,15 +902,15 @@
             model = models.DescribePushTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReportData(self, request):
         """DescribeReportData 用于查询域名/项目维度的日/周/月报表数据。
 
         :param request: Request instance for DescribeReportData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeReportDataRequest`
@@ -925,15 +925,15 @@
             model = models.DescribeReportDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScdnBotData(self, request):
         """获取BOT统计数据列表
 
         :param request: Request instance for DescribeScdnBotData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeScdnBotDataRequest`
@@ -948,15 +948,15 @@
             model = models.DescribeScdnBotDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScdnBotRecords(self, request):
         """查询BOT会话记录列表
 
         :param request: Request instance for DescribeScdnBotRecords.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeScdnBotRecordsRequest`
@@ -971,15 +971,15 @@
             model = models.DescribeScdnBotRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScdnConfig(self, request):
         """DescribeScdnConfig 用于查询指定 SCDN 加速域名的安全相关配置
 
         :param request: Request instance for DescribeScdnConfig.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeScdnConfigRequest`
@@ -994,15 +994,15 @@
             model = models.DescribeScdnConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScdnIpStrategy(self, request):
         """查询在SCDN IP安全策略
 
         :param request: Request instance for DescribeScdnIpStrategy.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeScdnIpStrategyRequest`
@@ -1017,15 +1017,15 @@
             model = models.DescribeScdnIpStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScdnTopData(self, request):
         """获取SCDN的Top数据
 
         :param request: Request instance for DescribeScdnTopData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeScdnTopDataRequest`
@@ -1040,15 +1040,15 @@
             model = models.DescribeScdnTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopData(self, request):
         """DescribeTopData 通过入参 Metric 和 Filter 组合不同，可以查询以下排序数据：
 
         + 依据总流量、总请求数对访问 IP 排序，从大至小返回 TOP 100 IP
         + 依据总流量、总请求数对访问 Refer 排序，从大至小返回 TOP 100 Refer
@@ -1073,15 +1073,15 @@
             model = models.DescribeTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficPackages(self, request):
         """DescribeTrafficPackages 用于查询 CDN 流量包详情。
 
         :param request: Request instance for DescribeTrafficPackages.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeTrafficPackagesRequest`
@@ -1096,15 +1096,15 @@
             model = models.DescribeTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUrlViolations(self, request):
         """DescribeUrlViolations 用于查询被 CDN 系统扫描到的域名违规 URL 列表及当前状态。
         对应内容分发网络控制台【图片鉴黄】页面。
 
         :param request: Request instance for DescribeUrlViolations.
@@ -1120,15 +1120,15 @@
             model = models.DescribeUrlViolationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWafData(self, request):
         """Waf统计数据查询
 
         :param request: Request instance for DescribeWafData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeWafDataRequest`
@@ -1143,15 +1143,15 @@
             model = models.DescribeWafDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableCaches(self, request):
         """DisableCaches 用于禁用 CDN 上指定 URL 的访问，禁用完成后，中国境内访问会直接返回 403。（注：接口尚在内测中，暂未全量开放；封禁URL并非无限期永久封禁）
 
         :param request: Request instance for DisableCaches.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DisableCachesRequest`
@@ -1166,15 +1166,15 @@
             model = models.DisableCachesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableClsLogTopic(self, request):
         """DisableClsLogTopic 用于停止日志主题投递。注意：停止后，所有绑定该日志主题域名的日志将不再继续投递至该主题，已经投递的日志将会继续保留。生效时间约为 5~15 分钟。
 
         :param request: Request instance for DisableClsLogTopic.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DisableClsLogTopicRequest`
@@ -1189,15 +1189,15 @@
             model = models.DisableClsLogTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DuplicateDomainConfig(self, request):
         """拷贝参考域名的配置至新域名。暂不支持自有证书以及定制化配置
 
         :param request: Request instance for DuplicateDomainConfig.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DuplicateDomainConfigRequest`
@@ -1212,15 +1212,15 @@
             model = models.DuplicateDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableCaches(self, request):
         """EnableCaches 用于解禁手工封禁的 URL，解禁成功后，全网生效时间约 5~10 分钟。（接口尚在内测中，暂未全量开放使用）
 
         :param request: Request instance for EnableCaches.
         :type request: :class:`tencentcloud.cdn.v20180606.models.EnableCachesRequest`
@@ -1235,15 +1235,15 @@
             model = models.EnableCachesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableClsLogTopic(self, request):
         """EnableClsLogTopic 用于启动日志主题投递。注意：启动后，所有绑定该日志主题域名的日志将继续投递至该主题。生效时间约为 5~15 分钟。
 
         :param request: Request instance for EnableClsLogTopic.
         :type request: :class:`tencentcloud.cdn.v20180606.models.EnableClsLogTopicRequest`
@@ -1258,15 +1258,15 @@
             model = models.EnableClsLogTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDisableRecords(self, request):
         """GetDisableRecords 用于查询资源禁用历史，及 URL 当前状态。（接口尚在内测中，暂未全量开放使用）
 
         :param request: Request instance for GetDisableRecords.
         :type request: :class:`tencentcloud.cdn.v20180606.models.GetDisableRecordsRequest`
@@ -1281,15 +1281,15 @@
             model = models.GetDisableRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListClsLogTopics(self, request):
         """ListClsLogTopics 用于显示日志主题列表。注意：一个日志集下至多含10个日志主题。
 
         :param request: Request instance for ListClsLogTopics.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListClsLogTopicsRequest`
@@ -1304,15 +1304,15 @@
             model = models.ListClsLogTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListClsTopicDomains(self, request):
         """ListClsTopicDomains 用于获取某日志主题下绑定的域名列表。
 
         :param request: Request instance for ListClsTopicDomains.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListClsTopicDomainsRequest`
@@ -1327,15 +1327,15 @@
             model = models.ListClsTopicDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListDiagnoseReport(self, request):
         """ListDiagnoseReport 用于获取用户诊断URL访问后各个子任务的简要详情， <font color=red>将于 **2023年5月31日** 下线</font><br>
 
         :param request: Request instance for ListDiagnoseReport.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListDiagnoseReportRequest`
@@ -1350,15 +1350,15 @@
             model = models.ListDiagnoseReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListScdnDomains(self, request):
         """ListScdnDomains 用于查询 SCDN 安全加速域名列表，及域名基本配置信息
 
         :param request: Request instance for ListScdnDomains.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListScdnDomainsRequest`
@@ -1373,15 +1373,15 @@
             model = models.ListScdnDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListScdnLogTasks(self, request):
         """ListScdnLogTasks 用于查询SCDN日志下载任务列表,以及展示下载任务基本信息
 
         :param request: Request instance for ListScdnLogTasks.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListScdnLogTasksRequest`
@@ -1396,15 +1396,15 @@
             model = models.ListScdnLogTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListScdnTopBotData(self, request):
         """获取Bot攻击的Top数据列表
 
         :param request: Request instance for ListScdnTopBotData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListScdnTopBotDataRequest`
@@ -1419,15 +1419,15 @@
             model = models.ListScdnTopBotDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopBotData(self, request):
         """获取Bot攻击的Top信息
 
         :param request: Request instance for ListTopBotData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListTopBotDataRequest`
@@ -1442,15 +1442,15 @@
             model = models.ListTopBotDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopCcData(self, request):
         """获取CC攻击Top数据
 
         :param request: Request instance for ListTopCcData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListTopCcDataRequest`
@@ -1465,15 +1465,15 @@
             model = models.ListTopCcDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopClsLogData(self, request):
         """通过CLS日志计算Top信息。支持近7天的日志数据。
 
         :param request: Request instance for ListTopClsLogData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListTopClsLogDataRequest`
@@ -1488,15 +1488,15 @@
             model = models.ListTopClsLogDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopDDoSData(self, request):
         """获取DDoS攻击Top数据
 
         :param request: Request instance for ListTopDDoSData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListTopDDoSDataRequest`
@@ -1511,15 +1511,15 @@
             model = models.ListTopDDoSDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopData(self, request):
         """ListTopData 通过入参 Metric 和 Filter 组合不同，可以查询以下排序数据：
 
         + 依据总流量、总请求数对访问 URL 排序，从大至小返回 TOP 1000 URL
         + 依据总流量、总请求数对客户端省份排序，从大至小返回省份列表
@@ -1542,15 +1542,15 @@
             model = models.ListTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopWafData(self, request):
         """获取Waf攻击Top数据
 
         :param request: Request instance for ListTopWafData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ListTopWafDataRequest`
@@ -1565,15 +1565,15 @@
             model = models.ListTopWafDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageClsTopicDomains(self, request):
         """ManageClsTopicDomains 用于管理某日志主题下绑定的域名列表。
 
         :param request: Request instance for ManageClsTopicDomains.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ManageClsTopicDomainsRequest`
@@ -1588,15 +1588,15 @@
             model = models.ManageClsTopicDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainConfig(self, request):
         """ModifyDomainConfig 用于修改内容分发网络加速域名配置信息
         注意：
         Route 字段，使用点分隔，最后一段称为叶子节点，非叶子节点配置保持不变；
         Value 字段，使用 json 进行序列化，其中固定 update 作为 key，配置路径值参考 https://cloud.tencent.com/document/product/228/41116 接口各配置项复杂类型，为配置路径对应复杂类型下的节点。
@@ -1615,15 +1615,15 @@
             model = models.ModifyDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPurgeFetchTaskStatus(self, request):
         """ModifyPurgeFetchTaskStatus 用于上报定时刷新预热任务执行状态
 
         :param request: Request instance for ModifyPurgeFetchTaskStatus.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ModifyPurgeFetchTaskStatusRequest`
@@ -1638,15 +1638,15 @@
             model = models.ModifyPurgeFetchTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PurgePathCache(self, request):
         """PurgePathCache 用于批量提交目录刷新，根据域名的加速区域进行对应区域的刷新。
         默认情况下境内、境外加速区域每日目录刷新额度为各 100 条，每次最多可提交 500 条。
 
         :param request: Request instance for PurgePathCache.
@@ -1662,15 +1662,15 @@
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
         """PurgeUrlsCache 用于批量提交 URL 进行刷新，根据 URL 中域名的当前加速区域进行对应区域的刷新。
         默认情况下境内、境外加速区域每日 URL 刷新额度各为 10000 条，每次最多可提交 1000 条。
 
         :param request: Request instance for PurgeUrlsCache.
@@ -1686,15 +1686,15 @@
             model = models.PurgeUrlsCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PushUrlsCache(self, request):
         """PushUrlsCache 用于将指定 URL 资源列表加载至 CDN 节点，支持指定加速区域预热。
         默认情况下境内、境外每日预热 URL 限额为各 1000 条，每次最多可提交 500 条。注意：中国境外区域预热，资源默认加载至中国境外边缘节点，所产生的边缘层流量会计入计费流量。
 
         :param request: Request instance for PushUrlsCache.
@@ -1710,15 +1710,15 @@
             model = models.PushUrlsCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchClsLog(self, request):
         """SearchClsLog 用于 CLS 日志检索。支持检索今天，24小时（可选近7中的某一天），近7天的日志数据。
 
         :param request: Request instance for SearchClsLog.
         :type request: :class:`tencentcloud.cdn.v20180606.models.SearchClsLogRequest`
@@ -1733,15 +1733,15 @@
             model = models.SearchClsLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartCdnDomain(self, request):
         """StartCdnDomain 用于启用已停用域名的加速服务
 
         :param request: Request instance for StartCdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.StartCdnDomainRequest`
@@ -1756,15 +1756,15 @@
             model = models.StartCdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartScdnDomain(self, request):
         """StartScdnDomain 用于开启域名的安全防护配置
 
         :param request: Request instance for StartScdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.StartScdnDomainRequest`
@@ -1779,15 +1779,15 @@
             model = models.StartScdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopCdnDomain(self, request):
         """StopCdnDomain 用于停止域名的加速服务。
         注意：停止加速服务后，访问至加速节点的请求将会直接返回 404。为避免对您的业务造成影响，请在停止加速服务前将解析切走。
 
         :param request: Request instance for StopCdnDomain.
@@ -1803,15 +1803,15 @@
             model = models.StopCdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopScdnDomain(self, request):
         """StopScdnDomain 用于关闭域名的安全防护配置
 
         :param request: Request instance for StopScdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.StopScdnDomainRequest`
@@ -1826,15 +1826,15 @@
             model = models.StopScdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDomainConfig(self, request):
         """UpdateDomainConfig 用于修改内容分发网络加速域名配置信息。
         注意：如果需要更新复杂类型的配置项，必须传递整个对象的所有属性，未传递的属性将使用默认值，建议通过查询接口获取配置属性后，直接修改后传递给本接口。
         云审计相关：接口的入参可能包含密钥等敏感信息，所以此接口的入参不会上报到云审计。
 
@@ -1851,15 +1851,15 @@
             model = models.UpdateDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateImageConfig(self, request):
         """UpdateImageConfig 用于更新控制台图片优化的相关配置，支持Webp、TPG、 Guetzli 和 Avif。
 
         :param request: Request instance for UpdateImageConfig.
         :type request: :class:`tencentcloud.cdn.v20180606.models.UpdateImageConfigRequest`
@@ -1874,15 +1874,15 @@
             model = models.UpdateImageConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePayType(self, request):
         """本接口(UpdatePayType)用于修改账号计费类型，暂不支持月结用户或子账号修改。
 
         :param request: Request instance for UpdatePayType.
         :type request: :class:`tencentcloud.cdn.v20180606.models.UpdatePayTypeRequest`
@@ -1897,15 +1897,15 @@
             model = models.UpdatePayTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScdnDomain(self, request):
         """UpdateScdnDomain 用于修改 SCDN 加速域名安全相关配置
 
         :param request: Request instance for UpdateScdnDomain.
         :type request: :class:`tencentcloud.cdn.v20180606.models.UpdateScdnDomainRequest`
@@ -1920,15 +1920,15 @@
             model = models.UpdateScdnDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyDomainRecord(self, request):
         """VerifyDomainRecord 用于验证域名解析值。
         验证域名解析记录值前，您需要通过 [CreateVerifyRecord](https://cloud.tencent.com/document/product/228/48118) 生成校验解析值，验证通过后，24小时有效。
         具体流程可参考：[使用API接口进行域名归属校验](https://cloud.tencent.com/document/product/228/61702#.E6.96.B9.E6.B3.95.E4.B8.89.EF.BC.9Aapi-.E6.8E.A5.E5.8F.A3.E6.93.8D.E4.BD.9C)
 
@@ -1945,8 +1945,8 @@
             model = models.VerifyDomainRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/cdn/v20180606/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/README.rst` & `tencentcloud-sdk-python-cdn-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.938/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

