# Comparing `tmp/port_pulumi-0.9.4.tar.gz` & `tmp/port_pulumi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-0.9.4.tar", last modified: Mon Apr 17 12:16:53 2023, max compression
+gzip compressed data, was "port_pulumi-1.0.0.tar", last modified: Wed Jul 12 17:52:59 2023, max compression
```

## Comparing `port_pulumi-0.9.4.tar` & `port_pulumi-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:16:53.707849 port_pulumi-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-17 12:16:53.707849 port_pulumi-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:16:53.703849 port_pulumi-0.9.4/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:16:53.707849 port_pulumi-0.9.4/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:16:53.707849 port_pulumi-0.9.4/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:16:53.707849 port_pulumi-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-17 12:16:53.000000 port_pulumi-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70602 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33763 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55056 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/setup.py
```

### Comparing `port_pulumi-0.9.4/PKG-INFO` & `port_pulumi-1.0.0/port_pulumi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: port_pulumi
-Version: 0.9.4
+Name: port-pulumi
+Version: 1.0.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
-Project-URL: Repository, https://github.com/port-labs/pulumi
+Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
@@ -18,25 +18,24 @@
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
-
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @port-labs/pulumi
+npm install @port-labs/port
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @port-labs/pulumi
+yarn add @port-labs/port
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -44,21 +43,21 @@
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
-go get github.com/port-labs/pulumi/sdk
+go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:baseUrl` (environment: `PORT_BASE_URL`) - This is the Port base URL. 
-- `port:clientId` (environment: `PORT_CLIENT_ID`) - This is the Port client ID.
-- `port:secret` (environment: `PORT_CLIENT_SECRET`) - This is the Port secret.
-- `port:token` - This is the Port token.
+- `port:clientId` - This is the Port client ID.
+- `port:secret` - This is the Port secret.
+- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-0.9.4/README.md` & `port_pulumi-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
-
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @port-labs/pulumi
+npm install @port-labs/port
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @port-labs/pulumi
+yarn add @port-labs/port
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -32,19 +31,19 @@
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
-go get github.com/port-labs/pulumi/sdk
+go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:baseUrl` (environment: `PORT_BASE_URL`) - This is the Port base URL. 
-- `port:clientId` (environment: `PORT_CLIENT_ID`) - This is the Port client ID.
-- `port:secret` (environment: `PORT_CLIENT_SECRET`) - This is the Port secret.
-- `port:token` - This is the Port token.
+- `port:clientId` - This is the Port client ID.
+- `port:secret` - This is the Port secret.
+- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-0.9.4/port_pulumi/__init__.py` & `port_pulumi-1.0.0/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.4/port_pulumi/_utilities.py` & `port_pulumi-1.0.0/port_pulumi/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "github://api.github.com/port-labs/pulumi"
+	return "github://api.github.com/port-labs/pulumi-port"
```

### Comparing `port_pulumi-0.9.4/port_pulumi/action.py` & `port_pulumi-1.0.0/port_pulumi/entity.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,473 +7,581 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['ActionArgs', 'Action']
+__all__ = ['EntityArgs', 'Entity']
 
 @pulumi.input_type
-class ActionArgs:
+class EntityArgs:
     def __init__(__self__, *,
-                 blueprint_identifier: pulumi.Input[str],
-                 identifier: pulumi.Input[str],
-                 invocation_method: pulumi.Input['ActionInvocationMethodArgs'],
-                 title: pulumi.Input[str],
-                 trigger: pulumi.Input[str],
-                 description: Optional[pulumi.Input[str]] = None,
+                 blueprint: pulumi.Input[str],
                  icon: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]] = None):
+                 identifier: Optional[pulumi.Input[str]] = None,
+                 properties: Optional[pulumi.Input['EntityPropertiesArgs']] = None,
+                 relations: Optional[pulumi.Input['EntityRelationsArgs']] = None,
+                 run_id: Optional[pulumi.Input[str]] = None,
+                 teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 title: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Entity resource.
+        :param pulumi.Input[str] blueprint: The blueprint identifier the entity relates to
+        :param pulumi.Input[str] icon: The icon of the entity
+        :param pulumi.Input[str] identifier: The identifier of the entity
+        :param pulumi.Input['EntityPropertiesArgs'] properties: The properties of the entity
+        :param pulumi.Input['EntityRelationsArgs'] relations: The relations of the entity
+        :param pulumi.Input[str] run_id: The runID of the action run that created the entity
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: The teams the entity belongs to
+        :param pulumi.Input[str] title: The title of the entity
         """
-        The set of arguments for constructing a Action resource.
-        :param pulumi.Input[str] blueprint_identifier: The identifier of the blueprint
-        :param pulumi.Input[str] identifier: The identifier of the action
-        :param pulumi.Input['ActionInvocationMethodArgs'] invocation_method: The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
-        :param pulumi.Input[str] title: The display name of the action
-        :param pulumi.Input[str] trigger: The type of the action, one of CREATE, DAY-2, DELETE
-        :param pulumi.Input[str] description: The description of the action
-        :param pulumi.Input[str] icon: The icon of the action
-        :param pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]] user_properties: The input properties of the action
-        """
-        pulumi.set(__self__, "blueprint_identifier", blueprint_identifier)
-        pulumi.set(__self__, "identifier", identifier)
-        pulumi.set(__self__, "invocation_method", invocation_method)
-        pulumi.set(__self__, "title", title)
-        pulumi.set(__self__, "trigger", trigger)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "blueprint", blueprint)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
-        if user_properties is not None:
-            pulumi.set(__self__, "user_properties", user_properties)
+        if identifier is not None:
+            pulumi.set(__self__, "identifier", identifier)
+        if properties is not None:
+            pulumi.set(__self__, "properties", properties)
+        if relations is not None:
+            pulumi.set(__self__, "relations", relations)
+        if run_id is not None:
+            pulumi.set(__self__, "run_id", run_id)
+        if teams is not None:
+            pulumi.set(__self__, "teams", teams)
+        if title is not None:
+            pulumi.set(__self__, "title", title)
 
     @property
