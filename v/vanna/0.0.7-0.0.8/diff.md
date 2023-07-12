# Comparing `tmp/vanna-0.0.7.tar.gz` & `tmp/vanna-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.7.tar", last modified: Fri Jul  7 21:11:48 2023, max compression
+gzip compressed data, was "vanna-0.0.8.tar", last modified: Wed Jul 12 16:48:33 2023, max compression
```

## Comparing `vanna-0.0.7.tar` & `vanna-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 21:11:34.000000 vanna-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:11:48.157350 vanna-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 21:11:34.000000 vanna-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 21:11:35.000000 vanna-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:11:48.157350 vanna-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-07 21:11:35.000000 vanna-0.0.7/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 21:11:35.000000 vanna-0.0.7/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 16:48:06.000000 vanna-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-12 16:48:33.458595 vanna-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-12 16:48:06.000000 vanna-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-12 16:48:06.000000 vanna-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:48:33.458595 vanna-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.454595 vanna-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    16009 2023-07-12 16:48:06.000000 vanna-0.0.8/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-12 16:48:06.000000 vanna-0.0.8/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.7/LICENSE` & `vanna-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.7/pyproject.toml` & `vanna-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "vanna"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "requests", "tabulate", "plotly"
+    "requests", "tabulate", "plotly", "pandas"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/vanna-ai/vanna-py"
 "Bug Tracker" = "https://github.com/vanna-ai/vanna-py/issues"
```

### Comparing `vanna-0.0.7/src/vanna/__init__.py` & `vanna-0.0.8/src/vanna/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             'Vanna-Key': api_key,
             'Vanna-Org': __org
         }
     else:
         headers = {
             'Content-Type': 'application/json',
             'Vanna-Key': api_key,
-            'Vanna-Org': 'demo-sales'
+            'Vanna-Org': 'demo-tpc-h'
         }
 
     data = {
         "method": method,
         "params": [__dataclass_to_dict(obj) for obj in params]
     }
 
@@ -196,15 +196,15 @@
         if status.success:
             raise Exception(f"An organization with the name {org} already exists")
 
         create = input(f"Would you like to create organization '{org}'? (y/n): ")
 
         if create.lower() == 'y':
             db_type = input("What type of database would you like to use? (Snowflake, BigQuery, Postgres, etc.): ")
-            __org = 'demo-sales'
+            __org = 'demo-tpc-h'
             if create_org(org=org, db_type=db_type):
                 __org = org
             else:
                 __org = None
                 raise Exception("Failed to create organization")
     else:
         __org = org
@@ -285,14 +285,42 @@
     if 'result' not in d:
         return False
     
     status = Status(**d['result'])
 
     return status.success
 
+# def read_questions_from_github(url: str) -> List[QuestionSQLPair]:
+#     """
+#     ## Example
+#     ```python
+#     url = "https://raw.githubusercontent.com/vanna-ai/vanna-ai/main/data/questions.json"
+#     questions = vn.read_questions_from_github(url)
+#     ```
+#     Read questions and SQL queries from a GitHub URL.
+
+#     Args:
+#         url (str): The URL to read from.
+
+#     Returns:
+#         List[QuestionSQLPair]: A list of [`QuestionSQLPair`][vanna.QuestionSQLPair] objects.
+#     """
+#     response = requests.get(url)
+#     data = response.json()
+
+#     question_sql_pairs = []
+#     for item in data:
+#         question = item.get('question')
+#         sql = item.get('sql')
+#         if question and sql:
+#             question_sql_pair = QuestionSQLPair(question=question, sql=sql)
+#             question_sql_pairs.append(question_sql_pair)
+
+#     return question_sql_pairs
+
 def remove_sql(question: str) -> bool:
     """
     ## Example
     ```python
     vn.remove_sql(question="What is the average salary of employees?")
     ```
     Remove a question and its corresponding SQL query from the Vanna.AI database.
```

### Comparing `vanna-0.0.7/src/vanna/types.py` & `vanna-0.0.8/src/vanna/types.py`

 * *Files identical despite different names*

