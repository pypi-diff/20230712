# Comparing `tmp/aider-chat-0.8.2.tar.gz` & `tmp/aider-chat-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.8.2.tar", last modified: Sat Jul  8 13:10:32 2023, max compression
+gzip compressed data, was "aider-chat-0.8.3.tar", last modified: Wed Jul 12 01:48:36 2023, max compression
```

## Comparing `aider-chat-0.8.2.tar` & `aider-chat-0.8.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-08 13:10:22.000000 aider-chat-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 13:10:22.000000 aider-chat-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 13:10:32.455631 aider-chat-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-08 13:10:22.000000 aider-chat-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.451631 aider-chat-0.8.2/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.451631 aider-chat-0.8.2/aider/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34402 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/base_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/single_wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/single_wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/prompts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/rungrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 13:10:22.000000 aider-chat-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:10:32.455631 aider-chat-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-08 13:10:22.000000 aider-chat-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_editblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_wholefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-12 01:48:26.000000 aider-chat-0.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 01:48:26.000000 aider-chat-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-12 01:48:36.224317 aider-chat-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-12 01:48:26.000000 aider-chat-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.220317 aider-chat-0.8.3/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34993 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/single_wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/single_wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/prompts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/rungrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 01:48:26.000000 aider-chat-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:48:36.224317 aider-chat-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-12 01:48:26.000000 aider-chat-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_wholefile.py
```

### Comparing `aider-chat-0.8.2/LICENSE.txt` & `aider-chat-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/PKG-INFO` & `aider-chat-0.8.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-Metadata-Version: 2.1
-Name: aider-chat
-Version: 0.8.2
-Summary: aider is GPT powered coding in your terminal
-Home-page: https://github.com/paul-gauthier/aider
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
+Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
+![aider screencast](assets/screencast.svg)
 
