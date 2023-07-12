# Comparing `tmp/mqtt-client-1.6.0.tar.gz` & `tmp/mqtt-client-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-client-1.6.0.tar", last modified: Thu Mar 31 11:21:17 2022, max compression
+gzip compressed data, was "mqtt-client-1.6.1.tar", last modified: Wed Jul 12 17:32:22 2023, max compression
```

## Comparing `mqtt-client-1.6.0.tar` & `mqtt-client-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2022-03-31 11:21:17.183372 mqtt-client-1.6.0/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3257 2022-03-31 11:21:17.183372 mqtt-client-1.6.0/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2962 2022-03-31 09:35:48.000000 mqtt-client-1.6.0/README.md
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2022-03-31 11:21:17.183372 mqtt-client-1.6.0/mqtt_client/
--rw-r--r--   0 samuel    (1000) samuel    (1000)        0 2019-11-08 10:04:20.000000 mqtt-client-1.6.0/mqtt_client/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5907 2022-03-31 09:32:28.000000 mqtt-client-1.6.0/mqtt_client/__main__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4796 2022-03-31 09:35:48.000000 mqtt-client-1.6.0/mqtt_client/mqtt_client.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      825 2022-03-31 09:32:57.000000 mqtt-client-1.6.0/mqtt_client/subscribe_callbacks.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2022-03-31 11:21:17.183372 mqtt-client-1.6.0/mqtt_client.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3257 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      340 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       59 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/entry_points.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       32 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/requires.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       12 2022-03-31 11:21:17.000000 mqtt-client-1.6.0/mqtt_client.egg-info/top_level.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       38 2022-03-31 11:21:17.183372 mqtt-client-1.6.0/setup.cfg
--rw-r--r--   0 samuel    (1000) samuel    (1000)      776 2022-03-31 09:32:28.000000 mqtt-client-1.6.0/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-12 17:32:22.074302 mqtt-client-1.6.1/
+-rw-r--r--   0 sam       (1000) sam       (1000)     3220 2023-07-12 17:32:22.073302 mqtt-client-1.6.1/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     2962 2023-07-12 17:29:42.000000 mqtt-client-1.6.1/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-12 17:32:22.072302 mqtt-client-1.6.1/mqtt_client/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-07-12 16:52:29.000000 mqtt-client-1.6.1/mqtt_client/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6133 2023-07-12 17:30:36.000000 mqtt-client-1.6.1/mqtt_client/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4865 2023-07-12 17:30:58.000000 mqtt-client-1.6.1/mqtt_client/mqtt_client.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      825 2023-07-12 16:52:29.000000 mqtt-client-1.6.1/mqtt_client/subscribe_callbacks.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-12 17:32:22.073302 mqtt-client-1.6.1/mqtt_client.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     3220 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      340 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       58 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       32 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       12 2023-07-12 17:32:22.000000 mqtt-client-1.6.1/mqtt_client.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       38 2023-07-12 17:32:22.074302 mqtt-client-1.6.1/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      776 2023-07-12 17:30:00.000000 mqtt-client-1.6.1/setup.py
```

### Comparing `mqtt-client-1.6.0/PKG-INFO` & `mqtt-client-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mqtt-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simple MQTT Client.
 Home-page: https://mqtt.clubpulp.com/
 Author: Samuel de Ancos
 Author-email: sdeancos@gmail.com
-License: UNKNOWN
 Keywords: mqtt
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # MQTT Client 
 
