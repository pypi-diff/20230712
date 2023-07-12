# Comparing `tmp/crossrefapi-1.5.0.tar.gz` & `tmp/crossrefapi-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crossrefapi-1.5.0.tar", last modified: Wed Jun 17 17:05:23 2020, max compression
+gzip compressed data, was "crossrefapi-1.6.0.tar", max compression
```

## Comparing `crossrefapi-1.5.0.tar` & `crossrefapi-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,7 @@
-drwxr-xr-x   0 fabiobatalha  (1000) fabiobatalha  (1000)        0 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)    27205 2019-10-18 18:57:01.000000 crossrefapi-1.5.0/README.rst
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)       39 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/MANIFEST.in
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      491 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/PKG-INFO
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      180 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/setup.cfg
-drwxr-xr-x   0 fabiobatalha  (1000) fabiobatalha  (1000)        0 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/tests/
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)        1 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/tests/__init__.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)     4267 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/tests/test_restful.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)     2348 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/tests/test_validators.py
-drwxr-xr-x   0 fabiobatalha  (1000) fabiobatalha  (1000)        0 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossref/
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)       18 2020-06-17 17:05:06.000000 crossrefapi-1.5.0/crossref/__init__.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      438 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/crossref/utils.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)     2480 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/crossref/validators.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)    66140 2020-06-17 17:04:53.000000 crossrefapi-1.5.0/crossref/restful.py
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      835 2018-02-13 17:05:30.000000 crossrefapi-1.5.0/setup.py
-drwxr-xr-x   0 fabiobatalha  (1000) fabiobatalha  (1000)        0 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)       15 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/top_level.txt
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      362 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/SOURCES.txt
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)        1 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/dependency_links.txt
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)      491 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/PKG-INFO
--rw-r--r--   0 fabiobatalha  (1000) fabiobatalha  (1000)       17 2020-06-17 17:05:23.000000 crossrefapi-1.5.0/crossrefapi.egg-info/requires.txt
+-rw-r--r--   0        0        0     1318 2023-07-12 13:13:30.714106 crossrefapi-1.6.0/LICENSE
+-rw-r--r--   0        0        0       74 2023-07-12 19:19:31.815763 crossrefapi-1.6.0/crossref/__init__.py
+-rw-r--r--   0        0        0    68063 2023-07-12 19:19:31.816263 crossrefapi-1.6.0/crossref/restful.py
+-rw-r--r--   0        0        0      421 2023-07-12 19:19:31.816669 crossrefapi-1.6.0/crossref/utils.py
+-rw-r--r--   0        0        0     2325 2023-07-12 19:19:31.816937 crossrefapi-1.6.0/crossref/validators.py
+-rw-r--r--   0        0        0      500 2023-07-12 19:30:07.367476 crossrefapi-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 crossrefapi-1.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crossrefapi-1.5.0/crossref/restful.py` & `crossrefapi-1.6.0/crossref/restful.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# coding: utf-8
+from __future__ import annotations
 
-import requests
-import json
+import contextlib
+import typing
 from time import sleep
 
-from datetime import datetime, timedelta
+import requests
 
-from crossref import validators, VERSION
+from crossref import VERSION, validators
 
 LIMIT = 100
 MAXOFFSET = 10000
 FACETS_MAX_LIMIT = 1000
 
 API = "api.crossref.org"
 
@@ -23,203 +23,216 @@
     pass
 
 
 class UrlSyntaxError(CrossrefAPIError, ValueError):
     pass
 
 
-class HTTPRequest(object):
-
-    THROTTLING_TUNNING_TIME = 600
+class HTTPRequest:
 
     def __init__(self, throttle=True):
         self.throttle = throttle
-        self.rate_limits = {
-            'X-Rate-Limit-Limit': 50,
-            'X-Rate-Limit-Interval': 1
-        }
+        self.rate_limits = {"x-rate-limit-limit": 50, "x-rate-limit-interval": 1}
 
     def _update_rate_limits(self, headers):
 
-        self.rate_limits['X-Rate-Limit-Limit'] = int(headers.get('X-Rate-Limit-Limit', 50))
+        with contextlib.suppress(ValueError):
+            self.rate_limits["x-rate-limit-limit"] = int(headers.get("x-rate-limit-limit", 50))
 
-        interval_value = int(headers.get('X-Rate-Limit-Interval', '1s')[:-1])
-        interval_scope = headers.get('X-Rate-Limit-Interval', '1s')[-1]
+        with contextlib.suppress(ValueError):
+            interval_value = int(headers.get("x-rate-limit-interval", "1s")[:-1])
 
-        if interval_scope == 'm':
+        interval_scope = headers.get("x-rate-limit-interval", "1s")[-1]
+
+        if interval_scope == "m":
             interval_value = interval_value * 60
 
-        if interval_scope == 'h':
+        if interval_scope == "h":
             interval_value = interval_value * 60 * 60
 
-        self.rate_limits['X-Rate-Limit-Interval'] = interval_value
+        self.rate_limits["x-rate-limit-interval"] = interval_value
 
     @property
     def throttling_time(self):
-        return self.rate_limits['X-Rate-Limit-Interval'] / self.rate_limits['X-Rate-Limit-Limit']
+        return self.rate_limits["x-rate-limit-interval"] / self.rate_limits["x-rate-limit-limit"]
 
-    def do_http_request(self, method, endpoint, data=None, files=None, timeout=100, only_headers=False, custom_header=None):
+    def do_http_request(  # noqa: PLR0913
+            self,
+            method,
+            endpoint,
+            data=None,
+            files=None,
+            timeout=100,
+            only_headers=False,
+            custom_header=None,
+    ):
 
         if only_headers is True:
-            return requests.head(endpoint)
+            return requests.head(endpoint, timeout=2)
 
-        if method == 'post':
-            action = requests.post
-        else:
-            action = requests.get
+        action = requests.post if method == "post" else requests.get
 
-        if custom_header:
-            headers = custom_header
-        else:
-            headers = {'user-agent': str(Etiquette())}
-        if method == 'post':
+        headers = custom_header if custom_header else {"user-agent": str(Etiquette())}
+        if method == "post":
             result = action(endpoint, data=data, files=files, timeout=timeout, headers=headers)
         else:
             result = action(endpoint, params=data, timeout=timeout, headers=headers)
 
         if self.throttle is True:
             self._update_rate_limits(result.headers)
             sleep(self.throttling_time)
 
         return result
 
 
 def build_url_endpoint(endpoint, context=None):
+    endpoint = "/".join([i for i in [context, endpoint] if i])
 
-    endpoint = '/'.join([i for i in [context, endpoint] if i])
-
-    return 'https://%s/%s' % (API, endpoint)
+    return f"https://{API}/{endpoint}"
 
 
 class Etiquette:
-
-    def __init__(self, application_name='undefined', application_version='undefined', application_url='undefined', contact_email='anonymous'):
+    def __init__(
+            self,
+            application_name="undefined",
+            application_version="undefined",
+            application_url="undefined",
+            contact_email="anonymous",
+    ):
         self.application_name = application_name
         self.application_version = application_version
         self.application_url = application_url
         self.contact_email = contact_email
 
     def __str__(self):
-
-        return '%s/%s (%s; mailto:%s) BasedOn: CrossrefAPI/%s' % (
+        return "{}/{} ({}; mailto:{}) BasedOn: CrossrefAPI/{}".format(
             self.application_name,
             self.application_version,
             self.application_url,
             self.contact_email,
-            VERSION
+            VERSION,
         )
 
 
 class Endpoint:
-
     CURSOR_AS_ITER_METHOD = False
 
-    def __init__(self, request_url=None, request_params=None, context=None, etiquette=None, throttle=True, crossref_plus_token=None):
+    def __init__( # noqa: PLR0913
+            self,
+            request_url=None,
+            request_params=None,
+            context=None,
+            etiquette=None,
+            throttle=True,
+            crossref_plus_token=None,
+            timeout=30,
+    ):
         self.do_http_request = HTTPRequest(throttle=throttle).do_http_request
         self.etiquette = etiquette or Etiquette()
-        self.custom_header = {'user-agent': str(self.etiquette)}
+        self.custom_header = {"user-agent": str(self.etiquette)}
         self.crossref_plus_token = crossref_plus_token
         if crossref_plus_token:
             self.custom_header["Crossref-Plus-API-Token"] = self.crossref_plus_token
         self.request_url = request_url or build_url_endpoint(self.ENDPOINT, context)
-        self.request_params = request_params or dict()
-        self.context = context or ''
+        self.request_params = request_params or {}
+        self.context = context or ""
+        self.timeout = timeout
 
     @property
     def _rate_limits(self):
-        request_params = dict(self.request_params)
         request_url = str(self.request_url)
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             only_headers=True,
             custom_header=self.custom_header,
-            throttle=False
+            timeout=self.timeout,
+            throttle=False,
         )
 
