# Comparing `tmp/zoom_python_client-0.1.1.tar.gz` & `tmp/zoom_python_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom_python_client-0.1.1.tar", max compression
+gzip compressed data, was "zoom_python_client-0.2.0.tar", max compression
```

## Comparing `zoom_python_client-0.1.1.tar` & `zoom_python_client-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1100 2023-06-01 10:22:42.927116 zoom_python_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     3306 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/README.md
--rw-r--r--   0        0        0     1346 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/__init__.py
--rw-r--r--   0        0        0     2401 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/api_client.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0        0        0     1722 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0        0        0      624 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/meetings_component.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0        0        0     1286 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/users/users_component.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0        0        0     1583 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0        0        0      401 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinars/webinars_component.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/__init__.py
--rw-r--r--   0        0        0      221 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/file_system.py
--rw-r--r--   0        0        0      731 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/logger.py
--rw-r--r--   0        0        0     8132 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_api_client.py
--rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0        0        0     4629 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
--rw-r--r--   0        0        0      817 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_client_interface.py
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 zoom_python_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-12 13:16:09.560706 zoom_python_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3398 2023-07-12 13:16:09.560706 zoom_python_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1346 2023-07-12 13:16:09.560706 zoom_python_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/__init__.py
+-rw-r--r--   0        0        0     2401 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0        0        0     1722 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0        0        0      624 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/meetings/meetings_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/rooms/__init__.py
+-rw-r--r--   0        0        0     3103 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/rooms/rooms_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0        0        0     1286 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/users/users_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/client_components/webinars/webinars_component.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/utils/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/utils/file_system.py
+-rw-r--r--   0        0        0      731 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/utils/logger.py
+-rw-r--r--   0        0        0      773 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/utils/typed_dict_parameters.py
+-rw-r--r--   0        0        0     8260 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/zoom_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0        0        0     4629 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
+-rw-r--r--   0        0        0      817 2023-07-12 13:16:09.564706 zoom_python_client-0.2.0/zoom_python_client/zoom_client_interface.py
+-rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 zoom_python_client-0.2.0/PKG-INFO
```

### Comparing `zoom_python_client-0.1.1/LICENSE` & `zoom_python_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/README.md` & `zoom_python_client-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,54 +25,54 @@
 - ZOOM_ACCOUNT_ID
 - ZOOM_CLIENT_ID
 - ZOOM_CLIENT_SECRET
 
 ### Initialize the ZoomApiClient from environment variables
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient.init_from_env()
 ```
 
 ### Initialize the ZoomApiClient from .env
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient.init_from_dotenv()
 ```
+
 ### Initialize the ZoomApiClient manually
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>")
 ```
 
 ### Use the file system to store the access token instead of environment
 
 There are some cases where you might want to store the access token in the file system in order to share its value with other elements of the application (Ex. different pods on a Kubernetes/Openshift application).
 
 You can define the path where the token will be stored, passing the `use_path` variable to the constructor:
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>",
         use_path="/path/to/token/folder")
 ```
 
-
 ## How to make API calls
 
 ```python
 MEETING_ID = "12345"
 USER_ID = "abcdfgh"
 
 result = zoom_client.users.get_user(USER_ID)
@@ -89,22 +89,37 @@
 
 setup_logs(log_level=logging.DEBUG)
 ```
 
 ## Available endpoints
 
 ### **users**:
+
 1. get user details
 2. get user meetings
+
 ### **meetings**:
+
 1. get meeting details
 2. get meeting token
+
 ### **meeting live streams**:
+
 1. get meeting live stream
 2. update live stream
 3. update livestream status
+
 ### **webinars**:
+
 1. get webinar details
+
 ### **webinar live streams**:
+
 1. get webinar live stream
 2. update webinar live stream
-3. update webinar livestream status
+3. update webinar livestream status
+
+### **zoom rooms**:
+
+1. get all zoom rooms
+2. get zoom room details
+3. get zoom room sensor data
```

### Comparing `zoom_python_client-0.1.1/pyproject.toml` & `zoom_python_client-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoom-python-client"
-version = "0.1.1"
+version = "0.2.0"
 authors = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 maintainers = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
