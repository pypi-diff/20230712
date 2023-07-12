# Comparing `tmp/pvcheetahdemo-1.1.4.tar.gz` & `tmp/pvcheetahdemo-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvcheetahdemo-1.1.4.tar", last modified: Tue Apr 11 00:49:17 2023, max compression
+gzip compressed data, was "pvcheetahdemo-1.1.5.tar", last modified: Wed Jul 12 19:00:09 2023, max compression
```

## Comparing `pvcheetahdemo-1.1.4.tar` & `pvcheetahdemo-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/
--rw-rw-r--   0 eric      (1000) eric      (1000)      115 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/MANIFEST.in
--rw-rw-r--   0 eric      (1000) eric      (1000)     2399 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1687 2022-08-18 00:29:46.000000 pvcheetahdemo-1.1.4/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/pvcheetahdemo/
--rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)     3023 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_file.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2931 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_mic.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     2399 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      345 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      131 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       35 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)     2014 2023-04-11 00:48:37.000000 pvcheetahdemo-1.1.4/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:00:09.401795 pvcheetahdemo-1.1.5/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      115 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2362 2023-07-12 19:00:09.401795 pvcheetahdemo-1.1.5/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1687 2022-12-21 19:08:54.000000 pvcheetahdemo-1.1.5/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:00:09.401795 pvcheetahdemo-1.1.5/pvcheetahdemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     3023 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo/cheetah_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     3047 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo/cheetah_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:00:09.401795 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2362 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      345 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      130 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       35 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       14 2023-07-12 19:00:09.000000 pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 19:00:09.401795 pvcheetahdemo-1.1.5/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2014 2023-07-12 18:58:34.000000 pvcheetahdemo-1.1.5/setup.py
```

### Comparing `pvcheetahdemo-1.1.4/PKG-INFO` & `pvcheetahdemo-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvcheetahdemo
-Version: 1.1.4
+Version: 1.1.5
 Summary: Cheetah speech-to-text engine demos
 Home-page: https://github.com/Picovoice/cheetah
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
@@ -69,9 +67,7 @@
 
 ```console
 cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
 ```
 
 Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
 (single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
-
-
```

### Comparing `pvcheetahdemo-1.1.4/README.md` & `pvcheetahdemo-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.4/pvcheetahdemo/LICENSE` & `pvcheetahdemo-1.1.5/pvcheetahdemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_file.py` & `pvcheetahdemo-1.1.5/pvcheetahdemo/cheetah_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_mic.py` & `pvcheetahdemo-1.1.5/pvcheetahdemo/cheetah_demo_mic.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,33 @@
         action='store_true',
         help='Disable insertion of automatic punctuation')
     parser.add_argument('--audio_device_index', type=int, default=-1, help='Index of input audio device')
     parser.add_argument('--show_audio_devices', action='store_true', help='Only list available devices and exit')
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        for index, name in enumerate(PvRecorder.get_audio_devices()):
+        for index, name in enumerate(PvRecorder.get_available_devices()):
             print('Device #%d: %s' % (index, name))
         return
+    
+    if not args.access_key:
+        print('--access_key is required.')
+        return
 
     cheetah = create(
         access_key=args.access_key,
         library_path=args.library_path,
         model_path=args.model_path,
         endpoint_duration_sec=args.endpoint_duration_sec,
         enable_automatic_punctuation=not args.disable_automatic_punctuation)
 
     try:
         print('Cheetah version : %s' % cheetah.version)
 
-        recorder = PvRecorder(device_index=-1, frame_length=cheetah.frame_length)
+        recorder = PvRecorder(frame_length=cheetah.frame_length, device_index=args.audio_device_index)
         recorder.start()
         print('Listening... (press Ctrl+C to stop)')
 
         try:
             while True:
                 partial_transcript, is_endpoint = cheetah.process(recorder.read())
                 print(partial_transcript, end='', flush=True)
```

### Comparing `pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/PKG-INFO` & `pvcheetahdemo-1.1.5/pvcheetahdemo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvcheetahdemo
-Version: 1.1.4
+Version: 1.1.5
 Summary: Cheetah speech-to-text engine demos
 Home-page: https://github.com/Picovoice/cheetah
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
@@ -69,9 +67,7 @@
 
 ```console
 cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
 ```
 
 Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
 (single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
-
-
```

### Comparing `pvcheetahdemo-1.1.4/setup.py` & `pvcheetahdemo-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvcheetahdemo/cheetah_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvcheetahdemo",
-    version="1.1.4",
+    version="1.1.5",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Cheetah speech-to-text engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/cheetah",
     packages=["pvcheetahdemo"],
-    install_requires=["pvcheetah==1.1.3", "pvrecorder==1.1.1"],
+    install_requires=["pvcheetah==1.1.3", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

