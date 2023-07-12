# Comparing `tmp/pveagledemo-0.1.0.tar.gz` & `tmp/pveagledemo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pveagledemo-0.1.0.tar", last modified: Mon May 29 20:16:28 2023, max compression
+gzip compressed data, was "pveagledemo-0.1.1.tar", last modified: Wed Jul 12 19:09:34 2023, max compression
```

## Comparing `pveagledemo-0.1.0.tar` & `pveagledemo-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-05-29 20:16:28.106507 pveagledemo-0.1.0/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      105 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5805 2023-05-29 20:16:28.106507 pveagledemo-0.1.0/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5146 2023-05-29 20:07:04.000000 pveagledemo-0.1.0/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-05-29 20:16:28.106507 pveagledemo-0.1.0/pveagledemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11357 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     8417 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo/eagle_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     9603 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo/eagle_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-05-29 20:16:28.106507 pveagledemo-0.1.0/pveagledemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5805 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      323 2023-05-29 20:16:28.000000 pveagledemo-0.1.0/pveagledemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      118 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       33 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       12 2023-05-29 20:16:27.000000 pveagledemo-0.1.0/pveagledemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-05-29 20:16:28.106507 pveagledemo-0.1.0/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1756 2023-05-29 20:07:04.000000 pveagledemo-0.1.0/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:09:34.159590 pveagledemo-0.1.1/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      105 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5805 2023-07-12 19:09:34.159590 pveagledemo-0.1.1/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5146 2023-07-12 19:02:32.000000 pveagledemo-0.1.1/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:09:34.159590 pveagledemo-0.1.1/pveagledemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11357 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     8417 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo/eagle_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     9607 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo/eagle_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 19:09:34.159590 pveagledemo-0.1.1/pveagledemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5805 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      323 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      118 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       33 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       12 2023-07-12 19:09:34.000000 pveagledemo-0.1.1/pveagledemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 19:09:34.159590 pveagledemo-0.1.1/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1756 2023-07-12 19:02:50.000000 pveagledemo-0.1.1/setup.py
```

### Comparing `pveagledemo-0.1.0/PKG-INFO` & `pveagledemo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pveagledemo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eagle Speaker Recognition Engine demos
 Home-page: https://github.com/Picovoice/eagle
 Author: Picovoice
 Author-email: hello@picovoice.ai
 Keywords: Speaker Recognition,Speaker Identification,Voice Recognition,Voice Identification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pveagledemo-0.1.0/README.md` & `pveagledemo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pveagledemo-0.1.0/pveagledemo/LICENSE` & `pveagledemo-0.1.1/pveagledemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pveagledemo-0.1.0/pveagledemo/eagle_demo_file.py` & `pveagledemo-0.1.1/pveagledemo/eagle_demo_file.py`

 * *Files identical despite different names*

### Comparing `pveagledemo-0.1.0/pveagledemo/eagle_demo_mic.py` & `pveagledemo-0.1.1/pveagledemo/eagle_demo_mic.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         required=True,
         nargs='+',
         help='Absolute path(s) to speaker profile(s)')
 
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        for index, name in enumerate(PvRecorder.get_audio_devices()):
+        for index, name in enumerate(PvRecorder.get_available_devices()):
             print('Device #%d: %s' % (index, name))
         return
 
     if args.command == 'enroll':
         try:
             eagle_profiler = pveagle.create_profiler(
                 access_key=args.access_key,
@@ -142,15 +142,15 @@
             print("If all other arguments seem valid, ensure that '%s' is a valid AccessKey" % args.access_key)
             raise
         except pveagle.EagleError as e:
             print("Failed to initialize Eagle: %s" % e)
             raise
 
         print('Eagle version: %s' % eagle_profiler.version)
-        recorder = PvRecorder(device_index=args.audio_device_index, frame_length=PV_RECORDER_FRAME_LENGTH)
+        recorder = PvRecorder(frame_length=PV_RECORDER_FRAME_LENGTH, device_index=args.audio_device_index)
         print("Recording audio from '%s'" % recorder.selected_device)
         num_enroll_frames = eagle_profiler.min_enroll_samples // PV_RECORDER_FRAME_LENGTH
         sample_rate = eagle_profiler.sample_rate
         enrollment_animation = EnrollmentAnimation()
         print('Please keep speaking until the enrollment percentage reaches 100%')
         try:
             with contextlib.ExitStack() as file_stack:
```

### Comparing `pveagledemo-0.1.0/pveagledemo.egg-info/PKG-INFO` & `pveagledemo-0.1.1/pveagledemo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pveagledemo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eagle Speaker Recognition Engine demos
 Home-page: https://github.com/Picovoice/eagle
 Author: Picovoice
 Author-email: hello@picovoice.ai
 Keywords: Speaker Recognition,Speaker Identification,Voice Recognition,Voice Identification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pveagledemo-0.1.0/setup.py` & `pveagledemo-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     f.write(manifest_in)
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pveagledemo",
-    version="0.1.0",
+    version="0.1.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Eagle Speaker Recognition Engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/eagle",
     packages=["pveagledemo"],
-    install_requires=["pveagle==0.1.0", "pvrecorder==1.1.1"],
+    install_requires=["pveagle==0.1.0", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

