# Comparing `tmp/developergpt-0.2.5.tar.gz` & `tmp/developergpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.2.5.tar", last modified: Tue May  2 20:59:45 2023, max compression
+gzip compressed data, was "developergpt-0.3.0.tar", last modified: Wed Jul 12 00:22:29 2023, max compression
```

## Comparing `developergpt-0.2.5.tar` & `developergpt-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 20:59:33.000000 developergpt-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 20:59:33.000000 developergpt-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-02 20:59:45.329928 developergpt-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-02 20:59:33.000000 developergpt-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:59:45.329928 developergpt-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-02 20:59:33.000000 developergpt-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:29.023183 developergpt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 00:22:20.000000 developergpt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 00:22:20.000000 developergpt-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-07-12 00:22:29.023183 developergpt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-12 00:22:20.000000 developergpt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:29.023183 developergpt-0.3.0/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-07-12 00:22:20.000000 developergpt-0.3.0/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:29.023183 developergpt-0.3.0/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 00:22:28.000000 developergpt-0.3.0/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 00:22:29.023183 developergpt-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-12 00:22:20.000000 developergpt-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:29.023183 developergpt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:20.000000 developergpt-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 00:22:20.000000 developergpt-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 00:22:20.000000 developergpt-0.3.0/tests/test_cli.py
```

### Comparing `developergpt-0.2.5/LICENSE` & `developergpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.5/PKG-INFO` & `developergpt-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.5
+Version: 0.3.0
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
-[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
-
+[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model and GPT-4 from OpenAI. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
+From testing, OpenAI GPT models generally yield better results and are able to handle more complex requests compared to the BLOOM model. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
-
-With both models, it is always good practice to manually verify the command output before running it.
+From testing, the GPT-3.5 model is accurate for the majority of natural langauge to command requests and is significantly cheaper to use than GPT-4. The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. With all models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
-
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
 
-#### OpenAI GPT-3.5 (Default)
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
+#### OpenAI GPT Models
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use GPT-3.5 or GPT-4, you will need an OpenAI API Key.
 
 1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -101,40 +97,52 @@
 
 Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
 ```bash
 # Natural Language to Terminal Commands using BLOOM model instead
 $ developergpt --model bloom cmd [your natural language command request]
 ```
 
+Use `developergpt --model bloom cmd` to use the GPT-4 model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using GPT-4 model instead
+$ developergpt --model gpt-4 cmd [your natural language command request]
+```
+
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 
 # Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
 $ developergpt --model bloom cmd --fast [your natural language command request]
+
+# Fast Mode (GPT-4): Commands are given without explanation (may be less accurate)
+$ developergpt --model gpt-4 cmd --fast [your natural language command request]
 ```
 
 #### Chat inside the Terminal
-DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+DeveloperGPT allows you to chat with the GPT models or the BLOOM model in the terminal. 
 
 ```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
+
+# chat with DeveloperGPT using GPT-4
+$ developergpt --model gpt-4 chat
 ```
 
-**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
-### OpenAI API Usage (GPT-3.5)
+### OpenAI API Usage
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
-DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
+By default, DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT with GPT-3.5 should cost no more than 10 cents per day.
 
 ### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.2.5/README.md` & `developergpt-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
-[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
-
+[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model and GPT-4 from OpenAI. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
+From testing, OpenAI GPT models generally yield better results and are able to handle more complex requests compared to the BLOOM model. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
-
-With both models, it is always good practice to manually verify the command output before running it.
+From testing, the GPT-3.5 model is accurate for the majority of natural langauge to command requests and is significantly cheaper to use than GPT-4. The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. With all models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
-
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
 
-#### OpenAI GPT-3.5 (Default)
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
+#### OpenAI GPT Models
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use GPT-3.5 or GPT-4, you will need an OpenAI API Key.
 
 1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -90,40 +86,52 @@
 
 Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
 ```bash
 # Natural Language to Terminal Commands using BLOOM model instead
 $ developergpt --model bloom cmd [your natural language command request]
 ```
 
+Use `developergpt --model bloom cmd` to use the GPT-4 model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using GPT-4 model instead
+$ developergpt --model gpt-4 cmd [your natural language command request]
+```
+
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 
 # Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
 $ developergpt --model bloom cmd --fast [your natural language command request]
+
+# Fast Mode (GPT-4): Commands are given without explanation (may be less accurate)
+$ developergpt --model gpt-4 cmd --fast [your natural language command request]
 ```
 
 #### Chat inside the Terminal
-DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+DeveloperGPT allows you to chat with the GPT models or the BLOOM model in the terminal. 
 
 ```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
+
+# chat with DeveloperGPT using GPT-4
+$ developergpt --model gpt-4 chat
 ```
 
-**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
-### OpenAI API Usage (GPT-3.5)
+### OpenAI API Usage
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
-DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
+By default, DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT with GPT-3.5 should cost no more than 10 cents per day.
 
 ### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.2.5/developergpt/cli.py` & `developergpt-0.3.0/developergpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 @click.option(
     "--temperature",
     default=0.1,
     help="The temperature of the model response (higher means more creative, lower means more predictable)",
 )
 @click.option(
     "--model",
-    default="gpt-3.5",
-    help="The language model to use. Options: gpt-3.5 (default), bloom",
+    default="gpt-3.5-turbo",
+    help="The language model to use. Options: gpt-3.5-turbo (default), gpt-4, bloom",
 )
 @click.pass_context
 def main(ctx, temperature, model):
     model = model.lower().strip()
     if not utils.check_connectivity():
         console.print(
             "[bold red]No internet connection. Please check your internet connection and try again.[/bold red]"
@@ -64,15 +64,15 @@
         console.print(
             f"""[bold red]Model {model} is not supported. 
             Supported models: {",".join(config.SUPPORTED_MODELS)}[/bold red]"""
         )
         sys.exit(-1)
 
     ctx.ensure_object(dict)
-    if model == config.GPT35:
+    if model == config.GPT35 or model == config.GPT4:
         openai.api_key = config.get_environ_key(config.OPEN_AI_API_KEY, console)
         openai_adapter.check_open_ai_key(console)
     elif model == config.BLOOM:
         ctx.obj["api_key"] = config.get_environ_key_optional(
             config.HUGGING_FACE_API_KEY, console
         )
         console.print(
@@ -90,32 +90,32 @@
 def chat(ctx, user_input):
     if user_input:
         user_input = str(" ".join(user_input))
         session.history.append_string(user_input)
 
     model = ctx.obj["model"]
 
-    if model == config.GPT35:
+    if model == config.GPT35 or model == config.GPT4:
         input_messages = [openai_adapter.INITIAL_CHAT_SYSTEM_MSG]
     elif model == config.BLOOM:
         input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
         api_token = ctx.obj.get("api_key", None)
     console.print("[gray]Type 'quit' to exit the chat[/gray]")
     while True:
         if not user_input:
             user_input = utils.prompt_user_input(
                 "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
             )
 
         if not user_input:
             continue
 
-        if model == config.GPT35:
+        if model == config.GPT35 or model == config.GPT4:
             input_messages = openai_adapter.get_model_chat_response(
-                user_input, console, input_messages, ctx.obj["temperature"]
+                user_input, console, input_messages, ctx.obj["temperature"], model
             )
         elif model == config.BLOOM:
             input_messages = huggingface_adapter.get_model_chat_response(
                 user_input, console, input_messages, api_token
             )
 
         user_input = None
@@ -164,16 +164,18 @@
                 complete_style=CompleteStyle.MULTI_COLUMN,
                 key_bindings=config.kb,
             )
 
         if not user_input:
             continue
 
-        if model == config.GPT35:
-            model_output = openai_adapter.model_command(user_input, console, fast)
+        if model == config.GPT35 or model == config.GPT4:
+            model_output = openai_adapter.model_command(
+                user_input, console, fast, model
+            )
         elif model == config.BLOOM:
             model_output = huggingface_adapter.model_command(
                 user_input, console, api_token, fast
             )
         user_input = None  # clear input for next iteration
 
         commands = utils.print_command_response(model_output, console, fast, model)
```

### Comparing `developergpt-0.2.5/developergpt/config.py` & `developergpt-0.3.0/developergpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 INPUT_STYLE = Style.from_dict(
     {
         "prompt": "bold ansigreen",
     }
 )
 
 # supported models
-GPT35 = "gpt-3.5"
+GPT35 = "gpt-3.5-turbo"
+GPT4 = "gpt-4"
 BLOOM = "bloom"
-SUPPORTED_MODELS = set([GPT35, BLOOM])
+SUPPORTED_MODELS = set([GPT35, BLOOM, GPT4])
 
 OPEN_AI_API_KEY = "OPENAI_API_KEY"
 HUGGING_FACE_API_KEY = "HUGGING_FACE_API_KEY"
 
 FEEDBACK_LINK = "https://forms.gle/J36KbztsRAPHXnrKA"
 
 USER_PLATFORM = platform.platform()
```

### Comparing `developergpt-0.2.5/developergpt/few_shot_prompts.py` & `developergpt-0.3.0/developergpt/few_shot_prompts.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.5/developergpt/huggingface_adapter.py` & `developergpt-0.3.0/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.5/developergpt/openai_adapter.py` & `developergpt-0.3.0/developergpt/openai_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,29 +154,29 @@
 
 
 def get_model_chat_response(
     user_input: str,
     console: Console,
     input_messages: list,
     temperature: float,
+    model: str,
 ) -> list:
-    MODEL = "gpt-3.5-turbo"
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
 
     input_messages.append({"role": "user", "content": user_input})
     input_messages, n_input_tokens = utils.check_reduce_context(
-        input_messages, MAX_INPUT_TOKENS, MODEL, ctx_removal_index=1
+        input_messages, MAX_INPUT_TOKENS, model, ctx_removal_index=1
     )
     n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
 
     """Get the response from the model."""
     response = openai.ChatCompletion.create(
-        model=MODEL,
+        model=model,
         messages=input_messages,
         max_tokens=n_output_tokens,
         temperature=temperature,
         stream=True,
     )
 
     collected_messages = []
@@ -197,44 +197,48 @@
             )
 
     full_response = "".join(collected_messages)
     input_messages.append(format_assistant_response(full_response))
     return input_messages
 
 
-def model_command(user_input: str, console: Console, fast_mode: bool) -> list:
-    MODEL = "gpt-3.5-turbo"
+def model_command(
+    user_input: str,
+    console: Console,
+    fast_mode: bool,
+    model: str,
+) -> list:
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
     TEMP = 0.05
 
     if fast_mode:
         input_messages = list(BASE_INPUT_CMD_MSGS_FAST)
     else:
         input_messages = list(BASE_INPUT_CMD_MSGS)
 
     input_messages.append(format_user_request(user_input))
 
-    n_input_tokens = utils.count_msg_tokens(input_messages, MODEL)
+    n_input_tokens = utils.count_msg_tokens(input_messages, model)
 
     if n_input_tokens > MAX_INPUT_TOKENS:
         input_messages, n_input_tokens = utils.remove_old_contexts(
             input_messages,
             MAX_INPUT_TOKENS,
             n_input_tokens,
-            MODEL,
+            model,
             ctx_removal_index=2,
         )
 
     n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
 
     with console.status("[bold blue]Decoding request") as _:
         response = openai.ChatCompletion.create(
-            model=MODEL,
+            model=model,
             messages=input_messages,
             max_tokens=n_output_tokens,
             temperature=TEMP,
         )
 
     model_output = response["choices"][0]["message"]["content"].strip()
```

### Comparing `developergpt-0.2.5/developergpt/utils.py` & `developergpt-0.3.0/developergpt/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,34 +145,37 @@
     """
     Returns the approximate number of tokens used by a list of messages
     function adapted from: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     """
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
-        # print("Warning: model not found. Using cl100k_base encoding.")
+        print("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model == "gpt-3.5-turbo":
-        # print(
-        #     "Warning: gpt-3.5-turbo may change over time. Returning num tokens assuming gpt-3.5-turbo-0301."
-        # )
-        return count_msg_tokens(messages, model="gpt-3.5-turbo-0301")
-    elif model == "gpt-4":
-        # print(
-        #     "Warning: gpt-4 may change over time. Returning num tokens assuming gpt-4-0314."
-        # )
-        return count_msg_tokens(messages, model="gpt-4-0314")
+    if model in {
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k-0613",
+        "gpt-4-0314",
+        "gpt-4-32k-0314",
+        "gpt-4-0613",
+        "gpt-4-32k-0613",
+    }:
+        tokens_per_message = 3
+        tokens_per_name = 1
     elif model == "gpt-3.5-turbo-0301":
         tokens_per_message = (
             4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         )
         tokens_per_name = -1  # if there's a name, the role is omitted
-    elif model == "gpt-4-0314":
-        tokens_per_message = 3
-        tokens_per_name = 1
+    elif "gpt-3.5-turbo" in model:
+        # print("Warning: gpt-3.5-turbo may update over time. Returning num tokens assuming gpt-3.5-turbo-0613.")
+        return count_msg_tokens(messages, model="gpt-3.5-turbo-0613")
+    elif "gpt-4" in model:
+        # print("Warning: gpt-4 may update over time. Returning num tokens assuming gpt-4-0613.")
+        return count_msg_tokens(messages, model="gpt-4-0613")
     else:
         raise NotImplementedError(
             f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
         )
     num_tokens = 0
     for message in messages:
         num_tokens += tokens_per_message
```

### Comparing `developergpt-0.2.5/developergpt.egg-info/PKG-INFO` & `developergpt-0.3.0/developergpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.5
+Version: 0.3.0
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
-[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
-
+[![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model and GPT-4 from OpenAI. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
+From testing, OpenAI GPT models generally yield better results and are able to handle more complex requests compared to the BLOOM model. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
-
-With both models, it is always good practice to manually verify the command output before running it.
+From testing, the GPT-3.5 model is accurate for the majority of natural langauge to command requests and is significantly cheaper to use than GPT-4. The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. With all models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
-**Supported Models:** GPT3.5 (default), BLOOM
+**Supported Models:** GPT-3.5 (default), GPT-4, BLOOM
 
 **Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
-
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
 
-#### OpenAI GPT-3.5 (Default)
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
+#### OpenAI GPT Models
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use GPT-3.5 or GPT-4, you will need an OpenAI API Key.
 
 1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -101,40 +97,52 @@
 
 Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
 ```bash
 # Natural Language to Terminal Commands using BLOOM model instead
 $ developergpt --model bloom cmd [your natural language command request]
 ```
 
+Use `developergpt --model bloom cmd` to use the GPT-4 model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using GPT-4 model instead
+$ developergpt --model gpt-4 cmd [your natural language command request]
+```
+
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 
 # Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
 $ developergpt --model bloom cmd --fast [your natural language command request]
+
+# Fast Mode (GPT-4): Commands are given without explanation (may be less accurate)
+$ developergpt --model gpt-4 cmd --fast [your natural language command request]
 ```
 
 #### Chat inside the Terminal
-DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+DeveloperGPT allows you to chat with the GPT models or the BLOOM model in the terminal. 
 
 ```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
+
+# chat with DeveloperGPT using GPT-4
+$ developergpt --model gpt-4 chat
 ```
 
-**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
-### OpenAI API Usage (GPT-3.5)
+### OpenAI API Usage
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
-DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
+By default, DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT with GPT-3.5 should cost no more than 10 cents per day.
 
 ### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.2.5/developergpt.egg-info/SOURCES.txt` & `developergpt-0.3.0/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.5/setup.py` & `developergpt-0.3.0/setup.py`

 * *Files identical despite different names*

