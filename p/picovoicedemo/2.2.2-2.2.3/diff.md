# Comparing `tmp/picovoicedemo-2.2.2.tar.gz` & `tmp/picovoicedemo-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoicedemo-2.2.2.tar", last modified: Wed Jun  7 21:32:04 2023, max compression
+gzip compressed data, was "picovoicedemo-2.2.3.tar", last modified: Wed Jul 12 18:34:48 2023, max compression
```

## Comparing `picovoicedemo-2.2.2.tar` & `picovoicedemo-2.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/MANIFEST.in
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4943 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4236 2023-06-07 20:45:36.000000 picovoicedemo-2.2.2/README.md
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/picovoicedemo/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/LICENSE
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6568 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_file.py
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6876 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_mic.py
-drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/picovoicedemo.egg-info/
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4943 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/PKG-INFO
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      349 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      139 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/entry_points.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       35 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/requires.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       14 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/top_level.txt
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/setup.cfg
--rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2537 2023-06-07 21:31:44.000000 picovoicedemo-2.2.2/setup.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:34:48.047424 picovoicedemo-2.2.3/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      119 2023-07-12 18:34:47.000000 picovoicedemo-2.2.3/MANIFEST.in
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4906 2023-07-12 18:34:48.043424 picovoicedemo-2.2.3/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4236 2023-04-19 17:30:10.000000 picovoicedemo-2.2.3/README.md
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:34:48.043424 picovoicedemo-2.2.3/picovoicedemo/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2023-07-12 18:34:47.000000 picovoicedemo-2.2.3/picovoicedemo/LICENSE
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6568 2023-07-12 18:34:47.000000 picovoicedemo-2.2.3/picovoicedemo/picovoice_demo_file.py
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6984 2023-07-12 18:34:47.000000 picovoicedemo-2.2.3/picovoicedemo/picovoice_demo_mic.py
+drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2023-07-12 18:34:48.043424 picovoicedemo-2.2.3/picovoicedemo.egg-info/
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4906 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      349 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      138 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       35 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/requires.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       14 2023-07-12 18:34:48.000000 picovoicedemo-2.2.3/picovoicedemo.egg-info/top_level.txt
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2023-07-12 18:34:48.047424 picovoicedemo-2.2.3/setup.cfg
+-rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2537 2023-07-12 18:31:15.000000 picovoicedemo-2.2.3/setup.py
```

### Comparing `picovoicedemo-2.2.2/PKG-INFO` & `picovoicedemo-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.2
+Version: 2.2.3
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -119,9 +117,7 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
-
-
```

### Comparing `picovoicedemo-2.2.2/README.md` & `picovoicedemo-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.2/picovoicedemo/LICENSE` & `picovoicedemo-2.2.3/picovoicedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_file.py` & `picovoicedemo-2.2.3/picovoicedemo/picovoice_demo_file.py`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_mic.py` & `picovoicedemo-2.2.3/picovoicedemo/picovoice_demo_mic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 Picovoice Inc.
+# Copyright 2020-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
@@ -18,26 +18,23 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         '--access_key',
-        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-        required=True)
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
 
     parser.add_argument(
         '--keyword_path',
-        help="Absolute path to a Porcupine keyword file.",
-        required=True)
+        help="Absolute path to a Porcupine keyword file.")
 
     parser.add_argument(
         '--context_path',
-        help="Absolute path to a Rhino context file.",
-        required=True)
+        help="Absolute path to a Rhino context file.")
 
     parser.add_argument(
         '--porcupine_library_path',
         help="Absolute path to Porcupine's dynamic library.")
 
     parser.add_argument(
         '--porcupine_model_path',
@@ -93,18 +90,22 @@
 
     if args.require_endpoint.lower() == 'false':
         require_endpoint = False
     else:
         require_endpoint = True
 
     if args.show_audio_devices:
-        for i, device in enumerate(PvRecorder.get_audio_devices()):
+        for i, device in enumerate(PvRecorder.get_available_devices()):
             print('Device %d: %s' % (i, device))
         return
 
+    if not args.access_key or not args.keyword_path or not args.context_path:
+        print('--access_key, --keyword_path and --context_path are required.')
+        return
+
     def wake_word_callback():
         print('[wake word]\n')
 
     def inference_callback(inference):
         if inference.is_understood:
             print('{')
             print("  intent : '%s'" % inference.intent)
@@ -151,16 +152,16 @@
         print("Failed to initialize Picovoice")
         raise e
 
     print('Picovoice version: %s' % picovoice.version)
     print('Context info: %s' % picovoice.context_info)
 
     recorder = PvRecorder(
-        device_index=args.audio_device_index,
         frame_length=picovoice.frame_length,
+        device_index=args.audio_device_index,
     )
     recorder.start()
 
     print('Listening ... (Press Ctrl+C to exit)\n')
 
     wav_file = None
     if args.output_path is not None:
```

### Comparing `picovoicedemo-2.2.2/picovoicedemo.egg-info/PKG-INFO` & `picovoicedemo-2.2.3/picovoicedemo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.2
+Version: 2.2.3
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -119,9 +117,7 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
-
-
```

### Comparing `picovoicedemo-2.2.2/setup.py` & `picovoicedemo-2.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2021 Picovoice Inc.
+# Copyright 2020-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
@@ -35,23 +35,23 @@
     f.write('include picovoicedemo/picovoice_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoicedemo",
-    version="2.2.2",
+    version="2.2.3",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoicedemo"],
-    install_requires=["picovoice==2.2.1", "pvrecorder==1.1.1"],
+    install_requires=["picovoice==2.2.1", "pvrecorder==1.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