-    @pulumi.getter(name="blueprintIdentifier")
-    def blueprint_identifier(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def blueprint(self) -> pulumi.Input[str]:
         """
-        The identifier of the blueprint
+        The blueprint identifier the entity relates to
         """
-        return pulumi.get(self, "blueprint_identifier")
+        return pulumi.get(self, "blueprint")
 
-    @blueprint_identifier.setter
-    def blueprint_identifier(self, value: pulumi.Input[str]):
-        pulumi.set(self, "blueprint_identifier", value)
+    @blueprint.setter
+    def blueprint(self, value: pulumi.Input[str]):
+        pulumi.set(self, "blueprint", value)
 
     @property
     @pulumi.getter
-    def identifier(self) -> pulumi.Input[str]:
+    def icon(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier of the action
+        The icon of the entity
         """
-        return pulumi.get(self, "identifier")
+        return pulumi.get(self, "icon")
 
-    @identifier.setter
-    def identifier(self, value: pulumi.Input[str]):
-        pulumi.set(self, "identifier", value)
+    @icon.setter
+    def icon(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "icon", value)
 
     @property
-    @pulumi.getter(name="invocationMethod")
-    def invocation_method(self) -> pulumi.Input['ActionInvocationMethodArgs']:
+    @pulumi.getter
+    def identifier(self) -> Optional[pulumi.Input[str]]:
         """
-        The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
+        The identifier of the entity
         """
-        return pulumi.get(self, "invocation_method")
+        return pulumi.get(self, "identifier")
 
-    @invocation_method.setter
-    def invocation_method(self, value: pulumi.Input['ActionInvocationMethodArgs']):
-        pulumi.set(self, "invocation_method", value)
+    @identifier.setter
+    def identifier(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "identifier", value)
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    def properties(self) -> Optional[pulumi.Input['EntityPropertiesArgs']]:
         """
-        The display name of the action
+        The properties of the entity
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "properties")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+    @properties.setter
+    def properties(self, value: Optional[pulumi.Input['EntityPropertiesArgs']]):
+        pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter
-    def trigger(self) -> pulumi.Input[str]:
+    def relations(self) -> Optional[pulumi.Input['EntityRelationsArgs']]:
         """
-        The type of the action, one of CREATE, DAY-2, DELETE
+        The relations of the entity
         """
-        return pulumi.get(self, "trigger")
+        return pulumi.get(self, "relations")
 
-    @trigger.setter
-    def trigger(self, value: pulumi.Input[str]):
-        pulumi.set(self, "trigger", value)
+    @relations.setter
+    def relations(self, value: Optional[pulumi.Input['EntityRelationsArgs']]):
+        pulumi.set(self, "relations", value)
 
     @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="runId")
+    def run_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The description of the action
+        The runID of the action run that created the entity
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "run_id")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @run_id.setter
+    def run_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "run_id", value)
 
     @property
     @pulumi.getter
-    def icon(self) -> Optional[pulumi.Input[str]]:
+    def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The icon of the action
+        The teams the entity belongs to
         """
-        return pulumi.get(self, "icon")
+        return pulumi.get(self, "teams")
 
-    @icon.setter
-    def icon(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "icon", value)
+    @teams.setter
+    def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "teams", value)
 
     @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]]:
+    @pulumi.getter
+    def title(self) -> Optional[pulumi.Input[str]]:
         """
-        The input properties of the action
+        The title of the entity
         """
-        return pulumi.get(self, "user_properties")
+        return pulumi.get(self, "title")
 
-    @user_properties.setter
-    def user_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]]):
-        pulumi.set(self, "user_properties", value)
+    @title.setter
+    def title(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "title", value)
 
 
 @pulumi.input_type
-class _ActionState:
+class _EntityState:
     def __init__(__self__, *,
-                 blueprint_identifier: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 created_at: Optional[pulumi.Input[str]] = None,
+                 created_by: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 invocation_method: Optional[pulumi.Input['ActionInvocationMethodArgs']] = None,
+                 properties: Optional[pulumi.Input['EntityPropertiesArgs']] = None,
+                 relations: Optional[pulumi.Input['EntityRelationsArgs']] = None,
+                 run_id: Optional[pulumi.Input[str]] = None,
+                 teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]] = None):
+                 updated_at: Optional[pulumi.Input[str]] = None,
+                 updated_by: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Action resources.
-        :param pulumi.Input[str] blueprint_identifier: The identifier of the blueprint
-        :param pulumi.Input[str] description: The description of the action
-        :param pulumi.Input[str] icon: The icon of the action
-        :param pulumi.Input[str] identifier: The identifier of the action
-        :param pulumi.Input['ActionInvocationMethodArgs'] invocation_method: The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
-        :param pulumi.Input[str] title: The display name of the action
-        :param pulumi.Input[str] trigger: The type of the action, one of CREATE, DAY-2, DELETE
-        :param pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]] user_properties: The input properties of the action
-        """
-        if blueprint_identifier is not None:
-            pulumi.set(__self__, "blueprint_identifier", blueprint_identifier)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
+        Input properties used for looking up and filtering Entity resources.
+        :param pulumi.Input[str] blueprint: The blueprint identifier the entity relates to
+        :param pulumi.Input[str] created_at: The creation date of the entity
+        :param pulumi.Input[str] created_by: The creator of the entity
+        :param pulumi.Input[str] icon: The icon of the entity
+        :param pulumi.Input[str] identifier: The identifier of the entity
+        :param pulumi.Input['EntityPropertiesArgs'] properties: The properties of the entity
+        :param pulumi.Input['EntityRelationsArgs'] relations: The relations of the entity
+        :param pulumi.Input[str] run_id: The runID of the action run that created the entity
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: The teams the entity belongs to
+        :param pulumi.Input[str] title: The title of the entity
+        :param pulumi.Input[str] updated_at: The last update date of the entity
+        :param pulumi.Input[str] updated_by: The last updater of the entity
+        """
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
+        if created_by is not None:
+            pulumi.set(__self__, "created_by", created_by)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
-        if invocation_method is not None:
-            pulumi.set(__self__, "invocation_method", invocation_method)
+        if properties is not None:
+            pulumi.set(__self__, "properties", properties)
+        if relations is not None:
+            pulumi.set(__self__, "relations", relations)
+        if run_id is not None:
+            pulumi.set(__self__, "run_id", run_id)
+        if teams is not None:
+            pulumi.set(__self__, "teams", teams)
         if title is not None:
             pulumi.set(__self__, "title", title)
-        if trigger is not None:
-            pulumi.set(__self__, "trigger", trigger)
-        if user_properties is not None:
-            pulumi.set(__self__, "user_properties", user_properties)
+        if updated_at is not None:
+            pulumi.set(__self__, "updated_at", updated_at)
+        if updated_by is not None:
+            pulumi.set(__self__, "updated_by", updated_by)
 
     @property
-    @pulumi.getter(name="blueprintIdentifier")
-    def blueprint_identifier(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier of the blueprint
+        The blueprint identifier the entity relates to
         """
-        return pulumi.get(self, "blueprint_identifier")
+        return pulumi.get(self, "blueprint")
 
-    @blueprint_identifier.setter
-    def blueprint_identifier(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "blueprint_identifier", value)
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
 
     @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The creation date of the entity
+        """
+        return pulumi.get(self, "created_at")
+
+    @created_at.setter
+    def created_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_at", value)
+
+    @property
+    @pulumi.getter(name="createdBy")
+    def created_by(self) -> Optional[pulumi.Input[str]]:
         """