-        rate_limits = {
-            'X-Rate-Limit-Limit': result.headers.get('X-Rate-Limit-Limit', 'undefined'),
-            'X-Rate-Limit-Interval': result.headers.get('X-Rate-Limit-Interval', 'undefined')
+        return {
+            "x-rate-limit-limit": result.headers.get("x-rate-limit-limit", "undefined"),
+            "x-rate-limit-interval": result.headers.get("x-rate-limit-interval", "undefined"),
         }
 
-        return rate_limits
-
     def _escaped_pagging(self):
-        escape_pagging = ['offset', 'rows']
+        escape_pagging = ["offset", "rows"]
         request_params = dict(self.request_params)
 
         for item in escape_pagging:
-            try:
-                del(request_params[item])
-            except KeyError:
-                pass
+            with contextlib.suppress(KeyError):
+                del request_params[item]
 
         return request_params
 
     @property
     def version(self):
         """
-            This attribute retrieve the API version.
+        This attribute retrieve the API version.
 
-            >>> Works().version
-            '1.0.0'
+        >>> Works().version
+        '1.0.0'
         """
         request_params = dict(self.request_params)
         request_url = str(self.request_url)
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         ).json()
 
-        return result['message-version']
+        return result["message-version"]
 
     @property
     def x_rate_limit_limit(self):
 
-        return self._rate_limits.get('X-Rate-Limit-Limit', 'undefined')
+        return self._rate_limits.get("x-rate-limit-limit", "undefined")
 
     @property
     def x_rate_limit_interval(self):
 
-        return self._rate_limits.get('X-Rate-Limit-Interval', 'undefined')
+        return self._rate_limits.get("x-rate-limit-interval", "undefined")
 
     def count(self):
         """
         This method retrieve the total of records resulting from a given query.
 
         This attribute can be used compounded with query, filter,
         sort, order and facet methods.
 
         Examples:
             >>> from crossref.restful import Works
             >>> Works().query('zika').count()
             3597
             >>> Works().query('zika').filter(prefix='10.1590').count()
             61
-            >>> Works().query('zika').filter(prefix='10.1590').sort('published').order('desc').filter(has_abstract='true').count()
+            >>> Works().query('zika').filter(prefix='10.1590').sort('published') \
+                .order('desc').filter(has_abstract='true').count()
             14
-            >>> Works().query('zika').filter(prefix='10.1590').sort('published').order('desc').filter(has_abstract='true').query(author='Marli').count()
+            >>> Works().query('zika').filter(prefix='10.1590').sort('published') \
+                .order('desc').filter(has_abstract='true').query(author='Marli').count()
             1
         """
         request_params = dict(self.request_params)
         request_url = str(self.request_url)
-        request_params['rows'] = 0
+        request_params["rows"] = 0
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         ).json()
 
-        return int(result['message']['total-results'])
+        return int(result["message"]["total-results"])
 
     @property
     def url(self):
         """
         This attribute retrieve the url that will be used as a HTTP request to
         the Crossref API.
 
@@ -228,317 +241,332 @@
 
         Examples:
             >>> from crossref.restful import Works
             >>> Works().query('zika').url
             'https://api.crossref.org/works?query=zika'
             >>> Works().query('zika').filter(prefix='10.1590').url
             'https://api.crossref.org/works?query=zika&filter=prefix%3A10.1590'
-            >>> Works().query('zika').filter(prefix='10.1590').sort('published').order('desc').url
-            'https://api.crossref.org/works?sort=published&order=desc&query=zika&filter=prefix%3A10.1590'
-            >>> Works().query('zika').filter(prefix='10.1590').sort('published').order('desc').filter(has_abstract='true').query(author='Marli').url
-            'https://api.crossref.org/works?sort=published&filter=prefix%3A10.1590%2Chas-abstract%3Atrue&query=zika&order=desc&query.author=Marli'
+            >>> Works().query('zika').filter(prefix='10.1590').sort('published') \
+                .order('desc').url
+            'https://api.crossref.org/works?sort=published
+            &order=desc&query=zika&filter=prefix%3A10.1590'
+            >>> Works().query('zika').filter(prefix='10.1590').sort('published') \
+                .order('desc').filter(has_abstract='true').query(author='Marli').url
+            'https://api.crossref.org/works?sort=published
+            &filter=prefix%3A10.1590%2Chas-abstract%3Atrue&query=zika&order=desc&query.author=Marli'
         """
         request_params = self._escaped_pagging()
 
         sorted_request_params = sorted([(k, v) for k, v in request_params.items()])
-        req = requests.Request(
-            'get', self.request_url, params=sorted_request_params).prepare()
+        req = requests.Request("get", self.request_url, params=sorted_request_params).prepare()
 
         return req.url
 
-    def all(self):
+    def all(self, request_params: dict | None):  # noqa: A003
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
-        request_params = {}
 
-        return iter(self.__class__(request_url, request_params, context, etiquette=self.etiquette, crossref_plus_token=self.crossref_plus_token))
+        if request_params is None:
+            request_params = {}
 
-    def __iter__(self):
+        return iter(
+            self.__class__(
+                request_url=request_url,
+                request_params=request_params,
+                context=context,
+                etiquette=self.etiquette,
+                crossref_plus_token=self.crossref_plus_token,
+                timeout=self.timeout,
+            ),
+        )
+
+    def __iter__(self): # noqa: PLR0912 - To many branches is not a problem.
         request_url = str(self.request_url)
 
-        if 'sample' in self.request_params:
+        if "sample" in self.request_params:
             request_params = self._escaped_pagging()
             result = self.do_http_request(
-                'get',
+                "get",
                 self.request_url,
                 data=request_params,
-                custom_header=self.custom_header
+                custom_header=self.custom_header,
+                timeout=self.timeout,
             )
 
             if result.status_code == 404:
-                raise StopIteration()
+                return
 
             result = result.json()
 
-            for item in result['message']['items']:
+            for item in result["message"]["items"]:
                 yield item
 
             return
 
         if self.CURSOR_AS_ITER_METHOD is True:
             request_params = dict(self.request_params)
-            request_params['cursor'] = '*'
-            request_params['rows'] = LIMIT
+            request_params["cursor"] = "*"
+            request_params["rows"] = LIMIT
             while True:
                 result = self.do_http_request(
-                    'get',
+                    "get",
                     request_url,
                     data=request_params,
-                    custom_header=self.custom_header
+                    custom_header=self.custom_header,
+                    timeout=self.timeout,
                 )
 
                 if result.status_code == 404:
-                    raise StopIteration()
+                    return
 
                 result = result.json()
 
-                if len(result['message']['items']) == 0:
+                if len(result["message"]["items"]) == 0:
                     return
 
-                for item in result['message']['items']:
+                for item in result["message"]["items"]:
                     yield item
 
-                request_params['cursor'] = result['message']['next-cursor']
+                request_params["cursor"] = result["message"]["next-cursor"]
         else:
             request_params = dict(self.request_params)
-            request_params['offset'] = 0
-            request_params['rows'] = LIMIT
+            request_params["offset"] = 0
+            request_params["rows"] = LIMIT
             while True:
                 result = self.do_http_request(
-                    'get',
+                    "get",
                     request_url,
                     data=request_params,
-                    custom_header=self.custom_header
+                    custom_header=self.custom_header,
+                    timeout=self.timeout,
                 )
 
                 if result.status_code == 404:
-                    raise StopIteration()
+                    return
 
                 result = result.json()
 
-                if len(result['message']['items']) == 0:
+                if len(result["message"]["items"]) == 0:
                     return
 
-                for item in result['message']['items']:
+                for item in result["message"]["items"]:
                     yield item
 
-                request_params['offset'] += LIMIT + 1
+                request_params["offset"] += LIMIT
 
-                if request_params['offset'] >= MAXOFFSET:
-                    raise MaxOffsetError(
-                        'Offset exceded the max offset of %d',
-                        MAXOFFSET
-                    )
+                if request_params["offset"] >= MAXOFFSET:
+                    msg = "Offset exceded the max offset of %d"
+                    raise MaxOffsetError(msg, MAXOFFSET)
 
 
 class Works(Endpoint):
-
     CURSOR_AS_ITER_METHOD = True
 
-    ENDPOINT = 'works'
+    ENDPOINT = "works"
 
