# Comparing `tmp/pymeteosource-1.5.0.tar.gz` & `tmp/pymeteosource-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteosource-1.5.0.tar", last modified: Tue Feb 14 10:44:23 2023, max compression
+gzip compressed data, was "pymeteosource-1.6.0.tar", last modified: Wed Jul 12 10:58:38 2023, max compression
```

## Comparing `pymeteosource-1.5.0.tar` & `pymeteosource-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       54 2021-09-07 15:41:14.000000 pymeteosource-1.5.0/.gitignore
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     1064 2021-09-15 15:33:11.000000 pymeteosource-1.5.0/LICENSE.txt
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    13196 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/PKG-INFO
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    12649 2023-02-14 10:37:59.000000 pymeteosource-1.5.0/README.md
-drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/pymeteosource/
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-06 15:51:26.000000 pymeteosource-1.5.0/pymeteosource/__init__.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     9359 2023-02-14 09:57:09.000000 pymeteosource-1.5.0/pymeteosource/api.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    20882 2023-02-14 10:37:10.000000 pymeteosource-1.5.0/pymeteosource/data.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     5191 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/pymeteosource/errors.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     1481 2022-09-27 07:38:47.000000 pymeteosource-1.5.0/pymeteosource/request_handler.py
-drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/pymeteosource/types/
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-07 06:44:47.000000 pymeteosource-1.5.0/pymeteosource/types/__init__.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       85 2021-12-29 17:50:33.000000 pymeteosource-1.5.0/pymeteosource/types/endpoints.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     2600 2022-10-27 11:54:12.000000 pymeteosource-1.5.0/pymeteosource/types/icons.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      124 2021-09-07 14:31:36.000000 pymeteosource-1.5.0/pymeteosource/types/langs.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      172 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/pymeteosource/types/sections.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      107 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/pymeteosource/types/tiers.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       83 2021-09-15 15:33:02.000000 pymeteosource-1.5.0/pymeteosource/types/time_formats.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       97 2021-09-07 14:31:25.000000 pymeteosource-1.5.0/pymeteosource/types/units.py
-drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/pymeteosource.egg-info/
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    13196 2023-02-14 10:44:22.000000 pymeteosource-1.5.0/pymeteosource.egg-info/PKG-INFO
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      717 2023-02-14 10:44:23.000000 pymeteosource-1.5.0/pymeteosource.egg-info/SOURCES.txt
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        1 2023-02-14 10:44:22.000000 pymeteosource-1.5.0/pymeteosource.egg-info/dependency_links.txt
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       37 2023-02-14 10:44:22.000000 pymeteosource-1.5.0/pymeteosource.egg-info/requires.txt
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       20 2023-02-14 10:44:22.000000 pymeteosource-1.5.0/pymeteosource.egg-info/top_level.txt
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       79 2023-02-14 10:44:23.144759 pymeteosource-1.5.0/setup.cfg
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      818 2023-02-14 10:08:58.000000 pymeteosource-1.5.0/setup.py
-drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-02-14 10:44:23.140759 pymeteosource-1.5.0/tests/
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-15 15:33:03.000000 pymeteosource-1.5.0/tests/__init__.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    14623 2021-09-15 15:33:07.000000 pymeteosource-1.5.0/tests/dst_changes_data.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)   403253 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/tests/sample_data.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    15786 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/tests/test_api.py
--rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     2455 2022-03-18 10:09:35.000000 pymeteosource-1.5.0/tests/variables_list.py
+drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       54 2021-09-07 15:41:14.000000 pymeteosource-1.6.0/.gitignore
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     1064 2021-09-15 15:33:11.000000 pymeteosource-1.6.0/LICENSE.txt
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    13369 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/PKG-INFO
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    12822 2023-07-12 10:54:33.000000 pymeteosource-1.6.0/README.md
+drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/pymeteosource/
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-06 15:51:26.000000 pymeteosource-1.6.0/pymeteosource/__init__.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     9359 2023-02-14 09:57:09.000000 pymeteosource-1.6.0/pymeteosource/api.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    21319 2023-07-12 10:51:49.000000 pymeteosource-1.6.0/pymeteosource/data.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     5191 2022-03-18 10:09:35.000000 pymeteosource-1.6.0/pymeteosource/errors.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     1481 2022-09-27 07:38:47.000000 pymeteosource-1.6.0/pymeteosource/request_handler.py
+drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/pymeteosource/types/
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-07 06:44:47.000000 pymeteosource-1.6.0/pymeteosource/types/__init__.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       85 2021-12-29 17:50:33.000000 pymeteosource-1.6.0/pymeteosource/types/endpoints.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     2600 2022-10-27 11:54:12.000000 pymeteosource-1.6.0/pymeteosource/types/icons.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      124 2021-09-07 14:31:36.000000 pymeteosource-1.6.0/pymeteosource/types/langs.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      172 2022-03-18 10:09:35.000000 pymeteosource-1.6.0/pymeteosource/types/sections.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      107 2022-03-18 10:09:35.000000 pymeteosource-1.6.0/pymeteosource/types/tiers.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       83 2021-09-15 15:33:02.000000 pymeteosource-1.6.0/pymeteosource/types/time_formats.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       97 2021-09-07 14:31:25.000000 pymeteosource-1.6.0/pymeteosource/types/units.py
+drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/pymeteosource.egg-info/
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    13369 2023-07-12 10:58:37.000000 pymeteosource-1.6.0/pymeteosource.egg-info/PKG-INFO
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      717 2023-07-12 10:58:38.000000 pymeteosource-1.6.0/pymeteosource.egg-info/SOURCES.txt
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        1 2023-07-12 10:58:37.000000 pymeteosource-1.6.0/pymeteosource.egg-info/dependency_links.txt
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       37 2023-07-12 10:58:37.000000 pymeteosource-1.6.0/pymeteosource.egg-info/requires.txt
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       20 2023-07-12 10:58:37.000000 pymeteosource-1.6.0/pymeteosource.egg-info/top_level.txt
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)       79 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/setup.cfg
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)      818 2023-07-12 10:55:56.000000 pymeteosource-1.6.0/setup.py
+drwxrwxr-x   0 dejdy     (1000) dejdy     (1000)        0 2023-07-12 10:58:38.137939 pymeteosource-1.6.0/tests/
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)        0 2021-09-15 15:33:03.000000 pymeteosource-1.6.0/tests/__init__.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    14623 2021-09-15 15:33:07.000000 pymeteosource-1.6.0/tests/dst_changes_data.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)   403663 2023-02-14 10:55:28.000000 pymeteosource-1.6.0/tests/sample_data.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)    15786 2022-03-18 10:09:35.000000 pymeteosource-1.6.0/tests/test_api.py
+-rw-rw-r--   0 dejdy     (1000) dejdy     (1000)     2455 2022-03-18 10:09:35.000000 pymeteosource-1.6.0/tests/variables_list.py
```

### Comparing `pymeteosource-1.5.0/LICENSE.txt` & `pymeteosource-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/PKG-INFO` & `pymeteosource-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pymeteosource
-Version: 1.5.0
+Version: 1.6.0
 Summary: Meteosource API wrapper library
