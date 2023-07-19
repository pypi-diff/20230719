# Comparing `tmp/modis_crawler_utils-0.2.77.tar.gz` & `tmp/modis_crawler_utils-0.2.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.2.77.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.2.78.tar", max compression
```

## Comparing `modis_crawler_utils-0.2.77.tar` & `modis_crawler_utils-0.2.78.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/README.md
--rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.77/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     5975 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.77/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0     1263 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-07-12 14:58:41.564515 modis_crawler_utils-0.2.77/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/domains.py
--rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3040 2023-07-12 14:56:04.814698 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1212 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    26349 2023-07-12 13:48:37.648012 modis_crawler_utils-0.2.77/crawler_utils/files.py
--rw-r--r--   0        0        0     5002 2023-07-12 13:48:37.648012 modis_crawler_utils-0.2.77/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/logstash.py
--rw-r--r--   0        0        0      581 2023-07-12 14:56:04.818698 modis_crawler_utils-0.2.77/crawler_utils/misc.py
--rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-07-12 14:58:41.564515 modis_crawler_utils-0.2.77/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    25668 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1955 2023-07-12 14:56:04.830697 modis_crawler_utils-0.2.77/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.77/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.77/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1480 2023-07-12 14:59:40.246196 modis_crawler_utils-0.2.77/pyproject.toml
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.77/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/README.md
+-rw-r--r--   0        0        0     1050 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     5975 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0     1263 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4105 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      703 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1373 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3040 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2177 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1513 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     2882 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    26371 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/files.py
+-rw-r--r--   0        0        0     5002 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3083 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/logstash.py
+-rw-r--r--   0        0        0      581 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/misc.py
+-rw-r--r--   0        0        0     4862 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    25668 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1955 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0     5751 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0      179 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1480 2023-07-19 15:28:53.533192 modis_crawler_utils-0.2.78/pyproject.toml
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.78/PKG-INFO
```

### Comparing `modis_crawler_utils-0.2.77/README.md` & `modis_crawler_utils-0.2.78/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/__init__.py` & `modis_crawler_utils-0.2.78/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.2.78/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.2.78/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.2.78/crawler_utils/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.2.78/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.2.78/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/domains.py` & `modis_crawler_utils-0.2.78/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/echo.py` & `modis_crawler_utils-0.2.78/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/files.py` & `modis_crawler_utils-0.2.78/crawler_utils/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         with suppress(KeyError):
             item_adapter = ItemAdapter(item)
             if item_adapter.get(self._result_field) is None:
                 item_adapter[self._result_field] = []
             item_adapter[self._result_field].extend(r for ok, r in results if ok)
         return item
 
-    def media_downloaded(self, response, request, info, **kwargs):
+    def media_downloaded(self, response, request, info, *, item=None):
         result = super().media_downloaded(response, request, info)
         result['filename'] = self._filename(request, response)
         return result
 
     def file_downloaded(self, response, request, info, *, item=None):
         if request.meta['is_image_request']:
             try:
@@ -372,19 +372,19 @@
                 raise
             except Exception:  # TODO narrow down
                 logger.warning(f'Failed to process {request.url} as image, saving as regular file',
                                exc_info=True)
         request.meta['is_image_request'] = False
         return FilesPipelineBase.file_downloaded(self, response, request, info, item=item)
 
-    def file_path(self, request, response=None, info=None, **kwargs):
+    def file_path(self, request, response=None, info=None, *, item=None):
         path = self._file_path(request, response, info)
         return self._truncate_path(path)
 
-    def thumb_path(self, request, thumb_id, response=None, info=None):
+    def thumb_path(self, request, thumb_id, response=None, info=None, *, item=None):
         attachment = request.meta.get('attachment') or {'url': request.url}
         type_tag = attachment.get('attachment_type') or self._default_type_tag
         thumb_type_tag = f'{type_tag}-{thumb_id}' if type_tag else thumb_id
         thumb_attachment = {**attachment, 'attachment_type': thumb_type_tag}
         thumb_request = request.replace(meta={**request.meta, 'attachment': thumb_attachment})
         return self.file_path(thumb_request, response, info)
```

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/images.py` & `modis_crawler_utils-0.2.78/crawler_utils/images.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/kafka.py` & `modis_crawler_utils-0.2.78/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/logstash.py` & `modis_crawler_utils-0.2.78/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/misc.py` & `modis_crawler_utils-0.2.78/crawler_utils/misc.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/mongodb.py` & `modis_crawler_utils-0.2.78/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/proxypy.py` & `modis_crawler_utils-0.2.78/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.2.78/crawler_utils/social_media/items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/socks.py` & `modis_crawler_utils-0.2.78/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/states/__init__.py` & `modis_crawler_utils-0.2.78/crawler_utils/states/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.2.78/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.2.78/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.2.78/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.2.78/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.2.78/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.2.78/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/trust_level.py` & `modis_crawler_utils-0.2.78/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/crawler_utils/validate_input.py` & `modis_crawler_utils-0.2.78/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.77/pyproject.toml` & `modis_crawler_utils-0.2.78/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.2.77"
+version = "0.2.78"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
```

### Comparing `modis_crawler_utils-0.2.77/PKG-INFO` & `modis_crawler_utils-0.2.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.2.77
+Version: 0.2.78
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

