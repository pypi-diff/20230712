# Comparing `tmp/pygoogalytics-0.5.1.tar.gz` & `tmp/pygoogalytics-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.5.1.tar", last modified: Tue Jul  4 16:59:23 2023, max compression
+gzip compressed data, was "pygoogalytics-0.5.2.tar", last modified: Wed Jul 12 12:38:30 2023, max compression
```

## Comparing `pygoogalytics-0.5.1.tar` & `pygoogalytics-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 16:59:23.637316 pygoogalytics-0.5.1/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.5.1/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.5.1/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-04 16:59:23.637161 pygoogalytics-0.5.1/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.5.1/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 16:59:23.634596 pygoogalytics-0.5.1/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-07-04 16:59:00.000000 pygoogalytics-0.5.1/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.5.1/pygoogalytics/ads_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.5.1/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 16:59:23.636018 pygoogalytics-0.5.1/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.5.1/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.5.1/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    40473 2023-07-04 11:40:14.000000 pygoogalytics-0.5.1/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    36814 2023-07-04 15:58:43.000000 pygoogalytics-0.5.1/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.5.1/pygoogalytics/kwp_wrappers.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 16:59:23.636915 pygoogalytics-0.5.1/pygoogalytics/utils/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.5.1/pygoogalytics/utils/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2804 2023-06-21 13:16:26.000000 pygoogalytics-0.5.1/pygoogalytics/utils/ads_reports_parsing.py
--rw-r--r--   0 joshua     (501) staff       (20)     3445 2023-07-03 12:25:40.000000 pygoogalytics-0.5.1/pygoogalytics/utils/ga4_parser.py
--rw-r--r--   0 joshua     (501) staff       (20)     3137 2023-06-29 09:27:17.000000 pygoogalytics-0.5.1/pygoogalytics/utils/general_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2685 2023-06-21 13:16:26.000000 pygoogalytics-0.5.1/pygoogalytics/utils/resource_utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 16:59:23.635641 pygoogalytics-0.5.1/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-04 16:59:23.000000 pygoogalytics-0.5.1/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      670 2023-07-04 16:59:23.000000 pygoogalytics-0.5.1/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-07-04 16:59:23.000000 pygoogalytics-0.5.1/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-07-04 16:59:23.000000 pygoogalytics-0.5.1/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-07-04 16:59:23.000000 pygoogalytics-0.5.1/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-07-04 16:59:23.637355 pygoogalytics-0.5.1/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1297 2023-07-04 16:59:00.000000 pygoogalytics-0.5.1/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-12 12:38:30.005448 pygoogalytics-0.5.2/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.5.2/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.5.2/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-12 12:38:30.005325 pygoogalytics-0.5.2/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.5.2/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-12 12:38:30.003050 pygoogalytics-0.5.2/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-07-12 12:23:50.000000 pygoogalytics-0.5.2/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.5.2/pygoogalytics/ads_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.5.2/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-12 12:38:30.004348 pygoogalytics-0.5.2/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.5.2/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.5.2/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)      343 2023-07-12 12:37:58.000000 pygoogalytics-0.5.2/pygoogalytics/framing.py
+-rw-r--r--   0 joshua     (501) staff       (20)    39878 2023-07-12 12:28:48.000000 pygoogalytics-0.5.2/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    36661 2023-07-12 12:31:51.000000 pygoogalytics-0.5.2/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.5.2/pygoogalytics/kwp_wrappers.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-12 12:38:30.005098 pygoogalytics-0.5.2/pygoogalytics/utils/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.5.2/pygoogalytics/utils/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2804 2023-06-21 13:16:26.000000 pygoogalytics-0.5.2/pygoogalytics/utils/ads_reports_parsing.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3445 2023-07-03 12:25:40.000000 pygoogalytics-0.5.2/pygoogalytics/utils/ga4_parser.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3214 2023-07-12 12:31:51.000000 pygoogalytics-0.5.2/pygoogalytics/utils/general_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2685 2023-06-21 13:16:26.000000 pygoogalytics-0.5.2/pygoogalytics/utils/resource_utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-12 12:38:30.004132 pygoogalytics-0.5.2/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-12 12:38:29.000000 pygoogalytics-0.5.2/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      695 2023-07-12 12:38:29.000000 pygoogalytics-0.5.2/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-07-12 12:38:29.000000 pygoogalytics-0.5.2/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-07-12 12:38:29.000000 pygoogalytics-0.5.2/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-07-12 12:38:29.000000 pygoogalytics-0.5.2/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-07-12 12:38:30.005485 pygoogalytics-0.5.2/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1297 2023-07-12 12:23:50.000000 pygoogalytics-0.5.2/setup.py
```

### Comparing `pygoogalytics-0.5.1/LICENCE.txt` & `pygoogalytics-0.5.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/LICENSE` & `pygoogalytics-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/PKG-INFO` & `pygoogalytics-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.5.1
+Version: 0.5.2
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.5.1/README.md` & `pygoogalytics-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/__init__.py` & `pygoogalytics-0.5.2/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.5.1/pygoogalytics/ads_wrapper.py` & `pygoogalytics-0.5.2/pygoogalytics/ads_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/client.py` & `pygoogalytics-0.5.2/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.5.2/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.5.2/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.5.2/pygoogalytics/googalytics_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 
 from . import googlepandas as gpd
 from .utils import general_utils
 from .utils.ga4_parser import parse_ga4_response, parse_ga3_response, join_ga4_responses
 from . import pga_logger
 
 
