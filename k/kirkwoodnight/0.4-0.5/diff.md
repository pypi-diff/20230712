# Comparing `tmp/kirkwoodnight-0.4.tar.gz` & `tmp/kirkwoodnight-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-0.4.tar", last modified: Wed Jul 12 20:27:13 2023, max compression
+gzip compressed data, was "kirkwoodnight-0.5.tar", last modified: Wed Jul 12 20:43:16 2023, max compression
```

## Comparing `kirkwoodnight-0.4.tar` & `kirkwoodnight-0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:27:13.784699 kirkwoodnight-0.4/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.4/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:27:13.784193 kirkwoodnight-0.4/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.4/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:27:13.781122 kirkwoodnight-0.4/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.4/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    18544 2023-07-12 20:26:31.000000 kirkwoodnight-0.4/kirkwoodnight/kirkwoodnight.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:27:13.783514 kirkwoodnight-0.4/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      311 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       67 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 20:27:13.000000 kirkwoodnight-0.4/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 20:27:13.784874 kirkwoodnight-0.4/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1090 2023-07-12 20:26:34.000000 kirkwoodnight-0.4/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:43:16.138757 kirkwoodnight-0.5/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.5/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:43:16.138221 kirkwoodnight-0.5/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.5/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:43:16.134715 kirkwoodnight-0.5/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.5/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2720 2023-07-12 20:39:59.000000 kirkwoodnight-0.5/kirkwoodnight/command_line.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 20:40:52.000000 kirkwoodnight-0.5/kirkwoodnight/kirkwoodnight.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:43:16.137489 kirkwoodnight-0.5/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      341 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 20:43:16.000000 kirkwoodnight-0.5/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 20:43:16.138967 kirkwoodnight-0.5/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-12 20:40:55.000000 kirkwoodnight-0.5/setup.py
```

### Comparing `kirkwoodnight-0.4/LICENSE.txt` & `kirkwoodnight-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.4/PKG-INFO` & `kirkwoodnight-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.4
+Version: 0.5
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.4/README.md` & `kirkwoodnight-0.5/README.md`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.4/kirkwoodnight/kirkwoodnight.py` & `kirkwoodnight-0.5/kirkwoodnight/kirkwoodnight.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# version 0.4
+# version 0.5
 
 # basic imports
 import os
 import numpy as np
 import pandas as pd
 
 # date/time functionality
@@ -335,46 +335,8 @@
         f.write("Time Partition (hrs): " + str(dt) + "\n" + "\n")
         f.write(str(len(selected_targets)) + " objects selected for observation: \n")
         for obj in selected_names:
             f.write(obj + "\n")
 
     print("Log file saved in " + subdir)
 
-    return target_df, time_df
-
-def_l = [str(date.today()), str(datetime.datetime.now().time()), 4, 10, 80, 5, None, None, None, 0.5]
-
-message_list = ["Which date would you like to observe on? (Enter as YYYY-MM-DD, default is today):",
-                "What time would you like to start your run? (Enter in military time as HH:MM, default is current local time):",
-                "How many hours would you like to observe for? (default is 4)",
-                "Would you like to change Kirkwood's minimum altitude limit (in degrees)? (Type value if desired, otherwise hit ENTER. Default is 10.)",
-                "Would you like to change Kirkwood's maximum altitude limit (in degrees)? (Type value if desired, otherwise hit ENTER. Default is 80.)",
-                "Would you like to change the minimum mandated distance (in degrees) from the Moon? (Type value if desired, otherwise hit ENTER. Default is 5.)",
-                "Would you like to specify a maximum allowed airmass? (Type value if desired, otherwise hit ENTER. Default is None.)",
-                "Would you like to specify a desired level of darkness for the night? (If desired, type 'civ' or 'naut' or 'astro' to respectively signify civil, nautical, or astronomical twilight. Otherwise hit ENTER. Default is None.)",
-                "Would you like to specify a maximum brightness level for the moon? (If desired, type 'grey' or 'dark', otherwise hit ENTER. Default is None.)",
-                "How often do you want to re-check for observability (in hours)? (type value if desired, otherwise hit ENTER. Default is 0.5, which creates a schedule in 30 minute intervals.)"]
-
-def main():   
-# print interactive prompts in terminal
-    print()
-    print("------------------------------------------------------------------------")
-    print("KIRKWOOD OBSERVING PLANNER")
-    print("CREATED BY: ARMAAN GOYAL, BRANDON RADZOM, JESSICA RANSHAW, XIAN-YU WANG")
-    print("LAST UPDATED ON 2023-07-14")
-    print("ACCESSED ON %s"%str(datetime.datetime.now()))
-    print("------------------------------------------------------------------------")
-
-    print("\n For best results, maximize terminal to fullscreen. \n")
-
-    for i in range(len(def_l)):
-        print(message_list[i])
-        var = input()
-        if var != "":
-            if i in [2, 3, 4, 5, 6, 9]:
-                var = float(var)
-            def_l[i] = var
-
-    print("Generating Info and Schedules...")
-
-    sim_kirkwood_obs(date = def_l[0], start_time = def_l[1], duration = def_l[2],
-                        alt_lim = (def_l[3], def_l[4]), moon_sep = def_l[5], max_airmass = def_l[6], night_type = def_l[7], moon_illum = def_l[8], dt = def_l[9])
+    return target_df, time_df
```

### Comparing `kirkwoodnight-0.4/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-0.5/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.4
+Version: 0.5
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.4/setup.py` & `kirkwoodnight-0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
@@ -22,15 +22,15 @@
     classifiers=[
         "License :: OSI Approved :: MIT License"
     ],
 
     # Specify console scripts
     entry_points={
         'console_scripts': [
-            'kirkwoodnight = kirkwoodnight.kirkwoodnight:main',
+            'kirkwoodnight = kirkwoodnight.command_line:main',
         ],
     },
 
     # Include additional files into the package
     package_data={'': ['obj_list.csv']},
 
     install_requires= get_requires(),
```

