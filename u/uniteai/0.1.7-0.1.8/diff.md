# Comparing `tmp/uniteai-0.1.7.tar.gz` & `tmp/uniteai-0.1.8.tar.gz`

## Comparing `uniteai-0.1.7.tar` & `uniteai-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/.dir-locals.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/common.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/config.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/edit.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/llm_server.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/local_llm.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/lsp_server.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/openai.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/server.py
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/transcription.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/contrib/example.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.7/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.7/LICENSE
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.7/README.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uniteai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 uniteai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/.dir-locals.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/__init__.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/common.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/config.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/edit.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/llm_server.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/local_llm.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/lsp_server.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/openai.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/server.py
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/transcription.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.8/uniteai/contrib/example.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.8/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.8/LICENSE
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.8/README.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uniteai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 uniteai-0.1.8/PKG-INFO
```

### Comparing `uniteai-0.1.7/uniteai/common.py` & `uniteai-0.1.8/uniteai/common.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/config.py` & `uniteai-0.1.8/uniteai/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,24 @@
 import sys
 import shutil
 import logging
 from uniteai.common import mk_logger
 
 log = mk_logger('CONFIG', logging.WARN)
 
+CONFIG_PATHS = [
+    '.uniteai.yml',
+    '.uniteai.yaml',
+    os.path.expanduser('~/.uniteai.yaml'),
+    os.path.expanduser('~/.uniteai.yml'),
+]
+
+
 def handle_missing_config():
+    '''Possibly create a default config, and then exit.'''
     log.error('No config file found!')
     ans = input('Would you like this process to copy the default `.uniteai.yml.example` config file into the current directory?')
 
     if ans.lower() in ['y', 'yes']:
         log.info('''
 Copying `.uniateai.yml.example` to `.uniteai.yml`
 Please review it before running the LSP again.
@@ -41,40 +50,34 @@
         if not os.path.exists(config_path):
             shutil.copyfile(example_config_path, config_path)
     else:
         log.error('''Please manually copy and update the file `.uniateai.yml.example` from https://github.com/freckletonj/uniteai.''')
     sys.exit(1)
 
 
-
-def load_config(file_paths):
+def load_config(file_paths=CONFIG_PATHS):
     ''' Return first config file that exists. '''
     for file_path in file_paths:
         if os.path.exists(file_path):
             log.info(f'Reading configuration from: {file_path}')
             with open(file_path, 'r') as f:
                 return yaml.safe_load(f)
-    return None
+
+    # Will exit after possibly copying a new config
+    if config_yaml is None:
+        handle_missing_config()
 
 def get_args():
     ''' This first pass will learn generic LSP-related config, and what further
     modules need to be loaded. Those modules will be able to specify their own
     configuration, which will be gathered in a second round of config parsing.
     '''
     # Load config file
 
-    config_yaml = load_config([
-        '.uniteai.yml',
-        '.uniteai.yaml',
-        os.path.expanduser('~/.uniteai.yaml'),
-        os.path.expanduser('~/.uniteai.yml'),
-    ])
-    print(f'CONFIGYAML: {config_yaml}')
-    if config_yaml is None:
-        handle_missing_config()
+    config_yaml = load_config(CONFIG_PATHS)
 
     # Parse command-line arguments
     parser = argparse.ArgumentParser()
 
     # LSP-related config
     parser.add_argument('--stdio', action='store_true', default=True)
     parser.add_argument('--tcp', action='store_true')
```

### Comparing `uniteai-0.1.7/uniteai/edit.py` & `uniteai-0.1.8/uniteai/edit.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/llm_server.py` & `uniteai-0.1.8/uniteai/llm_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from typing import List
 import threading
 import torch
 import yaml
 import multiprocessing as mp
 import logging
 from uniteai.common import get_nested
+from uniteai.config import load_config
 import uvicorn
 
 
 ##################################################
 # `transformers`
 
 def load_model(args):
@@ -87,17 +88,16 @@
         )
         return tokenizer, model
 
 
 ##################################################
 # Initialization
 
-with open(".uniteai.yml", 'r') as file:
-    config = yaml.safe_load(file)
-    args = config['local_llm']
+config = load_config()
+args = config['local_llm']
 
 
 ##################################################
 # Types
 
 class AutocompleteRequest(BaseModel):
     text: str
@@ -208,13 +208,13 @@
     ''' End ongoing inferrence '''
     global local_llm_stop_event
     local_llm_stop_event.set()
     return Response(status_code=200)
 
 
 def main():
-    uvicorn.run("llm_server:app",
+    uvicorn.run("uniteai.llm_server:app",
                 host=get_nested(config, ['local_llm', 'host']),
                 port=get_nested(config, ['local_llm', 'port']))
 
 if __name__ == "__main__":
     main()
```

### Comparing `uniteai-0.1.7/uniteai/local_llm.py` & `uniteai-0.1.8/uniteai/local_llm.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/lsp_server.py` & `uniteai-0.1.8/uniteai/lsp_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/openai.py` & `uniteai-0.1.8/uniteai/openai.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/server.py` & `uniteai-0.1.8/uniteai/server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/transcription.py` & `uniteai-0.1.8/uniteai/transcription.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/uniteai/contrib/example.py` & `uniteai-0.1.8/uniteai/contrib/example.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/LICENSE` & `uniteai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/README.md` & `uniteai-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.7/pyproject.toml` & `uniteai-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uniteai"
-version = "0.1.7"
+version = "0.1.8"
 description = "AI, Inside your Editor."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [{ name = "Josh Freckleton"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
```

### Comparing `uniteai-0.1.7/PKG-INFO` & `uniteai-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniteai
-Version: 0.1.7
+Version: 0.1.8
 Summary: AI, Inside your Editor.
 Project-URL: Homepage, https://github.com/freckletonj/uniteai
 Project-URL: Bug Tracker, https://github.com/freckletonj/uniteai/issues
 Author: Josh Freckleton
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