-        The description of the action
+        The creator of the entity
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "created_by")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @created_by.setter
+    def created_by(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_by", value)
 
     @property
     @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
-        The icon of the action
+        The icon of the entity
         """
         return pulumi.get(self, "icon")
 
     @icon.setter
     def icon(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "icon", value)
 
     @property
     @pulumi.getter
     def identifier(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier of the action
+        The identifier of the entity
         """
         return pulumi.get(self, "identifier")
 
     @identifier.setter
     def identifier(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "identifier", value)
 
     @property
-    @pulumi.getter(name="invocationMethod")
-    def invocation_method(self) -> Optional[pulumi.Input['ActionInvocationMethodArgs']]:
+    @pulumi.getter
+    def properties(self) -> Optional[pulumi.Input['EntityPropertiesArgs']]:
         """
-        The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
+        The properties of the entity
         """
-        return pulumi.get(self, "invocation_method")
+        return pulumi.get(self, "properties")
 
-    @invocation_method.setter
-    def invocation_method(self, value: Optional[pulumi.Input['ActionInvocationMethodArgs']]):
-        pulumi.set(self, "invocation_method", value)
+    @properties.setter
+    def properties(self, value: Optional[pulumi.Input['EntityPropertiesArgs']]):
+        pulumi.set(self, "properties", value)
+
+    @property
+    @pulumi.getter
+    def relations(self) -> Optional[pulumi.Input['EntityRelationsArgs']]:
+        """
+        The relations of the entity
+        """
+        return pulumi.get(self, "relations")
+
+    @relations.setter
+    def relations(self, value: Optional[pulumi.Input['EntityRelationsArgs']]):
+        pulumi.set(self, "relations", value)
+
+    @property
+    @pulumi.getter(name="runId")
+    def run_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The runID of the action run that created the entity
+        """
+        return pulumi.get(self, "run_id")
+
+    @run_id.setter
+    def run_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "run_id", value)
+
+    @property
+    @pulumi.getter
+    def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The teams the entity belongs to
+        """
+        return pulumi.get(self, "teams")
+
+    @teams.setter
+    def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
-        The display name of the action
+        The title of the entity
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
-    @pulumi.getter
-    def trigger(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the action, one of CREATE, DAY-2, DELETE
+        The last update date of the entity
         """
-        return pulumi.get(self, "trigger")
+        return pulumi.get(self, "updated_at")
 
-    @trigger.setter
-    def trigger(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "trigger", value)
+    @updated_at.setter
+    def updated_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "updated_at", value)
 
     @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]]:
+    @pulumi.getter(name="updatedBy")
+    def updated_by(self) -> Optional[pulumi.Input[str]]:
         """
-        The input properties of the action
+        The last updater of the entity
         """
-        return pulumi.get(self, "user_properties")
+        return pulumi.get(self, "updated_by")
 
-    @user_properties.setter
-    def user_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ActionUserPropertyArgs']]]]):
-        pulumi.set(self, "user_properties", value)
+    @updated_by.setter
+    def updated_by(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "updated_by", value)
 
 
-class Action(pulumi.CustomResource):
+class Entity(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 blueprint_identifier: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
+                 blueprint: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 invocation_method: Optional[pulumi.Input[pulumi.InputType['ActionInvocationMethodArgs']]] = None,
+                 properties: Optional[pulumi.Input[pulumi.InputType['EntityPropertiesArgs']]] = None,
+                 relations: Optional[pulumi.Input[pulumi.InputType['EntityRelationsArgs']]] = None,
+                 run_id: Optional[pulumi.Input[str]] = None,
+                 teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActionUserPropertyArgs']]]]] = None,
                  __props__=None):
         """
-        Create a Action resource with the given unique name, props, and options.
+        Create a Entity resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] blueprint_identifier: The identifier of the blueprint
-        :param pulumi.Input[str] description: The description of the action
-        :param pulumi.Input[str] icon: The icon of the action
-        :param pulumi.Input[str] identifier: The identifier of the action
-        :param pulumi.Input[pulumi.InputType['ActionInvocationMethodArgs']] invocation_method: The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
-        :param pulumi.Input[str] title: The display name of the action
-        :param pulumi.Input[str] trigger: The type of the action, one of CREATE, DAY-2, DELETE
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActionUserPropertyArgs']]]] user_properties: The input properties of the action
+        :param pulumi.Input[str] blueprint: The blueprint identifier the entity relates to
+        :param pulumi.Input[str] icon: The icon of the entity
+        :param pulumi.Input[str] identifier: The identifier of the entity
+        :param pulumi.Input[pulumi.InputType['EntityPropertiesArgs']] properties: The properties of the entity
+        :param pulumi.Input[pulumi.InputType['EntityRelationsArgs']] relations: The relations of the entity
+        :param pulumi.Input[str] run_id: The runID of the action run that created the entity
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: The teams the entity belongs to
+        :param pulumi.Input[str] title: The title of the entity
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ActionArgs,
+                 args: EntityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Action resource with the given unique name, props, and options.
+        Create a Entity resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ActionArgs args: The arguments to use to populate this resource's properties.
+        :param EntityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ActionArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EntityArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 blueprint_identifier: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
+                 blueprint: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 invocation_method: Optional[pulumi.Input[pulumi.InputType['ActionInvocationMethodArgs']]] = None,
+                 properties: Optional[pulumi.Input[pulumi.InputType['EntityPropertiesArgs']]] = None,
+                 relations: Optional[pulumi.Input[pulumi.InputType['EntityRelationsArgs']]] = None,
+                 run_id: Optional[pulumi.Input[str]] = None,
+                 teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActionUserPropertyArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ActionArgs.__new__(ActionArgs)
+            __props__ = EntityArgs.__new__(EntityArgs)
 
-            if blueprint_identifier is None and not opts.urn:
-                raise TypeError("Missing required property 'blueprint_identifier'")
-            __props__.__dict__["blueprint_identifier"] = blueprint_identifier
-            __props__.__dict__["description"] = description
+            if blueprint is None and not opts.urn:
+                raise TypeError("Missing required property 'blueprint'")
+            __props__.__dict__["blueprint"] = blueprint
             __props__.__dict__["icon"] = icon
-            if identifier is None and not opts.urn:
-                raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
-            if invocation_method is None and not opts.urn:
-                raise TypeError("Missing required property 'invocation_method'")
-            __props__.__dict__["invocation_method"] = invocation_method
-            if title is None and not opts.urn:
-                raise TypeError("Missing required property 'title'")
+            __props__.__dict__["properties"] = properties
+            __props__.__dict__["relations"] = relations
+            __props__.__dict__["run_id"] = run_id
+            __props__.__dict__["teams"] = teams
             __props__.__dict__["title"] = title
-            if trigger is None and not opts.urn:
-                raise TypeError("Missing required property 'trigger'")
-            __props__.__dict__["trigger"] = trigger
-            __props__.__dict__["user_properties"] = user_properties
-        super(Action, __self__).__init__(
-            'port:index/action:Action',
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["created_by"] = None
+            __props__.__dict__["updated_at"] = None
+            __props__.__dict__["updated_by"] = None
+        super(Entity, __self__).__init__(
+            'port:index/entity:Entity',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            blueprint_identifier: Optional[pulumi.Input[str]] = None,
-            description: Optional[pulumi.Input[str]] = None,
+            blueprint: Optional[pulumi.Input[str]] = None,
+            created_at: Optional[pulumi.Input[str]] = None,
+            created_by: Optional[pulumi.Input[str]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
-            invocation_method: Optional[pulumi.Input[pulumi.InputType['ActionInvocationMethodArgs']]] = None,
+            properties: Optional[pulumi.Input[pulumi.InputType['EntityPropertiesArgs']]] = None,
+            relations: Optional[pulumi.Input[pulumi.InputType['EntityRelationsArgs']]] = None,
+            run_id: Optional[pulumi.Input[str]] = None,
+            teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             title: Optional[pulumi.Input[str]] = None,
-            trigger: Optional[pulumi.Input[str]] = None,
-            user_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActionUserPropertyArgs']]]]] = None) -> 'Action':
+            updated_at: Optional[pulumi.Input[str]] = None,
+            updated_by: Optional[pulumi.Input[str]] = None) -> 'Entity':
         """
-        Get an existing Action resource's state with the given name, id, and optional extra
+        Get an existing Entity resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] blueprint_identifier: The identifier of the blueprint
-        :param pulumi.Input[str] description: The description of the action
-        :param pulumi.Input[str] icon: The icon of the action
-        :param pulumi.Input[str] identifier: The identifier of the action
-        :param pulumi.Input[pulumi.InputType['ActionInvocationMethodArgs']] invocation_method: The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
-        :param pulumi.Input[str] title: The display name of the action
-        :param pulumi.Input[str] trigger: The type of the action, one of CREATE, DAY-2, DELETE
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActionUserPropertyArgs']]]] user_properties: The input properties of the action
+        :param pulumi.Input[str] blueprint: The blueprint identifier the entity relates to
+        :param pulumi.Input[str] created_at: The creation date of the entity
+        :param pulumi.Input[str] created_by: The creator of the entity
+        :param pulumi.Input[str] icon: The icon of the entity
+        :param pulumi.Input[str] identifier: The identifier of the entity
+        :param pulumi.Input[pulumi.InputType['EntityPropertiesArgs']] properties: The properties of the entity
+        :param pulumi.Input[pulumi.InputType['EntityRelationsArgs']] relations: The relations of the entity
+        :param pulumi.Input[str] run_id: The runID of the action run that created the entity
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: The teams the entity belongs to
+        :param pulumi.Input[str] title: The title of the entity
+        :param pulumi.Input[str] updated_at: The last update date of the entity
+        :param pulumi.Input[str] updated_by: The last updater of the entity
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ActionState.__new__(_ActionState)
+        __props__ = _EntityState.__new__(_EntityState)
 
-        __props__.__dict__["blueprint_identifier"] = blueprint_identifier
-        __props__.__dict__["description"] = description
+        __props__.__dict__["blueprint"] = blueprint
+        __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["created_by"] = created_by
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
-        __props__.__dict__["invocation_method"] = invocation_method
+        __props__.__dict__["properties"] = properties
+        __props__.__dict__["relations"] = relations
+        __props__.__dict__["run_id"] = run_id
+        __props__.__dict__["teams"] = teams
         __props__.__dict__["title"] = title
-        __props__.__dict__["trigger"] = trigger
-        __props__.__dict__["user_properties"] = user_properties
-        return Action(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["updated_at"] = updated_at
+        __props__.__dict__["updated_by"] = updated_by
+        return Entity(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="blueprintIdentifier")
-    def blueprint_identifier(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def blueprint(self) -> pulumi.Output[str]:
         """
-        The identifier of the blueprint
+        The blueprint identifier the entity relates to
         """
-        return pulumi.get(self, "blueprint_identifier")
+        return pulumi.get(self, "blueprint")
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[str]:
         """
-        The description of the action
+        The creation date of the entity
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter(name="createdBy")
+    def created_by(self) -> pulumi.Output[str]:
+        """
+        The creator of the entity
+        """
+        return pulumi.get(self, "created_by")
 
     @property
     @pulumi.getter
     def icon(self) -> pulumi.Output[Optional[str]]:
         """
-        The icon of the action
+        The icon of the entity
         """
         return pulumi.get(self, "icon")
 
     @property
     @pulumi.getter
     def identifier(self) -> pulumi.Output[str]:
         """
-        The identifier of the action
+        The identifier of the entity
         """
         return pulumi.get(self, "identifier")
 
     @property
-    @pulumi.getter(name="invocationMethod")
-    def invocation_method(self) -> pulumi.Output['outputs.ActionInvocationMethod']:
+    @pulumi.getter
+    def properties(self) -> pulumi.Output[Optional['outputs.EntityProperties']]:
         """
-        The methods the action is dispatched in. Supports WEBHOOK, KAFKA, GITHUB and AZURE-DEVOPS
+        The properties of the entity
         """
-        return pulumi.get(self, "invocation_method")
+        return pulumi.get(self, "properties")
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Output[str]:
+    def relations(self) -> pulumi.Output[Optional['outputs.EntityRelations']]:
         """
-        The display name of the action
+        The relations of the entity
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "relations")
+
+    @property
+    @pulumi.getter(name="runId")
+    def run_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The runID of the action run that created the entity
+        """
+        return pulumi.get(self, "run_id")
 
     @property
     @pulumi.getter
-    def trigger(self) -> pulumi.Output[str]:
+    def teams(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        The teams the entity belongs to
+        """
+        return pulumi.get(self, "teams")
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Output[Optional[str]]:
+        """
+        The title of the entity
+        """
+        return pulumi.get(self, "title")
+
+    @property
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> pulumi.Output[str]:
         """
-        The type of the action, one of CREATE, DAY-2, DELETE
+        The last update date of the entity
         """
-        return pulumi.get(self, "trigger")
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> pulumi.Output[Optional[Sequence['outputs.ActionUserProperty']]]:
+    @pulumi.getter(name="updatedBy")
+    def updated_by(self) -> pulumi.Output[str]:
         """
-        The input properties of the action
+        The last updater of the entity
         """
-        return pulumi.get(self, "user_properties")
+        return pulumi.get(self, "updated_by")
```

### Comparing `port_pulumi-0.9.4/port_pulumi/blueprint.py` & `port_pulumi-1.0.0/port_pulumi/blueprint.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,57 +13,58 @@
 
 __all__ = ['BlueprintArgs', 'Blueprint']
 
 @pulumi.input_type
 class BlueprintArgs:
     def __init__(__self__, *,
                  identifier: pulumi.Input[str],
-                 properties: pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]],
                  title: pulumi.Input[str],
-                 calculation_properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]] = None,
-                 changelog_destination: Optional[pulumi.Input['BlueprintChangelogDestinationArgs']] = None,
-                 data_source: Optional[pulumi.Input[str]] = None,
+                 calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
-                 mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]] = None,
-                 relations: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]] = None):
+                 kafka_changelog_destination: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']] = None,
+                 mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]] = None,
+                 properties: Optional[pulumi.Input['BlueprintPropertiesArgs']] = None,
+                 relations: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]] = None,
+                 team_inheritance: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']] = None,
+                 webhook_changelog_destination: Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']] = None):
         """
         The set of arguments for constructing a Blueprint resource.
         :param pulumi.Input[str] identifier: The identifier of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]] properties: The metadata of the entity
         :param pulumi.Input[str] title: The display name of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
-        :param pulumi.Input['BlueprintChangelogDestinationArgs'] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        :param pulumi.Input[str] data_source: The data source for entities of this blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]] calculation_properties: The calculation properties of the blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-               Blueprint.
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]] relations: The blueprints that are connected to this blueprint
+        :param pulumi.Input['BlueprintKafkaChangelogDestinationArgs'] kafka_changelog_destination: The changelog destination of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]] mirror_properties: The mirror properties of the blueprint
+        :param pulumi.Input['BlueprintPropertiesArgs'] properties: The properties of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]] relations: The relations of the blueprint
+        :param pulumi.Input['BlueprintTeamInheritanceArgs'] team_inheritance: The team inheritance of the blueprint
+        :param pulumi.Input['BlueprintWebhookChangelogDestinationArgs'] webhook_changelog_destination: The webhook changelog destination of the blueprint
         """
         pulumi.set(__self__, "identifier", identifier)
-        pulumi.set(__self__, "properties", properties)
         pulumi.set(__self__, "title", title)
         if calculation_properties is not None:
             pulumi.set(__self__, "calculation_properties", calculation_properties)
-        if changelog_destination is not None:
-            pulumi.set(__self__, "changelog_destination", changelog_destination)
-        if data_source is not None:
-            warnings.warn("""Data source is ignored""", DeprecationWarning)
-            pulumi.log.warn("""data_source is deprecated: Data source is ignored""")
-        if data_source is not None:
-            pulumi.set(__self__, "data_source", data_source)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
+        if kafka_changelog_destination is not None:
+            pulumi.set(__self__, "kafka_changelog_destination", kafka_changelog_destination)
         if mirror_properties is not None:
             pulumi.set(__self__, "mirror_properties", mirror_properties)
+        if properties is not None:
+            pulumi.set(__self__, "properties", properties)
         if relations is not None:
             pulumi.set(__self__, "relations", relations)
+        if team_inheritance is not None:
+            pulumi.set(__self__, "team_inheritance", team_inheritance)
+        if webhook_changelog_destination is not None:
+            pulumi.set(__self__, "webhook_changelog_destination", webhook_changelog_destination)
 
     @property
     @pulumi.getter
     def identifier(self) -> pulumi.Input[str]:
         """
         The identifier of the blueprint
         """
@@ -71,73 +72,37 @@
 
     @identifier.setter
     def identifier(self, value: pulumi.Input[str]):
         pulumi.set(self, "identifier", value)
 
     @property
     @pulumi.getter
-    def properties(self) -> pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]:
-        """
-        The metadata of the entity
-        """
-        return pulumi.get(self, "properties")
-
-    @properties.setter
-    def properties(self, value: pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]):
-        pulumi.set(self, "properties", value)
-
-    @property
-    @pulumi.getter
     def title(self) -> pulumi.Input[str]:
         """
         The display name of the blueprint
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="calculationProperties")
-    def calculation_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]:
+    def calculation_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]]:
         """
-        A set of properties that are calculated upon entity's regular properties.
+        The calculation properties of the blueprint
         """
         return pulumi.get(self, "calculation_properties")
 
     @calculation_properties.setter