-    ORDER_VALUES = ('asc', 'desc', '1', '-1')
+    ORDER_VALUES = ("asc", "desc", "1", "-1")
 
     SORT_VALUES = (
-        'created',
-        'deposited',
-        'indexed',
-        'is-referenced-by-count',
-        'issued',
-        'published',
-        'published-online',
-        'published-print',
-        'references-count',
-        'relevance',
-        'score',
-        'submitted',
-        'updated'
+        "created",
+        "deposited",
+        "indexed",
+        "is-referenced-by-count",
+        "issued",
+        "published",
+        "published-online",
+        "published-print",
+        "references-count",
+        "relevance",
+        "score",
+        "submitted",
+        "updated",
     )
 
     FIELDS_QUERY = (
-        'affiliation',
-        'author',
-        'bibliographic',
-        'chair',
-        'container_title',
-        'contributor',
-        'editor',
-        'event_acronym',
-        'event_location',
-        'event_name',
-        'event_sponsor',
-        'event_theme',
-        'funder_name',
-        'publisher_location',
-        'publisher_name',
-        'translator'
+        "affiliation",
+        "author",
+        "bibliographic",
+        "chair",
+        "container_title",
+        "contributor",
+        "editor",
+        "event_acronym",
+        "event_location",
+        "event_name",
+        "event_sponsor",
+        "event_theme",
+        "funder_name",
+        "publisher_location",
+        "publisher_name",
+        "translator",
     )
 
     FIELDS_SELECT = (
-        'abstract',
-        'URL',
-        'member',
-        'posted',
-        'score',
-        'created',
-        'degree',
-        'update-policy',
-        'short-title',
-        'license',
-        'ISSN',
-        'container-title',
-        'issued',
-        'update-to',
-        'issue',
-        'prefix',
-        'approved',
-        'indexed',
-        'article-number',
-        'clinical-trial-number',
-        'accepted',
-        'author',
-        'group-title',
-        'DOI',
-        'is-referenced-by-count',
-        'updated-by',
-        'event',
-        'chair',
-        'standards-body',
-        'original-title',
-        'funder',
-        'translator',
-        'archive',
-        'published-print',
-        'alternative-id',
-        'subject',
-        'subtitle',
-        'published-online',
-        'publisher-location',
-        'content-domain',
-        'reference',
-        'title',
-        'link',
-        'type',
-        'publisher',
-        'volume',
-        'references-count',
-        'ISBN',
-        'issn-type',
-        'assertion',
-        'deposited',
-        'page',
-        'content-created',
-        'short-container-title',
-        'relation',
-        'editor'
+        "DOI",
+        "ISBN",
+        "ISSN",
+        "URL",
+        "abstract",
+        "accepted",
+        "alternative-id",
+        "approved",
+        "archive",
+        "article-number",
+        "assertion",
+        "author",
+        "chair",
+        "clinical-trial-number",
+        "container-title",
+        "content-created",
+        "content-domain",
+        "created",
+        "degree",
+        "deposited",
+        "editor",
+        "event",
+        "funder",
+        "group-title",
+        "indexed",
+        "is-referenced-by-count",
+        "issn-type",
+        "issue",
+        "issued",
+        "license",
+        "link",
+        "member",
+        "original-title",
+        "page",
+        "posted",
+        "prefix",
+        "published",
+        "published-online",
+        "published-print",
+        "publisher",
+        "publisher-location",
+        "reference",
+        "references-count",
+        "relation",
+        "score",
+        "short-container-title",
+        "short-title",
+        "standards-body",
+        "subject",
+        "subtitle",
+        "title",
+        "translator",
+        "type",
+        "update-policy",
+        "update-to",
+        "updated-by",
+        "volume",
     )
 
