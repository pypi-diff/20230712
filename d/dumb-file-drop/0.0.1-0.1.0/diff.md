# Comparing `tmp/dumb-file-drop-0.0.1.tar.gz` & `tmp/dumb-file-drop-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumb-file-drop-0.0.1.tar", last modified: Sun May 30 01:13:14 2021, max compression
+gzip compressed data, was "dumb-file-drop-0.1.0.tar", last modified: Wed Jul 12 06:41:59 2023, max compression
```

## Comparing `dumb-file-drop-0.0.1.tar` & `dumb-file-drop-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2021-05-30 01:13:14.254159 dumb-file-drop-0.0.1/
--rw-r--r--   0 alec       (501) staff       (20)    34913 2021-05-01 09:56:37.000000 dumb-file-drop-0.0.1/LICENSE.md
--rw-r--r--   0 alec       (501) staff       (20)       52 2021-05-28 00:58:38.000000 dumb-file-drop-0.0.1/MANIFEST.in
--rw-r--r--   0 alec       (501) staff       (20)     1437 2021-05-30 01:13:14.254056 dumb-file-drop-0.0.1/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      674 2021-05-28 00:12:44.000000 dumb-file-drop-0.0.1/README.md
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2021-05-30 01:13:14.252927 dumb-file-drop-0.0.1/dumb_file_drop/
--rw-r--r--   0 alec       (501) staff       (20)        0 2021-05-28 00:08:28.000000 dumb-file-drop-0.0.1/dumb_file_drop/__init__.py
--rw-r--r--   0 alec       (501) staff       (20)     1285 2021-05-28 01:01:51.000000 dumb-file-drop-0.0.1/dumb_file_drop/__main__.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2021-05-30 01:13:14.253772 dumb-file-drop-0.0.1/dumb_file_drop/templates/
--rw-r--r--   0 alec       (501) staff       (20)     2569 2021-05-28 00:50:26.000000 dumb-file-drop-0.0.1/dumb_file_drop/templates/index.html
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2021-05-30 01:13:14.253658 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)     1437 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      376 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)       55 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/entry_points.txt
--rw-r--r--   0 alec       (501) staff       (20)        6 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)       15 2021-05-30 01:13:14.000000 dumb-file-drop-0.0.1/dumb_file_drop.egg-info/top_level.txt
--rw-r--r--   0 alec       (501) staff       (20)      103 2021-03-05 07:52:18.000000 dumb-file-drop-0.0.1/pyproject.toml
--rw-r--r--   0 alec       (501) staff       (20)       38 2021-05-30 01:13:14.254194 dumb-file-drop-0.0.1/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)     1166 2021-05-28 11:17:45.000000 dumb-file-drop-0.0.1/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-12 06:41:59.455478 dumb-file-drop-0.1.0/
+-rw-r--r--   0 alec       (501) staff       (20)    34913 2022-12-23 07:51:44.000000 dumb-file-drop-0.1.0/LICENSE.md
+-rw-r--r--   0 alec       (501) staff       (20)       52 2022-12-23 07:51:44.000000 dumb-file-drop-0.1.0/MANIFEST.in
+-rw-r--r--   0 alec       (501) staff       (20)     1601 2023-07-12 06:41:59.455365 dumb-file-drop-0.1.0/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      875 2023-07-12 06:32:22.000000 dumb-file-drop-0.1.0/README.md
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-12 06:41:59.454339 dumb-file-drop-0.1.0/dumb_file_drop/
+-rw-r--r--   0 alec       (501) staff       (20)        0 2022-12-23 07:51:44.000000 dumb-file-drop-0.1.0/dumb_file_drop/__init__.py
+-rw-r--r--   0 alec       (501) staff       (20)     2373 2023-07-11 09:08:07.000000 dumb-file-drop-0.1.0/dumb_file_drop/__main__.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-12 06:41:59.455042 dumb-file-drop-0.1.0/dumb_file_drop/templates/
+-rw-r--r--   0 alec       (501) staff       (20)     4830 2023-07-11 08:59:25.000000 dumb-file-drop-0.1.0/dumb_file_drop/templates/index.html
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-12 06:41:59.454917 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)     1601 2023-07-12 06:41:59.000000 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      335 2023-07-12 06:41:59.000000 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2023-07-12 06:41:59.000000 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)       36 2023-07-12 06:41:59.000000 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)       15 2023-07-12 06:41:59.000000 dumb-file-drop-0.1.0/dumb_file_drop.egg-info/top_level.txt
+-rw-r--r--   0 alec       (501) staff       (20)      103 2022-12-23 07:51:44.000000 dumb-file-drop-0.1.0/pyproject.toml
+-rw-r--r--   0 alec       (501) staff       (20)       38 2023-07-12 06:41:59.455515 dumb-file-drop-0.1.0/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)     1089 2023-07-12 06:29:47.000000 dumb-file-drop-0.1.0/setup.py
```

### Comparing `dumb-file-drop-0.0.1/LICENSE.md` & `dumb-file-drop-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dumb-file-drop-0.0.1/PKG-INFO` & `dumb-file-drop-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dumb-file-drop
-Version: 0.0.1
-Summary: A simple webserver-based drop box which allows files uploads.  Good for quickly sharing files on your local network.
+Version: 0.1.0
+Summary: A simple webserver-based drop box which allows file uploads.  Good for quickly sharing files on your local network.
 Home-page: https://github.com/fastily/dumb-file-drop
 Author: Fastily
 Author-email: fastily@users.noreply.github.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fastily/dumb-file-drop/issues
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -21,16 +19,24 @@
 [![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 Simple webserver which allows files to be uploaded to it.  Good for quickly sharing files on your local network.
 
 Files will be uploaded to `./uploads`
 
-Run:
+## Install
 ```bash
-python -m dumb_file_drop
+pip install dumb-file-drop
 ```
 
-Endpoint: [localhost:5000](http://localhost:5000)
+## Run
+```bash
+# invoking this module directly, runs in debug mode
+python -m dumb_file_drop
+
+# prod
+gunicorn -b "0.0.0.0" -w 4 -k uvicorn.workers.UvicornWorker dumb_file_drop.__main__:app
+```
 
-⚠️ Do not run this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
+Endpoint: [localhost:8000](http://localhost:8000)
 
+⚠️ Do not use this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
```

### Comparing `dumb-file-drop-0.0.1/README.md` & `dumb-file-drop-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 [![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 Simple webserver which allows files to be uploaded to it.  Good for quickly sharing files on your local network.
 
 Files will be uploaded to `./uploads`
 
-Run:
+## Install
 ```bash
+pip install dumb-file-drop
+```
+
+## Run
+```bash
+# invoking this module directly, runs in debug mode
 python -m dumb_file_drop
+
+# prod
+gunicorn -b "0.0.0.0" -w 4 -k uvicorn.workers.UvicornWorker dumb_file_drop.__main__:app
 ```
 
-Endpoint: [localhost:5000](http://localhost:5000)
+Endpoint: [localhost:8000](http://localhost:8000)
 
-⚠️ Do not run this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
+⚠️ Do not use this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
```

### Comparing `dumb-file-drop-0.0.1/dumb_file_drop.egg-info/PKG-INFO` & `dumb-file-drop-0.1.0/dumb_file_drop.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dumb-file-drop
-Version: 0.0.1
-Summary: A simple webserver-based drop box which allows files uploads.  Good for quickly sharing files on your local network.
+Version: 0.1.0
+Summary: A simple webserver-based drop box which allows file uploads.  Good for quickly sharing files on your local network.
 Home-page: https://github.com/fastily/dumb-file-drop
 Author: Fastily
 Author-email: fastily@users.noreply.github.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fastily/dumb-file-drop/issues
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -21,16 +19,24 @@
 [![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 Simple webserver which allows files to be uploaded to it.  Good for quickly sharing files on your local network.
 
 Files will be uploaded to `./uploads`
 
-Run:
+## Install
 ```bash
-python -m dumb_file_drop
+pip install dumb-file-drop
 ```
 
-Endpoint: [localhost:5000](http://localhost:5000)
+## Run
+```bash
+# invoking this module directly, runs in debug mode
+python -m dumb_file_drop
+
+# prod
+gunicorn -b "0.0.0.0" -w 4 -k uvicorn.workers.UvicornWorker dumb_file_drop.__main__:app
+```
 
-⚠️ Do not run this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
+Endpoint: [localhost:8000](http://localhost:8000)
 
+⚠️ Do not use this on public/untrusted networks!  There's no built-in authentication, so anybody could upload files to your computer!
```

### Comparing `dumb-file-drop-0.0.1/setup.py` & `dumb-file-drop-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dumb-file-drop",
-    version="0.0.1",
+    version="0.1.0",
     author="Fastily",
     author_email="fastily@users.noreply.github.com",
-    description="A simple webserver-based drop box which allows files uploads.  Good for quickly sharing files on your local network.",
+    description="A simple webserver-based drop box which allows file uploads.  Good for quickly sharing files on your local network.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fastily/dumb-file-drop",
     project_urls={
         "Bug Tracker": "https://github.com/fastily/dumb-file-drop/issues",
     },
     include_package_data=True,
     packages=setuptools.find_packages(include=["dumb_file_drop"]),
-    install_requires=["Flask"],
-    entry_points={
-        'console_scripts': [
-            'dfd = dumb_file_drop.__main__:_main'
-        ]
-    },
+    install_requires=["aiofiles", "fastapi[all]", "gunicorn", "rich"],
     classifiers=[
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
```

