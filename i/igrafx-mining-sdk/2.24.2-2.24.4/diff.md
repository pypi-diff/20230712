# Comparing `tmp/igrafx_mining_sdk-2.24.2.tar.gz` & `tmp/igrafx_mining_sdk-2.24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\igrafx_mining_sdk-2.24.2.tar", last modified: Tue Jul 11 09:16:39 2023, max compression
+gzip compressed data, was "igrafx_mining_sdk-2.24.4.tar", last modified: Wed Jul 12 08:57:57 2023, max compression
```

## Comparing `igrafx_mining_sdk-2.24.2.tar` & `igrafx_mining_sdk-2.24.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.925983 igrafx_mining_sdk-2.24.2/
--rw-rw-rw-   0        0        0     1082 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/LICENSE
--rw-rw-rw-   0        0        0      341 2023-07-11 09:16:39.925983 igrafx_mining_sdk-2.24.2/PKG-INFO
--rw-rw-rw-   0        0        0     3644 2023-07-03 09:05:26.000000 igrafx_mining_sdk-2.24.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.896982 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/
--rw-rw-rw-   0        0        0     1754 2023-07-11 08:59:35.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/__init__.py
--rw-rw-rw-   0        0        0     6966 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/api_connector.py
--rw-rw-rw-   0        0        0    11537 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/column_mapping.py
--rw-rw-rw-   0        0        0     3153 2023-07-11 08:50:57.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/datasource.py
--rw-rw-rw-   0        0        0     3418 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/graph.py
--rw-rw-rw-   0        0        0    10081 2023-07-11 08:51:40.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/project.py
--rw-rw-rw-   0        0        0     3077 2023-07-11 08:51:10.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/workgroup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.917981 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/
--rw-rw-rw-   0        0        0      341 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      961 2023-07-11 08:43:20.000000 igrafx_mining_sdk-2.24.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 09:16:39.926979 igrafx_mining_sdk-2.24.2/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-07-11 09:16:37.000000 igrafx_mining_sdk-2.24.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.923991 igrafx_mining_sdk-2.24.2/tests/
--rw-rw-rw-   0        0        0     9022 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/tests/test_column_mapping.py
--rw-rw-rw-   0        0        0     3620 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_datasource.py
--rw-rw-rw-   0        0        0     2118 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_graph.py
--rw-rw-rw-   0        0        0     6863 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_project.py
--rw-rw-rw-   0        0        0     1553 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 08:57:37.000000 igrafx_mining_sdk-2.24.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_workgroup.py
```

### Comparing `igrafx_mining_sdk-2.24.2/README.md` & `igrafx_mining_sdk-2.24.4/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-
-
-# iGrafx P360 Live Mining SDK
-
-
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
-![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/igrafx/mining-python-sdk?color=orange)
-[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/igrafx/mining-python-sdk/blob/main/LICENSE)
-[![GitHub forks](https://badgen.net/github/forks/igrafx/mining-python-sdk)](https://github.com/igrafx/mining-python-sdk/forks)
-![GitHub issues](https://img.shields.io/github/issues/igrafx/mining-python-sdk?color=)
-[![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/igrafx/mining-python-sdk?color=purple)
-![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/igrafx/mining-python-sdk?color=pink)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
-
-***
-
-## Introduction
-
-The **iGrafx P360 Live Mining SDK** is an open source application that can be used to manage your mining projects.
-It is a python implementation of the iGrafx P360 Live Mining API.
-
-With this SDK, you will be able to create workgroups, projects, datasources and graphs (and graph instances). You will also be able to create and 
-add a column mapping.
-
-Please note that you must have an iGrafx account in order to be able to use the SDK properly. Please contact us to create an account.
-
-The iGrafx P360 Live Mining SDK uses Python.
-
-A detailed tutorial can be found in the [howto.md](https://github.com/igrafx/mining-python-sdk/blob/dev/howto.md) file.
-
-
-## Requirements
-
-This package requires python 3.6.8 or above. Get the latest version of [Python](https://www.python.org/).
-
-The required packages should be installed via the ```pyproject.toml``` when running the  ```poetry install``` command. 
-
-## Installing
-
-### With pip:
-To install the current release of the iGrafx P360 Live Mining SDK with **pip**, simply navigate to the console and type the following command: 
-````shell
-pip install igrafx_mining_sdk
-````
-
-### From Wheel:
-
-Download the latest version of the wheel. Then, navigate to your download folder and run: 
-```shell
-pip install igrafx_mining_sdk.whl
-```
-### To begin:
-Go ahead and **import** the package:
-```python
-import igrafx_mining_sdk as igx   # the 'as igx' is entirely optional, but it will make the rest of our code much more readable
-```
-
-## Documentation
-
-The full documentation can be found in the ```howto.md``` file [here](https://github.com/igrafx/mining-python-sdk/blob/dev/howto.md).
-Follow the instructions to try out the SDK.
-
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-
-For more information on how to contribute, please see the [CONTRIBUTING.md](https://github.com/igrafx/mining-python-sdk/blob/dev/CONTRIBUTING.md) file.
-
-## Support
-
-Support is available at the following address: [support@igrafx.com](mailto:support@igrafx.com).
-
-## Notice
-
-Your feedback and contributions are important to us. Don't hesitate to contribute to the project.
-
-## License
-
+
+
+# iGrafx P360 Live Mining SDK
+
+
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/igrafx/mining-python-sdk?color=orange)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/igrafx/mining-python-sdk/blob/main/LICENSE)
+[![GitHub forks](https://badgen.net/github/forks/igrafx/mining-python-sdk)](https://github.com/igrafx/mining-python-sdk/forks)
+![GitHub issues](https://img.shields.io/github/issues/igrafx/mining-python-sdk?color=)
+[![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/igrafx/mining-python-sdk?color=purple)
+![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/igrafx/mining-python-sdk?color=pink)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
+
+***
+
+## Introduction
+
+The **iGrafx P360 Live Mining SDK** is an open source application that can be used to manage your mining projects.
+It is a python implementation of the iGrafx P360 Live Mining API.
+
+With this SDK, you will be able to create workgroups, projects, datasources and graphs (and graph instances). You will also be able to create and 
+add a column mapping.
+
+Please note that you must have an iGrafx account in order to be able to use the SDK properly. Please contact us to create an account.
+
+The iGrafx P360 Live Mining SDK uses Python.
+
+A detailed tutorial can be found in the [howto.md](https://github.com/igrafx/mining-python-sdk/blob/dev/howto.md) file.
+
+
+## Requirements
+
+This package requires python 3.6.8 or above. Get the latest version of [Python](https://www.python.org/).
+
+The required packages should be installed via the ```pyproject.toml``` when running the  ```poetry install``` command. 
+
+## Installing
+
+### With pip:
+To install the current release of the iGrafx P360 Live Mining SDK with **pip**, simply navigate to the console and type the following command: 
+````shell
+pip install igrafx_mining_sdk
+````
+
+### From Wheel:
+
+Download the latest version of the wheel. Then, navigate to your download folder and run: 
+```shell
+pip install igrafx_mining_sdk.whl
+```
+### To begin:
+Go ahead and **import** the package:
+```python
+import igrafx_mining_sdk as igx   # the 'as igx' is entirely optional, but it will make the rest of our code much more readable
+```
+
+## Documentation
+
+The full documentation can be found in the ```howto.md``` file [here](https://github.com/igrafx/mining-python-sdk/blob/dev/howto.md).
+Follow the instructions to try out the SDK.
+
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+For more information on how to contribute, please see the [CONTRIBUTING.md](https://github.com/igrafx/mining-python-sdk/blob/dev/CONTRIBUTING.md) file.
+
+## Support
+
+Support is available at the following address: [support@igrafx.com](mailto:support@igrafx.com).
+
+## Notice
+
+Your feedback and contributions are important to us. Don't hesitate to contribute to the project.
+
+## License
+
 This SDK is licensed under the MIT License. See the ````LICENSE```` file for more details.
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-from igrafx_mining_sdk.column_mapping import FileType, FileStructure, ColumnMapping, MetricAggregation, DimensionAggregation
-from igrafx_mining_sdk.datasource import Datasource
-from igrafx_mining_sdk.workgroup import Workgroup
-from igrafx_mining_sdk.project import Project
-from igrafx_mining_sdk.graph import Graph, GraphInstance
-
-import toml
-from pathlib import Path
-import importlib
-
-
-def extract_metadata():
-    metadata = dict()
-    try:
-        root_dir = Path(__file__).parent.parent
-        with open(
-            root_dir / "pyproject.toml", encoding="utf-8"
-        ) as f:
-            pyproject_data = toml.load(f)
-            metadata['author'] = pyproject_data['tool']['poetry']['authors'][0]
-            metadata['email'] = "contact@igrafx.com"
-            metadata['version'] = pyproject_data['tool']['poetry']['version']
-    except (FileNotFoundError, StopIteration):
-        metadata['author'] = importlib.metadata.metadata('igrafx_mining_sdk')['Author']
-        metadata['email'] = importlib.metadata.metadata('igrafx_mining_sdk')['Author-email']
-        metadata['version'] = importlib.metadata.metadata('igrafx_mining_sdk')['Version']
-    return metadata
-
-
-metadata = extract_metadata()
-__author__ = metadata['author']
-__email__ = metadata['email']
-__version__ = metadata['version']
-__doc__ = """
-igrafx_mining_sdk
-================
-
-Description
------------
-igrafx_mining_sdk is a Python package created by iGrafx. 
-The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
-This information will show up when using the help function.
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+from igrafx_mining_sdk.column_mapping import FileType, FileStructure, ColumnMapping, MetricAggregation, DimensionAggregation
+from igrafx_mining_sdk.datasource import Datasource
+from igrafx_mining_sdk.workgroup import Workgroup
+from igrafx_mining_sdk.project import Project
+from igrafx_mining_sdk.graph import Graph, GraphInstance
+
+import toml
+from pathlib import Path
+import importlib
+
+
+def extract_metadata():
+    metadata = dict()
+    try:
+        root_dir = Path(__file__).parent.parent
+        with open(
+            root_dir / "pyproject.toml", encoding="utf-8"
+        ) as f:
+            pyproject_data = toml.load(f)
+            metadata['author'] = pyproject_data['tool']['poetry']['authors'][0]
+            metadata['email'] = "contact@igrafx.com"
+            metadata['version'] = pyproject_data['tool']['poetry']['version']
+    except (FileNotFoundError, StopIteration):
+        metadata['author'] = importlib.metadata.metadata('igrafx_mining_sdk')['Author']
+        metadata['email'] = importlib.metadata.metadata('igrafx_mining_sdk')['Author-email']
+        metadata['version'] = importlib.metadata.metadata('igrafx_mining_sdk')['Version']
+    return metadata
+
+
+metadata = extract_metadata()
+__author__ = metadata['author']
+__email__ = metadata['email']
+__version__ = metadata['version']
+__doc__ = """
+igrafx_mining_sdk
+================
+
+Description
+-----------
+igrafx_mining_sdk is a Python package created by iGrafx. 
+The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
+This information will show up when using the help function.
 """
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/api_connector.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-import requests as req
-
-class InvalidRouteError(Exception):
-    "Raised when Login failed after a number of try to login"
-    def __init__(self, message="Unauthorized to use this route"):
-        self.message = message
-        super().__init__(self.message)
-
-class APIConnector:
-    """Class to connect to the API. It allows us to log into the Mining Public API and retrive a token.
-    It also allows us to do HTTP GET, POST and DELETE requests."""
-    def __init__(self, wg_id: str, wg_key: str, apiurl: str, authurl: str, ssl_verify: bool):
-        """Initializes the APIConnector class.
-
-        :param wg_id: The ID of the workgroup
-        :param wg_key: The secret key of the workgroup
-        :param apiurl: The URL of the API
-        :param authurl: The URL of the authentication
-        :param ssl_verify: Verify SSL certificates
-        """
-
-        self.wg_id = wg_id
-        self.wg_key = wg_key
-        self.apiurl = self.__process_apiurl(self.__remove_slash(apiurl))
-        self._authurl = self.__remove_slash(authurl)
-        self.ssl_verify = ssl_verify
-        self.token_header = self.__login()
-
-    def __process_apiurl(self, apiurl):
-        """Ensure that the API URL ends with  /pub
-
-        :param apiurl: The URL of the API
-        """
-        return apiurl if apiurl.endswith("/pub") else apiurl + "/pub"
-
-    def __remove_slash(selfself, url):
-        """Ensure that any URL ending with  / are correctly managed and remove / if needed
-
-        :param url: The URL to analyse
-        """
-        return url.strip().rstrip('/')
-
-
-    def __login(self):
-        """Logs into the Mining Public API with the Workgroup's credentials and retrieves a token for later requests"""
-
-        # authurl now contains the realm /realm/logpickr
-        login_url = f"{self._authurl}/protocol/openid-connect/token"
-        login_data = {
-            "grant_type": "client_credentials",
-            "client_id": self.wg_id,
-            "client_secret": self.wg_key
-        }
-
-        try:
-            response = req.post(login_url, login_data, verify=self.ssl_verify)
-            response.raise_for_status()
-            return {"Authorization": "Bearer " + response.json()["access_token"]}
-
-        except req.exceptions.HTTPError as error:
-            print(f"HTTP Error occured: {error}")
-            if error.response.reason == 'Bad Request':
-                raise Exception("Invalid login credentials. \n\nTo check your credentials,"
-                                "please go to the Process Explorer 360.\n"
-                                "When on the platform, go to the workgroup settings and on the Open API tab and "
-                                "check that the correct credentials have been entered.\n\n"
-                                "There, you can find your workgroup's ID and secret key "
-                                "and the API and authentication url.")
-
-    def get_request(self, route, *, params=None, nblasttries=0, maxtries=3):
-        """Does an HTTP GET request to the Mining Public API by simply taking the route and eventual parameters
-
-        :param route: The route of the request
-        :param params: The parameters of the request
-        :param nbtries: The number of try of this route
-        """
-
-        response = None
-        _route = self.apiurl + (route if route.startswith('/') else '/' + route)
-        try:
-            response = req.get(_route,
-                               params=params,
-                               headers=self.token_header,
-                               verify=self.ssl_verify)
-            if response.status_code == 401:  # Only possible if the token has expired
-                if nblasttries < maxtries:
-                    self.token_header = self.__login()
-                    self.get_request(route, params=params, nblasttries=nblasttries+1, maxtries=maxtries)
-                else:
-                    raise InvalidRouteError()
-            response.raise_for_status()
-        except (req.HTTPError, InvalidRouteError) as error:
-            print(f"Http error occured: {error}")
-            print(response.text)
-        return response
-
-    def post_request(self, route, *, params=None, json=None, files=None, headers={}, nblasttries=0, maxtries=3):
-        """Does an HTTP POST request to the Mining Public API by simply taking the route, an eventual JSON, files and headers
-
-        :param route: The route of the request
-        :param params: The parameters of the request
-        :param json: A given JSON object
-        :param files: Eventual files
-        :param headers: Additional headers
-        """
-
-        response = None
-        _route = self.apiurl + (route if route.startswith('/') else '/' + route)
-        try:
-            response = req.post(_route,
-                                params=params,
-                                json=json,
-                                files=files,
-                                headers={**self.token_header, **headers},
-                                verify=self.ssl_verify)
-            if response.status_code == 401:  # Only possible if the token has expired
-                if nblasttries < maxtries:
-                    self.token_header = self.__login()
-                    self.post_request(route, json=json, files=files, headers=headers, nblasttries=nblasttries+1, maxtries=maxtries)
-                else:
-                    raise InvalidRouteError()
-            response.raise_for_status()
-        except (req.HTTPError, InvalidRouteError) as error:
-            if response is not None:
-                print(f"Http error occured: {error}")
-                print(response.text)
-        return response
-
-    def delete_request(self, route, nblasttries=0, maxtries=3):
-        """Does an HTTP DELETE request to the Mining Public API by simply taking the route
-
-        :param route: The route of the request
-        """
-
-        response = None
-        _route = self.apiurl +(route if route.startswith('/') else '/' + route)
-        try:
-            response = req.delete(_route,
-                                  headers=self.token_header,
-                                  verify=self.ssl_verify)
-            if response.status_code == 401:  # Only possible if the token has expired
-                if nblasttries < maxtries:
-                    self.token_header = self.__login()
-                    self.delete_request(route, nblasttries=nblasttries+1, maxtries=maxtries)
-                else:
-                    raise InvalidRouteError()
-            response.raise_for_status()
-        except (req.HTTPError, InvalidRouteError) as error:
-            print(f"Http error occured: {error}")
-            print(response.text)
-        return response
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+import requests as req
+
+class InvalidRouteError(Exception):
+    "Raised when Login failed after a number of try to login"
+    def __init__(self, message="Unauthorized to use this route"):
+        self.message = message
+        super().__init__(self.message)
+
+class APIConnector:
+    """Class to connect to the API. It allows us to log into the Mining Public API and retrive a token.
+    It also allows us to do HTTP GET, POST and DELETE requests."""
+    def __init__(self, wg_id: str, wg_key: str, apiurl: str, authurl: str, ssl_verify: bool):
+        """Initializes the APIConnector class.
+
+        :param wg_id: The ID of the workgroup
+        :param wg_key: The secret key of the workgroup
+        :param apiurl: The URL of the API
+        :param authurl: The URL of the authentication
+        :param ssl_verify: Verify SSL certificates
+        """
+
+        self.wg_id = wg_id
+        self.wg_key = wg_key
+        self.apiurl = self.__process_apiurl(self.__remove_slash(apiurl))
+        self._authurl = self.__remove_slash(authurl)
+        self.ssl_verify = ssl_verify
+        self.token_header = self.__login()
+
+    def __process_apiurl(self, apiurl):
+        """Ensure that the API URL ends with  /pub
+
+        :param apiurl: The URL of the API
+        """
+        return apiurl if apiurl.endswith("/pub") else apiurl + "/pub"
+
+    def __remove_slash(selfself, url):
+        """Ensure that any URL ending with  / are correctly managed and remove / if needed
+
+        :param url: The URL to analyse
+        """
+        return url.strip().rstrip('/')
+
+
+    def __login(self):
+        """Logs into the Mining Public API with the Workgroup's credentials and retrieves a token for later requests"""
+
+        # authurl now contains the realm /realm/logpickr
+        login_url = f"{self._authurl}/protocol/openid-connect/token"
+        login_data = {
+            "grant_type": "client_credentials",
+            "client_id": self.wg_id,
+            "client_secret": self.wg_key
+        }
+
+        try:
+            response = req.post(login_url, login_data, verify=self.ssl_verify)
+            response.raise_for_status()
+            return {"Authorization": "Bearer " + response.json()["access_token"]}
+
+        except req.exceptions.HTTPError as error:
+            print(f"HTTP Error occured: {error}")
+            if error.response.reason == 'Bad Request':
+                raise Exception("Invalid login credentials. \n\nTo check your credentials,"
+                                "please go to the Process Explorer 360.\n"
+                                "When on the platform, go to the workgroup settings and on the Open API tab and "
+                                "check that the correct credentials have been entered.\n\n"
+                                "There, you can find your workgroup's ID and secret key "
+                                "and the API and authentication url.")
+
+    def get_request(self, route, *, params=None, nblasttries=0, maxtries=3):
+        """Does an HTTP GET request to the Mining Public API by simply taking the route and eventual parameters
+
+        :param route: The route of the request
+        :param params: The parameters of the request
+        :param nbtries: The number of try of this route
+        """
+
+        response = None
+        _route = self.apiurl + (route if route.startswith('/') else '/' + route)
+        try:
+            response = req.get(_route,
+                               params=params,
+                               headers=self.token_header,
+                               verify=self.ssl_verify)
+            if response.status_code == 401:  # Only possible if the token has expired
+                if nblasttries < maxtries:
+                    self.token_header = self.__login()
+                    self.get_request(route, params=params, nblasttries=nblasttries+1, maxtries=maxtries)
+                else:
+                    raise InvalidRouteError()
+            response.raise_for_status()
+        except (req.HTTPError, InvalidRouteError) as error:
+            print(f"Http error occured: {error}")
+            print(response.text)
+        return response
+
+    def post_request(self, route, *, params=None, json=None, files=None, headers={}, nblasttries=0, maxtries=3):
+        """Does an HTTP POST request to the Mining Public API by simply taking the route, an eventual JSON, files and headers
+
+        :param route: The route of the request
+        :param params: The parameters of the request
+        :param json: A given JSON object
+        :param files: Eventual files
+        :param headers: Additional headers
+        """
+
+        response = None
+        _route = self.apiurl + (route if route.startswith('/') else '/' + route)
+        try:
+            response = req.post(_route,
+                                params=params,
+                                json=json,
+                                files=files,
+                                headers={**self.token_header, **headers},
+                                verify=self.ssl_verify)
+            if response.status_code == 401:  # Only possible if the token has expired
+                if nblasttries < maxtries:
+                    self.token_header = self.__login()
+                    self.post_request(route, json=json, files=files, headers=headers, nblasttries=nblasttries+1, maxtries=maxtries)
+                else:
+                    raise InvalidRouteError()
+            response.raise_for_status()
+        except (req.HTTPError, InvalidRouteError) as error:
+            if response is not None:
+                print(f"Http error occured: {error}")
+                print(response.text)
+        return response
+
+    def delete_request(self, route, nblasttries=0, maxtries=3):
+        """Does an HTTP DELETE request to the Mining Public API by simply taking the route
+
+        :param route: The route of the request
+        """
+
+        response = None
+        _route = self.apiurl +(route if route.startswith('/') else '/' + route)
+        try:
+            response = req.delete(_route,
+                                  headers=self.token_header,
+                                  verify=self.ssl_verify)
+            if response.status_code == 401:  # Only possible if the token has expired
+                if nblasttries < maxtries:
+                    self.token_header = self.__login()
+                    self.delete_request(route, nblasttries=nblasttries+1, maxtries=maxtries)
+                else:
+                    raise InvalidRouteError()
+            response.raise_for_status()
+        except (req.HTTPError, InvalidRouteError) as error:
+            print(f"Http error occured: {error}")
+            print(response.text)
+        return response
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/column_mapping.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-from enum import Enum
-from typing import List, Union
-
-
-class FileType(str, Enum):
-    """Type of the file that can be added."""
-    csv = "csv"
-    xls = "xls"
-    xlsx = "xlsx"
-
-
-class FileStructure:
-    """ A FileStructure used to create a column mapping"""
-    def __init__(self, file_type: FileType, charset: str = "UTF-8", delimiter: str = ",", quote_char: str = '"',
-                 escape_char: str = '\\',
-                 eol_char: str = "\\r\\n", comment_char: str = "#", sheet_name: str = None,
-                 header: bool = True):
-        """ Creates a FileStructure used to create a column mapping
-
-        :param file_type: the type of the file (CSV, XLS, XLSX)
-        :param charset: the charset of the file (UTF-8, ...)
-        :param delimiter: the delimiter of the file (';', ',', ...)
-        :param quote_char: the character to quote field in the file ('\',...)
-        :param escape_char: the character to escape('\\', ...)
-        :param eol_char: the character for the end of line ('\\n')
-        :param header: the character to comment ('#')
-        :param comment_char: boolean to say if the file contains a header
-        :param sheet_name: the name of the sheet in Excel file
-        """
-
-        self.file_type = file_type
-        self.charset = charset
-        self.delimiter = delimiter
-        self.quote_char = quote_char
-        self.escape_char = escape_char
-        self.eol_char = eol_char
-        self.header = header
-        self.comment_char = comment_char
-        self.sheet_name = sheet_name
-
-    def to_dict(self):
-        """Returns the JSON dictionnary format of the FileStructure"""
-
-        res = {
-            'fileType': self.file_type.value,
-            'charset': self.charset,
-            'delimiter': self.delimiter,
-            'quoteChar': self.quote_char,
-            'escapeChar': self.escape_char,
-            'eolChar': self.eol_char,
-            'header': self.header,
-            'commentChar': self.comment_char,
-        }
-        if self.sheet_name is not None:
-            res['sheetName'] = self.sheet_name
-        return res
-
-
-class DimensionAggregation(Enum):
-    """Class DimensionAggregation for the aggregation types used in column mapping"""
-    FIRST = "FIRST"
-    LAST = "LAST"
-    DISTINCT = "DISTINCT"
-
-
-class GroupedTasksDimensionAggregation(Enum):
-    """Class GroupedTasksDimensionAggregation for the aggregation types used in column mapping"""
-    FIRST = "FIRST"
-    LAST = "LAST"
-
-
-class MetricAggregation(Enum):
-    """Class MetricAggregation for the aggregation types used in column mapping"""
-    FIRST = "FIRST"
-    LAST = "LAST"
-    MIN = "MIN"
-    MAX = "MAX"
-    SUM = "SUM"
-    AVG = "AVG"
-    MEDIAN = "MEDIAN"
-
-
-class ColumnType(Enum):
-    """Class ColumnType for the column types used in column mapping"""
-    CASE_ID = "case_id"
-    TASK_NAME = "task_name"
-    TIME = "time"
-    METRIC = "metric"
-    DIMENSION = "dimension"
-
-
-class Column:
-    """A Column used in the column mapping"""
-    def __init__(self, name: str, index: int, column_type: ColumnType, *, is_case_scope: bool = False,
-                 aggregation: Union[MetricAggregation, DimensionAggregation] = None, grouped_tasks_columns: [] = None,
-                 grouped_tasks_aggregation: Union[GroupedTasksDimensionAggregation, MetricAggregation] = None,
-                 unit: str = None, time_format: str = None):
-        """
-        :param name: the name of the column
-        :param index: the index of the column
-        :param column_type: the type of the column, based on ColumnType
-        :param is_case_scope: boolean to say if the column is a case scope column
-        :param aggregation: the aggregation of the column
-        :param grouped_tasks_columns: list of columns indices that are grouped
-        :param grouped_tasks_aggregation: the aggregation of the grouped tasks
-        :param unit: the unit of the column
-        :param time_format: the time format of the column
-        """
-
-        self.name = name
-        self.index = index
-        self.column_type = column_type
-        self.is_case_scope = is_case_scope
-        self.aggregation = aggregation
-        self.grouped_tasks_columns = grouped_tasks_columns
-        self.grouped_tasks_aggregation = grouped_tasks_aggregation
-        self.unit = unit
-        self.time_format = time_format
-
-        if self.column_type == ColumnType.TIME:
-            if time_format is None:
-                raise ValueError("time_format is required for time column")
-        else:
-            if self.time_format is not None:
-                raise ValueError("time_format can only be used with 'time' column type")
-
-        if any(p is not None for p in [self.aggregation, self.unit]) and self.column_type not in [
-            ColumnType.METRIC, ColumnType.DIMENSION]:
-            raise ValueError(f"Aggregation and unit parameters are not allowed for {self.column_type.value} columns")
-
-        if self.column_type == ColumnType.METRIC and self.aggregation is not None and self.aggregation not in MetricAggregation:
-            raise ValueError("Aggregation of a 'metric' column type must be a MetricAggregation")
-
-        if self.column_type == ColumnType.DIMENSION and self.aggregation is not None and self.aggregation not in DimensionAggregation:
-            raise ValueError("Aggregation of a 'dimension' column type must be a DimensionAggregation")
-
-        if self.column_type == ColumnType.METRIC and self.grouped_tasks_aggregation is not None and self.grouped_tasks_aggregation not in MetricAggregation:
-            raise ValueError("Grouped task aggregation of a 'METRIC' column type must be a MetricAggregation")
-
-        if self.column_type == ColumnType.DIMENSION and self.grouped_tasks_aggregation is not None and self.grouped_tasks_aggregation not in GroupedTasksDimensionAggregation:
-            raise ValueError(
-                "Grouped task aggregation of a 'DIMENSION' column type must be a GroupedTasksDimensionAggregation")
-
-        if self.grouped_tasks_columns is not None and self.column_type != ColumnType.TASK_NAME:
-            raise ValueError("Attribute 'grouped_tasks_columns' can only be used with 'TASK_NAME' column type")
-
-    def to_dict(self):
-        """Returns the JSON dictionary format of the Column"""
-
-        res = {'columnIndex': self.index}
-        if self.aggregation is not None:
-            res['aggregation'] = self.aggregation.value
-        if self.unit is not None:
-            res['unit'] = self.unit
-        if self.column_type == ColumnType.TIME:
-            res['format'] = self.time_format
-        elif self.column_type in [ColumnType.METRIC, ColumnType.DIMENSION]:
-            res['name'] = self.name
-            res['isCaseScope'] = self.is_case_scope
-        if self.grouped_tasks_columns is not None:
-            res['groupedTasksColumns'] = self.grouped_tasks_columns
-        if self.grouped_tasks_aggregation is not None:
-            res['groupedTasksAggregation'] = self.grouped_tasks_aggregation
-        return res
-
-
-class ColumnMapping:
-    """Description of the columnMapping before sending a file"""
-    def __init__(self, column_list: List[Column]):
-        """ Creates a ColumnMapping
-
-        :param column_list: the list of columns to use
-        """
-        column_indices = [c.index for c in column_list]
-        if len(set(column_indices)) != len(column_indices):
-            raise ValueError("Duplicate column indices")
-
-        self.case_id_column = self.__get_columns_from_type(column_list, ColumnType.CASE_ID, expected_num=1)[0]
-        self.task_name_column = self.__get_columns_from_type(column_list, ColumnType.TASK_NAME, expected_num=1)[0]
-        self.time_columns = self.__get_columns_from_type(column_list, ColumnType.TIME, expected_num=[1, 2])
-        self.metric_columns = self.__get_columns_from_type(column_list, ColumnType.METRIC)
-        self.dimension_columns = self.__get_columns_from_type(column_list, ColumnType.DIMENSION)
-
-        if self.task_name_column.grouped_tasks_columns is not None:
-            if any(c.grouped_tasks_aggregation is None for c in self.metric_columns + self.dimension_columns):
-                raise ValueError('If using "grouped_tasks_columns" for "task_name_column", please provide "grouped_task_aggregations" for other columns')
-
-            if self.task_name_column.index not in self.task_name_column.grouped_tasks_columns:
-                raise ValueError(
-                    'The "grouped_tasks_columns" list must include at least an index of a column of type "TASK_NAME"')
-
-            if self.case_id_column.index in self.task_name_column.grouped_tasks_columns:
-                raise ValueError(
-                    'The "grouped_tasks_columns" list cannot contain the index of a column of type "CASE_ID"')
-
-            required_types = {ColumnType.METRIC, ColumnType.DIMENSION, ColumnType.TIME}
-            other_types = set(c.column_type for c in self.metric_columns + self.dimension_columns + self.time_columns)
-            # Check for the intersection of required_types and types of other columns.
-            # If there is no intersection (none of the required types are present), raise an error
-            if not required_types.intersection(other_types):
-                raise ValueError(
-                    'The "grouped_tasks_columns" list must contain the index of a column of type "METRIC", "DIMENSION", or "TIME"')
-
-        if self.task_name_column.grouped_tasks_columns is None:
-            if any(c.grouped_tasks_aggregation is not None for c in self.metric_columns + self.dimension_columns):
-                raise ValueError('If not using "grouped_tasks_columns" for "task_name_column", please do not provide "grouped_task_aggregations" for other columns')
-
-    def __get_columns_from_type(self, column_list: List[Column], filter: ColumnType, *,
-                                expected_num: Union[int, List[int]] = None) -> List[Column]:
-        """Returns a list of columns based on their type
-
-        :param column_list: the list of columns to use
-        :param filter: the type of the column
-        :param expected_num: the expected number of columns
-        :return: the list of columns
-        """
-        filtered_list = [c for c in column_list if c.column_type == filter]
-        if expected_num is not None:
-            if isinstance(expected_num, int):
-                if len(filtered_list) != expected_num:
-                    raise ValueError(f"Number of {filter} columns should be {expected_num}")
-            else:
-                if len(filtered_list) not in expected_num:
-                    raise ValueError(f"Number of {filter} columns should be one of following values: {expected_num}")
-        return filtered_list
-
-    def to_dict(self):
-        """Returns the JSON dictionary format of the ColumnMapping"""
-        return {
-            'caseIdMapping': self.case_id_column.to_dict(),
-            'activityMapping': self.task_name_column.to_dict(),  # activity = task_name
-            'timeMappings': [c.to_dict() for c in self.time_columns],
-            'dimensionsMappings': [c.to_dict() for c in self.dimension_columns],
-            'metricsMappings': [c.to_dict() for c in self.metric_columns],
-        }
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+from enum import Enum
+from typing import List, Union
+
+
+class FileType(str, Enum):
+    """Type of the file that can be added."""
+    csv = "csv"
+    xls = "xls"
+    xlsx = "xlsx"
+
+
+class FileStructure:
+    """ A FileStructure used to create a column mapping"""
+    def __init__(self, file_type: FileType, charset: str = "UTF-8", delimiter: str = ",", quote_char: str = '"',
+                 escape_char: str = '\\',
+                 eol_char: str = "\\r\\n", comment_char: str = "#", sheet_name: str = None,
+                 header: bool = True):
+        """ Creates a FileStructure used to create a column mapping
+
+        :param file_type: the type of the file (CSV, XLS, XLSX)
+        :param charset: the charset of the file (UTF-8, ...)
+        :param delimiter: the delimiter of the file (';', ',', ...)
+        :param quote_char: the character to quote field in the file ('\',...)
+        :param escape_char: the character to escape('\\', ...)
+        :param eol_char: the character for the end of line ('\\n')
+        :param header: the character to comment ('#')
+        :param comment_char: boolean to say if the file contains a header
+        :param sheet_name: the name of the sheet in Excel file
+        """
+
+        self.file_type = file_type
+        self.charset = charset
+        self.delimiter = delimiter
+        self.quote_char = quote_char
+        self.escape_char = escape_char
+        self.eol_char = eol_char
+        self.header = header
+        self.comment_char = comment_char
+        self.sheet_name = sheet_name
+
+    def to_dict(self):
+        """Returns the JSON dictionnary format of the FileStructure"""
+
+        res = {
+            'fileType': self.file_type.value,
+            'charset': self.charset,
+            'delimiter': self.delimiter,
+            'quoteChar': self.quote_char,
+            'escapeChar': self.escape_char,
+            'eolChar': self.eol_char,
+            'header': self.header,
+            'commentChar': self.comment_char,
+        }
+        if self.sheet_name is not None:
+            res['sheetName'] = self.sheet_name
+        return res
+
+
+class DimensionAggregation(Enum):
+    """Class DimensionAggregation for the aggregation types used in column mapping"""
+    FIRST = "FIRST"
+    LAST = "LAST"
+    DISTINCT = "DISTINCT"
+
+
+class GroupedTasksDimensionAggregation(Enum):
+    """Class GroupedTasksDimensionAggregation for the aggregation types used in column mapping"""
+    FIRST = "FIRST"
+    LAST = "LAST"
+
+
+class MetricAggregation(Enum):
+    """Class MetricAggregation for the aggregation types used in column mapping"""
+    FIRST = "FIRST"
+    LAST = "LAST"
+    MIN = "MIN"
+    MAX = "MAX"
+    SUM = "SUM"
+    AVG = "AVG"
+    MEDIAN = "MEDIAN"
+
+
+class ColumnType(Enum):
+    """Class ColumnType for the column types used in column mapping"""
+    CASE_ID = "case_id"
+    TASK_NAME = "task_name"
+    TIME = "time"
+    METRIC = "metric"
+    DIMENSION = "dimension"
+
+
+class Column:
+    """A Column used in the column mapping"""
+    def __init__(self, name: str, index: int, column_type: ColumnType, *, is_case_scope: bool = False,
+                 aggregation: Union[MetricAggregation, DimensionAggregation] = None, grouped_tasks_columns: [] = None,
+                 grouped_tasks_aggregation: Union[GroupedTasksDimensionAggregation, MetricAggregation] = None,
+                 unit: str = None, time_format: str = None):
+        """
+        :param name: the name of the column
+        :param index: the index of the column
+        :param column_type: the type of the column, based on ColumnType
+        :param is_case_scope: boolean to say if the column is a case scope column
+        :param aggregation: the aggregation of the column
+        :param grouped_tasks_columns: list of columns indices that are grouped
+        :param grouped_tasks_aggregation: the aggregation of the grouped tasks
+        :param unit: the unit of the column
+        :param time_format: the time format of the column
+        """
+
+        self.name = name
+        self.index = index
+        self.column_type = column_type
+        self.is_case_scope = is_case_scope
+        self.aggregation = aggregation
+        self.grouped_tasks_columns = grouped_tasks_columns
+        self.grouped_tasks_aggregation = grouped_tasks_aggregation
+        self.unit = unit
+        self.time_format = time_format
+
+        if self.column_type == ColumnType.TIME:
+            if time_format is None:
+                raise ValueError("time_format is required for time column")
+        else:
+            if self.time_format is not None:
+                raise ValueError("time_format can only be used with 'time' column type")
+
+        if any(p is not None for p in [self.aggregation, self.unit]) and self.column_type not in [
+            ColumnType.METRIC, ColumnType.DIMENSION]:
+            raise ValueError(f"Aggregation and unit parameters are not allowed for {self.column_type.value} columns")
+
+        if self.column_type == ColumnType.METRIC and self.aggregation is not None and self.aggregation not in MetricAggregation:
+            raise ValueError("Aggregation of a 'metric' column type must be a MetricAggregation")
+
+        if self.column_type == ColumnType.DIMENSION and self.aggregation is not None and self.aggregation not in DimensionAggregation:
+            raise ValueError("Aggregation of a 'dimension' column type must be a DimensionAggregation")
+
+        if self.column_type == ColumnType.METRIC and self.grouped_tasks_aggregation is not None and self.grouped_tasks_aggregation not in MetricAggregation:
+            raise ValueError("Grouped task aggregation of a 'METRIC' column type must be a MetricAggregation")
+
+        if self.column_type == ColumnType.DIMENSION and self.grouped_tasks_aggregation is not None and self.grouped_tasks_aggregation not in GroupedTasksDimensionAggregation:
+            raise ValueError(
+                "Grouped task aggregation of a 'DIMENSION' column type must be a GroupedTasksDimensionAggregation")
+
+        if self.grouped_tasks_columns is not None and self.column_type != ColumnType.TASK_NAME:
+            raise ValueError("Attribute 'grouped_tasks_columns' can only be used with 'TASK_NAME' column type")
+
+    def to_dict(self):
+        """Returns the JSON dictionary format of the Column"""
+
+        res = {'columnIndex': self.index}
+        if self.aggregation is not None:
+            res['aggregation'] = self.aggregation.value
+        if self.unit is not None:
+            res['unit'] = self.unit
+        if self.column_type == ColumnType.TIME:
+            res['format'] = self.time_format
+        elif self.column_type in [ColumnType.METRIC, ColumnType.DIMENSION]:
+            res['name'] = self.name
+            res['isCaseScope'] = self.is_case_scope
+        if self.grouped_tasks_columns is not None:
+            res['groupedTasksColumns'] = self.grouped_tasks_columns
+        if self.grouped_tasks_aggregation is not None:
+            res['groupedTasksAggregation'] = self.grouped_tasks_aggregation
+        return res
+
+
+class ColumnMapping:
+    """Description of the columnMapping before sending a file"""
+    def __init__(self, column_list: List[Column]):
+        """ Creates a ColumnMapping
+
+        :param column_list: the list of columns to use
+        """
+        column_indices = [c.index for c in column_list]
+        if len(set(column_indices)) != len(column_indices):
+            raise ValueError("Duplicate column indices")
+
+        self.case_id_column = self.__get_columns_from_type(column_list, ColumnType.CASE_ID, expected_num=1)[0]
+        self.task_name_column = self.__get_columns_from_type(column_list, ColumnType.TASK_NAME, expected_num=1)[0]
+        self.time_columns = self.__get_columns_from_type(column_list, ColumnType.TIME, expected_num=[1, 2])
+        self.metric_columns = self.__get_columns_from_type(column_list, ColumnType.METRIC)
+        self.dimension_columns = self.__get_columns_from_type(column_list, ColumnType.DIMENSION)
+
+        if self.task_name_column.grouped_tasks_columns is not None:
+            if any(c.grouped_tasks_aggregation is None for c in self.metric_columns + self.dimension_columns):
+                raise ValueError('If using "grouped_tasks_columns" for "task_name_column", please provide "grouped_task_aggregations" for other columns')
+
+            if self.task_name_column.index not in self.task_name_column.grouped_tasks_columns:
+                raise ValueError(
+                    'The "grouped_tasks_columns" list must include at least an index of a column of type "TASK_NAME"')
+
+            if self.case_id_column.index in self.task_name_column.grouped_tasks_columns:
+                raise ValueError(
+                    'The "grouped_tasks_columns" list cannot contain the index of a column of type "CASE_ID"')
+
+            required_types = {ColumnType.METRIC, ColumnType.DIMENSION, ColumnType.TIME}
+            other_types = set(c.column_type for c in self.metric_columns + self.dimension_columns + self.time_columns)
+            # Check for the intersection of required_types and types of other columns.
+            # If there is no intersection (none of the required types are present), raise an error
+            if not required_types.intersection(other_types):
+                raise ValueError(
+                    'The "grouped_tasks_columns" list must contain the index of a column of type "METRIC", "DIMENSION", or "TIME"')
+
+        if self.task_name_column.grouped_tasks_columns is None:
+            if any(c.grouped_tasks_aggregation is not None for c in self.metric_columns + self.dimension_columns):
+                raise ValueError('If not using "grouped_tasks_columns" for "task_name_column", please do not provide "grouped_task_aggregations" for other columns')
+
+    def __get_columns_from_type(self, column_list: List[Column], filter: ColumnType, *,
+                                expected_num: Union[int, List[int]] = None) -> List[Column]:
+        """Returns a list of columns based on their type
+
+        :param column_list: the list of columns to use
+        :param filter: the type of the column
+        :param expected_num: the expected number of columns
+        :return: the list of columns
+        """
+        filtered_list = [c for c in column_list if c.column_type == filter]
+        if expected_num is not None:
+            if isinstance(expected_num, int):
+                if len(filtered_list) != expected_num:
+                    raise ValueError(f"Number of {filter} columns should be {expected_num}")
+            else:
+                if len(filtered_list) not in expected_num:
+                    raise ValueError(f"Number of {filter} columns should be one of following values: {expected_num}")
+        return filtered_list
+
+    def to_dict(self):
+        """Returns the JSON dictionary format of the ColumnMapping"""
+        return {
+            'caseIdMapping': self.case_id_column.to_dict(),
+            'activityMapping': self.task_name_column.to_dict(),  # activity = task_name
+            'timeMappings': [c.to_dict() for c in self.time_columns],
+            'dimensionsMappings': [c.to_dict() for c in self.dimension_columns],
+            'metricsMappings': [c.to_dict() for c in self.metric_columns],
+        }
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/datasource.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-import pandas
-from pydruid import db
-from igrafx_mining_sdk.api_connector import APIConnector
-
-
-class Datasource:
-    """A Druid table that can be requested by the user"""
-    def __init__(self, name: str, dstype: str, host: str, port: str, api_connector: APIConnector):
-        """Initialise a datasource
-
-        :param name: the name of the datasource
-        :param dstype: the type of the datasource
-        :param host: the host of the datasource
-        :param port: the port number of the datasource
-        :param api_connector: an APIConnector object that can be used to send requests to the datasource
-        """
-
-        self.name = name
-        self.type = dstype
-        self.host = host
-        self.port = port
-        self.api_connector = api_connector
-        self._connection = None
-        self._cursor = None
-        self._columns = None
-
-    def load_dataframe(self, load_limit=None):
-        """Converts an SQL request to a dataframe
-
-        :param load_limit: Maximum number of rows to load
-        """
-        sqlreq = f'SELECT * FROM "{self.name}"'
-        if load_limit is not None:
-            sqlreq += f'LIMIT {load_limit}'
-        return self.request(sqlreq)
-
-    def request(self, sqlreq):
-        """Sends an SQL request to the datasource and returns the results as a pandas Dataframe
-
-        :param sqlreq: the SQL request to execute
-        """
-        self.cursor.execute(sqlreq)
-        rows = self.cursor.fetchall()
-        cols = [i[0] for i in self.cursor.description]
-        return pandas.DataFrame(rows, columns=cols)
-
-    @property
-    def columns(self):
-        """Returns the columns of the datasource"""
-        if self._columns is None:
-            res = self.request(
-                f"SELECT COLUMN_NAME, ORDINAL_POSITION, DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME ="
-                f" '{self.name}' ORDER BY 2")
-            self._columns = res["COLUMN_NAME"].to_list()
-        return self._columns
-
-    @property
-    def connection(self):
-        """Returns the Pydruid connection to the datasource, after initializing it, if need be"""
-        if self._connection is None:
-            self._connection = db.connect(self.host, self.port, path="/druid/v2/sql",
-                                          user=self.api_connector.wg_id,
-                                          password=self.api_connector.wg_key)
-        return self._connection
-
-    @property
-    def cursor(self):
-        """Returns the Pydruid cursor on the datasource, after initializing it if it doesn't exist"""
-        if self._cursor is None:
-            self._cursor = self.connection.cursor()
-        return self._cursor
-
-    def close(self):
-        """Closes the connection and the cursor if necessary"""
-        if self._cursor is not None:
-            self._cursor.close()
-            self._cursor = None
-        if self._connection is not None:
-            self._connection.close()
-            self._connection = None
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+import pandas
+from pydruid import db
+from igrafx_mining_sdk.api_connector import APIConnector
+
+
+class Datasource:
+    """A Druid table that can be requested by the user"""
+    def __init__(self, name: str, dstype: str, host: str, port: str, api_connector: APIConnector):
+        """Initialise a datasource
+
+        :param name: the name of the datasource
+        :param dstype: the type of the datasource
+        :param host: the host of the datasource
+        :param port: the port number of the datasource
+        :param api_connector: an APIConnector object that can be used to send requests to the datasource
+        """
+
+        self.name = name
+        self.type = dstype
+        self.host = host
+        self.port = port
+        self.api_connector = api_connector
+        self._connection = None
+        self._cursor = None
+        self._columns = None
+
+    def load_dataframe(self, load_limit=None):
+        """Converts an SQL request to a dataframe
+
+        :param load_limit: Maximum number of rows to load
+        """
+        sqlreq = f'SELECT * FROM "{self.name}"'
+        if load_limit is not None:
+            sqlreq += f'LIMIT {load_limit}'
+        return self.request(sqlreq)
+
+    def request(self, sqlreq):
+        """Sends an SQL request to the datasource and returns the results as a pandas Dataframe
+
+        :param sqlreq: the SQL request to execute
+        """
+        self.cursor.execute(sqlreq)
+        rows = self.cursor.fetchall()
+        cols = [i[0] for i in self.cursor.description]
+        return pandas.DataFrame(rows, columns=cols)
+
+    @property
+    def columns(self):
+        """Returns the columns of the datasource"""
+        if self._columns is None:
+            res = self.request(
+                f"SELECT COLUMN_NAME, ORDINAL_POSITION, DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME ="
+                f" '{self.name}' ORDER BY 2")
+            self._columns = res["COLUMN_NAME"].to_list()
+        return self._columns
+
+    @property
+    def connection(self):
+        """Returns the Pydruid connection to the datasource, after initializing it, if need be"""
+        if self._connection is None:
+            self._connection = db.connect(self.host, self.port, path="/druid/v2/sql",
+                                          user=self.api_connector.wg_id,
+                                          password=self.api_connector.wg_key)
+        return self._connection
+
+    @property
+    def cursor(self):
+        """Returns the Pydruid cursor on the datasource, after initializing it if it doesn't exist"""
+        if self._cursor is None:
+            self._cursor = self.connection.cursor()
+        return self._cursor
+
+    def close(self):
+        """Closes the connection and the cursor if necessary"""
+        if self._cursor is not None:
+            self._cursor.close()
+            self._cursor = None
+        if self._connection is not None:
+            self._connection.close()
+            self._connection = None
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/graph.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-import json
-import networkx as nx
-
-
-class Graph(nx.DiGraph):
-    """A graph from a iGrafx P360 Live Mining project, created with the parent Project's ID, a list of nodes and a list of edges"""
-    def __init__(self, project_id: str, nodes_list: list, edges_list: list):
-        """Initializes a graph from a Mining project, created with the parent Project's ID'
-
-        :param project_id: the ID of the parent project
-        :param nodes_list: the list of nodes
-        :param edges_list: the list of edges
-        """
-        super().__init__()
-        self.project_id = project_id
-        self.graph['project_id'] = project_id
-        self.add_nodes_from(nodes_list)
-        self.add_edges_from(edges_list)
-
-    @staticmethod
-    def from_dict(project_id, jgraph):
-        """Static method that creates a Graph based on the dictionary representation of the graph
-
-        :param project_id: the ID of the project the graph is in
-        :param jgraph: the dictionary we want to parse the graph from
-        """
-        nodes_list = [(item["id"], item) for item in jgraph["vertices"]]
-        edges_list = [(item["source"], item["destination"], item) for item in jgraph["edges"]]
-        return Graph(project_id, nodes_list, edges_list)
-
-    @staticmethod
-    def from_json(project_id, path):
-        """Static method that creates a Graph based on the JSON returned by the iGrafx Mining Public API
-
-        :param project_id: the ID of the project the graph is in
-        :param path: the path to the JSON file we want to parse the graph from
-        """
-        with open(path, 'r') as f:
-            jgraph = json.load(f)
-        return Graph.from_dict(project_id, jgraph)
-
-
-class GraphInstance(Graph):
-    """A graph instance from a iGrafx P360 Live Mining project, created with the parent Project's ID,
-    a list of vertex instances and a list of edge instances
-    """
-    def __init__(self, project_id: str, nodes_list: list, edges_list: list, rework_total: int, concurrency_rate: float):
-        super().__init__(project_id, nodes_list, edges_list)
-        self.rework_total = rework_total
-        self.concurrency_rate = concurrency_rate
-
-    @staticmethod
-    def from_dict(project_id, jgraph):
-        """Static method that creates a GraphInstance based on the dictionary representation of the graph instance
-
-        :param project_id: the ID of the project the graph instance is in
-        :param jgraph: the dictionary we want to parse the graph instance from
-        """
-        nodes_list = [(item["id"], item) for item in jgraph["vertexInstances"]]
-        edges_list = [(item["source"]["id"], item["destination"]["id"]) for item in jgraph["edgeInstances"]]
-        return GraphInstance(project_id, nodes_list, edges_list, jgraph["reworkTotal"], jgraph["concurrencyRate"])
-
-    @staticmethod
-    def from_json(project_id, path):
-        """Static method that creates a GraphInstance based on the json representation returned by the Logpickr API
-
-        :param project_id: the ID of the project the graph is in
-        :param path: the path to the JSON file we want to parse the graph from"""
-
-        with open(path, 'r') as f:
-            jgraph = json.load(f)
-        return GraphInstance.from_dict(project_id, jgraph)
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+import json
+import networkx as nx
+
+
+class Graph(nx.DiGraph):
+    """A graph from a iGrafx P360 Live Mining project, created with the parent Project's ID, a list of nodes and a list of edges"""
+    def __init__(self, project_id: str, nodes_list: list, edges_list: list):
+        """Initializes a graph from a Mining project, created with the parent Project's ID'
+
+        :param project_id: the ID of the parent project
+        :param nodes_list: the list of nodes
+        :param edges_list: the list of edges
+        """
+        super().__init__()
+        self.project_id = project_id
+        self.graph['project_id'] = project_id
+        self.add_nodes_from(nodes_list)
+        self.add_edges_from(edges_list)
+
+    @staticmethod
+    def from_dict(project_id, jgraph):
+        """Static method that creates a Graph based on the dictionary representation of the graph
+
+        :param project_id: the ID of the project the graph is in
+        :param jgraph: the dictionary we want to parse the graph from
+        """
+        nodes_list = [(item["id"], item) for item in jgraph["vertices"]]
+        edges_list = [(item["source"], item["destination"], item) for item in jgraph["edges"]]
+        return Graph(project_id, nodes_list, edges_list)
+
+    @staticmethod
+    def from_json(project_id, path):
+        """Static method that creates a Graph based on the JSON returned by the iGrafx Mining Public API
+
+        :param project_id: the ID of the project the graph is in
+        :param path: the path to the JSON file we want to parse the graph from
+        """
+        with open(path, 'r') as f:
+            jgraph = json.load(f)
+        return Graph.from_dict(project_id, jgraph)
+
+
+class GraphInstance(Graph):
+    """A graph instance from a iGrafx P360 Live Mining project, created with the parent Project's ID,
+    a list of vertex instances and a list of edge instances
+    """
+    def __init__(self, project_id: str, nodes_list: list, edges_list: list, rework_total: int, concurrency_rate: float):
+        super().__init__(project_id, nodes_list, edges_list)
+        self.rework_total = rework_total
+        self.concurrency_rate = concurrency_rate
+
+    @staticmethod
+    def from_dict(project_id, jgraph):
+        """Static method that creates a GraphInstance based on the dictionary representation of the graph instance
+
+        :param project_id: the ID of the project the graph instance is in
+        :param jgraph: the dictionary we want to parse the graph instance from
+        """
+        nodes_list = [(item["id"], item) for item in jgraph["vertexInstances"]]
+        edges_list = [(item["source"]["id"], item["destination"]["id"]) for item in jgraph["edgeInstances"]]
+        return GraphInstance(project_id, nodes_list, edges_list, jgraph["reworkTotal"], jgraph["concurrencyRate"])
+
+    @staticmethod
+    def from_json(project_id, path):
+        """Static method that creates a GraphInstance based on the json representation returned by the Logpickr API
+
+        :param project_id: the ID of the project the graph is in
+        :param path: the path to the JSON file we want to parse the graph from"""
+
+        with open(path, 'r') as f:
+            jgraph = json.load(f)
+        return GraphInstance.from_dict(project_id, jgraph)
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/project.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-import os
-import random
-from igrafx_mining_sdk.graph import Graph, GraphInstance
-from igrafx_mining_sdk.column_mapping import FileStructure, ColumnMapping
-from igrafx_mining_sdk.datasource import Datasource
-from igrafx_mining_sdk.api_connector import APIConnector
-
-
-class Project:
-    """A iGrafx P360 Live Mining project"""
-    def __init__(self, pid: str, api_connector: APIConnector):
-        """Create a iGrafx P360 Live Mining project from a project ID and the Workgroup it was created from
-
-        :param pid: the Project's ID
-        :param api_connector: the APIConnector object
-        """
-        self.id = pid
-        self.api_connector = api_connector
-        self._graph = None
-        self._ds_response = None
-        self._process_keys = []
-
-    @property
-    def exists(self):
-        """Check if the project exists"""
-        response_project_exist = self.api_connector.get_request(f"/project/{self.id}/exist").json()
-        return response_project_exist["exists"]
-
-    def delete_project(self):
-        """Deletes the project"""
-        response_project_delete = self.api_connector.delete_request(f"/project/{self.id}")
-        return response_project_delete
-
-    def get_project_name(self):
-        """Returns the name of the project"""
-        response_project_name = self.api_connector.get_request(f"/project/{self.id}/name").json()
-        return response_project_name["name"]
-
-    def graph(self, gateways=False):
-        """Performs a REST request for the project model graph if it hasn't already been retrieved.
-
-        :param gateways: Boolean that controls whether the graph returned will be BPMN-like or not
-        """
-        if self._graph is None:
-            params = {"mode": "gateways" if gateways else "simplified"}
-            response_graph = self.api_connector.get_request(
-                f"/project/{self.id}/graph",
-                params=params)
-            self._graph = Graph.from_dict(self.id, response_graph.json())
-        return self._graph
-
-    def get_graph_instances(self, limit=None, shuffle=False):
-        """Returns all the project's Graph Instances, performing a REST request for any instances that don't already
-        exist within the project.
-
-        :param limit: the maximum number of graph instances to return
-        :param shuffle: whether to shuffle the list of graph instances with a default value set to False
-        """
-        limit = min(limit, len(self.process_keys)) if limit is not None else len(self.process_keys)
-        sample = random.sample(self.process_keys, limit) if shuffle else self.process_keys[:limit]
-        return [self.graph_instance_from_key(k) for k in sample]
-
-    def graph_instance_from_key(self, process_id):
-        """Performs a REST request for the graph instance associated with a process key, and returns it.
-
-        :param process_id: the id of the process whose graph we want to get
-        """
-        parameters = {"processId": process_id}
-        response_graph_instance = None
-        try:
-            response_graph_instance = self.api_connector.get_request(
-                f"/project/{self.id}/graphInstance",
-                params=parameters)
-            graph = response_graph_instance.json()
-            graph_instance = GraphInstance.from_dict(self.id, graph)
-        except Exception as error:
-            print(f"Could not parse graph: {error}")
-            print(response_graph_instance)
-            return None
-        return graph_instance
-
-    def __datasource_request(self):
-        """Request datasources associated with the project"""
-
-        response_datasource = self.api_connector.get_request(f"/datasources/{self.id}")
-        return response_datasource.json()
-
-    @property
-    def nodes_datasource(self):
-        """Returns datasource of type '_vertex'"""
-        return self.__get_datasource_by_name('_vertex')
-
-    @property
-    def edges_datasource(self):
-        """Returns datasource of type '_simplifiedEdge'"""
-        return self.__get_datasource_by_name('_simplifiedEdge')
-
-
-    @property
-    def cases_datasource(self):
-        """Returns datasource of type 'cases'"""
-        return self.__get_datasource_by_name('cases')
-
-    def __get_datasource_by_name(self, ds_type):
-        """Helper method that filters the datasources based on the given type
-
-        :param ds_type: The type of datasource. Can be 'cases', '_simplifiedEdge' or '_vertex'
-        """
-        self._ds_response = self.__datasource_request() if self._ds_response is None else self._ds_response
-
-        for item in self._ds_response:
-            if "_simplifiedEdge" in item["name"]:
-                item["type"] = "_simplifiedEdge"
-            elif "_vertex" in item["name"]:
-                item["type"] = "_vertex"
-            else:
-                item["type"] = "cases"
-
-        response_filtered = [d for d in self._ds_response if d['type'] == ds_type][0]
-        return Datasource(
-            response_filtered["name"],
-            response_filtered["type"],
-            response_filtered["host"],
-            response_filtered["port"],
-            self.api_connector)
-
-    def get_project_variants(self, page_index: int, limit: int, search: str = None):
-        """Returns the project variants
-
-        :param page_index: the page index for pagination
-        :param limit: The maximum number of items to return per page
-        :param search: The search query to filter variants by name (optional)
-        """
-        params = {"projectId": self.id, "pageIndex": page_index, "limit": limit}
-        if search is not None:
-            params["search"] = search
-
-        route = f"/project/{self.id}/variants"
-        response_variants = self.api_connector.get_request(route, params=params)
-        return response_variants.json()
-
-    def get_project_completed_cases(self, page_index: int, limit: int, search_case_id: str = None):
-        """Returns the projects completed cases
-
-        :param page_index: the page index for pagination
-        :param limit: The maximum number of items to return per page
-        :param search: The search query to filter cases by ID (optional)
-
-        """
-        params = {"projectId": self.id, "pageIndex": page_index, "limit": limit}
-        if search_case_id is not None:
-            params["searchCaseId"] = search_case_id
-
-        route = f"/project/{self.id}/completedCases"
-        response_case_ids = self.api_connector.get_request(route, params=params)
-        return response_case_ids.json()
-
-    @property
-    def process_keys(self):
-        """Queries the datasources to find the different process keys of the project"""
-
-        if len(self._process_keys) == 0:
-            ds = self.edges_datasource
-            res = ds.request(f"SELECT DISTINCT processkey FROM \"{ds.name}\"")
-            self._process_keys = [key for key in res['processkey']]
-
-        return self._process_keys
-
-    def add_column_mapping(self, filestructure: FileStructure, columnmapping: ColumnMapping):
-        """Create a column mapping for the project
-
-        :param filestructure: the filestructure
-        :param columnmapping: the columnmapping
-        """
-        route = f"/project/{self.id}/column-mapping"
-        json = {'fileStructure': filestructure.to_dict(), 'columnMapping': columnmapping.to_dict()}
-        response_column_mapping = self.api_connector.post_request(route, json=json)
-        return response_column_mapping.status_code == 204
-
-    @property
-    def column_mapping_exists(self):
-        """Check if a column mapping exists"""
-
-        json_response = self.api_connector.get_request(f"/project/{self.id}/column-mapping-exists")
-        return json_response.json()['exists']
-
-    def get_mapping_infos(self):
-        """Returns the mapping infos of the project such as the column names"""
-
-        response_mapping_infos = self.api_connector.get_request(f"/project/{self.id}/mappingInfos").json()
-        return response_mapping_infos
-
-    def reset(self):
-        """Makes an API call to manually reset a project"""
-
-        response_reset = self.api_connector.post_request(f"/project/{self.id}/reset")
-        return response_reset.status_code == 204
-
-    def add_file(self, path):
-        """Adds a file to the project
-
-        :param path: the path to the file to add
-        """
-        route = f"/project/{self.id}/file?teamId={self.api_connector.wg_id}"
-        file_extension = os.path.splitext(path)[-1].lower()
-        if file_extension == ".csv":
-            mime_type = "text/csv"
-        elif file_extension == ".xlsx":
-            mime_type = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
-        elif file_extension == ".xls":
-            mime_type = "application/vnd.ms-excel"
-        else:
-            raise ValueError(f"File extension {file_extension} is not supported")
-
-        with open(path, 'rb') as file:
-            files = {'file': (os.path.basename(path), file, mime_type)}
-            headers = {"accept": "application/json, text/plain, */*"}
-            response_add_file = self.api_connector.post_request(route, files=files, headers=headers)
-
-        print(response_add_file)
-        return response_add_file.status_code == 201
-
-    @property
-    def train_status(self):
-        """Returns True if the train is currently running, False otherwise"""
-        json_response = self.api_connector.get_request(f"/train/{self.id}")
-        return json_response["isTrainRunning"]
-
-    def launch_train(self):
-        """Makes an API call to manually launch the train of a project"""
-        self.api_connector.post_request(f"/train/{self.id}/launch")
-
-    def stop_train(self):
-        """Makes an API call to manually stop the train of a project"""
-        self.api_connector.delete_request(f"/train/{self.id}")
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+import os
+import random
+from igrafx_mining_sdk.graph import Graph, GraphInstance
+from igrafx_mining_sdk.column_mapping import FileStructure, ColumnMapping
+from igrafx_mining_sdk.datasource import Datasource
+from igrafx_mining_sdk.api_connector import APIConnector
+
+
+class Project:
+    """A iGrafx P360 Live Mining project"""
+    def __init__(self, pid: str, api_connector: APIConnector):
+        """Create a iGrafx P360 Live Mining project from a project ID and the Workgroup it was created from
+
+        :param pid: the Project's ID
+        :param api_connector: the APIConnector object
+        """
+        self.id = pid
+        self.api_connector = api_connector
+        self._graph = None
+        self._ds_response = None
+        self._process_keys = []
+
+    @property
+    def exists(self):
+        """Check if the project exists"""
+        response_project_exist = self.api_connector.get_request(f"/project/{self.id}/exist").json()
+        return response_project_exist["exists"]
+
+    def delete_project(self):
+        """Deletes the project"""
+        response_project_delete = self.api_connector.delete_request(f"/project/{self.id}")
+        return response_project_delete
+
+    def get_project_name(self):
+        """Returns the name of the project"""
+        response_project_name = self.api_connector.get_request(f"/project/{self.id}/name").json()
+        return response_project_name["name"]
+
+    def graph(self, gateways=False):
+        """Performs a REST request for the project model graph if it hasn't already been retrieved.
+
+        :param gateways: Boolean that controls whether the graph returned will be BPMN-like or not
+        """
+        if self._graph is None:
+            params = {"mode": "gateways" if gateways else "simplified"}
+            response_graph = self.api_connector.get_request(
+                f"/project/{self.id}/graph",
+                params=params)
+            self._graph = Graph.from_dict(self.id, response_graph.json())
+        return self._graph
+
+    def get_graph_instances(self, limit=None, shuffle=False):
+        """Returns all the project's Graph Instances, performing a REST request for any instances that don't already
+        exist within the project.
+
+        :param limit: the maximum number of graph instances to return
+        :param shuffle: whether to shuffle the list of graph instances with a default value set to False
+        """
+        limit = min(limit, len(self.process_keys)) if limit is not None else len(self.process_keys)
+        sample = random.sample(self.process_keys, limit) if shuffle else self.process_keys[:limit]
+        return [self.graph_instance_from_key(k) for k in sample]
+
+    def graph_instance_from_key(self, process_id):
+        """Performs a REST request for the graph instance associated with a process key, and returns it.
+
+        :param process_id: the id of the process whose graph we want to get
+        """
+        parameters = {"processId": process_id}
+        response_graph_instance = None
+        try:
+            response_graph_instance = self.api_connector.get_request(
+                f"/project/{self.id}/graphInstance",
+                params=parameters)
+            graph = response_graph_instance.json()
+            graph_instance = GraphInstance.from_dict(self.id, graph)
+        except Exception as error:
+            print(f"Could not parse graph: {error}")
+            print(response_graph_instance)
+            return None
+        return graph_instance
+
+    def __datasource_request(self):
+        """Request datasources associated with the project"""
+
+        response_datasource = self.api_connector.get_request(f"/datasources/{self.id}")
+        return response_datasource.json()
+
+    @property
+    def nodes_datasource(self):
+        """Returns datasource of type '_vertex'"""
+        return self.__get_datasource_by_name('_vertex')
+
+    @property
+    def edges_datasource(self):
+        """Returns datasource of type '_simplifiedEdge'"""
+        return self.__get_datasource_by_name('_simplifiedEdge')
+
+
+    @property
+    def cases_datasource(self):
+        """Returns datasource of type 'cases'"""
+        return self.__get_datasource_by_name('cases')
+
+    def __get_datasource_by_name(self, ds_type):
+        """Helper method that filters the datasources based on the given type
+
+        :param ds_type: The type of datasource. Can be 'cases', '_simplifiedEdge' or '_vertex'
+        """
+        self._ds_response = self.__datasource_request() if self._ds_response is None else self._ds_response
+
+        for item in self._ds_response:
+            if "_simplifiedEdge" in item["name"]:
+                item["type"] = "_simplifiedEdge"
+            elif "_vertex" in item["name"]:
+                item["type"] = "_vertex"
+            else:
+                item["type"] = "cases"
+
+        response_filtered = [d for d in self._ds_response if d['type'] == ds_type][0]
+        return Datasource(
+            response_filtered["name"],
+            response_filtered["type"],
+            response_filtered["host"],
+            response_filtered["port"],
+            self.api_connector)
+
+    def get_project_variants(self, page_index: int, limit: int, search: str = None):
+        """Returns the project variants
+
+        :param page_index: the page index for pagination
+        :param limit: The maximum number of items to return per page
+        :param search: The search query to filter variants by name (optional)
+        """
+        params = {"projectId": self.id, "pageIndex": page_index, "limit": limit}
+        if search is not None:
+            params["search"] = search
+
+        route = f"/project/{self.id}/variants"
+        response_variants = self.api_connector.get_request(route, params=params)
+        return response_variants.json()
+
+    def get_project_completed_cases(self, page_index: int, limit: int, search_case_id: str = None):
+        """Returns the projects completed cases
+
+        :param page_index: the page index for pagination
+        :param limit: The maximum number of items to return per page
+        :param search: The search query to filter cases by ID (optional)
+
+        """
+        params = {"projectId": self.id, "pageIndex": page_index, "limit": limit}
+        if search_case_id is not None:
+            params["searchCaseId"] = search_case_id
+
+        route = f"/project/{self.id}/completedCases"
+        response_case_ids = self.api_connector.get_request(route, params=params)
+        return response_case_ids.json()
+
+    @property
+    def process_keys(self):
+        """Queries the datasources to find the different process keys of the project"""
+
+        if len(self._process_keys) == 0:
+            ds = self.edges_datasource
+            res = ds.request(f"SELECT DISTINCT processkey FROM \"{ds.name}\"")
+            self._process_keys = [key for key in res['processkey']]
+
+        return self._process_keys
+
+    def add_column_mapping(self, filestructure: FileStructure, columnmapping: ColumnMapping):
+        """Create a column mapping for the project
+
+        :param filestructure: the filestructure
+        :param columnmapping: the columnmapping
+        """
+        route = f"/project/{self.id}/column-mapping"
+        json = {'fileStructure': filestructure.to_dict(), 'columnMapping': columnmapping.to_dict()}
+        response_column_mapping = self.api_connector.post_request(route, json=json)
+        return response_column_mapping.status_code == 204
+
+    @property
+    def column_mapping_exists(self):
+        """Check if a column mapping exists"""
+
+        json_response = self.api_connector.get_request(f"/project/{self.id}/column-mapping-exists")
+        return json_response.json()['exists']
+
+    def get_mapping_infos(self):
+        """Returns the mapping infos of the project such as the column names"""
+
+        response_mapping_infos = self.api_connector.get_request(f"/project/{self.id}/mappingInfos").json()
+        return response_mapping_infos
+
+    def reset(self):
+        """Makes an API call to manually reset a project"""
+
+        response_reset = self.api_connector.post_request(f"/project/{self.id}/reset")
+        return response_reset.status_code == 204
+
+    def add_file(self, path):
+        """Adds a file to the project
+
+        :param path: the path to the file to add
+        """
+        route = f"/project/{self.id}/file?teamId={self.api_connector.wg_id}"
+        file_extension = os.path.splitext(path)[-1].lower()
+        if file_extension == ".csv":
+            mime_type = "text/csv"
+        elif file_extension == ".xlsx":
+            mime_type = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
+        elif file_extension == ".xls":
+            mime_type = "application/vnd.ms-excel"
+        else:
+            raise ValueError(f"File extension {file_extension} is not supported")
+
+        with open(path, 'rb') as file:
+            files = {'file': (os.path.basename(path), file, mime_type)}
+            headers = {"accept": "application/json, text/plain, */*"}
+            response_add_file = self.api_connector.post_request(route, files=files, headers=headers)
+
+        print(response_add_file)
+        return response_add_file.status_code == 201
+
+    @property
+    def train_status(self):
+        """Returns True if the train is currently running, False otherwise"""
+        json_response = self.api_connector.get_request(f"/train/{self.id}")
+        return json_response["isTrainRunning"]
+
+    def launch_train(self):
+        """Makes an API call to manually launch the train of a project"""
+        self.api_connector.post_request(f"/train/{self.id}/launch")
+
+    def stop_train(self):
+        """Makes an API call to manually stop the train of a project"""
+        self.api_connector.delete_request(f"/train/{self.id}")
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/workgroup.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-import requests as req
-from igrafx_mining_sdk.project import Project
-from igrafx_mining_sdk.api_connector import APIConnector
-
-
-class Workgroup:
-    """A iGrafx P360 Live Mining workgroup, which is used to log in and access projects"""
-
-    def __init__(self, w_id: str, w_key: str, apiurl: str, authurl: str, ssl_verify=True):
-        """ Creates a iGrafx P360 Live Mining Workgroup and automatically logs into the iMining Public API using the provided client id and
-        secret key
-
-        :param w_id: the workgroup ID, which can be found in iGrafx P360 Live Mining
-        :param w_key: the workgroup's secret key, used for authetication, also found in iGrafx P360 Live Mining
-        :param apiurl: the URL of the api found in iGrafx P360 Live Mining
-        :param authurl: the URL of the authentication found in iGrafx P360 Live Mining
-        :param ssl_verify: verify SSL certificates
-        """
-        self.w_id = w_id
-        self.w_key = w_key
-        self._datasources = []
-        self.api_connector = APIConnector(w_id, w_key, apiurl, authurl, ssl_verify)
-
-    def get_project_list(self):
-        """Returns a list of all projects in the workgroup"""
-        response_project_list = self.api_connector.get_request("/projects").json()
-        return response_project_list
-
-    def create_project(self, project_name: str, description: str = None):
-        """Creates a project within the workgroup"""
-
-        params = {"name": project_name, "workgroupId": self.w_id}
-        if description is not None:
-            params["description"] = description
-
-        route = f"/project"
-        response_project_creation = self.api_connector.post_request(route, params=params)
-
-        if response_project_creation.status_code == 201:
-            created_project = Project(response_project_creation.json()["message"], self.api_connector)
-            return created_project
-        else:
-            raise ValueError(f"Failed to create project. Status code: {response_project_creation.status_code}")
-
-    @property
-    def datasources(self):
-        """Requests and returns the list of datasources associated with the workgroup"""
-        try:
-            self._datasources = []
-            for p_id in self.get_project_list():
-                project = self.project_from_id(p_id)
-                if project:
-                    self._datasources.append(project.nodes_datasource)
-                    self._datasources.append(project.edges_datasource)
-                    self._datasources.append(project.cases_datasource)
-
-        except req.HTTPError as error:
-            print(f"HTTP Error occurred: {error}")
-
-        return self._datasources
-
-    def project_from_id(self, pid):
-        """Returns a project based on its id, or None if no such project exists
-
-        :param pid: the id of the project"""
-        p = Project(pid, self.api_connector)
-        return p if p.exists else None
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+import requests as req
+from igrafx_mining_sdk.project import Project
+from igrafx_mining_sdk.api_connector import APIConnector
+
+
+class Workgroup:
+    """A iGrafx P360 Live Mining workgroup, which is used to log in and access projects"""
+
+    def __init__(self, w_id: str, w_key: str, apiurl: str, authurl: str, ssl_verify=True):
+        """ Creates a iGrafx P360 Live Mining Workgroup and automatically logs into the iMining Public API using the provided client id and
+        secret key
+
+        :param w_id: the workgroup ID, which can be found in iGrafx P360 Live Mining
+        :param w_key: the workgroup's secret key, used for authetication, also found in iGrafx P360 Live Mining
+        :param apiurl: the URL of the api found in iGrafx P360 Live Mining
+        :param authurl: the URL of the authentication found in iGrafx P360 Live Mining
+        :param ssl_verify: verify SSL certificates
+        """
+        self.w_id = w_id
+        self.w_key = w_key
+        self._datasources = []
+        self.api_connector = APIConnector(w_id, w_key, apiurl, authurl, ssl_verify)
+
+    def get_project_list(self):
+        """Returns a list of all projects in the workgroup"""
+        response_project_list = self.api_connector.get_request("/projects").json()
+        return response_project_list
+
+    def create_project(self, project_name: str, description: str = None):
+        """Creates a project within the workgroup"""
+
+        params = {"name": project_name, "workgroupId": self.w_id}
+        if description is not None:
+            params["description"] = description
+
+        route = f"/project"
+        response_project_creation = self.api_connector.post_request(route, params=params)
+
+        if response_project_creation.status_code == 201:
+            created_project = Project(response_project_creation.json()["message"], self.api_connector)
+            return created_project
+        else:
+            raise ValueError(f"Failed to create project. Status code: {response_project_creation.status_code}")
+
+    @property
+    def datasources(self):
+        """Requests and returns the list of datasources associated with the workgroup"""
+        try:
+            self._datasources = []
+            for p_id in self.get_project_list():
+                project = self.project_from_id(p_id)
+                if project:
+                    self._datasources.append(project.nodes_datasource)
+                    self._datasources.append(project.edges_datasource)
+                    self._datasources.append(project.cases_datasource)
+
+        except req.HTTPError as error:
+            print(f"HTTP Error occurred: {error}")
+
+        return self._datasources
+
+    def project_from_id(self, pid):
+        """Returns a project based on its id, or None if no such project exists
+
+        :param pid: the id of the project"""
+        p = Project(pid, self.api_connector)
+        return p if p.exists else None
```

### Comparing `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/SOURCES.txt` & `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.2/pyproject.toml` & `igrafx_mining_sdk-2.24.4/pyproject.toml`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[tool.poetry]
-name = "igrafx_mining_sdk"
-version = "2.24.2"
-description = "The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects."
-authors = ["iGrafx <contact@igrafx.com>"]
-license = "MIT"
-readme = "README.md"
-#packages = [{ include = "igrafx_mining_sdk" , from = "igrafx_mining_sdk" }]
-homepage = "https://www.grafx.com/"
-repository = "https://github.com/igrafx/mining-python-sdk"
-keywords = ["process mining"]
-
-[tool.poetry.dependencies]
-python = "^3.7.1,<3.11"
-requests = "2.29.0"
-pydruid = "0.6.5"
-pandas = "1.3.5"
-SQLAlchemy = "2.0.12"
-networkx = "2.6.3"
-numpy = "1.21.6"
-toml = "0.10.2"
-python-dotenv = "0.19.2"
-
-[tool.poetry.group.test.dependencies]
-pytest = "7.3.1"
-pytest-dependency = "0.5.1"
-
-
-[tool.pytest.ini_options]
-pythonpath = "igrafx_mining_sdk"
-testpaths = ["tests"]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "igrafx_mining_sdk"
+version = "2.24.2"
+description = "The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects."
+authors = ["iGrafx <contact@igrafx.com>"]
+license = "MIT"
+readme = "README.md"
+#packages = [{ include = "igrafx_mining_sdk" , from = "igrafx_mining_sdk" }]
+homepage = "https://www.grafx.com/"
+repository = "https://github.com/igrafx/mining-python-sdk"
+keywords = ["process mining"]
+
+[tool.poetry.dependencies]
+python = "^3.7.1,<3.11"
+requests = "2.29.0"
+pydruid = "0.6.5"
+pandas = "1.3.5"
+SQLAlchemy = "2.0.12"
+networkx = "2.6.3"
+numpy = "1.21.6"
+toml = "0.10.2"
+python-dotenv = "0.19.2"
+
+[tool.poetry.group.test.dependencies]
+pytest = "7.3.1"
+pytest-dependency = "0.5.1"
+
+
+[tool.pytest.ini_options]
+pythonpath = "igrafx_mining_sdk"
+testpaths = ["tests"]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `igrafx_mining_sdk-2.24.2/setup.py` & `igrafx_mining_sdk-2.24.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from setuptools import setup, find_packages
-import toml
-import re
-
-# Parse pyproject.toml file
-with open('./pyproject.toml', 'r') as f:
-    pyproject_data = toml.load(f)
-
-# Extract package information
-package_infos = {
-    "__author__": pyproject_data['tool']['poetry']['authors'][0].split('<')[0].rstrip(),
-    "__version__": pyproject_data['tool']['poetry']['version'],
-    "__doc__": pyproject_data['tool']['poetry']['description'],
-    "__email__": re.findall("[0-9a-zA-z]+@[0-9a-zA-z]+\.[0-9a-zA-z]+", pyproject_data['tool']['poetry']['authors'][0])[0]
-}
-
-# Extract requirements
-requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
-
-setup(
-    name="igrafx_mining_sdk",
-    version=package_infos['__version__'],
-    description=package_infos['__doc__'],
-    url="https://www.logpickr.com/fr/accueil.html",
-    author=package_infos['__author__'],
-    author_email=package_infos['__email__'],
-    packages=find_packages(),    #["igrafx_mining_sdk"],
-    licence="Apache License 2.0"
-)
+from setuptools import setup, find_packages
+import toml
+import re
+
+# Parse pyproject.toml file
+with open('./pyproject.toml', 'r') as f:
+    pyproject_data = toml.load(f)
+
+# Extract package information
+package_infos = {
+    "__author__": pyproject_data['tool']['poetry']['authors'][0].split('<')[0].rstrip(),
+    "__version__": pyproject_data['tool']['poetry']['version'],
+    "__doc__": pyproject_data['tool']['poetry']['description'],
+    "__email__": re.findall("[0-9a-zA-z]+@[0-9a-zA-z]+\.[0-9a-zA-z]+", pyproject_data['tool']['poetry']['authors'][0])[0]
+}
+
+# Extract requirements
+requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
+
+setup(
+    name="igrafx_mining_sdk",
+    version='2.24.4',
+    description=package_infos['__doc__'],
+    long_description=open("README.md", 'r').read(),
+    long_description_content_type='text/markdown',
+    url="https://www.logpickr.com/fr/accueil.html",
+    author=package_infos['__author__'],
+    author_email=package_infos['__email__'],
+    packages=find_packages(),
+    licence="Apache License 2.0"
+)
```

### Comparing `igrafx_mining_sdk-2.24.2/tests/test_datasource.py` & `igrafx_mining_sdk-2.24.4/tests/test_datasource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-from pathlib import Path
-import pytest
-from igrafx_mining_sdk.project import Project
-from igrafx_mining_sdk.datasource import Datasource
-from igrafx_mining_sdk.workgroup import Workgroup
-from dotenv import load_dotenv
-import os
-
-# Load environment variables from .env file
-dotenv_path = Path(__file__).parent.parent / '.env'
-load_dotenv(dotenv_path)
-
-NAME = os.environ.get('NAME')
-TYPE = os.environ.get('TYPE')
-HOST = os.environ.get('HOST')
-PORT = os.environ.get('PORT')
-
-wg_id = os.environ.get('WG_ID')
-wg_key = os.environ.get('WG_KEY')
-wg_url = os.environ.get('WG_URL')
-wg_auth = os.environ.get('WG_AUTH')
-project_id = os.environ.get('PROJECT_ID')
-
-
-class TestDatasource:
-    """Class for testing Datasource class.
-    Workgroup and project are pytest fixtures defined in conftest.py file.
-    """
-
-    def test_create_datasource(self, workgroup):
-        """Test creating a Datasource"""
-        ds = Datasource(NAME, TYPE, HOST, PORT, workgroup.api_connector)
-        assert isinstance(ds, Datasource)
-
-    def test_columns(self, workgroup, project):
-        """Test the columns of a Datasource"""
-
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        p = Project(project_id, w.api_connector)
-        ds = p.edges_datasource
-        assert ds.columns != []
-
-    def test_non_empty_ds(self):
-        """Test that the datasource is not empty"""
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        for pr in w.get_project_list():
-            try:
-                len(pr.process_keys)
-                project = pr
-                break
-            except Exception:
-                continue
-
-        ds = project.nodes_datasource
-        assert 0 < len(ds.load_dataframe(load_limit=10)) <= 10
-
-    def test_read_only(self):
-        """Test that the datasource is read only"""
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        for pr in w.get_project_list():
-            try:
-                len(pr.process_keys)
-                project = pr
-                break
-            except Exception:
-                continue
-
-        ds = project.edges_datasource
-        pk = project.process_keys[0]
-        # Test that all of those requests will fail
-        with pytest.raises(Exception):
-            assert ds.request(f'DELETE FROM "{ds.name}" WHERE processkey = \'{pk}\'')
-        with pytest.raises(Exception):
-            assert ds.request(f'INSERT INTO "{ds.name}"(processkey) VALUES (\'{pk}\')')
-        with pytest.raises(Exception):
-            assert ds.request(f'DROP TABLE "{ds.name}"')
-            ds.drop()
-        with pytest.raises(Exception):
-            assert ds.request(f'ALTER TABLE "{ds.name}" DROP COLUMN processkey')
-
-    def test_close(self, workgroup, project):
-        """Test that the Datasource can be closed"""
-        ds = Datasource(NAME, TYPE, HOST, PORT, workgroup.api_connector)
-        # ensure connection and cursor are none
-        assert ds._cursor is None
-        assert ds._connection is None
-
-        # initialize both cursor and connection
-        cursor = ds.cursor
-        connection = ds.connection
-        assert cursor is not None
-        assert connection is not None
-
-        # close cursor and connection then check that they are none again
-        ds.close()
-        assert ds._cursor is None
-        assert ds._connection is None
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+from pathlib import Path
+import pytest
+from igrafx_mining_sdk.project import Project
+from igrafx_mining_sdk.datasource import Datasource
+from igrafx_mining_sdk.workgroup import Workgroup
+from dotenv import load_dotenv
+import os
+
+# Load environment variables from .env file
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
+
+NAME = os.environ.get('NAME')
+TYPE = os.environ.get('TYPE')
+HOST = os.environ.get('HOST')
+PORT = os.environ.get('PORT')
+
+wg_id = os.environ.get('WG_ID')
+wg_key = os.environ.get('WG_KEY')
+wg_url = os.environ.get('WG_URL')
+wg_auth = os.environ.get('WG_AUTH')
+project_id = os.environ.get('PROJECT_ID')
+
+
+class TestDatasource:
+    """Class for testing Datasource class.
+    Workgroup and project are pytest fixtures defined in conftest.py file.
+    """
+
+    def test_create_datasource(self, workgroup):
+        """Test creating a Datasource"""
+        ds = Datasource(NAME, TYPE, HOST, PORT, workgroup.api_connector)
+        assert isinstance(ds, Datasource)
+
+    def test_columns(self):
+        """Test the columns of a Datasource"""
+
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        p = Project(project_id, w.api_connector)
+        ds = p.edges_datasource
+        assert ds.columns != []
+
+    def test_non_empty_ds(self):
+        """Test that the datasource is not empty"""
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        for pr in w.get_project_list():
+            try:
+                len(pr.process_keys)
+                project = pr
+                break
+            except Exception:
+                continue
+
+        ds = project.nodes_datasource
+        assert 0 < len(ds.load_dataframe(load_limit=10)) <= 10
+
+    def test_read_only(self):
+        """Test that the datasource is read only"""
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        for pr in w.get_project_list():
+            try:
+                len(pr.process_keys)
+                project = pr
+                break
+            except Exception:
+                continue
+
+        ds = project.edges_datasource
+        pk = project.process_keys[0]
+        # Test that all of those requests will fail
+        with pytest.raises(Exception):
+            assert ds.request(f'DELETE FROM "{ds.name}" WHERE processkey = \'{pk}\'')
+        with pytest.raises(Exception):
+            assert ds.request(f'INSERT INTO "{ds.name}"(processkey) VALUES (\'{pk}\')')
+        with pytest.raises(Exception):
+            assert ds.request(f'DROP TABLE "{ds.name}"')
+            ds.drop()
+        with pytest.raises(Exception):
+            assert ds.request(f'ALTER TABLE "{ds.name}" DROP COLUMN processkey')
+
+    def test_close(self, workgroup, project):
+        """Test that the Datasource can be closed"""
+        ds = Datasource(NAME, TYPE, HOST, PORT, workgroup.api_connector)
+        # ensure connection and cursor are none
+        assert ds._cursor is None
+        assert ds._connection is None
+
+        # initialize both cursor and connection
+        cursor = ds.cursor
+        connection = ds.connection
+        assert cursor is not None
+        assert connection is not None
+
+        # close cursor and connection then check that they are none again
+        ds.close()
+        assert ds._cursor is None
+        assert ds._connection is None
```

### Comparing `igrafx_mining_sdk-2.24.2/tests/test_graph.py` & `igrafx_mining_sdk-2.24.4/tests/test_graph.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-from pathlib import Path
-import pytest
-from igrafx_mining_sdk.project import Project
-from igrafx_mining_sdk.workgroup import Workgroup
-from igrafx_mining_sdk.graph import Graph
-from dotenv import load_dotenv
-import os
-
-# Load environment variables from .env file
-dotenv_path = Path(__file__).parent.parent / '.env'
-load_dotenv(dotenv_path)
-
-wg_id = os.environ.get('WG_ID')
-wg_key = os.environ.get('WG_KEY')
-wg_url = os.environ.get('WG_URL')
-wg_auth = os.environ.get('WG_AUTH')
-project_id = os.environ.get('PROJECT_ID')
-
-
-class TestGraph:
-    """Tests for the Graph class.
-    Workgroup and project are pytest fixtures defined in conftest.py file.
-    """
-    def test_graph_creation(self, workgroup, project):
-        """Test the creation of a Graph object."""
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        g = project.graph()
-        assert isinstance(g, Graph)
-
-    def test_graph_instance(self):
-        """Test the creation of a Graph object."""
-        # Test with another project because indexation time returns error
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        g = project.get_graph_instances(limit=1)[0]
-        assert g.rework_total is not None
-        assert g.concurrency_rate is not None
-
-    def test_graph_with_bad_edges(self):
-        """Test a graph that has bad edges."""
-        base_dir = Path(__file__).resolve().parent
-        file_path = base_dir / 'data' / 'graphs' / 'graph_with_invalid_edges.json'
-        with pytest.raises(Exception):
-            assert Graph.from_json(14, str(file_path))
-
-    def test_from_json(self):
-        """Test the creation of a Graph object from a json string and display."""
-        base_dir = Path(__file__).resolve().parent
-        file_path = base_dir / 'data' / 'graphs' / 'graph.json'
-        g = Graph.from_json(0, str(file_path))
-        assert len(g) > 0
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+from pathlib import Path
+import pytest
+from igrafx_mining_sdk.project import Project
+from igrafx_mining_sdk.workgroup import Workgroup
+from igrafx_mining_sdk.graph import Graph
+from dotenv import load_dotenv
+import os
+
+# Load environment variables from .env file
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
+
+wg_id = os.environ.get('WG_ID')
+wg_key = os.environ.get('WG_KEY')
+wg_url = os.environ.get('WG_URL')
+wg_auth = os.environ.get('WG_AUTH')
+project_id = os.environ.get('PROJECT_ID')
+
+
+class TestGraph:
+    """Tests for the Graph class.
+    Workgroup and project are pytest fixtures defined in conftest.py file.
+    """
+    def test_graph_creation(self, workgroup, project):
+        """Test the creation of a Graph object."""
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        g = project.graph()
+        assert isinstance(g, Graph)
+
+    def test_graph_instance(self):
+        """Test the creation of a Graph object."""
+        # Test with another project because indexation time returns error
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        g = project.get_graph_instances(limit=1)[0]
+        assert g.rework_total is not None
+        assert g.concurrency_rate is not None
+
+    def test_graph_with_bad_edges(self):
+        """Test a graph that has bad edges."""
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'graphs' / 'graph_with_invalid_edges.json'
+        with pytest.raises(Exception):
+            assert Graph.from_json(14, str(file_path))
+
+    def test_from_json(self):
+        """Test the creation of a Graph object from a json string and display."""
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'graphs' / 'graph.json'
+        g = Graph.from_json(0, str(file_path))
+        assert len(g) > 0
```

### Comparing `igrafx_mining_sdk-2.24.2/tests/test_project.py` & `igrafx_mining_sdk-2.24.4/tests/test_project.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-# MIT License, Copyright 2023 iGrafx
-# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
-from pathlib import Path
-from igrafx_mining_sdk.project import Project, FileStructure
-from igrafx_mining_sdk.column_mapping import Column, ColumnType, ColumnMapping, FileType
-from igrafx_mining_sdk.datasource import Datasource
-from igrafx_mining_sdk.workgroup import Workgroup
-import pytest
-from dotenv import load_dotenv
-import os
-
-# Load environment variables from .env file
-dotenv_path = Path(__file__).parent.parent / '.env'
-load_dotenv(dotenv_path)
-
-wg_id = os.environ.get('WG_ID')
-wg_key = os.environ.get('WG_KEY')
-wg_url = os.environ.get('WG_URL')
-wg_auth = os.environ.get('WG_AUTH')
-project_id = os.environ.get('PROJECT_ID')
-
-
-class TestProject:
-    """Tests for Project class.
-    Workgroup and project are pytest fixtures defined in conftest.py file.
-    """
-
-    def test_project_exists(self, workgroup, project):
-        """Test that a project exists."""
-        project_exists = project.exists
-        assert project_exists is True
-
-    def test_init_project(self, workgroup, project):
-        """Test initialization of a project."""
-        assert isinstance(project, Project)
-
-    def test_get_project_name(self, workgroup, project):
-        """ Test that the project name is returned and correct."""
-        project_name = project.get_project_name()
-        assert project_name == "Test Project"
-
-    @pytest.mark.dependency()
-    def test_reset(self, workgroup, project):
-        """Test that a project can be reset."""
-        assert project.reset()
-
-    @pytest.mark.dependency(depends=["TestProject::test_reset"])  # Will skip test if test_reset fails
-    def test_add_column_mapping(self, workgroup, project):
-        """Test that a column mapping can be created."""
-        filestructure = FileStructure(
-            file_type=FileType.xlsx,
-            sheet_name="Sheet1"
-        )
-        column_list = [
-            Column('case_id', 0, ColumnType.CASE_ID),
-            Column('task_name', 1, ColumnType.TASK_NAME),
-            Column('time', 2, ColumnType.TIME, time_format='%Y-%m-%dT%H:%M')
-        ]
-        column_mapping = ColumnMapping(column_list)
-        assert project.add_column_mapping(filestructure, column_mapping)
-
-    def test_column_mapping_exists(self, workgroup, project):
-        """Test that a column mapping can be created."""
-        assert project.column_mapping_exists
-
-    def test_get_mapping_infos(self, workgroup, project):
-        """Test that the correct mapping infos can be returned"""
-        assert project.get_mapping_infos()
-
-    def test_add_csv_file(self, workgroup, project):
-        """Test that a csv file can be added to a project."""
-        project.reset()
-        filestructure = FileStructure(
-            file_type=FileType.csv,
-        )
-        column_list = [
-            Column('Case ID', 0, ColumnType.CASE_ID),
-            Column('Activity', 1, ColumnType.TASK_NAME),
-            Column('Start Date', 2, ColumnType.TIME, time_format='%d/%m/%Y %H:%M'),
-            Column('End Date', 3, ColumnType.TIME, time_format='%d/%m/%Y %H:%M'),
-        ]
-        column_mapping = ColumnMapping(column_list)
-        base_dir = Path(__file__).resolve().parent
-        file_path = base_dir / 'data' / 'tables' / 'testdata.csv'
-        assert project.add_column_mapping(filestructure, column_mapping)
-        assert project.add_file(str(file_path))
-
-    def test_add_xlsx_file(self, workgroup, project):
-        """Test that an xlsx file can be added to a project."""
-        project.reset()
-        filestructure = FileStructure(
-            file_type=FileType.xlsx,
-            sheet_name="Sheet1"
-        )
-        column_list = [
-            Column('Case ID', 0, ColumnType.CASE_ID),
-            Column('Start Timestamp', 1, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
-            Column('Complete Timestamp', 2, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
-            Column('Activity', 3, ColumnType.TASK_NAME),
-            Column('Ressource', 4, ColumnType.DIMENSION),
-        ]
-        column_mapping = ColumnMapping(column_list)
-        base_dir = Path(__file__).resolve().parent
-        file_path = base_dir / 'data' / 'tables' / 'p2pShortExcel.xlsx'
-        assert project.add_column_mapping(filestructure, column_mapping)
-        assert project.add_file(str(file_path))
-
-    def test_add_xls_file(self, workgroup, project):
-        """Test that an xls file can be added to a project."""
-        project.reset()
-        filestructure = FileStructure(
-            file_type=FileType.xls,
-            sheet_name="Sheet1"
-        )
-        column_list = [
-            Column('Case ID', 0, ColumnType.CASE_ID),
-            Column('Start Timestamp', 1, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
-            Column('Complete Timestamp', 2, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
-            Column('Activity', 3, ColumnType.TASK_NAME),
-            Column('Ressource', 4, ColumnType.DIMENSION),
-        ]
-        column_mapping = ColumnMapping(column_list)
-        base_dir = Path(__file__).resolve().parent
-        file_path = base_dir / 'data' / 'tables' / 'p2pShortExcel.xls'
-        assert project.add_column_mapping(filestructure, column_mapping)
-        assert project.add_file(str(file_path))
-
-    def test_graph(self, workgroup, project):
-        """Test the creation of a graph."""
-        assert project.graph is not None
-
-    def test_graph_instances(self):
-        """Test the graph instances."""
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        print(project_id)
-        assert len(project.get_graph_instances(limit=3, shuffle=False)) == 2
-        assert len(project.get_graph_instances(limit=3, shuffle=True)) == 2
-
-    def test_datasources_types(self):
-        """Test the types of the datasources"""
-        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
-        project = Project(project_id, w.api_connector)
-        assert project.nodes_datasource.__class__ == Datasource
-        assert project.edges_datasource.__class__ == Datasource
-        assert project.cases_datasource.__class__ == Datasource
-
-    def test_get_project_variants(self, workgroup, project):
-        """Test that the project correct variants are returned."""
-        assert project.get_project_variants(1, 3)
-
-    def test_get_project_completed_cases(self, project):
-        """Test that the projects correct completed cases are returned."""
-        # No Search Case ID
-        assert project.get_project_completed_cases(1, 3)
-        # With Search Case ID
-        assert project.get_project_completed_cases(1, 3, "IF-1609205")
-
-
-
+# MIT License, Copyright 2023 iGrafx
+# https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+
+from pathlib import Path
+from igrafx_mining_sdk.project import Project, FileStructure
+from igrafx_mining_sdk.column_mapping import Column, ColumnType, ColumnMapping, FileType
+from igrafx_mining_sdk.datasource import Datasource
+from igrafx_mining_sdk.workgroup import Workgroup
+import pytest
+from dotenv import load_dotenv
+import os
+
+# Load environment variables from .env file
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
+
+wg_id = os.environ.get('WG_ID')
+wg_key = os.environ.get('WG_KEY')
+wg_url = os.environ.get('WG_URL')
+wg_auth = os.environ.get('WG_AUTH')
+project_id = os.environ.get('PROJECT_ID')
+
+
+class TestProject:
+    """Tests for Project class.
+    Workgroup and project are pytest fixtures defined in conftest.py file.
+    """
+
+    def test_project_exists(self, workgroup, project):
+        """Test that a project exists."""
+        project_exists = project.exists
+        assert project_exists is True
+
+    def test_init_project(self, workgroup, project):
+        """Test initialization of a project."""
+        assert isinstance(project, Project)
+
+    def test_get_project_name(self, workgroup, project):
+        """ Test that the project name is returned and correct."""
+        project_name = project.get_project_name()
+        assert project_name == "Test Project"
+
+    @pytest.mark.dependency()
+    def test_reset(self, workgroup, project):
+        """Test that a project can be reset."""
+        assert project.reset()
+
+    @pytest.mark.dependency(depends=["TestProject::test_reset"])  # Will skip test if test_reset fails
+    def test_add_column_mapping(self, workgroup, project):
+        """Test that a column mapping can be created."""
+        filestructure = FileStructure(
+            file_type=FileType.xlsx,
+            sheet_name="Sheet1"
+        )
+        column_list = [
+            Column('case_id', 0, ColumnType.CASE_ID),
+            Column('task_name', 1, ColumnType.TASK_NAME),
+            Column('time', 2, ColumnType.TIME, time_format='%Y-%m-%dT%H:%M')
+        ]
+        column_mapping = ColumnMapping(column_list)
+        assert project.add_column_mapping(filestructure, column_mapping)
+
+    def test_column_mapping_exists(self, workgroup, project):
+        """Test that a column mapping can be created."""
+        assert project.column_mapping_exists
+
+    def test_get_mapping_infos(self, workgroup, project):
+        """Test that the correct mapping infos can be returned"""
+        assert project.get_mapping_infos()
+
+    def test_add_csv_file(self, workgroup, project):
+        """Test that a csv file can be added to a project."""
+        project.reset()
+        filestructure = FileStructure(
+            file_type=FileType.csv,
+        )
+        column_list = [
+            Column('Case ID', 0, ColumnType.CASE_ID),
+            Column('Activity', 1, ColumnType.TASK_NAME),
+            Column('Start Date', 2, ColumnType.TIME, time_format='%d/%m/%Y %H:%M'),
+            Column('End Date', 3, ColumnType.TIME, time_format='%d/%m/%Y %H:%M'),
+        ]
+        column_mapping = ColumnMapping(column_list)
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'tables' / 'testdata.csv'
+        assert project.add_column_mapping(filestructure, column_mapping)
+        assert project.add_file(str(file_path))
+
+    def test_add_xlsx_file(self, workgroup, project):
+        """Test that an xlsx file can be added to a project."""
+        project.reset()
+        filestructure = FileStructure(
+            file_type=FileType.xlsx,
+            sheet_name="Sheet1"
+        )
+        column_list = [
+            Column('Case ID', 0, ColumnType.CASE_ID),
+            Column('Start Timestamp', 1, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
+            Column('Complete Timestamp', 2, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
+            Column('Activity', 3, ColumnType.TASK_NAME),
+            Column('Ressource', 4, ColumnType.DIMENSION),
+        ]
+        column_mapping = ColumnMapping(column_list)
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'tables' / 'p2pShortExcel.xlsx'
+        assert project.add_column_mapping(filestructure, column_mapping)
+        assert project.add_file(str(file_path))
+
+    def test_add_xls_file(self, workgroup, project):
+        """Test that an xls file can be added to a project."""
+        project.reset()
+        filestructure = FileStructure(
+            file_type=FileType.xls,
+            sheet_name="Sheet1"
+        )
+        column_list = [
+            Column('Case ID', 0, ColumnType.CASE_ID),
+            Column('Start Timestamp', 1, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
+            Column('Complete Timestamp', 2, ColumnType.TIME, time_format='%Y/%m/%d %H:%M:%S.%f'),
+            Column('Activity', 3, ColumnType.TASK_NAME),
+            Column('Ressource', 4, ColumnType.DIMENSION),
+        ]
+        column_mapping = ColumnMapping(column_list)
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'tables' / 'p2pShortExcel.xls'
+        assert project.add_column_mapping(filestructure, column_mapping)
+        assert project.add_file(str(file_path))
+
+    def test_graph(self, workgroup, project):
+        """Test the creation of a graph."""
+        assert project.graph is not None
+
+    def test_graph_instances(self):
+        """Test the graph instances."""
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        print(project_id)
+        assert len(project.get_graph_instances(limit=3, shuffle=False)) == 2
+        assert len(project.get_graph_instances(limit=3, shuffle=True)) == 2
+
+    def test_datasources_types(self):
+        """Test the types of the datasources"""
+        w = Workgroup(wg_id, wg_key, wg_url, wg_auth)
+        project = Project(project_id, w.api_connector)
+        assert project.nodes_datasource.__class__ == Datasource
+        assert project.edges_datasource.__class__ == Datasource
+        assert project.cases_datasource.__class__ == Datasource
+
+    def test_get_project_variants(self, workgroup, project):
+        """Test that the project correct variants are returned."""
+        assert project.get_project_variants(1, 3)
+
+    def test_get_project_completed_cases(self, project):
+        """Test that the projects correct completed cases are returned."""
+        # No Search Case ID
+        assert project.get_project_completed_cases(1, 3)
+        # With Search Case ID
+        assert project.get_project_completed_cases(1, 3, "IF-1609205")
+
+
+
```