```

### Comparing `zoom_python_client-0.1.1/zoom_python_client/api_client.py` & `zoom_python_client-0.2.0/zoom_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py` & `zoom_python_client-0.2.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/meetings_component.py` & `zoom_python_client-0.2.0/zoom_python_client/client_components/meetings/meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/client_components/users/users_component.py` & `zoom_python_client-0.2.0/zoom_python_client/client_components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py` & `zoom_python_client-0.2.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/utils/logger.py` & `zoom_python_client-0.2.0/zoom_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/zoom_api_client.py` & `zoom_python_client-0.2.0/zoom_python_client/zoom_api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from zoom_python_client.api_client import ApiClient
 from zoom_python_client.client_components.meeting_livestreams.meeting_livestreams_component import (
     MeetingLiveStreamsComponent,
 )
 from zoom_python_client.client_components.meetings.meetings_component import (
     MeetingsComponent,
 )
+from zoom_python_client.client_components.rooms.rooms_component import RoomsComponent
 from zoom_python_client.client_components.users.users_component import UsersComponent
 from zoom_python_client.client_components.webinar_livestreams.webinar_livestreams_component import (
     WebinarLiveStreamsComponent,
 )
 from zoom_python_client.client_components.webinars.webinars_component import (
     WebinarsComponent,
 )
@@ -68,14 +69,15 @@
     def init_components(self):
         # Add all the new components here
         self.users = UsersComponent(self)
         self.meetings = MeetingsComponent(self)
         self.meeting_livestreams = MeetingLiveStreamsComponent(self)
         self.webinars = WebinarsComponent(self)
         self.webinar_livestreams = WebinarLiveStreamsComponent(self)
+        self.rooms = RoomsComponent(self)
 
     def __init__(
         self,
         account_id: str,
         client_id: str,
         client_secret: str,
         api_endpoint="https://api.zoom.us/v2",
```

### Comparing `zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py` & `zoom_python_client-0.2.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/zoom_python_client/zoom_client_interface.py` & `zoom_python_client-0.2.0/zoom_python_client/zoom_client_interface.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.1/PKG-INFO` & `zoom_python_client-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: Zoom API client for Python using server to server tokens
 Home-page: https://github.com/cern-vc/zoom-python-client
 License: MIT
 Keywords: zoom,api
 Author: Rene Fernandez Sanchez
 Author-email: rene.fernandez@cern.ch
 Maintainer: Rene Fernandez Sanchez
@@ -50,54 +50,54 @@
 - ZOOM_ACCOUNT_ID
 - ZOOM_CLIENT_ID
 - ZOOM_CLIENT_SECRET
 
 ### Initialize the ZoomApiClient from environment variables
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient.init_from_env()
 ```
 
 ### Initialize the ZoomApiClient from .env
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient.init_from_dotenv()
 ```
+
 ### Initialize the ZoomApiClient manually
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>")
 ```
 
 ### Use the file system to store the access token instead of environment
 
 There are some cases where you might want to store the access token in the file system in order to share its value with other elements of the application (Ex. different pods on a Kubernetes/Openshift application).
 
 You can define the path where the token will be stored, passing the `use_path` variable to the constructor:
 
 ```python
-from src.zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.zoom_api_client import ZoomApiClient
 
 zoom_client = ZoomApiClient(
         account_id="<YOUR ACCOUNT ID>",
         client_id="<YOUR CLIENT ID>",
         client_secret="<YOUR CLIENT SECRET>",
         use_path="/path/to/token/folder")
 ```
 
-
 ## How to make API calls
 
 ```python
 MEETING_ID = "12345"
 USER_ID = "abcdfgh"
 
 result = zoom_client.users.get_user(USER_ID)
@@ -114,22 +114,38 @@
 
 setup_logs(log_level=logging.DEBUG)
 ```
 
 ## Available endpoints
 
 ### **users**:
+
 1. get user details
 2. get user meetings
+
 ### **meetings**:
+
 1. get meeting details
 2. get meeting token
+
 ### **meeting live streams**:
+
 1. get meeting live stream
 2. update live stream
 3. update livestream status
+
 ### **webinars**:
+
 1. get webinar details
+
 ### **webinar live streams**:
+
 1. get webinar live stream
 2. update webinar live stream
 3. update webinar livestream status
+
+### **zoom rooms**:
+
+1. get all zoom rooms
+2. get zoom room details
+3. get zoom room sensor data
+
```

