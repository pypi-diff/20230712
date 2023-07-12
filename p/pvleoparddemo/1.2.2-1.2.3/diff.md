# Comparing `tmp/pvleoparddemo-1.2.2.tar.gz` & `tmp/pvleoparddemo-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvleoparddemo-1.2.2.tar", last modified: Tue Apr 11 00:49:19 2023, max compression
+gzip compressed data, was "pvleoparddemo-1.2.3.tar", last modified: Wed Jul 12 18:54:15 2023, max compression
```

## Comparing `pvleoparddemo-1.2.2.tar` & `pvleoparddemo-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:19.625513 pvleoparddemo-1.2.2/
--rw-rw-r--   0 eric      (1000) eric      (1000)      115 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/MANIFEST.in
--rw-rw-r--   0 eric      (1000) eric      (1000)     2621 2023-04-11 00:49:19.625513 pvleoparddemo-1.2.2/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1909 2022-08-18 00:29:33.000000 pvleoparddemo-1.2.2/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:19.625513 pvleoparddemo-1.2.2/pvleoparddemo/
--rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)     2267 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo/leopard_demo_file.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4277 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo/leopard_demo_mic.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:19.625513 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     2621 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      345 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      131 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       52 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-04-11 00:49:19.000000 pvleoparddemo-1.2.2/pvleoparddemo.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:49:19.625513 pvleoparddemo-1.2.2/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)     2034 2023-04-11 00:48:47.000000 pvleoparddemo-1.2.2/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:54:15.476517 pvleoparddemo-1.2.3/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      115 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2585 2023-07-12 18:54:15.476517 pvleoparddemo-1.2.3/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1909 2022-08-15 19:00:11.000000 pvleoparddemo-1.2.3/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:54:15.476517 pvleoparddemo-1.2.3/pvleoparddemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2267 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo/leopard_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4349 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo/leopard_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:54:15.476517 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2585 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      345 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      130 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       52 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       14 2023-07-12 18:54:15.000000 pvleoparddemo-1.2.3/pvleoparddemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 18:54:15.476517 pvleoparddemo-1.2.3/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2034 2023-07-12 18:51:44.000000 pvleoparddemo-1.2.3/setup.py
```

### Comparing `pvleoparddemo-1.2.2/PKG-INFO` & `pvleoparddemo-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvleoparddemo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Leopard speech-to-text engine demos
 Home-page: https://github.com/Picovoice/leopard
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Text,ASR,Speech Recognition,Voice Recognition,Automatic Speech Recognition
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -81,8 +79,7 @@
 Press `ENTER` key and wait for the following message in the terminal:
 
 ```console
 >>> Recording ... Press `ENTER` to stop:
 ```
 
 Now start recording and when done press `ENTER` key to get the transcription.
-
```

### Comparing `pvleoparddemo-1.2.2/README.md` & `pvleoparddemo-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pvleoparddemo-1.2.2/pvleoparddemo/LICENSE` & `pvleoparddemo-1.2.3/pvleoparddemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvleoparddemo-1.2.2/pvleoparddemo/leopard_demo_file.py` & `pvleoparddemo-1.2.3/pvleoparddemo/leopard_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvleoparddemo-1.2.2/pvleoparddemo/leopard_demo_mic.py` & `pvleoparddemo-1.2.3/pvleoparddemo/leopard_demo_mic.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def is_recording(self):
         return self._is_recording
 
     def run(self):
         self._is_recording = True
 
-        recorder = PvRecorder(device_index=self._audio_device_index, frame_length=160)
+        recorder = PvRecorder(frame_length=160, device_index=self._audio_device_index)
         recorder.start()
 
         while not self._stop:
             self._pcm.extend(recorder.read())
         recorder.stop()
 
         self._is_recording = False
@@ -51,16 +51,15 @@
         return self._pcm
 
 
 def main():
     parser = ArgumentParser()
     parser.add_argument(
         '--access_key',
-        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-        required=True)
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
     parser.add_argument(
         '--library_path',
         help='Absolute path to dynamic library. Default: using the library provided by `pvleopard`')
     parser.add_argument(
         '--model_path',
         help='Absolute path to Leopard model. Default: using the model provided by `pvleopard`')
     parser.add_argument(
@@ -79,24 +78,28 @@
         '--audio_device_index',
         default=-1,
         type=int,
         help='Audio device index to use from --show_audio_devices')
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        for index, name in enumerate(PvRecorder.get_audio_devices()):
+        for index, name in enumerate(PvRecorder.get_available_devices()):
             print('Device #%d: %s' % (index, name))
         return
 
     if args.audio_device_index != -1:
-        devices_length = len(PvRecorder.get_audio_devices())
+        devices_length = len(PvRecorder.get_available_devices())
         if args.audio_device_index < 0 or args.audio_device_index >= devices_length:
             print('Invalid audio device index provided.')
             sys.exit(1)
 
+    if not args.access_key:
+        print('--access_key is required.')
+        return
+
     leopard = create(
         access_key=args.access_key,
         model_path=args.model_path,
         library_path=args.library_path,
         enable_automatic_punctuation=not args.disable_automatic_punctuation)
 
     recorder = None
```

### Comparing `pvleoparddemo-1.2.2/pvleoparddemo.egg-info/PKG-INFO` & `pvleoparddemo-1.2.3/pvleoparddemo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvleoparddemo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Leopard speech-to-text engine demos
 Home-page: https://github.com/Picovoice/leopard
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Text,ASR,Speech Recognition,Voice Recognition,Automatic Speech Recognition
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -81,8 +79,7 @@
 Press `ENTER` key and wait for the following message in the terminal:
 
 ```console
 >>> Recording ... Press `ENTER` to stop:
 ```
 
 Now start recording and when done press `ENTER` key to get the transcription.
-
```

### Comparing `pvleoparddemo-1.2.2/setup.py` & `pvleoparddemo-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvleoparddemo/leopard_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvleoparddemo",
-    version="1.2.2",
+    version="1.2.3",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Leopard speech-to-text engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/leopard",
     packages=["pvleoparddemo"],
-    install_requires=["pvleopard==1.2.2", "pvrecorder==1.1.1", "tabulate==0.8.10"],
+    install_requires=["pvleopard==1.2.2", "pvrecorder==1.2.0", "tabulate==0.8.10"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

