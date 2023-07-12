# Comparing `tmp/aicodebot-0.9.3.tar.gz` & `tmp/aicodebot-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.9.3.tar", last modified: Wed Jul 12 03:48:30 2023, max compression
+gzip compressed data, was "aicodebot-0.9.4.tar", last modified: Wed Jul 12 04:28:35 2023, max compression
```

## Comparing `aicodebot-0.9.3.tar` & `aicodebot-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 03:48:03.000000 aicodebot-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 03:48:30.240017 aicodebot-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 03:48:03.000000 aicodebot-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-12 03:48:03.000000 aicodebot-0.9.3/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:48:30.240017 aicodebot-0.9.3/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 03:48:30.000000 aicodebot-0.9.3/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 03:48:03.000000 aicodebot-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:48:30.240017 aicodebot-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-12 03:48:03.000000 aicodebot-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:28:35.811463 aicodebot-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 04:28:06.000000 aicodebot-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 04:28:35.811463 aicodebot-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 04:28:06.000000 aicodebot-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:28:35.811463 aicodebot-0.9.4/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-12 04:28:06.000000 aicodebot-0.9.4/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:28:35.811463 aicodebot-0.9.4/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 04:28:35.000000 aicodebot-0.9.4/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 04:28:06.000000 aicodebot-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 04:28:35.811463 aicodebot-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 04:28:06.000000 aicodebot-0.9.4/setup.py
```

### Comparing `aicodebot-0.9.3/LICENSE` & `aicodebot-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/PKG-INFO` & `aicodebot-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.3
-Summary: Your AI-powered coding sidekick 🤖
+Version: 0.9.4
+Summary: AI-powered tool for developers, simplifying coding tasks and improving workflow efficiency.
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.9.3/README.md` & `aicodebot-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/aicodebot/cli.py` & `aicodebot-0.9.4/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/aicodebot/coder.py` & `aicodebot-0.9.4/aicodebot/coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,17 @@
     def git_diff_context(commit=None):
         """Get a text representation of the git diff for the current commit or staged files, including new files"""
         base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
 
         if commit:
             # If a commit is provided, just get the diff for that commit
             logger.debug(f"Getting diff for commit {commit}")
-            return exec_and_get_output(["git", "show", commit])
+            show = exec_and_get_output(["git", "show", commit])
+            logger.debug(f"Diff for commit {commit}: {show}")
+            return show
         else:
             # Otherwise, get the diff for the staged files, or if there are none, the diff for the unstaged files
             staged_files = exec_and_get_output(["git", "diff", "--cached", "--name-only"]).splitlines()
             if staged_files:
                 logger.debug(f"Getting diff for staged files: {staged_files}")
                 diff_type = "--cached"
             else:
```

### Comparing `aicodebot-0.9.3/aicodebot/config.py` & `aicodebot-0.9.4/aicodebot/config.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/aicodebot/helpers.py` & `aicodebot-0.9.4/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/aicodebot/prompts.py` & `aicodebot-0.9.4/aicodebot/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     "Peter": SimpleNamespace(name="Peter", prompt=PETER, description="Peter Griffin from Family Guy"),
     "Sherlock": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
     "Socrates": SimpleNamespace(
         name="Socrates", prompt=SOCRATES, description="Socrates, the classical Greek philosopher"
     ),
     "Spock": SimpleNamespace(name="Spock", prompt=SPOCK, description="Dr. Spock from Star Trek"),
 }
-DEFAULT_PERSONALITY = PERSONALITIES["Einstein"]
+DEFAULT_PERSONALITY = PERSONALITIES["Spock"]
 
 
 def get_personality_prompt():
     """Generates a prompt for the sidekick personality."""
     default_personality = DEFAULT_PERSONALITY.name
     if os.getenv("AICODEBOT_PERSONALITY"):
         personality = os.getenv("AICODEBOT_PERSONALITY")
```

### Comparing `aicodebot-0.9.3/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.4/aicodebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.3
-Summary: Your AI-powered coding sidekick 🤖
+Version: 0.9.4
+Summary: AI-powered tool for developers, simplifying coding tasks and improving workflow efficiency.
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.9.3/pyproject.toml` & `aicodebot-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.3/setup.py` & `aicodebot-0.9.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if __name__ == "__main__":  # Only run setup if this is the main file (allows this file to be imported for __version__)
     setup(
         name="aicodebot",
         python_requires=">=3.9",
         version=version,
         url="https://github.com/gorillamania/AICodeBot",
         author="Nick Sullivan",
-        description="Your AI-powered coding sidekick 🤖",
+        description="AI-powered tool for developers, simplifying coding tasks and improving workflow efficiency.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         keywords="AI, coding, assistant, pair-programming, automation",
         install_requires=requirements,
         entry_points={
             "console_scripts": [
                 "aicodebot = aicodebot.cli:cli",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

