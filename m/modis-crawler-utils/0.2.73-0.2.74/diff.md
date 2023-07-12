# Comparing `tmp/modis_crawler_utils-0.2.73.tar.gz` & `tmp/modis_crawler_utils-0.2.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.2.73.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.2.74.tar", max compression
```

## Comparing `modis_crawler_utils-0.2.73.tar` & `modis_crawler_utils-0.2.74.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.73/README.md
--rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.73/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.73/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.73/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.73/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     6914 2023-07-11 08:36:53.787989 modis_crawler_utils-0.2.73/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0      598 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-07-11 13:10:57.264858 modis_crawler_utils-0.2.73/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/domains.py
--rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3192 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1212 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    25796 2023-07-11 13:09:37.311760 modis_crawler_utils-0.2.73/crawler_utils/files.py
--rw-r--r--   0        0        0     4955 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.73/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/logstash.py
--rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-07-11 13:10:57.264858 modis_crawler_utils-0.2.73/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    25668 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.73/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1298 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.73/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.73/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.73/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1660 2023-07-11 13:11:56.042702 modis_crawler_utils-0.2.73/pyproject.toml
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.73/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/README.md
+-rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.74/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.74/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     6914 2023-07-11 08:36:53.787989 modis_crawler_utils-0.2.74/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0      598 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:10:01.207932 modis_crawler_utils-0.2.74/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3192 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1212 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    26315 2023-07-12 07:56:37.380101 modis_crawler_utils-0.2.74/crawler_utils/files.py
+-rw-r--r--   0        0        0     4955 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.74/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/logstash.py
+-rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:10:01.207932 modis_crawler_utils-0.2.74/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    25668 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.74/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1298 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.74/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.74/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.74/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1660 2023-07-12 08:10:56.489721 modis_crawler_utils-0.2.74/pyproject.toml
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.74/PKG-INFO
```

### Comparing `modis_crawler_utils-0.2.73/README.md` & `modis_crawler_utils-0.2.74/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/__init__.py` & `modis_crawler_utils-0.2.74/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.2.74/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.2.74/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.2.74/crawler_utils/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.2.74/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.2.74/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.2.74/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/domains.py` & `modis_crawler_utils-0.2.74/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/echo.py` & `modis_crawler_utils-0.2.74/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/request_fingerprint.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/request_fingerprint.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.2.74/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/files.py` & `modis_crawler_utils-0.2.74/crawler_utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 import binascii
 import hashlib
 import logging
 import mimetypes
 import re
 from collections.abc import Iterable
 from contextlib import suppress
+from io import BytesIO
 from os.path import basename, join, splitext
 from typing import BinaryIO, Union
 from urllib.parse import quote_plus, unquote, urlsplit
 
 from itemadapter import ItemAdapter
 from scrapy import Request
 from scrapy.crawler import Crawler
-from scrapy.pipelines.files import FSFilesStore, FilesPipeline as FilesPipelineBase
+from scrapy.pipelines.files import FSFilesStore, FilesPipeline as FilesPipelineBase, GCSFilesStore
 from scrapy.pipelines.images import ImageException, ImagesPipeline as ImagesPipelineBase
 from scrapy.settings import Settings
 from scrapy.utils.defer import deferred_to_future
 from scrapy.utils.log import failure_to_exc_info
 from scrapy.utils.misc import md5sum
+from twisted.internet.defer import maybeDeferred
 
 from crawler_utils.elasticsearch.request_fingerprint import default_request_fingerprint
 
 logger = logging.getLogger(__name__)
 
 
 class FilesPipeline(ImagesPipelineBase, FilesPipelineBase):
@@ -411,18 +413,31 @@
             if not url:
                 raise ValueError('Either url or store_path must be provided')
             if not filename:
                 filename = self._filename_from_url(url)
             attachment = {'url': url, 'filename': filename, 'attachment_type': type_tag}
             request = Request(url, meta={'attachment': attachment, 'resource_tag': resource_tag})
             store_path = self.file_path(request, info=self.spiderinfo)
+
+        if isinstance(data, bytes):
+            data = BytesIO(data)
+            close_stream = True
+        elif isinstance(self.store, (FSFilesStore, GCSFilesStore)):
+            # these stores support only BytesIO buffer
+            data.seek(0)
+            data_bytes = data.read()
+            if close_stream:
+                data.close()
+            data = BytesIO(data_bytes)
+            close_stream = True
+
         data.seek(0)
         checksum = md5sum(data)
         data.seek(0)
-        dfd = self.store.persist_file(store_path, data, info=self.spiderinfo)
+        dfd = maybeDeferred(self.store.persist_file, store_path, data, info=self.spiderinfo)
         result = {
             'url': url,
             'path': join(self._store_uri, store_path),
             'checksum': checksum,
             'filename': filename
         }
         if close_stream:
```

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/images.py` & `modis_crawler_utils-0.2.74/crawler_utils/images.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/kafka.py` & `modis_crawler_utils-0.2.74/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/logstash.py` & `modis_crawler_utils-0.2.74/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/mongodb.py` & `modis_crawler_utils-0.2.74/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/proxypy.py` & `modis_crawler_utils-0.2.74/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.2.74/crawler_utils/social_media/items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/socks.py` & `modis_crawler_utils-0.2.74/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/states/__init__.py` & `modis_crawler_utils-0.2.74/crawler_utils/states/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.2.74/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.2.74/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.2.74/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.2.74/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.2.74/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.2.74/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/trust_level.py` & `modis_crawler_utils-0.2.74/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/crawler_utils/validate_input.py` & `modis_crawler_utils-0.2.74/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.73/pyproject.toml` & `modis_crawler_utils-0.2.74/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.2.73"
+version = "0.2.74"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
```

### Comparing `modis_crawler_utils-0.2.73/PKG-INFO` & `modis_crawler_utils-0.2.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.2.73
+Version: 0.2.74
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

