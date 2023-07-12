# Comparing `tmp/py-helper-mod-0.0.38.tar.gz` & `tmp/py-helper-mod-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.38.tar", last modified: Tue Jul 11 19:52:54 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.39.tar", last modified: Wed Jul 12 16:44:46 2023, max compression
```

## Comparing `py-helper-mod-0.0.38.tar` & `py-helper-mod-0.0.39.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89040 2023-07-11 19:52:17.000000 py-helper-mod-0.0.38/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.38/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89230 2023-07-12 16:40:01.000000 py-helper-mod-0.0.39/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-12 16:44:46.393261 py-helper-mod-0.0.39/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.39/setup.py
```

### Comparing `py-helper-mod-0.0.38/LICENSE` & `py-helper-mod-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.38/PKG-INFO` & `py-helper-mod-0.0.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.38
+Version: 0.0.39
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.38/py_helper.py` & `py-helper-mod-0.0.39/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,26 +1181,26 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,37)
+VERSION=(0,0,38)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
 
 # Debug/Breakpoint Flags
-DebugEnabled = None		# Dictionary of labels, not enabled is None
-DebugLabelExists = True		# If true, NONE (no label) and non-explicitly defined labels are all enabled by default
+DebugLabels = None		# Dictionary of labels, not enabled is None
+DebugLabelExists = False	# If False, NONE (no label) and non-explicitly defined labels are all enabled by default
 
 # Signals Module is being used in Cmd Line Mode
 __CmdLineMode__ = False
 
 # Notes:
 # DebugMode puts the module in DebugMode, i.e. it activates DbgMsg() to output
 # 	when DebugMode is false, DbgMsg does nothing.
@@ -1378,71 +1378,78 @@
 
 	if Teefile != None:
 		Log(msg,logfile=Teefile)
 
 def SetDebugLabel(dbglabel,value):
 	"""Enable Debug Label"""
 
-	global DebugEnabled
+	global DebugLabels
 
-	if DebugEnabled is not None:
-		DebugEnabled[dbglabel] = value
+	if DebugLabels is None:
+		DebugLabels = dict()
+
+	DebugLabels[dbglabel] = value
 
 def EnableDebugLabel(dbglabel):
 	"""Enable Debug Label"""
 
 	SetDebugLabel(dbglabel,True)
 
 def DisableDebugLabel(dbglabel):
 	"""Disable Debug Label"""
 
 	SetDebugLabel(dbglabel,False)
 
 def DebugLabelBehavior(value=None):
-	"""Set the default debug label behavior"""
+	"""
+	Set the default debug label behavior
+
+	True to treat 'None' labels and labels not existing in DebugLabels dictionary as enabled
+	False to only consider enabled labels in the DebugLabels dictionary.
+	"""
 
 	global DebugLabelExists
 
 	if not value is None:
 		DebugLabelExists = value
 
 	return DebugLabelExists
 
 def LoadDebugEnableFile(filename):
 	"""Load Debug Enablement Data File"""
 
-	global DebugEnabled, DebugLabelExists
+	global DebugLabels, DebugLabelExists
 
-	if DebugEnabled is not None:
-		del DebugEnabled
+	if DebugLabels is not None:
+		del DebugLabels
 
-	DebugEnabled = None
+	DebugLabels = None
 
 	if os.path.exists(filename):
-		DebugEnabled = dict()
+		DebugLabels = dict()
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
-				if row[0] == "default":
+				if row[0] in [ "default", "behavior", "mustexist" ]:
 					DebugLabelExists = True if row[1] in [ "True","true","TRUE","1","yes","Yes","y","Y" ] else False
 				else:
-					DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","1","Yes","yes","y","Y" ] else False
+					DebugLabels[row[0]] = True if row[1] in [ "True","true","TRUE","1","Yes","yes","y","Y" ] else False
 
 def IsDebugLabelEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
-	global DebugEnabled, DebugLabelExists
+	global DebugLabels, DebugLabelExists
 
-	enabled = DebugLabelExists
+	enabled = not DebugLabelExists
 
-	if DebugEnabled is not None and dbglabel is not None:
-		if dbglabel in DebugEnabled:
-			enabled = DebugEnabled[dbglabel]
+	if DebugLabels is not None and dbglabel is not None:
+		if dbglabel in DebugLabels:
+			enabled = DebugLabels[dbglabel]
 
 	return enabled
 
 def Breakpoint(dbglabel,test_flag=True):
 	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
 
 	enabled = IsDebugLabelEnabled(dbglabel)
@@ -1455,15 +1462,15 @@
 # If "func" is supplied, DbgMsg uses it for output instead of printing to stdout
 def DbgMsg(msg,func=None,prefix="***",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""
 	Messaging function that only prints when in DebugMode.
 	Ignores CmdLineMode/ModuleMode.
 	"""
 
-	global __DebugMode__, DebugEnabled
+	global __DebugMode__
 
 	if __DebugMode__:
 		if not IsDebugLabelEnabled(dbglabel):
 			return
 
 		delta = None
```

### Comparing `py-helper-mod-0.0.38/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.39/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.38
+Version: 0.0.39
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.38/setup.cfg` & `py-helper-mod-0.0.39/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.38
+version = 0.0.39
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