-    FILTER_VALIDATOR = {
-        'alternative_id': None,
-        'archive': validators.archive,
-        'article_number': None,
-        'assertion': None,
-        'assertion-group': None,
-        'award.funder': None,
-        'award.number': None,
-        'category-name': None,
-        'clinical-trial-number': None,
-        'container-title': None,
-        'content-domain': None,
-        'directory': validators.directory,
-        'doi': None,
-        'from-accepted-date': validators.is_date,
-        'from-created-date': validators.is_date,
-        'from-deposit-date': validators.is_date,
-        'from-event-end-date': validators.is_date,
-        'from-event-start-date': validators.is_date,
-        'from-index-date': validators.is_date,
-        'from-issued-date': validators.is_date,
-        'from-online-pub-date': validators.is_date,
-        'from-posted-date': validators.is_date,
-        'from-print-pub-date': validators.is_date,
-        'from-pub-date': validators.is_date,
-        'from-update-date': validators.is_date,
-        'full-text.application': None,
-        'full-text.type': None,
-        'full-text.version': None,
-        'funder': None,
-        'funder-doi-asserted-by': None,
-        'group-title': None,
-        'has-abstract': validators.is_bool,
-        'has-affiliation': validators.is_bool,
-        'has-archive': validators.is_bool,
-        'has-assertion': validators.is_bool,
-        'has-authenticated-orcid': validators.is_bool,
-        'has-award': validators.is_bool,
-        'has-clinical-trial-number': validators.is_bool,
-        'has-content-domain': validators.is_bool,
-        'has-domain-restriction': validators.is_bool,
-        'has-event': validators.is_bool,
-        'has-full-text': validators.is_bool,
-        'has-funder': validators.is_bool,
-        'has-funder-doi': validators.is_bool,
-        'has-license': validators.is_bool,
-        'has-orcid': validators.is_bool,
-        'has-references': validators.is_bool,
-        'has-relation': validators.is_bool,
-        'has-update': validators.is_bool,
-        'has-update-policy': validators.is_bool,
-        'is-update': validators.is_bool,
-        'isbn': None,
-        'issn': None,
-        'license.delay': validators.is_integer,
-        'license.url': None,
-        'license.version': None,
-        'location': None,
-        'member': validators.is_integer,
-        'orcid': None,
-        'prefix': None,
-        'relation.object': None,
-        'relation.object-type': None,
-        'relation.type': None,
-        'type': validators.document_type,
-        'type-name': None,
-        'until-accepted-date': validators.is_date,
-        'until-created-date': validators.is_date,
-        'until-deposit-date': validators.is_date,
-        'until-event-end-date': validators.is_date,
-        'until-event-start-date': validators.is_date,
-        'until-index-date': validators.is_date,
-        'until-issued-date': validators.is_date,
-        'until-online-pub-date': validators.is_date,
-        'until-posted-date': validators.is_date,
-        'until-print-pub-date': validators.is_date,
-        'until-pub-date': validators.is_date,
-        'until-update-date': validators.is_date,
-        'update-type': None,
-        'updates': None
-     }
-
-    FACET_VALUES = {
-        'archive': None,
-        'affiliation': None,
-        'assertion': None,
-        'assertion-group': None,
-        'category-name': None,
-        'container-title': 1000,
-        'license': None,
-        'funder-doi': None,
-        'funder-name': None,
-        'issn': 1000,
-        'orcid': 1000,
-        'published': None,
-        'publisher-name': None,
-        'relation-type': None,
-        'source': None,
-        'type-name': None,
-        'update-type': None
+    FILTER_VALIDATOR: typing.ClassVar[dict] = {
+        "alternative_id": None,
+        "archive": validators.archive,
+        "article_number": None,
+        "assertion": None,
+        "assertion-group": None,
+        "award.funder": None,
+        "award.number": None,
+        "category-name": None,
+        "clinical-trial-number": None,
+        "container-title": None,
+        "content-domain": None,
+        "directory": validators.directory,
+        "doi": None,
+        "from-accepted-date": validators.is_date,
+        "from-created-date": validators.is_date,
+        "from-deposit-date": validators.is_date,
+        "from-event-end-date": validators.is_date,
+        "from-event-start-date": validators.is_date,
+        "from-index-date": validators.is_date,
+        "from-issued-date": validators.is_date,
+        "from-online-pub-date": validators.is_date,
+        "from-posted-date": validators.is_date,
+        "from-print-pub-date": validators.is_date,
+        "from-pub-date": validators.is_date,
+        "from-update-date": validators.is_date,
+        "full-text.application": None,
+        "full-text.type": None,
+        "full-text.version": None,
+        "funder": None,
+        "funder-doi-asserted-by": None,
+        "group-title": None,
+        "has-abstract": validators.is_bool,
+        "has-affiliation": validators.is_bool,
+        "has-archive": validators.is_bool,
+        "has-assertion": validators.is_bool,
+        "has-authenticated-orcid": validators.is_bool,
+        "has-award": validators.is_bool,
+        "has-clinical-trial-number": validators.is_bool,
+        "has-content-domain": validators.is_bool,
+        "has-domain-restriction": validators.is_bool,
+        "has-event": validators.is_bool,
+        "has-full-text": validators.is_bool,
+        "has-funder": validators.is_bool,
+        "has-funder-doi": validators.is_bool,
+        "has-license": validators.is_bool,
+        "has-orcid": validators.is_bool,
+        "has-references": validators.is_bool,
+        "has-relation": validators.is_bool,
+        "has-update": validators.is_bool,
+        "has-update-policy": validators.is_bool,
+        "is-update": validators.is_bool,
+        "isbn": None,
+        "issn": None,
+        "license.delay": validators.is_integer,
+        "license.url": None,
+        "license.version": None,
+        "location": None,
+        "member": validators.is_integer,
+        "orcid": None,
+        "prefix": None,
+        "relation.object": None,
+        "relation.object-type": None,
+        "relation.type": None,
+        "type": validators.document_type,
+        "type-name": None,
+        "until-accepted-date": validators.is_date,
+        "until-created-date": validators.is_date,
+        "until-deposit-date": validators.is_date,
+        "until-event-end-date": validators.is_date,
+        "until-event-start-date": validators.is_date,
+        "until-index-date": validators.is_date,
+        "until-issued-date": validators.is_date,
+        "until-online-pub-date": validators.is_date,
+        "until-posted-date": validators.is_date,
+        "until-print-pub-date": validators.is_date,
+        "until-pub-date": validators.is_date,
+        "until-update-date": validators.is_date,
+        "update-type": None,
+        "updates": None,
+    }
+
+    FACET_VALUES: typing.ClassVar[dict] = {
+        "archive": None,
+        "affiliation": None,
+        "assertion": None,
+        "assertion-group": None,
+        "category-name": None,
+        "container-title": 1000,
+        "license": None,
+        "funder-doi": None,
+        "funder-name": None,
+        "issn": 1000,
+        "orcid": 1000,
+        "published": None,
+        "publisher-name": None,
+        "relation-type": None,
+        "source": None,
+        "type-name": None,
+        "update-type": None,
     }
 
-    def order(self, order='asc'):
+    def order(self, order="asc"):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
         This method can be used compounded with query, filter,
         sort and facet methods.
@@ -551,48 +579,53 @@
             >>> from crossref.restful import Works
             >>> works.query('zika').sort('deposited').order('asc').url
             'https://api.crossref.org/works?sort=deposited&query=zika&order=asc'
             >>> query = works.query('zika').sort('deposited').order('asc')
             >>> for item in query:
             ...    print(item['title'], item['deposited']['date-time'])
             ...
-            ['A Facile Preparation of 1-(6-Hydroxyindol-1-yl)-2,2-dimethylpropan-1-one'] 2007-02-13T20:56:13Z
-            ['Contributions to the Flora of the Lake Champlain Valley, New York and Vermont, III'] 2007-02-13T20:56:13Z
+            ['A Facile Preparation of ... an-1-one'] 2007-02-13T20:56:13Z
+            ['Contributions to the F  ... Vermont, III'] 2007-02-13T20:56:13Z
             ['Pilularia americana A. Braun in Klamath County, Oregon'] 2007-02-13T20:56:13Z
             ...
 
         Example 2:
             >>> from crossref.restful import Works
             >>> works.query('zika').sort('deposited').order('desc').url
             'https://api.crossref.org/works?sort=deposited&query=zika&order=desc'
             >>> query = works.query('zika').sort('deposited').order('desc')
             >>> for item in query:
             ...    print(item['title'], item['deposited']['date-time'])
             ...
-            ["Planning for the unexpected: Ebola virus, Zika virus, what's next?"] 2017-05-29T12:55:53Z
-            ['Sensitivity of RT-PCR method in samples shown to be positive for Zika virus by RT-qPCR in vector competence studies'] 2017-05-29T12:53:54Z
-            ['Re-evaluation of routine dengue virus serology in travelers in the era of Zika virus emergence'] 2017-05-29T10:46:11Z
+            ["Planning for the unexpected: ... , Zika virus, what's next?"] 2017-05-29T12:55:53Z
+            ['Sensitivity of RT-PCR method ... or competence studies'] 2017-05-29T12:53:54Z
+            ['Re-evaluation of routine den ... a of Zika virus emergence'] 2017-05-29T10:46:11Z
             ...
         """
 
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         if order not in self.ORDER_VALUES:
+            msg = "Sort order specified as {} but must be one of: {}".format(str(order), ", ".join(
+                self.ORDER_VALUES))
             raise UrlSyntaxError(
-                'Sort order specified as %s but must be one of: %s' % (
-                    str(order),
-                    ', '.join(self.ORDER_VALUES)
-                )
+                msg,
             )
 
-        request_params['order'] = order
+        request_params["order"] = order
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def select(self, *args):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
@@ -602,59 +635,63 @@
         args: valid FIELDS_SELECT arguments.
 
         return: iterable object of Works metadata
 
         Example 1:
             >>> from crossref.restful import Works
             >>> works = Works()
-            >>> for i in works.filter(has_funder='true', has_license='true').sample(5).select('DOI, prefix'):
+            >>> for i in works.filter(has_funder='true', has_license='true') \
+                .sample(5).select('DOI, prefix'):
             ...     print(i)
             ...
-            {'DOI': '10.1016/j.jdiacomp.2016.06.005', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.mssp.2015.07.076', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1002/slct.201700168', 'prefix': '10.1002', 'member': 'http://id.crossref.org/member/311'}
-            {'DOI': '10.1016/j.actbio.2017.01.034', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.optcom.2013.11.013', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
+            {'DOI': '10.1016/j.jdiacomp.2016.06.005', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.mssp.2015.07.076', 'prefix': '10.1016'}
+            {'DOI': '10.1002/slct.201700168', 'prefix': '10.1002'}
+            {'DOI': '10.1016/j.actbio.2017.01.034', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.optcom.2013.11.013', 'prefix': '10.1016'}
             ...
         Example 2:
             >>> from crossref.restful import Works
             >>> works = Works()
 
-            >>> for i in works.filter(has_funder='true', has_license='true').sample(5).select('DOI').select('prefix'):
+            >>> for i in works.filter(has_funder='true', has_license='true') \
+                .sample(5).select('DOI').select('prefix'):
             >>>     print(i)
             ...
-            {'DOI': '10.1016/j.sajb.2016.03.010', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.jneumeth.2009.08.017', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.tetlet.2016.05.058', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1007/s00170-017-0689-z', 'prefix': '10.1007', 'member': 'http://id.crossref.org/member/297'}
-            {'DOI': '10.1016/j.dsr.2016.03.004', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
+            {'DOI': '10.1016/j.sajb.2016.03.010', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.jneumeth.2009.08.017', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.tetlet.2016.05.058', 'prefix': '10.1016'}
+            {'DOI': '10.1007/s00170-017-0689-z', 'prefix': '10.1007'}
+            {'DOI': '10.1016/j.dsr.2016.03.004', 'prefix': '10.1016'}
             ...
         Example: 3:
             >>> from crossref.restful import Works
             >>> works = Works()
-            >>>: for i in works.filter(has_funder='true', has_license='true').sample(5).select(['DOI', 'prefix']):
+            >>>: for i in works.filter(has_funder='true', has_license='true') \
+                .sample(5).select(['DOI', 'prefix']):
             >>>      print(i)
             ...
-            {'DOI': '10.1111/zoj.12146', 'prefix': '10.1093', 'member': 'http://id.crossref.org/member/286'}
-            {'DOI': '10.1016/j.bios.2014.04.018', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.cej.2016.10.011', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.dci.2017.08.001', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.icheatmasstransfer.2016.09.012', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
+            {'DOI': '10.1111/zoj.12146', 'prefix': '10.1093'}
+            {'DOI': '10.1016/j.bios.2014.04.018', 'prefix': '10.1016}
+            {'DOI': '10.1016/j.cej.2016.10.011', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.dci.2017.08.001', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.icheatmasstransfer.2016.09.012', 'prefix': '10.1016'}
             ...
         Example: 4:
             >>> from crossref.restful import Works
             >>> works = Works()
-            >>>: for i in works.filter(has_funder='true', has_license='true').sample(5).select('DOI', 'prefix'):
+            >>>: for i in works.filter(has_funder='true', has_license='true') \
+                .sample(5).select('DOI', 'prefix'):
             >>>      print(i)
             ...
-            {'DOI': '10.1111/zoj.12146', 'prefix': '10.1093', 'member': 'http://id.crossref.org/member/286'}
-            {'DOI': '10.1016/j.bios.2014.04.018', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.cej.2016.10.011', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.dci.2017.08.001', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
-            {'DOI': '10.1016/j.icheatmasstransfer.2016.09.012', 'prefix': '10.1016', 'member': 'http://id.crossref.org/member/78'}
+            {'DOI': '10.1111/zoj.12146', 'prefix': '10.1093'}
+            {'DOI': '10.1016/j.bios.2014.04.018', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.cej.2016.10.011', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.dci.2017.08.001', 'prefix': '10.1016'}
+            {'DOI': '10.1016/j.icheatmasstransfer.2016.09.012', 'prefix': '10.1016'}
             ...
         """
 
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
@@ -662,33 +699,39 @@
 
         invalid_select_args = []
         for item in args:
             if isinstance(item, list):
                 select_args += [i.strip() for i in item]
 
             if isinstance(item, str):
-                select_args += [i.strip() for i in item.split(',')]
+                select_args += [i.strip() for i in item.split(",")]
 
         invalid_select_args = set(select_args) - set(self.FIELDS_SELECT)
 
         if len(invalid_select_args) != 0:
+            msg = "Select field's specified as ({}) but must be one of: {}".format(
+                ", ".join(invalid_select_args), ", ".join(self.FIELDS_SELECT))
             raise UrlSyntaxError(
-                'Select field\'s specified as (%s) but must be one of: %s' % (
-                    ', '.join(invalid_select_args),
-                    ', '.join(self.FIELDS_SELECT)
-                )
+                msg,
             )
 
-        request_params['select'] = ','.join(
-            sorted([i for i in set(request_params.get('select', '').split(',') + select_args) if i])
+        request_params["select"] = ",".join(
+            sorted(
+                [i for i in set(request_params.get("select", "").split(",") + select_args) if i]),
         )
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
-    def sort(self, sort='score'):
+    def sort(self, sort="score"):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
         This method can be used compounded with query, filter,
         order and facet methods.
@@ -700,121 +743,149 @@
         Example 1:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> query = works.sort('deposited')
             >>> for item in query:
             ...     print(item['title'])
             ...
-            ['Integralidade e transdisciplinaridade em equipes multiprofissionais na saúde coletiva']
+            ['Integralidade e transdisciplinaridade em ... multiprofissionais na saúde coletiva']
             ['Aprendizagem em grupo operativo de diabetes: uma abordagem etnográfica']
-            ['A rotatividade de enfermeiros e médicos: um impasse na implementação da Estratégia de Saúde da Família']
+            ['A rotatividade de enfermeiros e médicos: ... da Estratégia de Saúde da Família']
             ...
 
         Example 2:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> query = works.sort('relevance')
             >>> for item in query:
             ...     print(item['title'])
             ...
             ['Proceedings of the American Physical Society']
             ['Annual Meeting of the Research Society on Alcoholism']
-            ['Local steroid injections: Comment on the American college of rheumatology guidelines for the management of osteoarthritis of the hip and on the letter by Swezey']
+            ['Local steroid injections: ... hip and on the letter by Swezey']
             ['Intraventricular neurocytoma']
             ['Mammography accreditation']
             ['Temporal lobe necrosis in nasopharyngeal carcinoma: Pictorial essay']
             ...
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         if sort not in self.SORT_VALUES:
+            msg = "Sort field specified as {} but must be one of: {}".format(str(sort), ", ".join(
+                self.SORT_VALUES))
             raise UrlSyntaxError(
-                'Sort field specified as %s but must be one of: %s' % (
-                    str(sort),
-                    ', '.join(self.SORT_VALUES)
-                )
+                msg,
             )
 
-        request_params['sort'] = sort
+        request_params["sort"] = sort
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs):  # noqa: A003
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
         This method can be used compounded and recursively with query, filter,
         order, sort and facet methods.
 
-        kwargs: valid FILTER_VALIDATOR arguments.
+        kwargs: valid FILTER_VALIDATOR arguments. Replace `.` with `__` and
+        `-` with `_` when using parameters.
 
         return: iterable object of Works metadata
 
         Example:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> query = works.filter(has_funder='true', has_license='true')
             >>> for item in query:
             ...     print(item['title'])
             ...
             ['Design of smiling-face-shaped band-notched UWB antenna']
-            ['Phase I clinical and pharmacokinetic study of PM01183 (a tetrahydroisoquinoline, Lurbinectedin) in combination with gemcitabine in patients with advanced solid tumors']
+            ['Phase I clinical and pharmacokinetic ... tients with advanced solid tumors']
             ...
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         for fltr, value in kwargs.items():
-            decoded_fltr = fltr.replace('__', '.').replace('_', '-')
+            decoded_fltr = fltr.replace("__", ".").replace("_", "-")
             if decoded_fltr not in self.FILTER_VALIDATOR.keys():
+                msg = (
+                    f"Filter {decoded_fltr!s} specified but there is no such filter for"
+                    f" this route. Valid filters for this route"
+                    f" are: {', '.join(self.FILTER_VALIDATOR.keys())}"
+                )
                 raise UrlSyntaxError(
-                    'Filter %s specified but there is no such filter for this route. Valid filters for this route are: %s' % (
-                        str(decoded_fltr),
-                        ', '.join(self.FILTER_VALIDATOR.keys())
-                    )
+                    msg,
                 )
 
             if self.FILTER_VALIDATOR[decoded_fltr] is not None:
                 self.FILTER_VALIDATOR[decoded_fltr](str(value))
 
-            if 'filter' not in request_params:
-                request_params['filter'] = decoded_fltr + ':' + str(value)
+            if "filter" not in request_params:
+                request_params["filter"] = decoded_fltr + ":" + str(value)
             else:
-                request_params['filter'] += ',' + decoded_fltr + ':' + str(value)
+                request_params["filter"] += "," + decoded_fltr + ":" + str(value)
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def facet(self, facet_name, facet_count=100):
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
-        request_params['rows'] = 0
+        request_params["rows"] = 0
 
         if facet_name not in self.FACET_VALUES.keys():
-            raise UrlSyntaxError('Facet %s specified but there is no such facet for this route. Valid facets for this route are: *, affiliation, funder-name, funder-doi, publisher-name, orcid, container-title, assertion, archive, update-type, issn, published, source, type-name, license, category-name, relation-type, assertion-group' %
-                    str(facet_name),
-                    ', '.join(self.FACET_VALUES.keys())
-                )
+            msg = (
+                f"Facet {facet_name} specified but there is no such facet for this route."
+                f" Valid facets for this route are: *, affiliation, funder-name, funder-doi,"
+                f" publisher-name, orcid, container-title, assertion, archive, update-type,"
+                f" issn, published, source, type-name, license, category-name, relation-type,"
+                f" assertion-group"
+            )
+            raise UrlSyntaxError((
+                msg
+            ),
+                ", ".join(self.FACET_VALUES.keys()),
+            )
 
-        facet_count = self.FACET_VALUES[facet_name] if self.FACET_VALUES[facet_name] is not None and self.FACET_VALUES[facet_name] <= facet_count else facet_count
+        facet_count = (
+            self.FACET_VALUES[facet_name]
+            if self.FACET_VALUES[facet_name] is not None
+               and self.FACET_VALUES[facet_name] <= facet_count
+            else facet_count
+        )
 
-        request_params['facet'] = '%s:%s' % (facet_name, facet_count)
+        request_params["facet"] = f"{facet_name}:{facet_count}"
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         ).json()
 
