# Comparing `tmp/streamlithelpers-0.1.2.tar.gz` & `tmp/streamlithelpers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlithelpers-0.1.2.tar", last modified: Wed Jul 12 13:38:07 2023, max compression
+gzip compressed data, was "streamlithelpers-0.1.3.tar", last modified: Wed Jul 12 15:40:12 2023, max compression
```

## Comparing `streamlithelpers-0.1.2.tar` & `streamlithelpers-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.439475 streamlithelpers-0.1.2/
--rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.2/LICENSE.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 13:38:07.439591 streamlithelpers-0.1.2/PKG-INFO
--rw-r--r--   0 adr27     (1415) adr27     (1415)     2804 2023-07-12 13:37:07.000000 streamlithelpers-0.1.2/README.md
--rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 13:38:07.440012 streamlithelpers-0.1.2/setup.cfg
--rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 13:35:00.000000 streamlithelpers-0.1.2/setup.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.438549 streamlithelpers-0.1.2/streamlithelpers/
--rw-r--r--   0 adr27     (1415) adr27     (1415)      220 2023-07-12 10:51:30.000000 streamlithelpers-0.1.2/streamlithelpers/__init__.py
--rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.2/streamlithelpers/streamlit_helpers.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.439298 streamlithelpers-0.1.2/streamlithelpers.egg-info/
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/PKG-INFO
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/SOURCES.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/dependency_links.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/requires.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/top_level.txt
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 15:40:12.314512 streamlithelpers-0.1.3/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.3/LICENSE.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 15:40:12.314581 streamlithelpers-0.1.3/PKG-INFO
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)     3022 2023-07-12 15:39:10.000000 streamlithelpers-0.1.3/README.md
+-rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 15:40:12.314839 streamlithelpers-0.1.3/setup.cfg
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 15:38:53.000000 streamlithelpers-0.1.3/setup.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 15:40:12.313620 streamlithelpers-0.1.3/streamlithelpers/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      232 2023-07-12 15:37:55.000000 streamlithelpers-0.1.3/streamlithelpers/__init__.py
+-rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.3/streamlithelpers/streamlit_helpers.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 15:40:12.314409 streamlithelpers-0.1.3/streamlithelpers.egg-info/
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 15:40:12.000000 streamlithelpers-0.1.3/streamlithelpers.egg-info/PKG-INFO
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 15:40:12.000000 streamlithelpers-0.1.3/streamlithelpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 15:40:12.000000 streamlithelpers-0.1.3/streamlithelpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 15:40:12.000000 streamlithelpers-0.1.3/streamlithelpers.egg-info/requires.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 15:40:12.000000 streamlithelpers-0.1.3/streamlithelpers.egg-info/top_level.txt
```

### Comparing `streamlithelpers-0.1.2/LICENSE.txt` & `streamlithelpers-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.2/PKG-INFO` & `streamlithelpers-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.3.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamlithelpers-0.1.2/README.md` & `streamlithelpers-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Install
+
+`pip install streamlithelpers`
+
 # Session state helpers
 
 ## Basic
 
 Helper functions like `set_state(key, value)`, `get_state(key)` and `init_state(key, value)` 
 avoid repetitive if-statement and None checking patterns.
 
@@ -38,14 +42,17 @@
 ```
 
 Here the last `10` results of calls to `result()` are stored, and can be acquired via `result.history()`.
 And `cleanup(result.get())` is run first when `result.clear()` is called if `result.get()` is not None.
 
 # Widget helpers
 
+Some functions are provided which display one or more streamlit widgets to support common workflows.
+They all start with `st_`.
+
 ## Downloading
 Currently, if you make a download button with Streamlit, the contents must already be in memory, 
 so below are some helpers for dealing with that.
 
 `st_dataframe_with_download()` : displays a st.dataframe() widget with an accompanying download 
 button which downloads a CSV of the dataframe - the button is primed with the full contents of the
 CSV for you. The dataframe to string conversion is cached for an hour.
@@ -56,12 +63,12 @@
 function relies on a library function that writes to file.
 
 ## Display
 
 `st_status(message, type)` : displays a status message in a colour appropriate to a specified type (error/warn/info/success)
 with an appropriate icon.
 
-`st_source_code(obj)` : uses a python language `st.code` (which accepts a String of code only) 
-widget to display the source code of the specified object using Pythons `inspect.getsource()`.
+`st_source_code(obj)` : the streamlit widget `st.code()` will display only a String literal representing some code. This function
+takes any Python object, finds its source code via Python's `inspect.getsource()` and displays that code.
 
 `st_code_editor` : display a code editor backed by `st_ace` library, but doing some annoying defaults,
-like making sure initial state is empty string not `None`, and that state is initialised.
+like making sure initial state is empty string not `None`, and that state is initialised.
```

### Comparing `streamlithelpers-0.1.2/setup.py` & `streamlithelpers-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='streamlithelpers',
     packages=['streamlithelpers'],
-    version='0.1.2',
+    version='0.1.3',
     license='MIT',
     description='Simple utilities to help streamlit app development',
     author='Andrew Robertson',
     author_email='',
     url='https://github.com/andehr/streamlit-helpers',
-    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz',
+    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.3.tar.gz',
     keywords=['streamlit', 'utility'],
     install_requires=[
         'pandas',
         'streamlit',
         'streamlit-ace'
     ],
     classifiers=[
```

### Comparing `streamlithelpers-0.1.2/streamlithelpers/streamlit_helpers.py` & `streamlithelpers-0.1.3/streamlithelpers/streamlit_helpers.py`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.2/streamlithelpers.egg-info/PKG-INFO` & `streamlithelpers-0.1.3/streamlithelpers.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.3.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

