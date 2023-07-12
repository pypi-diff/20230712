# Comparing `tmp/aws_a2i-0.2.1.tar.gz` & `tmp/aws_a2i-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_a2i-0.2.1.tar", last modified: Mon Feb 20 15:33:43 2023, max compression
+gzip compressed data, was "aws_a2i-0.3.1.tar", last modified: Wed Jul 12 00:44:23 2023, max compression
```

## Comparing `aws_a2i-0.2.1.tar` & `aws_a2i-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-20 15:33:43.244434 aws_a2i-0.2.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1117 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      315 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     3433 2023-02-20 15:33:43.244282 aws_a2i-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2385 2023-02-18 04:56:27.000000 aws_a2i-0.2.1/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-20 15:33:43.241679 aws_a2i-0.2.1/aws_a2i/
--rw-r--r--   0 sanhehu    (505) staff       (20)     1670 2023-02-20 15:16:24.000000 aws_a2i-0.2.1/aws_a2i/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-20 15:30:56.000000 aws_a2i-0.2.1/aws_a2i/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-20 15:33:43.243639 aws_a2i-0.2.1/aws_a2i/better_boto/
--rw-r--r--   0 sanhehu    (505) staff       (20)       24 2023-02-18 04:00:13.000000 aws_a2i-0.2.1/aws_a2i/better_boto/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    12219 2023-02-20 14:45:33.000000 aws_a2i-0.2.1/aws_a2i/better_boto/flow_definition.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     9355 2023-02-20 15:22:44.000000 aws_a2i-0.2.1/aws_a2i/better_boto/human_loop.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5035 2023-02-20 14:45:10.000000 aws_a2i-0.2.1/aws_a2i/better_boto/human_task_ui.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-20 15:33:43.243978 aws_a2i-0.2.1/aws_a2i/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/aws_a2i/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      220 2023-02-18 03:04:23.000000 aws_a2i-0.2.1/aws_a2i/helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      299 2023-02-17 17:29:52.000000 aws_a2i-0.2.1/aws_a2i/tagging.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      907 2023-02-18 04:40:35.000000 aws_a2i-0.2.1/aws_a2i/tools.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1402 2023-02-18 04:09:58.000000 aws_a2i-0.2.1/aws_a2i/waiter.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-20 15:33:43.242580 aws_a2i-0.2.1/aws_a2i.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     3433 2023-02-20 15:33:43.000000 aws_a2i-0.2.1/aws_a2i.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      589 2023-02-20 15:33:43.000000 aws_a2i-0.2.1/aws_a2i.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-20 15:33:43.000000 aws_a2i-0.2.1/aws_a2i.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      316 2023-02-20 15:33:43.000000 aws_a2i-0.2.1/aws_a2i.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        8 2023-02-20 15:33:43.000000 aws_a2i-0.2.1/aws_a2i.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     2169 2023-02-20 15:30:33.000000 aws_a2i-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      347 2023-02-18 04:41:07.000000 aws_a2i-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      183 2023-02-18 02:47:17.000000 aws_a2i-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      139 2023-02-20 15:13:18.000000 aws_a2i-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-20 15:33:43.244479 aws_a2i-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7653 2023-02-18 04:57:02.000000 aws_a2i-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.410836 aws_a2i-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1117 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3602 2023-07-12 00:44:23.410671 aws_a2i-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2554 2023-07-12 00:38:36.000000 aws_a2i-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.408332 aws_a2i-0.3.1/aws_a2i/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1679 2023-07-11 20:00:14.000000 aws_a2i-0.3.1/aws_a2i/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-12 00:39:29.000000 aws_a2i-0.3.1/aws_a2i/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2184 2023-07-12 00:15:09.000000 aws_a2i-0.3.1/aws_a2i/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.409933 aws_a2i-0.3.1/aws_a2i/better_boto/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/aws_a2i/better_boto/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13953 2023-07-12 00:24:02.000000 aws_a2i-0.3.1/aws_a2i/better_boto/flow_definition.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11991 2023-07-12 00:22:45.000000 aws_a2i-0.3.1/aws_a2i/better_boto/human_loop.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-07-11 20:31:42.000000 aws_a2i-0.3.1/aws_a2i/better_boto/human_task_ui.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.410210 aws_a2i-0.3.1/aws_a2i/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/aws_a2i/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      220 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/aws_a2i/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5861 2023-07-11 21:21:43.000000 aws_a2i-0.3.1/aws_a2i/playground.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      299 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/aws_a2i/tagging.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1173 2023-07-12 00:33:41.000000 aws_a2i-0.3.1/aws_a2i/tools.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2332 2023-07-11 20:23:13.000000 aws_a2i-0.3.1/aws_a2i/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.409109 aws_a2i-0.3.1/aws_a2i.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3602 2023-07-12 00:44:23.000000 aws_a2i-0.3.1/aws_a2i.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      644 2023-07-12 00:44:23.000000 aws_a2i-0.3.1/aws_a2i.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-12 00:44:23.000000 aws_a2i-0.3.1/aws_a2i.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      374 2023-07-12 00:44:23.000000 aws_a2i-0.3.1/aws_a2i.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        8 2023-07-12 00:44:23.000000 aws_a2i-0.3.1/aws_a2i.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4404 2023-07-12 00:42:29.000000 aws_a2i-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      347 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      197 2023-07-11 19:56:30.000000 aws_a2i-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-12 00:44:23.410886 aws_a2i-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7653 2023-07-10 20:01:35.000000 aws_a2i-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 00:44:23.410372 aws_a2i-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1516 2023-07-12 00:15:42.000000 aws_a2i-0.3.1/tests/test_api.py
```

### Comparing `aws_a2i-0.2.1/LICENSE.txt` & `aws_a2i-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_a2i-0.2.1/PKG-INFO` & `aws_a2i-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_a2i
-Version: 0.2.1
+Version: 0.3.1
 Summary: Amazon Augmented AI for Human.
 Home-page: https://github.com/MacHu-GWU/aws_a2i-project
