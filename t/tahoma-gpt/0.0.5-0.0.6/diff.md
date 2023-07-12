# Comparing `tmp/tahoma_gpt-0.0.5.tar.gz` & `tmp/tahoma_gpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma_gpt-0.0.5.tar", last modified: Wed Jul 12 02:05:28 2023, max compression
+gzip compressed data, was "tahoma_gpt-0.0.6.tar", last modified: Wed Jul 12 02:20:21 2023, max compression
```

## Comparing `tahoma_gpt-0.0.5.tar` & `tahoma_gpt-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:05:28.409925 tahoma_gpt-0.0.5/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.5/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.5/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 02:05:28.410042 tahoma_gpt-0.0.5/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.5/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.5/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.5/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:52:47.000000 tahoma_gpt-0.0.5/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 02:05:28.410416 tahoma_gpt-0.0.5/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.5/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:05:28.405684 tahoma_gpt-0.0.5/tahoma_gpt/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.5/tahoma_gpt/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 02:05:09.000000 tahoma_gpt-0.0.5/tahoma_gpt/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:59:32.000000 tahoma_gpt-0.0.5/tahoma_gpt/__version__.py~
--rwxrwx---   0 neptune   (1000) neptune   (1000)    37454 2023-07-12 02:04:47.000000 tahoma_gpt-0.0.5/tahoma_gpt/tahoma_gpt.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    37464 2023-07-12 01:59:04.000000 tahoma_gpt-0.0.5/tahoma_gpt/tahoma_gpt.py~
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:05:28.409503 tahoma_gpt-0.0.5/tahoma_gpt/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.5/tahoma_gpt/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.5/tahoma_gpt/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:05:28.408525 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      480 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 02:05:28.000000 tahoma_gpt-0.0.5/tahoma_gpt.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:20:21.316079 tahoma_gpt-0.0.6/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.6/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.6/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 02:20:21.316182 tahoma_gpt-0.0.6/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.6/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.6/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.6/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:52:47.000000 tahoma_gpt-0.0.6/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 02:20:21.316527 tahoma_gpt-0.0.6/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.6/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:20:21.312585 tahoma_gpt-0.0.6/tahoma_gpt/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.6/tahoma_gpt/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 02:19:57.000000 tahoma_gpt-0.0.6/tahoma_gpt/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    37799 2023-07-12 02:19:46.000000 tahoma_gpt-0.0.6/tahoma_gpt/tahoma_gpt.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:20:21.315783 tahoma_gpt-0.0.6/tahoma_gpt/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.6/tahoma_gpt/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.6/tahoma_gpt/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 02:20:21.315030 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      427 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 02:20:21.000000 tahoma_gpt-0.0.6/tahoma_gpt.egg-info/top_level.txt
```

### Comparing `tahoma_gpt-0.0.5/LICENSE` & `tahoma_gpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.5/PKG-INFO` & `tahoma_gpt-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma_gpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tahoma_gpt-0.0.5/PYPI_README.md` & `tahoma_gpt-0.0.6/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.5/README.md` & `tahoma_gpt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.5/pyproject.toml` & `tahoma_gpt-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.5/tahoma_gpt/tahoma_gpt.py` & `tahoma_gpt-0.0.6/tahoma_gpt/tahoma_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,36 +42,43 @@
 #arguments
 args = sys.argv
 
 def main():
     version = str(__version__.__version__)
     langage="english"
     version='tahoma_gpt : Pypi version '+version+"_"+langage
+
     def search(filename_to_find):
         # Répertoire d'exécution du script
         try:
             script_directory = os.path.dirname(os.path.abspath(__file__))
         except:
             script_directory = os.path.dirname(os.path.abspath(__name__))
+        
         # Fonction récursive pour rechercher le fichier dans les répertoires
         def search_directory_for_file(directory, filename):
             for root, dirs, files in os.walk(directory):
                 if filename in files:
                     file_path = os.path.join(root, filename)
                     return file_path
-            return None  
-        file_path = search_directory_for_file(script_directory, filename_to_find)
-        if file_path:
-            folder_path = os.path.dirname(file_path)
-            #print("Le fichier", filename_to_find, "a été trouvé dans le dossier :", folder_path)
-        else:
-            pass
-            #print("Le fichier", filename_to_find, "n'a pas été trouvé dans les répertoires.")    
-        return file_path
-    #folder_path=search('tahoma.py')
+            return None
+        current_directory = script_directory
+        while True:
+            file_path = search_directory_for_file(current_directory, filename_to_find)
+            if file_path:
+                folder_path = os.path.dirname(file_path)
+                #print("Le fichier", filename_to_find, "a été trouvé dans le dossier :", folder_path)
+                return file_path
+            parent_directory = os.path.dirname(current_directory)
+            # Vérifier si le dossier parent est le même que le dossier actuel pour éviter une boucle infinie
+            if parent_directory == current_directory:
+                break
+            current_directory = parent_directory
+        #print("Le fichier", filename_to_find, "n'a pas été trouvé dans les répertoires.")
+        return None
 
     try:
         names = subprocess.check_output("'"+str(search('tahoma')) + "' -ln", shell=True)
         names = names.decode('utf-8')
         index_exclusion = names.find("You must provide a part of the NAME as argument")
         if index_exclusion != -1:
             names = names[:index_exclusion]
```

### Comparing `tahoma_gpt-0.0.5/tahoma_gpt.egg-info/PKG-INFO` & `tahoma_gpt-0.0.6/tahoma_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma-gpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