-        return result['message']['facets']
+        return result["message"]["facets"]
 
     def query(self, *args, **kwargs):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
@@ -846,26 +917,33 @@
             ...
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         if args:
-            request_params['query'] = ' '.join([str(i) for i in args])
+            request_params["query"] = " ".join([str(i) for i in args])
 
         for field, value in kwargs.items():
             if field not in self.FIELDS_QUERY:
+                msg = (
+                    f"Field query {field!s} specified but there is no such field query for"
+                    " this route."
+                    f" Valid field queries for this route are: {', '.join(self.FIELDS_QUERY)}"
+                )
                 raise UrlSyntaxError(
-                    'Field query %s specified but there is no such field query for this route. Valid field queries for this route are: %s' % (
-                        str(field), ', '.join(self.FIELDS_QUERY)
-                    )
+                    msg,
                 )
-            request_params['query.%s' % field.replace('_', '-')] = value
+            request_params["query.%s" % field.replace("_", "-")] = value
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(request_url=request_url,
+                              request_params=request_params,
+                              context=context,
+                              etiquette=self.etiquette,
+                              timeout=self.timeout)
 
     def sample(self, sample_size=20):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
@@ -876,125 +954,138 @@
         Example:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> works.sample(2).url
             'https://api.crossref.org/works?sample=2'
             >>> [i['title'] for i in works.sample(2)]
             [['A study on the hemolytic properties ofPrevotella nigrescens'],
-            ['The geometry and the radial breathing mode of carbon nanotubes: beyond the ideal behaviour']]
+            ['The geometry and the radial ... of carbon nanotubes: beyond the ideal behaviour']]
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         try:
             if sample_size > 100:
-                raise UrlSyntaxError(
-                    'Integer specified as %s but must be a positive integer less than or equal to 100.' % str(sample_size)
+                msg = (
+                    f"Integer specified as {sample_size!s} but"
+                    " must be a positive integer less than or equal to 100."
                 )
-        except TypeError:
-            raise UrlSyntaxError(
-                'Integer specified as %s but must be a positive integer less than or equal to 100.' % str(sample_size)
+                raise UrlSyntaxError(msg)  # noqa: TRY301
+        except TypeError as exc:
+            msg = (
+                f"Integer specified as {sample_size!s} but"
+                " must be a positive integer less than or equal to 100."
             )
+            raise UrlSyntaxError(msg) from exc
 
-        request_params['sample'] = sample_size
+        request_params["sample"] = sample_size
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def doi(self, doi, only_message=True):
         """
         This method retrieve the DOI metadata related to a given DOI
         number.
 
         args: Crossref DOI id (String)
 
         return: JSON
 
         Example:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> works.doi('10.1590/S0004-28032013005000001')
-            {'is-referenced-by-count': 6, 'reference-count': 216, 'DOI': '10.1590/s0004-28032013005000001',
+            {'is-referenced-by-count': 6, 'reference-count': 216,
+            'DOI': '10.1590/s0004-28032013005000001',
             'subtitle': [], 'issued': {'date-parts': [[2013, 4, 19]]}, 'source': 'Crossref',
-            'short-container-title': ['Arq. Gastroenterol.'], 'references-count': 216, 'short-title': [],
+            'short-container-title': ['Arq. Gastroenterol.'], 'references-count': 216,
+            'short-title': [],
             'deposited': {'timestamp': 1495911725000, 'date-time': '2017-05-27T19:02:05Z',
             'date-parts': [[2017, 5, 27]]}, 'ISSN': ['0004-2803'], 'type': 'journal-article',
             'URL': 'http://dx.doi.org/10.1590/s0004-28032013005000001',
             'indexed': {'timestamp': 1496034748592, 'date-time': '2017-05-29T05:12:28Z',
-            'date-parts': [[2017, 5, 29]]}, 'content-domain': {'crossmark-restriction': False, 'domain': []},
+            'date-parts': [[2017, 5, 29]]}, 'content-domain': {'crossmark-restriction': False,
+            'domain': []},
             'created': {'timestamp': 1374613284000, 'date-time': '2013-07-23T21:01:24Z',
-            'date-parts': [[2013, 7, 23]]}, 'issn-type': [{'value': '0004-2803', 'type': 'electronic'}],
+            'date-parts': [[2013, 7, 23]]}, 'issn-type': [{'value': '0004-2803',
+            'type': 'electronic'}],
             'page': '81-96', 'volume': '50', 'original-title': [], 'subject': ['Gastroenterology'],
             'relation': {}, 'container-title': ['Arquivos de Gastroenterologia'], 'member': '530',
             'prefix': '10.1590', 'published-print': {'date-parts': [[2013, 4, 19]]},
             'title': ['3rd BRAZILIAN CONSENSUS ON Helicobacter pylori'],
             'publisher': 'FapUNIFESP (SciELO)', 'alternative-id': ['S0004-28032013000200081'],
             'abstract': '<jats:p>Significant abstract data.....  .</jats:p>',
             'author': [{'affiliation': [{'name': 'Universidade Federal de Minas Gerais,  BRAZIL'}],
             'family': 'Coelho', 'given': 'Luiz Gonzaga'}, {'affiliation': [
             {'name': 'Universidade Federal do Rio Grande do Sul,  Brazil'}], 'family': 'Maguinilk',
             'given': 'Ismael'}, {'affiliation': [
-            {'name': 'Presidente de Honra do Núcleo Brasileiro para Estudo do Helicobacter,  Brazil'}],
+            {'name': 'Presidente de Honra do Núcleo ... para Estudo do Helicobacter,  Brazil'}],
             'family': 'Zaterka', 'given': 'Schlioma'}, {'affiliation': [
-            {'name': 'Universidade Federal do Piauí,  Brasil'}], 'family': 'Parente', 'given': 'José Miguel'},
+            {'name': 'Universidade Federal do Piauí,  Brasil'}], 'family': 'Parente',
+             'given': 'José Miguel'},
             {'affiliation': [{'name': 'Universidade Federal de Minas Gerais,  BRAZIL'}],
             'family': 'Passos', 'given': 'Maria do Carmo Friche'}, {'affiliation': [
             {'name': 'Universidade de São Paulo,  Brasil'}], 'family': 'Moraes-Filho',
             'given': 'Joaquim Prado P.'}], 'score': 1.0, 'issue': '2'}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, doi])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, doi]))
         request_params = {}
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def agency(self, doi, only_message=True):
         """
         This method retrieve the DOI Agency metadata related to a given DOI
         number.
 
         args: Crossref DOI id (String)
 
         return: JSON
 
         Example:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> works.agency('10.1590/S0004-28032013005000001')
-            {'DOI': '10.1590/s0004-28032013005000001', 'agency': {'label': 'CrossRef', 'id': 'crossref'}}
+            {'DOI': '10.1590/s0004-2...5000001', 'agency': {'label': 'CrossRef', 'id': 'crossref'}}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, doi, 'agency'])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, doi, "agency"]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def doi_exists(self, doi):
         """
         This method retrieve a boolean according to the existence of a crossref
         DOI number. It returns False if the API results a 404 status code.
 
         args: Crossref DOI id (String)
@@ -1009,42 +1100,38 @@
 
         Example 2:
             >>> from crossref.restful import Works
             >>> works = Works()
             >>> works.doi_exists('10.1590/S0004-28032013005000001_invalid_doi')
             False
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, doi])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, doi]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
             only_headers=True,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
             return False
 
         return True
 
 
 class Funders(Endpoint):
-
     CURSOR_AS_ITER_METHOD = False
 
-    ENDPOINT = 'funders'
+    ENDPOINT = "funders"
 
-    FILTER_VALIDATOR = {
-        'location': None,
-    }
+    FILTER_VALIDATOR: typing.ClassVar[dict] = {"location": None}
 
     def query(self, *args):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
@@ -1063,19 +1150,24 @@
             'tokens': ['abbey', 'awards', 'abbey'],
             'uri': 'http://dx.doi.org/10.13039/501100000314'}
         """
         request_url = build_url_endpoint(self.ENDPOINT)
         request_params = dict(self.request_params)
 
         if args:
