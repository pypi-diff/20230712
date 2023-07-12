# Comparing `tmp/pvcobrademo-1.2.3.tar.gz` & `tmp/pvcobrademo-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvcobrademo-1.2.3.tar", last modified: Wed Jun  7 21:45:13 2023, max compression
+gzip compressed data, was "pvcobrademo-1.2.4.tar", last modified: Wed Jul 12 18:41:38 2023, max compression
```

## Comparing `pvcobrademo-1.2.3.tar` & `pvcobrademo-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      105 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/MANIFEST.in
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6091 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5417 2023-06-07 20:46:18.000000 pvcobrademo-1.2.3/README.md
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/pvcobrademo/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/LICENSE
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2469 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/cobra_demo_file.py
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4556 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/cobra_demo_mic.py
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/pvcobrademo.egg-info/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6091 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      323 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/SOURCES.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/dependency_links.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/entry_points.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       33 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/requires.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       12 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/top_level.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/setup.cfg
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     1937 2023-06-07 21:44:56.000000 pvcobrademo-1.2.3/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:41:38.003010 pvcobrademo-1.2.4/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      105 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6054 2023-07-12 18:41:37.999010 pvcobrademo-1.2.4/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5417 2022-07-25 18:37:11.000000 pvcobrademo-1.2.4/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:41:37.999010 pvcobrademo-1.2.4/pvcobrademo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2469 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo/cobra_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4573 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo/cobra_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:41:37.999010 pvcobrademo-1.2.4/pvcobrademo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6054 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      323 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      118 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       33 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       12 2023-07-12 18:41:37.000000 pvcobrademo-1.2.4/pvcobrademo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 18:41:38.003010 pvcobrademo-1.2.4/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1937 2023-07-12 18:39:24.000000 pvcobrademo-1.2.4/setup.py
```

### Comparing `pvcobrademo-1.2.3/PKG-INFO` & `pvcobrademo-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvcobrademo
-Version: 1.2.3
+Version: 1.2.4
 Summary: Cobra voice activity detection (VAD) engine demos.
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: voice activity detection engine,VAD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -117,9 +115,7 @@
 
 ```console
 cobra_demo_file --access_key {AccessKey} --input_audio_path ${AUDIO_PATH} \
  --threshold 0.9
 ```
 
 Threshold is a floating point number within `[0, 1]`. A higher threshold reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvcobrademo-1.2.3/README.md` & `pvcobrademo-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.3/pvcobrademo/LICENSE` & `pvcobrademo-1.2.4/pvcobrademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.3/pvcobrademo/cobra_demo_file.py` & `pvcobrademo-1.2.4/pvcobrademo/cobra_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.3/pvcobrademo/cobra_demo_mic.py` & `pvcobrademo-1.2.4/pvcobrademo/cobra_demo_mic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021 Picovoice Inc.
+# Copyright 2021-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
@@ -57,15 +57,15 @@
         recorder = None
         wav_file = None
 
         try:
             cobra = pvcobra.create(
                 library_path=self._library_path, access_key=self._access_key)
             print("Cobra version: %s" % cobra.version)
-            recorder = PvRecorder(device_index=self._input_device_index, frame_length=512)
+            recorder = PvRecorder(frame_length=512, device_index=self._input_device_index)
             recorder.start()
 
             if self._output_path is not None:
                 wav_file = wave.open(self._output_path, "w")
                 wav_file.setparams((1, 2, 16000, 512, "NONE", "NONE"))
 
             print("Listening...")
@@ -92,16 +92,16 @@
             if wav_file is not None:
                 wav_file.close()
 
             if recorder is not None:
                 recorder.delete()
 
     @classmethod
-    def show_audio_devices(cls):
-        devices = PvRecorder.get_audio_devices()
+    def show_available_devices(cls):
+        devices = PvRecorder.get_available_devices()
         for i in range(len(devices)):
             print('index: %d, device name: %s' % (i, devices[i]))
 
 
 def main():
     parser = argparse.ArgumentParser()
 
@@ -119,15 +119,15 @@
         '--output_path', help='Absolute path to recorded audio for debugging.', default=None)
 
     parser.add_argument('--show_audio_devices', action='store_true')
 
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        CobraDemo.show_audio_devices()
+        CobraDemo.show_available_devices()
     else:
         if args.access_key is None:
             print("missing AccessKey")
         else:
             CobraDemo(
                 library_path=args.library_path,
                 access_key=args.access_key,
```

### Comparing `pvcobrademo-1.2.3/pvcobrademo.egg-info/PKG-INFO` & `pvcobrademo-1.2.4/pvcobrademo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvcobrademo
-Version: 1.2.3
+Version: 1.2.4
 Summary: Cobra voice activity detection (VAD) engine demos.
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: voice activity detection engine,VAD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -117,9 +115,7 @@
 
 ```console
 cobra_demo_file --access_key {AccessKey} --input_audio_path ${AUDIO_PATH} \
  --threshold 0.9
 ```
 
 Threshold is a floating point number within `[0, 1]`. A higher threshold reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvcobrademo-1.2.3/setup.py` & `pvcobrademo-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvcobrademo/cobra_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvcobrademo",
-    version="1.2.3",
+    version="1.2.4",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Cobra voice activity detection (VAD) engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/cobra",
     packages=["pvcobrademo"],
-    install_requires=["pvcobra==1.2.2", "pvrecorder==1.1.1"],
+    install_requires=["pvcobra==1.2.2", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