-    def calculation_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]):
+    def calculation_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]]):
         pulumi.set(self, "calculation_properties", value)
 
     @property
-    @pulumi.getter(name="changelogDestination")
-    def changelog_destination(self) -> Optional[pulumi.Input['BlueprintChangelogDestinationArgs']]:
-        """
-        Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        """
-        return pulumi.get(self, "changelog_destination")
-
-    @changelog_destination.setter
-    def changelog_destination(self, value: Optional[pulumi.Input['BlueprintChangelogDestinationArgs']]):
-        pulumi.set(self, "changelog_destination", value)
-
-    @property
-    @pulumi.getter(name="dataSource")
-    def data_source(self) -> Optional[pulumi.Input[str]]:
-        """
-        The data source for entities of this blueprint
-        """
-        return pulumi.get(self, "data_source")
-
-    @data_source.setter
-    def data_source(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "data_source", value)
-
-    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         The description of the blueprint
         """
         return pulumi.get(self, "description")
 
@@ -154,157 +119,190 @@
         return pulumi.get(self, "icon")
 
     @icon.setter
     def icon(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "icon", value)
 
     @property
+    @pulumi.getter(name="kafkaChangelogDestination")
+    def kafka_changelog_destination(self) -> Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']]:
+        """
+        The changelog destination of the blueprint
+        """
+        return pulumi.get(self, "kafka_changelog_destination")
+
+    @kafka_changelog_destination.setter
+    def kafka_changelog_destination(self, value: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']]):
+        pulumi.set(self, "kafka_changelog_destination", value)
+
+    @property
     @pulumi.getter(name="mirrorProperties")
-    def mirror_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]]:
+    def mirror_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]]:
         """
