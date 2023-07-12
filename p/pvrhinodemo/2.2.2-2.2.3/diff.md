# Comparing `tmp/pvrhinodemo-2.2.2.tar.gz` & `tmp/pvrhinodemo-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvrhinodemo-2.2.2.tar", last modified: Wed Jun  7 20:59:02 2023, max compression
+gzip compressed data, was "pvrhinodemo-2.2.3.tar", last modified: Wed Jul 12 18:21:54 2023, max compression
```

## Comparing `pvrhinodemo-2.2.2.tar` & `pvrhinodemo-2.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      102 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/MANIFEST.in
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4079 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     3359 2023-06-07 20:37:59.000000 pvrhinodemo-2.2.2/README.md
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/pvrhinodemo/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5697 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_file.py
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6010 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_mic.py
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4079 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      303 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/entry_points.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       33 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/requires.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       12 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/top_level.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/setup.cfg
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     1979 2023-06-07 20:58:47.000000 pvrhinodemo-2.2.2/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:21:54.026464 pvrhinodemo-2.2.3/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      102 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4042 2023-07-12 18:21:54.026464 pvrhinodemo-2.2.3/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     3359 2023-05-10 20:35:02.000000 pvrhinodemo-2.2.3/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:21:54.026464 pvrhinodemo-2.2.3/pvrhinodemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5697 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo/rhino_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6100 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo/rhino_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:21:54.026464 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4042 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      303 2023-07-12 18:21:54.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      118 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       33 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       12 2023-07-12 18:21:53.000000 pvrhinodemo-2.2.3/pvrhinodemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 18:21:54.026464 pvrhinodemo-2.2.3/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1979 2023-07-12 18:17:36.000000 pvrhinodemo-2.2.3/setup.py
```

### Comparing `pvrhinodemo-2.2.2/PKG-INFO` & `pvrhinodemo-2.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.2
+Version: 2.2.3
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -111,9 +109,7 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
-
-
```

### Comparing `pvrhinodemo-2.2.2/README.md` & `pvrhinodemo-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_file.py` & `pvrhinodemo-2.2.3/pvrhinodemo/rhino_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_mic.py` & `pvrhinodemo-2.2.3/pvrhinodemo/rhino_demo_mic.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,19 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         '--access_key',
-        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-        required=True)
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
 
     parser.add_argument(
         '--context_path',
-        help="Absolute path to context file.",
-        required=True)
+        help="Absolute path to context file.")
 
     parser.add_argument(
         '--library_path',
         help='Absolute path to dynamic library. Default: using the library provided by `pvrhino`')
 
     parser.add_argument(
         '--model_path',
@@ -73,18 +71,22 @@
 
     if args.require_endpoint.lower() == 'false':
         require_endpoint = False
     else:
         require_endpoint = True
 
     if args.show_audio_devices:
-        for i, device in enumerate(PvRecorder.get_audio_devices()):
+        for i, device in enumerate(PvRecorder.get_available_devices()):
             print('Device %d: %s' % (i, device))
         return
 
+    if not args.access_key or not args.context_path:
+        print('--access_key and --context_path are required.')
+        return
+
     try:
         rhino = pvrhino.create(
             access_key=args.access_key,
             library_path=args.library_path,
             model_path=args.model_path,
             context_path=args.context_path,
             sensitivity=args.sensitivity,
@@ -110,16 +112,16 @@
         print("Failed to initialize Rhino")
         raise e
 
     print('Rhino version: %s' % rhino.version)
     print('Context info: %s' % rhino.context_info)
 
     recorder = PvRecorder(
-        device_index=args.audio_device_index,
-        frame_length=rhino.frame_length)
+        frame_length=rhino.frame_length,
+        device_index=args.audio_device_index)
     recorder.start()
 
     print('Using device: %s' % recorder.selected_device)
     print('Listening ... Press Ctrl+C to exit.\n')
 
     wav_file = None
     if args.output_path is not None:
```

### Comparing `pvrhinodemo-2.2.2/pvrhinodemo.egg-info/PKG-INFO` & `pvrhinodemo-2.2.3/pvrhinodemo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.2
+Version: 2.2.3
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -111,9 +109,7 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
-
-
```

### Comparing `pvrhinodemo-2.2.2/setup.py` & `pvrhinodemo-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvrhinodemo/rhino_demo_mic.py')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvrhinodemo",
-    version="2.2.2",
+    version="2.2.3",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Rhino Speech-to-Intent engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/rhino",
     packages=["pvrhinodemo"],
-    install_requires=["pvrhino==2.2.2", "pvrecorder==1.1.1"],
+    install_requires=["pvrhino==2.2.2", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

