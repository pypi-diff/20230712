# Comparing `tmp/talk_codebase-0.1.42.tar.gz` & `tmp/talk_codebase-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.42.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.43.tar", max compression
```

## Comparing `talk_codebase-0.1.42.tar` & `talk_codebase-0.1.43.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3183 2023-07-05 11:00:37.949703 talk_codebase-0.1.42/README.md
--rw-r--r--   0        0        0      984 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/cli.py
--rw-r--r--   0        0        0     2250 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/config.py
--rw-r--r--   0        0        0     1946 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/consts.py
--rw-r--r--   0        0        0     4921 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/utils.py
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 talk_codebase-0.1.42/PKG-INFO
+-rw-r--r--   0        0        0     2762 2023-07-12 00:42:08.867523 talk_codebase-0.1.43/README.md
+-rw-r--r--   0        0        0      984 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/cli.py
+-rw-r--r--   0        0        0     3765 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/config.py
+-rw-r--r--   0        0        0     1860 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/consts.py
+-rw-r--r--   0        0        0     4921 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-12 00:42:08.871523 talk_codebase-0.1.43/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 talk_codebase-0.1.43/PKG-INFO
```

### Comparing `talk_codebase-0.1.42/README.md` & `talk_codebase-0.1.43/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,52 @@
-## talk-codebase 
+# talk-codebase
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
-* Simple configuration in just a couple of clicks
-* Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
-* It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
-* Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
+Talk-codebase is a tool that allows you to converse with your codebase using Large Language Models (LLMs) to answer your queries. It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you. Please note that talk-codebase is still under development and is recommended for educational purposes, not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
 
-To install talk-codebase, you need to have:
-
-* Python 3.9
-* An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
-
 ```bash
-# Install talk-codebase
 pip install talk-codebase
+```
+
+After installation, you can use it to chat with your codebase in the current directory by running the following command:
 
-# If you want some files to be ignored, add them to .gitignore.
-# Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
+```bash
 talk-codebase chat .
 ```
 
+Select model type: Local or OpenAI
+
+<img width="300" alt="select_type" src="https://github.com/rsaryev/talk-codebase/assets/70219513/05196fe5-78ff-44ff-8ca3-0313ccef572a">
+
+
+If you use the OpenAI model, you need an OpenAI API key. You can get it from [here](https://beta.openai.com/). Then you will be offered a choice of available models.
+
+<img width="300" alt="select" src="https://github.com/rsaryev/talk-codebase/assets/70219513/889ad7c8-a489-4ce8-83af-148b7df09229">
+
+If you want some files to be ignored, add them to .gitignore.
+
 ## Reset configuration
+
+To reset the configuration, run the following command:
+
 ```bash
-# If you want to reset the configuration, you can run the following command:
 talk-codebase configure
 ```
 
 ## Advanced configuration
 
-You can also edit the configuration manually by editing the `~/.config.yaml` file.
-If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
-the path to the configuration file.
-
-```yaml
-# The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
-api_key: sk-xxx
-
-# Configuration for chunking
-chunk_overlap: 50
-chunk_size: 500
-
-# Configuration for sampling
-k: 4
-max_tokens: 1048
-
-# Configuration for the LLM model
-openai_model_name: gpt-3.5-turbo
-# Type of model to use. You can choose between `openai` and `local`.
-model_type: openai
-local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
-# Path to local model. If you want to use a local model, you need to specify the path to it.
-model_path: 'absolute path to local model'
-```
+You can manually edit the configuration by editing the `~/.config.yaml` file. If you cannot find the configuration file, run the tool and it will output the path to the configuration file at the very beginning.
 
-## Supports the following extensions:
+## Supported Extensions
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
 - [x] `.epub`
 - [x] `.md`
 - [x] `.pdf`
```

### Comparing `talk_codebase-0.1.42/pyproject.toml` & `talk_codebase-0.1.43/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.42"
+version = "0.1.43"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.42/talk_codebase/consts.py` & `talk_codebase-0.1.43/talk_codebase/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,22 @@
                '.sh', '.pl', '.pm', '.lua', '.sql']
 EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
 MODEL_TYPES = {
     "OPENAI": "openai",
     "LOCAL": "local",
 }
 DEFAULT_LOCAL_MODEL = "orca-mini-3b.ggmlv3.q4_0.bin"
