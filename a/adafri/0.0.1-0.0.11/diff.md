# Comparing `tmp/adafri-0.0.1.tar.gz` & `tmp/adafri-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.1.tar", last modified: Tue Jul 11 19:57:42 2023, max compression
+gzip compressed data, was "adafri-0.0.11.tar", last modified: Tue Jul 11 22:02:38 2023, max compression
```

## Comparing `adafri-0.0.1.tar` & `adafri-0.0.11.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.963232 adafri-0.0.1/
--rw-r--r--   0 ibrahima   (502) staff       (20)      551 2023-07-11 19:57:42.962885 adafri-0.0.1/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.951304 adafri-0.0.1/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       50 2023-07-11 19:48:50.000000 adafri-0.0.1/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.954990 adafri-0.0.1/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:20:11.000000 adafri-0.0.1/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.1/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    12814 2023-07-11 19:22:02.000000 adafri-0.0.1/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.955906 adafri-0.0.1/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       23 2023-07-11 19:50:15.000000 adafri-0.0.1/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.956755 adafri-0.0.1/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       42 2023-07-11 19:50:47.000000 adafri-0.0.1/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.959112 adafri-0.0.1/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:36:21.000000 adafri-0.0.1/adafri/v1/auth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5254 2023-07-11 19:45:53.000000 adafri-0.0.1/adafri/v1/auth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4321 2023-07-11 19:45:25.000000 adafri-0.0.1/adafri/v1/auth/models/client_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.959961 adafri-0.0.1/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 19:52:27.000000 adafri-0.0.1/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.961887 adafri-0.0.1/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:52:05.000000 adafri-0.0.1/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9078 2023-07-11 19:46:28.000000 adafri-0.0.1/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4519 2023-07-11 19:25:49.000000 adafri-0.0.1/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:57:42.953368 adafri-0.0.1/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      551 2023-07-11 19:57:42.000000 adafri-0.0.1/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)      501 2023-07-11 19:57:42.000000 adafri-0.0.1/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-11 19:57:42.000000 adafri-0.0.1/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-11 19:57:42.000000 adafri-0.0.1/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 19:57:42.963389 adafri-0.0.1/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      999 2023-07-11 19:56:34.000000 adafri-0.0.1/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.406222 adafri-0.0.11/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:02:38.405889 adafri-0.0.11/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.391914 adafri-0.0.11/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       50 2023-07-11 19:48:50.000000 adafri-0.0.11/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.397325 adafri-0.0.11/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       79 2023-07-11 21:48:50.000000 adafri-0.0.11/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1114 2023-07-11 21:45:31.000000 adafri-0.0.11/adafri/utils/firebase_collection.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.11/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    12814 2023-07-11 19:22:02.000000 adafri-0.0.11/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.398171 adafri-0.0.11/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       40 2023-07-11 21:48:14.000000 adafri-0.0.11/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.398941 adafri-0.0.11/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       42 2023-07-11 19:50:47.000000 adafri-0.0.11/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.401030 adafri-0.0.11/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:36:21.000000 adafri-0.0.11/adafri/v1/auth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5254 2023-07-11 19:45:53.000000 adafri-0.0.11/adafri/v1/auth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4321 2023-07-11 19:45:25.000000 adafri-0.0.11/adafri/v1/auth/models/client_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.402119 adafri-0.0.11/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       21 2023-07-11 21:22:03.000000 adafri-0.0.11/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.404636 adafri-0.0.11/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-11 21:47:06.000000 adafri-0.0.11/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     8801 2023-07-11 21:51:21.000000 adafri-0.0.11/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4519 2023-07-11 19:25:49.000000 adafri-0.0.11/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.394114 adafri-0.0.11/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)      537 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 22:02:38.406365 adafri-0.0.11/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1000 2023-07-11 22:02:24.000000 adafri-0.0.11/setup.py
```

### Comparing `adafri-0.0.1/PKG-INFO` & `adafri-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adafri
-Version: 0.0.1
+Version: 0.0.11
 Summary: Adafri python module
 Home-page: UNKNOWN
 Author: Ibrahima Touré
 Author-email: ibrahima.toure.dev@gmail.com
 License: UNKNOWN
 Description: Adafri python module
 Keywords: python,first package
```

### Comparing `adafri-0.0.1/adafri/utils/response.py` & `adafri-0.0.11/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.1/adafri/utils/utils.py` & `adafri-0.0.11/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.1/adafri/v1/auth/models/client.py` & `adafri-0.0.11/adafri/v1/auth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.1/adafri/v1/auth/models/client_fields.py` & `adafri-0.0.11/adafri/v1/auth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.1/adafri/v1/user/models/user.py` & `adafri-0.0.11/adafri/v1/user/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from utils.utils import JsonEncoder, DictUtils, Crypto
+from utils import DictUtils
 from .user_fields import UserFields, UserFieldProps
