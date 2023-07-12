# Comparing `tmp/minchin.pelican.plugins.autoloader-1.1.0.tar.gz` & `tmp/minchin.pelican.plugins.autoloader-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minchin.pelican.plugins.autoloader-1.1.0.tar", last modified: Sat Apr  9 17:12:01 2022, max compression
+gzip compressed data, was "minchin.pelican.plugins.autoloader-1.2.0.tar", last modified: Wed Jul 12 05:20:47 2023, max compression
```

## Comparing `minchin.pelican.plugins.autoloader-1.1.0.tar` & `minchin.pelican.plugins.autoloader-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.772565 minchin.pelican.plugins.autoloader-1.1.0/
--rw-rw-rw-   0        0        0      734 2022-04-09 17:06:45.000000 minchin.pelican.plugins.autoloader-1.1.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1088 2021-10-24 03:20:54.000000 minchin.pelican.plugins.autoloader-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       72 2022-04-09 16:22:44.000000 minchin.pelican.plugins.autoloader-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4702 2022-04-09 17:12:01.772565 minchin.pelican.plugins.autoloader-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2022-04-09 17:06:14.000000 minchin.pelican.plugins.autoloader-1.1.0/README.rst
--rw-rw-rw-   0        0        0      464 2021-10-25 04:15:42.000000 minchin.pelican.plugins.autoloader-1.1.0/invoke.yaml
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.656941 minchin.pelican.plugins.autoloader-1.1.0/minchin/
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.656941 minchin.pelican.plugins.autoloader-1.1.0/minchin/pelican/
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.772565 minchin.pelican.plugins.autoloader-1.1.0/minchin/pelican/plugins/
--rw-rw-rw-   0        0        0     4657 2022-04-09 17:11:59.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin/pelican/plugins/autoloader.py
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.756919 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/
--rw-rw-rw-   0        0        0     4702 2022-04-09 17:12:01.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2022-04-09 17:12:01.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-09 17:12:01.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2022-04-09 17:12:01.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2022-04-09 17:12:01.000000 minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.656941 minchin.pelican.plugins.autoloader-1.1.0/pelican/
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.656941 minchin.pelican.plugins.autoloader-1.1.0/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2022-04-09 17:12:01.772565 minchin.pelican.plugins.autoloader-1.1.0/pelican/plugins/autoloader/
--rw-rw-rw-   0        0        0       70 2021-10-24 18:13:52.000000 minchin.pelican.plugins.autoloader-1.1.0/pelican/plugins/autoloader/__init__.py
--rw-rw-rw-   0        0        0      429 2021-10-25 04:15:49.000000 minchin.pelican.plugins.autoloader-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      773 2022-03-21 03:39:37.000000 minchin.pelican.plugins.autoloader-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-09 17:12:01.772565 minchin.pelican.plugins.autoloader-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     5041 2022-03-21 03:36:14.000000 minchin.pelican.plugins.autoloader-1.1.0/setup.py
--rw-rw-rw-   0        0        0       43 2021-10-25 03:26:23.000000 minchin.pelican.plugins.autoloader-1.1.0/tasks.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/
+-rw-rw-rw-   0        0        0      895 2023-07-11 20:36:02.000000 minchin.pelican.plugins.autoloader-1.2.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1092 2023-07-11 20:36:41.000000 minchin.pelican.plugins.autoloader-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       72 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4695 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3280 2023-07-11 20:45:34.000000 minchin.pelican.plugins.autoloader-1.2.0/README.rst
+-rw-rw-rw-   0        0        0      464 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/invoke.yaml
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/minchin/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.288687 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/
+-rw-rw-rw-   0        0        0     4689 2023-07-12 05:20:45.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/autoloader.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.287685 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/
+-rw-rw-rw-   0        0        0     4695 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       36 2023-07-12 05:20:47.000000 minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/pelican/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.260685 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:20:47.289686 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/autoloader/
+-rw-rw-rw-   0        0        0       70 2023-07-11 20:29:20.000000 minchin.pelican.plugins.autoloader-1.2.0/pelican/plugins/autoloader/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-07-11 20:38:02.000000 minchin.pelican.plugins.autoloader-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      815 2023-07-11 20:47:01.000000 minchin.pelican.plugins.autoloader-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:20:47.291686 minchin.pelican.plugins.autoloader-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4567 2023-07-11 21:16:46.000000 minchin.pelican.plugins.autoloader-1.2.0/setup.py
+-rw-rw-rw-   0        0        0      127 2023-07-12 05:00:33.000000 minchin.pelican.plugins.autoloader-1.2.0/tasks.py
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/LICENSE.txt` & `minchin.pelican.plugins.autoloader-1.2.0/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 MinchinWeb
+Copyright (c) 2021-23 Wm. Minchin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/PKG-INFO` & `minchin.pelican.plugins.autoloader-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: minchin.pelican.plugins.autoloader
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pelican plugin, used to auto-load my other plugins.
 Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
