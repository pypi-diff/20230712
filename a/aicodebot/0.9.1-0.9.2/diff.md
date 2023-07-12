# Comparing `tmp/aicodebot-0.9.1.tar.gz` & `tmp/aicodebot-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.9.1.tar", last modified: Mon Jul 10 19:53:00 2023, max compression
+gzip compressed data, was "aicodebot-0.9.2.tar", last modified: Wed Jul 12 01:45:37 2023, max compression
```

## Comparing `aicodebot-0.9.1.tar` & `aicodebot-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-10 19:52:37.000000 aicodebot-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-10 19:53:00.781555 aicodebot-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-10 19:52:37.000000 aicodebot-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-10 19:52:37.000000 aicodebot-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:53:00.781555 aicodebot-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 19:52:37.000000 aicodebot-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 01:45:13.000000 aicodebot-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 01:45:37.304956 aicodebot-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 01:45:13.000000 aicodebot-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17535 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 01:45:13.000000 aicodebot-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:45:37.304956 aicodebot-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-12 01:45:13.000000 aicodebot-0.9.2/setup.py
```

### Comparing `aicodebot-0.9.1/LICENSE` & `aicodebot-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.1/PKG-INFO` & `aicodebot-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.1
+Version: 0.9.2
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -38,25 +38,27 @@
 
 ## Current features - how you can use it today
 
 | Task | Status |
 | --- | --- |
 | Generating quality commit messages | ✅ |
 | Thinking through tasks as a pair programmer | ✅ |
-| Suggestions for simple changes | ✅ |
+| Coding with a small number of files | ✅ |
 | Debugging | ✅ |
 | Doing code reviews | ✅ |
 | Explaining code | ✅ |
 | Writing tests | ✅ |
-| Modifying local files | Not yet, but soon! |
-| Searching the internet for answers | Not yet, but soon! |
-| Reading library documentation | Not yet, but soon! |
-| Writing senior developer level code | Not for a long time |
-| Major refactors | Not for a long time |
-| Build an app for me | Nope |
+| Modifying local files | In Progress |
+| Searching the internet for answers | In Progress |
+| Reading library documentation | In Progress |
+| Coding with a large number of files |  As LLMs improve |
+| Writing senior developer level code | Eventually |
+| Major refactors | Eventually |
+| Build an entire app | Nope |
+| Replace Developers | Nope |
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
```

### Comparing `aicodebot-0.9.1/README.md` & `aicodebot-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 
 ## Current features - how you can use it today
 
 | Task | Status |
 | --- | --- |
 | Generating quality commit messages | ✅ |
 | Thinking through tasks as a pair programmer | ✅ |
-| Suggestions for simple changes | ✅ |
+| Coding with a small number of files | ✅ |
 | Debugging | ✅ |
 | Doing code reviews | ✅ |
 | Explaining code | ✅ |
 | Writing tests | ✅ |
-| Modifying local files | Not yet, but soon! |
-| Searching the internet for answers | Not yet, but soon! |
-| Reading library documentation | Not yet, but soon! |
-| Writing senior developer level code | Not for a long time |
-| Major refactors | Not for a long time |
-| Build an app for me | Nope |
+| Modifying local files | In Progress |
+| Searching the internet for answers | In Progress |
+| Reading library documentation | In Progress |
+| Coding with a large number of files |  As LLMs improve |
+| Writing senior developer level code | Eventually |
+| Major refactors | Eventually |
+| Build an entire app | Nope |
+| Replace Developers | Nope |
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
```

### Comparing `aicodebot-0.9.1/aicodebot/cli.py` & `aicodebot-0.9.2/aicodebot/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 from aicodebot import version as aicodebot_version
-from aicodebot.helpers import (
-    exec_and_get_output,
-    get_config_file,
-    get_llm_model,
-    get_token_length,
-    git_diff_context,
-    logger,
-    read_config,
-)
+from aicodebot.coder import CREATIVE_TEMPERATURE, DEFAULT_MAX_TOKENS, Coder
+from aicodebot.config import get_config_file, read_config
+from aicodebot.helpers import RichLiveCallbackHandler, exec_and_get_output, logger
 from aicodebot.prompts import DEFAULT_PERSONALITY, PERSONALITIES, generate_files_context, get_prompt