-Download-URL: https://pypi.python.org/pypi/aws_a2i/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_a2i/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -45,14 +45,17 @@
 
 .. image:: https://img.shields.io/pypi/l/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
 .. image:: https://img.shields.io/pypi/pyversions/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/aws_a2i-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/aws_a2i-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `aws_a2i-0.2.1/README.rst` & `aws_a2i-0.3.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 .. image:: https://img.shields.io/pypi/l/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
 .. image:: https://img.shields.io/pypi/pyversions/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/aws_a2i-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/aws_a2i-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `aws_a2i-0.2.1/aws_a2i/__init__.py` & `aws_a2i-0.3.1/aws_a2i/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,9 @@
         to_tag_list,
         to_tag_dict,
     )
     from .helper import (
         sha256_of_bytes,
         vprint,
     )
-except ImportError:  # pragma: no cover
-    pass
+except ImportError as e:  # pragma: no cover
+    print(e)
```

### Comparing `aws_a2i-0.2.1/aws_a2i/better_boto/flow_definition.py` & `aws_a2i-0.3.1/aws_a2i/better_boto/flow_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     get_task_template_arn,
 )
 
 
 # --- Data Model
 @dataclasses.dataclass
 class HumanLoopConfig:
+    """
+    An attribute of :class:`FlowDefinition`.
+    """
+
     work_team_arn: T.Optional[str] = dataclasses.field(default=None)
     human_task_ui_arn: T.Optional[str] = dataclasses.field(default=None)
     task_title: T.Optional[str] = dataclasses.field(default=None)
     task_description: T.Optional[str] = dataclasses.field(default=None)
     task_count: T.Optional[int] = dataclasses.field(default=None)
     task_availability_lifetime_in_seconds: T.Optional[int] = dataclasses.field(
         default=None
@@ -33,37 +37,57 @@
     @property
     def human_task_ui_name(self) -> str:
         return self.task_title
 
 
 @dataclasses.dataclass
 class OutputConfig:
+    """
+    An attribute of :class:`FlowDefinition`.
+    """
+
     s3_output_path: T.Optional[str] = dataclasses.field(default=None)
     kms_key_id: T.Optional[str] = dataclasses.field(default=None)
 
 
 class FlowDefinitionStatusEnum(str, enum.Enum):
+    """
+    human review workflow definition status enumeration.
+    """
+
     Initializing = "Initializing"
     Active = "Active"
     Failed = "Failed"
     Deleting = "Deleting"
 
 
 @dataclasses.dataclass
 class FlowDefinition:
+    """
+    The data model of a human review workflow definition.
+
+    :param data: the raw data from the ``describe_flow_definition`` api response.
+    """
+
     arn: T.Optional[str] = dataclasses.field(default=None)
     name: T.Optional[str] = dataclasses.field(default=None)
     status: T.Optional[str] = dataclasses.field(default=None)
     creation_time: T.Optional[datetime] = dataclasses.field(default=None)
     role_arn: T.Optional[str] = dataclasses.field(default=None)
     human_loop_config: T.Optional[HumanLoopConfig] = dataclasses.field(default=None)
     output_config: T.Optional[OutputConfig] = dataclasses.field(default=None)
+    data: T.Optional[dict] = dataclasses.field(default=None)
 
     @classmethod
     def from_describe_flow_definition_response(cls, response: dict) -> "FlowDefinition":
+        """
+        Reference:
+
+        - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_flow_definition.html
+        """
         return cls(
             arn=response["FlowDefinitionArn"],
             name=response["FlowDefinitionName"],
             status=response["FlowDefinitionStatus"],
             role_arn=response["RoleArn"],
             creation_time=response["CreationTime"],
             human_loop_config=HumanLoopConfig(
@@ -79,16 +103,29 @@
                     "TaskTimeLimitInSeconds"
                 ),
             ),
             output_config=OutputConfig(
                 s3_output_path=response["OutputConfig"]["S3OutputPath"],
                 kms_key_id=response["OutputConfig"].get("KmsKeyId"),
             ),
+            data=response,
         )
 
