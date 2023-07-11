# Comparing `tmp/connpy-3.2.8.tar.gz` & `tmp/connpy-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.8.tar", last modified: Wed May 24 21:15:10 2023, max compression
+gzip compressed data, was "connpy-3.3.0.tar", last modified: Tue Jul 11 22:34:40 2023, max compression
```

## Comparing `connpy-3.2.8.tar` & `connpy-3.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 21:14:54.000000 connpy-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-24 21:15:10.386407 connpy-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-24 21:14:54.000000 connpy-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22046 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-24 21:15:10.386407 connpy-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 21:14:54.000000 connpy-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 22:34:26.000000 connpy-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-11 22:34:40.562689 connpy-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-11 22:34:26.000000 connpy-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24594 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4518 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56866 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29185 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 22:34:40.566689 connpy-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 22:34:26.000000 connpy-3.3.0/setup.py
```

### Comparing `connpy-3.2.8/LICENSE` & `connpy-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.8/PKG-INFO` & `connpy-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.8
+Version: 3.3.0
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -154,14 +154,15 @@
   move (mv)      Move node
   copy (cp)      Copy node
   list (ls)      List profiles, nodes or folders
   bulk           Add nodes in bulk
   run            Run scripts or commands on nodes
   config         Manage app config
   api            Start and stop connpy api
+  ai             Make request to an AI
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.2.8/README.md` & `connpy-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
   move (mv)      Move node
   copy (cp)      Copy node
   list (ls)      List profiles, nodes or folders
   bulk           Add nodes in bulk
   run            Run scripts or commands on nodes
   config         Manage app config
   api            Start and stop connpy api
+  ai             Make request to an AI
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.2.8/connpy/__init__.py` & `connpy-3.3.0/connpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
   move (mv)      Move node
   copy (cp)      Copy node
   list (ls)      List profiles, nodes or folders
   bulk           Add nodes in bulk
   run            Run scripts or commands on nodes
   config         Manage app config
   api            Start and stop connpy api