-        When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-        Blueprint.
+        The mirror properties of the blueprint
         """
         return pulumi.get(self, "mirror_properties")
 
     @mirror_properties.setter
-    def mirror_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]]):
+    def mirror_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]]):
         pulumi.set(self, "mirror_properties", value)
 
     @property
     @pulumi.getter
-    def relations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]]:
+    def properties(self) -> Optional[pulumi.Input['BlueprintPropertiesArgs']]:
         """
-        The blueprints that are connected to this blueprint
+        The properties of the blueprint
+        """
+        return pulumi.get(self, "properties")
+
+    @properties.setter
+    def properties(self, value: Optional[pulumi.Input['BlueprintPropertiesArgs']]):
+        pulumi.set(self, "properties", value)
+
+    @property
+    @pulumi.getter
+    def relations(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]]:
+        """
+        The relations of the blueprint
         """
         return pulumi.get(self, "relations")
 
     @relations.setter
-    def relations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]]):
+    def relations(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]]):
         pulumi.set(self, "relations", value)
 
+    @property
+    @pulumi.getter(name="teamInheritance")
+    def team_inheritance(self) -> Optional[pulumi.Input['BlueprintTeamInheritanceArgs']]:
+        """
+        The team inheritance of the blueprint
+        """
+        return pulumi.get(self, "team_inheritance")
+
+    @team_inheritance.setter
+    def team_inheritance(self, value: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']]):
+        pulumi.set(self, "team_inheritance", value)
+
+    @property
+    @pulumi.getter(name="webhookChangelogDestination")
+    def webhook_changelog_destination(self) -> Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']]:
+        """
+        The webhook changelog destination of the blueprint
+        """
+        return pulumi.get(self, "webhook_changelog_destination")
+
+    @webhook_changelog_destination.setter
+    def webhook_changelog_destination(self, value: Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']]):
+        pulumi.set(self, "webhook_changelog_destination", value)
+
 
 @pulumi.input_type
 class _BlueprintState:
     def __init__(__self__, *,
-                 calculation_properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]] = None,
-                 changelog_destination: Optional[pulumi.Input['BlueprintChangelogDestinationArgs']] = None,
+                 calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  created_by: Optional[pulumi.Input[str]] = None,
-                 data_source: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]] = None,
-                 properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]] = None,
-                 relations: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]] = None,
+                 kafka_changelog_destination: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']] = None,
+                 mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]] = None,
+                 properties: Optional[pulumi.Input['BlueprintPropertiesArgs']] = None,
+                 relations: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]] = None,
+                 team_inheritance: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
-                 updated_by: Optional[pulumi.Input[str]] = None):
+                 updated_by: Optional[pulumi.Input[str]] = None,
+                 webhook_changelog_destination: Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']] = None):
         """
         Input properties used for looking up and filtering Blueprint resources.
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
-        :param pulumi.Input['BlueprintChangelogDestinationArgs'] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        :param pulumi.Input[str] data_source: The data source for entities of this blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]] calculation_properties: The calculation properties of the blueprint
+        :param pulumi.Input[str] created_at: The creation date of the blueprint
+        :param pulumi.Input[str] created_by: The creator of the blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-               Blueprint.
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]] properties: The metadata of the entity
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]] relations: The blueprints that are connected to this blueprint
+        :param pulumi.Input['BlueprintKafkaChangelogDestinationArgs'] kafka_changelog_destination: The changelog destination of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]] mirror_properties: The mirror properties of the blueprint
+        :param pulumi.Input['BlueprintPropertiesArgs'] properties: The properties of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]] relations: The relations of the blueprint
+        :param pulumi.Input['BlueprintTeamInheritanceArgs'] team_inheritance: The team inheritance of the blueprint
         :param pulumi.Input[str] title: The display name of the blueprint