@@ -36,26 +35,27 @@
 AutoLoader
 ==========
 
 ``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
 a static site generator written in Python.
 
 ``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespace (``minchin.pelican.plugins``). It can also be extended to autoload
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
 plugins in other namespaces, for example, to autoload the ``pelican.plugins``
 namespace on versions of Pelican before 4.5 (when autoloading to those plugins
 was added to the Pelican core).
 
 .. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
     :alt: PyPI version number
 
-.. image:: https://img.shields.io/badge/-Changelog-success
-   :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-   :alt: Changelog
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
 
 .. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
     :alt: Supported Python version
 
 .. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
     :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
@@ -122,9 +122,7 @@
   ]
 
 Usage Notes
 ===========
 
 - the plugins loaded by this plugin will not be shown when you run
   ``pelican-plugins``
-
-
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/README.rst` & `minchin.pelican.plugins.autoloader-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 AutoLoader
 ==========
 
 ``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
 a static site generator written in Python.
 
 ``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespace (``minchin.pelican.plugins``). It can also be extended to autoload
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
 plugins in other namespaces, for example, to autoload the ``pelican.plugins``
 namespace on versions of Pelican before 4.5 (when autoloading to those plugins
 was added to the Pelican core).
 
 .. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
     :alt: PyPI version number
 
-.. image:: https://img.shields.io/badge/-Changelog-success
-   :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-   :alt: Changelog
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
 
 .. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
     :alt: Supported Python version
 
 .. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
     :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/minchin/pelican/plugins/autoloader.py` & `minchin.pelican.plugins.autoloader-1.2.0/minchin/pelican/plugins/autoloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 import semantic_version
 
 from pelican import __version__ as pelican_version
 from pelican import signals
 
 __title__ = "minchin.pelican.plugins.autoloader"
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __description__ = "Pelican plugin, used to auto-load my other plugins."
 __author__ = "W. Minchin"
 __email__ = "w_minchin@hotmail.com"
 __url__ = "https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader"
 __license__ = "MIT License"
 
 LOG_PREFIX = "[AutoLoader]"
 DEFAULT_NAMESPACE_LIST = [
     "minchin.pelican.plugins",
+    "minchin.pelican.readers",
 ]
 DEFAULT_PLUGIN_BLACKLIST = [
     "pelican.plugins._utils",
     "pelican.plugins.signals",
 ]
 
 logger = logging.getLogger(__name__)
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO` & `minchin.pelican.plugins.autoloader-1.2.0/minchin.pelican.plugins.autoloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: minchin.pelican.plugins.autoloader
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pelican plugin, used to auto-load my other plugins.
 Home-page: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
@@ -36,26 +35,27 @@
 AutoLoader
 ==========
 
 ``AutoLoader`` is a plugin for `Pelican <http://docs.getpelican.com/>`_,
 a static site generator written in Python.
 
 ``AutoLoader`` is designed to autoload the other Pelican plugins in my
