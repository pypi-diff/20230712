# Comparing `tmp/selenium_remote-0.1.4.tar.gz` & `tmp/selenium_remote-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_remote-0.1.4.tar", max compression
+gzip compressed data, was "selenium_remote-0.1.5.tar", max compression
```

## Comparing `selenium_remote-0.1.4.tar` & `selenium_remote-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.000000 selenium_remote-0.1.4/LICENSE
--rw-r--r--   0        0        0       91 2023-07-11 13:29:28.000000 selenium_remote-0.1.4/README.md
--rw-r--r--   0        0        0      735 2023-07-12 11:53:11.546946 selenium_remote-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:36:32.000000 selenium_remote-0.1.4/selenium_remote/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-12 11:46:42.715270 selenium_remote-0.1.4/selenium_remote/main.py
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 selenium_remote-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.000000 selenium_remote-0.1.5/LICENSE
+-rw-r--r--   0        0        0       91 2023-07-11 13:29:28.000000 selenium_remote-0.1.5/README.md
+-rw-r--r--   0        0        0      735 2023-07-12 12:56:27.686955 selenium_remote-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:36:32.000000 selenium_remote-0.1.5/selenium_remote/__init__.py
+-rw-r--r--   0        0        0     2521 2023-07-12 12:55:16.506962 selenium_remote-0.1.5/selenium_remote/main.py
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 selenium_remote-0.1.5/PKG-INFO
```

### Comparing `selenium_remote-0.1.4/LICENSE` & `selenium_remote-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.4/pyproject.toml` & `selenium_remote-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selenium-remote"
-version = "0.1.4"
+version = "0.1.5"
 description = "A package for handling and using a selenium grid server."
 authors = ["George Pamfilis <gpamfilis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "selenium_remote"}]
 repository = "https://github.com/gpamfilis/selenium-remote"
 keywords = ["selenium", "scraping", "webscraping"]
```

### Comparing `selenium_remote-0.1.4/selenium_remote/main.py` & `selenium_remote-0.1.5/selenium_remote/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from fake_useragent import UserAgent
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from urllib3.exceptions import MaxRetryError
 from webdriver_manager.chrome import ChromeDriverManager
+import json
+import requests
 
 logger = logging.getLogger(__name__)
 
 
 def create_remote_driver(
     selenium_grid_url="http://localhost:4445/wd/hub", fake_user_agent=True, remote=True
 ):
@@ -38,14 +40,34 @@
             raise ConnectionError("There was an error with the connection.") from error
         return driver
     service = Service(executable_path=ChromeDriverManager().install())
     driver = webdriver.Chrome(service=service, options=chrome_options)
     return driver
 
 
+def clear_sessions(session_id=None, selenium_grid_url="http://selenium:4444"):
+    """
+    Here we query and delete orphan sessions
+    docs: https://www.selenium.dev/documentation/grid/advanced_features/endpoints/
+    :return: None
+    """
+    if not session_id:
+        # delete all sessions
+        r = requests.get("{}/status".format(selenium_grid_url))
+        data = json.loads(r.text)
+        for node in data["value"]["nodes"]:
+            for slot in node["slots"]:
+                if slot["session"]:
+                    id = slot["session"]["sessionId"]
+                    r = requests.delete("{}/session/{}".format(selenium_grid_url, id))
+    else:
+        # delete session from params
+        r = requests.delete("{}/session/{}".format(selenium_grid_url, session_id))
+
+
 def main():
     """
     This is a test
     """
     return "This is a test"
```

### Comparing `selenium_remote-0.1.4/PKG-INFO` & `selenium_remote-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-remote
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for handling and using a selenium grid server.
 Home-page: https://github.com/gpamfilis/selenium-remote
 Keywords: selenium,scraping,webscraping
 Author: George Pamfilis
 Author-email: gpamfilis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

