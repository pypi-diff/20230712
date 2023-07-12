# Comparing `tmp/easycompletion-0.1.7.tar.gz` & `tmp/easycompletion-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.7.tar", last modified: Wed Jul 12 02:51:40 2023, max compression
+gzip compressed data, was "easycompletion-0.1.8.tar", last modified: Wed Jul 12 20:41:04 2023, max compression
```

## Comparing `easycompletion-0.1.7.tar` & `easycompletion-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.700489 easycompletion-0.1.7/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.7/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:51:40.700332 easycompletion-0.1.7/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     5917 2023-07-10 21:51:01.000000 easycompletion-0.1.7/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.699358 easycompletion-0.1.7/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-12 02:51:36.000000 easycompletion-0.1.7/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.7/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    13812 2023-07-10 21:51:51.000000 easycompletion-0.1.7/easycompletion/model.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.7/easycompletion/prompt.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.7/easycompletion/test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.700119 easycompletion-0.1.7/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-12 02:51:40.700537 easycompletion-0.1.7/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1415 2023-07-12 02:51:36.000000 easycompletion-0.1.7/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 20:41:04.110138 easycompletion-0.1.8/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.8/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 20:41:04.109969 easycompletion-0.1.8/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5917 2023-07-10 21:51:01.000000 easycompletion-0.1.8/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 20:41:04.107988 easycompletion-0.1.8/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-12 20:41:00.000000 easycompletion-0.1.8/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.8/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    13934 2023-07-12 20:36:53.000000 easycompletion-0.1.8/easycompletion/model.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5231 2023-07-12 20:37:03.000000 easycompletion-0.1.8/easycompletion/prompt.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 20:41:04.109698 easycompletion-0.1.8/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 20:41:04.000000 easycompletion-0.1.8/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      319 2023-07-12 20:41:04.000000 easycompletion-0.1.8/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-12 20:41:04.000000 easycompletion-0.1.8/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-12 20:41:04.000000 easycompletion-0.1.8/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-12 20:41:04.000000 easycompletion-0.1.8/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-12 20:41:04.110213 easycompletion-0.1.8/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1415 2023-07-12 20:41:00.000000 easycompletion-0.1.8/setup.py
```

### Comparing `easycompletion-0.1.7/LICENSE` & `easycompletion-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.7/PKG-INFO` & `easycompletion-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.7
+Version: 0.1.8
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.7/README.md` & `easycompletion-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.7/easycompletion/__init__.py` & `easycompletion-0.1.8/easycompletion/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 easycompletion
 
 Leveraging conversational AI for bicameral decision making.
 """
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/easycompletion"
 
 from .model import (
     openai_function_call,
     openai_text_call,
     compose_function,
```

### Comparing `easycompletion-0.1.7/easycompletion/model.py` & `easycompletion-0.1.8/easycompletion/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 import re
 import json
 import ast
 
 from dotenv import load_dotenv
 
 # Load environment variables from .env file
-load_dotenv()  
+load_dotenv()
 
-from constants import (
+from .constants import (
     default_text_model,
     long_text_model,
     openai_api_key,
     default_chunk_length,
 )
 
-from prompt import count_tokens
+from .prompt import count_tokens
 
 # Set the OpenAI API key
 openai.api_key = openai_api_key
 
 
 def parse_arguments(arguments):
     """
     Parses arguments that are expected to be either a JSON string, dictionary, or a list.
 
     Parameters:
         arguments (str or dict or list): Arguments in string or dictionary or list format.
-    
+
     Returns:
         A dictionary or list of arguments if arguments are valid, None otherwise.
-        
+
     Usage:
         arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
     """
     try:
         # Handle string inputs, remove any ellipsis from the string
         if isinstance(arguments, str):
             arguments = re.sub(r"\.\.\.|\…", "", arguments)
@@ -67,15 +67,15 @@
     Parameters:
         response (dict): The response from OpenAI API.
         functions (list): A list of function definitions.
         function_call (dict or str): The expected function call.
 
     Returns:
         True if function call matches with the response, False otherwise.
-        
+
     Usage:
         isValid = validate_functions(response, functions, function_call)
     """
     # Extract the function call from the response
     response_function_call = response["choices"][0]["message"]["function_call"]
 
     # If function_call is not "auto" and the name does not match with the response, return False
@@ -148,15 +148,21 @@
             "type": "object",
             "properties": properties,
             "required": required_properties,
         },
     }
 
 