+  ai             Make request to an AI
 ```
 
 ###   Manage profiles
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.2.8/connpy/ai.py` & `connpy-3.3.0/connpy/ai.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         - temp       (float): Value between 0 and 1 that control the randomness 
                               of generated text, with higher values increasing 
                               creativity. Default is 0.7.
 
         '''
 
-    def __init__(self, config, org = None, api_key = None, model = "gpt-3.5-turbo", temp = 0.7):
+    def __init__(self, config, org = None, api_key = None, model = None, temp = 0.7):
         ''' 
             
         ### Parameters:  
 
             - config (obj): Pass the object created with class configfile with 
                             key for decryption and extra configuration if you 
                             are using connection manager.  
@@ -56,92 +56,128 @@
         if api_key:
             openai.api_key = api_key
         else:
             try: 
                 openai.api_key = self.config.config["openai"]["api_key"]
             except:
                 raise ValueError("Missing openai api_key")
+        if model:
+            self.model = model
+        else:
+            try:
+                self.model = self.config.config["openai"]["model"]
+            except:
+                self.model = "gpt-3.5-turbo-0613"
+        self.temp = temp
         self.__prompt = {}
         self.__prompt["original_system"] = """
-            You are the AI assistant of a network connection manager and automation app called connpy. When provided with user input analyze the input and extract the following information:
+            You are the AI chatbot and assistant of a network connection manager and automation app called connpy. When provided with user input analyze the input and extract the following information. If user wants to chat just reply and don't call a function:
 
-            - app_related: True if the input is related to the application's purpose and the request is understood; False if the input is not related, not understood, or if mandatory information like filter is missing. If user ask information about the app it should be false 
             - type: Given a user input, identify the type of request they want to make. The input will represent one of two options: 
 
                 1. "command" - The user wants to get information from devices by running commands.
                 2. "list_nodes" - The user wants to get a list of nodes, devices, servers, or routers.
                 The 'type' field should reflect whether the user input is a command or a request for a list of nodes.
 
-            - filter: One or more regex patterns indicating the device or group of devices the command should be run on, returned as a Python list (e.g., ['hostname', 'hostname@folder', '@subfolder@folder']). The filter can have different formats, such as:
+            - filter: One or more regex patterns indicating the device or group of devices the command should be run on. The filter can have different formats, such as:
                 - hostname
                 - hostname@folder
                 - hostname@subfolder@folder
                 - partofhostname
                 - @folder
                 - @subfolder@folder
                 - regex_pattern
 
                 The filter should be extracted from the user input exactly as it was provided.
                 Always preserve the exact filter pattern provided by the user, with no modifications. Do not process any regex, the application can do that.
-                If no filter is specified, set it to None.
 
-            - Expected: This field represents an expected output to search for when running the command. It's an optional value for the user.
-Set it to 'None' if no value was captured.
-The expected value should ALWAYS come from the user input explicitly.
-Users will typically use words like verify, check, make sure, or similar to refer to the expected value.
-
-            - response: An optional field to be filled when app_related is False or when providing an explanation related to the app. This is where you can engage in small talk, answer questions not related to the app, or provide explanations about the extracted information.
-            
-            Always respond in the following format:
-                
-                app_related: {{app_related}}
-                Type: {{command}}
-                Filter: {{filter}}
-                Expected: {{expected}}
-                Response: {{response}}
     """ 
         self.__prompt["original_user"] = "Get the IP addresses of loopback0 for all routers from w2az1 and e1.*(prod|dev) and check if they have the ip 192.168.1.1"
-        self.__prompt["original_assistant"] = "app_related: True\nType: Command\nFilter: ['w2az1', 'e1.*(prod|dev)']\nExpected: 192.168.1.1"
+        self.__prompt["original_assistant"] = {"name": "get_network_device_info", "arguments": "{\n  \"type\": \"command\",\n  \"filter\": [\"w2az1\",\"e1.*(prod|dev)\"]\n}"}
+        self.__prompt["original_function"] = {}
+        self.__prompt["original_function"]["name"] = "get_network_device_info"
+        self.__prompt["original_function"]["descriptions"] = "You are the AI chatbot and assistant of a network connection manager and automation app called connpy. When provided with user input analyze the input and extract the information acording to the function, If user wants to chat just reply and don't call a function",
+        self.__prompt["original_function"]["parameters"] = {}
+        self.__prompt["original_function"]["parameters"]["type"] = "object"
+        self.__prompt["original_function"]["parameters"]["properties"] = {}
+        self.__prompt["original_function"]["parameters"]["properties"]["type"] = {}
+        self.__prompt["original_function"]["parameters"]["properties"]["type"]["type"] = "string"
+        self.__prompt["original_function"]["parameters"]["properties"]["type"]["description"] ="""
+Categorize the user's request based on the operation they want to perform on the nodes. The requests can be classified into the following categories:
+
+    1. "command" - This represents a request to retrieve specific information or configurations from nodes. An example would be: "go to routers in @office and get the config".
+
+    2. "list_nodes" - This is when the user wants a list of nodes. An example could be: "get me the nodes in @office".
+"""
+        self.__prompt["original_function"]["parameters"]["properties"]["type"]["enum"] = ["command", "list_nodes"]
+        self.__prompt["original_function"]["parameters"]["properties"]["filter"] = {}
+        self.__prompt["original_function"]["parameters"]["properties"]["filter"]["type"] = "array"
+        self.__prompt["original_function"]["parameters"]["properties"]["filter"]["items"] = {}
+        self.__prompt["original_function"]["parameters"]["properties"]["filter"]["items"]["type"] = "string"
+        self.__prompt["original_function"]["parameters"]["properties"]["filter"]["items"]["description"] = """One or more regex patterns indicating the device or group of devices the command should be run on.  The filter should be extracted from the user input exactly as it was provided. 
+                The filter can have different formats, such as:
+                - hostname
+                - hostname@folder
+                - hostname@subfolder@folder
+                - partofhostname
+                - @folder
+                - @subfolder@folder
+                - regex_pattern
+                """
+        self.__prompt["original_function"]["parameters"]["required"] = ["type", "filter"]
         self.__prompt["command_system"] = """
-        For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server). Always format your response as a Python list (e.g., ['command1', 'command2']). 
-
+        For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server).
         The application knows how to connect to devices via SSH, so you only need to provide the command(s) to run after connecting. 
-
         If the commands needed are not for the specific OS type, just send an empty list (e.g., []). 
-
-        It is crucial to always include the device name provided in your response, even when there is only one device.
-
         Note: Preserving the integrity of user-provided commands is of utmost importance. If a user has provided a specific command to run, include that command exactly as it was given, even if it's not recognized or understood. Under no circumstances should you modify or alter user-provided commands.
-
-        Your response has to be always like this:
-            node1: ["command1", "command2"]
-            node2: ["command1", "command2", "command3"]
-            node1@folder: ["command1"]
-            Node4@subfolder@folder: []
     """
         self.__prompt["command_user"]= """
     input: show me the full configuration for all this devices:
 
     Devices:
     router1: cisco ios
     """
-        self.__prompt["command_assistant"]= """
-    router1: ['show running-config']
+        self.__prompt["command_assistant"] = {"name": "get_commands", "arguments": "{\n  \"router1\": \"show running-configuration\"\n}"}
+        self.__prompt["command_function"] = {}
+        self.__prompt["command_function"]["name"] = "get_commands"
+        self.__prompt["command_function"]["descriptions"] = """ 
+        For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server).
+        The application knows how to connect to devices via SSH, so you only need to provide the command(s) to run after connecting. 
+        If the commands needed are not for the specific OS type, just send an empty list (e.g., []). 
     """
+        self.__prompt["command_function"]["parameters"] = {}
+        self.__prompt["command_function"]["parameters"]["type"] = "object"
+        self.__prompt["command_function"]["parameters"]["properties"] = {}
         self.__prompt["confirmation_system"] = """
         Please analyze the user's input and categorize it as either an affirmation or negation. Based on this analysis, respond with:
 
-            'True' if the input is an affirmation like 'do it', 'go ahead', 'sure', etc.
-            'False' if the input is a negation.
-            If the input does not fit into either of these categories, kindly express that you didn't understand and request the user to rephrase their response.
+            'true' if the input is an affirmation like 'do it', 'go ahead', 'sure', etc.
+            'false' if the input is a negation.
+            'none' If the input does not fit into either of these categories.
             """
         self.__prompt["confirmation_user"] = "Yes go ahead!"
         self.__prompt["confirmation_assistant"] = "True"
-        self.model = model
-        self.temp = temp
+        self.__prompt["confirmation_function"] = {}
+        self.__prompt["confirmation_function"]["name"] = "get_confirmation"
+        self.__prompt["confirmation_function"]["descriptions"] = """ 
+        Analize user request and respond:
+    """
+        self.__prompt["confirmation_function"]["parameters"] = {}
+        self.__prompt["confirmation_function"]["parameters"]["type"] = "object"
+        self.__prompt["confirmation_function"]["parameters"]["properties"] = {}
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["result"] = {}
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["description"] = """'true' if the input is an affirmation like 'do it', 'go ahead', 'sure', etc.
+'false' if the input is a negation.
+'none' If the input does not fit into either of these categories"""
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["type"] = "string"
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["enum"] = ["true", "false", "none"]
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["response"] = {}
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["description"] = "If the user don't message is not an affiramtion or negation, kindly ask the user to rephrase."
+        self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["type"] = "string"
+        self.__prompt["confirmation_function"]["parameters"]["required"] = ["result"]
 
     def process_string(self, s):
         if s.startswith('[') and s.endswith(']') and not (s.startswith("['") and s.endswith("']")) and not (s.startswith('["') and s.endswith('"]')):
             # Extract the content inside square brackets and split by comma
             content = s[1:-1].split(',')
             # Add single quotes around each item and join them back together with commas
             new_content = ', '.join(f"'{item.strip()}'" for item in content)
@@ -161,154 +197,131 @@
                 time.sleep(wait_time)
                 retries += 1
                 continue
         if retries == max_retries:
             myfunction = False
         return myfunction
 
-    def _clean_original_response(self, raw_response):
-        #Parse response for first request to openAI GPT.
-        info_dict = {}
-        info_dict["app_related"] = False
-        current_key = "response"
-        for line in raw_response.split("\n"):
-            if line.strip() == "":
-                line = "\n"
-            possible_keys = ["app_related", "type", "filter", "expected", "response"]
-            if ':' in line and (key := line.split(':', 1)[0].strip().lower()) in possible_keys:
-                key, value = line.split(":", 1)
-                key = key.strip().lower()
-                value = value.strip()
-                # Convert "true" or "false" (case-insensitive) to Python boolean
-                if value.lower() == "true":
-                    value = True
-                elif value.lower() == "false":
-                    value = False
-                elif value.lower() == "none":
-                    value = None
-                if key == "filter":
-                    value = self.process_string(value)
-                    value = ast.literal_eval(value)
-                #store in dictionary
-                info_dict[key] = value
-                current_key = key
-            else:
-                if current_key == "response":
-                    if "response" in info_dict:
-                        info_dict[current_key] += "\n" + line
-                    else:
-                        info_dict[current_key] = line
-
-        return info_dict
-
     def _clean_command_response(self, raw_response):
         #Parse response for command request to openAI GPT.
         info_dict = {}
         info_dict["commands"] = []
         info_dict["variables"] = {}
         info_dict["variables"]["__global__"] = {}
-        for line in raw_response.split("\n"):
-            if ":" in line:
-                key, value = line.split(":", 1)
-                key = key.strip()
-                newvalue = {}
-                pattern = r'\[.*?\]'
-                match = re.search(pattern, value.strip())
-                try:
-                    value = ast.literal_eval(match.group(0))
-                    for i,e in enumerate(value, start=1):
-                        newvalue[f"command{i}"] = e
-                        if f"{{command{i}}}" not in info_dict["commands"]:
-                            info_dict["commands"].append(f"{{command{i}}}")
-                            info_dict["variables"]["__global__"][f"command{i}"] = ""
-                    info_dict["variables"][key] = newvalue
-                except:
-                    pass
+        for key, value in raw_response.items():
+            key = key.strip()
+            newvalue = {}
+            for i,e in enumerate(value, start=1):
+                newvalue[f"command{i}"] = e
+                if f"{{command{i}}}" not in info_dict["commands"]:
+                    info_dict["commands"].append(f"{{command{i}}}")
+                    info_dict["variables"]["__global__"][f"command{i}"] = ""
+                info_dict["variables"][key] = newvalue
         return info_dict
 
-    def _clean_confirmation_response(self, raw_response):
-        #Parse response for confirmation request to openAI GPT.
-        value = raw_response.strip()
-        if value.strip(".").lower() == "true":
-            value = True
-        elif value.strip(".").lower() == "false":
-            value = False
-        return value
-
     def _get_commands(self, user_input, nodes):
         #Send the request for commands for each device to openAI GPT.
         output_list = []
+        command_function = deepcopy(self.__prompt["command_function"])
         for key, value in nodes.items():
             tags = value.get('tags', {})
             try:
                 if os_value := tags.get('os'):
                     output_list.append(f"{key}: {os_value}")
+                    command_function["parameters"]["properties"][key] = {}
+                    command_function["parameters"]["properties"][key]["type"] = "array"
+                    command_function["parameters"]["properties"][key]["description"] = f"OS: {os_value}"
+                    command_function["parameters"]["properties"][key]["items"] = {}
+                    command_function["parameters"]["properties"][key]["items"]["type"] = "string" 
             except:
                 pass
         output_str = "\n".join(output_list)
         command_input = f"input: {user_input}\n\nDevices:\n{output_str}"
         message = []
         message.append({"role": "system", "content": dedent(self.__prompt["command_system"]).strip()})
         message.append({"role": "user", "content": dedent(self.__prompt["command_user"]).strip()})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["command_assistant"]).strip()})
+        message.append({"role": "assistant", "content": None, "function_call": self.__prompt["command_assistant"]})
         message.append({"role": "user", "content": command_input})
+        functions = [command_function]
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
+            functions=functions,
+            function_call={"name": "get_commands"},
             temperature=self.temp
             )
         output = {}
-        output["dict_response"] = response
-        output["raw_response"] = response["choices"][0]["message"]["content"] 
-        output["response"] = self._clean_command_response(output["raw_response"])
+        result = response["choices"][0]["message"].to_dict()
+        json_result = json.loads(result["function_call"]["arguments"])
+        output["response"] = self._clean_command_response(json_result)
         return output
 
     def _get_filter(self, user_input, chat_history = None):
         #Send the request to identify the filter and other attributes from the user input to GPT.
         message = []
         message.append({"role": "system", "content": dedent(self.__prompt["original_system"]).strip()})
         message.append({"role": "user", "content": dedent(self.__prompt["original_user"]).strip()})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["original_assistant"]).strip()})
+        message.append({"role": "assistant", "content": None, "function_call": self.__prompt["original_assistant"]})
+        functions = [self.__prompt["original_function"]]
         if not chat_history:
             chat_history = []
         chat_history.append({"role": "user", "content": user_input})
         message.extend(chat_history)
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
+            functions=functions,
+            function_call="auto",
             temperature=self.temp,
             top_p=1
             )
 
+        def extract_quoted_strings(text):
+            pattern = r'["\'](.*?)["\']'
+            matches = re.findall(pattern, text)
+            return matches
+        expected = extract_quoted_strings(user_input)
         output = {}
-        output["dict_response"] = response
-        output["raw_response"] = response["choices"][0]["message"]["content"] 
-        chat_history.append({"role": "assistant", "content": output["raw_response"]})
+        result = response["choices"][0]["message"].to_dict()
+        if result["content"]:
+            output["app_related"] = False
+            chat_history.append({"role": "assistant", "content": result["content"]})
+            output["response"] = result["content"]
+        else:
+            json_result = json.loads(result["function_call"]["arguments"])
+            output["app_related"] = True
+            output["filter"] = json_result["filter"]
+            output["type"] = json_result["type"]
+            chat_history.append({"role": "assistant", "content": result["content"], "function_call": {"name": result["function_call"]["name"], "arguments": json.dumps(json_result)}})
+        output["expected"] = expected
         output["chat_history"] = chat_history
-        clear_response = self._clean_original_response(output["raw_response"])
-        output["response"] = self._clean_original_response(output["raw_response"])
         return output
         
     def _get_confirmation(self, user_input):
         #Send the request to identify if user is confirming or denying the task
         message = []
-        message.append({"role": "system", "content": dedent(self.__prompt["confirmation_system"]).strip()})
-        message.append({"role": "user", "content": dedent(self.__prompt["confirmation_user"]).strip()})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["confirmation_assistant"]).strip()})
         message.append({"role": "user", "content": user_input})
+        functions = [self.__prompt["confirmation_function"]]
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
+            functions=functions,
+            function_call={"name": "get_confirmation"},
             temperature=self.temp,
             top_p=1
             )
+        result = response["choices"][0]["message"].to_dict()
+        json_result = json.loads(result["function_call"]["arguments"])
         output = {}
-        output["dict_response"] = response
-        output["raw_response"] = response["choices"][0]["message"]["content"] 
-        output["response"] = self._clean_confirmation_response(output["raw_response"])
+        if json_result["result"] == "true":
+            output["result"] = True
+        elif json_result["result"] == "false":
+            output["result"] = False
+        elif json_result["result"] == "none":
+            output["result"] = json_result["response"]
         return output
 
     def confirm(self, user_input, max_retries=3, backoff_num=1):
         '''
         Send the user input to openAI GPT and verify if response is afirmative or negative.
 
         ### Parameters:  
@@ -323,15 +336,15 @@
 
         ### Returns:  
 
             bool or str: True, False or str if AI coudn't understand the response
         '''
         result = self._retry_function(self._get_confirmation, max_retries, backoff_num, user_input)
         if result:
-            output = result["response"]
+            output = result["result"]
         else:
             output = f"{self.model} api is not responding right now, please try again later."
         return output
 
     def ask(self, user_input, dryrun = False, chat_history = None,  max_retries=3, backoff_num=1):
         '''
         Send the user input to openAI GPT and parse the response to run an action in the application.
@@ -385,22 +398,22 @@
         output["dryrun"] = dryrun
         output["input"] = user_input
         original = self._retry_function(self._get_filter, max_retries, backoff_num, user_input, chat_history)
         if not original:
             output["app_related"] = False
             output["response"] = f"{self.model} api is not responding right now, please try again later."
             return output
-        output["app_related"] = original["response"]["app_related"]
+        output["app_related"] = original["app_related"]
         output["chat_history"] = original["chat_history"]
         if not output["app_related"]:
-            output["response"] = original["response"]["response"]
+            output["response"] = original["response"]
         else:
-            type = original["response"]["type"].lower()
-            if "filter" in original["response"]:
-                output["filter"] = original["response"]["filter"]
+            type = original["type"]
+            if "filter" in original:
+                output["filter"] = original["filter"]
                 if not self.config.config["case"]:
                     if isinstance(output["filter"], list):
                         output["filter"] = [item.lower() for item in output["filter"]]
                     else:
                         output["filter"] = output["filter"].lower()
                 if not dryrun or type == "command":
                     thisnodes = self.config._getallnodesfull(output["filter"])
@@ -419,16 +432,16 @@
                     output["app_related"] = False
                     output["response"] = f"{self.model} api is not responding right now, please try again later."
                     return output
                 output["args"] = {}
                 output["args"]["commands"] = commands["response"]["commands"]
                 output["args"]["vars"] = commands["response"]["variables"]
                 output["nodes"] = [item for item in output["nodes"] if output["args"]["vars"].get(item)]
-                if original["response"].get("expected"):
-                    output["args"]["expected"] = original["response"]["expected"]
+                if original.get("expected"):
+                    output["args"]["expected"] = original["expected"]
                     output["action"] = "test"
                 else:
                     output["action"] = "run"
                 if dryrun:
                     output["task"] = []
                     if output["action"] == "test":
                         output["task"].append({"Task": "Verify if expected value is in command(s) output"})
```