-namespace (``minchin.pelican.plugins``). It can also be extended to autoload
+namespaces (``minchin.pelican.plugins`` and ``minchin.pelican.readers``).
+It can also be extended to autoload
 plugins in other namespaces, for example, to autoload the ``pelican.plugins``
 namespace on versions of Pelican before 4.5 (when autoloading to those plugins
 was added to the Pelican core).
 
 .. image:: https://img.shields.io/pypi/v/minchin.pelican.plugins.autoloader.svg?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader
     :alt: PyPI version number
 
-.. image:: https://img.shields.io/badge/-Changelog-success
-   :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
-   :alt: Changelog
+.. image:: https://img.shields.io/badge/-Changelog-success?style=flat
+    :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/CHANGELOG.rst
+    :alt: Changelog
 
 .. image:: https://img.shields.io/pypi/pyversions/minchin.pelican.plugins.autoloader?style=flat
     :target: https://pypi.python.org/pypi/minchin.pelican.plugins.autoloader/
     :alt: Supported Python version
 
 .. image:: https://img.shields.io/pypi/l/minchin.pelican.plugins.autoloader.svg?style=flat&color=green
     :target: https://github.com/MinchinWeb/minchin.pelican.plugins.autoloader/blob/master/LICENSE.txt
@@ -122,9 +122,7 @@
   ]
 
 Usage Notes
 ===========
 
 - the plugins loaded by this plugin will not be shown when you run
   ``pelican-plugins``
-
-
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/requirements.txt` & `minchin.pelican.plugins.autoloader-1.2.0/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
 #    pip-compile
 #
-blinker==1.4
+blinker==1.6.2
     # via pelican
-colorama==0.4.4
-    # via rich
-commonmark==0.9.1
-    # via rich
-docutils==0.17.1
+docutils==0.20.1
     # via pelican
-feedgenerator==2.0.0
+feedgenerator==2.1.0
     # via pelican
-jinja2==3.0.2
+jinja2==3.1.2
     # via pelican
-markupsafe==2.0.1
+markdown-it-py==3.0.0
+    # via rich
+markupsafe==2.1.3
     # via jinja2
-pelican==4.7.1
+mdurl==0.1.2
+    # via markdown-it-py
+pelican==4.8.0
     # via minchin.pelican.plugins.autoloader (setup.py)
-pygments==2.10.0
-    # via
-    #   pelican
+pygments==2.15.1
+    # via
+    #   pelican
     #   rich
-python-dateutil==2.8.2
+python-dateutil==2.8.2
     # via pelican
-pytz==2021.3
-    # via
-    #   feedgenerator
+pytz==2023.3
+    # via
+    #   feedgenerator
     #   pelican
-rich==10.12.0
+rich==13.4.2
     # via pelican
-semantic-version==2.8.5
+semantic-version==2.10.0
     # via minchin.pelican.plugins.autoloader (setup.py)
-six==1.16.0
+six==1.16.0
     # via python-dateutil
-unidecode==1.3.2
+unidecode==1.3.6
     # via pelican
```

### Comparing `minchin.pelican.plugins.autoloader-1.1.0/setup.py` & `minchin.pelican.plugins.autoloader-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,29 +88,19 @@
     # 'Development Status :: 3 - Alpha',
     # "Development Status :: 4 - Beta",
     'Development Status :: 5 - Production/Stable',
     # 'Development Status :: 6 - Mature',
     # 'Development Status :: 7 - Inactive',
     "Environment :: Console",
     "Framework :: Pelican :: Plugins",
-    # "Framework :: Pelican :: Themes",
-    # 'Programming Language :: Python :: 2',
-    # 'Programming Language :: Python :: 2.6',
-    # 'Programming Language :: Python :: 2.7',
-    # 'Programming Language :: Python :: 2 :: Only',
     "Programming Language :: Python :: 3",
-    # 'Programming Language :: Python :: 3.2',
-    # 'Programming Language :: Python :: 3.3',
-    # 'Programming Language :: Python :: 3.4',
-    # "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 ##############################################################################
```

