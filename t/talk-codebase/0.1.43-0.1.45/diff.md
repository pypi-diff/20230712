# Comparing `tmp/talk_codebase-0.1.43.tar.gz` & `tmp/talk_codebase-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.43.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.45.tar", max compression
```

## Comparing `talk_codebase-0.1.43.tar` & `talk_codebase-0.1.45.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2762 2023-07-12 00:42:08.867523 talk_codebase-0.1.43/README.md
--rw-r--r--   0        0        0      984 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/cli.py
--rw-r--r--   0        0        0     3765 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/config.py
--rw-r--r--   0        0        0     1860 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/consts.py
--rw-r--r--   0        0        0     4921 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/utils.py
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 talk_codebase-0.1.43/PKG-INFO
+-rw-r--r--   0        0        0     2951 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/README.md
+-rw-r--r--   0        0        0      984 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/cli.py
+-rw-r--r--   0        0        0     3765 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/config.py
+-rw-r--r--   0        0        0     1762 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/consts.py
+-rw-r--r--   0        0        0     4921 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-12 00:56:27.642209 talk_codebase-0.1.45/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 talk_codebase-0.1.45/PKG-INFO
```

### Comparing `talk_codebase-0.1.43/README.md` & `talk_codebase-0.1.45/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,25 @@
 talk-codebase chat .
 ```
 
 Select model type: Local or OpenAI
 
 <img width="300" alt="select_type" src="https://github.com/rsaryev/talk-codebase/assets/70219513/05196fe5-78ff-44ff-8ca3-0313ccef572a">
 
+OpenAI
 
 If you use the OpenAI model, you need an OpenAI API key. You can get it from [here](https://beta.openai.com/). Then you will be offered a choice of available models.
 
 <img width="300" alt="select" src="https://github.com/rsaryev/talk-codebase/assets/70219513/889ad7c8-a489-4ce8-83af-148b7df09229">
 
+
+Local
+
+<img width="696" alt="Снимок экрана 2023-07-12 в 03 47 58" src="https://github.com/rsaryev/talk-codebase/assets/70219513/16988911-c605-4570-bfb4-4a34a03cd4a1">
+
 If you want some files to be ignored, add them to .gitignore.
 
 ## Reset configuration
 
 To reset the configuration, run the following command:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `talk_codebase-0.1.43/pyproject.toml` & `talk_codebase-0.1.45/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.43"
+version = "0.1.45"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.43/talk_codebase/cli.py` & `talk_codebase-0.1.45/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.43/talk_codebase/config.py` & `talk_codebase-0.1.45/talk_codebase/config.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.43/talk_codebase/consts.py` & `talk_codebase-0.1.45/talk_codebase/consts.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,22 @@
                '.java', '.c', '.cpp', '.cs', '.go', '.php', '.rb', '.rs', '.swift', '.kt', '.scala', '.m', '.h',
                '.sh', '.pl', '.pm', '.lua', '.sql']
 EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
 MODEL_TYPES = {
     "OPENAI": "openai",
     "LOCAL": "local",
 }
-DEFAULT_LOCAL_MODEL = "orca-mini-3b.ggmlv3.q4_0.bin"
 DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all").replace("\\", "\\\\")
 
 DEFAULT_CONFIG = {
     "max_tokens": "2056",
     "chunk_size": "2056",
     "chunk_overlap": "256",
     "k": "1",
     "temperature": "0.7",
-    "local_model_name": DEFAULT_LOCAL_MODEL,
     "model_path": DEFAULT_MODEL_DIRECTORY,
     "n_batch": "8",
 }
 
 LOADER_MAPPING = {
     ".csv": {
         "loader": CSVLoader,
```

### Comparing `talk_codebase-0.1.43/talk_codebase/llm.py` & `talk_codebase-0.1.45/talk_codebase/llm.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.43/talk_codebase/utils.py` & `talk_codebase-0.1.45/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.43/PKG-INFO` & `talk_codebase-0.1.45/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.43
+Version: 0.1.45
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -46,19 +46,25 @@
 talk-codebase chat .
 ```
 
 Select model type: Local or OpenAI
 
 <img width="300" alt="select_type" src="https://github.com/rsaryev/talk-codebase/assets/70219513/05196fe5-78ff-44ff-8ca3-0313ccef572a">
 
+OpenAI
 
 If you use the OpenAI model, you need an OpenAI API key. You can get it from [here](https://beta.openai.com/). Then you will be offered a choice of available models.
 
 <img width="300" alt="select" src="https://github.com/rsaryev/talk-codebase/assets/70219513/889ad7c8-a489-4ce8-83af-148b7df09229">
 
+
+Local
+
+<img width="696" alt="Снимок экрана 2023-07-12 в 03 47 58" src="https://github.com/rsaryev/talk-codebase/assets/70219513/16988911-c605-4570-bfb4-4a34a03cd4a1">
+
 If you want some files to be ignored, add them to .gitignore.
 
 ## Reset configuration
 
 To reset the configuration, run the following command:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

