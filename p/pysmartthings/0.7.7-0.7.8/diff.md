# Comparing `tmp/pysmartthings-0.7.7.tar.gz` & `tmp/pysmartthings-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmartthings-0.7.7.tar", last modified: Fri Nov 12 18:43:43 2021, max compression
+gzip compressed data, was "pysmartthings-0.7.8.tar", last modified: Wed Jul 12 01:44:31 2023, max compression
```

## Comparing `pysmartthings-0.7.7.tar` & `pysmartthings-0.7.8.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 18:43:43.169926 pysmartthings-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (121)    10892 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-11-12 18:43:43.169926 pysmartthings-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 18:43:43.165926 pysmartthings-0.7.7/pysmartthings/
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15594 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13422 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    13938 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/capability.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/const.py
--rw-r--r--   0 runner    (1001) docker     (121)    49389 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/installedapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/location.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/oauthtoken.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/room.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/scene.py
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/smartthings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7977 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/pysmartthings/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 18:43:43.169926 pysmartthings-0.7.7/pysmartthings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-12 18:43:43.000000 pysmartthings-0.7.7/pysmartthings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-12 18:43:43.169926 pysmartthings-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-11-12 18:43:27.000000 pysmartthings-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:31.662599 pysmartthings-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-12 01:44:31.662599 pysmartthings-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:31.658599 pysmartthings-0.7.8/pysmartthings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51348 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/installedapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/oauthtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/smartthings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/pysmartthings/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:31.658599 pysmartthings-0.7.8/pysmartthings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 01:44:31.000000 pysmartthings-0.7.8/pysmartthings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:31.662599 pysmartthings-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:31.662599 pysmartthings-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59248 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_installedapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_oauthtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_smartthings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-12 01:44:10.000000 pysmartthings-0.7.8/tests/test_subscription.py
```

### Comparing `pysmartthings-0.7.7/LICENSE` & `pysmartthings-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/PKG-INFO` & `pysmartthings-0.7.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pysmartthings
-Version: 0.7.7
+Version: 0.7.8
 Summary: A python library for interacting with the SmartThings cloud API build with asyncio and aiohttp.
 Home-page: https://github.com/andrewsayre/pysmartthings
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: ASL 2.0
 Keywords: smartthings
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmartthings
 