### Comparing `connpy-3.2.8/connpy/api.py` & `connpy-3.3.0/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.8/connpy/completion.py` & `connpy-3.3.0/connpy/completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import json
+import glob
 
 def _getallnodes(config):
     #get all nodes on configfile
     nodes = []
     layer1 = [k for k,v in config["connections"].items() if isinstance(v, dict) and v["type"] == "connection"]
     folders = [k for k,v in config["connections"].items() if isinstance(v, dict) and v["type"] == "folder"]
     nodes.extend(layer1)
@@ -32,48 +33,71 @@
     defaultdir = home + '/.config/conn'
     defaultfile = defaultdir + '/config.json'
     jsonconf = open(defaultfile)
     config = json.load(jsonconf)
     nodes = _getallnodes(config)
     folders = _getallfolders(config)
     profiles = list(config["profiles"].keys())
-    wordsnumber = int(sys.argv[1])
-    words = sys.argv[3:]
+    app = sys.argv[1]
+    if app in ["bash", "zsh"]:
+        positions = [2,4]
+    else:
+        positions = [1,3]
+    wordsnumber = int(sys.argv[positions[0]])
+    words = sys.argv[positions[1]:]
     if wordsnumber == 2:
-        strings=["--add", "--del", "--rm", "--edit", "--mod", "--show", "mv", "move", "ls", "list", "cp", "copy", "profile", "run", "bulk", "config", "api", "--help"]
+        strings=["--add", "--del", "--rm", "--edit", "--mod", "--show", "mv", "move", "ls", "list", "cp", "copy", "profile", "run", "bulk", "config", "api", "ai", "--help"]
         strings.extend(nodes)
         strings.extend(folders)
 
