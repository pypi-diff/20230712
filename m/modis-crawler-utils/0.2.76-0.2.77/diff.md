# Comparing `tmp/modis_crawler_utils-0.2.76.tar.gz` & `tmp/modis_crawler_utils-0.2.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.2.76.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.2.77.tar", max compression
```

## Comparing `modis_crawler_utils-0.2.76.tar` & `modis_crawler_utils-0.2.77.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1784 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/README.md
--rw-r--r--   0        0        0     1050 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     6914 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0      598 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4105 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      703 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/domains.py
--rw-r--r--   0        0        0     1373 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3192 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-07-12 07:57:47.966938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2177 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1212 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     2882 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    26349 2023-07-12 14:01:57.313969 modis_crawler_utils-0.2.76/crawler_utils/files.py
--rw-r--r--   0        0        0     5002 2023-07-12 14:01:57.313969 modis_crawler_utils-0.2.76/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3083 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/logstash.py
--rw-r--r--   0        0        0     4862 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    25668 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1298 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-07-12 07:57:47.970938 modis_crawler_utils-0.2.76/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0     5751 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0      179 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-07-12 07:57:47.974938 modis_crawler_utils-0.2.76/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1480 2023-07-12 14:06:29.865457 modis_crawler_utils-0.2.76/pyproject.toml
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.76/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/README.md
+-rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.77/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.77/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     5975 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.77/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0     1263 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:58:41.564515 modis_crawler_utils-0.2.77/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3040 2023-07-12 14:56:04.814698 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1212 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    26349 2023-07-12 13:48:37.648012 modis_crawler_utils-0.2.77/crawler_utils/files.py
+-rw-r--r--   0        0        0     5002 2023-07-12 13:48:37.648012 modis_crawler_utils-0.2.77/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/logstash.py
+-rw-r--r--   0        0        0      581 2023-07-12 14:56:04.818698 modis_crawler_utils-0.2.77/crawler_utils/misc.py
+-rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:58:41.564515 modis_crawler_utils-0.2.77/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    25668 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.77/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1955 2023-07-12 14:56:04.830697 modis_crawler_utils-0.2.77/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.77/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.77/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.77/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1480 2023-07-12 14:59:40.246196 modis_crawler_utils-0.2.77/pyproject.toml
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.77/PKG-INFO
```

### Comparing `modis_crawler_utils-0.2.76/README.md` & `modis_crawler_utils-0.2.77/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/__init__.py` & `modis_crawler_utils-0.2.77/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.2.77/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.2.77/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.2.77/crawler_utils/credentials/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import random
 from typing import Callable, List, Optional, Union
 
-from scrapy.exceptions import NotConfigured
 from scrapy.settings import Settings
-from scrapy.utils.misc import create_instance, load_object
 
 from crawler_utils.credentials.credential import Credential
-from crawler_utils.credentials.store import CredentialVersionConflictError, CredentialsStore
-from crawler_utils.credentials.store.local import FileCredentialsStore, InMemoryCredentialsStore
+from crawler_utils.credentials.store import CredentialVersionConflictError, CredentialsStore, create_credentials_store
 from crawler_utils.credentials.store.talisman import TalismanCredentialsStore
 
 SelectionStrategy = Callable[[List[Credential]], Credential]
 ConflictResolutionStrategy = Callable[[Credential, Credential], bool]
 
 
 class CredentialsManager:
@@ -55,47 +52,28 @@
             self._credentials = [credential]
         else:
             self._credentials = self._store.get(self._domain)
 
     @classmethod
     def from_settings(cls, settings: Settings, store: CredentialsStore = None, **kwargs):
         if not store:
-            store = cls.load_credentials_store(settings)
+            store = create_credentials_store(settings)
         if isinstance(store, TalismanCredentialsStore):
             credential_id = store.job_env.credential_id
         else:
             credential_id = settings.get('CREDENTIAL_ID')
         return cls(**{
             'store': store,
             'credential_id': credential_id,
             'domain': settings.get('CREDENTIALS_DOMAIN'),
             'selection_strategy': settings.get('CREDENTIALS_SELECTION_STRATEGY', 'least used'),
             'conflict_resolution_strategy': settings.get('CREDENTIALS_CONFLICT_RESOLUTION_STRATEGY', 'pull'),
             **kwargs
         })
 
-    _STORE_TYPES = {
-        'talisman': TalismanCredentialsStore,
-        'memory': InMemoryCredentialsStore,
-        'file': FileCredentialsStore
-    }
-
-    @classmethod
-    def load_credentials_store(cls, settings: Settings):
-        if store_type_name := settings.get('CREDENTIALS_STORE'):
-            if not (store_type := cls._STORE_TYPES.get(store_type_name)):
-                store_type = load_object(store_type_name)
-            return create_instance(store_type, settings, None)
-        for store_type in cls._STORE_TYPES.values():
-            try:
-                return create_instance(store_type, settings=settings, crawler=None)
-            except NotConfigured:
-                pass
-        raise NotConfigured('Failed to load credentials store')
-
     def get_credential(self, **kwargs) -> Optional[Credential]:
         """
         Selects single credential.
         """
         valid_credentials = [c for c in self._credentials if c.status == 'Valid']
         if not valid_credentials:
             return None