-DEFAULT_OPENAI_MODEL = "gpt-3.5-turbo"
 DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all").replace("\\", "\\\\")
 
 DEFAULT_CONFIG = {
     "max_tokens": "2056",
     "chunk_size": "2056",
     "chunk_overlap": "256",
     "k": "1",
     "temperature": "0.7",
-    "openai_model_name": DEFAULT_OPENAI_MODEL,
     "local_model_name": DEFAULT_LOCAL_MODEL,
     "model_path": DEFAULT_MODEL_DIRECTORY,
     "n_batch": "8",
 }
 
 LOADER_MAPPING = {
     ".csv": {
```

### Comparing `talk_codebase-0.1.42/talk_codebase/llm.py` & `talk_codebase-0.1.43/talk_codebase/llm.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.42/talk_codebase/utils.py` & `talk_codebase-0.1.43/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.42/PKG-INFO` & `talk_codebase-0.1.43/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.42
+Version: 0.1.43
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -21,76 +21,59 @@
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
-## talk-codebase 
+# talk-codebase
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
-* Simple configuration in just a couple of clicks
-* Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
-* It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
-* Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
+Talk-codebase is a tool that allows you to converse with your codebase using Large Language Models (LLMs) to answer your queries. It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you. Please note that talk-codebase is still under development and is recommended for educational purposes, not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
 
-To install talk-codebase, you need to have:
-
-* Python 3.9
-* An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
-
 ```bash
-# Install talk-codebase
 pip install talk-codebase
+```
+
+After installation, you can use it to chat with your codebase in the current directory by running the following command:
 
-# If you want some files to be ignored, add them to .gitignore.
-# Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
+```bash
 talk-codebase chat .
 ```
 
+Select model type: Local or OpenAI
+
+<img width="300" alt="select_type" src="https://github.com/rsaryev/talk-codebase/assets/70219513/05196fe5-78ff-44ff-8ca3-0313ccef572a">
+
+
+If you use the OpenAI model, you need an OpenAI API key. You can get it from [here](https://beta.openai.com/). Then you will be offered a choice of available models.
+
+<img width="300" alt="select" src="https://github.com/rsaryev/talk-codebase/assets/70219513/889ad7c8-a489-4ce8-83af-148b7df09229">
+
+If you want some files to be ignored, add them to .gitignore.
+
 ## Reset configuration
+
+To reset the configuration, run the following command:
+
 ```bash
-# If you want to reset the configuration, you can run the following command:
 talk-codebase configure
 ```
 
 ## Advanced configuration
 
-You can also edit the configuration manually by editing the `~/.config.yaml` file.
-If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
-the path to the configuration file.
-
-```yaml
-# The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
-api_key: sk-xxx
-
-# Configuration for chunking
-chunk_overlap: 50
-chunk_size: 500
-
-# Configuration for sampling
-k: 4
-max_tokens: 1048
-
-# Configuration for the LLM model
-openai_model_name: gpt-3.5-turbo
-# Type of model to use. You can choose between `openai` and `local`.
-model_type: openai
-local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
-# Path to local model. If you want to use a local model, you need to specify the path to it.
-model_path: 'absolute path to local model'
-```
+You can manually edit the configuration by editing the `~/.config.yaml` file. If you cannot find the configuration file, run the tool and it will output the path to the configuration file at the very beginning.
 
-## Supports the following extensions:
+## Supported Extensions
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
 - [x] `.epub`
 - [x] `.md`
 - [x] `.pdf`
```