+    elif wordsnumber >= 3 and words[0] == "ai":
+        if wordsnumber == 3:
+            strings = ["--help", "--org", "--model", "--api_key"]
+        else:
+            strings = ["--org", "--model", "--api_key"]
     elif wordsnumber == 3:
         strings=[]
         if words[0] == "profile":
             strings=["--add", "--rm", "--del", "--edit", "--mod", "--show", "--help"]
         if words[0] == "config":
-            strings=["--allow-uppercase", "--keepalive", "--completion", "--fzf", "--configfolder", "--help"]
+            strings=["--allow-uppercase", "--keepalive", "--completion", "--fzf", "--configfolder", "--openai-org", "--openai-org-api-key", "--openai-org-model","--help"]
         if words[0] == "api":
             strings=["--start", "--stop", "--restart", "--debug", "--help"]
         if words[0] in ["--mod", "--edit", "-e", "--show", "-s", "--add", "-a", "--rm", "--del", "-r"]:
             strings=["profile"]
         if words[0] in ["list", "ls"]:
             strings=["profiles", "nodes", "folders"]
         if words[0] in ["bulk", "mv", "cp", "copy", "run"]:
             strings=["--help"]
         if words[0] in ["--rm", "--del", "-r"]:
             strings.extend(folders)
-        if words[0] in ["--rm", "--del", "-r", "--mod", "--edit", "-e", "--show", "-s", "mv", "move", "cp", "copy", "run"]:
+        if words[0] in ["--rm", "--del", "-r", "--mod", "--edit", "-e", "--show", "-s", "mv", "move", "cp", "copy"]:
+            strings.extend(nodes)
+        if words[0] == "run":
+            if words[-1] == "run":
+                path = './*'
+            else:
+                path = words[-1] + "*"
+            strings = glob.glob(path)
+            for i in range(len(strings)):
+                if os.path.isdir(strings[i]):
+                    strings[i] += '/'
+            strings = [s[2:] if s.startswith('./') else s for s in strings]
             strings.extend(nodes)
 
     elif wordsnumber == 4:
           strings=[]
           if words[0] == "profile" and words[1] in ["--rm", "--del", "-r", "--mod", "--edit", "-e", "--show", "-s"]:
               strings.extend(profiles)
           if words[1] == "profile" and words[0] in ["--rm", "--del", "-r", "--mod", "--edit", "-e", "--show", "-s"]:
               strings.extend(profiles)
           if words[0] == "config" and words[1] == "--completion":
               strings=["bash", "zsh"]
           if words[0] == "config" and words[1] in ["--fzf", "--allow-uppercase"]:
               strings=["true", "false"]
 