+class MissingID(AttributeError):
+    """Error raised when Property ID is not specified"""
+    def __init__(self, message="Missing ID"):
+        self.message = message
+        super().__init__(self.message)
+
+
 class GoogalyticsWrapper:
     """
     The GoogalyticsWrapper requires the following arguments to access data:
     - for GSC data: sc_domain. This is the url-like string you see in the Google Search Console web application
     when selecting the site. It is either a full url (e.g. `https://www.example.com/`) or something like `sc_domain:example.com`
     - for GA3 data: the "view_id" you see in "settings" on the GA web application. This is usually an 8- or 9-digit number, passed as a string
     - for GA4 data: the ga4 property id.
@@ -250,26 +257,14 @@
                          metrics: list[str] | str | None = None,
                          ga_filters: dict | None = None,
                          raise_http_error: bool = False,
                          log_error: bool = True,
                          filter_google_organic: bool = False,
                          _print_log: bool = False) -> Optional[dict]:
 
-        if dimensions is None:
-            dimensions = ['productName']
-        elif isinstance(dimensions, str):
-            dimensions = dimensions.split('+')
-        dimensions = [re.sub(r"^ga:", "", _) for _ in dimensions]
-
-        if metrics is None:
-            metrics = ['itemRevenue']
-        elif isinstance(metrics, str):
-            metrics = [metrics]
-        metrics = [re.sub(r"^ga:", "", _) for _ in metrics]
-
         ga_dimensions = ['ga:' + _s if not re.match(r'ga:', _s) else _s for _s in dimensions]
         ga_metrics = ['ga:'+_s if not re.match(r'ga:', _s) else _s for _s in metrics]
 
         r = self._ga3_response_raw(
             start_date=start_date,
             end_date=end_date,
             ga_dimensions=ga_dimensions,
@@ -303,15 +298,23 @@
 
         # print(f"\ndimensions: {ga_dimensions} \n"
         #       f"metrics: {ga_metrics} \n "
         #       f"data: len={len(data)}, \n"
         #       f"error_type: {error_type} \n"
         #       f"column_header: {column_header} \n")
 
-        response = parse_ga3_response(column_header=column_header, response_rows=data)
+        if column_header is not None:
+            response = parse_ga3_response(column_header=column_header, response_rows=data)
+        else:
+            response = {
+                'dimension_headers': dimensions,
+                'metric_headers': metrics,
+                'row_count': 0,
+                'rows': []
+            }
 
         response['response_type'] = 'GA3'
         response['start_date'] = start_date
         response['end_date'] = end_date
 
         response['error'] = error
         response['error_type'] = error_type
@@ -326,19 +329,19 @@
                           ga_filters: dict | None = None,
                           filter_google_organic: bool = False,
                           return_raw_response: bool = False,
                           page_token: str = None,
                           _print_log: bool = False):
 
         if not self.view_id:
-            # If there is no view_id we stop here and return None,
-            # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
-            pga_logger.warning(f"{self.__class__.__name__}.get_ga3_response() :: view id is not set")
-            if not raise_http_error:
-                return None
+            _r = {
+                'error': PermissionError("view_id is not set"),
+                'error_type': 'missing_view_id'
+            }
+            return _r
 
         start_date_string = start_date.strftime("%Y-%m-%d")
         end_date_string = end_date.strftime("%Y-%m-%d")
 
         _dfc = []  # dimension filter clauses
         _mfc = []  # metric filter clauses
         _orderby = []
@@ -433,14 +436,17 @@
                          start_date: datetime.date,
                          end_date: datetime.date,
                          ga4_dimensions: list[ga_data_types.Dimension],
                          ga4_metrics: list[ga_data_types.Metric],
                          limit: int,
                          offset: int):
 
+        if not self.ga4_property_id:
+            raise MissingID("ga4_property_id is not set")
+
         request = ga_data_types.RunReportRequest(
             property=f"properties/{self.ga4_property_id}",
             dimensions=ga4_dimensions,
             metrics=ga4_metrics,
             date_ranges=[
                 ga_data_types.DateRange(
                     start_date=start_date.strftime("%Y-%m-%d"),
@@ -454,88 +460,71 @@
         ga4_response = self.ga4_resource.run_report(request)
 
         return ga4_response
 
     def get_ga4_response(self,
                          start_date: datetime.date,
                          end_date: datetime.date,
-                         ga_dimensions: list[str] | str | None = None,
-                         ga_metrics: list[str] | str | None = None,
-                         filter_google_organic: bool = False,
-                         raise_http_error: bool = False,
+                         dimensions: list[str],
+                         metrics: list[str],
                          limit: int | None = None) -> (list, dict, Any):
 
-        if not self.ga4_property_id:
-            # If there is no view_id we stop here and return None,
-            # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
-            pga_logger.warning(f"{self.__class__.__name__}.get_ga4_response() :: ga4_property_id is not set")
-            if not raise_http_error:
-                return None
-
-        if ga_dimensions is None:
-            ga_dimensions = ["dateHour", "landingPage"]
-        elif isinstance(ga_dimensions, str):
-            ga_dimensions = [_.strip() for _ in ga_dimensions.split(',')]
-
-        if ga_metrics is None:
-            ga_metrics = ["totalUsers"]
-        elif isinstance(ga_metrics, str):
-            ga_metrics = [_.strip() for _ in ga_metrics.split(',')]
-
-        dimensions = [ga_data_types.Dimension(name=_) for _ in ga_dimensions]
-        metrics = [ga_data_types.Metric(name=_) for _ in ga_metrics]
+        ga_dimensions = [ga_data_types.Dimension(name=_) for _ in dimensions]
+        ga_metrics = [ga_data_types.Metric(name=_) for _ in metrics]
 
         request_limit = 100_000
         if limit is None:
             limit = 1_000_000_000
         elif limit < 100_000:
             request_limit = limit
 
-        offset: int = 0
         complete: bool = False
         error_type: str | None = None
         responses: list[dict] = []
         error = None
-
-        tokens_per_hour_consumed: int = 0
-        tokens_per_day_consumed: int = 0
+        offset: int = 0
 
         while not complete:
             num_tries = 0
             success = False
             response = dict()
             while num_tries < 3 and not success:
                 error = None
                 try:
                     ga4_response = self._ga4_response_raw(
                         start_date=start_date,
                         end_date=end_date,
-                        ga4_dimensions=dimensions,
-                        ga4_metrics=metrics,
+                        ga4_dimensions=ga_dimensions,
+                        ga4_metrics=ga_metrics,
                         limit=request_limit,
                         offset=offset
                     )
                     response = parse_ga4_response(ga4_response)
                     success = True
                 except PermissionDenied as _permission_denied_error:
                     complete = True
                     error_type = 'permission_denied'
                     error = _permission_denied_error
-                    num_tries = 7
+                    num_tries = 1_000
                 except ResourceExhausted as _resource_exhausted_error:
                     error_type = 'quota_reached'
                     complete = True
                     error = _resource_exhausted_error
-                    num_tries = 7
+                    num_tries = 1_000
+                except MissingID as _id_error:
+                    complete = True
+                    error_type = 'missing_id'
+                    error = _id_error
+                    num_tries = 1_000
                 except InvalidArgument as _invalid_argument_error:
                     if re.search(r"metrics are incompatible", _invalid_argument_error.message):
                         error_type = 'invalid_arguments'
                     complete = True
                     error = _invalid_argument_error
-                    num_tries = 7
+                    num_tries = 1_000
                 except Exception as _e:
                     error = _e
                     num_tries += 1
 
             if success:
                 offset += response.get('row_count', 0)
                 if offset >= limit:
@@ -554,21 +543,19 @@
             response = responses[0]
             if response.get('row_count', 0) == 0:
                 error = AttributeError("Empty response")
                 error_type = "empty_response"
         else:
             response = {
                 'response_type': 'GA4',
-                'dimension_headers': ga_dimensions,
-                'metric_headers': ga_metrics,
+                'dimension_headers': dimensions,
+                'metric_headers': metrics,
                 'rows': []
             }
 
-
-
         response['start_date'] = start_date
         response['end_date'] = end_date
 
         response['error'] = error
         response['error_type'] = error_type
 
         return response
@@ -672,32 +659,30 @@
             url_list = [url_list]
 
         if re.match(r"GA4", result):
             return self._get_analytics_df(
                 response_type='GA4',
                 start_date=start_date,
                 end_date=end_date,
-                ga_dimensions=dimensions,
-                ga_metrics=metrics,
+                dimensions=dimensions,
+                metrics=metrics,
                 add_boolean_metrics=add_boolean_metrics,
                 limit=row_limit,
                 filters=filters,
                 return_response=_return_response,
-                raise_errors=raise_errors
             )
         elif re.match(r"GA3", result):
             return self._get_analytics_df(
                 response_type='GA3',
                 start_date=start_date,
                 end_date=end_date,
-                ga_dimensions=dimensions,
-                ga_metrics=metrics,
+                dimensions=dimensions,
+                metrics=metrics,
                 filters=filters,
                 add_boolean_metrics=add_boolean_metrics,
-                raise_errors=raise_errors,
                 return_response=_return_response
             )
         elif re.match(r"GSC", result) and result != "GSCQ":
             if row_limit is None:
                 row_limit = 100000
             return self._get_gsc_df(start_date=start_date,
                                     end_date=end_date,
@@ -794,60 +779,71 @@
 
         return gsc_df
 
     def _get_analytics_df(self,
                     response_type: str,
                     start_date: datetime.date | str,
                     end_date: datetime.date | str | None = None,
-                    ga_dimensions: Optional[List[str]] = None,
-                    ga_metrics: list[str] | list[list[str]] = None,
+                    dimensions: Optional[List[str]] = None,
+                    metrics: list[str] | list[list[str]] = None,
                     add_boolean_metrics: bool = True,
                     filters: Optional[dict] = None,
                     limit: int | None = 100_000_000,
                     return_response: bool = False,
-                    raise_errors: bool = True) -> gpd.GADataFrame:
+                    raise_errors: bool = False) -> gpd.GADataFrame:
+
+        if dimensions is None:
+            dimensions = ['dateHour']
+        elif isinstance(dimensions, str):
+            dimensions = dimensions.split(';')
+        dimensions = [re.sub(r"^ga:", "", _) for _ in dimensions]
+
+        if metrics is None:
+            metrics = ['itemRevenue']
 
         if not end_date:
             end_date = start_date
         if isinstance(start_date, str):
             start_date = general_utils.parse_date(start_date)
         if isinstance(end_date, str):
             end_date = general_utils.parse_date(end_date)
         if end_date < start_date:
             raise ValueError("date range incompatible: end_date < start_date")
         if start_date > datetime.date.today():
             raise ValueError("date range incompatible: start_date in the future")
 
-        if all(isinstance(_, str) for _ in ga_metrics):
-            ga_metrics = [ga_metrics]
+        if isinstance(metrics, str):
+            metrics = metrics.split(';')
+        if all(isinstance(_, str) for _ in metrics):
+            metrics = [metrics]
 
         metrics_list: list[list[str]] = []
-        for _list in ga_metrics:
+        for _list in metrics:
             metrics_list.extend([_list[10 * i:10 * i + 10] for i in range((len(_list) - 1) // 10 + 1)])
+        metrics_list = [[re.sub(r"^ga:", "", _m) for _m in _sub_list] for _sub_list in metrics_list]
 
         responses: list = []
         breaking_error: bool = False
         breaking_error_type: str | None = None
-        for _ga_metrics in metrics_list:
+        for _metrics in metrics_list:
             if response_type == 'GA3':
                 _r = self.get_ga3_response(
                     start_date=start_date,
                     end_date=end_date,
-                    dimensions=ga_dimensions,
+                    dimensions=dimensions,
+                    metrics=_metrics,
                     ga_filters=filters,
-                    metrics=_ga_metrics,
                     raise_http_error=False
                 )
             elif response_type == 'GA4':
                 _r = self.get_ga4_response(
                     start_date=start_date,
                     end_date=end_date,
-                    ga_dimensions=ga_dimensions,
-                    ga_metrics=_ga_metrics,
-                    raise_http_error=False,
+                    dimensions=dimensions,
+                    metrics=_metrics,
                     limit=limit
                 )
             else:
                 raise KeyError("response_type not recognised")
 
             responses.append(_r)
             if _r.get('error_type') is not None:
@@ -869,24 +865,24 @@
             frames = [gpd.from_response(response=_r) for _r in responses]
 
         # if len(frames)>0:
         #     return frames
 
         if len(frames) == 0:
             dataframe = gpd.GADataFrame(df_input=None,
-                                     dimensions=ga_dimensions,
-                                     metrics=general_utils.expand_list(ga_metrics),
+                                     dimensions=dimensions,
+                                     metrics=general_utils.expand_list(metrics_list),
                                      start_date=start_date,
                                      end_date=end_date,
                                      error = breaking_error_type)
 
         elif all(len(_frame) == 0 for _frame in frames):
             dataframe = gpd.GADataFrame(df_input=None,
-                                     dimensions=ga_dimensions,
-                                     metrics=general_utils.expand_list(ga_metrics),
+                                     dimensions=dimensions,
+                                     metrics=general_utils.expand_list(metrics_list),
                                      start_date=start_date,
                                      end_date=end_date,
                                         error = breaking_error_type)
         elif len(frames) == 1:
             dataframe = frames[0]
         else:
             dataframe = frames[0]
```

### Comparing `pygoogalytics-0.5.1/pygoogalytics/googlepandas.py` & `pygoogalytics-0.5.2/pygoogalytics/googlepandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from google.analytics.data_v1beta.types.analytics_data_api import RunReportResponse
 
 from typing import List, Optional, Union, Pattern
 
 from .utils import general_utils
 from .utils.ga4_parser import parse_ga4_response, parse_ga3_response
 
-gpd_logger = logging.getLogger("googlepandas")
-
 
 def camel_to_snake(string: str):
     return general_utils.RE_C2S.sub('_', string).lower()
 
 
 def from_response(response: dict | RunReportResponse,
                   response_type: str = None,
@@ -38,15 +36,14 @@
         elif response.get('reports', None):
             response = parse_ga3_response(response)
         return from_standard_analytics_response(response, start_date=start_date, end_date=end_date)
 
     elif response_type == 'GSC':
         rows = response.get('rows', [])
         response_aggregation = response.get('responseAggregationType', None)
-        gpd_logger.debug("from_response: creating GSCDataFrame")
         _gsc_df = GSCDataFrame(df_input=rows,
                                gsc_dimensions=gsc_dimensions,
                                from_gsc_response=True)
         _gsc_df.response_aggregation = response_aggregation
         return _gsc_df
 
 def from_standard_analytics_response(response: dict, start_date: datetime.date=None, end_date: datetime.date=None):
@@ -71,19 +68,17 @@
                        error=response.get('error_type'),
                        from_ga_response=from_ga_response)
 
 def from_csv(csv_file_path):
     pandas_df = pd.read_csv(csv_file_path)
     r_type = response_type_from_file(csv_file_path)
     if r_type == 'GA':
-        gpd_logger.debug("creating GADataFrame from csv")
         return GADataFrame(df_input=pandas_df,
                            from_ga_response=False)
     if r_type == 'GSC' or r_type == 'GSCQ':
-        gpd_logger.debug("creating GSCDataFrame from csv")
         return GSCDataFrame(df_input=pandas_df,
                             from_gsc_response=False)
 
 
 class GADataFrame(pd.DataFrame):
     """
     Subclass of pandas.DataFrame specifically for use with Google Analytics responses.