-ver: 1.6.0
+ver: 1.6.1
 
 [Documentation](https://mqtt.clubpulp.com/)
 
 [![Downloads](https://pepy.tech/badge/mqtt-client)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/month)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/week)](https://pepy.tech/project/mqtt-client)
 
 ## Install
 
@@ -93,9 +91,7 @@
   "cert_path": "",
   "qos": 0,
   "retain": false,
   "callback": "",
   "command": ""
 }
 ```
-
-
```

### Comparing `mqtt-client-1.6.0/README.md` & `mqtt-client-1.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MQTT Client 
 
-ver: 1.6.0
+ver: 1.6.1
 
 [Documentation](https://mqtt.clubpulp.com/)
 
 [![Downloads](https://pepy.tech/badge/mqtt-client)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/month)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/week)](https://pepy.tech/project/mqtt-client)
 
 ## Install
```

### Comparing `mqtt-client-1.6.0/mqtt_client/__main__.py` & `mqtt-client-1.6.1/mqtt_client/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 import readline
 import json
 
 from terminaltables import SingleTable
 
 from mqtt_client import mqtt_client
 
-NAME, VERSION = 'MQTT Client', '1.6.0'
-AUTHOR = 'Samuel de Ancos (2018-2022) <https://github.com/sdeancos/mqtt-client>'
+NAME, VERSION = 'MQTT Client', '1.6.1'
+AUTHOR = 'Samuel de Ancos (2018-2023) <https://github.com/sdeancos/mqtt-client>'
 
 
 def main():
     arguments = docopt(f'{NAME} {VERSION}\n{AUTHOR}\n\n{__doc__}', version=f'{NAME} {VERSION}')
 
     config = None
     if arguments['--config']:
@@ -138,22 +138,31 @@
             elif '--payload' in arguments:
                 payload = arguments['--payload']
             else:
                 exit(f'│ERROR│ Not payload defined')
 
             is_published = mqtt_client.publish(mqtt_handler=mqtt_handler, payload=payload, qos=qos, retain=retain)
         else:
+            mqtt_handler.loop_start()
+            exit_by = ''
             while True:
                 try:
                     payload = input('[insert payload] ? ')
                     is_published = mqtt_client.publish(mqtt_handler=mqtt_handler, payload=payload,
                                                        qos=qos, retain=retain)
                 except KeyboardInterrupt:
-                    exit('[CTRL+C] Exit')
+                    exit_by = '[CTRL+C] Exit'
+                    break
                 except EOFError:
-                    exit('[CTRL+D] Exit')
+                    exit_by = '[CTRL+D] Exit'
+                    break
+
+            mqtt_handler.loop_stop()
+
+            if exit_by is not '':
+                exit(exit_by)
 
     if arguments['subscribe']:
         mqtt_client.subscribe(mqtt_handler=mqtt_handler, callback=callback, command=command)
 
 if __name__ == '__main__':
     main()
```

### Comparing `mqtt-client-1.6.0/mqtt_client/mqtt_client.py` & `mqtt-client-1.6.1/mqtt_client/mqtt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
     def on_connect(self, mqttc, obj, flags, rc):
         if rc != 0:
             print('│ERROR│ from connect - rc: {}'.format(rc))
 
     def loop_start(self):
         self.client.loop_start()
 
+    def loop_stop(self):
+        self.client.loop_stop(force=False)
+
     def loop_forever(self):
         try:
             self.client.loop_forever()
         except KeyboardInterrupt:
             exit('│CTRL+C│ Exit by KeyboardInterrupt')
 
     def publish(self, payload, qos=0, retain=False):
```

### Comparing `mqtt-client-1.6.0/mqtt_client/subscribe_callbacks.py` & `mqtt-client-1.6.1/mqtt_client/subscribe_callbacks.py`

 * *Files identical despite different names*

### Comparing `mqtt-client-1.6.0/mqtt_client.egg-info/PKG-INFO` & `mqtt-client-1.6.1/mqtt_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mqtt-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simple MQTT Client.
 Home-page: https://mqtt.clubpulp.com/
 Author: Samuel de Ancos
 Author-email: sdeancos@gmail.com
-License: UNKNOWN
 Keywords: mqtt
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # MQTT Client 
 
-ver: 1.6.0
+ver: 1.6.1
 
 [Documentation](https://mqtt.clubpulp.com/)
 
 [![Downloads](https://pepy.tech/badge/mqtt-client)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/month)](https://pepy.tech/project/mqtt-client) [![Downloads](https://pepy.tech/badge/mqtt-client/week)](https://pepy.tech/project/mqtt-client)
 
 ## Install
 
@@ -93,9 +91,7 @@
   "cert_path": "",
   "qos": 0,
   "retain": false,
   "callback": "",
   "command": ""
 }
 ```
-
-
```

### Comparing `mqtt-client-1.6.0/setup.py` & `mqtt-client-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mqtt-client',
-    version='1.6.0',
+    version='1.6.1',
     description='Simple MQTT Client.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='mqtt',
     author='Samuel de Ancos',
     author_email='sdeancos@gmail.com',
     url='https://mqtt.clubpulp.com/',
```

