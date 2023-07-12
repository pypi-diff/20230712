# Comparing `tmp/grassmanntn-1.2.0.tar.gz` & `tmp/grassmanntn-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.2.0.tar", last modified: Tue Jul 11 05:16:53 2023, max compression
+gzip compressed data, was "grassmanntn-1.2.1.tar", last modified: Wed Jul 12 07:39:46 2023, max compression
```

## Comparing `grassmanntn-1.2.0.tar` & `grassmanntn-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.2.0/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.2.0/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   108809 2023-07-11 05:12:08.000000 grassmanntn-1.2.0/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.2.0/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.2.0/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.2.0/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-11 05:13:36.000000 grassmanntn-1.2.0/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.2.1/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.2.1/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109008 2023-07-12 07:37:50.000000 grassmanntn-1.2.1/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.2.1/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.2.1/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.2.1/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-12 07:39:27.000000 grassmanntn-1.2.1/setup.py
```

### Comparing `grassmanntn-1.2.0/LICENSE.txt` & `grassmanntn-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.0/PKG-INFO` & `grassmanntn-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.2.0
+Version: 1.2.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.2.0/README.md` & `grassmanntn-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.0/grassmanntn/__init__.py` & `grassmanntn-1.2.1/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,15 +963,14 @@
 
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #              Step 0: Input processing
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     # remove spaces ---------------------------------------------------------------------------------
     instruction_string = args[0].replace(" ","")
-
     instruction_string = denumerate(instruction_string)
 
     has_output = instruction_string.count("->") > 0
     if instruction_string.count("->") > 1 :
         error("Error[einsum]: Only one arrow is allowed in the input string!")
 
     if has_output:
@@ -1622,14 +1621,15 @@
     process_name = "join_legs"
     process_length = 6
     process_color="green"
     step = 1
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
 
+    string_inp = string_inp.replace(" ","")
     string_inp = denumerate(string_inp)
 
     intermediate_stat = make_tuple(intermediate_stat)
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     # Always output the parity-preserving encoder
     #===============================================================================#
@@ -1732,14 +1732,15 @@
     process_name = "split_legs"
     process_length = 6
     process_color="green"
     step = 1
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
 
+    string_inp = string_inp.replace(" ","")
     string_inp = denumerate(string_inp)
 
     intermediate_stat = make_tuple(intermediate_stat)
     final_stat = make_tuple(final_stat)
     final_shape = make_tuple(final_shape)
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
@@ -2141,14 +2142,15 @@
     s00 = time.time()
     progress_space()
 
     global skip_power_of_two_check
 
     # the string is of the form aaaa|bbb
 
+    string = string.replace(" ","")
     string = denumerate(string)
 
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
@@ -2485,14 +2487,15 @@
     s00 = time.time()
     progress_space()
 
     global skip_power_of_two_check
 
     # the string is of the form aaaa|bbb
 
+    string = string.replace(" ","")
     string = denumerate(string)
 
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
@@ -2716,14 +2719,15 @@
     process_name = "hconjugate"
     process_length = 6
     process_color="yellow"
     step = 1
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
 
+    string = string.replace(" ","")
     string = denumerate(string)
     
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
         string = string.replace(")(","|")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[hconjugate]: Parentheses don't match")
```

### Comparing `grassmanntn-1.2.0/grassmanntn/example.py` & `grassmanntn-1.2.1/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.0/grassmanntn/gauge2d.py` & `grassmanntn-1.2.1/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.0/grassmanntn/param.py` & `grassmanntn-1.2.1/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.0/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.2.1/grassmanntn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.2.0
+Version: 1.2.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.2.0/setup.py` & `grassmanntn-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.2.0',      # Start with a small number and increase it with every change you make
+  version = '1.2.1',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

