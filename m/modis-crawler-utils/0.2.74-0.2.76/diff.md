# Comparing `tmp/modis_crawler_utils-0.2.74.tar.gz` & `tmp/modis_crawler_utils-0.2.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.2.74.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.2.76.tar", max compression
```

## Comparing `modis_crawler_utils-0.2.74.tar` & `modis_crawler_utils-0.2.76.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/README.md
--rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.74/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     6914 2023-07-11 08:36:53.787989 modis_crawler_utils-0.2.74/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0      598 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-07-12 08:10:01.207932 modis_crawler_utils-0.2.74/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/domains.py
--rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3192 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1212 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    26315 2023-07-12 07:56:37.380101 modis_crawler_utils-0.2.74/crawler_utils/files.py
--rw-r--r--   0        0        0     4955 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.74/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/logstash.py
--rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-07-12 08:10:01.207932 modis_crawler_utils-0.2.74/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    25668 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1298 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.74/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.74/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1660 2023-07-12 08:10:56.489721 modis_crawler_utils-0.2.74/pyproject.toml
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.74/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/README.md
+-rw-r--r--   0        0        0     1050 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     6914 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0      598 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4105 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      703 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1373 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3192 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2177 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1212 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     2882 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    26349 2023-07-12 14:01:57.313969 modis_crawler_utils-0.2.76/crawler_utils/files.py
+-rw-r--r--   0        0        0     5002 2023-07-12 14:01:57.313969 modis_crawler_utils-0.2.76/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3083 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/logstash.py
+-rw-r--r--   0        0        0     4862 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    25668 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1298 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0     5751 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0      179 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1480 2023-07-12 14:06:29.865457 modis_crawler_utils-0.2.76/pyproject.toml
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.76/PKG-INFO
```

### Comparing `modis_crawler_utils-0.2.74/README.md` & `modis_crawler_utils-0.2.76/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/__init__.py` & `modis_crawler_utils-0.2.76/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.2.76/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.2.76/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.2.76/crawler_utils/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.2.76/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.2.76/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/domains.py` & `modis_crawler_utils-0.2.76/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/echo.py` & `modis_crawler_utils-0.2.76/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/request_fingerprint.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/request_fingerprint.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/files.py` & `modis_crawler_utils-0.2.76/crawler_utils/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     DEFAULT_TYPE_TAG = 'data'
 
     PROCESS_IMAGES = False
     IMAGE_ATTACHMENT_TYPES = ('image',)
     IMAGE_SAVE_EXTENSION = '.jpg'
 
     KEY_PREFIX = 'FILES'
+    CRAWLER_ATTRIBUTE_NAME = 'files_pipeline'
 
     def __init__(self, store_uri, download_func=None, settings=None):
         if not store_uri.endswith('/'):
             # Ensure trailing slash for consistency between different stores: in S3/GCS stores
             # prefix and generated path are concatenated, in other stores - joined with slash
             store_uri += '/'
 
@@ -208,19 +209,18 @@
     def from_settings(cls, settings):
         return super(ImagesPipelineBase, cls).from_settings(settings)
 
     @classmethod
     def from_crawler(cls, crawler: 'Crawler'):
         # Bind pipeline to crawler object to reuse download caches in spiders
         # TODO maybe it is better to create a singleton metaclass instead?
-        if pipeline := getattr(crawler, '_files_pipeline', None):
+        if pipeline := getattr(crawler, cls.CRAWLER_ATTRIBUTE_NAME, None):
             return pipeline
-        pipeline = cls.from_settings(crawler.settings)
-        pipeline.crawler = crawler
-        crawler._files_pipeline = pipeline
+        pipeline = super().from_crawler(crawler)
+        setattr(crawler, cls.CRAWLER_ATTRIBUTE_NAME, pipeline)
         return pipeline
 
     def _resolve_key(self, key, settings):
         return self._key_for_pipe(f'{self.KEY_PREFIX}_{key}',
                                   base_class_name='FilesPipeline',
                                   settings=settings)
```

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/images.py` & `modis_crawler_utils-0.2.76/crawler_utils/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     DENY_ATTACHMENT_TYPES = ()
 
     DEFAULT_IMAGES_RESULT_FIELD = '_attachments'
 
     DEFAULT_TYPE_TAG = 'image'
 
     KEY_PREFIX = 'IMAGES'
+    CRAWLER_ATTRIBUTE_NAME = 'images_pipeline'
 
     @classmethod
     def from_settings(cls, settings):
         logger.warning(
             f'{ImagesPipeline.__module__}.{ImagesPipeline.__name__} is deprecated and might be removed in future. '
             f'Consider using {FilesPipeline.__module__}.{FilesPipeline.__name__} instead.')
         return super(FilesPipeline, cls).from_settings(settings)
```

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/kafka.py` & `modis_crawler_utils-0.2.76/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/logstash.py` & `modis_crawler_utils-0.2.76/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/mongodb.py` & `modis_crawler_utils-0.2.76/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/proxypy.py` & `modis_crawler_utils-0.2.76/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.2.76/crawler_utils/social_media/items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/socks.py` & `modis_crawler_utils-0.2.76/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/states/__init__.py` & `modis_crawler_utils-0.2.76/crawler_utils/states/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.2.76/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.2.76/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.2.76/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.2.76/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.2.76/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.2.76/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/trust_level.py` & `modis_crawler_utils-0.2.76/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/crawler_utils/validate_input.py` & `modis_crawler_utils-0.2.76/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.74/pyproject.toml` & `modis_crawler_utils-0.2.76/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.2.74"
+version = "0.2.76"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
 homepage = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
 packages = [{ include = "crawler_utils" }]
 license = "BSD"
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Framework :: Scrapy',
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: BSD License'
 ]
 
 [tool.poetry.scripts]
 build-egg = "crawler_utils.deploy.create_egg:main"
 build-md = "crawler_utils.deploy.make_arguments_md_file:main"
 bump-version = "crawler_utils.deploy.bump_version:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-scrapy = ">=2.1.0"
+scrapy = ">=2.6.0"
 pymongo = ">=3.10.1"
 Pillow = ">=7.1.2"
 kafka-python = ">=2.0.1"
 requests = ">=2.23.0"
 itemadapter = ">=0.2.0"
 python-logstash = ">=0.4.6"
 elasticsearch = "7.8.1"
```

### Comparing `modis_crawler_utils-0.2.74/PKG-INFO` & `modis_crawler_utils-0.2.76/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.2.74
+Version: 0.2.76
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,31 +13,27 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: Pillow (>=7.1.2)
 Requires-Dist: certifi
 Requires-Dist: cryptography (==36.0.2)
 Requires-Dist: dateparser (>=1.0.0)
 Requires-Dist: elasticsearch (==7.8.1)
 Requires-Dist: ephemeral-port-reserve (>=1.1.1)
 Requires-Dist: itemadapter (>=0.2.0)
 Requires-Dist: kafka-python (>=2.0.1)
 Requires-Dist: pymongo (>=3.10.1)
 Requires-Dist: pyopenssl (==22.0.0)
 Requires-Dist: python-logstash (>=0.4.6)
 Requires-Dist: requests (>=2.23.0)
-Requires-Dist: scrapy (>=2.1.0)
+Requires-Dist: scrapy (>=2.6.0)
 Requires-Dist: scrapy-puppeteer-client (>=0.0.6)
 Requires-Dist: scrapy-splash (>=0.8.0)
 Requires-Dist: twisted
 Project-URL: Repository, https://gitlab.at.ispras.ru/crawlers/crawler-utils
 Description-Content-Type: text/markdown
 
 # crawler-utils
```