-Home-page: https://github.com/Meteosource/pymeteosource/archive/v1.5.0.tar.gz
+Home-page: https://github.com/Meteosource/pymeteosource/archive/v1.6.0.tar.gz
 Author: Meteosource
 Author-email: support@meteosource.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -100,15 +100,15 @@
     tz='US/Pacific',  # Defaults to 'UTC', regardless of the point location
     lang=langs.ENGLISH,  # Defaults to 'en'
     units=units.US  # Defaults to 'auto'
 )
 ```
 
 ### Historical weather
-Users with paid subscription to Meteosource can retrieve historical weather and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
+Users with paid subscription to Meteosource can retrieve historical weather, daily summaries and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
 
 ```python
 # Get the historical weather
 time_machine = meteosource.get_time_machine(
     date='2019-12-25',  # You can also pass list/tuple/set of dates, which can be 'str' or 'datetime' objects
     date_from=None,  # You can specify the range for dates you need, instead of list
     date_to=None,  # You can specify the range for dates you need, instead of list
@@ -187,18 +187,19 @@
 forecast.alerts.get_active_alerts() # returns list of SingleTimeData instances
 # You can use either string...
 forecast.alerts.get_active_alerts('2022-03-08T22:00:00')
 # ... or datetime (both tz-aware and naive)
 forecast.alerts.get_active_alerts(datetime(2022, 3, 8, 23, 0, 0))
 ```
 
-There are sections `data` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
+There are sections `data`, `daily` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
 ```python
 print(time_machine.data)  # <Instance of MultipleTimesData (time_machine) with 24 timesteps from 2019-12-25T00:00:00 to 2019-12-25T23:00:00>
 print(time_machine.statistics)  # <Instance of MultipleTimesData (statistics) with 1 timesteps from 2019-12-25 to 2019-12-25>
+print(time_machine.daily)  # <Instance of MultipleTimesData (daily) with 1 timesteps from 2019-12-25 to 2019-12-25>
 ```
 
 ### Time indexing
 
 As mentioned above, the `minutely`, `hourly`, `daily` sections of `Forecast` and the `data` section of `TimeMachine` contain data for more timesteps. To get the data for a single time, you have several options.
 
   **1. Indexing with integer**
@@ -277,14 +278,15 @@
 df = forecast.hourly.to_pandas()
 print(df)
 ```
 
 For historical weather data, you can also call the method on the `TimeMachine` object directly, so all following calls are valid:
 ```python
 time_machine.data.to_pandas()
+time_machine.daily.to_pandas()
 time_machine.statistics.to_pandas()
 time_machine.to_pandas()
 ```
 
 You can also merge the daily statistics and the hourly historical data into single `pandas` `DataFrame`. In this case, the daily statistics are duplicated into all hours of each day:
 ```python
 time_machine.to_pandas(include_statistics=True)
```

### Comparing `pymeteosource-1.5.0/README.md` & `pymeteosource-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     tz='US/Pacific',  # Defaults to 'UTC', regardless of the point location
     lang=langs.ENGLISH,  # Defaults to 'en'
     units=units.US  # Defaults to 'auto'
 )
 ```
 
 ### Historical weather
-Users with paid subscription to Meteosource can retrieve historical weather and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
+Users with paid subscription to Meteosource can retrieve historical weather, daily summaries and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
 
 ```python
 # Get the historical weather
 time_machine = meteosource.get_time_machine(
     date='2019-12-25',  # You can also pass list/tuple/set of dates, which can be 'str' or 'datetime' objects
     date_from=None,  # You can specify the range for dates you need, instead of list
     date_to=None,  # You can specify the range for dates you need, instead of list
@@ -171,18 +171,19 @@
 forecast.alerts.get_active_alerts() # returns list of SingleTimeData instances
 # You can use either string...
 forecast.alerts.get_active_alerts('2022-03-08T22:00:00')
 # ... or datetime (both tz-aware and naive)
 forecast.alerts.get_active_alerts(datetime(2022, 3, 8, 23, 0, 0))
 ```
 
-There are sections `data` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
+There are sections `data`, `daily` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
 ```python
 print(time_machine.data)  # <Instance of MultipleTimesData (time_machine) with 24 timesteps from 2019-12-25T00:00:00 to 2019-12-25T23:00:00>
 print(time_machine.statistics)  # <Instance of MultipleTimesData (statistics) with 1 timesteps from 2019-12-25 to 2019-12-25>
+print(time_machine.daily)  # <Instance of MultipleTimesData (daily) with 1 timesteps from 2019-12-25 to 2019-12-25>
 ```
 
 ### Time indexing
 
 As mentioned above, the `minutely`, `hourly`, `daily` sections of `Forecast` and the `data` section of `TimeMachine` contain data for more timesteps. To get the data for a single time, you have several options.
 
   **1. Indexing with integer**
@@ -261,14 +262,15 @@
 df = forecast.hourly.to_pandas()
 print(df)
 ```
 
 For historical weather data, you can also call the method on the `TimeMachine` object directly, so all following calls are valid:
 ```python
 time_machine.data.to_pandas()
+time_machine.daily.to_pandas()
 time_machine.statistics.to_pandas()
 time_machine.to_pandas()
 ```
 
 You can also merge the daily statistics and the hourly historical data into single `pandas` `DataFrame`. In this case, the daily statistics are duplicated into all hours of each day:
 ```python
 time_machine.to_pandas(include_statistics=True)
```

### Comparing `pymeteosource-1.5.0/pymeteosource/api.py` & `pymeteosource-1.6.0/pymeteosource/api.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/pymeteosource/data.py` & `pymeteosource-1.6.0/pymeteosource/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -514,14 +514,18 @@
         self.timezone = tz
         self.units = data['units']
         self.data = MultipleTimesData(data, 'time_machine', self.timezone)
         # Preprocess statistics to fit data structures
         statistics = {'data': [{'statistics': data['statistics']}]}
         statistics['data'][0]['day'] = day
         self.statistics = MultipleTimesData(statistics, 'statistics', 'UTC')
+        # Preprocess daily to fit data structures
+        daily = {'data': [{'daily': data['daily']}]}
+        daily['data'][0]['day'] = day
+        self.daily = MultipleTimesData(daily, 'daily', 'UTC')
 
         # Assing human-readable weather category from icon number
         for x in self.data.data:
             x.weather = ICONS.get(x.icon, 1)['weather']
             x.weather_id = ICONS.get(x.icon, 1)['weather_id']
 
     def append(self, other):
@@ -529,14 +533,15 @@
         Append another TimeMachine instance's data to this instance
 
         :param TimeMachine: TimeMachine instance to be appended
         """
         # Call MultipleTimesData's 'append' method
         self.data.append(other.data)
         self.statistics.append(other.statistics)
+        self.daily.append(other.daily)
 
     def __repr__(self):
         """
         Override __repr__ to have usefull text when attepting to print
         """
         return '<TimeMachine for lat: {}, lon: {}>'.format(self.lat, self.lon)
 
@@ -555,20 +560,26 @@
         setup.py to keep the dependencies as minimal as possible. To use this
         feature, use 'pip install pymeteosource[pandas]' to install this
         package, or install pandas manually using 'pip install pandas'.
 
         :param bool: If True, includes daily long term statistics epanded to hours
         :return pandas.DataFrame: The DataFrame with 'date' as index
         """
+        from pandas.api.types import is_datetime64_any_dtype as is_datetime
+
         res = self.data.to_pandas()
         if not include_statistics:
             return res
 
         # Convert statistics to pandas
         stats = self.statistics.to_pandas()
+        if is_datetime(stats.index):
+            stats.index = stats.index.date
+            stats.index.name = 'day'
+
         # Create helper column to merge the data on
         res['day'] = res.index.tz_convert('UTC').date
 
         # Merge the data with statistics and reset index to original
         res = res.reset_index().merge(stats, on='day', how='left').set_index('date')
         # Drop the helper column
         res = res.drop('day', axis=1)
```

### Comparing `pymeteosource-1.5.0/pymeteosource/errors.py` & `pymeteosource-1.6.0/pymeteosource/errors.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/pymeteosource/request_handler.py` & `pymeteosource-1.6.0/pymeteosource/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/pymeteosource/types/icons.py` & `pymeteosource-1.6.0/pymeteosource/types/icons.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/pymeteosource.egg-info/PKG-INFO` & `pymeteosource-1.6.0/pymeteosource.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pymeteosource
-Version: 1.5.0
+Version: 1.6.0
 Summary: Meteosource API wrapper library
-Home-page: https://github.com/Meteosource/pymeteosource/archive/v1.5.0.tar.gz
+Home-page: https://github.com/Meteosource/pymeteosource/archive/v1.6.0.tar.gz
 Author: Meteosource
 Author-email: support@meteosource.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -100,15 +100,15 @@
     tz='US/Pacific',  # Defaults to 'UTC', regardless of the point location
     lang=langs.ENGLISH,  # Defaults to 'en'
     units=units.US  # Defaults to 'auto'
 )
 ```
 
 ### Historical weather
-Users with paid subscription to Meteosource can retrieve historical weather and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
+Users with paid subscription to Meteosource can retrieve historical weather, daily summaries and long-term statistics from `time_machine` endpoint, using `get_time_machine()` method:
 
 ```python
 # Get the historical weather
 time_machine = meteosource.get_time_machine(
     date='2019-12-25',  # You can also pass list/tuple/set of dates, which can be 'str' or 'datetime' objects
     date_from=None,  # You can specify the range for dates you need, instead of list
     date_to=None,  # You can specify the range for dates you need, instead of list
@@ -187,18 +187,19 @@
 forecast.alerts.get_active_alerts() # returns list of SingleTimeData instances
 # You can use either string...
 forecast.alerts.get_active_alerts('2022-03-08T22:00:00')
 # ... or datetime (both tz-aware and naive)
 forecast.alerts.get_active_alerts(datetime(2022, 3, 8, 23, 0, 0))
 ```
 
-There are sections `data` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
+There are sections `data`, `daily` and `statistics` for historical weather as attributes in the `TimeMachine` object, both represented by `MultipleTimesData`.
 ```python
 print(time_machine.data)  # <Instance of MultipleTimesData (time_machine) with 24 timesteps from 2019-12-25T00:00:00 to 2019-12-25T23:00:00>
 print(time_machine.statistics)  # <Instance of MultipleTimesData (statistics) with 1 timesteps from 2019-12-25 to 2019-12-25>
+print(time_machine.daily)  # <Instance of MultipleTimesData (daily) with 1 timesteps from 2019-12-25 to 2019-12-25>
 ```
 
 ### Time indexing
 
 As mentioned above, the `minutely`, `hourly`, `daily` sections of `Forecast` and the `data` section of `TimeMachine` contain data for more timesteps. To get the data for a single time, you have several options.
 
   **1. Indexing with integer**
@@ -277,14 +278,15 @@
 df = forecast.hourly.to_pandas()
 print(df)
 ```
 
 For historical weather data, you can also call the method on the `TimeMachine` object directly, so all following calls are valid:
 ```python
 time_machine.data.to_pandas()
+time_machine.daily.to_pandas()
 time_machine.statistics.to_pandas()
 time_machine.to_pandas()
 ```
 
 You can also merge the daily statistics and the hourly historical data into single `pandas` `DataFrame`. In this case, the daily statistics are duplicated into all hours of each day:
 ```python
 time_machine.to_pandas(include_statistics=True)
```

### Comparing `pymeteosource-1.5.0/pymeteosource.egg-info/SOURCES.txt` & `pymeteosource-1.6.0/pymeteosource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/setup.py` & `pymeteosource-1.6.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 
 setup(
-    version="1.5.0",
+    version="1.6.0",
     name="pymeteosource",
     packages=find_packages(),
     install_requires=["wheel", "requests", "pytz"],
     extras_require={"pandas": "pandas"},
     description="Meteosource API wrapper library",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type='text/markdown',
     author="Meteosource",
     author_email="support@meteosource.com",
-    url="https://github.com/Meteosource/pymeteosource/archive/v1.5.0.tar.gz",
+    url="https://github.com/Meteosource/pymeteosource/archive/v1.6.0.tar.gz",
     license="MIT",
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.6",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `pymeteosource-1.5.0/tests/dst_changes_data.py` & `pymeteosource-1.6.0/tests/dst_changes_data.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/tests/sample_data.py` & `pymeteosource-1.6.0/tests/sample_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -25197,8 +25197,33 @@
 000626c0: 7970 6522 3a20 226e 6f6e 6522 0a20 2020  ype": "none".   
 000626d0: 2020 207d 2c0a 2020 2020 2020 2263 6170     },.      "cap
 000626e0: 6522 3a20 302c 0a20 2020 2020 2022 6576  e": 0,.      "ev
 000626f0: 6170 6f72 6174 696f 6e22 3a20 302c 0a20  aporation": 0,. 
 00062700: 2020 2020 2022 6972 7261 6469 616e 6365       "irradiance
 00062710: 223a 2030 2c0a 2020 2020 2020 226f 7a6f  ": 0,.      "ozo
 00062720: 6e65 223a 2032 3834 0a20 2020 207d 0a20  ne": 284.    }. 
-00062730: 205d 0a7d 0a                              ].}.
+00062730: 205d 2c0a 2020 2020 2273 7461 7469 7374   ],.    "statist
+00062740: 6963 7322 3a7b 0a20 2020 2020 2022 7465  ics":{.      "te
+00062750: 6d70 6572 6174 7572 6522 3a7b 0a20 2020  mperature":{.   
+00062760: 2020 2020 2020 2261 7667 223a 3133 2e30        "avg":13.0
+00062770: 2c0a 2020 2020 2020 2020 2022 6176 675f  ,.         "avg_
+00062780: 6d69 6e22 3a38 2e35 2c0a 2020 2020 2020  min":8.5,.      
+00062790: 2020 2022 6176 675f 6d61 7822 3a31 372e     "avg_max":17.
+000627a0: 352c 0a20 2020 2020 2020 2020 2272 6563  5,.         "rec
+000627b0: 6f72 645f 6d69 6e22 3a32 2e30 2c0a 2020  ord_min":2.0,.  
+000627c0: 2020 2020 2020 2022 7265 636f 7264 5f6d         "record_m
+000627d0: 6178 223a 3235 2e32 0a20 2020 2020 207d  ax":25.2.      }
+000627e0: 2c0a 2020 2020 2020 2277 696e 6422 3a7b  ,.      "wind":{
+000627f0: 0a20 2020 2020 2020 2020 2261 7667 5f73  .         "avg_s
+00062800: 7065 6564 223a 322e 392c 0a20 2020 2020  peed":2.9,.     
+00062810: 2020 2020 2261 7667 5f61 6e67 6c65 223a      "avg_angle":
+00062820: 3138 332c 0a20 2020 2020 2020 2020 2261  183,.         "a
+00062830: 7667 5f64 6972 223a 2253 222c 0a20 2020  vg_dir":"S",.   
+00062840: 2020 2020 2020 226d 6178 5f73 7065 6564        "max_speed
+00062850: 223a 3130 2e34 2c0a 2020 2020 2020 2020  ":10.4,.        
+00062860: 2022 6d61 785f 6775 7374 223a 3230 2e39   "max_gust":20.9
+00062870: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
+00062880: 2270 7265 6369 7069 7461 7469 6f6e 223a  "precipitation":
+00062890: 7b0a 2020 2020 2020 2020 2022 6176 6722  {.         "avg"
+000628a0: 3a31 2e30 2c0a 2020 2020 2020 2020 2022  :1.0,.         "
+000628b0: 7072 6f62 6162 696c 6974 7922 3a33 310a  probability":31.
+000628c0: 2020 2020 2020 7d0a 2020 207d 0a7d 0a          }.   }.}.
```

### Comparing `pymeteosource-1.5.0/tests/test_api.py` & `pymeteosource-1.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymeteosource-1.5.0/tests/variables_list.py` & `pymeteosource-1.6.0/tests/variables_list.py`

 * *Files identical despite different names*