-    print(*strings)
+    if app == "bash":
+        strings = [s if s.endswith('/') else f"'{s} '" for s in strings]
+    print('\t'.join(strings))
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `connpy-3.2.8/connpy/configfile.py` & `connpy-3.3.0/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.8/connpy/connapp.py` & `connpy-3.3.0/connpy/connapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 import ast
 import argparse
 import sys
 import inquirer
 from .core import node,nodes
 from ._version import __version__
 from .api import start_api,stop_api,debug_api
+from .ai import ai
 import yaml
 import ast
+from rich import print as mdprint
+from rich.markdown import Markdown
 try:
     from pyfzf.pyfzf import FzfPrompt
 except:
     FzfPrompt = None
 home = os.path.expanduser("~")
 defaultdir = home + '/.config/conn'
 
@@ -95,14 +98,21 @@
         lsparser = subparsers.add_parser("list", aliases=["ls"], help="List profiles, nodes or folders") 
         lsparser.add_argument("ls", action=self._store_type, choices=["profiles","nodes","folders"], help="List profiles, nodes or folders", default=False)
         lsparser.set_defaults(func=self._func_others)
         #BULKPARSER
         bulkparser = subparsers.add_parser("bulk", help="Add nodes in bulk") 
         bulkparser.add_argument("bulk", const="bulk", nargs=0, action=self._store_type, help="Add nodes in bulk")
         bulkparser.set_defaults(func=self._func_others)
+        # AIPARSER
+        aiparser = subparsers.add_parser("ai", help="Make request to an AI") 
+        aiparser.add_argument("ask", nargs='*', help="Ask connpy AI something")
+        aiparser.add_argument("--model", nargs=1, help="Set the OPENAI model id")
+        aiparser.add_argument("--org", nargs=1, help="Set the OPENAI organization id")
+        aiparser.add_argument("--api_key", nargs=1, help="Set the OPENAI API key")
+        aiparser.set_defaults(func=self._func_ai)
         #RUNPARSER
         runparser = subparsers.add_parser("run", help="Run scripts or commands on nodes", formatter_class=argparse.RawTextHelpFormatter) 
         runparser.add_argument("run", nargs='+', action=self._store_type, help=self._help("run"), default="run")
         runparser.add_argument("-g","--generate", dest="action", action="store_const", help="Generate yaml file template", const="generate", default="run")
         runparser.set_defaults(func=self._func_run)
         #APIPARSER
         apiparser = subparsers.add_parser("api", help="Start and stop connpy api") 
@@ -116,18 +126,20 @@
         configparser = subparsers.add_parser("config", help="Manage app config") 
         configcrud = configparser.add_mutually_exclusive_group(required=True)
         configcrud.add_argument("--allow-uppercase", dest="case", nargs=1, action=self._store_type, help="Allow case sensitive names", choices=["true","false"])
         configcrud.add_argument("--fzf", dest="fzf", nargs=1, action=self._store_type, help="Use fzf for lists", choices=["true","false"])
         configcrud.add_argument("--keepalive", dest="idletime", nargs=1, action=self._store_type, help="Set keepalive time in seconds, 0 to disable", type=int, metavar="INT")
         configcrud.add_argument("--completion", dest="completion", nargs=1, choices=["bash","zsh"], action=self._store_type, help="Get terminal completion configuration for conn")
         configcrud.add_argument("--configfolder", dest="configfolder", nargs=1, action=self._store_type, help="Set the default location for config file", metavar="FOLDER")
-        configcrud.add_argument("--openai", dest="openai", nargs=2, action=self._store_type, help="Set openai organization and api_key", metavar=("ORGANIZATION", "API_KEY"))
+        configcrud.add_argument("--openai-org", dest="organization", nargs=1, action=self._store_type, help="Set openai organization", metavar="ORGANIZATION")
+        configcrud.add_argument("--openai-api-key", dest="api_key", nargs=1, action=self._store_type, help="Set openai api_key", metavar="API_KEY")
+        configcrud.add_argument("--openai-model", dest="model", nargs=1, action=self._store_type, help="Set openai model", metavar="MODEL")
         configparser.set_defaults(func=self._func_others)
         #Manage sys arguments
-        commands = ["node", "profile", "mv", "move","copy", "cp", "bulk", "ls", "list", "run", "config", "api"]
+        commands = ["node", "profile", "mv", "move","copy", "cp", "bulk", "ls", "list", "run", "config", "api", "ai"]
         profilecmds = ["--add", "-a", "--del", "--rm",  "-r", "--mod", "--edit", "-e", "--show", "-s"]
         if len(argv) >= 2 and argv[1] == "profile" and argv[0] in profilecmds:
             argv[1] = argv[0]
             argv[0] = "profile"
         if len(argv) < 1 or argv[0] not in commands:
             argv.insert(0,"node")
         args = defaultparser.parse_args(argv)
@@ -262,18 +274,22 @@
         if len(matches) == 0:
             print("{} not found".format(args.data))
             exit(2)
         node = self.config.getitem(matches[0])
         for k, v in node.items():
             if isinstance(v, str):
                 print(k + ": " + v)
-            else:
+            elif isinstance(v, list):
                 print(k + ":")
                 for i in v:
                     print("  - " + i)
+            elif isinstance(v, dict):
+                print(k + ":")
+                for i,d in v.items():
+                    print("  - " + i + ": " + d)
 
     def _mod(self, args):
         if args.data == None:
             print("Missing argument node")
             exit(3)
         matches = list(filter(lambda k: k == args.data, self.nodes))
         if len(matches) == 0:
@@ -330,18 +346,22 @@
         if len(matches) == 0:
             print("{} not found".format(args.data[0]))
             exit(2)
         profile = self.config.profiles[matches[0]]
         for k, v in profile.items():
             if isinstance(v, str):
                 print(k + ": " + v)
-            else:
+            elif isinstance(v, list):
                 print(k + ":")
                 for i in v:
                     print("  - " + i)
+            elif isinstance(v, dict):
+                print(k + ":")
+                for i,d in v.items():
+                    print("  - " + i + ": " + d)
 
     def _profile_add(self, args):
         matches = list(filter(lambda k: k == args.data[0], self.profiles))
         if len(matches) > 0:
             print("Profile {} Already exist".format(matches[0]))
             exit(4)
         newprofile = self._questions_profiles(args.data[0])
@@ -371,15 +391,15 @@
         else:
             self.config._profiles_add(**updateprofile)
             self.config._saveconfig(self.config.file)
             print("{} edited succesfully".format(args.data[0]))
     
     def _func_others(self, args):
         #Function called when using other commands
-        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime, "configfolder": self._configfolder, "openai": self._openai}
+        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime, "configfolder": self._configfolder, "organization": self._openai, "api_key": self._openai, "model": self._openai}
         return actions.get(args.command)(args)
 
     def _ls(self, args):
         print(*getattr(self, args.data), sep="\n")
 
     def _mvcp(self, args):
         if not self.case:
@@ -489,31 +509,142 @@
             pathfile = defaultdir + "/.folder"
             folder = os.path.abspath(args.data[0]).rstrip('/')
             with open(pathfile, "w") as f:
                 f.write(str(folder))
             print("Config saved")
         
     def _openai(self, args):
-        openaikeys = {}
-        openaikeys["organization"] = args.data[0]
-        openaikeys["api_key"] = args.data[1]
-        self._change_settings(args.command, openaikeys)
+        if "openai" in self.config.config:
+            openaikeys = self.config.config["openai"]
+        else:
+            openaikeys = {}
+        openaikeys[args.command] = args.data[0]
+        self._change_settings("openai", openaikeys)
 
 
     def _change_settings(self, name, value):
         self.config.config[name] = value
         self.config._saveconfig(self.config.file)
         print("Config saved")
 
     def _func_run(self, args):
         if len(args.data) > 1:
             args.action = "noderun"
         actions = {"noderun": self._node_run, "generate": self._yaml_generate, "run": self._yaml_run}
         return actions.get(args.action)(args)
 
+    def _func_ai(self, args):
+        arguments = {}
+        if args.model:
+            arguments["model"] = args.model[0]
+        if args.org:
+            arguments["org"] = args.org[0]
+        if args.api_key:
+            arguments["api_key"] = args.api_key[0]
+        self.myai = ai(self.config, **arguments)
+        if args.ask:
+            input = " ".join(args.ask)
+            request = self.myai.ask(input, dryrun = True)
+            if not request["app_related"]:
+                mdprint(Markdown(request["response"]))
+                print("\r")
+            else:
+                if request["action"] == "list_nodes":
+                    if request["filter"]:
+                        nodes = self.config._getallnodes(request["filter"])
+                    else:
+                        nodes = self.config._getallnodes()
+                    list = "\n".join(nodes)
+                    print(list)
+                else:
+                    yaml_data = yaml.dump(request["task"])
+                    confirmation = f"I'm going to run the following task:\n```{yaml_data}```"
+                    mdprint(Markdown(confirmation))
+                    question = [inquirer.Confirm("task", message="Are you sure you want to continue?")]
+                    print("\r")
+                    confirm = inquirer.prompt(question)
+                    if confirm == None:
+                        exit(7)
+                    if confirm["task"]:
+                        script = {}
+                        script["name"] = "RESULT"
+                        script["output"] = "stdout"
+                        script["nodes"] = request["nodes"]
+                        script["action"] = request["action"]
+                        if "expected" in request:
+                            script["expected"] = request["expected"]
+                        script.update(request["args"])
+                        self._cli_run(script)
+        else:
+            history = None
+            mdprint(Markdown("**Chatbot**: Hi! How can I help you today?\n\n---"))
+            while True:
+                questions = [
+                        inquirer.Text('message', message="User", validate=self._ai_validation),
+                    ]
+                answers = inquirer.prompt(questions)
+                if answers == None:
+                    exit(7)
+                response, history = self._process_input(answers["message"], history)
+                mdprint(Markdown(f"""**Chatbot**:\n{response}\n\n---"""))
+        return
+
+
+    def _ai_validation(self, answers, current, regex = "^.+$"):
+        #Validate ai user chat.
+        if not re.match(regex, current):
+            raise inquirer.errors.ValidationError("", reason="Can't send empty messages")
+        return True
+
+    def _process_input(self, input, history):
+        response = self.myai.ask(input , chat_history = history, dryrun = True)
+        if not response["app_related"]:
+            if not history:
+                history = []
+            history.extend(response["chat_history"])
+            return response["response"], history
+        else:
+            history = None
+            if response["action"] == "list_nodes":
+                if response["filter"]:
+                    nodes = self.config._getallnodes(response["filter"])
+                else:
+                    nodes = self.config._getallnodes()
+                list = "\n".join(nodes)
+                response = f"```{list}\n```"
+            else:
+                yaml_data = yaml.dump(response["task"])
+                confirmresponse = f"I'm going to run the following task:\n```{yaml_data}```\nPlease confirm"
+                while True:
+                    mdprint(Markdown(f"""**Chatbot**:\n{confirmresponse}"""))
+                    questions = [
+                            inquirer.Text('message', message="User", validate=self._ai_validation),
+                        ]
+                    answers = inquirer.prompt(questions)
+                    if answers == None:
+                        exit(7)
+                    confirmation = self.myai.confirm(answers["message"])
+                    if isinstance(confirmation, bool):
+                        if not confirmation:
+                            response = "Request cancelled"
+                        else:
+                            nodes = self.connnodes(self.config.getitems(response["nodes"]), config = self.config)
+                            if response["action"] == "run":
+                                output = nodes.run(**response["args"])
+                                response = ""
+                            elif response["action"] == "test":
+                                result = nodes.test(**response["args"])
+                                yaml_result = yaml.dump(result,default_flow_style=False, indent=4)
+                                output = nodes.output
+                                response = f"This is the result for your test:\n```\n{yaml_result}\n```"
+                            for k,v in output.items():
+                                response += f"\n***{k}***:\n```\n{v}\n```\n"
+                        break
+            return response, history
+
     def _func_api(self, args):
         if args.command == "stop" or args.command == "restart":
             args.data = stop_api()
         if args.command == "start" or args.command == "restart":
             if args.data:
                 start_api(args.data)
             else:
@@ -551,76 +682,75 @@
         try:
             with open(args.data[0]) as file:
                 scripts = yaml.load(file, Loader=yaml.FullLoader)
         except:
             print("failed reading file {}".format(args.data[0]))
             exit(10)
         for script in scripts["tasks"]:
-            args = {}
-            try:
-                action = script["action"]
-                nodelist = script["nodes"]
-                args["commands"] = script["commands"]
-                output = script["output"]
-                if action == "test":
-                    args["expected"] = script["expected"]
-            except KeyError as e:
-                print("'{}' is mandatory".format(e.args[0]))
-                exit(11)
-            nodes = self.connnodes(self.config.getitems(nodelist), config = self.config)
-            stdout = False
-            if output is None:
-                pass
-            elif output == "stdout":
-                stdout = True
-            elif isinstance(output, str) and action == "run":
-                args["folder"] = output
-            try:
-                args["vars"] = script["variables"]
-            except:
-                pass
-            try:
-                options = script["options"]
-                thisoptions = {k: v for k, v in options.items() if k in ["prompt", "parallel", "timeout"]}
-                args.update(thisoptions)
-            except:
-                options = None
-            size = str(os.get_terminal_size())
-            p = re.search(r'.*columns=([0-9]+)', size)
-            columns = int(p.group(1))
-            if action == "run":
-                nodes.run(**args)
-                print(script["name"].upper() + "-" * (columns - len(script["name"])))
-                for i in nodes.status.keys():
-                    print("   " + i + " " + "-" * (columns - len(i) - 13) + (" PASS(0)" if nodes.status[i] == 0 else " FAIL({})".format(nodes.status[i])))
-                    if stdout:
-                        for line in nodes.output[i].splitlines():
-                            print("      " + line)
-            elif action == "test":
-                nodes.test(**args)
-                print(script["name"].upper() + "-" * (columns - len(script["name"])))
-                for i in nodes.status.keys():
-                    print("   " + i + " " + "-" * (columns - len(i) - 13) + (" PASS(0)" if nodes.status[i] == 0 else " FAIL({})".format(nodes.status[i])))
+            self._cli_run(script)
+
+
+    def _cli_run(self, script):
+        args = {}
+        try:
+            action = script["action"]
+            nodelist = script["nodes"]
+            args["commands"] = script["commands"]
+            output = script["output"]
+            if action == "test":
+                args["expected"] = script["expected"]
+        except KeyError as e:
+            print("'{}' is mandatory".format(e.args[0]))
+            exit(11)
+        nodes = self.connnodes(self.config.getitems(nodelist), config = self.config)
+        stdout = False
+        if output is None:
+            pass
+        elif output == "stdout":
+            stdout = True
+        elif isinstance(output, str) and action == "run":
+            args["folder"] = output
+        if "variables" in script:
+            args["vars"] = script["variables"]
+        if "vars" in script:
+            args["vars"] = script["vars"]
+        try:
+            options = script["options"]
+            thisoptions = {k: v for k, v in options.items() if k in ["prompt", "parallel", "timeout"]}
+            args.update(thisoptions)
+        except:
+            options = None
+        size = str(os.get_terminal_size())
+        p = re.search(r'.*columns=([0-9]+)', size)
+        columns = int(p.group(1))
+        if action == "run":
+            nodes.run(**args)
+            print(script["name"].upper() + "-" * (columns - len(script["name"])))
+            for i in nodes.status.keys():
+                print("   " + i + " " + "-" * (columns - len(i) - 13) + (" PASS(0)" if nodes.status[i] == 0 else " FAIL({})".format(nodes.status[i])))
+                if stdout:
+                    for line in nodes.output[i].splitlines():
+                        print("      " + line)
+        elif action == "test":
+            nodes.test(**args)
+            print(script["name"].upper() + "-" * (columns - len(script["name"])))
+            for i in nodes.status.keys():
+                print("   " + i + " " + "-" * (columns - len(i) - 13) + (" PASS(0)" if nodes.status[i] == 0 else " FAIL({})".format(nodes.status[i])))
+                if nodes.status[i] == 0:
+                    max_length = max(len(s) for s in nodes.result[i].keys())
+                    for k,v in nodes.result[i].items():
+                        print("     TEST for '{}'".format(k) +  " "*(max_length - len(k) + 1) + "--> " + str(v).upper())
+                if stdout:
                     if nodes.status[i] == 0:
-                        try:
-                            myexpected = args["expected"].format(**args["vars"][i])
-                        except:
-                            try:
-                                myexpected = args["expected"].format(**args["vars"]["__global__"])
-                            except:
-                                myexpected = args["expected"]
-                        print("     TEST for '{}' --> ".format(myexpected) + str(nodes.result[i]).upper())
-                    if stdout:
-                        if nodes.status[i] == 0:
-                            print("     " + "-" * (len(myexpected) + 16 + len(str(nodes.result[i]))))
-                        for line in nodes.output[i].splitlines():
-                            print("      " + line)
-            else:
-                print("Wrong action '{}'".format(action))
-                exit(13)
+                        print("     " + "-" * (max_length + 21))
+                    for line in nodes.output[i].splitlines():
+                        print("      " + line)
+        else:
+            print("Wrong action '{}'".format(action))
+            exit(13)
 
     def _choose(self, list, name, action):
         #Generates an inquirer list to pick
         if FzfPrompt and self.fzf:
             fzf = FzfPrompt(executable_path="fzf-tmux")
             if not self.case:
                 fzf = FzfPrompt(executable_path="fzf-tmux -i")
@@ -944,36 +1074,45 @@
     def _help(self, type):
         #Store text for help and other commands
         if type == "node":
             return "node[@subfolder][@folder]\nConnect to specific node or show all matching nodes\n[@subfolder][@folder]\nShow all available connections globaly or in specified path"
         if type == "usage":
             return "conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]\n       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ..."
         if type == "end":
-            return "Commands:\n  profile        Manage profiles\n  move (mv)      Move node\n  copy (cp)      Copy node\n  list (ls)      List profiles, nodes or folders\n  bulk           Add nodes in bulk\n  run            Run scripts or commands on nodes\n  config         Manage app config\n  api            Start and stop connpy api"
+            return "Commands:\n  profile        Manage profiles\n  move (mv)      Move node\n  copy (cp)      Copy node\n  list (ls)      List profiles, nodes or folders\n  bulk           Add nodes in bulk\n  run            Run scripts or commands on nodes\n  config         Manage app config\n  api            Start and stop connpy api\n  ai             Make request to an AI"
         if type == "bashcompletion":
             return '''
 #Here starts bash completion for conn
 _conn()
 {
-        strings="$(connpy-completion-helper ${#COMP_WORDS[@]} ${COMP_WORDS[@]})"
-        COMPREPLY=($(compgen -W "$strings" -- "${COMP_WORDS[-1]}"))
+        mapfile -t strings < <(connpy-completion-helper "bash" "${#COMP_WORDS[@]}" "${COMP_WORDS[@]}")
+        local IFS=$'\\t\\n'
+        COMPREPLY=($(compgen -W "$(printf '%s' "${strings[@]}")" -- "${COMP_WORDS[-1]}"))
 }
-complete -o nosort -F _conn conn
-complete -o nosort -F _conn connpy
+
+complete -o nospace -o nosort -F _conn conn
+complete -o nospace -o nosort -F _conn connpy
 #Here ends bash completion for conn
         '''
         if type == "zshcompletion":
             return '''
-
 #Here starts zsh completion for conn
 autoload -U compinit && compinit
 _conn()
 {
-    strings=($(connpy-completion-helper ${#words} $words))
-    compadd "$@" -- `echo $strings`
+    strings=($(connpy-completion-helper "zsh" ${#words} $words))
+    for string in "${strings[@]}"; do
+        if [[ "${string}" =~ .*/$ ]]; then
+            # If the string ends with a '/', do not append a space
+            compadd -S '' -- "$string"
+        else
+            # If the string does not end with a '/', append a space
+            compadd -S ' ' -- "$string"
+        fi
+    done
 }
 compdef _conn conn
 compdef _conn connpy
 #Here ends zsh completion for conn
             '''
         if type == "run":
             return "node[@subfolder][@folder] commmand to run\nRun the specific command on the node and print output\n/path/to/file.yaml\nUse a yaml file to run an automation script"
```