-from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
-from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationTokenBufferMemory
 from openai.api_resources import engine
 from pathlib import Path
+from prompt_toolkit import prompt as input_prompt
+from prompt_toolkit.history import FileHistory
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser, yaml
 
 # ----------------------------- Default settings ----------------------------- #
 
-DEFAULT_MAX_TOKENS = 512
-PRECISE_TEMPERATURE = 0.1
-CREATIVE_TEMPERATURE = 0.7
 DEFAULT_SPINNER = "point"
 
 # ----------------------- Setup for rich console output ---------------------- #
 
 console = Console()
 bot_style = Style(color="#30D5C8")
 error_style = Style(color="#FF0000")
@@ -56,32 +47,31 @@
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=350)
 def alignment(response_token_size, verbose):
     """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
-    config = setup_config()
+    setup_config()
 
     # Load the prompt
     prompt = get_prompt("alignment")
     logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
-    model = get_llm_model(get_token_length(prompt.template))
+    model_name = Coder.get_llm_model_name(Coder.get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
-        llm = ChatOpenAI(
-            model=model,
+        llm = Coder.get_llm(
+            model_name,
+            verbose,
+            response_token_size,
             temperature=CREATIVE_TEMPERATURE,
-            openai_api_key=config["openai_api_key"],
-            max_tokens=response_token_size,
-            verbose=verbose,
             streaming=True,
-            callbacks=[RichLiveCallbackHandler(live)],
+            callbacks=[RichLiveCallbackHandler(live, bot_style)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
         chain.run({})
 
@@ -89,15 +79,15 @@
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=250)
 @click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
 @click.option("--skip-pre-commit", is_flag=True, help="Skip running pre-commit (otherwise run it if it is found).")
 def commit(verbose, response_token_size, yes, skip_pre_commit):
     """Generate a commit message based on your changes."""
-    config = setup_config()
+    setup_config()
 
     # Check if pre-commit is installed and .pre-commit-config.yaml exists
     if not skip_pre_commit and Path(".pre-commit-config.yaml").exists():
         console.print("Running pre-commit checks...")
         result = subprocess.run(["pre-commit", "run", "--all-files"])
         if result.returncode != 0:
             console.print("🛑 Pre-commit checks failed. Please fix the issues and try again.")
@@ -115,36 +105,29 @@
         exec_and_get_output(["git", "add", "-A"])
         # Get the list of files to be committed
         files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     else:
         # The list of files to be committed is the same as the list of staged files
         files = staged_files
 
-    diff_context = git_diff_context()
+    diff_context = Coder.git_diff_context()
 
     if not diff_context:
         console.print("No changes to commit. 🤷")
         sys.exit(0)
 
     # Check the size of the diff context and adjust accordingly
-    request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
-    model = get_llm_model(request_token_size)
-    if model is None:
+    request_token_size = Coder.get_token_length(diff_context) + Coder.get_token_length(prompt.template)
+    model_name = Coder.get_llm_model_name(request_token_size)
+    if model_name is None:
         raise click.ClickException(
             f"The diff is too large to generate a commit message ({request_token_size} tokens). 😢"
         )
 
-    # Set up the language model
-    llm = ChatOpenAI(
-        model=model,
-        openai_api_key=config["openai_api_key"],
-        temperature=PRECISE_TEMPERATURE,
-        max_tokens=DEFAULT_MAX_TOKENS,
-        verbose=verbose,
-    )
+    llm = Coder.get_llm(model_name, verbose, 350)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     console.print("The following files will be committed:\n" + files)
     with console.status("Examining the diff and generating the commit message", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
@@ -222,17 +205,15 @@
         console.print(
             "An OpenAI API key is required to use AICodeBot. You can get one for free on the OpenAI website.\n"
         )
         openai_api_key_url = "https://platform.openai.com/account/api-keys"
         if click.confirm("Open the OpenAI API keys page for you in a browser?", default=False):
             webbrowser.open(openai_api_key_url)
 
-        config_data["openai_api_key"] = click.prompt(
-            "Please enter your OpenAI API key", default=config_data["openai_api_key"]
-        )
+        config_data["openai_api_key"] = input_prompt("Please enter your OpenAI API key")
 
     # Validate the API key
     try:
         openai.api_key = config_data["openai_api_key"]
         click.echo("Validating the OpenAI API key")
         engine.Engine.list()
     except Exception as e:
@@ -266,15 +247,15 @@
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("command", nargs=-1)
 @click.option("-v", "--verbose", count=True)
 def debug(command, verbose):
     """Run a command and debug the output."""
-    config = setup_config()
+    setup_config()
 
     # Run the command and capture its output
     command_str = " ".join(command)
     console.print(f"Executing the command:\n{command_str}")
     process = subprocess.run(command_str, shell=True, capture_output=True, text=True)  # noqa: S602
 
     # Print the output of the command
@@ -292,101 +273,94 @@
     console.print(f"The command exited with status {process.returncode}.")
 
     # Load the prompt
     prompt = get_prompt("debug")
     logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
-    request_token_size = get_token_length(error_output) + get_token_length(prompt.template)
-    model = get_llm_model(request_token_size)
-    if model is None:
+    request_token_size = Coder.get_token_length(error_output) + Coder.get_token_length(prompt.template)
+    model_name = Coder.get_llm_model_name(request_token_size)
+    if model_name is None:
         raise click.ClickException(f"The output is too large to debug ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
-        llm = ChatOpenAI(
-            model=model,
-            temperature=PRECISE_TEMPERATURE,
-            openai_api_key=config["openai_api_key"],
-            max_tokens=DEFAULT_MAX_TOKENS,
-            verbose=verbose,
+        llm = Coder.get_llm(
+            model_name,
+            verbose,
             streaming=True,
-            callbacks=[RichLiveCallbackHandler(live)],
+            callbacks=[RichLiveCallbackHandler(live, bot_style)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
         chain.run(error_output)
 
     sys.exit(process.returncode)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
-@click.option("-t", "--response-token-size", type=int, default=350)
+@click.option("-t", "--response-token-size", type=int, default=250)
 def fun_fact(verbose, response_token_size):
     """Get a fun fact about programming and artificial intelligence."""
-    config = setup_config()
+    setup_config()
 
     # Load the prompt
     prompt = get_prompt("fun_fact")
     logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
-    model = get_llm_model(get_token_length(prompt.template))
+    model_name = Coder.get_llm_model_name(Coder.get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
-        llm = ChatOpenAI(
-            model=model,
-            temperature=PRECISE_TEMPERATURE,
-            max_tokens=response_token_size,
-            openai_api_key=config["openai_api_key"],
-            verbose=verbose,
+        llm = Coder.get_llm(
+            model_name,
+            verbose,
+            response_token_size=response_token_size,
+            temperature=CREATIVE_TEMPERATURE,
             streaming=True,
-            callbacks=[RichLiveCallbackHandler(live)],
+            callbacks=[RichLiveCallbackHandler(live, bot_style)],
         )
-
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
         year = random.randint(1942, datetime.datetime.utcnow().year)
         chain.run(f"programming and artificial intelligence in the year {year}")
 
 
 @cli.command
 @click.option("-c", "--commit", help="The commit hash to review (otherwise look at [un]staged changes).")
 @click.option("-v", "--verbose", count=True)
 def review(commit, verbose):
     """Do a code review, with [un]staged changes, or a specified commit."""
-    config = setup_config()
+    setup_config()
 
-    diff_context = git_diff_context(commit)
+    diff_context = Coder.git_diff_context(commit)
     if not diff_context:
         console.print("No changes detected for review. 🤷")
         sys.exit(0)
 
     # Load the prompt
     prompt = get_prompt("review")
     logger.trace(f"Prompt: {prompt}")
 
     # Check the size of the diff context and adjust accordingly
     response_token_size = DEFAULT_MAX_TOKENS * 2
-    request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
-    model = get_llm_model(request_token_size)
-    if model is None:
+    request_token_size = Coder.get_token_length(diff_context) + Coder.get_token_length(prompt.template)
+    model_name = Coder.get_llm_model_name(request_token_size)
+    if model_name is None:
         raise click.ClickException(f"The diff is too large to review ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
-        llm = ChatOpenAI(
-            model=model,
-            temperature=PRECISE_TEMPERATURE,
-            openai_api_key=config["openai_api_key"],
-            max_tokens=response_token_size,
-            verbose=verbose,
+        llm = Coder.get_llm(
+            model_name,
+            verbose,
+            response_token_size=response_token_size,
             streaming=True,
-            callbacks=[RichLiveCallbackHandler(live)],
+            callbacks=[RichLiveCallbackHandler(live, bot_style)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
         chain.run(diff_context)
 
@@ -400,71 +374,62 @@
     """
     EXPERIMENTAL: Coding help from your AI sidekick\n
     FILES: List of files to be used as context for the session
     """
 
     console.print("This is an experimental feature. Play with it, but don't count on it.", style=warning_style)
 
-    config = setup_config()
+    setup_config()
 
     # Pull in context. Right now it's just the contents of files that we passed in.
     # Soon, we could add vector embeddings of:
     # imported code / modules / libraries
     # Style guides/reference code
     # git history
     context = generate_files_context(files)
 
     # Generate the prompt and set up the model
     prompt = get_prompt("sidekick")
-    request_token_size = get_token_length(prompt.template) + get_token_length(context)
-    model = get_llm_model(request_token_size)
-    if model is None:
+    request_token_size = Coder.get_token_length(prompt.template) + Coder.get_token_length(context)
+    model_name = Coder.get_llm_model_name(request_token_size)
+    if model_name is None:
         raise click.ClickException(
             f"The file context you supplied is too large ({request_token_size} tokens). 😢 Try again with less files."
         )
 
-    llm = ChatOpenAI(
-        model=model,
-        openai_api_key=config["openai_api_key"],
-        temperature=PRECISE_TEMPERATURE,
-        max_tokens=response_token_size,
-        verbose=verbose,
-        streaming=True,
-    )
+    llm = Coder.get_llm(model_name, verbose, response_token_size, streaming=True)
 
     # Open the temporary file in the user's editor
     editor = Path(os.getenv("EDITOR", "/usr/bin/vim")).name
 
     # Set up the chain
     memory = ConversationTokenBufferMemory(
         memory_key="chat_history", input_key="task", llm=llm, max_token_limit=DEFAULT_MAX_TOKENS
     )
     chain = LLMChain(llm=llm, prompt=prompt, memory=memory, verbose=verbose)
+    history_file = Path.home() / ".aicodebot_request_history"
 
     while True:  # continuous loop for multiple questions
         if request:
             human_input = request
         else:
-            human_input = click.prompt(
-                f"Enter a question OR (q) quit, OR (e) to edit using {editor}\n>>>",
-                prompt_suffix="",
-            )
+            console.print(f"Enter a request OR (q) quit, OR (e) to edit using {editor}")
+            human_input = input_prompt("➤ ", history=FileHistory(history_file))
             if len(human_input) == 1:
                 if human_input.lower() == "q":
                     break
                 elif human_input.lower() == "e":
                     human_input = click.edit()
             elif human_input.lower()[-2:] == r"\e":
                 # If the text ends with \e then we want to edit it
                 human_input = click.edit(human_input[:-2])
 
         with Live(Markdown(""), auto_refresh=True) as live:
-            callback = RichLiveCallbackHandler(live)
-            callback.buffer = []
-            llm.callbacks = [callback]
+            callback = RichLiveCallbackHandler(live, bot_style)
+            llm.callbacks = [callback]  # a fresh callback handler for each question
             chain.run({"task": human_input, "context": context})
 
         if request:
             # If we were given a request, then we only want to run once
             break
 
 
@@ -479,20 +444,9 @@
         console.print("No config file found. Running configure...\n")
         configure.callback(openai_api_key=None, verbose=0)
         sys.exit()
     else:
         return existing_config
 
 
-class RichLiveCallbackHandler(BaseCallbackHandler):
-    buffer = []
-
-    def __init__(self, live):
-        self.live = live
-
-    def on_llm_new_token(self, token, **kwargs):
-        self.buffer.append(token)
-        self.live.update(Markdown("".join(self.buffer), style=bot_style))
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `aicodebot-0.9.1/aicodebot/helpers.py` & `aicodebot-0.9.2/aicodebot/coder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,158 @@
-from loguru import logger
+from aicodebot.config import read_config
+from aicodebot.helpers import exec_and_get_output, logger
+from langchain.chat_models import ChatOpenAI
 from openai.api_resources import engine
 from pathlib import Path
-import fnmatch, openai, os, subprocess, sys, tiktoken, yaml
+import fnmatch, openai, tiktoken
 
-# ---------------------------------------------------------------------------- #
-#                    Global logging configuration for loguru                   #
-# ---------------------------------------------------------------------------- #
-
-
-logger.remove()
-logger_format = (
-    "<level>{time}</level> {message} | <level>{level}</level> "
-    "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan>"
-)
-logger.add(sys.stderr, catch=True, format=logger_format, level=os.getenv("LOG_LEVEL", "WARNING"))
-logger = logger.opt(colors=True)
-
-# ---------------------------------------------------------------------------- #
-#                                Misc functions                                #
-# ---------------------------------------------------------------------------- #
-
-
-def generate_directory_structure(path, ignore_patterns=None, use_gitignore=True, indent=0):
-    """Generate a text representation of the directory structure of a path."""
-    ignore_patterns = ignore_patterns.copy() if ignore_patterns else []
-
-    base_path = Path(path)
-
-    if use_gitignore:
-        # Note: .gitignore files can exist in sub directories as well, such as * in __pycache__ directories
-        gitignore_file = base_path / ".gitignore"
-        if gitignore_file.exists():
-            with gitignore_file.open() as f:
-                ignore_patterns.extend(line.strip() for line in f if line.strip() and not line.startswith("#"))
-
-    structure = ""
-    if base_path.is_dir():
-        if not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
-            structure += "  " * indent + f"- [Directory] {base_path.name}\n"
-            for item in base_path.iterdir():
-                structure += generate_directory_structure(item, ignore_patterns, use_gitignore, indent + 1)
-    elif not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
-        structure += "  " * indent + f"- [File] {base_path.name}\n"
-
-    return structure
-
-
-def get_llm_model(token_size=0):
-    model_options = {
-        "gpt-4": 8192,
-        "gpt-4-32k": 32768,
-        "gpt-3.5-turbo": 4096,
-        "gpt-3.5-turbo-16k": 16384,
-    }
-
-    config = read_config()
-    openai.api_key = config["openai_api_key"]
-    engines = engine.Engine.list()
-    logger.trace(f"Engines: {engines}")
-
-    # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
-    token_size = int(token_size * 1.1)
-
-    # Try to use GPT-4 if it is supported and the token size is small enough
-    if "gpt-4" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4"]:
-        logger.info(f"Using GPT-4 for token size {token_size}")
-        return "gpt-4"
-    elif "gpt-4-32k" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4-32k"]:
-        logger.info(f"Using GPT-4-32k for token size {token_size}")
-        return "gpt-4-32k"
-    elif token_size <= model_options["gpt-3.5-turbo"]:
-        logger.info(f"Using GPT-3.5-turbo for token size {token_size}")
-        return "gpt-3.5-turbo"
-    elif token_size <= model_options["gpt-3.5-turbo-16k"]:
-        logger.info(f"Using GPT-3.5-turbo-16k for token size {token_size}")
-        return "gpt-3.5-turbo-16k"
-    else:
-        logger.critical(
-            f"🛑 The context is too large ({token_size})"
-            "for the any of the models supported by your Open AI API key. 😞"
+DEFAULT_MAX_TOKENS = 512
+PRECISE_TEMPERATURE = 0.1
+CREATIVE_TEMPERATURE = 0.7
+
+
+class Coder:
+    """
+    The Coder class encapsulates the functionality of interacting with LLMs,
+    git, and the local file system.
+
+    """
+
+    @classmethod
+    def generate_directory_structure(cls, path, ignore_patterns=None, use_gitignore=True, indent=0):
+        """Generate a text representation of the directory structure of a path."""
+        ignore_patterns = ignore_patterns.copy() if ignore_patterns else []
+
+        base_path = Path(path)
+
+        if use_gitignore:
+            # Note: .gitignore files can exist in sub directories as well, such as * in __pycache__ directories
+            gitignore_file = base_path / ".gitignore"
+            if gitignore_file.exists():
+                with gitignore_file.open() as f:
+                    ignore_patterns.extend(line.strip() for line in f if line.strip() and not line.startswith("#"))
+
+        structure = ""
+        if base_path.is_dir():
+            if not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
+                structure += "  " * indent + f"- [Directory] {base_path.name}\n"
+                for item in base_path.iterdir():
+                    structure += cls.generate_directory_structure(item, ignore_patterns, use_gitignore, indent + 1)
+        elif not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
+            structure += "  " * indent + f"- [File] {base_path.name}\n"
+
+        return structure
+
+    @staticmethod
+    def get_llm(
+        model_name,
+        verbose=False,
+        response_token_size=DEFAULT_MAX_TOKENS,
+        temperature=PRECISE_TEMPERATURE,
+        live=None,
+        streaming=False,
+        callbacks=None,
+    ):
+        config = read_config()
+
+        return ChatOpenAI(
+            openai_api_key=config["openai_api_key"],
+            model=model_name,
+            max_tokens=response_token_size,
+            verbose=verbose,
+            temperature=temperature,
+            streaming=streaming,
+            callbacks=callbacks,
         )
-        return None
 
-
-def get_token_length(text, model="gpt-3.5-turbo"):
-    """Get the number of tokens in a string using the tiktoken library."""
-    encoding = tiktoken.encoding_for_model(model)
-    tokens = encoding.encode(text)
-    token_length = len(tokens)
-    logger.debug(f"Token length for text {text[0:10]}...: {token_length}")
-    return token_length
-
-
-def git_diff_context(commit=None):
-    """Get a text representation of the git diff for the current commit or staged files, including new files"""
-    base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
-
-    if commit:
-        # If a commit is provided, just get the diff for that commit
-        logger.debug(f"Getting diff for commit {commit}")
-        return exec_and_get_output(["git", "show", commit])
-    else:
-        # Otherwise, get the diff for the staged files, or if there are none, the diff for the unstaged files
-        staged_files = exec_and_get_output(["git", "diff", "--cached", "--name-only"]).splitlines()
-        if staged_files:
-            logger.debug(f"Getting diff for staged files: {staged_files}")
-            diff_type = "--cached"
+    @staticmethod
+    def get_llm_model_name(token_size=0):
+        model_options = {
+            "gpt-4": 8192,
+            "gpt-4-32k": 32768,
+            "gpt-3.5-turbo": 4096,
+            "gpt-3.5-turbo-16k": 16384,
+        }
+
+        config = read_config()
+        openai.api_key = config["openai_api_key"]
+        engines = engine.Engine.list()
+
+        # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
+        token_size = int(token_size * 1.1)
+
+        # Try to use GPT-4 if it is supported and the token size is small enough
+        if "gpt-4" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4"]:
+            logger.info(f"Using GPT-4 for token size {token_size}")
+            return "gpt-4"
+        elif "gpt-4-32k" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4-32k"]:
+            logger.info(f"Using GPT-4-32k for token size {token_size}")
+            return "gpt-4-32k"
+        elif token_size <= model_options["gpt-3.5-turbo"]:
+            logger.info(f"Using GPT-3.5-turbo for token size {token_size}")
+            return "gpt-3.5-turbo"
+        elif token_size <= model_options["gpt-3.5-turbo-16k"]:
+            logger.info(f"Using GPT-3.5-turbo-16k for token size {token_size}")
+            return "gpt-3.5-turbo-16k"
+        else:
+            logger.critical(
+                f"🛑 The context is too large ({token_size})"
+                "for the any of the models supported by your Open AI API key. 😞"
+            )
+            return None
+
+    @staticmethod
+    def get_token_length(text, model="gpt-3.5-turbo"):
+        """Get the number of tokens in a string using the tiktoken library."""
+        encoding = tiktoken.encoding_for_model(model)
+        tokens = encoding.encode(text)
+        token_length = len(tokens)
+        logger.debug(f"Token length for text {text[0:10]}...: {token_length}")
+        return token_length
+
+    @staticmethod
+    def git_diff_context(commit=None):
+        """Get a text representation of the git diff for the current commit or staged files, including new files"""
+        base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
+
+        if commit:
+            # If a commit is provided, just get the diff for that commit
+            logger.debug(f"Getting diff for commit {commit}")
+            return exec_and_get_output(["git", "show", commit])
         else:
-            logger.debug(f"Getting diff for unstaged files: {staged_files}")
-            diff_type = "HEAD"
+            # Otherwise, get the diff for the staged files, or if there are none, the diff for the unstaged files
+            staged_files = exec_and_get_output(["git", "diff", "--cached", "--name-only"]).splitlines()
+            if staged_files:
+                logger.debug(f"Getting diff for staged files: {staged_files}")
+                diff_type = "--cached"
+            else:
+                logger.debug(f"Getting diff for unstaged files: {staged_files}")
+                diff_type = "HEAD"
 
-        file_status = exec_and_get_output(["git", "diff", diff_type, "--name-status"]).splitlines()
+            file_status = exec_and_get_output(["git", "diff", diff_type, "--name-status"]).splitlines()
 
-        diffs = []
-        for status in file_status:
-            status_parts = status.split("\t")
-            status_code = status_parts[0][0]  # Get the first character of the status code
-            if status_code == "A":
-                # If the file is new, include the entire file content
-                file_name = status_parts[1]
-                contents = Path(file_name).read_text()
-                diffs.append(f"## New file added: {file_name}")
-                diffs.append(contents)
-            elif status_code == "R":
-                # If the file is renamed, get the diff and note the old and new names
-                old_file_name, new_file_name = status_parts[1], status_parts[2]
-                diffs.append(f"## File renamed: {old_file_name} -> {new_file_name}")
-                diffs.append(exec_and_get_output(base_git_diff + [diff_type, "--", new_file_name]))
-            elif status_code == "D":
-                # If the file is deleted, note the deletion
-                file_name = status_parts[1]
-                diffs.append(f"## File deleted: {file_name}")
-            else:
-                # If the file is not new, renamed, or deleted, get the diff
-                file_name = status_parts[1]
-                diffs.append(f"## File changed: {file_name}")
-                diffs.append(exec_and_get_output(base_git_diff + [diff_type, "--", file_name]))
-
-        return "\n".join(diffs)
-
-
-def exec_and_get_output(command):
-    """Execute a command and return its output as a string."""
-    logger.debug(f"Executing command: {' '.join(command)}")
-    result = subprocess.run(command, capture_output=True, text=True)  # noqa: S603
-    if result.returncode != 0:
-        raise Exception(f"Command '{' '.join(command)}' failed with error:\n{result.stderr}")  # noqa: TRY002
-    return result.stdout
-
-
-def get_config_file():
-    if "AICODEBOT_CONFIG_FILE" in os.environ:
-        config_file = Path(os.getenv("AICODEBOT_CONFIG_FILE"))
-    else:
-        config_file = Path(Path.home() / ".aicodebot.yaml")
-    logger.debug(f"Using config file {config_file}")
-    return config_file
-
-
-def read_config():
-    """Read the config file and return its contents as a dictionary."""
-    config_file = get_config_file()
-    if config_file.exists():
-        logger.debug(f"Config file {config_file} exists")
-        with Path(config_file).open("r") as f:
-            return yaml.safe_load(f)
-    else:
-        logger.debug(f"Config file {config_file} does not exist")
-        return None
+            diffs = []
+            for status in file_status:
+                status_parts = status.split("\t")
+                status_code = status_parts[0][0]  # Get the first character of the status code
+                if status_code == "A":
+                    # If the file is new, include the entire file content
+                    file_name = status_parts[1]
+                    contents = Path(file_name).read_text()
+                    diffs.append(f"## New file added: {file_name}")
+                    diffs.append(contents)
+                elif status_code == "R":
+                    # If the file is renamed, get the diff and note the old and new names
+                    old_file_name, new_file_name = status_parts[1], status_parts[2]
+                    diffs.append(f"## File renamed: {old_file_name} -> {new_file_name}")
+                    diffs.append(exec_and_get_output(base_git_diff + [diff_type, "--", new_file_name]))
+                elif status_code == "D":
+                    # If the file is deleted, note the deletion
+                    file_name = status_parts[1]
+                    diffs.append(f"## File deleted: {file_name}")
+                else:
+                    # If the file is not new, renamed, or deleted, get the diff
+                    file_name = status_parts[1]
+                    diffs.append(f"## File changed: {file_name}")
+                    diffs.append(exec_and_get_output(base_git_diff + [diff_type, "--", file_name]))
+
+            return "\n".join(diffs)
```

### Comparing `aicodebot-0.9.1/aicodebot/prompts.py` & `aicodebot-0.9.2/aicodebot/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from aicodebot.helpers import generate_directory_structure, get_token_length, logger, read_config
+from aicodebot.coder import Coder
+from aicodebot.config import read_config
+from aicodebot.helpers import logger
 from langchain import PromptTemplate
 from pathlib import Path
 from types import SimpleNamespace
 import os
 
 # ---------------------------------------------------------------------------- #
 #                              Personality helpers                             #
@@ -128,23 +130,23 @@
 def generate_files_context(files):
     """Generate the files context for the sidekick prompt.
 
     This includes a directory structure and the contents of $files
 
     """
     files_context = "\nHere is the directory structure we are working with in this session:\n"
-    files_context += generate_directory_structure(".", ignore_patterns=[".git"], use_gitignore=True)
+    files_context += Coder.generate_directory_structure(".", ignore_patterns=[".git"], use_gitignore=True)
 
     if not files:
         return files_context
 
     files_context += "Here are the relevant files we are working with in this session:\n"
     for file_name in files:
         contents = Path(file_name).read_text()
-        token_length = get_token_length(contents)
+        token_length = Coder.get_token_length(contents)
         if token_length > 2_000:
             logger.warning(f"File {file_name} is large, using {token_length} tokens")
         else:
             logger.debug(f"File {file_name} is {token_length} tokens")
         files_context += f"--- START OF FILE: {file_name} ---\n"
         files_context += contents
         files_context += f"\n--- END OF FILE: {file_name} ---\n\n"
```

### Comparing `aicodebot-0.9.1/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.2/aicodebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.1
+Version: 0.9.2
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -38,25 +38,27 @@
 
 ## Current features - how you can use it today
 
 | Task | Status |
 | --- | --- |
 | Generating quality commit messages | ✅ |
 | Thinking through tasks as a pair programmer | ✅ |
-| Suggestions for simple changes | ✅ |
+| Coding with a small number of files | ✅ |
 | Debugging | ✅ |
 | Doing code reviews | ✅ |
 | Explaining code | ✅ |
 | Writing tests | ✅ |
-| Modifying local files | Not yet, but soon! |
-| Searching the internet for answers | Not yet, but soon! |
-| Reading library documentation | Not yet, but soon! |
-| Writing senior developer level code | Not for a long time |
-| Major refactors | Not for a long time |
-| Build an app for me | Nope |
+| Modifying local files | In Progress |
+| Searching the internet for answers | In Progress |
+| Reading library documentation | In Progress |
+| Coding with a large number of files |  As LLMs improve |
+| Writing senior developer level code | Eventually |
+| Major refactors | Eventually |
+| Build an entire app | Nope |
+| Replace Developers | Nope |
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
```

### Comparing `aicodebot-0.9.1/pyproject.toml` & `aicodebot-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.1/setup.py` & `aicodebot-0.9.2/setup.py`

 * *Files identical despite different names*

