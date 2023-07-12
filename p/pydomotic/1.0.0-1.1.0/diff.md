# Comparing `tmp/pydomotic-1.0.0.tar.gz` & `tmp/pydomotic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydomotic-1.0.0.tar", last modified: Sun Jul  9 21:07:00 2023, max compression
+gzip compressed data, was "pydomotic-1.1.0.tar", last modified: Wed Jul 12 00:40:09 2023, max compression
```

## Comparing `pydomotic-1.0.0.tar` & `pydomotic-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-09 21:07:00.131058 pydomotic-1.0.0/
--rw-r--r--   0 rabo       (501) staff       (20)     4135 2023-07-09 21:07:00.130881 pydomotic-1.0.0/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)     3048 2023-07-09 20:48:49.000000 pydomotic-1.0.0/README.md
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-09 21:07:00.128510 pydomotic-1.0.0/pydomotic/
--rw-r--r--   0 rabo       (501) staff       (20)      388 2023-07-05 03:41:17.000000 pydomotic-1.0.0/pydomotic/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)      113 2023-07-04 19:56:42.000000 pydomotic-1.0.0/pydomotic/__main__.py
--rw-r--r--   0 rabo       (501) staff       (20)     1600 2023-07-08 03:14:05.000000 pydomotic-1.0.0/pydomotic/actions.py
--rw-r--r--   0 rabo       (501) staff       (20)     1268 2023-07-04 20:42:23.000000 pydomotic-1.0.0/pydomotic/components.py
--rw-r--r--   0 rabo       (501) staff       (20)     7881 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/context.py
--rw-r--r--   0 rabo       (501) staff       (20)      165 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/exceptions.py
--rw-r--r--   0 rabo       (501) staff       (20)     2385 2023-07-07 03:00:41.000000 pydomotic-1.0.0/pydomotic/handlers.py
--rw-r--r--   0 rabo       (501) staff       (20)       63 2023-07-05 03:26:18.000000 pydomotic-1.0.0/pydomotic/lambda_handler.py
--rw-r--r--   0 rabo       (501) staff       (20)    21606 2023-07-09 04:16:08.000000 pydomotic-1.0.0/pydomotic/parsers.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-09 21:07:00.130335 pydomotic-1.0.0/pydomotic/providers/
--rw-r--r--   0 rabo       (501) staff       (20)        0 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/providers/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)     2635 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/providers/airthings.py
--rw-r--r--   0 rabo       (501) staff       (20)      488 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/providers/base.py
--rw-r--r--   0 rabo       (501) staff       (20)      958 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/providers/fujitsu.py
--rw-r--r--   0 rabo       (501) staff       (20)     1383 2023-07-08 03:38:52.000000 pydomotic-1.0.0/pydomotic/providers/moen.py
--rw-r--r--   0 rabo       (501) staff       (20)      585 2023-07-04 21:25:43.000000 pydomotic-1.0.0/pydomotic/providers/noop.py
--rw-r--r--   0 rabo       (501) staff       (20)     1009 2023-07-05 02:57:40.000000 pydomotic-1.0.0/pydomotic/providers/tuya.py
--rw-r--r--   0 rabo       (501) staff       (20)     4934 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/sensors.py
--rw-r--r--   0 rabo       (501) staff       (20)     3608 2023-07-06 00:52:26.000000 pydomotic-1.0.0/pydomotic/triggers.py
--rw-r--r--   0 rabo       (501) staff       (20)     2931 2023-07-04 07:17:33.000000 pydomotic-1.0.0/pydomotic/utils.py
--rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-09 21:05:56.000000 pydomotic-1.0.0/pydomotic/version.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-09 21:07:00.129175 pydomotic-1.0.0/pydomotic.egg-info/
--rw-r--r--   0 rabo       (501) staff       (20)     4135 2023-07-09 21:07:00.000000 pydomotic-1.0.0/pydomotic.egg-info/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)      678 2023-07-09 21:07:00.000000 pydomotic-1.0.0/pydomotic.egg-info/SOURCES.txt
--rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-09 21:07:00.000000 pydomotic-1.0.0/pydomotic.egg-info/dependency_links.txt
--rw-r--r--   0 rabo       (501) staff       (20)      238 2023-07-09 21:07:00.000000 pydomotic-1.0.0/pydomotic.egg-info/requires.txt
--rw-r--r--   0 rabo       (501) staff       (20)       10 2023-07-09 21:07:00.000000 pydomotic-1.0.0/pydomotic.egg-info/top_level.txt
--rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-09 21:07:00.131261 pydomotic-1.0.0/setup.cfg
--rw-r--r--   0 rabo       (501) staff       (20)     2129 2023-07-09 07:41:05.000000 pydomotic-1.0.0/setup.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.341011 pydomotic-1.1.0/
+-rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-12 00:40:09.340868 pydomotic-1.1.0/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)     2770 2023-07-12 00:34:08.000000 pydomotic-1.1.0/README.md
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.338296 pydomotic-1.1.0/pydomotic/
+-rw-r--r--   0 rabo       (501) staff       (20)      388 2023-07-05 03:41:17.000000 pydomotic-1.1.0/pydomotic/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)      113 2023-07-04 19:56:42.000000 pydomotic-1.1.0/pydomotic/__main__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1600 2023-07-08 03:14:05.000000 pydomotic-1.1.0/pydomotic/actions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1268 2023-07-04 20:42:23.000000 pydomotic-1.1.0/pydomotic/components.py
+-rw-r--r--   0 rabo       (501) staff       (20)     7881 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/context.py
+-rw-r--r--   0 rabo       (501) staff       (20)      165 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/exceptions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2385 2023-07-07 03:00:41.000000 pydomotic-1.1.0/pydomotic/handlers.py
+-rw-r--r--   0 rabo       (501) staff       (20)       63 2023-07-05 03:26:18.000000 pydomotic-1.1.0/pydomotic/lambda_handler.py
+-rw-r--r--   0 rabo       (501) staff       (20)    21710 2023-07-12 00:11:15.000000 pydomotic-1.1.0/pydomotic/parsers.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.340566 pydomotic-1.1.0/pydomotic/providers/
+-rw-r--r--   0 rabo       (501) staff       (20)        0 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2635 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/airthings.py
+-rw-r--r--   0 rabo       (501) staff       (20)      488 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/base.py
+-rw-r--r--   0 rabo       (501) staff       (20)      958 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/fujitsu.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1383 2023-07-08 03:38:52.000000 pydomotic-1.1.0/pydomotic/providers/moen.py
+-rw-r--r--   0 rabo       (501) staff       (20)      585 2023-07-04 21:25:43.000000 pydomotic-1.1.0/pydomotic/providers/noop.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1040 2023-07-12 00:14:50.000000 pydomotic-1.1.0/pydomotic/providers/tuya.py
+-rw-r--r--   0 rabo       (501) staff       (20)     4934 2023-07-10 04:10:04.000000 pydomotic-1.1.0/pydomotic/sensors.py
+-rw-r--r--   0 rabo       (501) staff       (20)     3608 2023-07-06 00:52:26.000000 pydomotic-1.1.0/pydomotic/triggers.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2931 2023-07-09 23:04:01.000000 pydomotic-1.1.0/pydomotic/utils.py
+-rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-12 00:40:00.000000 pydomotic-1.1.0/pydomotic/version.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.338973 pydomotic-1.1.0/pydomotic.egg-info/
+-rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)      678 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/SOURCES.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/dependency_links.txt
+-rw-r--r--   0 rabo       (501) staff       (20)      393 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/requires.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       10 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/top_level.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-12 00:40:09.341057 pydomotic-1.1.0/setup.cfg
+-rw-r--r--   0 rabo       (501) staff       (20)     2367 2023-07-12 00:19:04.000000 pydomotic-1.1.0/setup.py
```

### Comparing `pydomotic-1.0.0/PKG-INFO` & `pydomotic-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydomotic
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for home automation execution, enabling seamless control and management of your IoT devices
 Home-page: https://github.com/purple4reina/pydomotic
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/pydomotic
 Project-URL: Bug Tracker, https://github.com/purple4reina/pydomotic/issues