### Comparing `connpy-3.2.8/connpy/core.py` & `connpy-3.3.0/connpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,20 +137,20 @@
 
     def _logclean(self, logfile, var = False):
         #Remove special ascii characters and other stuff from logfile.
         if var == False:
             t = open(logfile, "r").read()
         else:
             t = logfile
+        while t.find("\b") != -1:
+            t = re.sub('[^\b]\b', '', t)
         t = t.replace("\n","",1)
         t = t.replace("\a","")
         t = t.replace('\n\n', '\n')
         t = re.sub(r'.\[K', '', t)
-        while t.find("\b") != -1:
-            t = re.sub('[^\b]\b', '', t)
         ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/ ]*[@-~])')
         t = ansi_escape.sub('', t)
         t = t.lstrip(" \n\r")
         t = t.replace("\r","")
         t = t.replace("\x0E","")
         t = t.replace("\x0F","")
         if var == False:
@@ -345,14 +345,16 @@
         if connect == True:
             if "prompt" in self.tags:
                 prompt = self.tags["prompt"]
             expects = [prompt, pexpect.EOF, pexpect.TIMEOUT]
             output = ''
             if not isinstance(commands, list):
                 commands = [commands]
+            if not isinstance(expected, list):
+                expected = [expected]
             if "screen_length_command" in self.tags:
                 commands.insert(0, self.tags["screen_length_command"])
             self.mylog = io.BytesIO()
             self.child.logfile_read = self.mylog
             for c in commands:
                 if vars is not None:
                     c = c.format(**vars)
