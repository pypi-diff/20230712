# Comparing `tmp/lnetatmo-2.0.0.tar.gz` & `tmp/lnetatmo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lnetatmo-2.0.0.tar", last modified: Mon Dec  7 10:49:39 2020, max compression
+gzip compressed data, was "dist/lnetatmo-2.1.0.tar", last modified: Mon Dec 14 10:24:28 2020, max compression
```

## Comparing `lnetatmo-2.0.0.tar` & `lnetatmo-2.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-07 10:49:39.065949 lnetatmo-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      598 2020-12-07 10:49:39.065949 lnetatmo-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34931 2020-12-07 10:06:50.040965 lnetatmo-2.0.0/lnetatmo.py
--rw-r--r--   0 root         (0) root         (0)       41 2020-03-16 08:41:16.034868 lnetatmo-2.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      760 2020-12-07 10:08:04.503859 lnetatmo-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 10:24:28.150337 lnetatmo-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      598 2020-12-14 10:24:28.150337 lnetatmo-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34958 2020-12-14 10:08:31.628481 lnetatmo-2.1.0/lnetatmo.py
+-rw-r--r--   0 root         (0) root         (0)       41 2020-03-16 08:41:16.034868 lnetatmo-2.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      760 2020-12-14 10:23:24.603278 lnetatmo-2.1.0/setup.py
```

### Comparing `lnetatmo-2.0.0/PKG-INFO` & `lnetatmo-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: lnetatmo
-Version: 2.0.0
+Version: 2.1.0
 Summary: Simple API to access Netatmo weather station data from any python script.
 Home-page: https://github.com/philippelt/netatmo-api-python
 Author: Philippe Larduinat
 Author-email: ph.larduinat@wanadoo.fr
 License: GPL V3
-Download-URL: https://github.com/philippelt/netatmo-api-python/tarball/v2.0.0.tar.gz
+Download-URL: https://github.com/philippelt/netatmo-api-python/archive/v2.1.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnetatmo-2.0.0/lnetatmo.py` & `lnetatmo-2.1.0/lnetatmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 _GETHOMEDATA_REQ       = _BASE_URL + "api/gethomedata"
 _GETCAMERAPICTURE_REQ  = _BASE_URL + "api/getcamerapicture"
 _GETEVENTSUNTIL_REQ    = _BASE_URL + "api/geteventsuntil"
 
 
 #TODO# Undocumented (but would be very usefull) API : Access currently forbidden (403)
 
-# _POST_UPDATE_HOME_REQ  = _BASE_URL + "/api/updatehome"
+_POST_UPDATE_HOME_REQ  = _BASE_URL + "/api/updatehome"
 
 # For presence setting (POST BODY):
 # _PRES_BODY_REC_SET     = "home_id=%s&presence_settings[presence_record_%s]=%s"   # (HomeId, DetectionKind, DetectionSetup.index)
 _PRES_DETECTION_KIND   = ("humans", "animals", "vehicles", "movements")
 _PRES_DETECTION_SETUP  = ("ignore", "record", "record & notify")
 
 # _PRES_BODY_ALERT_TIME  = "home_id=%s&presence_settings[presence_notify_%s]=%s"   # (HomeID, "from"|"to", "hh:mm")
@@ -271,15 +271,15 @@
         self.getAuthToken = authData.accessToken
         postParams = {
                 "access_token" : self.getAuthToken
                 }
         resp = postRequest(_GETTHERMOSTATDATA_REQ, postParams)
         self.rawData = resp['body']['devices']
         if not self.rawData : raise NoDevice("No thermostat available")
-        self.thermostatData = filter_home_data(rawData, home)
+        self.thermostatData = filter_home_data(self.rawData, home)
         if not self.thermostatData : raise NoHome("No home %s found" % home)
         self.thermostatData['name'] = self.thermostatData['home_name']
         for m in self.thermostatData['modules']:
             m['name'] = m['module_name']
         self.defaultThermostat = self.thermostatData['home_name']
         self.defaultThermostatId = self.thermostatData['_id']
         self.defaultModule = self.thermostatData['modules'][0]