@@ -21,32 +21,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: airthings
 Provides-Extra: fujitsu
 Provides-Extra: moen
 Provides-Extra: tuya
 Provides-Extra: s3
 Provides-Extra: tz
+Provides-Extra: all
 
 # pydomotic
 
-<!--
-  + [x] change top level "triggers" yaml
-  + README
-    - [x] Deploying
-    - [ ] Contributing (defer)
-    - [x] Actions
-    - [ ] Why you should use this package (defer)
-    - [ ] Available device actions (defer)
-  + [x] update setup.py and dependencies
-  + [x] document installing extras: `pip install pydomotic[tuya]`
-  + [ ] bump major version and push to pypi
-  + [ ] add status tags to README
-  + [x] update home-automations
-  + [ ] improve test coverage
--->
+[![PyPI version](https://badge.fury.io/py/pydomotic.svg)](https://badge.fury.io/py/pydomotic)
 
 A Python library for home automation execution, enabling seamless control and
 management of your IoT devices.
 
 _"Domotics": The automatic control of home appliances by electronic systems.
 Contraction of domestic robotics, from the Latin domus ("home"), and robotics._
 
@@ -89,17 +76,17 @@
 
 1. Running the following will check each trigger and execute any actions.
 
     ```bash
     $ python -m pydomotic
     ```
 
-Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](./docs/CONFIGURATION.md).
+Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](https://github.com/purple4reina/pydomotic/blob/main/docs/CONFIGURATION.md)
 
-For more details on deployment options, see [DEPLOYING.md](./docs/DEPLOYING.md).
+For more details on deployment options, see [DEPLOYING.md](https://github.com/purple4reina/pydomotic/blob/main/docs/DEPLOYING.md)
 
 ## Glossary
 
 **trigger:** A small piece of code which evaluates to either true or false.
 Usually it calls on devices or 3rd party APIs to make this determination.
 
 **action:** A small piece of code which is run when a trigger fires. Usually
```

### Comparing `pydomotic-1.0.0/README.md` & `pydomotic-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,10 @@
 # pydomotic
 
-<!--
-  + [x] change top level "triggers" yaml
-  + README
-    - [x] Deploying
-    - [ ] Contributing (defer)
-    - [x] Actions
-    - [ ] Why you should use this package (defer)
-    - [ ] Available device actions (defer)
-  + [x] update setup.py and dependencies
-  + [x] document installing extras: `pip install pydomotic[tuya]`
-  + [ ] bump major version and push to pypi
-  + [ ] add status tags to README
-  + [x] update home-automations
-  + [ ] improve test coverage
--->
+[![PyPI version](https://badge.fury.io/py/pydomotic.svg)](https://badge.fury.io/py/pydomotic)
 
 A Python library for home automation execution, enabling seamless control and
 management of your IoT devices.
 
 _"Domotics": The automatic control of home appliances by electronic systems.
 Contraction of domestic robotics, from the Latin domus ("home"), and robotics._
 
@@ -61,17 +47,17 @@
 
 1. Running the following will check each trigger and execute any actions.
 
     ```bash
     $ python -m pydomotic
     ```
 
-Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](./docs/CONFIGURATION.md).
+Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](https://github.com/purple4reina/pydomotic/blob/main/docs/CONFIGURATION.md)
 
-For more details on deployment options, see [DEPLOYING.md](./docs/DEPLOYING.md).
+For more details on deployment options, see [DEPLOYING.md](https://github.com/purple4reina/pydomotic/blob/main/docs/DEPLOYING.md)
 
 ## Glossary
 
 **trigger:** A small piece of code which evaluates to either true or false.
 Usually it calls on devices or 3rd party APIs to make this determination.
 
 **action:** A small piece of code which is run when a trigger fires. Usually
```

### Comparing `pydomotic-1.0.0/pydomotic/actions.py` & `pydomotic-1.1.0/pydomotic/actions.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/components.py` & `pydomotic-1.1.0/pydomotic/components.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/context.py` & `pydomotic-1.1.0/pydomotic/context.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/handlers.py` & `pydomotic-1.1.0/pydomotic/handlers.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/parsers.py` & `pydomotic-1.1.0/pydomotic/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,18 +121,19 @@
 
     username = _parse_string(provider['username'])
     password = _parse_string(provider['password'])
     access_id = _parse_string(provider['access_id'])
     access_key = _parse_string(provider['access_key'])
 
     cache_secs = provider.get('device_status_cache_seconds')
+    timeout = provider.get('timeout_seconds')
 
     from .providers.tuya import TuyaProvider
     return TuyaProvider(username, password, access_id, access_key,
-            status_cache_seconds=cache_secs)
+            status_cache_seconds=cache_secs, timeout=timeout)
 
 def _parse_fujitsu_provider(provider):
     for key in ('username', 'password'):
         if key not in provider:
             raise PyDomoticConfigParsingError(
                     f'provider fujitsu requires key "{key}"')
 
@@ -255,26 +256,26 @@
         trigger = _parse_radon_trigger(value, context, sensor=sensor)
     elif typ == 'webhook':
         # TODO: test _parse_triggers
         trigger = _parse_webhook_trigger(value, context, sensor=sensor)
     elif typ in context.devices:
         if sensor:
             raise PyDomoticConfigParsingError('nested sensor confs not allowed')
-        trigger = _parse_sensor(typ, value, context)
+        trigger = _parse_sensor_trigger(typ, value, context)
     else:
         raise PyDomoticConfigParsingError(f'unknown trigger type "{typ}"')
     return trigger
 
 _ranged_value_aqi_re = re.compile(r'(<|>|==|<=|>=)?\s*(\d+\.?\d*)')
 _ranged_value_temp_re = re.compile(r'(<|>|==|<=|>=)?\s*(\d+\.?\d*|\$\{temp\})')
 def _parse_ranged_values(value, typ, context):
     if not isinstance(value, (str, int, float)):
         raise PyDomoticConfigParsingError(
-                f'invalid {typ} trigger value "{value}", expecting value like '
-                '">100", "<100", or "100"')
+                f'invalid {typ} trigger value "{value}", expecting string or '
+                'number value like ">100", "<100", or "100"')
 
     def _ranged_func(start, end):
         return lambda a: a >= start and a <= end
 
     def _relative_func(op, val):
         value_func = _get_value_func(val)
         if op == '>':
@@ -322,19 +323,19 @@
         elif len(ranged_val) == 2:
             try:
                 start_val = float(ranged_val[0])
                 end_val = float(ranged_val[1])
                 _check_func = _ranged_func(start_val, end_val)
             except:
                 raise PyDomoticConfigParsingError(
-                        f'invalid {typ} trigger value "{val}", expecting value '
-                        'like "80-100"')
+                        f'invalid {typ} trigger value "{val}", expecting ranged '
+                        'value like "80-100"')
 
         else:
-            raise PyDomoticConfigParsingError(f'unknown {typ} "{val}')
+            raise PyDomoticConfigParsingError(f'unknown {typ} "{val}"')
 
         _check_funcs.append(_check_func)
     return lambda a: any(fn(a) for fn in _check_funcs)
 
 def _parse_aqi_trigger(value, context, sensor=None):
     _check_func = _parse_ranged_values(value, 'aqi', context)
     sensor = sensor or context.aqi_sensor
@@ -478,15 +479,15 @@
     _check_func = _parse_ranged_values(value, 'radon', context)
     return RadonTrigger(_check_func, sensor)
 
 def _parse_webhook_trigger(value, context, sensor=None):
     # TODO: test _parse_webhook_trigger
     return WebhookTrigger(value, sensor or context.webhook_sensor)
 
-def _parse_sensor(device_name, value, context):
+def _parse_sensor_trigger(device_name, value, context):
     # TODO: test value is None
     if value is None:
         raise PyDomoticConfigParsingError(
                 f'sensor trigger for {device_name} requires a value')
     sensor = context.device_sensor(device_name)
     trigger_type, trigger_value = value.popitem()
     if value:
```

### Comparing `pydomotic-1.0.0/pydomotic/providers/airthings.py` & `pydomotic-1.1.0/pydomotic/providers/airthings.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/providers/fujitsu.py` & `pydomotic-1.1.0/pydomotic/providers/fujitsu.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/providers/moen.py` & `pydomotic-1.1.0/pydomotic/providers/moen.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/providers/noop.py` & `pydomotic-1.1.0/pydomotic/providers/noop.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/sensors.py` & `pydomotic-1.1.0/pydomotic/sensors.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/triggers.py` & `pydomotic-1.1.0/pydomotic/triggers.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic/utils.py` & `pydomotic-1.1.0/pydomotic/utils.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/pydomotic.egg-info/PKG-INFO` & `pydomotic-1.1.0/pydomotic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydomotic
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for home automation execution, enabling seamless control and management of your IoT devices
 Home-page: https://github.com/purple4reina/pydomotic
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/pydomotic
 Project-URL: Bug Tracker, https://github.com/purple4reina/pydomotic/issues
@@ -21,32 +21,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: airthings
 Provides-Extra: fujitsu
 Provides-Extra: moen
 Provides-Extra: tuya
 Provides-Extra: s3
 Provides-Extra: tz
+Provides-Extra: all
 
 # pydomotic
 
-<!--
-  + [x] change top level "triggers" yaml
-  + README
-    - [x] Deploying
-    - [ ] Contributing (defer)
-    - [x] Actions
-    - [ ] Why you should use this package (defer)
-    - [ ] Available device actions (defer)
-  + [x] update setup.py and dependencies
-  + [x] document installing extras: `pip install pydomotic[tuya]`
-  + [ ] bump major version and push to pypi
-  + [ ] add status tags to README
-  + [x] update home-automations
-  + [ ] improve test coverage
--->
+[![PyPI version](https://badge.fury.io/py/pydomotic.svg)](https://badge.fury.io/py/pydomotic)
 
 A Python library for home automation execution, enabling seamless control and
 management of your IoT devices.
 
 _"Domotics": The automatic control of home appliances by electronic systems.
 Contraction of domestic robotics, from the Latin domus ("home"), and robotics._
 
@@ -89,17 +76,17 @@
 
 1. Running the following will check each trigger and execute any actions.
 
     ```bash
     $ python -m pydomotic
     ```
 
-Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](./docs/CONFIGURATION.md).
+Note that each configured provider will require separate installation of its specific dependencies. For installing these dependencies and full configuration documentation, see [CONFIGURATION.md](https://github.com/purple4reina/pydomotic/blob/main/docs/CONFIGURATION.md)
 
-For more details on deployment options, see [DEPLOYING.md](./docs/DEPLOYING.md).
+For more details on deployment options, see [DEPLOYING.md](https://github.com/purple4reina/pydomotic/blob/main/docs/DEPLOYING.md)
 
 ## Glossary
 
 **trigger:** A small piece of code which evaluates to either true or false.
 Usually it calls on devices or 3rd party APIs to make this determination.
 
 **action:** A small piece of code which is run when a trigger fires. Usually
```

### Comparing `pydomotic-1.0.0/pydomotic.egg-info/SOURCES.txt` & `pydomotic-1.1.0/pydomotic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydomotic-1.0.0/setup.py` & `pydomotic-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,35 @@
     for line in read(rel_path).splitlines():
         if line.startswith('version'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError('Unable to find version string.')
 
+def get_extras_require():
+    # providers
+    airthings = []
+    fujitsu = ['pyfujitsu>=0.9.0,<1.0']
+    moen = ['pyflowater>=0.5.2,<1.0', 'retry>=0.9.2,<1.0']
+    tuya = ['gosundpy>=0.7.0,<1.0']
+
+    # features
+    s3 = ['boto3>=1.26.3,<2.0']
+    tz = ['timezonefinder>=6.1.8,<7.0']
+
+    return {
+        'airthings': airthings,
+        'fujitsu': fujitsu,
+        'moen': moen,
+        'tuya': tuya,
+        's3': s3,
+        'tz': tz,
+        'all': airthings + fujitsu + moen + tuya + s3 + tz,
+    }
+
 setup(
     name='pydomotic',
     version=get_version('pydomotic/version.py'),
     url='https://github.com/purple4reina/pydomotic',
     author='Rey Abolofia',
     author_email='purple4reina@gmail.com',
     keywords='iot,python,home,automation,smart,domotic',
@@ -44,20 +65,11 @@
     ],
     install_requires=[
         'PyYAML>=6.0,<7.0',
         'astral>=3.0,<4.0',
         'croniter>=1.3.15,<2.0',
         'pyowm>=3.3.0,<4.0',
     ],
-    extras_require={
-        # providers
-        'airthings': [],
-        'fujitsu': ['pyfujitsu>=0.9.0,<1.0'],
-        'moen': ['pyflowater>=0.5.2,<1.0'],
-        'tuya': ['gosundpy>=0.6.2,<1.0'],
-        # features
-        's3': ['boto3>=1.26.3,<2.0'],
-        'tz': ['timezonefinder>=6.1.8,<7.0'],
-    },
+    extras_require=get_extras_require(),
     packages=find_packages(),
     python_requires='>=3.8,<4',
 )
```