+        :param pulumi.Input[str] updated_at: The last update date of the blueprint
+        :param pulumi.Input[str] updated_by: The last updater of the blueprint
+        :param pulumi.Input['BlueprintWebhookChangelogDestinationArgs'] webhook_changelog_destination: The webhook changelog destination of the blueprint
         """
         if calculation_properties is not None:
             pulumi.set(__self__, "calculation_properties", calculation_properties)
-        if changelog_destination is not None:
-            pulumi.set(__self__, "changelog_destination", changelog_destination)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
-        if data_source is not None:
-            warnings.warn("""Data source is ignored""", DeprecationWarning)
-            pulumi.log.warn("""data_source is deprecated: Data source is ignored""")
-        if data_source is not None:
-            pulumi.set(__self__, "data_source", data_source)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
+        if kafka_changelog_destination is not None:
+            pulumi.set(__self__, "kafka_changelog_destination", kafka_changelog_destination)
         if mirror_properties is not None:
             pulumi.set(__self__, "mirror_properties", mirror_properties)
         if properties is not None:
             pulumi.set(__self__, "properties", properties)
         if relations is not None:
             pulumi.set(__self__, "relations", relations)
+        if team_inheritance is not None:
+            pulumi.set(__self__, "team_inheritance", team_inheritance)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if updated_at is not None:
             pulumi.set(__self__, "updated_at", updated_at)
         if updated_by is not None:
             pulumi.set(__self__, "updated_by", updated_by)
+        if webhook_changelog_destination is not None:
+            pulumi.set(__self__, "webhook_changelog_destination", webhook_changelog_destination)
 
     @property
     @pulumi.getter(name="calculationProperties")
-    def calculation_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]:
+    def calculation_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]]:
         """
-        A set of properties that are calculated upon entity's regular properties.
+        The calculation properties of the blueprint
         """
         return pulumi.get(self, "calculation_properties")
 
     @calculation_properties.setter
-    def calculation_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]):
+    def calculation_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]]):
         pulumi.set(self, "calculation_properties", value)
 
     @property
-    @pulumi.getter(name="changelogDestination")
-    def changelog_destination(self) -> Optional[pulumi.Input['BlueprintChangelogDestinationArgs']]:
-        """
-        Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        """
-        return pulumi.get(self, "changelog_destination")
-
-    @changelog_destination.setter
-    def changelog_destination(self, value: Optional[pulumi.Input['BlueprintChangelogDestinationArgs']]):
-        pulumi.set(self, "changelog_destination", value)
-
-    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The creation date of the blueprint
+        """
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="createdBy")
     def created_by(self) -> Optional[pulumi.Input[str]]:
+        """
+        The creator of the blueprint
+        """
         return pulumi.get(self, "created_by")
 
     @created_by.setter
     def created_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_by", value)
 
     @property
-    @pulumi.getter(name="dataSource")
-    def data_source(self) -> Optional[pulumi.Input[str]]:
-        """
-        The data source for entities of this blueprint
-        """
-        return pulumi.get(self, "data_source")
-
-    @data_source.setter
-    def data_source(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "data_source", value)
-
-    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         The description of the blueprint
         """
         return pulumi.get(self, "description")
 
@@ -333,112 +331,154 @@
         return pulumi.get(self, "identifier")
 
     @identifier.setter
     def identifier(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "identifier", value)
 
     @property
+    @pulumi.getter(name="kafkaChangelogDestination")
+    def kafka_changelog_destination(self) -> Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']]:
+        """
+        The changelog destination of the blueprint
+        """
+        return pulumi.get(self, "kafka_changelog_destination")
+
+    @kafka_changelog_destination.setter
+    def kafka_changelog_destination(self, value: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']]):
+        pulumi.set(self, "kafka_changelog_destination", value)
+
+    @property
     @pulumi.getter(name="mirrorProperties")
-    def mirror_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]]:
+    def mirror_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]]:
         """
-        When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-        Blueprint.
+        The mirror properties of the blueprint
         """
         return pulumi.get(self, "mirror_properties")
 
     @mirror_properties.setter
-    def mirror_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]]):
+    def mirror_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]]):
         pulumi.set(self, "mirror_properties", value)
 
     @property
     @pulumi.getter
-    def properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]]:
+    def properties(self) -> Optional[pulumi.Input['BlueprintPropertiesArgs']]:
         """
-        The metadata of the entity
+        The properties of the blueprint
         """
         return pulumi.get(self, "properties")
 
     @properties.setter
-    def properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]]):
+    def properties(self, value: Optional[pulumi.Input['BlueprintPropertiesArgs']]):
         pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter
-    def relations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]]:
+    def relations(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]]:
         """
-        The blueprints that are connected to this blueprint
+        The relations of the blueprint
         """
         return pulumi.get(self, "relations")
 
     @relations.setter
-    def relations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]]):
+    def relations(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]]):
         pulumi.set(self, "relations", value)
 
     @property
+    @pulumi.getter(name="teamInheritance")
+    def team_inheritance(self) -> Optional[pulumi.Input['BlueprintTeamInheritanceArgs']]:
+        """
+        The team inheritance of the blueprint
+        """
+        return pulumi.get(self, "team_inheritance")
+
+    @team_inheritance.setter
+    def team_inheritance(self, value: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']]):
+        pulumi.set(self, "team_inheritance", value)
+
+    @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
         The display name of the blueprint
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="updatedAt")
     def updated_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The last update date of the blueprint
+        """
         return pulumi.get(self, "updated_at")
 
     @updated_at.setter
     def updated_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated_at", value)
 
     @property
     @pulumi.getter(name="updatedBy")
     def updated_by(self) -> Optional[pulumi.Input[str]]:
