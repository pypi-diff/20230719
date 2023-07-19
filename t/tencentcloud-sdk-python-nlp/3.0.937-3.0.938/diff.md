# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.937.tar", last modified: Tue Jul 18 00:28:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.938.tar", last modified: Wed Jul 19 00:43:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.937.tar` & `tencentcloud-sdk-python-nlp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49107 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   134539 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49259 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   134539 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:27.000000 tencentcloud-sdk-python-nlp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/setup.py` & `tencentcloud-sdk-python-nlp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AnalyzeSentimentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AutoSummarization(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         利用人工智能算法，自动抽取文本中的关键信息并生成指定长度的文本摘要。可用于新闻标题生成、科技文献摘要生成和商品评论摘要等。
 
@@ -67,15 +67,15 @@
             model = models.AutoSummarizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChatBot(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         闲聊服务基于腾讯领先的NLP引擎能力、数据运算能力和千亿级互联网语料数据的支持，同时集成了广泛的知识问答能力，可实现上百种自定义属性配置，以及儿童语言风格及说话方式，从而让聊天变得更睿智、简单和有趣。
 
@@ -93,15 +93,15 @@
             model = models.ChatBotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClassifyContent(self, request):
         """文本分类接口能够对用户输入的文章进行自动分类，将其映射到具体的类目上，用户只需要提供待分类的文本，而无需关注具体实现。该功能定义了一套较为完备的[三级分类体系](https://cloud.tencent.com/document/product/271/94286)，积累了数百万的语料，经过多轮迭代优化打造了较先进的深度学习模型，以保证效果不断提升。
 
         :param request: Request instance for ClassifyContent.
         :type request: :class:`tencentcloud.nlp.v20190408.models.ClassifyContentRequest`
@@ -116,15 +116,15 @@
             model = models.ClassifyContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ComposeCouplet(self, request):
         """对联生成接口根据用户输入的命题关键词，智能生成一副完整的春联，包括上联、下联和横批。该接口利用先进的自然语言处理技术，确保生成的春联既符合传统对仗、对韵、对义的要求，又具有新意和创意，为用户提供独特的春节祝福。
 
         :param request: Request instance for ComposeCouplet.
         :type request: :class:`tencentcloud.nlp.v20190408.models.ComposeCoupletRequest`
@@ -139,15 +139,15 @@
             model = models.ComposeCoupletResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ComposePoetry(self, request):
         """诗词生成接口利用现代的自然语言处理和深度学习技术，模仿了古代著名诗人的风格，为用户产生独特的诗词。用户只需输入的命题关键词，接口就能自动生成一首七言律诗或五言律诗。
 
         :param request: Request instance for ComposePoetry.
         :type request: :class:`tencentcloud.nlp.v20190408.models.ComposePoetryRequest`
@@ -162,15 +162,15 @@
             model = models.ComposePoetryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDict(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         根据指定的名称、描述创建自定义词库。
 
@@ -187,15 +187,15 @@
             model = models.CreateDictResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWordItems(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         向指定的词库中添加词条。
 
@@ -212,15 +212,15 @@
             model = models.CreateWordItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDict(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         删除自定义词库，会附带相应删除词库包含的所有词条。
 
@@ -237,15 +237,15 @@
             model = models.DeleteDictResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWordItems(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         用于删除自定义词库中的词条。
 
@@ -262,15 +262,15 @@
             model = models.DeleteWordItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DependencyParsing(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         句法依存分析接口能够分析出句子中词与词之间的相互依存关系，并揭示其句法结构，包括主谓关系、动宾关系、核心关系等等，可用于提取句子主干、提取句子核心词等，在机器翻译、自动问答、知识抽取等领域都有很好的应用。
 
@@ -287,15 +287,15 @@
             model = models.DependencyParsingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDict(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         根据id或名称查询自定义词库信息。
 
@@ -312,15 +312,15 @@
             model = models.DescribeDictResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDicts(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         返回属于当前用户的所有自定义词库列表。
 
@@ -337,15 +337,15 @@
             model = models.DescribeDictsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWordItems(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         依据自定义词库的ID，查询对应的词条信息。
 
@@ -362,15 +362,15 @@
             model = models.DescribeWordItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EvaluateSentenceSimilarity(self, request):
         """通过计算句子间的语义相似性，帮助您快速找到文本中重复或相似的句子，用于文本聚类、相似问题检索等应用场景。
 
         :param request: Request instance for EvaluateSentenceSimilarity.
         :type request: :class:`tencentcloud.nlp.v20190408.models.EvaluateSentenceSimilarityRequest`
@@ -385,15 +385,15 @@
             model = models.EvaluateSentenceSimilarityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EvaluateWordSimilarity(self, request):
         """评估两个词语在语义空间的相似程度，为您的场景应用提供有力支持，如关键词过滤、热门话题挖掘等。（目前仅支持中文）
 
         :param request: Request instance for EvaluateWordSimilarity.
         :type request: :class:`tencentcloud.nlp.v20190408.models.EvaluateWordSimilarityRequest`
@@ -408,15 +408,15 @@
             model = models.EvaluateWordSimilarityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateCouplet(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         根据用户输入的命题关键词自动生成一副春联，包括上联、下联和横批。（如需开通请联系商务）
 
@@ -433,15 +433,15 @@
             model = models.GenerateCoupletResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateKeywordSentence(self, request):
         """提取文本中的关键信息，生成简洁明了的关键句子，便于用户快速获取核心观点。
 
         :param request: Request instance for GenerateKeywordSentence.
         :type request: :class:`tencentcloud.nlp.v20190408.models.GenerateKeywordSentenceRequest`
@@ -456,15 +456,15 @@
             model = models.GenerateKeywordSentenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GeneratePoetry(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         根据用户输入的命题关键词自动生成一首七言律诗或五言律诗。（如需开通请联系商务）
 
@@ -481,15 +481,15 @@
             model = models.GeneratePoetryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KeywordsExtraction(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         基于关键词提取平台，通过对文本内容进行深度分析，提取出文本内容中的关键信息，为用户实现诸如新闻内容关键词自动提取、评论关键词提取等提供基础服务。
 
@@ -506,15 +506,15 @@
             model = models.KeywordsExtractionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LexicalAnalysis(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         词法分析接口提供以下三个功能：
 
@@ -539,15 +539,15 @@
             model = models.LexicalAnalysisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseWords(self, request):
         """通过精准地对文本进行分词、词性标注、命名实体识别等功能，助您更好地理解文本内容，挖掘出潜在的价值信息。
 
         :param request: Request instance for ParseWords.
         :type request: :class:`tencentcloud.nlp.v20190408.models.ParseWordsRequest`
@@ -562,15 +562,15 @@
             model = models.ParseWordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetrieveSimilarWords(self, request):
         """基于大数据和深度学习技术，可以快速地找到与给定词语高度相似的其他词语，有助于提高搜索和推荐的准确性。（目前仅支持中文）
 
         :param request: Request instance for RetrieveSimilarWords.
         :type request: :class:`tencentcloud.nlp.v20190408.models.RetrieveSimilarWordsRequest`
@@ -585,15 +585,15 @@
             model = models.RetrieveSimilarWordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchWordItems(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         查询指定自定义词库中的词条是否存在。
 
@@ -610,15 +610,15 @@
             model = models.SearchWordItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SentenceCorrection(self, request):
         """智能识别并纠正句子中的语法、拼写、用词等错误，确保文本的准确性和可读性。
 
         :param request: Request instance for SentenceCorrection.
         :type request: :class:`tencentcloud.nlp.v20190408.models.SentenceCorrectionRequest`
@@ -633,15 +633,15 @@
             model = models.SentenceCorrectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SentenceEmbedding(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         句向量接口能够将输入的句子映射成一个固定维度的向量，用来表示这个句子的语义特征，可用于文本聚类、文本相似度、文本分类等任务，能够显著提高它们的效果。
 
@@ -660,15 +660,15 @@
             model = models.SentenceEmbeddingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SentimentAnalysis(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         情感分析接口能够对带有情感色彩的主观性文本进行分析、处理、归纳和推理，识别出用户的情感倾向，是积极还是消极，并且提供各自概率。
 
@@ -687,15 +687,15 @@
             model = models.SentimentAnalysisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SimilarWords(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         相似词接口能够基于同义词库及词向量技术，检索出与输入词语在语义上最相似的若干个词语，可广泛用于检索系统、问答系统、文档归档等场景。
 
@@ -712,15 +712,15 @@
             model = models.SimilarWordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextClassification(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         文本分类接口能够对用户输入的文本进行自动分类，将其映射到具体的类目上，用户只需要提供待分类的文本，而无需关注具体实现。
 
@@ -743,15 +743,15 @@
             model = models.TextClassificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextCorrection(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         提供对中文文本的自动纠错功能，能够识别输入文本中的错误片段，定位错误并给出正确的文本结果；支持长度不超过2000字符（含标点符号）的长文本纠错。
 
@@ -770,15 +770,15 @@
             model = models.TextCorrectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextCorrectionPro(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         提供对中文文本的自动纠错功能，能够识别输入文本中的错误片段，定位错误并给出正确的文本结果；支持长度不超过128字符（含标点符号）的长文本纠错。
 
@@ -797,15 +797,15 @@
             model = models.TextCorrectionProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextEmbellish(self, request):
         """运用先进的自然语言处理技术，对原始文本进行优化润色，提升文本的通顺性、表达力和语言质量。
 
         :param request: Request instance for TextEmbellish.
         :type request: :class:`tencentcloud.nlp.v20190408.models.TextEmbellishRequest`
@@ -820,15 +820,15 @@
             model = models.TextEmbellishResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextSimilarity(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         句子相似度接口能够基于深度学习技术来计算一个源句子和多个目标句子的相似度，相似度分值越大的两个句子在语义上越相似。目前仅支持短文本（不超过500字符）的相似度计算，长文本的相似度计算也即将推出。
 
@@ -849,15 +849,15 @@
             model = models.TextSimilarityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextSimilarityPro(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         句子相似度接口能够基于深度学习技术来计算一个源句子和多个目标句子的相似度，相似度分值越大的两个句子在语义上越相似。目前仅支持短文本（不超过128字符）的相似度计算，长文本的相似度计算也即将推出。
 
@@ -878,15 +878,15 @@
             model = models.TextSimilarityProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextWriting(self, request):
         """通过自动补全文本片段，帮助用户快速生成高质量、连贯的完整文本，提高创作效率。
 
         :param request: Request instance for TextWriting.
         :type request: :class:`tencentcloud.nlp.v20190408.models.TextWritingRequest`
@@ -901,15 +901,15 @@
             model = models.TextWritingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDict(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         修改自定义词库元数据信息，包括名称、描述。
 
@@ -926,15 +926,15 @@
             model = models.UpdateDictResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WordEmbedding(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         词向量接口能够将输入的词语映射成一个固定维度的词向量，用来表示这个词语的语义特征。词向量是很多自然语言处理技术的基础，能够显著提高它们的效果。
 
@@ -953,15 +953,15 @@
             model = models.WordEmbeddingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WordSimilarity(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         词相似度接口能够基于词向量技术来计算两个输入词语的余弦相似度，相似度数值越大的两个词语在语义上越相似。
 
@@ -978,8 +978,8 @@
             model = models.WordSimilarityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.938/tencentcloud/nlp/v20190408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.938/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.937/README.rst` & `tencentcloud-sdk-python-nlp-3.0.938/README.rst`

 * *Files identical despite different names*

