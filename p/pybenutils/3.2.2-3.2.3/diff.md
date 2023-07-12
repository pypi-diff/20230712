# Comparing `tmp/pybenutils-3.2.2.tar.gz` & `tmp/pybenutils-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybenutils-3.2.2.tar", last modified: Thu Jul  6 12:21:00 2023, max compression
+gzip compressed data, was "pybenutils-3.2.3.tar", last modified: Wed Jul 12 12:48:40 2023, max compression
```

## Comparing `pybenutils-3.2.2.tar` & `pybenutils-3.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.955077 pybenutils-3.2.2/
--rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.2.2/LICENSE
--rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4061 2023-07-06 12:21:00.955077 pybenutils-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.2.2/README.md
--rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.2.2/deploy_requirements.txt
--rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.2.2/deployment_checklist.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.861329 pybenutils-3.2.2/pybenutils/
--rw-rw-rw-   0        0        0      153 2023-07-06 12:12:38.000000 pybenutils-3.2.2/pybenutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.881276 pybenutils-3.2.2/pybenutils/amazon_boto3/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/amazon_boto3/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/amazon_boto3/amazon_obj.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.889255 pybenutils-3.2.2/pybenutils/autogui/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/__main__.py
--rw-rw-rw-   0        0        0     5874 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/auto_gui_cls.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.910197 pybenutils-3.2.2/pybenutils/browsers/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/chrome.py
--rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/firefox.py
--rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/selenium_utils.py
--rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/simple_browser_controller_cls.py
--rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/web_driver.py
--rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/windows_browsers_keywords.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.926155 pybenutils-3.2.2/pybenutils/network/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/download_manager.py
--rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/http_cert_info.py
--rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/s3_bucket_cls.py
--rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/ssh_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.946102 pybenutils-3.2.2/pybenutils/os_operations/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/__init__.py
--rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/files_and_directories.py
--rw-rw-rw-   0        0        0    18745 2023-07-06 12:12:38.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_application_control.py
--rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_input_control.py
--rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_operations.py
--rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_popup_handler.py
--rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/window_operations.py
--rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/useful.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.950091 pybenutils-3.2.2/pybenutils/utils_logger/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/utils_logger/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/utils_logger/config_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.876289 pybenutils-3.2.2/pybenutils.egg-info/
--rw-rw-rw-   0        0        0     4061 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.2.2/requirements.txt
--rw-rw-rw-   0        0        0      243 2023-07-06 12:21:00.957073 pybenutils-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1965 2023-07-06 12:04:25.000000 pybenutils-3.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.953083 pybenutils-3.2.2/tests/
--rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.2.2/tests/test_self_import.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.362550 pybenutils-3.2.3/
+-rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.2.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4061 2023-07-12 12:48:40.362550 pybenutils-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.2.3/README.md
+-rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.2.3/deploy_requirements.txt
+-rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.2.3/deployment_checklist.md
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.302710 pybenutils-3.2.3/pybenutils/
+-rw-rw-rw-   0        0        0      153 2023-07-12 12:33:03.000000 pybenutils-3.2.3/pybenutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.313681 pybenutils-3.2.3/pybenutils/amazon_boto3/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/amazon_boto3/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/amazon_boto3/amazon_obj.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.320662 pybenutils-3.2.3/pybenutils/autogui/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/autogui/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/autogui/__main__.py
+-rw-rw-rw-   0        0        0     6044 2023-07-12 12:33:03.000000 pybenutils-3.2.3/pybenutils/autogui/auto_gui_cls.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.331632 pybenutils-3.2.3/pybenutils/browsers/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/chrome.py
+-rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/firefox.py
+-rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/selenium_utils.py
+-rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/simple_browser_controller_cls.py
+-rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/web_driver.py
+-rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/windows_browsers_keywords.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.339611 pybenutils-3.2.3/pybenutils/network/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/download_manager.py
+-rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/http_cert_info.py
+-rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/s3_bucket_cls.py
+-rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/ssh_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.354571 pybenutils-3.2.3/pybenutils/os_operations/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/__init__.py
+-rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/files_and_directories.py
+-rw-rw-rw-   0        0        0    18745 2023-07-06 12:12:38.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_application_control.py
+-rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_input_control.py
+-rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_operations.py
+-rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_popup_handler.py
+-rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/window_operations.py
+-rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/useful.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.358561 pybenutils-3.2.3/pybenutils/utils_logger/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/utils_logger/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/utils_logger/config_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.310689 pybenutils-3.2.3/pybenutils.egg-info/
+-rw-rw-rw-   0        0        0     4061 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.2.3/requirements.txt
+-rw-rw-rw-   0        0        0      243 2023-07-12 12:48:40.364544 pybenutils-3.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1965 2023-07-06 12:04:25.000000 pybenutils-3.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.360556 pybenutils-3.2.3/tests/
+-rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.2.3/tests/test_self_import.py
```

### Comparing `pybenutils-3.2.2/LICENSE` & `pybenutils-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/PKG-INFO` & `pybenutils-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.2.2
+Version: 3.2.3
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pybenutils-3.2.2/README.md` & `pybenutils-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/deployment_checklist.md` & `pybenutils-3.2.3/deployment_checklist.md`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/amazon_boto3/amazon_obj.py` & `pybenutils-3.2.3/pybenutils/amazon_boto3/amazon_obj.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/autogui/__main__.py` & `pybenutils-3.2.3/pybenutils/autogui/__main__.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/autogui/auto_gui_cls.py` & `pybenutils-3.2.3/pybenutils/autogui/auto_gui_cls.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,33 @@
     from pywinauto import application
     from pywinauto.timings import TimeoutError as pywinautoTimeoutError
 
 logger = get_logger()
 
 
 class AutoGui:
-    def __init__(self, title, app_path, pywinauto_backend='uia'):
+    def __init__(self, title: str, app_path: str, pywinauto_backend='uia', found_index=0):
         """Unified interface to interact with Gui Elements
 
         :param title: Window title
         :param app_path: Application/Exe path
         :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
+        :param found_index: In case more than one matching items are found, select this index from the list (win only)
         """
         self.title = title
         self.app_path = app_path
         assert title or app_path, 'Please provide a title or application path to connect to.\n' \
                                   '\n----------\n' \
                                   'Run "python(3) -m pybenutils.autogui -h" for more information.\n' \
                                   'Run "python(3) -m pybenutils.autogui -eh" for even more information' \
                                   '\n----------\n'
         if sys.platform == 'win32':
             self.app = application.Application(backend=pywinauto_backend)
             try:
-                self.app.connect(title=self.title, timeout=10)
+                self.app.connect(title=self.title, timeout=10, found_index=found_index)
             except pywinautoTimeoutError:
                 logger.debug('Failed to connect to a live window. Will start a new instance')
                 self.app.start(self.app_path)
             self.main_window = self.app.window(title=self.title)
         elif sys.platform == 'darwin':
             self.app = ApplicationControl(self.app_path)
             self.app.application_process_name = self.title
```