@@ -362,26 +364,33 @@
                     break
             if not result == 2:
                 result = self.child.expect(expects, timeout = timeout)
             self.child.close()
             output = self._logclean(self.mylog.getvalue().decode(), True)
             self.output = output
             if result in [0, 1]:
-                lastcommand = commands[-1]
-                if vars is not None:
-                    expected = expected.format(**vars)
-                    lastcommand = lastcommand.format(**vars)
-                last_command_index = output.rfind(lastcommand)
-                cleaned_output = output[last_command_index + len(lastcommand):].strip()
-                if expected in cleaned_output:
-                    self.result = True
-                else:
-                    self.result = False
+                # lastcommand = commands[-1]
+                # if vars is not None:
+                    # lastcommand = lastcommand.format(**vars)
+                # last_command_index = output.rfind(lastcommand)
+                # cleaned_output = output[last_command_index + len(lastcommand):].strip()
+                self.result = {}
+                for e in expected:
+                    if vars is not None:
+                        e = e.format(**vars)
+                    updatedprompt = re.sub(r'(?<!\\)\$', '', prompt)
+                    newpattern = f".*({updatedprompt}).*{e}.*"
+                    cleaned_output = output
+                    cleaned_output = re.sub(newpattern, '', cleaned_output)
+                    if e in cleaned_output:
+                        self.result[e] = True
+                    else:
+                        self.result[e]= False
                 self.status = 0
-                return False
+                return self.result
             if result == 2:
                 self.result = None
                 self.status = 2
                 return output
         else:
             self.result = None
             self.output = connect
```

### Comparing `connpy-3.2.8/connpy.egg-info/PKG-INFO` & `connpy-3.3.0/connpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.8
+Version: 3.3.0
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -154,14 +154,15 @@
   move (mv)      Move node
   copy (cp)      Copy node
   list (ls)      List profiles, nodes or folders
   bulk           Add nodes in bulk
   run            Run scripts or commands on nodes
   config         Manage app config
   api            Start and stop connpy api
+  ai             Make request to an AI
 ```
 
 ### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
```

### Comparing `connpy-3.2.8/setup.cfg` & `connpy-3.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 	inquirer
 	pexpect
 	pycryptodome
 	Flask
 	waitress
 	PyYAML
 	openai
+	rich
 
 [options.extras_require]
 fuzzysearch = pyfzf
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
```