-            request_params['query'] = ' '.join([str(i) for i in args])
+            request_params["query"] = " ".join([str(i) for i in args])
 
-        return self.__class__(request_url, request_params, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs):  # noqa: A003
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
         This method can be used compounded and recursively with query, filter,
         order, sort and facet methods.
@@ -1097,35 +1189,42 @@
             ...
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         for fltr, value in kwargs.items():
-            decoded_fltr = fltr.replace('__', '.').replace('_', '-')
+            decoded_fltr = fltr.replace("__", ".").replace("_", "-")
             if decoded_fltr not in self.FILTER_VALIDATOR.keys():
+                msg = (
+                    f"Filter {decoded_fltr!s} specified but there is no such filter for this route."
+                    f" Valid filters for this route are: {', '.join(self.FILTER_VALIDATOR.keys())}"
+                )
                 raise UrlSyntaxError(
-                    'Filter %s specified but there is no such filter for this route. Valid filters for this route are: %s' % (
-                        str(decoded_fltr),
-                        ', '.join(self.FILTER_VALIDATOR.keys())
-                    )
+                    msg,
                 )
 
             if self.FILTER_VALIDATOR[decoded_fltr] is not None:
                 self.FILTER_VALIDATOR[decoded_fltr](str(value))
 
-            if 'filter' not in request_params:
-                request_params['filter'] = decoded_fltr + ':' + str(value)
+            if "filter" not in request_params:
+                request_params["filter"] = decoded_fltr + ":" + str(value)
             else:
-                request_params['filter'] += ',' + decoded_fltr + ':' + str(value)
+                request_params["filter"] += "," + decoded_fltr + ":" + str(value)
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def funder(self, funder_id, only_message=True):
-        """funder
+        """
         This method retrive a crossref funder metadata related to the
         given funder_id.
 
         args: Funder ID (Integer)
 
         Example:
             >>> from crossref.restful import Funders
