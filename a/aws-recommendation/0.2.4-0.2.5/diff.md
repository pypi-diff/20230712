# Comparing `tmp/aws_recommendation-0.2.4.tar.gz` & `tmp/aws_recommendation-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_recommendation-0.2.4.tar", last modified: Fri May  5 08:30:12 2023, max compression
+gzip compressed data, was "aws_recommendation-0.2.5.tar", last modified: Wed Jul 12 10:02:27 2023, max compression
```

## Comparing `aws_recommendation-0.2.4.tar` & `aws_recommendation-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:30:12.193559 aws_recommendation-0.2.4/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.4/LICENCE
--rw-rw-rw-   0        0        0     1220 2023-05-05 08:30:12.191558 aws_recommendation-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:30:12.167557 aws_recommendation-0.2.4/aws_recommendation/
--rw-rw-rw-   0        0        0     2329 2023-05-05 08:29:45.000000 aws_recommendation-0.2.4/aws_recommendation/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/cloudwatch.py
--rw-rw-rw-   0        0        0    11769 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/cost_estimations.py
--rw-rw-rw-   0        0        0     4287 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/dynamodb.py
--rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/ebs.py
--rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/ec2.py
--rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/elb.py
--rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/kms.py
--rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/rds.py
--rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/redshift.py
--rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/s3.py
--rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/truted_advisor.py
--rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.4/aws_recommendation/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:30:12.186557 aws_recommendation-0.2.4/aws_recommendation.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-05-05 08:30:11.000000 aws_recommendation-0.2.4/aws_recommendation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-05 08:30:11.000000 aws_recommendation-0.2.4/aws_recommendation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:30:11.000000 aws_recommendation-0.2.4/aws_recommendation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 08:30:11.000000 aws_recommendation-0.2.4/aws_recommendation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 08:30:11.000000 aws_recommendation-0.2.4/aws_recommendation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      525 2023-05-05 08:29:45.000000 aws_recommendation-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:30:12.193559 aws_recommendation-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.5/LICENCE
+-rw-rw-rw-   0        0        0     1220 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.003237 aws_recommendation-0.2.5/aws_recommendation/
+-rw-rw-rw-   0        0        0     2329 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/aws_recommendation/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/cloudwatch.py
+-rw-rw-rw-   0        0        0    11769 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/cost_estimations.py
+-rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/aws_recommendation/dynamodb.py
+-rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/ebs.py
+-rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/ec2.py
+-rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/elb.py
+-rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/kms.py
+-rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/rds.py
+-rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/redshift.py
+-rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/s3.py
+-rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/truted_advisor.py
+-rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/aws_recommendation.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      525 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/setup.cfg
```

### Comparing `aws_recommendation-0.2.4/PKG-INFO` & `aws_recommendation-0.2.5/aws_recommendation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws_recommendation
-Version: 0.2.4
+Name: aws-recommendation
+Version: 0.2.5
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.4/README.md` & `aws_recommendation-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/__init__.py` & `aws_recommendation-0.2.5/aws_recommendation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Any
 
 from botocore.exceptions import ClientError
 
 from boto3 import session
 
 __author__ = "Dheeraj Banodha"
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 
 import logging
 
 from aws_recommendation.cloudwatch import cloudwatch
 from aws_recommendation.dynamodb import dynamodb
 from aws_recommendation.ebs import ebs
 from aws_recommendation.ec2 import ec2
```

### Comparing `aws_recommendation-0.2.4/aws_recommendation/cloudwatch.py` & `aws_recommendation-0.2.5/aws_recommendation/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/cost_estimations.py` & `aws_recommendation-0.2.5/aws_recommendation/cost_estimations.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/dynamodb.py` & `aws_recommendation-0.2.5/aws_recommendation/dynamodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                             temp = {
                                 'Service Name': 'DynamoDB',
                                 'Id': table,
                                 'Recommendation': 'Remove Dynamodb table',
                                 'Description': 'Identify any unused Amazon DynamoDB tables available within your AWS account and remove them to help lower the cost of your monthly AWS bill. A DynamoDB table is considered unused if it’s ItemCount parameter, which describes the number of items in the table, is equal to 0 (zero)',
                                 'Metadata': {
                                     'Region': region,
-                                    'TableStatus': table_desc['TableStatus']
+                                    'TableStatus': table_desc['Table']['TableStatus']
                                 },
                                 'Recommendation Reason': {
                                     'reason': "The ItemCount parameter value is 0, therefore the selected amazon dynamodb table is not currently in use and can be safely removed from your AWS Account"
                                 },
                                 'Risk': 'Medium',
                                 'Savings': None,
                                 'Source': 'Klera',
```

### Comparing `aws_recommendation-0.2.4/aws_recommendation/ebs.py` & `aws_recommendation-0.2.5/aws_recommendation/ebs.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/ec2.py` & `aws_recommendation-0.2.5/aws_recommendation/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/elb.py` & `aws_recommendation-0.2.5/aws_recommendation/elb.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/kms.py` & `aws_recommendation-0.2.5/aws_recommendation/kms.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/rds.py` & `aws_recommendation-0.2.5/aws_recommendation/rds.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/redshift.py` & `aws_recommendation-0.2.5/aws_recommendation/redshift.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/s3.py` & `aws_recommendation-0.2.5/aws_recommendation/s3.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/truted_advisor.py` & `aws_recommendation-0.2.5/aws_recommendation/truted_advisor.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation/utils.py` & `aws_recommendation-0.2.5/aws_recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/aws_recommendation.egg-info/PKG-INFO` & `aws_recommendation-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws-recommendation
-Version: 0.2.4
+Name: aws_recommendation
+Version: 0.2.5
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.4/aws_recommendation.egg-info/SOURCES.txt` & `aws_recommendation-0.2.5/aws_recommendation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.4/pyproject.toml` & `aws_recommendation-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_recommendation"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="dheeraj.banodha", email="dheerajmbanodha@gmail.com" },
 ]
 description = "Provides AWS recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

