# Comparing `tmp/tencentcloud-sdk-python-tiia-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tiia-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.937.tar", last modified: Tue Jul 18 00:33:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.938.tar", last modified: Wed Jul 19 00:50:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiia-3.0.937.tar` & `tencentcloud-sdk-python-tiia-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32443 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/tiia_client.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   146146 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:33:11.000000 tencentcloud-sdk-python-tiia-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32535 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/tiia_client.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   146146 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:50:50.000000 tencentcloud-sdk-python-tiia-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/setup.py` & `tencentcloud-sdk-python-tiia-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.938/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/tiia_client.py` & `tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/tiia_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             model = models.AssessQualityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGroup(self, request):
         """本接口用于创建一个空的图片库，图片库主要用于存储在创建图片时提取的图片特征数据，如果图片库已存在则返回错误。不同的图片库类型对应不同的图像搜索服务类型，根据输入参数GroupType区分。
 
         <table>
             <th>服务类型</th><th>GroupType</th><th>功能描述</th>
@@ -95,15 +95,15 @@
             model = models.CreateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImage(self, request):
         """创建图片，并添加对应图片的自定义信息。模型将在创建图片时自动提取图像特征并存储到指定的图片库中，每创建一张图片会对应提取和存储一条图片特征数据。
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -122,15 +122,15 @@
             model = models.CreateImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CropImage(self, request):
         """根据输入的裁剪比例，智能判断一张图片的最佳裁剪区域，确保原图的主体区域不受影响，以适应不同平台、设备的展示要求，避免简单拉伸带来的变形。
 
         >
         - 可前往 [图像处理](https://cloud.tencent.com/document/product/1590) 产品文档中查看更多产品信息。
@@ -149,15 +149,15 @@
             model = models.CropImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImages(self, request):
         """删除图片。
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -175,15 +175,15 @@
             model = models.DeleteImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroups(self, request):
         """查询所有的图库信息。
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -201,15 +201,15 @@
             model = models.DescribeGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """获取指定图片库中的图片列表。
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -227,15 +227,15 @@
             model = models.DescribeImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectChefDress(self, request):
         """可对图片中厨师穿戴进行识别，支持厨师服识别，厨师帽识别，赤膊识别和口罩识别,可应用于明厨亮灶场景。
         "被优选过滤"标签值在人体优选开关开启时才会返回。
         厨师服：厨师服定义为白色上衣
         厨师服识别(酒店版)：厨师服定义为红色，白色，黑色上衣
@@ -261,15 +261,15 @@
             model = models.DetectChefDressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectDisgust(self, request):
         """输入一张图片，返回AI针对一张图片是否是恶心的一系列判断值。
 
         通过恶心图片识别, 可以判断一张图片是否令人恶心, 同时给出它属于的潜在类别, 让您能够过滤掉使人不愉快的图片。
         >
@@ -288,15 +288,15 @@
             model = models.DetectDisgustResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectEnvelope(self, request):
         """文件封识别可检测图片中是否包含符合文件封（即文件、单据、资料等的袋状包装）特征的物品，覆盖顺丰快递文件封、文件袋、档案袋等多种文件封类型，可应用于物流行业对文件快递的包装审核等场景。
 
         >?
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
@@ -314,15 +314,15 @@
             model = models.DetectEnvelopeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectLabel(self, request):
         """图像标签利用深度学习技术，可以对图片进行智能分类、物体识别等。
 
         目前支持八个大类、六十多个子类、数千个标签，涵盖各种日常场景、动植物、物品、美食等。
 