@@ -1134,32 +1233,31 @@
             {'hierarchy': {'501100000314': {}}, 'alt-names': ['Abbey'],
             'work-count': 3, 'replaced-by': [], 'replaces': [],
             'hierarchy-names': {'501100000314': 'ABBEY AWARDS'},
             'uri': 'http://dx.doi.org/10.13039/501100000314', 'location': 'United Kingdom',
             'descendant-work-count': 3, 'descendants': [], 'name': 'ABBEY AWARDS',
             'id': '501100000314', 'tokens': ['abbey', 'awards', 'abbey']}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(funder_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(funder_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def funder_exists(self, funder_id):
         """
         This method retrieve a boolean according to the existence of a crossref
         funder. It returns False if the API results a 404 status code.
 
         args: Crossref Funder id (Integer)
@@ -1174,25 +1272,24 @@
 
         Example 2:
             >>> from crossref.restful import Funders
             >>> funders = Funders()
             >>> funders.funder_exists('999999999999')
             False
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(funder_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(funder_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
             only_headers=True,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
             return False
 
         return True
 
@@ -1200,29 +1297,28 @@
         """
         This method retrieve a iterable of Works of the given funder.
 
         args: Crossref allowed document Types (String)
 
         return: Works()
         """
-        context = '%s/%s' % (self.ENDPOINT, str(funder_id))
+        context = f"{self.ENDPOINT}/{funder_id!s}"
         return Works(context=context)
 
 
 class Members(Endpoint):
-
     CURSOR_AS_ITER_METHOD = False
 
-    ENDPOINT = 'members'
+    ENDPOINT = "members"
 
-    FILTER_VALIDATOR = {
-        'prefix': None,
-        'has-public-references': validators.is_bool,
-        'backfile-doi-count': validators.is_integer,
-        'current-doi-count': validators.is_integer
+    FILTER_VALIDATOR: typing.ClassVar[dict] = {
+        "prefix": None,
+        "has-public-references": validators.is_bool,
+        "backfile-doi-count": validators.is_integer,
+        "current-doi-count": validators.is_integer,
     }
 
     def query(self, *args):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
@@ -1234,45 +1330,58 @@
         Example:
             >>> from crossref.restful import Members
             >>> members = Members().query('Korean Association')
             members.query('Korean Association').url
             'https://api.crossref.org/journals?query=Public+Health+Health+Science'
             >>> next(iter(members.query('Korean Association')))
             {'prefix': [{'value': '10.20433', 'public-references': False,
-            'name': 'The New Korean Philosophical Association'}], 'counts': {'total-dois': 0, 'backfile-dois': 0,
+            'name': 'The New Korean Philosophical Association'}],
+            'counts': {'total-dois': 0, 'backfile-dois': 0,
             'current-dois': 0}, 'coverage': {'references-backfile': 0, 'references-current': 0,
-            'abstracts-current': 0, 'update-policies-backfile': 0, 'orcids-current': 0, 'orcids-backfile': 0,
-            'licenses-current': 0, 'affiliations-backfile': 0, 'licenses-backfile': 0, 'update-policies-current': 0,
+            'abstracts-current': 0, 'update-policies-backfile': 0, 'orcids-current': 0,
+            'orcids-backfile': 0,
+            'licenses-current': 0, 'affiliations-backfile': 0, 'licenses-backfile': 0,
+            'update-policies-current': 0,
             'resource-links-current': 0, 'resource-links-backfile': 0, 'award-numbers-backfile': 0,
-            'abstracts-backfile': 0, 'funders-current': 0, 'funders-backfile': 0, 'affiliations-current': 0,
+            'abstracts-backfile': 0, 'funders-current': 0, 'funders-backfile': 0,
+            'affiliations-current': 0,
             'award-numbers-current': 0}, 'flags': {'deposits-orcids-backfile': False,
-            'deposits-references-backfile': False, 'deposits-licenses-current': False, 'deposits': False,
-            'deposits-abstracts-current': False, 'deposits-award-numbers-current': False, 'deposits-articles': False,
+            'deposits-references-backfile': False, 'deposits-licenses-current': False,
+            'deposits': False,
+            'deposits-abstracts-current': False, 'deposits-award-numbers-current': False,
+            'deposits-articles': False,
             'deposits-resource-links-backfile': False, 'deposits-funders-current': False,
             'deposits-award-numbers-backfile': False, 'deposits-references-current': False,
             'deposits-abstracts-backfile': False, 'deposits-funders-backfile': False,
             'deposits-update-policies-current': False, 'deposits-orcids-current': False,
             'deposits-licenses-backfile': False, 'deposits-affiliations-backfile': False,
             'deposits-update-policies-backfile': False, 'deposits-resource-links-current': False,
-            'deposits-affiliations-current': False}, 'names': ['The New Korean Philosophical Association'],
-            'breakdowns': {'dois-by-issued-year': []}, 'location': 'Dongsin Tower, 4th Floor 5, Mullae-dong 6-ga,
+            'deposits-affiliations-current': False}, 'names': ['The New Korean ... Association'],
+            'breakdowns': {'dois-by-issued-year': []}, 'location': 'Dongsin Tow ... llae-dong 6-ga,
             Mullae-dong 6-ga Seoul 150-096 South Korea', 'prefixes': ['10.20433'],
-            'last-status-check-time': 1496034177684, 'id': 8334, 'tokens': ['the', 'new', 'korean', 'philosophical',
+            'last-status-check-time': 1496034177684, 'id': 8334,
+            'tokens': ['the', 'new', 'korean', 'philosophical',
             'association'], 'primary-name': 'The New Korean Philosophical Association'}
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT)
         request_params = dict(self.request_params)
 
         if args:
-            request_params['query'] = ' '.join([str(i) for i in args])
+            request_params["query"] = " ".join([str(i) for i in args])
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs):  # noqa: A003
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
         This method can be used compounded and recursively with query, filter,
         order, sort and facet methods.
@@ -1284,41 +1393,53 @@
         Example:
             >>> from crossref.restful import Members
             >>> members = Members()
             >>> query = members.filter(has_public_references='true')
             >>> for item in query:
             ...     print(item['prefix'])
             ...
-            [{u'public-references': False, u'name': u'Open Library of Humanities', u'value': u'10.16995'}, {u'public-references': True, u'name': u'Martin Eve', u'value': u'10.7766'}]
-            [{u'public-references': True, u'name': u'Institute of Business Research', u'value': u'10.24122'}]
+            [
+            {u'public-references': False, u'name': u'Open Library of Humanities',
+            u'value': u'10.16995'},
+            {u'public-references': True, u'name': u'Martin Eve', u'value': u'10.7766'}
+            ]
+            [
+            {u'public-references': True, u'name': u'Institute of Business Research',
+            u'value': u'10.24122'}
+            ]
             ...
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT, context)
         request_params = dict(self.request_params)
 
         for fltr, value in kwargs.items():
-            decoded_fltr = fltr.replace('__', '.').replace('_', '-')
+            decoded_fltr = fltr.replace("__", ".").replace("_", "-")
             if decoded_fltr not in self.FILTER_VALIDATOR.keys():
-                raise UrlSyntaxError(
-                    'Filter %s specified but there is no such filter for this route. Valid filters for this route are: %s' % (
-                        str(decoded_fltr),
-                        ', '.join(self.FILTER_VALIDATOR.keys())
-                    )
+                msg = (
+                    f"Filter {decoded_fltr!s} specified but there is no such filter for this route."
+                    f" Valid filters for this route are: {', '.join(self.FILTER_VALIDATOR.keys())}"
                 )
+                raise UrlSyntaxError(msg)
 
             if self.FILTER_VALIDATOR[decoded_fltr] is not None:
                 self.FILTER_VALIDATOR[decoded_fltr](str(value))
 
-            if 'filter' not in request_params:
-                request_params['filter'] = decoded_fltr + ':' + str(value)
+            if "filter" not in request_params:
+                request_params["filter"] = decoded_fltr + ":" + str(value)
             else:
-                request_params['filter'] += ',' + decoded_fltr + ':' + str(value)
+                request_params["filter"] += "," + decoded_fltr + ":" + str(value)
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def member(self, member_id, only_message=True):
         """
         This method retrive a crossref member metadata related to the
         given member_id.
 
         args: Member ID (Integer)
@@ -1326,59 +1447,67 @@
         Example:
             >>> from crossref.restful import Members
             >>> members = Members()
             >>> members.member(101)
             {'prefix': [{'value': '10.1024', 'public-references': False,
             'name': 'Hogrefe Publishing Group'}, {'value': '10.1027', 'public-references': False,
             'name': 'Hogrefe Publishing Group'}, {'value': '10.1026', 'public-references': False,
-            'name': 'Hogrefe Publishing Group'}], 'counts': {'total-dois': 35039, 'backfile-dois': 31430,
+            'name': 'Hogrefe Publishing Group'}], 'counts': {'total-dois': 35039,
+            'backfile-dois': 31430,
             'current-dois': 3609}, 'coverage': {'references-backfile': 0.3601972758769989,
             'references-current': 0.019118869677186012, 'abstracts-current': 0.0,
             'update-policies-backfile': 0.0, 'orcids-current': 0.0, 'orcids-backfile': 0.0,
             'licenses-current': 0.0, 'affiliations-backfile': 0.05685650557279587,
             'licenses-backfile': 0.0, 'update-policies-current': 0.0, 'resource-links-current': 0.0,
-            'resource-links-backfile': 0.0, 'award-numbers-backfile': 0.0, 'abstracts-backfile': 0.0,
-            'funders-current': 0.0, 'funders-backfile': 0.0, 'affiliations-current': 0.15710723400115967,
+            'resource-links-backfile': 0.0, 'award-numbers-backfile': 0.0,
+            'abstracts-backfile': 0.0,
+            'funders-current': 0.0, 'funders-backfile': 0.0,
+            'affiliations-current': 0.15710723400115967,
             'award-numbers-current': 0.0}, 'flags': {'deposits-orcids-backfile': False,
-            'deposits-references-backfile': True, 'deposits-licenses-current': False, 'deposits': True,
+            'deposits-references-backfile': True, 'deposits-licenses-current': False,
+            'deposits': True,
             'deposits-abstracts-current': False, 'deposits-award-numbers-current': False,
             'deposits-articles': True, 'deposits-resource-links-backfile': False,
             'deposits-funders-current': False, 'deposits-award-numbers-backfile': False,
             'deposits-references-current': True, 'deposits-abstracts-backfile': False,
             'deposits-funders-backfile': False, 'deposits-update-policies-current': False,
             'deposits-orcids-current': False, 'deposits-licenses-backfile': False,
             'deposits-affiliations-backfile': True, 'deposits-update-policies-backfile': False,
             'deposits-resource-links-current': False, 'deposits-affiliations-current': True},
             'names': ['Hogrefe Publishing Group'], 'breakdowns': {'dois-by-issued-year':
-            [[2003, 2329], [2004, 2264], [2002, 2211], [2005, 2204], [2006, 2158], [2007, 2121], [2016, 1954],
-            [2008, 1884], [2015, 1838], [2012, 1827], [2013, 1805], [2014, 1796], [2009, 1760], [2010, 1718],
-            [2011, 1681], [2001, 1479], [2000, 1477], [1999, 1267], [2017, 767], [1997, 164], [1996, 140],
+            [[2003, 2329], [2004, 2264], [2002, 2211], [2005, 2204], [2006, 2158],
+            [2007, 2121], [2016, 1954],
+            [2008, 1884], [2015, 1838], [2012, 1827], [2013, 1805], [2014, 1796],
+            [2009, 1760], [2010, 1718],
+            [2011, 1681], [2001, 1479], [2000, 1477], [1999, 1267], [2017, 767],
+            [1997, 164], [1996, 140],
             [1998, 138], [1995, 103], [1994, 11], [1993, 11], [0, 1]]},
-            'location': 'Langgass-Strasse 76 Berne CH-3000 Switzerland', 'prefixes': ['10.1024', '10.1027',
-            '10.1026'], 'last-status-check-time': 1496034132646, 'id': 101, 'tokens': ['hogrefe', 'publishing',
+            'location': 'Langgass-Strasse 76 Berne CH-3000 Switzerland', 'prefixes':
+            ['10.1024', '10.1027',
+            '10.1026'], 'last-status-check-time': 1496034132646, 'id': 101, 'tokens':
+            ['hogrefe', 'publishing',
             'group'], 'primary-name': 'Hogrefe Publishing Group'}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(member_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(member_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def member_exists(self, member_id):
         """
         This method retrieve a boolean according to the existence of a crossref
         member. It returns False if the API results a 404 status code.
 
         args: Crossref allowed document Type (String)
@@ -1393,25 +1522,24 @@
 
         Example 2:
             >>> from crossref.restful import Members
             >>> members = Members()
             >>> members.member_exists(88888)
             False
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(member_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(member_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
             only_headers=True,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
             return False
 
         return True
 
@@ -1419,55 +1547,53 @@
         """
         This method retrieve a iterable of Works of the given member.
 
         args: Member ID (Integer)
 
         return: Works()
         """
-        context = '%s/%s' % (self.ENDPOINT, str(member_id))
+        context = f"{self.ENDPOINT}/{member_id!s}"
         return Works(context=context)
 
 
 class Types(Endpoint):
-
     CURSOR_AS_ITER_METHOD = False
 
-    ENDPOINT = 'types'
+    ENDPOINT = "types"
 
-    def type(self, type_id, only_message=True):
+    def type(self, type_id, only_message=True):  # noqa: A003
         """
         This method retrive a crossref document type metadata related to the
         given type_id.
 
         args: Crossref allowed document Types (String)
 
         Example:
             >>> types.type('journal-article')
             {'label': 'Journal Article', 'id': 'journal-article'}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(type_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(type_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
-    def all(self):
+    def all(self):  # noqa: A003
         """
         This method retrieve an iterator with all the available types.
 
         return: iterator of crossref document types
 
         Example:
             >>> from crossref.restful import Types
@@ -1482,27 +1608,27 @@
             ...
             }]
         """
         request_url = build_url_endpoint(self.ENDPOINT, self.context)
         request_params = dict(self.request_params)
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            raise StopIteration()
+            return
 
         result = result.json()
 
-        for item in result['message']['items']:
-            yield item
+        yield from result["message"]["items"]
 
     def type_exists(self, type_id):
         """
         This method retrieve a boolean according to the existence of a crossref
         document type. It returns False if the API results a 404 status code.
 
         args: Crossref allowed document Type (String)
@@ -1517,25 +1643,24 @@
 
         Example 2:
             >>> from crossref.restful import Types
             >>> types = Types()
             >>> types.type_exists('unavailable type')
             False
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(type_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(type_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
             only_headers=True,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
             return False
 
         return True
 
@@ -1543,23 +1668,22 @@
         """
         This method retrieve a iterable of Works of the given type.
 
         args: Crossref allowed document Types (String)
 
         return: Works()
         """
-        context = '%s/%s' % (self.ENDPOINT, str(type_id))
+        context = f"{self.ENDPOINT}/{type_id!s}"
         return Works(context=context)
 
 
 class Prefixes(Endpoint):
-
     CURSOR_AS_ITER_METHOD = False
 
-    ENDPOINT = 'prefixes'
+    ENDPOINT = "prefixes"
 
     def prefix(self, prefix_id, only_message=True):
         """
         This method retrieve a json with the given Prefix metadata
 
         args: Crossref Prefix (String)
 
@@ -1568,50 +1692,48 @@
         Example:
             >>> from crossref.restful import Prefixes
             >>> prefixes = Prefixes()
             >>> prefixes.prefix('10.1590')
             {'name': 'FapUNIFESP (SciELO)', 'member': 'http://id.crossref.org/member/530',
             'prefix': 'http://id.crossref.org/prefix/10.1590'}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(prefix_id)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(prefix_id)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def works(self, prefix_id):
         """
         This method retrieve a iterable of Works of the given prefix.
 
         args: Crossref Prefix (String)
 
         return: Works()
         """
-        context = '%s/%s' % (self.ENDPOINT, str(prefix_id))
+        context = f"{self.ENDPOINT}/{prefix_id!s}"
         return Works(context=context)
 
 
 class Journals(Endpoint):
-
     CURSOR_AS_ITER_METHOD = False
 
-    ENDPOINT = 'journals'
+    ENDPOINT = "journals"
 
     def query(self, *args):
         """
         This method retrieve an iterable object that implements the method
         __iter__. The arguments given will compose the parameters in the
         request url.
 
@@ -1631,17 +1753,23 @@
             'title': 'International Journal of Medical Science and Public Health'}
         """
         context = str(self.context)
         request_url = build_url_endpoint(self.ENDPOINT)
         request_params = dict(self.request_params)
 
         if args:
-            request_params['query'] = ' '.join([str(i) for i in args])
+            request_params["query"] = " ".join([str(i) for i in args])
 
-        return self.__class__(request_url, request_params, context, self.etiquette)
+        return self.__class__(
+            request_url=request_url,
+            request_params=request_params,
+            context=context,
+            etiquette=self.etiquette,
+            timeout=self.timeout,
+        )
 
     def journal(self, issn, only_message=True):
         """
         This method retrieve a json with the given ISSN metadata
 
         args: Journal ISSN (String)
 
@@ -1652,32 +1780,31 @@
             >>> journals = Journals()
             >>> journals.journal('2277-338X')
             {'last-status-check-time': None, 'counts': None, 'coverage': None,
             'publisher': 'ScopeMed International Medical Journal Managment and Indexing System',
             'flags': None, 'breakdowns': None, 'ISSN': ['2320-4664', '2277-338X'],
             'title': 'International Journal of Medical Science and Public Health'}
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(issn)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(issn)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
-            return
+            return None
 
         result = result.json()
 
-        return result['message'] if only_message is True else result
+        return result["message"] if only_message is True else result
 
     def journal_exists(self, issn):
         """
         This method retrieve a boolean according to the existence of a journal
         in the Crossref database. It returns False if the API results a 404
         status code.
 
@@ -1693,25 +1820,24 @@
 
         Example 2:
             >>> from crossref.restful import Journals
             >>> journals = Journals()
             >>> journals.journal_exists('9999-AAAA')
             False
         """
-        request_url = build_url_endpoint(
-            '/'.join([self.ENDPOINT, str(issn)])
-        )
+        request_url = build_url_endpoint("/".join([self.ENDPOINT, str(issn)]))
         request_params = {}
 
         result = self.do_http_request(
-            'get',
+            "get",
             request_url,
             data=request_params,
             only_headers=True,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
         if result.status_code == 404:
             return False
 
         return True
 
@@ -1720,121 +1846,105 @@
         This method retrieve a iterable of Works of the given journal.
 
         args: Journal ISSN (String)
 
         return: Works()
         """
 
-        context = '%s/%s' % (self.ENDPOINT, str(issn))
+        context = f"{self.ENDPOINT}/{issn!s}"
         return Works(context=context)
 
 
-class Depositor(object):
-
-    def __init__(self, prefix, api_user, api_key, etiquette=None,
-                 use_test_server=False):
+class Depositor:
+    def __init__( # noqa: PLR0913
+            self, prefix, api_user, api_key, etiquette=None, use_test_server=False,
+    ):
         self.do_http_request = HTTPRequest(throttle=False).do_http_request
         self.etiquette = etiquette or Etiquette()
-        self.custom_header = {'user-agent': str(self.etiquette)}
+        self.custom_header = {"user-agent": str(self.etiquette)}
         self.prefix = prefix
         self.api_user = api_user
         self.api_key = api_key
         self.use_test_server = use_test_server
 
     def get_endpoint(self, verb):
-        subdomain = 'test' if self.use_test_server else 'doi'
-        return "https://{}.crossref.org/servlet/{}".format(subdomain, verb)
+        subdomain = "test" if self.use_test_server else "doi"
+        return f"https://{subdomain}.crossref.org/servlet/{verb}"
 
     def register_doi(self, submission_id, request_xml):
         """
         This method registry a new DOI number in Crossref or update some DOI
         metadata.
 
         submission_id: Will be used as the submission file name. The file name
         could be used in future requests to retrieve the submission status.
 
         request_xml: The XML with the document metadata. It must be under
         compliance with the Crossref Submission Schema.
         """
 
-        endpoint = self.get_endpoint('deposit')
+        endpoint = self.get_endpoint("deposit")
 
-        files = {
-            'mdFile': ('%s.xml' % submission_id, request_xml)
-        }
+        files = {"mdFile": ("%s.xml" % submission_id, request_xml)}
 
         params = {
-            'operation': 'doMDUpload',
-            'login_id': self.api_user,
-            'login_passwd': self.api_key
+            "operation": "doMDUpload",
+            "login_id": self.api_user,
+            "login_passwd": self.api_key,
         }
 
-        result = self.do_http_request(
-            'post',
+        return self.do_http_request(
+            "post",
             endpoint,
             data=params,
             files=files,
-            timeout=10,
-            custom_header=self.custom_header
+            custom_header=self.custom_header,
+            timeout=self.timeout,
         )
 
-        return result
-
-    def request_doi_status_by_filename(self, file_name, data_type='result'):
+    def request_doi_status_by_filename(self, file_name, data_type="result"):
         """
         This method retrieve the DOI requests status.
 
         file_name: Used as unique ID to identify a deposit.
 
         data_type: [contents, result]
             contents - retrieve the XML submited by the publisher
             result - retrieve a JSON with the status of the submission
         """
 
-        endpoint = self.get_endpoint('submissionDownload')
+        endpoint = self.get_endpoint("submissionDownload")
 
         params = {
-            'usr': self.api_user,
-            'pwd': self.api_key,
-            'file_name': file_name,
-            'type': data_type
+            "usr": self.api_user,
+            "pwd": self.api_key,
+            "file_name": file_name,
+            "type": data_type,
         }
 
-        result = self.do_http_request(
-            'get',
-            endpoint,
-            data=params,
-            timeout=10,
-            custom_header=self.custom_header
+        return self.do_http_request(
+            "get", endpoint, data=params, custom_header=self.custom_header, timeout=self.timeout,
         )
 
-        return result
-
-    def request_doi_status_by_batch_id(self, doi_batch_id, data_type='result'):
+    def request_doi_status_by_batch_id(self, doi_batch_id, data_type="result"):
         """
         This method retrieve the DOI requests status.
 
         file_name: Used as unique ID to identify a deposit.
 
         data_type: [contents, result]
             contents - retrieve the XML submited by the publisher
             result - retrieve a XML with the status of the submission
         """
 
-        endpoint = self.get_endpoint('submissionDownload')
+        endpoint = self.get_endpoint("submissionDownload")
 
         params = {
-            'usr': self.api_user,
-            'pwd': self.api_key,
-            'doi_batch_id': doi_batch_id,
-            'type': data_type
+            "usr": self.api_user,
+            "pwd": self.api_key,
+            "doi_batch_id": doi_batch_id,
+            "type": data_type,
         }
 
-        result = self.do_http_request(
-            'get',
-            endpoint,
-            data=params,
-            timeout=10,
-            custom_header=self.custom_header
+        return self.do_http_request(
+            "get", endpoint, data=params, custom_header=self.custom_header, timeout=self.timeout,
         )
-
-        return result
```