@@ -557,17 +552,14 @@
 
         :param df_input:
         :param gsc_dimensions:
         :param from_gsc_response: The init can either come from some date structure that ordinary pandas DataFrame
         can initialize, or a GSC response dictionary
         """
 
-        # self.logger = logging.getLogger("GADataFrame")
-        # self.logger.debug("initializing GADataFrame")
-
         if gsc_dimensions is None:
             gsc_dimensions = ['country', 'device', 'page', 'query']
 
         self.dimensions = gsc_dimensions
 
         if df_input is None:
             self.metrics = ['clicks', 'impressions', 'ctr', 'position']
@@ -717,14 +709,19 @@
         binned_df = _df.groupby('position').sum()[['clicks', 'impressions']]
         binned_df.insert(loc=0, column='queries', value=_df.groupby('position').size())
         if reset_index:
             return binned_df.reset_index()
         else:
             return binned_df
 
+    def add_row_id(self):
+        self.reset_index(drop=True, inplace=True)
+        self.reset_index(drop=False, inplace=True)
+        self.rename(columns={'index': 'row_id'}, inplace=True)
+
 
 def is_question(query: str) -> bool:
     if general_utils.RE_QUESTION.match(query):
         return True
     else:
         return False
```

### Comparing `pygoogalytics-0.5.1/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.5.2/pygoogalytics/kwp_wrappers.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/utils/ads_reports_parsing.py` & `pygoogalytics-0.5.2/pygoogalytics/utils/ads_reports_parsing.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/utils/ga4_parser.py` & `pygoogalytics-0.5.2/pygoogalytics/utils/ga4_parser.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics/utils/general_utils.py` & `pygoogalytics-0.5.2/pygoogalytics/utils/general_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 RE_TRANSACTIONAL = re.compile(TRANSACTION)
 RE_INVESTIGATION = re.compile(INVESTIGATION)
 RE_URL = re.compile(URL)
 RE_URL_PATH_CAPTURE = re.compile(URL_PATH_CAPTURE)
 RE_C2S = re.compile(r"(?<!^)(?=[A-Z])")
 
 
+def camel_to_snake(string: str):
+    return RE_C2S.sub('_', string).lower()
+
 def strip_url(url: str) -> str:
     url = url.split('?')[0]
     if _match := RE_URL_PATH_CAPTURE.match(url):
         return _match.group(1)
     else:
         return url
```

### Comparing `pygoogalytics-0.5.1/pygoogalytics/utils/resource_utils.py` & `pygoogalytics-0.5.2/pygoogalytics/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.5.1/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.5.2/pygoogalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.5.1
+Version: 0.5.2
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.5.1/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.5.2/pygoogalytics.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENCE.txt
 LICENSE
 README.md
 setup.py
 pygoogalytics/__init__.py
 pygoogalytics/ads_wrapper.py
 pygoogalytics/client.py
+pygoogalytics/framing.py
 pygoogalytics/googalytics_wrapper.py
 pygoogalytics/googlepandas.py
 pygoogalytics/kwp_wrappers.py
 pygoogalytics.egg-info/PKG-INFO
 pygoogalytics.egg-info/SOURCES.txt
 pygoogalytics.egg-info/dependency_links.txt
 pygoogalytics.egg-info/requires.txt
```

### Comparing `pygoogalytics-0.5.1/setup.py` & `pygoogalytics-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.5.1',
+    version='0.5.2',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