+    def is_initializing(self) -> bool:
+        return self.status == FlowDefinitionStatusEnum.Initializing.value
+
+    def is_active(self) -> bool:
+        return self.status == FlowDefinitionStatusEnum.Active.value
+
+    def is_failed(self) -> bool:
+        return self.status == FlowDefinitionStatusEnum.Failed.value
+
+    def is_deleting(self) -> bool:
+        return self.status == FlowDefinitionStatusEnum.Deleting.value
+
 
 # --- Low level API
 def get_flow_definition_arn(
     aws_account_id: str,
     aws_region: str,
     flow_definition_name: str,
 ) -> str:
@@ -99,16 +136,17 @@
 
 
 def get_flow_definition_console_url(
     aws_region: str,
     flow_definition_name: str,
 ) -> str:
     return (
-        f"https://console.aws.amazon.com/a2i/home?region={aws_region}#"
-        f"/human-review-workflows/{flow_definition_name}"
+        f"https://{aws_region}.console.aws.amazon.com/sagemaker"
+        f"/groundtruth?region={aws_region}#"
+        f"/a2i/human-review-workflows/{flow_definition_name}"
     )
 
 
 def parse_flow_definition_name_from_arn(arn: str) -> str:
     """
     Example:
 
@@ -129,22 +167,24 @@
     task_description: str,
     task_count: int,
     task_availability_life_time_in_seconds: T.Optional[int] = None,
     task_time_limit_in_seconds: T.Optional[int] = None,
     tags: T.Optional[T.Dict[str, str]] = None,
 ) -> dict:
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition
     """
     task_template_arn = get_task_template_arn(
         aws_account_id=bsm.aws_account_id,
         aws_region=bsm.aws_region,
         task_template_name=task_template_name,
     )