@@ -359,15 +359,15 @@
             model = models.DetectLabelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectLabelBeta(self, request):
         """图像标签测试接口
 
         >
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
@@ -385,15 +385,15 @@
             model = models.DetectLabelBetaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectLabelPro(self, request):
         """通用图像标签可识别数千种常见物体或场景，覆盖日常物品、场景、动物、植物、食物、饮品、交通工具等多个大类，返回主体的标签名称和所属细分类目等。
 
         >
         - 可前往 [图像标签](https://cloud.tencent.com/document/product/1588) 产品文档中查看更多产品信息。
@@ -412,15 +412,15 @@
             model = models.DetectLabelProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectMisbehavior(self, request):
         """可以识别输入的图片中是否包含不良行为，例如打架斗殴、赌博、抽烟等，可以应用于广告图、直播截图、短视频截图等审核，减少不良行为对平台内容质量的影响，维护健康向上的互联网环境。
         >
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
 
@@ -437,15 +437,15 @@
             model = models.DetectMisbehaviorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectPet(self, request):
         """传入一张图片，识别出图片中是否存在宠物
         >
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
 
@@ -462,15 +462,15 @@
             model = models.DetectPetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectProduct(self, request):
         """本接口支持识别图片中包含的商品，能够输出商品的品类名称、类别，还可以输出商品在图片中的位置。支持一张图片多个商品的识别。
         >?
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
 
@@ -487,15 +487,15 @@
             model = models.DetectProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectProductBeta(self, request):
         """商品识别-微信识物版，基于人工智能技术、海量训练图片、亿级商品库，可以实现全覆盖、细粒度、高准确率的商品识别和商品推荐功能。
         本服务可以识别出图片中的主体位置、主体商品类型，覆盖亿级SKU，输出具体商品的价格、型号等详细信息。
         客户无需自建商品库，即可快速实现商品识别、拍照搜商品等功能。
         >?
@@ -514,15 +514,15 @@
             model = models.DetectProductBetaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectSecurity(self, request):
         """安全属性识别可对图片中人体安全防护属性进行识别，支持识别安全帽，反光衣，护目镜，工服，手套，工地安全带，口罩，抽烟，玩手机等多种属性。
         "被优选过滤"标签值在人体优选开关开启时才会返回。
 
         |序号 | 标签名称 | 标签值 |
@@ -550,15 +550,15 @@
             model = models.DetectSecurityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnhanceImage(self, request):
         """传入一张图片，输出清晰度提升后的图片。
 
         可以消除图片有损压缩导致的噪声，和使用滤镜、拍摄失焦导致的模糊。让图片的边缘和细节更加清晰自然。
 
@@ -579,15 +579,15 @@
             model = models.EnhanceImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecognizeCar(self, request):
         """车辆识别可对图片中车辆的车型进行识别，输出车辆的品牌（如路虎）、车系（如神行者2）、类型（如中型SUV）、颜色和车辆在图中的坐标等信息，覆盖轿车、SUV、大型客车等市面常见车，支持三千多种车辆型号。如果图片中存在多辆车，会分别输出每辆车的车型和坐标。
 
         >?
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
@@ -605,15 +605,15 @@
             model = models.RecognizeCarResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecognizeCarPro(self, request):
         """车辆识别（增强版）在车辆识别的基础上**增加了车牌识别的功能，并升级了车型识别的效果**。可对图片中车辆的车型和车牌进行同时识别，输出车辆的车牌信息，以及车辆品牌（如路虎）、车系（如神行者2）、类型（如中型SUV）、颜色和车辆在图中的坐标等信息，覆盖轿车、SUV、大型客车等市面常见车，支持三千多种车辆型号。如果图片中存在多辆车，会分别输出每辆车的车型、车牌和坐标。
 
         >?
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
@@ -631,15 +631,15 @@
             model = models.RecognizeCarProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchImage(self, request):
         """本接口用于对一张图片，在指定图片库中检索出与之相似的图片列表。
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -658,15 +658,15 @@
             model = models.SearchImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateImage(self, request):
         """本接口支持根据图库ID、物品ID、图片名称来修改图片信息（暂仅支持修改Tags）
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
@@ -685,8 +685,8 @@
             model = models.UpdateImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/errorcodes.py` & `tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/tencentcloud/tiia/v20190529/models.py` & `tencentcloud-sdk-python-tiia-3.0.938/tencentcloud/tiia/v20190529/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.937/README.rst` & `tencentcloud-sdk-python-tiia-3.0.938/README.rst`

 * *Files identical despite different names*