+[![CI Status](https://github.com/andrewsayre/pysmartthings/workflows/CI/badge.svg)](https://github.com/andrewsayre/pysmartthings/actions)
+[![codecov](https://codecov.io/gh/andrewsayre/pysmartthings/branch/dev/graph/badge.svg?token=Q13LDPU5MF)](https://codecov.io/gh/andrewsayre/pysmartthings)
 [![image](https://img.shields.io/pypi/v/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/pyversions/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/l/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 
 A python library for interacting with the SmartThings cloud API build with [asyncio](https://docs.python.org/3/library/asyncio.html) and [aiohttp](https://aiohttp.readthedocs.io/en/stable/).
 
 ## Features
@@ -157,8 +159,13 @@
 Devices with the `switchLevel` capability have the following function that sets the target brightness level and transitions using a specific duration (seconds).
 
 ```pythonstub
     result = await device.set_level(75, 2)
     assert result == True
 ```
 
+Devices with the `windowShadeLevel` capability have the following function that sets the target shade level.
 
+```pythonstub
+    result = await device.set_window_shade_level(50)
+    assert result == True
+```
```

### Comparing `pysmartthings-0.7.7/README.md` & `pysmartthings-0.7.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pysmartthings
 
+[![CI Status](https://github.com/andrewsayre/pysmartthings/workflows/CI/badge.svg)](https://github.com/andrewsayre/pysmartthings/actions)
+[![codecov](https://codecov.io/gh/andrewsayre/pysmartthings/branch/dev/graph/badge.svg?token=Q13LDPU5MF)](https://codecov.io/gh/andrewsayre/pysmartthings)
 [![image](https://img.shields.io/pypi/v/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/pyversions/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/l/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 
 A python library for interacting with the SmartThings cloud API build with [asyncio](https://docs.python.org/3/library/asyncio.html) and [aiohttp](https://aiohttp.readthedocs.io/en/stable/).
 
 ## Features
@@ -135,7 +137,14 @@
 
 Devices with the `switchLevel` capability have the following function that sets the target brightness level and transitions using a specific duration (seconds).
 
 ```pythonstub
     result = await device.set_level(75, 2)
     assert result == True
 ```
+
+Devices with the `windowShadeLevel` capability have the following function that sets the target shade level.
+
+```pythonstub
+    result = await device.set_window_shade_level(50)
+    assert result == True
+```
```

### Comparing `pysmartthings-0.7.7/pysmartthings/__init__.py` & `pysmartthings-0.7.8/pysmartthings/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/api.py` & `pysmartthings-0.7.8/pysmartthings/api.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/app.py` & `pysmartthings-0.7.8/pysmartthings/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,15 @@
         """
         return self._app_type
 
     @app_type.setter
     def app_type(self, value: str):
         """Set the app type."""
         if value not in (APP_TYPE_LAMBDA, APP_TYPE_WEBHOOK):
-            raise ValueError(
-                "value must be 'LAMBDA_SMART_APP' " "or 'WEBHOOK_SMART_APP'"
-            )
+            raise ValueError("value must be 'LAMBDA_SMART_APP' or 'WEBHOOK_SMART_APP'")
         self._app_type = value
 
     @property
     def lambda_functions(self) -> List[str]:
         """
         Get the list of AWS arns referencing a Lambda function.
```

### Comparing `pysmartthings-0.7.7/pysmartthings/capability.py` & `pysmartthings-0.7.8/pysmartthings/capability.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "dryerJobState",
         "completionTime",
     ],
     "dustSensor": ["fineDustLevel", "dustLevel"],
     "energyMeter": ["energy"],
     "equivalentCarbonDioxideMeasurement": ["equivalentCarbonDioxideMeasurement"],
     "execute": ["data"],
+    "fanOscillationMode": ["fanOscillationMode", "supportedFanOscillationModes"],
     "fanSpeed": ["fanSpeed"],
     "filterStatus": ["filterStatus"],
     "formaldehydeMeasurement": ["formaldehydeLevel"],
     "garageDoorControl": ["door"],
     "gasMeter": [
         "gasMeter",
         "gasMeterCalorific",
@@ -142,14 +143,16 @@
         "machineState",
         "supportedMachineStates",
         "washerJobState",
         "completionTime",
     ],
     "waterSensor": ["water"],
     "windowShade": ["windowShade"],
+    "windowShadeLevel": ["shadeLevel"],
+    "windowShadePreset": ["presetPosition"],
 }
 CAPABILITIES = list(CAPABILITIES_TO_ATTRIBUTES)
 ATTRIBUTES = {
     attrib
     for attributes in CAPABILITIES_TO_ATTRIBUTES.values()
     for attrib in attributes
 }
@@ -183,14 +186,15 @@
     door_control = "doorControl"
     dryer_mode = "dryerMode"
     dryer_operating_state = "dryerOperatingState"
     dust_sensor = "dustSensor"
     energy_meter = "energyMeter"
     equivalent_carbon_dioxide_measurement = "equivalentCarbonDioxideMeasurement"
     execute = "execute"
+    fan_oscillation_mode = "fanOscillationMode"
     fan_speed = "fanSpeed"
     filter_status = "filterStatus"
     formaldehyde_measurement = "formaldehydeMeasurement"
     garage_door_control = "garageDoorControl"
     gas_meter = "gasMeter"
     illuminance_measurement = "illuminanceMeasurement"
     infrared_level = "infraredLevel"
@@ -235,14 +239,16 @@
     ultraviolet_index = "ultravioletIndex"
     valve = "valve"
     voltage_measurement = "voltageMeasurement"
     washer_mode = "washerMode"
     washer_operating_state = "washerOperatingState"
     water_sensor = "waterSensor"
     window_shade = "windowShade"
+    window_shade_level = "windowShadeLevel"
+    window_shade_preset = "windowShadePreset"
 
 
 class Attribute:
     """Define common attributes."""
 
     acceleration = "acceleration"
     air_conditioner_mode = "airConditionerMode"
@@ -271,14 +277,15 @@
     drlc_status = "drlcStatus"
     dryer_job_state = "dryerJobState"
     dryer_mode = "dryerMode"
     dust_level = "dustLevel"
     energy = "energy"
     equivalent_carbon_dioxide_measurement = "equivalentCarbonDioxideMeasurement"
     fan_mode = "fanMode"
+    fan_oscillation_mode = "fanOscillationMode"
     fan_speed = "fanSpeed"
     filter_status = "filterStatus"
     fine_dust_level = "fineDustLevel"
     formaldehyde_level = "formaldehydeLevel"
     gas_meter = "gasMeter"
     gas_meter_calorific = "gasMeterCalorific"
     gas_meter_conversion = "gasMeterConversion"
@@ -320,29 +327,32 @@
     playback_repeat_mode = "playbackRepeatMode"
     playback_shuffle = "playbackShuffle"
     playback_status = "playbackStatus"
     power = "power"
     power_consumption = "powerConsumption"
     power_source = "powerSource"
     presence = "presence"
+    preset_position = "presetPosition"
     progress = "progress"
     rapid_cooling = "rapidCooling"
     refrigeration_setpoint = "refrigerationSetpoint"
     robot_cleaner_cleaning_mode = "robotCleanerCleaningMode"
     robot_cleaner_movement = "robotCleanerMovement"
     robot_cleaner_turbo_mode = "robotCleanerTurboMode"
     rssi = "rssi"
     saturation = "saturation"
     schedule = "schedule"
+    shade_level = "shadeLevel"
     smoke = "smoke"
     sound = "sound"
     st = "st"
     supported_ac_fan_modes = "supportedAcFanModes"
     supported_ac_modes = "supportedAcModes"
     supported_button_values = "supportedButtonValues"
+    supported_fan_oscillation_modes = "supportedFanOscillationModes"
     supported_input_sources = "supportedInputSources"
     supported_machine_states = "supportedMachineStates"
     supported_playback_commands = "supportedPlaybackCommands"
     supported_thermostat_fan_modes = "supportedThermostatFanModes"
     supported_thermostat_modes = "supportedThermostatModes"
     switch = "switch"
     tamper = "tamper"
```

### Comparing `pysmartthings-0.7.7/pysmartthings/device.py` & `pysmartthings-0.7.8/pysmartthings/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,22 +54,24 @@
     preset_position = "presetPosition"
     request_drlc_action = "requestDrlcAction"
     set_air_flow_direction = "setAirFlowDirection"
     set_air_conditioner_mode = "setAirConditionerMode"
     set_color = "setColor"
     set_color_temperature = "setColorTemperature"
     set_cooling_setpoint = "setCoolingSetpoint"
+    set_fan_oscillation_mode = "setFanOscillationMode"
     set_fan_mode = "setFanMode"
     set_fan_speed = "setFanSpeed"
     set_heating_setpoint = "setHeatingSetpoint"
     set_hue = "setHue"
     set_level = "setLevel"
     set_saturation = "setSaturation"
     set_thermostat_fan_mode = "setThermostatFanMode"
     set_thermostat_mode = "setThermostatMode"
+    set_shade_level = "setShadeLevel"
     unlock = "unlock"
     mute = "mute"
     unmute = "unmute"
     set_volume = "setVolume"
     volume_up = "volumeUp"
     volume_down = "volumeDown"
     play = "play"
@@ -608,14 +610,19 @@
 
     @property
     def fan_mode(self) -> Optional[str]:
         """Get the fan mode attribute."""
         return self._attributes[Attribute.fan_mode].value
 
     @property
+    def fan_oscillation_mode(self) -> Optional[str]:
+        """Get the fan oscillation mode attribute."""
+        return self._attributes[Attribute.fan_oscillation_mode].value
+
+    @property
     def supported_ac_fan_modes(self) -> Sequence[str]:
         """Get the supported AC fan modes attribute."""
         value = self._attributes[Attribute.supported_ac_fan_modes].value
         # pylint: disable=isinstance-second-argument-not-valid-type
         if isinstance(value, Sequence):
             return sorted(value)
         return []
@@ -717,14 +724,26 @@
         self.update_attribute_value(Attribute.tv_channel, value)
 
     @property
     def media_title(self) -> bool:
         """Get the trackDescription attribute."""
         return self._attributes["trackDescription"].value
 
+    @property
+    def shade_level(self) -> int:
+        """Get the shadeLevel attribute, scaled 0-100."""
+        return int(self._attributes[Attribute.shade_level].value or 0)
+
+    @shade_level.setter
+    def shade_level(self, value: int):
+        """Set the level of the attribute, scaled 0-100."""
+        if not 0 <= value <= 100:
+            raise ValueError("value must be scaled between 0-100.")
+        self.update_attribute_value(Attribute.shade_level, value)
+
 
 class DeviceStatus(DeviceStatusBase):
     """Define the device status."""
 
     def __init__(self, api: Api, device_id: str, data=None):
         """Create a new instance of the DeviceStatusEntity class."""
         super().__init__("main")
@@ -838,15 +857,15 @@
         component_id: str = "main",
     ) -> bool:
         """Call the set color command."""
         color_map = {}
         if color_hex:
             if not COLOR_HEX_MATCHER.match(color_hex):
                 raise ValueError(
-                    "color_hex was not a properly formatted " "color hex, i.e. #000000."
+                    "color_hex was not a properly formatted color hex, i.e. #000000."
                 )
             color_map["hex"] = color_hex
         else:
             if not 0 <= hue <= 100:
                 raise ValueError("hue must be scaled between 0-100.")
             if not 0 <= saturation <= 100:
                 raise ValueError("saturation must be scaled between 0-100.")
@@ -1176,14 +1195,28 @@
             Command.set_fan_mode,
             [mode],
         )
         if result and set_status:
             self.status.update_attribute_value(Attribute.fan_mode, mode)
         return result
 
+    async def set_fan_oscillation_mode(
+        self, mode: str, *, set_status: bool = False, component_id: str = "main"
+    ):
+        """Call the setFanOscillationMode command."""
+        result = await self.command(
+            component_id,
+            Capability.fan_oscillation_mode,
+            Command.set_fan_oscillation_mode,
+            [mode],
+        )
+        if result and set_status:
+            self.status.update_attribute_value(Attribute.fan_oscillation_mode, mode)
+        return result
+
     async def set_air_flow_direction(
         self, direction: str, *, set_status: bool = False, component_id: str = "main"
     ):
         """Call the setAirFlowDirection command."""
         result = await self.command(
             component_id,
             Capability.air_flow_direction,
@@ -1366,11 +1399,33 @@
         self, set_status: bool = False, *, component_id: str = "main"
     ) -> bool:
         """Call the channelDown command."""
         return await self.command(
             component_id, Capability.tv_channel, Command.channel_down
         )
 
+    async def set_window_shade_level(
+        self,
+        level: int,
+        set_status: bool = False,
+        *,
+        component_id: str = "main",
+    ) -> bool:
+        """Call the set shade level device command."""
+        if not 0 <= level <= 100:
+            raise ValueError("level must be scaled between 0-100.")
+
+        result = await self.command(
+            component_id,
+            Capability.window_shade_level,
+            Command.set_shade_level,
+            [level],
+        )
+        if result and set_status:
+            self.status.shade_level = level
+            self.status.switch = level > 0
+        return result
+
     @property
     def status(self):
         """Get the status entity of the device."""
         return self._status
```

### Comparing `pysmartthings-0.7.7/pysmartthings/errors.py` & `pysmartthings-0.7.8/pysmartthings/errors.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/installedapp.py` & `pysmartthings-0.7.8/pysmartthings/installedapp.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/location.py` & `pysmartthings-0.7.8/pysmartthings/location.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/oauthtoken.py` & `pysmartthings-0.7.8/pysmartthings/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/room.py` & `pysmartthings-0.7.8/pysmartthings/room.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/scene.py` & `pysmartthings-0.7.8/pysmartthings/scene.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/smartthings.py` & `pysmartthings-0.7.8/pysmartthings/smartthings.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings/subscription.py` & `pysmartthings-0.7.8/pysmartthings/subscription.py`

 * *Files identical despite different names*

### Comparing `pysmartthings-0.7.7/pysmartthings.egg-info/PKG-INFO` & `pysmartthings-0.7.8/pysmartthings.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pysmartthings
-Version: 0.7.7
+Version: 0.7.8
 Summary: A python library for interacting with the SmartThings cloud API build with asyncio and aiohttp.
 Home-page: https://github.com/andrewsayre/pysmartthings
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: ASL 2.0
 Keywords: smartthings
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmartthings
 
+[![CI Status](https://github.com/andrewsayre/pysmartthings/workflows/CI/badge.svg)](https://github.com/andrewsayre/pysmartthings/actions)
+[![codecov](https://codecov.io/gh/andrewsayre/pysmartthings/branch/dev/graph/badge.svg?token=Q13LDPU5MF)](https://codecov.io/gh/andrewsayre/pysmartthings)
 [![image](https://img.shields.io/pypi/v/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/pyversions/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 [![image](https://img.shields.io/pypi/l/pysmartthings.svg)](https://pypi.org/project/pysmartthings/)
 
 A python library for interacting with the SmartThings cloud API build with [asyncio](https://docs.python.org/3/library/asyncio.html) and [aiohttp](https://aiohttp.readthedocs.io/en/stable/).
 
 ## Features
@@ -157,8 +159,13 @@
 Devices with the `switchLevel` capability have the following function that sets the target brightness level and transitions using a specific duration (seconds).
 
 ```pythonstub
     result = await device.set_level(75, 2)
     assert result == True
 ```
 
+Devices with the `windowShadeLevel` capability have the following function that sets the target shade level.
 
+```pythonstub
+    result = await device.set_window_shade_level(50)
+    assert result == True
+```
```

### Comparing `pysmartthings-0.7.7/setup.py` & `pysmartthings-0.7.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andrewsayre/pysmartthings",
     author="Andrew Sayre",
     author_email="andrew@sayre.net",
     license="ASL 2.0",
     packages=find_packages(exclude=("tests*",)),
-    install_requires=["aiohttp>=3.8.0,<4.0.0"],
+    install_requires=["aiohttp>=3.8.4,<4.0.0"],
     tests_require=[],
     platforms=["any"],
     keywords="smartthings",
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries",
         "Topic :: Home Automation",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

