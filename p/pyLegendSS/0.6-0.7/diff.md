# Comparing `tmp/pyLegendSS-0.6.tar.gz` & `tmp/pyLegendSS-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.6.tar", last modified: Wed Jul 12 18:23:08 2023, max compression
+gzip compressed data, was "pyLegendSS-0.7.tar", last modified: Wed Jul 12 18:28:24 2023, max compression
```

## Comparing `pyLegendSS-0.6.tar` & `pyLegendSS-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:23:08.657229 pyLegendSS-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 18:22:51.000000 pyLegendSS-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/pyLegendSS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:23:08.657229 pyLegendSS-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 18:22:51.000000 pyLegendSS-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.458551 pyLegendSS-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.454551 pyLegendSS-0.7/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:28:24.458551 pyLegendSS-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 18:28:11.000000 pyLegendSS-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.458551 pyLegendSS-0.7/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:28:24.458551 pyLegendSS-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 18:28:11.000000 pyLegendSS-0.7/setup.py
```

### Comparing `pyLegendSS-0.6/LICENSE` & `pyLegendSS-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.6/LegendSS/Data.py` & `pyLegendSS-0.7/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.6/LegendSS/generate.py` & `pyLegendSS-0.7/LegendSS/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             await client.send_message(
                 "me",
                 "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
                     "Pyrogram", string_session
                 ),
             )
     try:
-        client.join_chat("@LegendBot_OP")
+        await client.join_chat("@LegendBot_OP")
     except BaseException:
         pass
     await client.disconnect()
     await phone_code_msg.reply(
         "Successfully String  Session Has Been Generated {} \n\nPlease check your saved messages!".format(
             "TELETHON" if telethon else "PYROGRAM"
         ),
```

### Comparing `pyLegendSS-0.6/PKG-INFO` & `pyLegendSS-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.6
+Version: 0.7
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.6/pyLegendSS.egg-info/PKG-INFO` & `pyLegendSS-0.7/pyLegendSS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.6
+Version: 0.7
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.6/setup.py` & `pyLegendSS-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.6",
+    version="0.7",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

