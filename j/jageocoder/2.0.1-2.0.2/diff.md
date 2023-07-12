# Comparing `tmp/jageocoder-2.0.1.tar.gz` & `tmp/jageocoder-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.0.1.tar", max compression
+gzip compressed data, was "jageocoder-2.0.2.tar", max compression
```

## Comparing `jageocoder-2.0.1.tar` & `jageocoder-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      113 2023-04-28 00:22:42.161103 jageocoder-2.0.1/LICENSE
--rw-r--r--   0        0        0     8253 2023-04-28 00:22:42.161103 jageocoder-2.0.1/README.md
--rw-r--r--   0        0        0     1405 2023-04-29 00:02:26.756784 jageocoder-2.0.1/jageocoder/__init__.py
--rw-r--r--   0        0        0     4541 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/aliases.json
--rw-r--r--   0        0        0    12147 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/exceptions.py
--rw-r--r--   0        0        0    18862 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    11293 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/module.py
--rw-r--r--   0        0        0    37186 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/node.py
--rw-r--r--   0        0        0     2631 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/result.py
--rw-r--r--   0        0        0    15241 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/rtree.py
--rw-r--r--   0        0        0     7854 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/strlib.py
--rw-r--r--   0        0        0    48985 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/trie.py
--rw-r--r--   0        0        0     1223 2023-04-29 00:02:40.686784 jageocoder-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     9747 1970-01-01 00:00:00.000000 jageocoder-2.0.1/setup.py
--rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 jageocoder-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-17 09:16:28.271600 jageocoder-2.0.2/LICENSE
+-rw-r--r--   0        0        0     8253 2023-04-29 04:07:32.527460 jageocoder-2.0.2/README.md
+-rw-r--r--   0        0        0     1359 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/__init__.py
+-rw-r--r--   0        0        0     4622 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/aliases.json
+-rw-r--r--   0        0        0    12147 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    18862 2023-04-22 02:31:05.987235 jageocoder-2.0.2/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    10888 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/module.py
+-rw-r--r--   0        0        0    37186 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/node.py
+-rw-r--r--   0        0        0     2631 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/result.py
+-rw-r--r--   0        0        0    15241 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7854 2023-04-17 09:16:28.283600 jageocoder-2.0.2/jageocoder/strlib.py
+-rw-r--r--   0        0        0    48985 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/trie.py
+-rw-r--r--   0        0        0     1225 2023-07-12 05:31:17.491752 jageocoder-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 jageocoder-2.0.2/PKG-INFO
```

### Comparing `jageocoder-2.0.1/README.md` & `jageocoder-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/__init__.py` & `jageocoder-2.0.2/jageocoder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,39 +15,38 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.0.1'  # The package version
+__version__ = '2.0.2'  # The package version
 __dictionary_version__ = '20230405'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
     'set_search_config',
     'get_search_config',
     'get_db_dir',
     'get_module_tree',
     'download_dictionary',
     'install_dictionary',
     'uninstall_dictionary',
-    'migrate_dictionary',
     'create_trie_index',
     'search',
     'searchNode',
     'reverse',
     'version',
     'dictionary_version',
     'installed_dictionary_version',
     'instaleld_dictionary_readme',
 ]
 
 from jageocoder.module import init, free, is_initialized,\
     get_db_dir, set_search_config, get_search_config,\
     get_module_tree, download_dictionary, install_dictionary,\
-    uninstall_dictionary, migrate_dictionary, create_trie_index,\
+    uninstall_dictionary, create_trie_index,\
     search, searchNode, reverse, version, dictionary_version,\
     installed_dictionary_version, installed_dictionary_readme  # noqa: F401
```

### Comparing `jageocoder-2.0.1/jageocoder/__main__.py` & `jageocoder-2.0.2/jageocoder/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Usage:
   {p} -h
   {p} -v
   {p} search [-d] [--area=<area>] [--db-dir=<dir>] [--force-aza-skip|--disable-aza-skip] <address>
   {p} reverse [-d] [--level=<level>] [--db-dir=<dir>] <longitude> <latitude>
   {p} get-db-dir [-d]
   {p} download-dictionary [-d] <url>
-  {p} install-dictionary [-d] [--db-dir=<dir>] <path>
+  {p} install-dictionary [-d] [-y] [--db-dir=<dir>] <path>
   {p} uninstall-dictionary [-d] [--db-dir=<dir>]
 
 Options:
   -h --help           Show this help.
   -v --version        Show version number.
   -d --debug          Show debug messages.
   --area=<area>       Specify the target area by jiscode or names.
@@ -134,19 +134,20 @@
             exit(1)
 
     elif args['install-dictionary']:
         path = args['<path>']
         try:
             jageocoder.install_dictionary(
                 path=path,
-                db_dir=args['--db-dir']
+                db_dir=args['--db-dir'],
+                skip_confirmation=(args['-y'] is True),
             )
         except JageocoderError:
             logging.warning((
-                "Could not find the dictionary at '{}'.".format(path)
+                "辞書データファイルが '{}' にありません。".format(path)
             ))
             exit(1)
 
     elif args['uninstall-dictionary']:
         jageocoder.uninstall_dictionary(
             db_dir=args['--db-dir'])
     elif args['migrate-dictionary']:
```

### Comparing `jageocoder-2.0.1/jageocoder/address.py` & `jageocoder-2.0.2/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/aliases.json` & `jageocoder-2.0.2/jageocoder/aliases.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/aza_master.py` & `jageocoder-2.0.2/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/dataset.py` & `jageocoder-2.0.2/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/exceptions.py` & `jageocoder-2.0.2/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/itaiji.py` & `jageocoder-2.0.2/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/itaiji_dic.json` & `jageocoder-2.0.2/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/module.py` & `jageocoder-2.0.2/jageocoder/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,16 @@
         raise JageocoderError(
             "The dictionary file could not be downloaded"
             + " from the URL {}".format(url))
 
 
 def install_dictionary(
         path: os.PathLike,
-        db_dir: Optional[os.PathLike] = None) -> None:
+        db_dir: Optional[os.PathLike] = None,
+        skip_confirmation: bool = False) -> None:
     """
     Install address-dictionary from the specified path.
 
     Parameters
     ----------
     path: os.PathLike
         The file path where the zipped address-dictionary file exists.
@@ -189,14 +190,20 @@
 
         If omitted, use `get_db_dir()` to decide the directory.
     """
     # Set default value
     if db_dir is None:
         db_dir = get_db_dir(mode='w')
 
+    if skip_confirmation is not True and (db_dir / 'address_node').exists():
+        # Dictionary had been installed.
+        r = input("他の辞書がインストール済みです。上書きしますか？(Y/n) ")
+        if r.lower()[0] != 'y':
+            return
+
     if os.path.exists(path):
         path = path
     else:
         raise JageocoderError("Can't open file '{}'".format(path))
 
     # Unzip the archive
     shutil.rmtree(db_dir)
@@ -231,38 +238,14 @@
     # Remove the directory
     logger.info('Removing directory {}'.format(db_dir))
     import shutil
     shutil.rmtree(db_dir)
     logger.info('Dictionary has been uninstalled.')
 
 
-def migrate_dictionary(db_dir: Optional[os.PathLike] = None) -> None:
-    """
-    Migrate address-dictionary.
-
-    Parameters
-    ----------
-    db_dir: os.PathLike, optional
-        The directory where the database files has been installed.
-        If omitted, it will be determined by `get_db_dir()`.
-    """
-    # Set default value
-    if db_dir is None:
-        db_dir = get_db_dir(mode='a')
-
-    # Update the name and trie index
-    init(db_dir=db_dir, mode='a')
-    global _tree
-    # logger.info('Updating name index')
-    # _tree.update_name_index()
-    logger.info('Updating TRIE index {}'.format(_tree.trie_path))
-    _tree.create_trie_index()
-    logger.info('The dictionary is successfully migrated.')
-
-
 def installed_dictionary_version(db_dir: Optional[os.PathLike] = None) -> str:
     """
     Get the installed dictionary version.
 
     Parameters
     ----------
     db_dir: os.PathLike, optional
```

### Comparing `jageocoder-2.0.1/jageocoder/node.py` & `jageocoder-2.0.2/jageocoder/node.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/result.py` & `jageocoder-2.0.2/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/rtree.py` & `jageocoder-2.0.2/jageocoder/rtree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/strlib.py` & `jageocoder-2.0.2/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/tree.py` & `jageocoder-2.0.2/jageocoder/tree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/jageocoder/trie.py` & `jageocoder-2.0.2/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.1/pyproject.toml` & `jageocoder-2.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.0.1"
+version = "2.0.2"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
@@ -23,27 +23,27 @@
 python = "^3.7"
 marisa-trie = "^0.7.8"
 jaconv = "^0.3.4"
 docopt = "^0.6.2"
 deprecated = "^1.2.13"
 Werkzeug = ">=2.2.3"
 pycapnp = "^1.3.0"
-portabletab = "0.3.1"
+portabletab = ">=0.3.3"
 tqdm = "^4.00.0"
 rtree = "^1.0.0"
 geographiclib = "^2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^5.0.0"
 twine = "^4.0.2"
-flask = "^2.2.3"
 flask-cors = "^3.0.10"
 sphinx = "<6.0.0"
 sphinx-rtd-theme = "^1.2.0"
+flask = "^2.2.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 jageocoder = "jageocoder.__main__:main"
```

### Comparing `jageocoder-2.0.1/PKG-INFO` & `jageocoder-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Werkzeug (>=2.2.3)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: geographiclib (>=2.0,<3.0)
 Requires-Dist: jaconv (>=0.3.4,<0.4.0)
 Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
-Requires-Dist: portabletab (==0.3.1)
+Requires-Dist: portabletab (>=0.3.3)
 Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
 Requires-Dist: rtree (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.00.0,<5.0.0)
 Project-URL: Documentation, https://jageocoder.readthedocs.io/
 Project-URL: Repository, https://github.com/t-sagara/jageocoder/
 Description-Content-Type: text/markdown
```

