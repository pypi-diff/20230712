# Comparing `tmp/aicodebot-0.9.2.tar.gz` & `tmp/aicodebot-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.9.2.tar", last modified: Wed Jul 12 01:45:37 2023, max compression
+gzip compressed data, was "aicodebot-0.9.3.tar", last modified: Wed Jul 12 03:48:30 2023, max compression
```

## Comparing `aicodebot-0.9.2.tar` & `aicodebot-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 01:45:13.000000 aicodebot-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 01:45:37.304956 aicodebot-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 01:45:13.000000 aicodebot-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17535 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-12 01:45:13.000000 aicodebot-0.9.2/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:37.304956 aicodebot-0.9.2/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 01:45:37.000000 aicodebot-0.9.2/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 01:45:13.000000 aicodebot-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:45:37.304956 aicodebot-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-12 01:45:13.000000 aicodebot-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 03:48:03.000000 aicodebot-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 03:48:30.240017 aicodebot-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 03:48:03.000000 aicodebot-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 03:48:03.000000 aicodebot-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:48:30.240017 aicodebot-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-12 03:48:03.000000 aicodebot-0.9.3/setup.py
```

### Comparing `aicodebot-0.9.2/LICENSE` & `aicodebot-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/PKG-INFO` & `aicodebot-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.2
+Version: 0.9.3
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.9.2/README.md` & `aicodebot-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/aicodebot/cli.py` & `aicodebot-0.9.3/aicodebot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,71 +184,68 @@
 
     def write_config_file(config_data):
         with Path.open(config_file, "w") as f:
             yaml.dump(config_data, f)
             console.print(f"✅ Created config file at {config_file}")
 
     is_terminal = sys.stdout.isatty()
+    openai_api_key = openai_api_key or config_data["openai_api_key"] or os.getenv("OPENAI_API_KEY")
     if not is_terminal:
-        if config_data["openai_api_key"] is None:
+        if openai_api_key is None:
             raise click.ClickException(
                 "🛑 No OpenAI API key found.\n"
                 "Please set the OPENAI_API_KEY environment variable or call configure with --openai-api-key set."
             )
         else:
             # If we are not in a terminal, then we can't ask for input, so just use the defaults and write the file
             write_config_file(config_data)
             return
 
     # ---------------- Collect the OPENAI_API_KEY and validate it ---------------- #
 
     if config_data["openai_api_key"] is None:
         console.print(
-            "An OpenAI API key is required to use AICodeBot. You can get one for free on the OpenAI website.\n"
+            "You need an OpenAI API Key for AICodeBot. You can get one on the OpenAI website.",
+            style=bot_style,
         )
         openai_api_key_url = "https://platform.openai.com/account/api-keys"
-        if click.confirm("Open the OpenAI API keys page for you in a browser?", default=False):
+        if click.confirm("Open the api keys page in a browser?", default=False):
             webbrowser.open(openai_api_key_url)
 
-        config_data["openai_api_key"] = input_prompt("Please enter your OpenAI API key")
+        config_data["openai_api_key"] = click.prompt("Please enter your OpenAI API key").strip()
 
     # Validate the API key
     try:
         openai.api_key = config_data["openai_api_key"]
-        click.echo("Validating the OpenAI API key")
-        engine.Engine.list()
+        with console.status("Validating the OpenAI API key", spinner=DEFAULT_SPINNER):
+            engine.Engine.list()
     except Exception as e:
         raise click.ClickException(f"Failed to validate the API key: {str(e)}") from e
-    click.echo("✅ The API key is valid.")
+    console.print("✅ The API key is valid.")
 
     # ---------------------- Collect the personality choice ---------------------- #
 
     # Pull the choices from the name from each of the PERSONALITIES
-    personality_choices = "\nHow would you like your AI to act? You can choose from the following personalities:\n"
+    console.print(
+        "\nHow would you like your AI to act? You can choose from the following personalities:\n", style=bot_style
+    )
+    personality_choices = ""
     for key, personality in PERSONALITIES.items():
-        personality_choices += f"\t{key} - {personality.description}\n"
+        personality_choices += f"\t[b]{key}[/b] - {personality.description}\n"
     console.print(personality_choices)
 
     config_data["personality"] = click.prompt(
         "Please choose a personality",
         type=click.Choice(PERSONALITIES.keys(), case_sensitive=False),
         default=DEFAULT_PERSONALITY.name,
     )
 
     write_config_file(config_data)
     console.print("✅ Configuration complete, you're ready to run aicodebot!\n")
 
-    # After writing the config file, print the usage for the top-level group
-    ctx = click.get_current_context()
-    while ctx.parent is not None:
-        ctx = ctx.parent
-    console.print(ctx.get_help())
-
-    console.print("\nDon't know where to start? Try running `aicodebot alignment`.")
-
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("command", nargs=-1)
 @click.option("-v", "--verbose", count=True)
 def debug(command, verbose):
     """Run a command and debug the output."""
     setup_config()
@@ -371,19 +368,18 @@
 @click.option("-t", "--response-token-size", type=int, default=DEFAULT_MAX_TOKENS * 2)
 @click.argument("files", nargs=-1)
 def sidekick(request, verbose, response_token_size, files):
     """
     EXPERIMENTAL: Coding help from your AI sidekick\n
     FILES: List of files to be used as context for the session
     """
-
-    console.print("This is an experimental feature. Play with it, but don't count on it.", style=warning_style)
-
     setup_config()
 
+    console.print("This is an experimental feature", style=warning_style)
+
     # Pull in context. Right now it's just the contents of files that we passed in.
     # Soon, we could add vector embeddings of:
     # imported code / modules / libraries
     # Style guides/reference code
     # git history
     context = generate_files_context(files)
 
@@ -437,16 +433,16 @@
 #                               Helper functions                               #
 # ---------------------------------------------------------------------------- #
 
 
 def setup_config():
     existing_config = read_config()
     if not existing_config:
-        console.print("No config file found. Running configure...\n")
-        configure.callback(openai_api_key=None, verbose=0)
+        console.print("Welcome to AI Code Bot! 🤖. Let's set up your config file.\n", style=bot_style)
+        configure.callback(openai_api_key=os.getenv("OPENAI_API_KEY"), verbose=0)
         sys.exit()
     else:
         return existing_config
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `aicodebot-0.9.2/aicodebot/coder.py` & `aicodebot-0.9.3/aicodebot/coder.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/aicodebot/config.py` & `aicodebot-0.9.3/aicodebot/config.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/aicodebot/helpers.py` & `aicodebot-0.9.3/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/aicodebot/prompts.py` & `aicodebot-0.9.3/aicodebot/prompts.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.3/aicodebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.2
+Version: 0.9.3
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.9.2/pyproject.toml` & `aicodebot-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.2/setup.py` & `aicodebot-0.9.3/setup.py`

 * *Files identical despite different names*

