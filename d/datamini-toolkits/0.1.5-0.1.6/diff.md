# Comparing `tmp/datamini_toolkits-0.1.5.tar.gz` & `tmp/datamini_toolkits-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamini_toolkits-0.1.5.tar", last modified: Wed Jul 12 03:13:57 2023, max compression
+gzip compressed data, was "datamini_toolkits-0.1.6.tar", last modified: Wed Jul 12 03:15:26 2023, max compression
```

## Comparing `datamini_toolkits-0.1.5.tar` & `datamini_toolkits-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:13:57.326919 datamini_toolkits-0.1.5/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:13:57.326800 datamini_toolkits-0.1.5/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.5/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:13:57.323859 datamini_toolkits-0.1.5/datamini_toolkits/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.5/datamini_toolkits/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:13:57.325109 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.5/datamini_toolkits/cmysql/prompts.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:13:57.326480 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6142 2023-07-12 03:10:09.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2585 2023-07-12 03:13:46.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/prompts.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/test_tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.5/datamini_toolkits/mock_data/tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.5/datamini_toolkits/tests.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:13:57.324524 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:13:57.000000 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      757 2023-07-12 03:13:57.000000 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-12 03:13:57.000000 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-07-12 03:13:57.000000 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-12 03:13:57.000000 datamini_toolkits-0.1.5/datamini_toolkits.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-12 03:13:57.326954 datamini_toolkits-0.1.5/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-07-12 03:13:52.000000 datamini_toolkits-0.1.5/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.705357 datamini_toolkits-0.1.6/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:15:26.705241 datamini_toolkits-0.1.6/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.6/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.702155 datamini_toolkits-0.1.6/datamini_toolkits/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.6/datamini_toolkits/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.703474 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/prompts.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.704979 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6140 2023-07-12 03:14:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1614 2023-07-12 03:14:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2585 2023-07-12 03:13:46.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/prompts.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/test_tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.6/datamini_toolkits/tests.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.702830 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      757 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-12 03:15:26.705387 datamini_toolkits-0.1.6/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-07-12 03:15:25.000000 datamini_toolkits-0.1.6/setup.py
```

### Comparing `datamini_toolkits-0.1.5/README.md` & `datamini_toolkits-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/cmysql/cli.py` & `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/cli.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/cmysql/logs.py` & `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/cmysql/prompts.py` & `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/agent.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from langchain.agents import initialize_agent, AgentType
 from langchain.agents.tools import Tool
 from langchain.memory import ConversationBufferMemory
 from langchain.chains import SQLDatabaseChain
 
 
 from prompts import RECORD_CREATOR_PROMPT_TEMPLATE, TABLE_CREATOR_PROMPT_TEMPLATE, SCHEMA_DESIGNER_PROMPT_TEMPLATE
-from .base import ChatOpenAIWithLog, SQLDatabaseWithLog
-from .logs import log
+from base import ChatOpenAIWithLog, SQLDatabaseWithLog
+from logs import log
 
 
 
 class DataMakerAgentCreator(object):
     def __init__(self, db_uri):
 
         self.db_uri = db_uri
```

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/base.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from langchain.sql_database import SQLDatabase
 from langchain.sql_database import sqlalchemy
 from langchain.chat_models import ChatOpenAI
 
-from .tools import parse_sql_script, check_function_creation
-from .logs import log
+from tools import parse_sql_script, check_function_creation
+from logs import log
 
 class ChatOpenAIWithLog(ChatOpenAI):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def run(self, text: str, **kwargs) -> str:
         rst = super().predict(text=text, **kwargs)
```

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/cli.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/cli.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/logs.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/prompts.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/test_tools.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/test_tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits/mock_data/tools.py` & `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.5/datamini_toolkits.egg-info/SOURCES.txt` & `datamini_toolkits-0.1.6/datamini_toolkits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