+from utils import FirebaseCollectionBase
 from typing import List
 from typing import Any
 from dataclasses import dataclass
-import json
-import pydash
 
 @dataclass
 class Account:
     canManageClients: bool
     childs: List[object]
     currenyCode: str
     customerId: int
@@ -124,15 +123,15 @@
     def from_dict(obj: Any) -> 'PlateformRole':
         _id = str(DictUtils.pick(obj, "id", str))
         _partenerData = PartenerData.from_dict(DictUtils.pick(obj, "partenerData", dict))
         _text = str(DictUtils.pick(obj, "text", str))
         return PlateformRole(_id, _partenerData, _text)
 
 @dataclass
-class User:
+class User(FirebaseCollectionBase):
     account_value: int
     accounts: List[Account]
     addresse: str
     auth_code: str
     authorizedPush: bool
     country: Country
     credentials: List[Credential]
@@ -161,20 +160,17 @@
     showPushToken: bool
     telephone: str
     token: List[str]
     uid: str
     user_type: str
     password: str
     provider: str
-    collection_name = 'users';
 
-    
-    
     @staticmethod
-    def from_dict(obj: Any) -> 'User':
+    def from_dict(obj: Any, db=None, collection_name=None, fields_props=UserFieldProps) -> 'User':
         _account_value = DictUtils.pick(obj, "account_value", int)
         _accounts = [Account.from_dict(y) for y in DictUtils.pick(obj, "accounts", list)]
         _addresse = DictUtils.pick(obj, UserFields.address, str) 
         _auth_code = DictUtils.pick(obj, "auth_code", str)
         _authorizedPush = DictUtils.pick(obj, UserFields.authorizedPush, bool)
         _country = Country.from_dict(DictUtils.pick(obj, "country", dict))
         _credentials = [Credential.from_dict(y) for y in DictUtils.pick(obj, "credentials", list)]
@@ -203,26 +199,17 @@
         _showPushToken = DictUtils.pick(obj, UserFields.showPushToken, bool)
         _telephone = DictUtils.pick(obj, UserFields.telephone, str)
         _token = [y for y in DictUtils.pick(obj, UserFields.token, list)]
         _uid = DictUtils.pick(obj, UserFields.uid, str)
         _user_type = DictUtils.pick(obj, "user_type", str)
         _password = DictUtils.pick(obj, UserFields.password, str)
         _provider = DictUtils.pick(obj, UserFields.provider, str)
-        return User(_account_value, _accounts, _addresse, _auth_code, _authorizedPush, _country, _credentials, _deviceInfo, _displayName, _email, _entrepriseName, _entrepriseUrl, _first_name, _hasApprouvedPolicy, _invitedAccounts, _isConnectWithMailAndPassword, _isCorporate, _isDesktopDevice, _isMobile, _isParticular, _isTablet, _last_name, _linkedAccounts, _ownedAccounts, _phoneInfo, _photoURL, _plateformRole, _postal, _profileCompleted, _showPushToken, _telephone, _token, _uid, _user_type, _password, _provider)
-    
-    @staticmethod
-    def generate_model():
-        user = {};
-        for k in DictUtils.get_keys(UserFieldProps):
-            _key_ = 'default_value';
-            user[k] = UserFieldProps[k][_key_];
-        return user;
-
-
-    def to_json(self, fields=None):
-        if fields is None or type(fields) is not list:
-            return json.loads(JsonEncoder().encode(self));
+        _user = User(_account_value, _accounts, _addresse, _auth_code, _authorizedPush, _country, _credentials, _deviceInfo, _displayName, _email, _entrepriseName, _entrepriseUrl, _first_name, _hasApprouvedPolicy, _invitedAccounts, _isConnectWithMailAndPassword, _isCorporate, _isDesktopDevice, _isMobile, _isParticular, _isTablet, _last_name, _linkedAccounts, _ownedAccounts, _phoneInfo, _photoURL, _plateformRole, _postal, _profileCompleted, _showPushToken, _telephone, _token, _uid, _user_type, _password, _provider)
+        _user.db = db;
+        _user.collection_name = collection_name;
+        _user.fields_props = fields_props;
+        
+        return _user
     
-        return pydash.pick(json.loads(JsonEncoder().encode(self)), fields)
```

### Comparing `adafri-0.0.1/adafri/v1/user/models/user_fields.py` & `adafri-0.0.11/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.1/adafri.egg-info/PKG-INFO` & `adafri-0.0.11/adafri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adafri
-Version: 0.0.1
+Version: 0.0.11
 Summary: Adafri python module
 Home-page: UNKNOWN
 Author: Ibrahima Touré
 Author-email: ibrahima.toure.dev@gmail.com
 License: UNKNOWN
 Description: Adafri python module
 Keywords: python,first package
```

### Comparing `adafri-0.0.1/setup.py` & `adafri-0.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.11' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