### Comparing `pybenutils-3.2.2/pybenutils/browsers/chrome.py` & `pybenutils-3.2.3/pybenutils/browsers/chrome.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/browsers/firefox.py` & `pybenutils-3.2.3/pybenutils/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/browsers/selenium_utils.py` & `pybenutils-3.2.3/pybenutils/browsers/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/browsers/simple_browser_controller_cls.py` & `pybenutils-3.2.3/pybenutils/browsers/simple_browser_controller_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/browsers/web_driver.py` & `pybenutils-3.2.3/pybenutils/browsers/web_driver.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/browsers/windows_browsers_keywords.py` & `pybenutils-3.2.3/pybenutils/browsers/windows_browsers_keywords.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/network/download_manager.py` & `pybenutils-3.2.3/pybenutils/network/download_manager.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/network/http_cert_info.py` & `pybenutils-3.2.3/pybenutils/network/http_cert_info.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/network/s3_bucket_cls.py` & `pybenutils-3.2.3/pybenutils/network/s3_bucket_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/network/ssh_helper.py` & `pybenutils-3.2.3/pybenutils/network/ssh_helper.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/files_and_directories.py` & `pybenutils-3.2.3/pybenutils/os_operations/files_and_directories.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/mac_application_control.py` & `pybenutils-3.2.3/pybenutils/os_operations/mac_application_control.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/mac_input_control.py` & `pybenutils-3.2.3/pybenutils/os_operations/mac_input_control.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/mac_operations.py` & `pybenutils-3.2.3/pybenutils/os_operations/mac_operations.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/mac_popup_handler.py` & `pybenutils-3.2.3/pybenutils/os_operations/mac_popup_handler.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/process.py` & `pybenutils-3.2.3/pybenutils/os_operations/process.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/os_operations/window_operations.py` & `pybenutils-3.2.3/pybenutils/os_operations/window_operations.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/useful.py` & `pybenutils-3.2.3/pybenutils/useful.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils/utils_logger/config_logger.py` & `pybenutils-3.2.3/pybenutils/utils_logger/config_logger.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/pybenutils.egg-info/PKG-INFO` & `pybenutils-3.2.3/pybenutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.2.2
+Version: 3.2.3
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pybenutils-3.2.2/pybenutils.egg-info/SOURCES.txt` & `pybenutils-3.2.3/pybenutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.2/setup.py` & `pybenutils-3.2.3/setup.py`

 * *Files identical despite different names*