@@ -316,18 +316,18 @@
         self.rawData = resp['body']['devices']
         # Weather data
         if not self.rawData : raise NoDevice("No weather station in any homes")
         # Stations are no longer in the Netatmo API, keeping them for compatibility
         self.stations = { d['station_name'] : d for d in self.rawData }
         self.homes = { d['home_name'] : d["station_name"] for d in self.rawData }
         # Keeping the old behavior for default station name
-        if station and station not in self.stations: raise NoDevice("No station with name %s" % station)
-        self.default_station = station or list(self.stations.keys())[0]
         if home and home not in self.homes : raise NoHome("No home with name %s" % home)
         self.default_home = home or list(self.homes.keys())[0]
+        if station and station not in self.stations: raise NoDevice("No station with name %s" % station)
+        self.default_station = station or [v["station_name"] for k,v in self.stations.items() if v["home_name"] == self.default_home][0]
         self.modules = dict()
         self.default_station_data = self.stationByName(self.default_station)
         if 'modules' in self.default_station_data:
             for m in self.default_station_data['modules']:
                 self.modules[ m['_id'] ] = m
         # User data
         userData = resp['body']['user']
@@ -388,23 +388,23 @@
                     lastD[module['module_name']] = ds.copy()
                     lastD[module['module_name']]['When'] = lastD[module['module_name']].pop("time_utc") if 'time_utc' in lastD[module['module_name']] else time.time()
                     # For potential use, add battery and radio coverage information to module data if present
                     for i in ('battery_vp', 'battery_percent', 'rf_status') :
                         if i in module : lastD[module['module_name']][i] = module[i]
         return lastD
 
-    def checkNotUpdated(self, station=None, delay=3600):
-        res = self.lastData(station)
+    def checkNotUpdated(self, delay=3600):
+        res = self.lastData()
         ret = []
         for mn,v in res.items():
             if time.time()-v['When'] > delay : ret.append(mn)
         return ret if ret else None
 
-    def checkUpdated(self, station=None, delay=3600):
-        res = self.lastData(station)
+    def checkUpdated(self, delay=3600):
+        res = self.lastData()
         ret = []
         for mn,v in res.items():
             if time.time()-v['When'] < delay : ret.append(mn)
         return ret if ret else None
 
     def getMeasure(self, device_id, scale, mtype, module_id=None, date_begin=None, date_end=None, limit=None, optimize=False, real_time=False):
         postParams = { "access_token" : self.getAuthToken }
@@ -820,15 +820,15 @@
     if module == "*":
         result = dict()
         for m in lastD.keys():
             if time.time()-lastD[m]['When'] > 3600 : continue
             r = devList.MinMaxTH(module=m)
             result[m] = (r[0], lastD[m]['Temperature'], r[1])
     else:
-        if time.time()-lastD[mname]['When'] > 3600 : result = ["-", "-"]
+        if time.time()-lastD[module]['When'] > 3600 : result = ["-", "-"]
         else : 
             result = [lastD[module]['Temperature'], lastD[module]['Humidity']]
             result.extend(devList.MinMaxTH(module))
     return result
 
 
 # auto-test when executed directly
```

### Comparing `lnetatmo-2.0.0/setup.py` & `lnetatmo-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # python setup.py --dry-run --verbose install
 
 from distutils.core import setup
 
 setup(
     name='lnetatmo',
-    version='2.0.0',
+    version='2.1.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3'
         ],
     author='Philippe Larduinat',
     author_email='ph.larduinat@wanadoo.fr',
     py_modules=['lnetatmo'],
     scripts=[],
     data_files=[],
     url='https://github.com/philippelt/netatmo-api-python',
-    download_url='https://github.com/philippelt/netatmo-api-python/tarball/v2.0.0.tar.gz',
+    download_url='https://github.com/philippelt/netatmo-api-python/archive/v2.1.0.tar.gz',
     license='GPL V3',
     description='Simple API to access Netatmo weather station data from any python script.'
 )
```