+        """
+        The last updater of the blueprint
+        """
         return pulumi.get(self, "updated_by")
 
     @updated_by.setter
     def updated_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated_by", value)
 
+    @property
+    @pulumi.getter(name="webhookChangelogDestination")
+    def webhook_changelog_destination(self) -> Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']]:
+        """
+        The webhook changelog destination of the blueprint
+        """
+        return pulumi.get(self, "webhook_changelog_destination")
+
+    @webhook_changelog_destination.setter
+    def webhook_changelog_destination(self, value: Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']]):
+        pulumi.set(self, "webhook_changelog_destination", value)
+
 
 class Blueprint(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 calculation_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]]] = None,
-                 changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']]] = None,
-                 data_source: Optional[pulumi.Input[str]] = None,
+                 calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]]] = None,
-                 properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintPropertyArgs']]]]] = None,
-                 relations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]]] = None,
+                 kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
+                 mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
+                 properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
+                 relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
+                 team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
                  title: Optional[pulumi.Input[str]] = None,
+                 webhook_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintWebhookChangelogDestinationArgs']]] = None,
                  __props__=None):
         """
         Create a Blueprint resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
-        :param pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        :param pulumi.Input[str] data_source: The data source for entities of this blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]] calculation_properties: The calculation properties of the blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-               Blueprint.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintPropertyArgs']]]] properties: The metadata of the entity
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]] relations: The blueprints that are connected to this blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']] kafka_changelog_destination: The changelog destination of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]] mirror_properties: The mirror properties of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']] properties: The properties of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]] relations: The relations of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']] team_inheritance: The team inheritance of the blueprint
         :param pulumi.Input[str] title: The display name of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintWebhookChangelogDestinationArgs']] webhook_changelog_destination: The webhook changelog destination of the blueprint
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BlueprintArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -455,152 +495,145 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 calculation_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]]] = None,
-                 changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']]] = None,
-                 data_source: Optional[pulumi.Input[str]] = None,
+                 calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
-                 mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]]] = None,
-                 properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintPropertyArgs']]]]] = None,
-                 relations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]]] = None,
+                 kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
+                 mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
+                 properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
+                 relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
+                 team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
                  title: Optional[pulumi.Input[str]] = None,
+                 webhook_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintWebhookChangelogDestinationArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BlueprintArgs.__new__(BlueprintArgs)
 
             __props__.__dict__["calculation_properties"] = calculation_properties
-            __props__.__dict__["changelog_destination"] = changelog_destination
-            if data_source is not None and not opts.urn:
-                warnings.warn("""Data source is ignored""", DeprecationWarning)
-                pulumi.log.warn("""data_source is deprecated: Data source is ignored""")
-            __props__.__dict__["data_source"] = data_source
             __props__.__dict__["description"] = description
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
+            __props__.__dict__["kafka_changelog_destination"] = kafka_changelog_destination
             __props__.__dict__["mirror_properties"] = mirror_properties
-            if properties is None and not opts.urn:
-                raise TypeError("Missing required property 'properties'")
             __props__.__dict__["properties"] = properties
             __props__.__dict__["relations"] = relations
+            __props__.__dict__["team_inheritance"] = team_inheritance
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
             __props__.__dict__["title"] = title
+            __props__.__dict__["webhook_changelog_destination"] = webhook_changelog_destination
             __props__.__dict__["created_at"] = None
             __props__.__dict__["created_by"] = None
             __props__.__dict__["updated_at"] = None
             __props__.__dict__["updated_by"] = None
         super(Blueprint, __self__).__init__(
             'port:index/blueprint:Blueprint',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            calculation_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]]] = None,
-            changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']]] = None,
+            calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             created_by: Optional[pulumi.Input[str]] = None,
-            data_source: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
-            mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]]] = None,
-            properties: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintPropertyArgs']]]]] = None,
-            relations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]]] = None,
+            kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
+            mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
+            properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
+            relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
+            team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
             title: Optional[pulumi.Input[str]] = None,
             updated_at: Optional[pulumi.Input[str]] = None,
-            updated_by: Optional[pulumi.Input[str]] = None) -> 'Blueprint':
+            updated_by: Optional[pulumi.Input[str]] = None,
+            webhook_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintWebhookChangelogDestinationArgs']]] = None) -> 'Blueprint':
         """
         Get an existing Blueprint resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
-        :param pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        :param pulumi.Input[str] data_source: The data source for entities of this blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]] calculation_properties: The calculation properties of the blueprint
+        :param pulumi.Input[str] created_at: The creation date of the blueprint
+        :param pulumi.Input[str] created_by: The creator of the blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-               Blueprint.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintPropertyArgs']]]] properties: The metadata of the entity
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]] relations: The blueprints that are connected to this blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']] kafka_changelog_destination: The changelog destination of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]] mirror_properties: The mirror properties of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']] properties: The properties of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]] relations: The relations of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']] team_inheritance: The team inheritance of the blueprint
         :param pulumi.Input[str] title: The display name of the blueprint
+        :param pulumi.Input[str] updated_at: The last update date of the blueprint
+        :param pulumi.Input[str] updated_by: The last updater of the blueprint
+        :param pulumi.Input[pulumi.InputType['BlueprintWebhookChangelogDestinationArgs']] webhook_changelog_destination: The webhook changelog destination of the blueprint
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BlueprintState.__new__(_BlueprintState)
 
         __props__.__dict__["calculation_properties"] = calculation_properties
-        __props__.__dict__["changelog_destination"] = changelog_destination
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["created_by"] = created_by
-        __props__.__dict__["data_source"] = data_source
         __props__.__dict__["description"] = description
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
+        __props__.__dict__["kafka_changelog_destination"] = kafka_changelog_destination
         __props__.__dict__["mirror_properties"] = mirror_properties
         __props__.__dict__["properties"] = properties
         __props__.__dict__["relations"] = relations
+        __props__.__dict__["team_inheritance"] = team_inheritance
         __props__.__dict__["title"] = title
         __props__.__dict__["updated_at"] = updated_at
         __props__.__dict__["updated_by"] = updated_by
+        __props__.__dict__["webhook_changelog_destination"] = webhook_changelog_destination
         return Blueprint(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="calculationProperties")
-    def calculation_properties(self) -> pulumi.Output[Optional[Sequence['outputs.BlueprintCalculationProperty']]]:
+    def calculation_properties(self) -> pulumi.Output[Optional[Mapping[str, 'outputs.BlueprintCalculationProperties']]]:
         """
-        A set of properties that are calculated upon entity's regular properties.
+        The calculation properties of the blueprint
         """
         return pulumi.get(self, "calculation_properties")
 
     @property
