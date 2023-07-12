# Comparing `tmp/pvporcupinedemo-2.2.1.tar.gz` & `tmp/pvporcupinedemo-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvporcupinedemo-2.2.1.tar", last modified: Wed Jun  7 17:53:53 2023, max compression
+gzip compressed data, was "pvporcupinedemo-2.2.2.tar", last modified: Wed Jul 12 17:20:04 2023, max compression
```

## Comparing `pvporcupinedemo-2.2.1.tar` & `pvporcupinedemo-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      125 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/MANIFEST.in
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6497 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5782 2023-06-07 17:44:48.000000 pvporcupinedemo-2.2.1/README.md
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/pvporcupinedemo/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/LICENSE
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5453 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_file.py
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5572 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_mic.py
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6497 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      367 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      143 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/entry_points.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       37 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/requires.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       16 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/top_level.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 17:53:53.110758 pvporcupinedemo-2.2.1/setup.cfg
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2053 2023-06-07 17:53:21.000000 pvporcupinedemo-2.2.1/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 17:20:04.310292 pvporcupinedemo-2.2.2/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      125 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6460 2023-07-12 17:20:04.310292 pvporcupinedemo-2.2.2/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5782 2023-04-19 17:19:30.000000 pvporcupinedemo-2.2.2/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 17:20:04.310292 pvporcupinedemo-2.2.2/pvporcupinedemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5453 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo/porcupine_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5553 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo/porcupine_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 17:20:04.310292 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6460 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      367 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      142 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       37 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       16 2023-07-12 17:20:04.000000 pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 17:20:04.310292 pvporcupinedemo-2.2.2/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2053 2023-07-12 17:17:00.000000 pvporcupinedemo-2.2.2/setup.py
```

### Comparing `pvporcupinedemo-2.2.1/PKG-INFO` & `pvporcupinedemo-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -171,9 +169,7 @@
 porcupine_demo_file --access_key ${ACCESS_KEY} \
 --wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvporcupinedemo-2.2.1/README.md` & `pvporcupinedemo-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.1/pvporcupinedemo/LICENSE` & `pvporcupinedemo-2.2.2/pvporcupinedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_file.py` & `pvporcupinedemo-2.2.2/pvporcupinedemo/porcupine_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_mic.py` & `pvporcupinedemo-2.2.2/pvporcupinedemo/porcupine_demo_mic.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         '--access_key',
-        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-        required=True)
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
 
     parser.add_argument(
         '--keywords',
         nargs='+',
         help='List of default keywords for detection. Available keywords: %s' % ', '.join(
             '%s' % w for w in sorted(pvporcupine.KEYWORDS)),
         choices=sorted(pvporcupine.KEYWORDS),
@@ -63,15 +62,15 @@
     parser.add_argument('--output_path', help='Absolute path to recorded audio for debugging.', default=None)
 
     parser.add_argument('--show_audio_devices', action='store_true')
 
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        for i, device in enumerate(PvRecorder.get_audio_devices()):
+        for i, device in enumerate(PvRecorder.get_available_devices()):
             print('Device %d: %s' % (i, device))
         return
 
     if args.keyword_paths is None:
         if args.keywords is None:
             raise ValueError("Either `--keywords` or `--keyword_paths` must be set.")
 
@@ -119,16 +118,16 @@
             keywords.append(' '.join(keyword_phrase_part[0:-6]))
         else:
             keywords.append(keyword_phrase_part[0])
 
     print('Porcupine version: %s' % porcupine.version)
 
     recorder = PvRecorder(
-        device_index=args.audio_device_index,
-        frame_length=porcupine.frame_length)
+        frame_length=porcupine.frame_length,
+        device_index=args.audio_device_index)
     recorder.start()
 
     wav_file = None
     if args.output_path is not None:
         wav_file = wave.open(args.output_path, "w")
         wav_file.setnchannels(1)
         wav_file.setsampwidth(2)
```

### Comparing `pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/PKG-INFO` & `pvporcupinedemo-2.2.2/pvporcupinedemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -171,9 +169,7 @@
 porcupine_demo_file --access_key ${ACCESS_KEY} \
 --wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvporcupinedemo-2.2.1/setup.py` & `pvporcupinedemo-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvporcupinedemo/porcupine_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvporcupinedemo",
-    version="2.2.1",
+    version="2.2.2",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Porcupine wake word engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/porcupine",
     packages=["pvporcupinedemo"],
-    install_requires=["pvporcupine==2.2.1", "pvrecorder==1.1.1"],
+    install_requires=["pvporcupine==2.2.1", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