-def openai_text_call(text, model_failure_retries=5, model=None, chunk_length=default_chunk_length, api_key=None):
+def openai_text_call(
+    text,
+    model_failure_retries=5,
+    model=None,
+    chunk_length=default_chunk_length,
+    api_key=None,
+):
     """
     Function for sending text to the OpenAI API and returning a text response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
         model (str, optional): The model to use. Default is the default_text_model defined in constants.py.
@@ -165,15 +171,15 @@
 
     Returns:
         str: The response content from the model.
 
     Example:
         >>> openai_text_call("Hello, how are you?", model_failure_retries=3, model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key')
     """
-    
+
     # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
     # Use the default model if no model is specified
     if model == None:
         model = default_text_model
@@ -205,15 +211,19 @@
     response = None
     for i in range(model_failure_retries):
         response = try_request()
         if response:
             break
 
     # If response is not valid, print an error message and return None
-    if response is None or response["choices"] is None or response["choices"][0] is None:
+    if (
+        response is None
+        or response["choices"] is None
+        or response["choices"][0] is None
+    ):
         print("Error: Could not get a successful response from OpenAI API")
         return None
 
     # Extract content from the response
     response_data = response["choices"][0]["message"]
     content = response_data["content"]
 
@@ -242,15 +252,15 @@
         function_call (str | dict | None): 'auto' to let the model decide, or a function name or a dictionary containing the function name (default is "auto").
         function_failure_retries (int): Number of times to retry the request if the function call is invalid (default is 10).
         chunk_length (int): The length of each chunk to be processed.
         model (str | None): The model to use (default is the default_text_model, i.e. gpt-3.5-turbo).
         api_key (str | None): If you'd like to pass in a key to override the environment variable OPENAI_API_KEY.
 
     Returns:
-        dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing 
+        dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing
         "text" (response from the model), "function_name" (name of the function called), "arguments" (arguments for the function), "error" (None).
 
     Example:
         >>> function = {'name': 'function1', 'parameters': {'param1': 'value1'}}
         >>> openai_function_call("Call the function.", function)
     """
 
@@ -269,15 +279,17 @@
             and "name" in functions
             and "parameters" in functions
         ):
             # A single function is provided as a dictionary, convert it to a list
             functions = [functions]
         else:
             # Functions must be either a list of dictionaries or a single dictionary
-            return {"error": "functions must be a list of functions or a single function"}
+            return {
+                "error": "functions must be a list of functions or a single function"
+            }
 
     # Set the function call to the name of the function if only one function is provided
     # If there are multiple functions, use "auto"
     if function_call is None:
         function_call = functions[0]["name"] if len(functions) == 1 else "auto"
 
     # Make sure text is provided
@@ -285,15 +297,17 @@
         return {"error": "text is required"}
 
     # Check if the function call is valid
     if function_call != "auto":
         if isinstance(function_call, str):
             function_call = {"name": function_call}
         elif "name" not in function_call:
-            return {"error": "function_call had an invalid name. Should be a string of the function name or an object with a name property"}
+            return {
+                "error": "function_call had an invalid name. Should be a string of the function name or an object with a name property"
+            }
 
     # Use the default text model if no model is specified
     if model is None:
         model = default_text_model
 
     # Count the number of tokens in the message
     message_tokens = count_tokens(text, model=model)
@@ -342,15 +356,19 @@
             response = try_request()
             if response:
                 break
         if functions is None or validate_functions(response, functions, function_call):
             break
 
     # Check if we have a valid response from OpenAI API
-    if response is None or not response.get("choices") or response["choices"][0] is None:
+    if (
+        response is None
+        or not response.get("choices")
+        or response["choices"][0] is None
+    ):
         error = "Could not get a successful response from OpenAI API"
         print(error)
         return {"error": error}
 
     # Extracting the content and function call response from API response
     response_data = response["choices"][0]["message"]
     content = response_data["content"]
```

### Comparing `easycompletion-0.1.7/easycompletion/prompt.py` & `easycompletion-0.1.8/easycompletion/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import tiktoken
 
-from easycompletion.constants import (
+from .constants import (
     default_text_model,
     default_chunk_length,
 )
 
 
 def trim_prompt(
     text, max_tokens=default_chunk_length, model=default_text_model, preserve_top=True
```

### Comparing `easycompletion-0.1.7/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.1.8/easycompletion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.7
+Version: 0.1.8
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.7/setup.py` & `easycompletion-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.1.7',
+    version='0.1.8',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/lalalune/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