-    if output_key.endswith("/"):
+    if output_key.endswith("/"):  # aws will treat this as a folder
         output_key = output_key[:-1]
     human_loop_config = {
         "WorkteamArn": labeling_team_arn,
         "HumanTaskUiArn": task_template_arn,
         "TaskTitle": task_template_name,
         "TaskDescription": task_description,
         "TaskCount": task_count,
@@ -170,28 +210,32 @@
 
 
 def delete_flow_definition(
     bsm: BotoSesManager,
     flow_definition_name: str,
 ):
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_flow_definition
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_flow_definition
     """
     return bsm.sagemaker_client.delete_flow_definition(
         FlowDefinitionName=flow_definition_name
     )
 
 
 # --- High level API
 def is_flow_definition_exists(
     bsm: BotoSesManager,
     flow_definition_name: str,
 ) -> T.Tuple[bool, T.Optional[FlowDefinition]]:
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_flow_definition
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_flow_definition
 
     :return: tuple of two item, first item is a boolean value, second value is
         the response of ``describe_flow_definition()``, you can call it flow details.
     """
     try:
         response = bsm.sagemaker_client.describe_flow_definition(
             FlowDefinitionName=flow_definition_name
@@ -207,14 +251,17 @@
 def remove_flow_definition(
     bsm: BotoSesManager,
     flow_definition_name: str,
     wait: bool = True,
     wait_timeout: int = 30,
     verbose: bool = True,
 ):
+    """
+    High level api to remove a human review workflow definition.
+    """
     vprint(
         f"{emojis.delete} Remove Human review workflow definition, it may takes 30 sec ~ 1 minute",
         verbose,
     )
     flow_definition_console_url = get_flow_definition_console_url(
         bsm.aws_region,
         flow_definition_name,
@@ -233,20 +280,24 @@
         if wait:
             for _ in Waiter(delays=1, timeout=wait_timeout, indent=2, verbose=verbose):
                 is_flow_exists, flow_def = is_flow_definition_exists(
                     bsm=bsm,
                     flow_definition_name=flow_definition_name,
                 )
                 if is_flow_exists is False:
+                    vprint("", verbose)
                     break
                 if flow_def.status == "Failed":
                     raise Exception("Failed!")
     else:
         vprint("  Flow definition doesn't exists, do nothing.", verbose)
-    vprint(f"  {emojis.succeeded} Successfully delete flow definition {flow_definition_name!r}", verbose)
+    vprint(
+        f"  {emojis.succeeded} Successfully delete flow definition {flow_definition_name!r}",
+        verbose,
+    )
 
 
 def deploy_flow_definition(
     bsm: BotoSesManager,
     flow_definition_name: str,
     flow_execution_role_arn: str,
     labeling_team_arn: str,
@@ -255,19 +306,23 @@
     task_template_name: str,
     task_description: str,
     task_count: int,
     task_availability_life_time_in_seconds: T.Optional[int] = None,
     task_time_limit_in_seconds: T.Optional[int] = None,
     tags: T.Optional[T.Dict[str, str]] = None,
     wait: bool = True,
+    wait_delay: int = 3,
     wait_timeout: int = 30,
     verbose: bool = True,
-):
+) -> T.Optional[dict]:
     """
-    Deploy a Human in Loop workflow. in smart way.
+    High level api to deploy a Human review workflow, smartly.
+
+    :return: if deployment happens, then return the response of ``create_flow_definition()``,
+        otherwise return ``None``.
     """
     vprint(
         f"{emojis.deploy} Deploy Human review workflow definition, it may takes 30 sec ~ 1 minute",
         verbose,
     )
     flow_definition_console_url = get_flow_definition_console_url(
         aws_region=bsm.aws_region,
@@ -302,24 +357,25 @@
                 flow_def.output_config.s3_output_path
                 == f"s3://{output_bucket}/{output_key}"
             )
         )
         # no need to deploy
         if no_change_flag:
             vprint("  No configuration changed, do nothing.", verbose)
-            return
+            return None
         # remove existing one first
         remove_flow_definition(
             bsm=bsm,
             flow_definition_name=flow_definition_name,
             wait=True,
             verbose=verbose,
         )
+
     vprint("Create Human review workflow definition ...", verbose)
-    create_flow_definition(
+    response = create_flow_definition(
         bsm,
         flow_definition_name=flow_definition_name,
         flow_execution_role_arn=flow_execution_role_arn,
         labeling_team_arn=labeling_team_arn,
         output_bucket=output_bucket,
         output_key=output_key,
         task_template_name=task_template_name,
@@ -327,22 +383,33 @@
         task_count=task_count,
         task_availability_life_time_in_seconds=task_availability_life_time_in_seconds,
         task_time_limit_in_seconds=task_time_limit_in_seconds,
         tags=tags,
     )
 
     if wait:
-        for _ in Waiter(delays=1, timeout=wait_timeout, indent=2, verbose=verbose):
+        for _ in Waiter(
+            delays=wait_delay, timeout=wait_timeout, indent=2, verbose=verbose
+        ):
             is_flow_exists, flow_def = is_flow_definition_exists(
                 bsm=bsm,
                 flow_definition_name=flow_definition_name,
             )
+            # create_flow_definition() may return before the flow definition
+            # is created
             if is_flow_exists is False:
+                continue
+
+            if flow_def.is_active():
+                vprint("", verbose)
                 break
-            if flow_def.status == FlowDefinitionStatusEnum.Active.value:
-                break
-            if flow_def.status == FlowDefinitionStatusEnum.Failed.value:
-                raise Exception("Failed")
+
+            if flow_def.is_failed():
+                raise Exception(
+                    f"Creating Human Review Workflow {flow_definition_name!r} Failed"
+                )
 
     vprint(
-        f"  {emojis.succeeded} Successfully deployed flow definition {flow_definition_name!r}", verbose
+        f"  {emojis.succeeded} Successfully deployed flow definition {flow_definition_name!r}",
+        verbose,
     )
+    return response
```

### Comparing `aws_a2i-0.2.1/aws_a2i/better_boto/human_loop.py` & `aws_a2i-0.3.1/aws_a2i/better_boto/human_loop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,103 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import json
 import enum
 import dataclasses
-from datetime import datetime
+from datetime import datetime, timezone
 
 from light_emoji import common as emojis
 from iterproxy import IterProxy
 from boto_session_manager import BotoSesManager
 
 from ..helper import vprint
 
 from .flow_definition import (
     parse_flow_definition_name_from_arn,
 )
 
 # --- Data Model
+date_fmt = "%Y-%m-%dT%H:%M:%S.%fZ"
+
+
+@dataclasses.dataclass
+class HumanAnswer:
+    acceptanceTime: str
+    answerContent: dict
+    submissionTime: str
+    timeSpentInSeconds: float
+    workerId: str
+    workerMetadata: dict
+
+    @classmethod
+    def from_dict(cls, dct: dict):
+        return cls(**dct)
+
+    @property
+    def acceptance_datetime(self) -> datetime:
+        return datetime.strptime(self.acceptanceTime, date_fmt).replace(
+            tzinfo=timezone.utc
+        )
+
+    @property
+    def submission_datetime(self) -> datetime:
+        return datetime.strptime(self.submissionTime, date_fmt).replace(
+            tzinfo=timezone.utc
+        )
+
+
+@dataclasses.dataclass
+class HumanLoopOutput:
+    """
+    Human loop output data model.
+    """
+
+    flowDefinitionArn: str
+    humanAnswers: T.List[HumanAnswer]
+    humanLoopName: str
+    inputContent: dict
+
+    @classmethod
+    def from_dict(cls, dct: dict):
+        dct["humanAnswers"] = [
+            HumanAnswer.from_dict(dct) for dct in dct.get("humanAnswers", [])
+        ]
+        return cls(**dct)
+
+
 class HumanLoopStatusEnum(str, enum.Enum):
+    """
+    Human loop status enumeration
+    """
+
     InProgress = "InProgress"
     Failed = "Failed"
     Completed = "Completed"
     Stopped = "Stopped"
     Stopping = "Stopping"
 
 
 @dataclasses.dataclass
 class HumanLoop:
+    """
+    The data model of a human loop.
+
+    :param data: the raw data from the ``describe_human_loop`` api response.
+    """
+
     creation_time: T.Optional[datetime] = dataclasses.field(default=None)
     failure_reason: T.Optional[str] = dataclasses.field(default=None)
     failure_code: T.Optional[str] = dataclasses.field(default=None)
     human_loop_status: T.Optional[str] = dataclasses.field(default=None)
     human_loop_name: T.Optional[str] = dataclasses.field(default=None)
     human_loop_arn: T.Optional[str] = dataclasses.field(default=None)
     flow_definition_arn: T.Optional[str] = dataclasses.field(default=None)
     human_loop_output_s3uri: T.Optional[str] = dataclasses.field(default=None)
+    data: T.Optional[dict] = dataclasses.field(default=None)
 
     def get_details(self, bsm: BotoSesManager) -> "HumanLoop":
         """
         Call ``describe_human_loop`` API to fetch additional details.
         """
         if self.human_loop_name is not None:
             human_loop = get_human_loop_details(
@@ -56,16 +115,43 @@
         self.failure_reason = human_loop.failure_reason
         self.failure_code = human_loop.failure_code
         self.human_loop_status = human_loop.human_loop_status
         self.human_loop_name = human_loop.human_loop_name
         self.human_loop_arn = human_loop.human_loop_arn
         self.flow_definition_arn = human_loop.flow_definition_arn
         self.human_loop_output_s3uri = human_loop.human_loop_output_s3uri
+        self.data = human_loop.data
         return self
 
+    def is_in_progress(self) -> bool:
+        return self.human_loop_status == HumanLoopStatusEnum.InProgress.value
+
+    def is_failed(self) -> bool:
+        return self.human_loop_status == HumanLoopStatusEnum.Failed.value
+
+    def is_completed(self) -> bool:
+        return self.human_loop_status == HumanLoopStatusEnum.Completed.value
+
+    def is_stopped(self) -> bool:
+        return self.human_loop_status == HumanLoopStatusEnum.Stopped.value
+
+    def is_stopping(self) -> bool:
+        return self.human_loop_status == HumanLoopStatusEnum.Stopping.value
+
+    def get_output(self, bsm: BotoSesManager) -> HumanLoopOutput:
+        parts = self.human_loop_output_s3uri.split("/", 3)
+        bucket = parts[2]
+        key = parts[3]
+        res = bsm.s3_client.get_object(
+            Bucket=bucket,
+            Key=key,
+        )
+        data = json.loads(res["Body"].read())
+        return HumanLoopOutput.from_dict(data)
+
 
 # --- Low level API
 def parse_team_name_from_private_team_arn(arn: str) -> str:
     """
     Example:
 
          >>> parse_team_name_from_private_team_arn(
@@ -93,17 +179,17 @@
 
 def get_hil_console_url(
     aws_region: str,
     flow_definition_name: str,
     hil_name: str,
 ) -> str:
     return (
-        f"https://{aws_region}.console.aws.amazon.com/a2i/home?"
-        f"region={aws_region}#/human-review-workflows/"
-        f"{flow_definition_name}/human-loops/{hil_name}"
+        f"https://{aws_region}.console.aws.amazon.com/sagemaker"
+        f"/groundtruth?region={aws_region}#/a2i/human-review-workflows"
+        f"/{flow_definition_name}/human-loops/{hil_name}"
     )
 
 
 def parse_hil_name_from_hil_arn(arn: str) -> str:
     """
     Example:
 
@@ -114,39 +200,45 @@
 
 
 def describe_human_loop(
     bsm: BotoSesManager,
     human_loop_name: str,
 ) -> dict:
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop
     """
     return bsm.sagemaker_a2i_runtime_client.describe_human_loop(
         HumanLoopName=human_loop_name,
     )
 
 
 def stop_human_loop(
     bsm: BotoSesManager,
     human_loop_name: str,
 ):
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop
     """
     return bsm.sagemaker_a2i_runtime_client.stop_human_loop(
         HumanLoopName=human_loop_name,
     )
 
 
 def delete_human_loop(
     bsm: BotoSesManager,
     human_loop_name: str,
 ):
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop
     """
     return bsm.sagemaker_a2i_runtime_client.delete_human_loop(
         HumanLoopName=human_loop_name,
     )
 
 
 # --- High level API
@@ -155,15 +247,17 @@
     human_loop_name: str,
     flow_definition_arn: str,
     input_data: dict,
     data_attributes: T.Optional[dict] = None,
     verbose: bool = True,
 ) -> str:
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop
 
     :return: the human in loop task ARN.
     """
     vprint(
         f"{emojis.play_or_pause} Start a Human Loop Task {human_loop_name!r}", verbose
     )
     flow_definition_name = parse_flow_definition_name_from_arn(flow_definition_arn)
@@ -205,14 +299,15 @@
         failure_reason=response.get("FailureReason"),
         failure_code=response.get("FailureCode"),
         human_loop_status=response["HumanLoopStatus"],
         human_loop_name=response["HumanLoopName"],
         human_loop_arn=response["HumanLoopArn"],
         flow_definition_arn=response["FlowDefinitionArn"],
         human_loop_output_s3uri=response["HumanLoopOutput"]["OutputS3Uri"],
+        data=response,
     )
 
 
 class HumanLoopIterProxy(IterProxy[HumanLoop]):
     pass
 
 
@@ -238,25 +333,30 @@
     else:
         kwargs["SortOrder"] = "Descending"
     kwargs["PaginationConfig"] = dict(
         MaxItems=max_items,
         PageSize=page_size,
     )
     response_iterator = paginator.paginate(**kwargs)
+    parts = flow_definition_arn.split(":")
+    aws_region = parts[3]
+    aws_account_id = parts[4]
     for response in response_iterator:
         for data in response["HumanLoopSummaries"]:
+            human_loop_name = data["HumanLoopName"]
             yield HumanLoop(
                 creation_time=data["CreationTime"],
                 failure_reason=data.get("FailureReason"),
                 failure_code=None,
                 human_loop_status=data["HumanLoopStatus"],
-                human_loop_name=data["HumanLoopName"],
-                human_loop_arn=None,
+                human_loop_name=human_loop_name,
+                human_loop_arn=f"arn:aws:sagemaker:{aws_region}:{aws_account_id}:human-loop/{human_loop_name}",
                 flow_definition_arn=data["FlowDefinitionArn"],
                 human_loop_output_s3uri=None,
+                data=data,
             )
 
 
 def list_human_loops(
     bsm: BotoSesManager,
     flow_definition_arn: str,
     creation_time_after: T.Optional[datetime] = None,
@@ -265,15 +365,17 @@
     max_items: T.Optional[int] = 1000,
     page_size: T.Optional[int] = 100,
 ) -> HumanLoopIterProxy:
     """
     List human loops. You can then call :meth:`HumanLoop.get_details()` method
     to fetch more details.
 
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops
     """
     return HumanLoopIterProxy(
         iterable=_list_human_loops(
             bsm=bsm,
             flow_definition_arn=flow_definition_arn,
             creation_time_after=creation_time_after,
             creation_time_before=creation_time_before,
```

### Comparing `aws_a2i-0.2.1/aws_a2i/better_boto/human_task_ui.py` & `aws_a2i-0.3.1/aws_a2i/better_boto/human_task_ui.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 
 
 def get_task_template_console_url(
     aws_region: str,
     task_template_name: str,
 ) -> str:
     return (
-        f"https://console.aws.amazon.com/a2i/home?region={aws_region}#"
-        f"/worker-task-templates/{task_template_name}"
+        f"https://{aws_region}.console.aws.amazon.com/sagemaker"
+        f"/groundtruth?region={aws_region}#/a2i/worker-task-templates"
+        f"/{task_template_name}"
     )
 
 
 def parse_task_template_name_from_arn(arn: str) -> str:
     """
     Example:
 
@@ -42,15 +43,17 @@
 
 
 def is_hil_task_template_exists(
     bsm: BotoSesManager,
     task_template_name: str,
 ) -> T.Tuple[bool, dict]:
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_human_task_ui
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_human_task_ui
 
     :return: tuple of two item, first item is a boolean value, second value is
         the response of ``describe_human_task_ui()``, you can call it task ui details.
     """
     try:
         response = bsm.sagemaker_client.describe_human_task_ui(
             HumanTaskUiName=task_template_name,
@@ -82,29 +85,34 @@
 
 
 def delete_human_task_ui(
     bsm: BotoSesManager,
     task_template_name: str,
 ):
     """
-    ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_human_task_ui
+    Reference:
+
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_human_task_ui
     """
     return bsm.sagemaker_client.delete_human_task_ui(HumanTaskUiName=task_template_name)
 
 
 # --- High level API
 def deploy_hil_task_template(
     bsm: BotoSesManager,
     task_template_name: str,
     task_template_content: str,
     tags: T.Optional[T.Dict[str, str]] = None,
     verbose: bool = True,
-):
+) -> T.Optional[dict]:
     """
-    Deploy HIL task template. in smart way.
+    Deploy HIL task template, smartly.
+
+    :return: if deployment happens, then return the response of ``create_human_task_ui()``,
+        otherwise return ``None``.
     """
     vprint(f"{emojis.deploy} Deploy Human in Loop task template", verbose)
     task_template_console_url = get_task_template_console_url(
         aws_region=bsm.aws_region,
         task_template_name=task_template_name,
     )
     vprint(f"  preview at {task_template_console_url}", verbose)
@@ -115,38 +123,47 @@
     if flag:
         content_sha256 = response["UiTemplate"]["ContentSha256"]
         if content_sha256 == sha256_of_bytes(task_template_content.encode("utf-8")):
             vprint(
                 "  a HIL task template with the same content already exists, do nothing.",
                 verbose,
             )
-            return
+            return None
         else:
             delete_human_task_ui(
                 bsm=bsm,
                 task_template_name=task_template_name,
             )
-            create_human_task_ui(
+            response = create_human_task_ui(
                 bsm=bsm,
                 task_template_name=task_template_name,
                 task_template_content=task_template_content,
                 tags=tags,
             )
     else:
-        create_human_task_ui(bsm, task_template_name, task_template_content, tags)
+        response = create_human_task_ui(
+            bsm, task_template_name, task_template_content, tags
+        )
     vprint(
-        f"  {emojis.succeeded} Successfully deployed task ui template {task_template_name!r}", verbose
+        f"  {emojis.succeeded} Successfully deployed task ui template {task_template_name!r}",
+        verbose,
     )
+    return response
 
 
 def remove_hil_task_template(
     bsm: BotoSesManager,
     task_template_name: str,
     verbose: bool = True,
-):
+) -> bool:
+    """
+    Remove HIL task template, smartly.
+
+    :return: a boolean flag indicating whether the delete operation happens.
+    """
     vprint(f"{emojis.delete} Remove Human in Loop task template", verbose)
     task_template_console_url = get_task_template_console_url(
         aws_region=bsm.aws_region,
         task_template_name=task_template_name,
     )
     vprint(f"  verify at {task_template_console_url}", verbose)
     flag, response = is_hil_task_template_exists(
@@ -156,8 +173,13 @@
     if flag:
         delete_human_task_ui(
             bsm=bsm,
             task_template_name=task_template_name,
         )
     else:
         vprint("  HIL task template doesn't exists, do nothing.", verbose)
-    vprint(f"  {emojis.succeeded} Successfully removed task ui template {task_template_name!r}", verbose)
+
+    vprint(
+        f"  {emojis.succeeded} Successfully removed task ui template {task_template_name!r}",
+        verbose,
+    )
+    return not flag
```

### Comparing `aws_a2i-0.2.1/aws_a2i/tools.py` & `aws_a2i-0.3.1/aws_a2i/tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import sys
 import subprocess
 from pathlib import Path
 
-from box import Box
-from liquid import Template
+try:
+    from box import Box
+    from liquid import Template
+
+    HAS_DEPENDENCIES = True
+except ImportError as e:
+    HAS_DEPENDENCIES = False
+
+
+def _warn_if_no_dependencies():
+    if HAS_DEPENDENCIES is False:
+        raise ImportError(f"cannot import 'box' or 'liquid' package")
 
 
 def render_task_template(
     task_template_content: str,
     input_data: dict,
     path_task_ui_html: T.Union[str, Path, T.Any],
     preview: bool = True,
 ):
+    _warn_if_no_dependencies()
+
     # read liquid template
     template = Template(task_template_content)
 
     # convert task data to box, so it support dot notation
     task = Box({"input": input_data})
 
     # render template
```

### Comparing `aws_a2i-0.2.1/aws_a2i.egg-info/PKG-INFO` & `aws_a2i-0.3.1/aws_a2i.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-a2i
-Version: 0.2.1
+Version: 0.3.1
 Summary: Amazon Augmented AI for Human.
 Home-page: https://github.com/MacHu-GWU/aws_a2i-project
-Download-URL: https://pypi.python.org/pypi/aws_a2i/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_a2i/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -45,14 +45,17 @@
 
 .. image:: https://img.shields.io/pypi/l/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
 .. image:: https://img.shields.io/pypi/pyversions/aws_a2i.svg
     :target: https://pypi.python.org/pypi/aws_a2i
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/aws_a2i-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/aws_a2i-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `aws_a2i-0.2.1/aws_a2i.egg-info/SOURCES.txt` & `aws_a2i-0.3.1/aws_a2i.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 requirements-dev.txt
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 aws_a2i/__init__.py
 aws_a2i/_version.py
+aws_a2i/api.py
 aws_a2i/helper.py
+aws_a2i/playground.py
 aws_a2i/tagging.py
 aws_a2i/tools.py
 aws_a2i/waiter.py
 aws_a2i.egg-info/PKG-INFO
 aws_a2i.egg-info/SOURCES.txt
 aws_a2i.egg-info/dependency_links.txt
 aws_a2i.egg-info/requires.txt
 aws_a2i.egg-info/top_level.txt
 aws_a2i/better_boto/__init__.py
 aws_a2i/better_boto/flow_definition.py
 aws_a2i/better_boto/human_loop.py
 aws_a2i/better_boto/human_task_ui.py
-aws_a2i/docs/__init__.py
+aws_a2i/docs/__init__.py
+tests/test_api.py
```

### Comparing `aws_a2i-0.2.1/requirements-doc.txt` & `aws_a2i-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_a2i-0.2.1/setup.py` & `aws_a2i-0.3.1/setup.py`

 * *Files identical despite different names*