+- [Getting started](#getting-started)
+- [Example chat transcripts](#example-chat-transcripts)
+- [Features](#features)
+- [Usage](#usage)
+- [In-chat commands](#in-chat-commands)
+- [Tips](#tips)
+- [GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35)
+- [Installation](https://aider.chat/docs/install.html)
 - [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
+See the
+[installation instructions](https://aider.chat/docs/install.html)
+for more details, but you can
+get started quickly like this:
+
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider myapp.py
+$ aider app.py
 
 Using git repo: .git
-Added myapp.py to the chat.
+Added app.py to the chat.
 
-myapp.py> change the fibonacci function from recursion to iteration
+app.py> make a flask app that replies "hello world" on /hello
 ```
 
 ## Example chat transcripts
 
-Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4. 
+Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
 
 * [**Javascript Game Modification**](https://aider.chat/examples/2048-game.html): Dive into an existing open-source repo, and get GPT's help to understand it and make modifications.
 
 * [**Complex Multi-file Change with Debugging**](https://aider.chat/examples/complex-change.html): GPT makes a complex code change that is coordinated across multiple source files, and resolves bugs by reviewing error output and doc snippets.
 
@@ -52,29 +58,14 @@
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
-## Installation
-
-1. Install the package with pip:
-  * PyPI: `python -m pip install aider-chat`
-  * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
-  * Local clone: `python -m pip install -e .` 
-
-2. Set up your OpenAI API key:
-  * As an environment variable:
-    * `export OPENAI_API_KEY=sk-...` on Linux or Mac
-    * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
-
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
-
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
@@ -113,69 +104,45 @@
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
 
 ## Tips
 
 * Think about which files need to be edited to make your change and add them to the chat.
-Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are able to structure code edits as simple "diffs"
-and use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact "diff" format.
-So aider has
-to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
-This rapidly uses up tokens and can hit the limits of the context window.
-
-For more detailed information and a quantitative comparison, here are
-[code editing benchmark results for GPT-3.5 and GPT-4](https://aider.chat/docs/benchmarks.html).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
-
-In practice, this means you can use aider to edit a set of source files
-that total up to the sizes below.
-You can (and should) add just the specific set of files to the chat
-that are relevant to the change you are requesting.
-This minimizes your use of the context window, as well as costs.
-
-| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
-| ----------------- | -- | --     | -----| -- | -- |
-| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
-| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
-| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
-| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
 
 ## Kind words from users
 
 * "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
+
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models.
+You can choose a model with the `--model` command line argument.
+
+You should probably use GPT-4 if you can. For more details see the
+[FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
+
+For a discussion of using other non-OpenAI models, see the
+[FAQ about other LLMs](https://aider.chat/docs/faq.html#can-i-use-aider-with-other-llms-local-llms-etc).
+
+## Installation
+
+See the [installation instructions](https://aider.chat/docs/install.html).
+
+## FAQ
 
+For more information, see the [FAQ](https://aider.chat/docs/faq.html).
```

### Comparing `aider-chat-0.8.2/README.md` & `aider-chat-0.8.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,46 @@
+Metadata-Version: 2.1
+Name: aider-chat
+Version: 0.8.3
+Summary: aider is GPT powered coding in your terminal
+Home-page: https://github.com/paul-gauthier/aider
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
+Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
-![aider screencast](assets/screencast.svg)
 
-- [Getting started](#getting-started)
-- [Example chat transcripts](#example-chat-transcripts)
-- [Features](#features)
-- [Installation](#installation)
-- [Usage](#usage)
-- [In-chat commands](#in-chat-commands)
-- [Tips](#tips)
-- [GPT-4 vs GPT-3.5](#gpt-4-vs-gpt-35)
-- [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
+See the
+[installation instructions](https://aider.chat/docs/install.html)
+for more details, but you can
+get started quickly like this:
+
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider myapp.py
+$ aider app.py
 
 Using git repo: .git
-Added myapp.py to the chat.
+Added app.py to the chat.
 
-myapp.py> change the fibonacci function from recursion to iteration
+app.py> make a flask app that replies "hello world" on /hello
 ```
 
 ## Example chat transcripts
 
-Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4. 
+Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
 
 * [**Javascript Game Modification**](https://aider.chat/examples/2048-game.html): Dive into an existing open-source repo, and get GPT's help to understand it and make modifications.
 
 * [**Complex Multi-file Change with Debugging**](https://aider.chat/examples/complex-change.html): GPT makes a complex code change that is coordinated across multiple source files, and resolves bugs by reviewing error output and doc snippets.
 
@@ -53,29 +56,14 @@
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
-## Installation
-
-1. Install the package with pip:
-  * PyPI: `python -m pip install aider-chat`
-  * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
-  * Local clone: `python -m pip install -e .` 
-
-2. Set up your OpenAI API key:
-  * As an environment variable:
-    * `export OPENAI_API_KEY=sk-...` on Linux or Mac
-    * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
-
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
-
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
@@ -114,69 +102,45 @@
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
 
 ## Tips
 
 * Think about which files need to be edited to make your change and add them to the chat.
-Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are able to structure code edits as simple "diffs"
-and use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact "diff" format.
-So aider has
-to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
-This rapidly uses up tokens and can hit the limits of the context window.
-
-For more detailed information and a quantitative comparison, here are
-[code editing benchmark results for GPT-3.5 and GPT-4](https://aider.chat/docs/benchmarks.html).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
-
-In practice, this means you can use aider to edit a set of source files
-that total up to the sizes below.
-You can (and should) add just the specific set of files to the chat
-that are relevant to the change you are requesting.
-This minimizes your use of the context window, as well as costs.
-
-| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
-| ----------------- | -- | --     | -----| -- | -- |
-| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
-| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
-| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
-| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
 
 ## Kind words from users
 
 * "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
+
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models.
+You can choose a model with the `--model` command line argument.
+
+You should probably use GPT-4 if you can. For more details see the
+[FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
+
+For a discussion of using other non-OpenAI models, see the
+[FAQ about other LLMs](https://aider.chat/docs/faq.html#can-i-use-aider-with-other-llms-local-llms-etc).
+
+## Installation
+
+See the [installation instructions](https://aider.chat/docs/install.html).
+
+## FAQ
 
+For more information, see the [FAQ](https://aider.chat/docs/faq.html).
```

### Comparing `aider-chat-0.8.2/aider/coders/base_coder.py` & `aider-chat-0.8.3/aider/coders/base_coder.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
         if use_git:
             self.set_repo(fnames)
         else:
             self.abs_fnames = set([str(Path(fname).resolve()) for fname in fnames])
 
         if self.repo:
-            rel_repo_dir = os.path.relpath(self.repo.git_dir, os.getcwd())
+            rel_repo_dir = self.get_rel_repo_dir()
             self.io.tool_output(f"Git repo: {rel_repo_dir}")
         else:
             self.io.tool_output("Git repo: none")
             self.find_common_root()
 
         if main_model.use_repo_map and self.repo and self.gpt_prompts.repo_content_prefix:
             self.repo_map = RepoMap(
@@ -206,14 +206,20 @@
         elif self.abs_fnames:
             self.root = os.path.commonpath(list(self.abs_fnames))
         else:
             self.root = os.getcwd()
 
         self.root = utils.safe_abs_path(self.root)
 
+    def get_rel_repo_dir(self):
+        try:
+            return os.path.relpath(self.repo.git_dir, os.getcwd())
+        except ValueError:
+            return self.repo.git_dir
+
     def add_rel_fname(self, rel_fname):
         self.abs_fnames.add(self.abs_root_path(rel_fname))
 
     def abs_root_path(self, path):
         res = Path(self.root) / path
         return utils.safe_abs_path(res)
 
@@ -261,15 +267,15 @@
             relative_fname = self.get_rel_fname(fname)
 
             tracked_files = set(self.get_tracked_files())
             if relative_fname not in tracked_files:
                 new_files.append(relative_fname)
 
         if new_files:
-            rel_repo_dir = os.path.relpath(self.repo.git_dir, os.getcwd())
+            rel_repo_dir = self.get_rel_repo_dir()
 
             self.io.tool_output(f"Files not tracked in {rel_repo_dir}:")
             for fn in new_files:
                 self.io.tool_output(f" - {fn}")
             if self.io.confirm_ask("Add them?"):
                 for relative_fname in new_files:
                     self.repo.git.add(relative_fname)
@@ -392,17 +398,21 @@
                 if self.num_control_c >= 2:
                     break
                 self.io.tool_error("^C again or /exit to quit")
             except EOFError:
                 return
 
     def should_dirty_commit(self, inp):
-        is_commit_command = inp and inp.startswith("/commit")
-        if is_commit_command:
-            return
+        cmds = self.commands.matching_commands(inp)
+        if cmds:
+            matching_commands, _, _ = cmds
+            if len(matching_commands) == 1:
+                cmd = matching_commands[0]
+                if cmd in ("/exit", "/commit"):
+                    return
 
         if not self.dirty_commits:
             return
         if not self.repo:
             return
         if not self.repo.is_dirty():
             return
@@ -426,14 +436,15 @@
             self.get_addable_relative_files(),
             self.commands,
         )
 
         self.num_control_c = 0
 
         if self.should_dirty_commit(inp):
+            self.io.tool_output("Git repo has uncommitted changes, preparing commit...")
             self.commit(ask=True, which="repo_files")
 
             # files changed, move cur messages back behind the files messages
             self.move_back_cur_messages(self.gpt_prompts.files_content_local_edits)
 
             if inp.strip():
                 self.io.tool_output("Use up-arrow to retry previous command:", inp)
@@ -602,15 +613,15 @@
         (
             Timeout,
             APIError,
             ServiceUnavailableError,
             RateLimitError,
             requests.exceptions.ConnectionError,
         ),
-        max_tries=5,
+        max_tries=10,
         on_backoff=lambda details: print(f"Retry in {details['wait']} seconds."),
     )
     def send_with_retries(self, model, messages, functions):
         kwargs = dict(
             model=model,
             messages=messages,
             temperature=0,
@@ -757,17 +768,16 @@
 
     def render_incremental_response(self, final):
         return self.partial_response_content
 
     def get_context_from_history(self, history):
         context = ""
         if history:
-            context += "# Context:\n"
             for msg in history:
-                context += msg["role"].upper() + ": " + msg["content"] + "\n"
+                context += "\n" + msg["role"].upper() + ": " + msg["content"] + "\n"
         return context
 
     def get_commit_message(self, diffs, context):
         if len(diffs) >= 4 * 1024 * 4:
             self.io.tool_error(
                 f"Diff is too large for {models.GPT35.name} to generate a commit message."
             )
@@ -887,15 +897,15 @@
                 self.io.tool_error("Skipped commmit.")
                 return
             if res.lower() not in ["y", "yes"] and res:
                 commit_message = res
 
         repo.git.add(*relative_dirty_fnames)
 
-        full_commit_message = commit_message + "\n\n" + context
+        full_commit_message = commit_message + "\n\n# Aider chat conversation:\n\n" + context
         repo.git.commit("-m", full_commit_message, "--no-verify")
         commit_hash = repo.head.commit.hexsha[:7]
         self.io.tool_output(f"Commit {commit_hash} {commit_message}")
 
         return commit_hash, commit_message
 
     def get_rel_fname(self, fname):
@@ -961,17 +971,28 @@
             self.io.write_text(full_path, write_content)
 
         return full_path
 
     def get_tracked_files(self):
         if not self.repo:
             return []
+
+        try:
+            commit = self.repo.head.commit
+        except ValueError:
+            return set()
+
+        files = []
+        for blob in commit.tree.traverse():
+            if blob.type == "blob":  # blob is a file
+                files.append(blob.path)
+
         # convert to appropriate os.sep, since git always normalizes to /
-        files = set(self.repo.git.ls_files().splitlines())
         res = set(str(Path(PurePosixPath(path))) for path in files)
+
         return res
 
     apply_update_errors = 0
 
     def apply_updates(self):
         max_apply_update_errors = 2
```

### Comparing `aider-chat-0.8.2/aider/coders/editblock_coder.py` & `aider-chat-0.8.3/aider/coders/editblock_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/editblock_func_coder.py` & `aider-chat-0.8.3/aider/coders/editblock_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/editblock_func_prompts.py` & `aider-chat-0.8.3/aider/coders/editblock_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/editblock_prompts.py` & `aider-chat-0.8.3/aider/coders/editblock_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/single_wholefile_func_coder.py` & `aider-chat-0.8.3/aider/coders/single_wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/single_wholefile_func_prompts.py` & `aider-chat-0.8.3/aider/coders/single_wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/wholefile_coder.py` & `aider-chat-0.8.3/aider/coders/wholefile_coder.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,55 +34,59 @@
             return self.update_files(mode="diff")
         except ValueError:
             return self.partial_response_content
 
     def update_files(self, mode="update"):
         content = self.partial_response_content
 
-        edited = set()
         chat_files = self.get_inchat_relative_files()
 
         output = []
         lines = content.splitlines(keepends=True)
 
+        edits = []
+
         saw_fname = None
         fname = None
+        fname_source = None
         new_lines = []
         for i, line in enumerate(lines):
             if line.startswith(self.fence[0]) or line.startswith(self.fence[1]):
                 if fname is not None:
                     # ending an existing block
                     saw_fname = None
 
                     full_path = (Path(self.root) / fname).absolute()
 
                     if mode == "diff":
-                        output += self.do_live_diff(full_path, new_lines)
-                    elif self.allowed_to_edit(fname):
-                        edited.add(fname)
-                        new_lines = "".join(new_lines)
-                        self.io.write_text(full_path, new_lines)
+                        output += self.do_live_diff(full_path, new_lines, True)
+                    else:
+                        edits.append((fname, fname_source, new_lines))
 
                     fname = None
+                    fname_source = None
                     new_lines = []
                     continue
 
                 # fname==None ... starting a new block
                 if i > 0:
+                    fname_source = "block"
                     fname = lines[i - 1].strip()
                     # Did gpt prepend a bogus dir? It especially likes to
                     # include the path/to prefix from the one-shot example in
                     # the prompt.
                     if fname and fname not in chat_files and Path(fname).name in chat_files:
                         fname = Path(fname).name
                 if not fname:  # blank line? or ``` was on first line i==0
                     if saw_fname:
                         fname = saw_fname
+                        fname_source = "saw"
                     elif len(chat_files) == 1:
                         fname = chat_files[0]
+                        fname_source = "chat"
                     else:
                         # TODO: sense which file it is by diff size
                         raise ValueError(
                             f"No filename provided before {self.fence[0]} in file listing"
                         )
 
             elif fname is not None:
@@ -97,33 +101,44 @@
 
                 output.append(line)
 
         if mode == "diff":
             if fname is not None:
                 # ending an existing block
                 full_path = (Path(self.root) / fname).absolute()
-                output += self.do_live_diff(full_path, new_lines)
+                output += self.do_live_diff(full_path, new_lines, False)
             return "\n".join(output)
 
         if fname:
-            full_path = self.allowed_to_edit(fname)
-            if full_path:
-                edited.add(fname)
+            edits.append((fname, fname_source, new_lines))
+
+        edited = set()
+        # process from most reliable filename, to least reliable
+        for source in ("block", "saw", "chat"):
+            for fname, fname_source, new_lines in edits:
+                if fname_source != source:
+                    continue
+                # if a higher priority source already edited the file, skip
+                if fname in edited:
+                    continue
+
+                # we have a winner
                 new_lines = "".join(new_lines)
-                self.io.write_text(full_path, new_lines)
+                if self.allowed_to_edit(fname, new_lines):
+                    edited.add(fname)
 
         return edited
 
-    def do_live_diff(self, full_path, new_lines):
+    def do_live_diff(self, full_path, new_lines, final):
         if full_path.exists():
             orig_lines = self.io.read_text(full_path).splitlines(keepends=True)
 
             show_diff = diffs.diff_partial_update(
                 orig_lines,
                 new_lines,
-                final=True,
+                final=final,
             ).splitlines()
             output = show_diff
         else:
             output = ["```"] + new_lines + ["```"]
 
         return output
```

### Comparing `aider-chat-0.8.2/aider/coders/wholefile_func_coder.py` & `aider-chat-0.8.3/aider/coders/wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/wholefile_func_prompts.py` & `aider-chat-0.8.3/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/coders/wholefile_prompts.py` & `aider-chat-0.8.3/aider/coders/wholefile_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/commands.py` & `aider-chat-0.8.3/aider/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,30 +42,37 @@
         cmd_method_name = f"cmd_{cmd_name}"
         cmd_method = getattr(self, cmd_method_name, None)
         if cmd_method:
             return cmd_method(args)
         else:
             self.io.tool_output(f"Error: Command {cmd_name} not found.")
 
-    def run(self, inp):
+    def matching_commands(self, inp):
         words = inp.strip().split()
         if not words:
             return
 
         first_word = words[0]
         rest_inp = inp[len(words[0]) :]
 
         all_commands = self.get_commands()
         matching_commands = [cmd for cmd in all_commands if cmd.startswith(first_word)]
+        return matching_commands, first_word, rest_inp
+
+    def run(self, inp):
+        res = self.matching_commands(inp)
+        if res is None:
+            return
+        matching_commands, first_word, rest_inp = res
         if len(matching_commands) == 1:
             return self.do_run(matching_commands[0][1:], rest_inp)
         elif len(matching_commands) > 1:
             self.io.tool_error(f"Ambiguous command: {', '.join(matching_commands)}")
         else:
-            self.io.tool_error(f"Error: {first_word} is not a valid command.")
+            self.io.tool_error(f"Invalid command: {first_word}")
 
     # any method called cmd_xxx becomes a command automatically.
     # each one must take an args param.
 
     def cmd_commit(self, args):
         "Commit edits to the repo made outside the chat (commit message optional)"
 
@@ -217,63 +224,73 @@
         files = set(self.coder.get_all_relative_files())
         files = files - set(self.coder.get_inchat_relative_files())
         for fname in files:
             if partial.lower() in fname.lower():
                 yield Completion(fname, start_position=-len(partial))
 
     def glob_filtered_to_repo(self, pattern):
-        matched_files = Path(self.coder.root).glob(pattern)
-        matched_files = [fn.relative_to(self.coder.root) for fn in matched_files]
+        raw_matched_files = list(Path(self.coder.root).glob(pattern))
+
+        matched_files = []
+        for fn in raw_matched_files:
+            matched_files += expand_subdir(fn.relative_to(self.coder.root))
 
         # if repo, filter against it
         if self.coder.repo:
             git_files = self.coder.get_tracked_files()
             matched_files = [fn for fn in matched_files if str(fn) in git_files]
 
-        return list(map(str, matched_files))
+        res = list(map(str, matched_files))
+        return res
 
     def cmd_add(self, args):
         "Add matching files to the chat session using glob patterns"
 
         added_fnames = []
         git_added = []
         git_files = self.coder.get_tracked_files()
 
+        all_matched_files = set()
         for word in args.split():
             matched_files = self.glob_filtered_to_repo(word)
 
             if not matched_files:
                 if any(char in word for char in "*?[]"):
                     self.io.tool_error(f"No files to add matching pattern: {word}")
                 else:
                     if Path(word).exists():
-                        matched_files = [word]
+                        if Path(word).is_file():
+                            matched_files = [word]
+                        else:
+                            self.io.tool_error(f"Unable to add: {word}")
                     elif self.io.confirm_ask(
                         f"No files matched '{word}'. Do you want to create the file?"
                     ):
                         (Path(self.coder.root) / word).touch()
                         matched_files = [word]
 
-            for matched_file in matched_files:
-                abs_file_path = self.coder.abs_root_path(matched_file)
+            all_matched_files.update(matched_files)
 
-                if self.coder.repo and matched_file not in git_files:
-                    self.coder.repo.git.add(abs_file_path)
-                    git_added.append(matched_file)
-
-                if abs_file_path not in self.coder.abs_fnames:
-                    content = self.io.read_text(abs_file_path)
-                    if content is not None:
-                        self.coder.abs_fnames.add(abs_file_path)
-                        self.io.tool_output(f"Added {matched_file} to the chat")
-                        added_fnames.append(matched_file)
-                    else:
-                        self.io.tool_error(f"Unable to read {matched_file}")
+        for matched_file in all_matched_files:
+            abs_file_path = self.coder.abs_root_path(matched_file)
+
+            if self.coder.repo and matched_file not in git_files:
+                self.coder.repo.git.add(abs_file_path)
+                git_added.append(matched_file)
+
+            if abs_file_path in self.coder.abs_fnames:
+                self.io.tool_error(f"{matched_file} is already in the chat")
+            else:
+                content = self.io.read_text(abs_file_path)
+                if content is None:
+                    self.io.tool_error(f"Unable to read {matched_file}")
                 else:
-                    self.io.tool_error(f"{matched_file} is already in the chat")
+                    self.coder.abs_fnames.add(abs_file_path)
+                    self.io.tool_output(f"Added {matched_file} to the chat")
+                    added_fnames.append(matched_file)
 
         if self.coder.repo and git_added:
             git_added = " ".join(git_added)
             commit_message = f"aider: Added {git_added}"
             self.coder.repo.git.commit("-m", commit_message, "--no-verify")
             commit_hash = self.coder.repo.head.commit.hexsha[:7]
             self.io.tool_output(f"Commit {commit_hash} {commit_message}")
@@ -376,7 +393,18 @@
             cmd_method_name = f"cmd_{cmd[1:]}"
             cmd_method = getattr(self, cmd_method_name, None)
             if cmd_method:
                 description = cmd_method.__doc__
                 self.io.tool_output(f"{cmd} {description}")
             else:
                 self.io.tool_output(f"{cmd} No description available.")
+
+
+def expand_subdir(file_path):
+    file_path = Path(file_path)
+    if file_path.is_file():
+        yield file_path
+        return
+
+    for file in file_path.rglob("*"):
+        if file.is_file():
+            yield str(file)
```

### Comparing `aider-chat-0.8.2/aider/diffs.py` & `aider-chat-0.8.3/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/dump.py` & `aider-chat-0.8.3/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/io.py` & `aider-chat-0.8.3/aider/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 from rich.console import Console
 from rich.text import Text
 
 from .dump import dump  # noqa: F401
 
 
 class AutoCompleter(Completer):
-    def __init__(self, root, rel_fnames, addable_rel_fnames, commands):
+    def __init__(self, root, rel_fnames, addable_rel_fnames, commands, encoding):
         self.commands = commands
         self.addable_rel_fnames = addable_rel_fnames
         self.rel_fnames = rel_fnames
+        self.encoding = encoding
 
         fname_to_rel_fnames = defaultdict(list)
         for rel_fname in addable_rel_fnames:
             fname = os.path.basename(rel_fname)
             if fname != rel_fname:
                 fname_to_rel_fnames[fname].append(rel_fname)
         self.fname_to_rel_fnames = fname_to_rel_fnames
@@ -34,17 +35,17 @@
 
         for rel_fname in addable_rel_fnames:
             self.words.add(rel_fname)
 
         for rel_fname in rel_fnames:
             self.words.add(rel_fname)
 
-            fname = os.path.join(root, rel_fname)
+            fname = Path(root) / rel_fname
             try:
-                with open(fname, "r") as f:
+                with open(fname, "r", encoding=self.encoding) as f:
                     content = f.read()
             except FileNotFoundError:
                 continue
             try:
                 lexer = guess_lexer_for_filename(fname, content)
             except ClassNotFound:
                 continue
@@ -177,15 +178,17 @@
                     "pygments.literal.string": f"bold italic {self.user_input_color}",
                 }
             )
         else:
             style = None
 
         while True:
-            completer_instance = AutoCompleter(root, rel_fnames, addable_rel_fnames, commands)
+            completer_instance = AutoCompleter(
+                root, rel_fnames, addable_rel_fnames, commands, self.encoding
+            )
             if multiline_input:
                 show = ". "
 
             session_kwargs = {
                 "message": show,
                 "completer": completer_instance,
                 "reserve_space_for_menu": 4,
@@ -303,9 +306,9 @@
             text = "> " + text
         if linebreak:
             text = text.rstrip()
             text = text + "  \n"
         if not text.endswith("\n"):
             text += "\n"
         if self.chat_history_file is not None:
-            with self.chat_history_file.open("a") as f:
+            with self.chat_history_file.open("a", encoding=self.encoding) as f:
                 f.write(text)
```

### Comparing `aider-chat-0.8.2/aider/main.py` & `aider-chat-0.8.3/aider/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,240 +38,278 @@
         description="aider is GPT powered coding in your terminal",
         add_config_file_help=True,
         default_config_files=default_config_files,
         config_file_parser_class=configargparse.YAMLConfigFileParser,
         auto_env_var_prefix="AIDER_",
     )
 
-    parser.add_argument(
-        "--version",
-        action="version",
-        version=f"%(prog)s {__version__}",
-        help="Show the version number and exit",
-    )
-
-    parser.add_argument(
-        "-c",
-        "--config",
-        is_config_file=True,
-        metavar="CONFIG_FILE",
-        help=(
-            "Specify the config file (default: search for .aider.conf.yml in git root, cwd"
-            " or home directory)"
-        ),
-    )
-
-    parser.add_argument(
+    ##########
+    core_group = parser.add_argument_group("Main")
+    core_group.add_argument(
         "files",
         metavar="FILE",
         nargs="*",
-        help="a list of source code files (optional)",
+        help="a list of source code files to edit with GPT (optional)",
     )
+    core_group.add_argument(
+        "--openai-api-key",
+        metavar="OPENAI_API_KEY",
+        help="Specify the OpenAI API key",
+        env_var="OPENAI_API_KEY",
+    )
+    core_group.add_argument(
+        "--model",
+        metavar="MODEL",
+        default=models.GPT4.name,
+        help=f"Specify the model to use for the main chat (default: {models.GPT4.name})",
+    )
+    core_group.add_argument(
+        "-3",
+        action="store_const",
+        dest="model",
+        const=models.GPT35_16k.name,
+        help=f"Use {models.GPT35_16k.name} model for the main chat (gpt-4 is better)",
+    )
+
+    ##########
+    model_group = parser.add_argument_group("Advanced Model Settings")
+    model_group.add_argument(
+        "--openai-api-base",
+        metavar="OPENAI_API_BASE",
+        default="https://api.openai.com/v1",
+        help="Specify the OpenAI API base endpoint (default: https://api.openai.com/v1)",
+    )
+    model_group.add_argument(
+        "--edit-format",
+        metavar="EDIT_FORMAT",
+        default=None,
+        help="Specify what edit format GPT should use (default depends on model)",
+    )
+    model_group.add_argument(
+        "--map-tokens",
+        type=int,
+        default=1024,
+        help="Max number of tokens to use for repo map, use 0 to disable (default: 1024)",
+    )
+
+    ##########
+    history_group = parser.add_argument_group("History Files")
     default_input_history_file = (
         os.path.join(git_root, ".aider.input.history") if git_root else ".aider.input.history"
     )
     default_chat_history_file = (
         os.path.join(git_root, ".aider.chat.history.md") if git_root else ".aider.chat.history.md"
     )
-
-    parser.add_argument(
+    history_group.add_argument(
         "--input-history-file",
         metavar="INPUT_HISTORY_FILE",
         default=default_input_history_file,
         help=f"Specify the chat input history file (default: {default_input_history_file})",
     )
-    parser.add_argument(
+    history_group.add_argument(
         "--chat-history-file",
         metavar="CHAT_HISTORY_FILE",
         default=default_chat_history_file,
         help=f"Specify the chat history file (default: {default_chat_history_file})",
     )
-    parser.add_argument(
-        "--model",
-        metavar="MODEL",
-        default=models.GPT4.name,
-        help=f"Specify the model to use for the main chat (default: {models.GPT4.name})",
-    )
-    parser.add_argument(
-        "-3",
-        action="store_const",
-        dest="model",
-        const=models.GPT35_16k.name,
-        help=f"Use {models.GPT35_16k.name} model for the main chat (gpt-4 is better)",
+
+    ##########
+    output_group = parser.add_argument_group("Output Settings")
+    output_group.add_argument(
+        "--dark-mode",
+        action="store_true",
+        help="Use colors suitable for a dark terminal background (default: False)",
+        default=False,
     )
-    parser.add_argument(
-        "--edit-format",
-        metavar="EDIT_FORMAT",
-        default=None,
-        help="Specify what edit format GPT should use (default depends on model)",
+    output_group.add_argument(
+        "--light-mode",
+        action="store_true",
+        help="Use colors suitable for a light terminal background (default: False)",
+        default=False,
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--pretty",
         action="store_true",
         default=True,
         help="Enable pretty, colorized output (default: True)",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--no-pretty",
         action="store_false",
         dest="pretty",
         help="Disable pretty, colorized output",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--no-stream",
         action="store_false",
         dest="stream",
         default=True,
         help="Disable streaming responses",
     )
-    parser.add_argument(
-        "--no-git",
-        action="store_false",
-        dest="git",
-        default=True,
-        help="Do not look for a git repo",
-    )
-    parser.add_argument(
+    output_group.add_argument(
         "--user-input-color",
-        default="green",
-        help="Set the color for user input (default: green)",
+        default="#00cc00",
+        help="Set the color for user input (default: #00cc00)",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--tool-output-color",
         default=None,
         help="Set the color for tool output (default: None)",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--tool-error-color",
-        default="red",
+        default="#FF2222",
         help="Set the color for tool error messages (default: red)",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--assistant-output-color",
-        default="blue",
-        help="Set the color for assistant output (default: blue)",
+        default="#0088ff",
+        help="Set the color for assistant output (default: #0088ff)",
     )
-    parser.add_argument(
+    output_group.add_argument(
         "--code-theme",
         default="default",
         help=(
             "Set the markdown code theme (default: default, other options include monokai,"
             " solarized-dark, solarized-light)"
         ),
     )
-    parser.add_argument(
-        "--apply",
-        metavar="FILE",
-        help="Apply the changes from the given file instead of running the chat (debug)",
+    output_group.add_argument(
+        "--show-diffs",
+        action="store_true",
+        help="Show diffs when committing changes (default: False)",
+        default=False,
     )
-    parser.add_argument(
+
+    ##########
+    git_group = parser.add_argument_group("Git Settings")
+    git_group.add_argument(
+        "--no-git",
+        action="store_false",
+        dest="git",
+        default=True,
+        help="Do not look for a git repo",
+    )
+    git_group.add_argument(
         "--auto-commits",
         action="store_true",
         dest="auto_commits",
         default=True,
         help="Enable auto commit of GPT changes (default: True)",
     )
-
-    parser.add_argument(
+    git_group.add_argument(
         "--no-auto-commits",
         action="store_false",
         dest="auto_commits",
         help="Disable auto commit of GPT changes (implies --no-dirty-commits)",
     )
-    parser.add_argument(
+    git_group.add_argument(
         "--dirty-commits",
         action="store_true",
         dest="dirty_commits",
         help="Enable commits when repo is found dirty",
         default=True,
     )
-    parser.add_argument(
+    git_group.add_argument(
         "--no-dirty-commits",
         action="store_false",
         dest="dirty_commits",
         help="Disable commits when repo is found dirty",
     )
-    parser.add_argument(
-        "--encoding",
-        default="utf-8",
-        help="Specify the encoding to use when reading files (default: utf-8)",
-    )
-    parser.add_argument(
-        "--openai-api-key",
-        metavar="OPENAI_API_KEY",
-        help="Specify the OpenAI API key",
-        env_var="OPENAI_API_KEY",
-    )
-    parser.add_argument(
-        "--openai-api-base",
-        metavar="OPENAI_API_BASE",
-        default="https://api.openai.com/v1",
-        help="Specify the OpenAI API base endpoint (default: https://api.openai.com/v1)",
-    )
-    parser.add_argument(
+    git_group.add_argument(
         "--dry-run",
         action="store_true",
-        help="Perform a dry run without applying changes (default: False)",
+        help="Perform a dry run without modifying files (default: False)",
         default=False,
     )
-    parser.add_argument(
-        "--show-diffs",
-        action="store_true",
-        help="Show diffs when committing changes (default: False)",
-        default=False,
+
+    ##########
+    other_group = parser.add_argument_group("Other Settings")
+    other_group.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+        help="Show the version number and exit",
     )
-    parser.add_argument(
-        "--map-tokens",
-        type=int,
-        default=1024,
-        help="Max number of tokens to use for repo map, use 0 to disable (default: 1024)",
+    other_group.add_argument(
+        "--apply",
+        metavar="FILE",
+        help="Apply the changes from the given file instead of running the chat (debug)",
     )
-    parser.add_argument(
+    other_group.add_argument(
         "--yes",
         action="store_true",
         help="Always say yes to every confirmation",
         default=None,
     )
-    parser.add_argument(
+    other_group.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Enable verbose output",
         default=False,
     )
-    parser.add_argument(
+    other_group.add_argument(
         "--message",
         "--msg",
         "-m",
         metavar="COMMAND",
         help="Specify a single message to send GPT, process reply then exit (disables chat mode)",
     )
+    other_group.add_argument(
+        "-c",
+        "--config",
+        is_config_file=True,
+        metavar="CONFIG_FILE",
+        help=(
+            "Specify the config file (default: search for .aider.conf.yml in git root, cwd"
+            " or home directory)"
+        ),
+    )
+
     args = parser.parse_args(args)
 
+    if args.dark_mode:
+        args.user_input_color = "#32FF32"
+        args.tool_error_color = "#FF3333"
+        args.assistant_output_color = "#00FFFF"
+        args.code_theme = "monokai"
+
+    if args.light_mode:
+        args.user_input_color = "green"
+        args.tool_error_color = "red"
+        args.assistant_output_color = "blue"
+        args.code_theme = "default"
+
     io = InputOutput(
         args.pretty,
         args.yes,
         args.input_history_file,
         args.chat_history_file,
         input=input,
         output=output,
         user_input_color=args.user_input_color,
         tool_output_color=args.tool_output_color,
         tool_error_color=args.tool_error_color,
         dry_run=args.dry_run,
     )
 
+    io.tool_output(f"Aider v{__version__}")
+
     if not git_root and args.git:
         if io.confirm_ask("No git repo found, create one to track GPT's changes (recommended)?"):
             repo = git.Repo.init(os.getcwd())
+            global_git_config = git.GitConfigParser(
+                [str(Path.home() / ".gitconfig")], read_only=True
+            )
             with repo.config_writer() as git_config:
-                if not git_config.has_option("user", "name"):
+                if not global_git_config.has_option("user", "name"):
                     git_config.set_value("user", "name", "Your Name")
                     io.tool_error('Update git name with: git config --global user.name "Your Name"')
-                if not git_config.has_option("user", "email"):
+                if not global_git_config.has_option("user", "email"):
                     git_config.set_value("user", "email", "you@example.com")
                     io.tool_error(
                         'Update git email with: git config --global user.email "you@example.com"'
                     )
             io.tool_output("Git repository created in the current working directory.")
 
     if args.verbose:
@@ -323,15 +361,15 @@
     if args.apply:
         content = io.read_text(args.apply)
         if content is None:
             return
         coder.apply_updates(content)
         return
 
-    io.tool_output("Use /help to see in-chat commands.")
+    io.tool_output("Use /help to see in-chat commands, run with --help to see cmd line args")
     if args.message:
         io.tool_output()
         coder.run(with_message=args.message)
     else:
         coder.run()
```

### Comparing `aider-chat-0.8.2/aider/models.py` & `aider-chat-0.8.3/aider/models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/prompts.py` & `aider-chat-0.8.3/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider/repomap.py` & `aider-chat-0.8.3/aider/repomap.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,18 @@
 
     def split_path(self, path):
         path = os.path.relpath(path, self.root)
         return [path + ":"]
 
     def run_ctags(self, filename):
         # Check if the file is in the cache and if the modification time has not changed
-        file_mtime = os.path.getmtime(filename)
+        file_mtime = self.get_mtime(filename)
+        if file_mtime is None:
+            return []
+
         cache_key = filename
         if cache_key in self.TAGS_CACHE and self.TAGS_CACHE[cache_key]["mtime"] == file_mtime:
             return self.TAGS_CACHE[cache_key]["data"]
 
         cmd = self.ctags_cmd + [
             f"--input-encoding={self.io.encoding}",
             filename,
@@ -235,16 +238,25 @@
 
     def load_ident_cache(self):
         self.IDENT_CACHE = Cache(self.IDENT_CACHE_DIR)
 
     def save_ident_cache(self):
         pass
 
+    def get_mtime(self, fname):
+        try:
+            return os.path.getmtime(fname)
+        except FileNotFoundError:
+            self.io.tool_error(f"File not found error: {fname}")
+
     def get_name_identifiers(self, fname, uniq=True):
-        file_mtime = os.path.getmtime(fname)
+        file_mtime = self.get_mtime(fname)
+        if file_mtime is None:
+            return set()
+
         cache_key = fname
         if cache_key in self.IDENT_CACHE and self.IDENT_CACHE[cache_key]["mtime"] == file_mtime:
             idents = self.IDENT_CACHE[cache_key]["data"]
         else:
             idents = self.get_name_identifiers_uncached(fname)
             self.IDENT_CACHE[cache_key] = {"mtime": file_mtime, "data": idents}
             self.save_ident_cache()
```

### Comparing `aider-chat-0.8.2/aider/utils.py` & `aider-chat-0.8.3/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.8.3/aider_chat.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.2
+Version: 0.8.3
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
+Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 
-- [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
+See the
+[installation instructions](https://aider.chat/docs/install.html)
+for more details, but you can
+get started quickly like this:
+
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider myapp.py
+$ aider app.py
 
 Using git repo: .git
-Added myapp.py to the chat.
+Added app.py to the chat.
 
-myapp.py> change the fibonacci function from recursion to iteration
+app.py> make a flask app that replies "hello world" on /hello
 ```
 
 ## Example chat transcripts
 
-Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4. 
+Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
 
 * [**Javascript Game Modification**](https://aider.chat/examples/2048-game.html): Dive into an existing open-source repo, and get GPT's help to understand it and make modifications.
 
 * [**Complex Multi-file Change with Debugging**](https://aider.chat/examples/complex-change.html): GPT makes a complex code change that is coordinated across multiple source files, and resolves bugs by reviewing error output and doc snippets.
 
@@ -52,29 +56,14 @@
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
-## Installation
-
-1. Install the package with pip:
-  * PyPI: `python -m pip install aider-chat`
-  * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
-  * Local clone: `python -m pip install -e .` 
-
-2. Set up your OpenAI API key:
-  * As an environment variable:
-    * `export OPENAI_API_KEY=sk-...` on Linux or Mac
-    * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
-
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
-
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
@@ -113,69 +102,45 @@
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
 
 ## Tips
 
 * Think about which files need to be edited to make your change and add them to the chat.
-Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are able to structure code edits as simple "diffs"
-and use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact "diff" format.
-So aider has
-to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
-This rapidly uses up tokens and can hit the limits of the context window.
-
-For more detailed information and a quantitative comparison, here are
-[code editing benchmark results for GPT-3.5 and GPT-4](https://aider.chat/docs/benchmarks.html).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
-
-In practice, this means you can use aider to edit a set of source files
-that total up to the sizes below.
-You can (and should) add just the specific set of files to the chat
-that are relevant to the change you are requesting.
-This minimizes your use of the context window, as well as costs.
-
-| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
-| ----------------- | -- | --     | -----| -- | -- |
-| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
-| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
-| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
-| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
 
 ## Kind words from users
 
 * "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
+
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models.
+You can choose a model with the `--model` command line argument.
+
+You should probably use GPT-4 if you can. For more details see the
+[FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
+
+For a discussion of using other non-OpenAI models, see the
+[FAQ about other LLMs](https://aider.chat/docs/faq.html#can-i-use-aider-with-other-llms-local-llms-etc).
+
+## Installation
+
+See the [installation instructions](https://aider.chat/docs/install.html).
+
+## FAQ
 
+For more information, see the [FAQ](https://aider.chat/docs/faq.html).
```

### Comparing `aider-chat-0.8.2/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.8.3/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/aider_chat.egg-info/requires.txt` & `aider-chat-0.8.3/aider_chat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/benchmark/benchmark.py` & `aider-chat-0.8.3/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/benchmark/rungrid.py` & `aider-chat-0.8.3/benchmark/rungrid.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/benchmark/test_benchmark.py` & `aider-chat-0.8.3/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/requirements.txt` & `aider-chat-0.8.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/setup.py` & `aider-chat-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 from aider import __version__
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     long_description = re.sub(r"\n!\[.*\]\(.*\)", "", long_description)
-    long_description = re.sub(r"\n- \[.*\]\(#.*\)", "", long_description)
+    long_description = re.sub(r"\n- \[.*\]\(.*\)", "", long_description)
 
 setup(
     name="aider-chat",
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
```

### Comparing `aider-chat-0.8.2/tests/test_coder.py` & `aider-chat-0.8.3/tests/test_coder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import os
 import tempfile
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
+import git
 import openai
 import requests
 
 from aider import models
 from aider.coders import Coder
 from aider.dump import dump  # noqa: F401
 from aider.io import InputOutput
@@ -25,17 +27,17 @@
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Mock the git repo
-        mock_repo = MagicMock()
-        mock_repo.git.ls_files.return_value = "file1.txt\nfile2.py"
-        coder.repo = mock_repo
+        mock = MagicMock()
+        mock.return_value = set(["file1.txt", "file2.py"])
+        coder.get_tracked_files = mock
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt and file2.py")
 
         # Check if coder.abs_fnames contains both files
         expected_files = set(
             map(
@@ -71,18 +73,17 @@
     def test_check_for_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
-        # Mock the git repo
-        mock_repo = MagicMock()
-        mock_repo.git.ls_files.return_value = "file1.txt\nfile2.py"
-        coder.repo = mock_repo
+        mock = MagicMock()
+        mock.return_value = set(["file1.txt", "file2.py"])
+        coder.get_tracked_files = mock
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt and file2.py")
 
         # Check if coder.abs_fnames contains both files
         expected_files = set(
             map(
@@ -98,18 +99,17 @@
     def test_check_for_ambiguous_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
-        # Mock the git repo
-        mock_repo = MagicMock()
-        mock_repo.git.ls_files.return_value = "file1.txt\nother/file1.txt"
-        coder.repo = mock_repo
+        mock = MagicMock()
+        mock.return_value = set(["file1.txt", "other/file1.txt"])
+        coder.get_tracked_files = mock
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt!")
 
         self.assertEqual(coder.abs_fnames, set())
 
     def test_get_commit_message(self):
@@ -339,9 +339,71 @@
             f.write(some_content_which_will_error_if_read_with_encoding_utf8)
 
         coder.run(with_message="hi")
 
         # both files should still be here
         self.assertEqual(len(coder.abs_fnames), 2)
 
+    @patch("aider.coders.base_coder.openai.ChatCompletion.create")
+    def test_run_with_invalid_request_error(self, mock_chat_completion_create):
+        # Mock the IO object
+        mock_io = MagicMock()
+
+        # Initialize the Coder object with the mocked IO and mocked repo
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+
+        # Set up the mock to raise InvalidRequestError
+        mock_chat_completion_create.side_effect = openai.error.InvalidRequestError(
+            "Invalid request", "param"
+        )
+
+        # Call the run method and assert that InvalidRequestError is raised
+        with self.assertRaises(openai.error.InvalidRequestError):
+            coder.run(with_message="hi")
+
+    def test_get_tracked_files(self):
+        # Create a temporary directory
+        tempdir = Path(tempfile.mkdtemp())
+
+        # Initialize a git repository in the temporary directory and set user name and email
+        repo = git.Repo.init(tempdir)
+        repo.config_writer().set_value("user", "name", "Test User").release()
+        repo.config_writer().set_value("user", "email", "testuser@example.com").release()
+
+        # Create three empty files and add them to the git repository
+        filenames = ["README.md", "subdir/fänny.md", "systemüber/blick.md", 'file"with"quotes.txt']
+        created_files = []
+        for filename in filenames:
+            file_path = tempdir / filename
+            try:
+                file_path.parent.mkdir(parents=True, exist_ok=True)
+                file_path.touch()
+                repo.git.add(str(file_path))
+                created_files.append(Path(filename))
+            except OSError:
+                # windows won't allow files with quotes, that's ok
+                self.assertIn('"', filename)
+                self.assertEqual(os.name, "nt")
+
+        self.assertTrue(len(created_files) >= 3)
+
+        repo.git.commit("-m", "added")
+
+        # Create a Coder object on the temporary directory
+        coder = Coder.create(
+            models.GPT4,
+            None,
+            io=InputOutput(),
+            openai_api_key="fake_key",
+            fnames=[str(tempdir / filenames[0])],
+        )
+
+        tracked_files = coder.get_tracked_files()
+
+        # On windows, paths will come back \like\this, so normalize them back to Paths
+        tracked_files = [Path(fn) for fn in tracked_files]
+
+        # Assert that coder.get_tracked_files() returns the three filenames
+        self.assertEqual(set(tracked_files), set(created_files))
+
     if __name__ == "__main__":
         unittest.main()
```

### Comparing `aider-chat-0.8.2/tests/test_editblock.py` & `aider-chat-0.8.3/tests/test_editblock.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/tests/test_io.py` & `aider-chat-0.8.3/tests/test_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,13 +12,13 @@
             self.assertFalse(io.pretty)
 
     def test_autocompleter_with_non_existent_file(self):
         root = ""
         rel_fnames = ["non_existent_file.txt"]
         addable_rel_fnames = []
         commands = None
-        autocompleter = AutoCompleter(root, rel_fnames, addable_rel_fnames, commands)
+        autocompleter = AutoCompleter(root, rel_fnames, addable_rel_fnames, commands, "utf-8")
         self.assertEqual(autocompleter.words, set(rel_fnames))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aider-chat-0.8.2/tests/test_main.py` & `aider-chat-0.8.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/tests/test_models.py` & `aider-chat-0.8.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/tests/test_repomap.py` & `aider-chat-0.8.3/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.2/tests/test_wholefile.py` & `aider-chat-0.8.3/tests/test_wholefile.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aider import models
 from aider.coders import Coder
 from aider.coders.wholefile_coder import WholeFileCoder
+from aider.dump import dump  # noqa: F401
 from aider.io import InputOutput
 
 
 class TestWholeFileCoder(unittest.TestCase):
     def setUp(self):
         self.original_cwd = os.getcwd()
         self.tempdir = tempfile.mkdtemp()
@@ -72,14 +73,32 @@
         self.assertIn("sample.txt", edited_files)
 
         # Check if the content of the sample file was updated
         with open(sample_file, "r") as f:
             updated_content = f.read()
         self.assertEqual(updated_content, "Updated content\n")
 
+    def test_update_files_live_diff(self):
+        # Create a sample file in the temporary directory
+        sample_file = "sample.txt"
+        with open(sample_file, "w") as f:
+            f.write("\n".join(map(str, range(0, 100))))
+
+        # Initialize WholeFileCoder with the temporary directory
+        io = InputOutput(yes=True)
+        coder = WholeFileCoder(main_model=models.GPT35, io=io, fnames=[sample_file])
+
+        # Set the partial response content with the updated content
+        coder.partial_response_content = f"{sample_file}\n```\n0\n\1\n2\n"
+
+        lines = coder.update_files(mode="diff").splitlines()
+
+        # the live diff should be concise, since we haven't changed anything yet
+        self.assertLess(len(lines), 20)
+
     def test_update_files_with_existing_fence(self):
         # Create a sample file in the temporary directory
         sample_file = "sample.txt"
         original_content = """
 Here is some quoted text:
 ```
 Quote!
@@ -227,14 +246,46 @@
         # Check if the sample file was updated
         self.assertIn(str(fname_a), edited_files)
         self.assertIn(str(fname_b), edited_files)
 
         self.assertEqual(fname_a.read_text(), "after a\n")
         self.assertEqual(fname_b.read_text(), "after b\n")
 
+    def test_update_named_file_but_extra_unnamed_code_block(self):
+        sample_file = "hello.py"
+        new_content = "new\ncontent\ngoes\nhere\n"
+
+        with open(sample_file, "w") as f:
+            f.write("Original content\n")
+
+        # Initialize WholeFileCoder with the temporary directory
+        io = InputOutput(yes=True)
+        coder = WholeFileCoder(main_model=models.GPT35, io=io, fnames=[sample_file])
+
+        # Set the partial response content with the updated content
+        coder.partial_response_content = (
+            f"Here's the modified `{sample_file}` file that implements the `accumulate`"
+            f" function as per the given instructions:\n\n```\n{new_content}```\n\nThis"
+            " implementation uses a list comprehension to apply the `operation` function to"
+            " each element of the `collection` and returns the resulting list.\n"
+            "Run it like this:\n\n"
+            "```\npython {sample_file}\n```\n\n"
+        )
+
+        # Call update_files method
+        edited_files = coder.update_files()
+
+        # Check if the sample file was updated
+        self.assertIn(sample_file, edited_files)
+
+        # Check if the content of the sample file was updated
+        with open(sample_file, "r") as f:
+            updated_content = f.read()
+        self.assertEqual(updated_content, new_content)
+
     def test_full_edit(self):
         # Create a few temporary files
         _, file1 = tempfile.mkstemp()
 
         with open(file1, "w", encoding="utf-8") as f:
             f.write("one\ntwo\nthree\n")
```