-    @pulumi.getter(name="changelogDestination")
-    def changelog_destination(self) -> pulumi.Output[Optional['outputs.BlueprintChangelogDestination']]:
-        """
-        Blueprints changelog destination, Supports WEBHOOK and KAFKA
-        """
-        return pulumi.get(self, "changelog_destination")
-
-    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
+        """
+        The creation date of the blueprint
+        """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="createdBy")
     def created_by(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "created_by")
-
-    @property
-    @pulumi.getter(name="dataSource")
-    def data_source(self) -> pulumi.Output[Optional[str]]:
         """
-        The data source for entities of this blueprint
+        The creator of the blueprint
         """
-        return pulumi.get(self, "data_source")
+        return pulumi.get(self, "created_by")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         The description of the blueprint
         """
@@ -619,49 +652,78 @@
     def identifier(self) -> pulumi.Output[str]:
         """
         The identifier of the blueprint
         """
         return pulumi.get(self, "identifier")
 
     @property
+    @pulumi.getter(name="kafkaChangelogDestination")
+    def kafka_changelog_destination(self) -> pulumi.Output[Optional['outputs.BlueprintKafkaChangelogDestination']]:
+        """
+        The changelog destination of the blueprint
+        """
+        return pulumi.get(self, "kafka_changelog_destination")
+
+    @property
     @pulumi.getter(name="mirrorProperties")
-    def mirror_properties(self) -> pulumi.Output[Optional[Sequence['outputs.BlueprintMirrorProperty']]]:
+    def mirror_properties(self) -> pulumi.Output[Optional[Mapping[str, 'outputs.BlueprintMirrorProperties']]]:
         """
-        When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
-        Blueprint.
+        The mirror properties of the blueprint
         """
         return pulumi.get(self, "mirror_properties")
 
     @property
     @pulumi.getter
-    def properties(self) -> pulumi.Output[Sequence['outputs.BlueprintProperty']]:
+    def properties(self) -> pulumi.Output[Optional['outputs.BlueprintProperties']]:
         """
-        The metadata of the entity
+        The properties of the blueprint
         """
         return pulumi.get(self, "properties")
 
     @property
     @pulumi.getter
-    def relations(self) -> pulumi.Output[Optional[Sequence['outputs.BlueprintRelation']]]:
+    def relations(self) -> pulumi.Output[Optional[Mapping[str, 'outputs.BlueprintRelations']]]:
         """
-        The blueprints that are connected to this blueprint
+        The relations of the blueprint
         """
         return pulumi.get(self, "relations")
 
     @property
+    @pulumi.getter(name="teamInheritance")
+    def team_inheritance(self) -> pulumi.Output[Optional['outputs.BlueprintTeamInheritance']]:
+        """
+        The team inheritance of the blueprint
+        """
+        return pulumi.get(self, "team_inheritance")
+
+    @property
     @pulumi.getter
     def title(self) -> pulumi.Output[str]:
         """
         The display name of the blueprint
         """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="updatedAt")
     def updated_at(self) -> pulumi.Output[str]:
+        """
+        The last update date of the blueprint
+        """
         return pulumi.get(self, "updated_at")
 
     @property
     @pulumi.getter(name="updatedBy")
     def updated_by(self) -> pulumi.Output[str]:
+        """
+        The last updater of the blueprint
+        """
         return pulumi.get(self, "updated_by")
 
+    @property
+    @pulumi.getter(name="webhookChangelogDestination")
+    def webhook_changelog_destination(self) -> pulumi.Output[Optional['outputs.BlueprintWebhookChangelogDestination']]:
+        """
+        The webhook changelog destination of the blueprint
+        """
+        return pulumi.get(self, "webhook_changelog_destination")
+
```

### Comparing `port_pulumi-0.9.4/port_pulumi/provider.py` & `port_pulumi-1.0.0/port_pulumi/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,34 +16,43 @@
     def __init__(__self__, *,
                  client_id: pulumi.Input[str],
                  secret: pulumi.Input[str],
                  base_url: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] client_id: Client ID for Port-labs
+        :param pulumi.Input[str] secret: Client Secret for Port-labs
+        :param pulumi.Input[str] token: Token for Port-labs
         """
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "secret", secret)
         if base_url is not None:
             pulumi.set(__self__, "base_url", base_url)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Input[str]:
+        """
+        Client ID for Port-labs
+        """
         return pulumi.get(self, "client_id")
 
     @client_id.setter
     def client_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Input[str]:
+        """
+        Client Secret for Port-labs
+        """
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret", value)
 
     @property
@@ -54,14 +63,17 @@
     @base_url.setter
     def base_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "base_url", value)
 
     @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
+        """
+        Token for Port-labs
+        """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
 
@@ -79,14 +91,17 @@
         The provider type for the port package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] client_id: Client ID for Port-labs
+        :param pulumi.Input[str] secret: Client Secret for Port-labs
+        :param pulumi.Input[str] token: Token for Port-labs
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -144,19 +159,28 @@
     @pulumi.getter(name="baseUrl")
     def base_url(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "base_url")
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Output[str]:
+        """
+        Client ID for Port-labs
+        """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[str]:
+        """
+        Client Secret for Port-labs
+        """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[Optional[str]]:
+        """
+        Token for Port-labs
+        """
         return pulumi.get(self, "token")
```

### Comparing `port_pulumi-0.9.4/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: port-pulumi
-Version: 0.9.4
+Name: port_pulumi
+Version: 1.0.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
-Project-URL: Repository, https://github.com/port-labs/pulumi
+Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
@@ -18,25 +18,24 @@
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
-
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @port-labs/pulumi
+npm install @port-labs/port
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @port-labs/pulumi
+yarn add @port-labs/port
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -44,21 +43,21 @@
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
-go get github.com/port-labs/pulumi/sdk
+go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:baseUrl` (environment: `PORT_BASE_URL`) - This is the Port base URL. 
-- `port:clientId` (environment: `PORT_CLIENT_ID`) - This is the Port client ID.
-- `port:secret` (environment: `PORT_CLIENT_SECRET`) - This is the Port secret.
-- `port:token` - This is the Port token.
+- `port:clientId` - This is the Port client ID.
+- `port:secret` - This is the Port secret.
+- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-0.9.4/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-1.0.0/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.4/setup.py` & `port_pulumi-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.4"
-PLUGIN_VERSION = "0.9.4"
+VERSION = "1.0.0"
+PLUGIN_VERSION = "1.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi-port'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the port resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
@@ -45,15 +45,15 @@
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi port category/utility',
       url='https://www.pulumi.com',
       project_urls={
-          'Repository': 'https://github.com/port-labs/pulumi'
+          'Repository': 'https://github.com/port-labs/pulumi-port'
       },
       license='Apache-2.0',
       packages=find_packages(),
       package_data={
           'port_pulumi': [
               'py.typed',
               'pulumi-plugin.json',
```