```

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import abc
 from typing import List
 
+from scrapy.exceptions import NotConfigured
+
 from crawler_utils.credentials import Credential
+from crawler_utils.misc import create_instance_from_settings
 
 
 class CredentialsStore(metaclass=abc.ABCMeta):
 
     @abc.abstractmethod
     def get(self, domain: str) -> List[Credential]:
         pass
@@ -25,7 +28,25 @@
 
 class NoSuchCredentialError(CredentialsStoreError):
     pass
 
 
 class CredentialVersionConflictError(CredentialsStoreError):
     pass
+
+
+_BUILTIN_STORES = {
+    'talisman': f'{__name__}.talisman.TalismanCredentialsStore',
+    'memory': f'{__name__}.local.InMemoryCredentialsStore',
+    'file': f'{__name__}.local.FileCredentialsStore'
+}
+
+
+def create_credentials_store(settings):
+    if store := create_instance_from_settings(
+            crawler=None,
+            settings=settings,
+            setting_key='CREDENTIALS_STORE',
+            aliases=_BUILTIN_STORES,
+            defaults=_BUILTIN_STORES.values()):
+        return store
+    raise NotConfigured('Failed to load credentials store')
```

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.2.77/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.2.77/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.2.77/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/domains.py` & `modis_crawler_utils-0.2.77/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/echo.py` & `modis_crawler_utils-0.2.77/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from abc import ABC
 from typing import Optional
 
 from scrapy import Request
 from scrapy.crawler import Crawler
 from scrapy.exceptions import NotConfigured
-from scrapy.utils.misc import create_instance, load_object
+
+from crawler_utils.misc import create_instance_from_settings
 
 logger = logging.getLogger(__name__)
 
 
 class ElasticDupeFilterStrategy(ABC):
     dupefilter = None
 
@@ -55,29 +56,27 @@
     @classmethod
     def from_crawler(cls, crawler: Crawler):
         if cls.instance is not None:
             return cls.instance
         if cls.error:
             raise cls.error
         try:
-            cls.instance = cls._from_crawler(crawler)
+            cls.instance = create_instance_from_settings(
+                crawler=crawler,
+                settings=crawler.settings,
+                setting_key='DUPEFILTER_STRATEGY',
+                aliases=BASE_DUPEFILTER_STRATEGIES,
+                defaults=[NoOpStrategy]
+            )
             logger.info(f'Initialized dupefilter strategy {type(cls.instance).__name__}')
             return cls.instance
         except Exception as error:
             cls.error = error
             raise cls.error
 
-    @classmethod
-    def _from_crawler(cls, crawler: Crawler):
-        settings = crawler.settings
-        strategy_name = settings.get('DUPEFILTER_STRATEGY', 'noop')
-        strategy_cls_path = BASE_DUPEFILTER_STRATEGIES.get(strategy_name, strategy_name)
-        strategy_cls = load_object(strategy_cls_path)
-        return create_instance(strategy_cls, crawler=crawler, settings=settings)
-
 
 class DupeFilterStrategyMiddlewareHook:
     """
     Allows to insert dupefilter strategy in middleware lists without explicitly specifying its type.
     For example, setting
     SPIDER_MIDDLEWARES = {
       'crawler_utils.elasticsearch.dupefilter_strategies.DupeFilterStrategyMiddlewareHook': 1,
```

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/request_fingerprint.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/request_fingerprint.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.2.77/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/files.py` & `modis_crawler_utils-0.2.77/crawler_utils/files.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/images.py` & `modis_crawler_utils-0.2.77/crawler_utils/images.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/kafka.py` & `modis_crawler_utils-0.2.77/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/logstash.py` & `modis_crawler_utils-0.2.77/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/mongodb.py` & `modis_crawler_utils-0.2.77/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/proxypy.py` & `modis_crawler_utils-0.2.77/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.2.77/crawler_utils/social_media/items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/socks.py` & `modis_crawler_utils-0.2.77/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.2.77/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.2.77/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.2.77/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.2.77/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.2.77/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.2.77/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/trust_level.py` & `modis_crawler_utils-0.2.77/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/crawler_utils/validate_input.py` & `modis_crawler_utils-0.2.77/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.76/pyproject.toml` & `modis_crawler_utils-0.2.77/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.2.76"
+version = "0.2.77"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
```

### Comparing `modis_crawler_utils-0.2.76/PKG-INFO` & `modis_crawler_utils-0.2.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.2.76
+Version: 0.2.77
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

