# Comparing `tmp/threddsclient-0.4.3.tar.gz` & `tmp/threddsclient-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threddsclient-0.4.3.tar", last modified: Fri Jul  7 14:32:07 2023, max compression
+gzip compressed data, was "threddsclient-0.4.4.tar", last modified: Wed Jul 12 16:03:08 2023, max compression
```

## Comparing `threddsclient-0.4.3.tar` & `threddsclient-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.684966 threddsclient-0.4.3/
--rw-r--r--   0 pingu      (501) staff       (20)       96 2023-07-07 14:28:04.000000 threddsclient-0.4.3/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     1212 2023-07-07 14:32:00.000000 threddsclient-0.4.3/CHANGES.rst
--rw-r--r--   0 pingu      (501) staff       (20)    11324 2023-07-07 14:28:04.000000 threddsclient-0.4.3/LICENCE.txt
--rw-r--r--   0 pingu      (501) staff       (20)       78 2023-07-07 14:28:04.000000 threddsclient-0.4.3/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     6208 2023-07-07 14:32:07.685189 threddsclient-0.4.3/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     4374 2023-07-07 14:28:04.000000 threddsclient-0.4.3/README.rst
--rw-r--r--   0 pingu      (501) staff       (20)       37 2023-07-07 14:28:04.000000 threddsclient-0.4.3/requirements-dev.txt
--rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-07 14:28:04.000000 threddsclient-0.4.3/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      548 2023-07-07 14:32:07.686100 threddsclient-0.4.3/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     1059 2023-07-07 14:32:00.000000 threddsclient-0.4.3/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.674707 threddsclient-0.4.3/tests/
--rw-r--r--   0 pingu      (501) staff       (20)     2985 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_birdhouse_sample.py
--rw-r--r--   0 pingu      (501) staff       (20)     2345 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_catalog.py
--rw-r--r--   0 pingu      (501) staff       (20)     2260 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_dataset.py
--rw-r--r--   0 pingu      (501) staff       (20)    10499 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_noaa_sample.py
--rw-r--r--   0 pingu      (501) staff       (20)      953 2023-07-07 14:32:00.000000 threddsclient-0.4.3/tests/test_online.py
--rw-r--r--   0 pingu      (501) staff       (20)      530 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.678711 threddsclient-0.4.3/threddsclient/
--rw-r--r--   0 pingu      (501) staff       (20)       98 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     5121 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/catalog.py
--rw-r--r--   0 pingu      (501) staff       (20)     2324 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/client.py
--rw-r--r--   0 pingu      (501) staff       (20)     6274 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/nodes.py
--rw-r--r--   0 pingu      (501) staff       (20)     1127 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.684396 threddsclient-0.4.3/threddsclient.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     6208 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)      598 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-07 14:30:19.000000 threddsclient-0.4.3/threddsclient.egg-info/not-zip-safe
--rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       14 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/top_level.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-12 16:03:08.813556 threddsclient-0.4.4/
+-rw-r--r--   0 pingu      (501) staff       (20)       96 2023-07-10 10:30:01.000000 threddsclient-0.4.4/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     3372 2023-07-12 16:02:17.000000 threddsclient-0.4.4/CHANGES.rst
+-rw-r--r--   0 pingu      (501) staff       (20)    11324 2023-07-10 10:30:01.000000 threddsclient-0.4.4/LICENCE.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       78 2023-07-10 10:30:01.000000 threddsclient-0.4.4/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     9649 2023-07-12 16:03:08.813838 threddsclient-0.4.4/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     5223 2023-07-10 10:30:01.000000 threddsclient-0.4.4/README.rst
+-rw-r--r--   0 pingu      (501) staff       (20)       37 2023-07-10 10:30:01.000000 threddsclient-0.4.4/requirements-dev.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-10 10:30:01.000000 threddsclient-0.4.4/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)     1192 2023-07-12 16:03:08.815078 threddsclient-0.4.4/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     1457 2023-07-10 10:30:01.000000 threddsclient-0.4.4/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-12 16:03:08.805325 threddsclient-0.4.4/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)     2985 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_birdhouse_sample.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2345 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_catalog.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2260 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_dataset.py
+-rw-r--r--   0 pingu      (501) staff       (20)    10499 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_noaa_sample.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1209 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_online.py
+-rw-r--r--   0 pingu      (501) staff       (20)      530 2023-07-10 10:30:01.000000 threddsclient-0.4.4/tests/test_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-12 16:03:08.808819 threddsclient-0.4.4/threddsclient/
+-rw-r--r--   0 pingu      (501) staff       (20)       98 2023-07-12 16:02:17.000000 threddsclient-0.4.4/threddsclient/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     5121 2023-07-10 10:30:01.000000 threddsclient-0.4.4/threddsclient/catalog.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2324 2023-07-10 10:30:01.000000 threddsclient-0.4.4/threddsclient/client.py
+-rw-r--r--   0 pingu      (501) staff       (20)     6274 2023-07-10 10:30:01.000000 threddsclient-0.4.4/threddsclient/nodes.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1127 2023-07-10 10:30:01.000000 threddsclient-0.4.4/threddsclient/utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-12 16:03:08.812966 threddsclient-0.4.4/threddsclient.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     9649 2023-07-12 16:03:08.000000 threddsclient-0.4.4/threddsclient.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)      598 2023-07-12 16:03:08.000000 threddsclient-0.4.4/threddsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-12 16:03:08.000000 threddsclient-0.4.4/threddsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-10 10:31:52.000000 threddsclient-0.4.4/threddsclient.egg-info/not-zip-safe
+-rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-12 16:03:08.000000 threddsclient-0.4.4/threddsclient.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       14 2023-07-12 16:03:08.000000 threddsclient-0.4.4/threddsclient.egg-info/top_level.txt
```

### Comparing `threddsclient-0.4.3/LICENCE.txt` & `threddsclient-0.4.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/PKG-INFO` & `threddsclient-0.4.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: threddsclient
-Version: 0.4.3
+Version: 0.4.4
 Summary: Thredds catalog client
 Author: Birdhouse
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Requires-Python: >=3.7,<3.12
 License-File: LICENCE.txt
 License-File: AUTHORS.rst
 
 =========================
 Thredds Client for Python
 =========================
 
@@ -22,102 +31,124 @@
 
 Installing Thredds Client
 =========================
 
 Anaconda
 --------
 
-|Version| |Downloads|
+|Version-GitHub| |Version-Anaconda| |Version-PyPI| |Downloads|
 
 Thredds client is available as Anaconda package. Install it with the
 following command:
 
-.. code:: bash
+.. code-block:: bash
 
-    $ conda install -c conda-forge threddsclient
+    conda install -c conda-forge threddsclient
 
-From github
+From PyPI
+---------
+
+Thredds Client is available from PyPI to install directly with ``pip`` or ``poetry``.
+
+.. code-block:: bash
+
+    pip install threddsclient
+
+
+.. code-block:: bash
+
+    poetry add threddsclient
+
+
+From GitHub
 -----------
 
 Check out code from the birdy GitHub repo and start the installation:
 
-.. code:: bash
+.. code-block:: bash
+
+    git clone https://github.com/bird-house/threddsclient.git
+    cd threddsclient
+    conda env create -f environment.yml
+    source activate threddsclient
+    python setup.py develop
+
+Alternatively, you can also install it directly with ``pip`` using a virtual environment of your choice:
+
+.. code-block:: bash
+
+    pip install "threddsclient @ git+https://github.com/bird-house/threddsclient.git"
 
-    $ git clone https://github.com/bird-house/threddsclient.git
-    $ cd threddsclient
-    $ conda env create -f environment.yml
-    $ source activate threddsclient
-    $ python setup.py develop
 
 Using Thredds Client
 ====================
 
 Read the Thredds tutorial on catalogs: `Thredds Catalog
 Primer <http://www.unidata.ucar.edu/software/thredds/current/tds/tutorial/CatalogPrimer.html>`__
 
 Get download URLs of a catalog
 ------------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.download_urls('http://example.com/thredds/catalog.xml')
 
 Get OpenDAP URLs of a catalog
 -----------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.opendap_urls('http://example.com/thredds/catalog.xml')
 
 Navigate in catalog
 -------------------
 
 Start reading a catalog
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         cat = threddsclient.read_url('http://example.com/thredds/catalog.xml')
 
 Get a list of references to other catalogs & follow them
 
-.. code:: python
+.. code-block:: python
 
         refs = cat.references
 
         print refs[0].name
         cat2 = refs[0].follow()
 
 Get a list of datasets in this catalog
 
-.. code:: python
+.. code-block:: python
 
         data  = cat.datasets
 
 Get flat list of all direct datasets (data files) in the catalog
 
-.. code:: python
+.. code-block:: python
 
         datasets = cat.flat_datasets()
 
 Get flat list of all references in the catalog
 
-.. code:: python
+.. code-block:: python
 
         references = cat.flat_references()
 
 Crawl thredds catalog
 ---------------------
 
 Crawl recursive all direct datasets in catalog following the catalog
-references. Stop recusion at a given depth level.
+references. Stop recursion at a given depth level.
 
-.. code:: python
+.. code-block:: python
 
        import threddsclient
        for ds in threddsclient.crawl('http://example.com/thredds/catalog.xml', depth=2):
            print ds.name
 
 Development
 ===========
@@ -125,24 +156,26 @@
 Install sources
 ---------------
 
 Check out code from the birdy GitHub repo and start the installation:
 
 .. code-block:: sh
 
-   $ git clone https://github.com/bird-house/threddsclient.git
-   $ cd threddsclient
-   $ conda env create -f environment.yml
-   $ python setup.py develop
-
-Install additional dependencies::
-
-  $ conda install pytest flake8 sphinx bumpversion
-  OR
-  $ pip install -r requirements_dev.txt
+   git clone https://github.com/bird-house/threddsclient.git
+   cd threddsclient
+   conda env create -f environment.yml
+   python setup.py develop
+
+Install additional dependencies:
+
+.. code-block:: sh
+
+    conda install pytest flake8 sphinx bumpversion
+    # OR
+    pip install -r requirements_dev.txt
 
 Bump a new version
 ------------------
 
 Make a new version of Birdy in the following steps:
 
 * Make sure everything is commit to GitHub.
@@ -166,97 +199,118 @@
    :target: https://travis-ci.org/bird-house/threddsclient
 .. |Install with Conda| image:: https://anaconda.org/conda-forge/threddsclient/badges/installer/conda.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |License| image:: https://anaconda.org/conda-forge/threddsclient/badges/license.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |Join the Chat| image:: https://badges.gitter.im/bird-house/birdhouse.svg
    :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Version| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
+.. |Version-GitHub| image:: https://img.shields.io/github/v/release/bird-house/threddsclient?label=GitHub
+   :target: https://github.com/bird-house/threddsclient/releases
+.. |Version-Anaconda| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
    :target: https://anaconda.org/conda-forge/threddsclient
+.. |Version-PyPI| image:: https://img.shields.io/pypi/v/threddsclient?color=blue
+   :target: https://pypi.org/project/threddsclient/
 .. |Downloads| image:: https://anaconda.org/conda-forge/threddsclient/badges/downloads.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 
 Authors
 =======
 
 *  Scott Wales scott.wales@unimelb.edu.au
 *  Carsten Ehbrecht ehbrecht@dkrz.de
 
 =======
 Changes
 =======
 
-0.4.3 (2023-05-31)
-==================
+`Unreleased <https://github.com/bird-house/threddsclient/tree/master>`_
+==========================================================================================
+
+* Nothing new for the moment.
+
+.. _changes_0.4.4:
+
+`0.4.4 <https://github.com/bird-house/threddsclient/tree/v0.4.4>`_ (2023-07-11)
+==========================================================================================
+
+* add shield badges for PyPI and GitHub releases
+* fix rendering of code blocks in ``README.rst``
+* add missing classifiers and python requirements to ``setup.py`` to allow validators to detect appropriate versions
+* add python 3.9, 3.10 and 3.11 to the supported versions in ``setup.py`` and validate them in GitHub CI
+* drop Travis CI configuration in favor of GitHub CI
+* fix ``test_noaa`` with the target THREDDS server responding differently than originally tested
+
+`0.4.3 <https://github.com/bird-house/threddsclient/tree/v0.4.3>`_ (2023-05-31)
+==========================================================================================
 
 * fix xml parsing for recent versions
 
-0.4.2 (2019-11-20)
-==================
+`0.4.2 <https://github.com/bird-house/threddsclient/tree/v0.4.2>`_ (2019-11-20)
+==========================================================================================
 
 * fixed conda links in Readme.
 
-0.4.1 (2019-11-06)
-==================
+`0.4.1 <https://github.com/bird-house/threddsclient/tree/v0.4.1>`_ (2019-11-06)
+==========================================================================================
 
 * fixed docs formatting.
 
-0.4.0 (2019-11-06)
-==================
+`0.4.0 <https://github.com/bird-house/threddsclient/tree/v0.4.0>`_ (2019-11-06)
+==========================================================================================
 
 * drop Python 2.7 (#5)
 * fix pip install (#4)
 
-0.3.5 (2018-10-05)
-==================
+`0.3.5 <https://github.com/bird-house/threddsclient/tree/v0.3.5>`_ (2018-10-05)
+==========================================================================================
 
 * support for Python 3.x (#1)
 
-0.3.4 (2015-10-25)
-==================
+`0.3.4 <https://github.com/bird-house/threddsclient/tree/v0.3.4>`_ (2015-10-25)
+==========================================================================================
 
 * fixed travis build/tests
 * updated docs
 
 0.3.3 (2015-10-24)
-==================
+==========================================================================================
 
 * converted docs to rst.
 * MANIFEST.in added.
 
 0.3.2 (2015-07-15)
-==================
+==========================================================================================
 
 *  append catalog.xml to catalog url if missing
 *  crawl method added
 
 0.3.1 (2015-06-14)
-==================
+==========================================================================================
 
 *  fixed catalog.follow()
 *  using dataset.download_url()
 *  added ipython example
 *  cleaned up Readme
 
 0.3.0 (2015-06-13)
-==================
+==========================================================================================
 
 *  Refactored
 *  added catalog.opendap_urls()
 
 0.2.0 (2015-06-08)
-==================
+==========================================================================================
 
 *  Refactored
 *  using CollectionDataset
 *  added catalog.download_urls()
 
 0.1.1 (2015-06-05)
-==================
+==========================================================================================
 
 *  Fixed catalog generation.
 *  added pytest dependency.
 
 0.1.0 (2015-03-13)
-==================
+==========================================================================================
 
 *  Version by https://github.com/ScottWales/threddsclient.
```

### Comparing `threddsclient-0.4.3/README.rst` & `threddsclient-0.4.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,102 +6,124 @@
 
 Installing Thredds Client
 =========================
 
 Anaconda
 --------
 
-|Version| |Downloads|
+|Version-GitHub| |Version-Anaconda| |Version-PyPI| |Downloads|
 
 Thredds client is available as Anaconda package. Install it with the
 following command:
 
-.. code:: bash
+.. code-block:: bash
 
-    $ conda install -c conda-forge threddsclient
+    conda install -c conda-forge threddsclient
 
-From github
+From PyPI
+---------
+
+Thredds Client is available from PyPI to install directly with ``pip`` or ``poetry``.
+
+.. code-block:: bash
+
+    pip install threddsclient
+
+
+.. code-block:: bash
+
+    poetry add threddsclient
+
+
+From GitHub
 -----------
 
 Check out code from the birdy GitHub repo and start the installation:
 
-.. code:: bash
+.. code-block:: bash
+
+    git clone https://github.com/bird-house/threddsclient.git
+    cd threddsclient
+    conda env create -f environment.yml
+    source activate threddsclient
+    python setup.py develop
+
+Alternatively, you can also install it directly with ``pip`` using a virtual environment of your choice:
+
+.. code-block:: bash
+
+    pip install "threddsclient @ git+https://github.com/bird-house/threddsclient.git"
 
-    $ git clone https://github.com/bird-house/threddsclient.git
-    $ cd threddsclient
-    $ conda env create -f environment.yml
-    $ source activate threddsclient
-    $ python setup.py develop
 
 Using Thredds Client
 ====================
 
 Read the Thredds tutorial on catalogs: `Thredds Catalog
 Primer <http://www.unidata.ucar.edu/software/thredds/current/tds/tutorial/CatalogPrimer.html>`__
 
 Get download URLs of a catalog
 ------------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.download_urls('http://example.com/thredds/catalog.xml')
 
 Get OpenDAP URLs of a catalog
 -----------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.opendap_urls('http://example.com/thredds/catalog.xml')
 
 Navigate in catalog
 -------------------
 
 Start reading a catalog
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         cat = threddsclient.read_url('http://example.com/thredds/catalog.xml')
 
 Get a list of references to other catalogs & follow them
 
-.. code:: python
+.. code-block:: python
 
         refs = cat.references
 
         print refs[0].name
         cat2 = refs[0].follow()
 
 Get a list of datasets in this catalog
 
-.. code:: python
+.. code-block:: python
 
         data  = cat.datasets
 
 Get flat list of all direct datasets (data files) in the catalog
 
-.. code:: python
+.. code-block:: python
 
         datasets = cat.flat_datasets()
 
 Get flat list of all references in the catalog
 
-.. code:: python
+.. code-block:: python
 
         references = cat.flat_references()
 
 Crawl thredds catalog
 ---------------------
 
 Crawl recursive all direct datasets in catalog following the catalog
-references. Stop recusion at a given depth level.
+references. Stop recursion at a given depth level.
 
-.. code:: python
+.. code-block:: python
 
        import threddsclient
        for ds in threddsclient.crawl('http://example.com/thredds/catalog.xml', depth=2):
            print ds.name
 
 Development
 ===========
@@ -109,24 +131,26 @@
 Install sources
 ---------------
 
 Check out code from the birdy GitHub repo and start the installation:
 
 .. code-block:: sh
 
-   $ git clone https://github.com/bird-house/threddsclient.git
-   $ cd threddsclient
-   $ conda env create -f environment.yml
-   $ python setup.py develop
-
-Install additional dependencies::
-
-  $ conda install pytest flake8 sphinx bumpversion
-  OR
-  $ pip install -r requirements_dev.txt
+   git clone https://github.com/bird-house/threddsclient.git
+   cd threddsclient
+   conda env create -f environment.yml
+   python setup.py develop
+
+Install additional dependencies:
+
+.. code-block:: sh
+
+    conda install pytest flake8 sphinx bumpversion
+    # OR
+    pip install -r requirements_dev.txt
 
 Bump a new version
 ------------------
 
 Make a new version of Birdy in the following steps:
 
 * Make sure everything is commit to GitHub.
@@ -150,11 +174,15 @@
    :target: https://travis-ci.org/bird-house/threddsclient
 .. |Install with Conda| image:: https://anaconda.org/conda-forge/threddsclient/badges/installer/conda.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |License| image:: https://anaconda.org/conda-forge/threddsclient/badges/license.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |Join the Chat| image:: https://badges.gitter.im/bird-house/birdhouse.svg
    :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Version| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
+.. |Version-GitHub| image:: https://img.shields.io/github/v/release/bird-house/threddsclient?label=GitHub
+   :target: https://github.com/bird-house/threddsclient/releases
+.. |Version-Anaconda| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
    :target: https://anaconda.org/conda-forge/threddsclient
+.. |Version-PyPI| image:: https://img.shields.io/pypi/v/threddsclient?color=blue
+   :target: https://pypi.org/project/threddsclient/
 .. |Downloads| image:: https://anaconda.org/conda-forge/threddsclient/badges/downloads.svg
    :target: https://anaconda.org/conda-forge/threddsclient
```

### Comparing `threddsclient-0.4.3/setup.py` & `threddsclient-0.4.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,23 @@
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX',
+    'Operating System :: OS Independent',
     'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3 :: Only',
     'Topic :: Scientific/Engineering :: Atmospheric Science',
 ]
 
 setup(
     name='threddsclient',
     version=version,
     description='Thredds catalog client',
@@ -30,8 +38,9 @@
     author='Birdhouse',
     email='',
     license='Apache 2.0',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=reqs,
+    python_requires=">=3.7,<3.12",
 )
```

### Comparing `threddsclient-0.4.3/tests/test_birdhouse_sample.py` & `threddsclient-0.4.4/tests/test_birdhouse_sample.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/tests/test_catalog.py` & `threddsclient-0.4.4/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/tests/test_dataset.py` & `threddsclient-0.4.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/tests/test_noaa_sample.py` & `threddsclient-0.4.4/tests/test_noaa_sample.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/tests/test_online.py` & `threddsclient-0.4.4/tests/test_online.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pytest
 
 from threddsclient import read_url
 
 
 def test_noaa():
+    # 'http://www.esrl.noaa.gov/psd/thredds/catalog.xml'
+    # now directly redirects to 'https://psl.noaa.gov/thredds/catalog/catalog.xml'
+    # therefore the name and returned references changed as well
     cat = read_url('http://www.esrl.noaa.gov/psd/thredds/catalog.xml')
-    assert cat.name == 'THREDDS PSD Test Catalog'
+    assert cat.name == 'THREDDS PSL Catalog'
     assert cat.url == 'http://www.esrl.noaa.gov/psd/thredds/catalog.xml'
-    assert len(cat.references) == 2
-    cat2 = cat.references[0].follow()
+    assert len(cat.references) == 3
+    cat2 = cat.references[0]  # .follow()  # no need to follow anymore, since directly redirected
     assert cat2.name == 'Datasets'
-    assert cat2.url == 'http://www.esrl.noaa.gov/psd/thredds/catalog/Datasets/catalog.xml'
+    assert cat2.url == 'http://www.esrl.noaa.gov/thredds/catalog/Datasets/catalog.xml'
 
 
 # def test_utas_tpac():
 #     cat = read_url('http://portal.sf.utas.edu.au/thredds/catalog.xml')
 #     assert cat.name == 'TPAC Digital Library Data Server Catalog'
 #     assert cat.url == 'http://portal.sf.utas.edu.au/thredds/catalog.xml'
```

### Comparing `threddsclient-0.4.3/tests/test_utils.py` & `threddsclient-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/threddsclient/catalog.py` & `threddsclient-0.4.4/threddsclient/catalog.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/threddsclient/client.py` & `threddsclient-0.4.4/threddsclient/client.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/threddsclient/nodes.py` & `threddsclient-0.4.4/threddsclient/nodes.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/threddsclient/utils.py` & `threddsclient-0.4.4/threddsclient/utils.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.3/threddsclient.egg-info/PKG-INFO` & `threddsclient-0.4.4/threddsclient.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: threddsclient
-Version: 0.4.3
+Version: 0.4.4
 Summary: Thredds catalog client
 Author: Birdhouse
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Requires-Python: >=3.7,<3.12
 License-File: LICENCE.txt
 License-File: AUTHORS.rst
 
 =========================
 Thredds Client for Python
 =========================
 
@@ -22,102 +31,124 @@
 
 Installing Thredds Client
 =========================
 
 Anaconda
 --------
 
-|Version| |Downloads|
+|Version-GitHub| |Version-Anaconda| |Version-PyPI| |Downloads|
 
 Thredds client is available as Anaconda package. Install it with the
 following command:
 
-.. code:: bash
+.. code-block:: bash
 
-    $ conda install -c conda-forge threddsclient
+    conda install -c conda-forge threddsclient
 
-From github
+From PyPI
+---------
+
+Thredds Client is available from PyPI to install directly with ``pip`` or ``poetry``.
+
+.. code-block:: bash
+
+    pip install threddsclient
+
+
+.. code-block:: bash
+
+    poetry add threddsclient
+
+
+From GitHub
 -----------
 
 Check out code from the birdy GitHub repo and start the installation:
 
-.. code:: bash
+.. code-block:: bash
+
+    git clone https://github.com/bird-house/threddsclient.git
+    cd threddsclient
+    conda env create -f environment.yml
+    source activate threddsclient
+    python setup.py develop
+
+Alternatively, you can also install it directly with ``pip`` using a virtual environment of your choice:
+
+.. code-block:: bash
+
+    pip install "threddsclient @ git+https://github.com/bird-house/threddsclient.git"
 
-    $ git clone https://github.com/bird-house/threddsclient.git
-    $ cd threddsclient
-    $ conda env create -f environment.yml
-    $ source activate threddsclient
-    $ python setup.py develop
 
 Using Thredds Client
 ====================
 
 Read the Thredds tutorial on catalogs: `Thredds Catalog
 Primer <http://www.unidata.ucar.edu/software/thredds/current/tds/tutorial/CatalogPrimer.html>`__
 
 Get download URLs of a catalog
 ------------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.download_urls('http://example.com/thredds/catalog.xml')
 
 Get OpenDAP URLs of a catalog
 -----------------------------
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         urls = threddsclient.opendap_urls('http://example.com/thredds/catalog.xml')
 
 Navigate in catalog
 -------------------
 
 Start reading a catalog
 
-.. code:: python
+.. code-block:: python
 
         import threddsclient
         cat = threddsclient.read_url('http://example.com/thredds/catalog.xml')
 
 Get a list of references to other catalogs & follow them
 
-.. code:: python
+.. code-block:: python
 
         refs = cat.references
 
         print refs[0].name
         cat2 = refs[0].follow()
 
 Get a list of datasets in this catalog
 
-.. code:: python
+.. code-block:: python
 
         data  = cat.datasets
 
 Get flat list of all direct datasets (data files) in the catalog
 
-.. code:: python
+.. code-block:: python
 
         datasets = cat.flat_datasets()
 
 Get flat list of all references in the catalog
 
-.. code:: python
+.. code-block:: python
 
         references = cat.flat_references()
 
 Crawl thredds catalog
 ---------------------
 
 Crawl recursive all direct datasets in catalog following the catalog
-references. Stop recusion at a given depth level.
+references. Stop recursion at a given depth level.
 
-.. code:: python
+.. code-block:: python
 
        import threddsclient
        for ds in threddsclient.crawl('http://example.com/thredds/catalog.xml', depth=2):
            print ds.name
 
 Development
 ===========
@@ -125,24 +156,26 @@
 Install sources
 ---------------
 
 Check out code from the birdy GitHub repo and start the installation:
 
 .. code-block:: sh
 
-   $ git clone https://github.com/bird-house/threddsclient.git
-   $ cd threddsclient
-   $ conda env create -f environment.yml
-   $ python setup.py develop
-
-Install additional dependencies::
-
-  $ conda install pytest flake8 sphinx bumpversion
-  OR
-  $ pip install -r requirements_dev.txt
+   git clone https://github.com/bird-house/threddsclient.git
+   cd threddsclient
+   conda env create -f environment.yml
+   python setup.py develop
+
+Install additional dependencies:
+
+.. code-block:: sh
+
+    conda install pytest flake8 sphinx bumpversion
+    # OR
+    pip install -r requirements_dev.txt
 
 Bump a new version
 ------------------
 
 Make a new version of Birdy in the following steps:
 
 * Make sure everything is commit to GitHub.
@@ -166,97 +199,118 @@
    :target: https://travis-ci.org/bird-house/threddsclient
 .. |Install with Conda| image:: https://anaconda.org/conda-forge/threddsclient/badges/installer/conda.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |License| image:: https://anaconda.org/conda-forge/threddsclient/badges/license.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 .. |Join the Chat| image:: https://badges.gitter.im/bird-house/birdhouse.svg
    :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Version| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
+.. |Version-GitHub| image:: https://img.shields.io/github/v/release/bird-house/threddsclient?label=GitHub
+   :target: https://github.com/bird-house/threddsclient/releases
+.. |Version-Anaconda| image:: https://anaconda.org/conda-forge/threddsclient/badges/version.svg
    :target: https://anaconda.org/conda-forge/threddsclient
+.. |Version-PyPI| image:: https://img.shields.io/pypi/v/threddsclient?color=blue
+   :target: https://pypi.org/project/threddsclient/
 .. |Downloads| image:: https://anaconda.org/conda-forge/threddsclient/badges/downloads.svg
    :target: https://anaconda.org/conda-forge/threddsclient
 
 Authors
 =======
 
 *  Scott Wales scott.wales@unimelb.edu.au
 *  Carsten Ehbrecht ehbrecht@dkrz.de
 
 =======
 Changes
 =======
 
-0.4.3 (2023-05-31)
-==================
+`Unreleased <https://github.com/bird-house/threddsclient/tree/master>`_
+==========================================================================================
+
+* Nothing new for the moment.
+
+.. _changes_0.4.4:
+
+`0.4.4 <https://github.com/bird-house/threddsclient/tree/v0.4.4>`_ (2023-07-11)
+==========================================================================================
+
+* add shield badges for PyPI and GitHub releases
+* fix rendering of code blocks in ``README.rst``
+* add missing classifiers and python requirements to ``setup.py`` to allow validators to detect appropriate versions
+* add python 3.9, 3.10 and 3.11 to the supported versions in ``setup.py`` and validate them in GitHub CI
+* drop Travis CI configuration in favor of GitHub CI
+* fix ``test_noaa`` with the target THREDDS server responding differently than originally tested
+
+`0.4.3 <https://github.com/bird-house/threddsclient/tree/v0.4.3>`_ (2023-05-31)
+==========================================================================================
 
 * fix xml parsing for recent versions
 
-0.4.2 (2019-11-20)
-==================
+`0.4.2 <https://github.com/bird-house/threddsclient/tree/v0.4.2>`_ (2019-11-20)
+==========================================================================================
 
 * fixed conda links in Readme.
 
-0.4.1 (2019-11-06)
-==================
+`0.4.1 <https://github.com/bird-house/threddsclient/tree/v0.4.1>`_ (2019-11-06)
+==========================================================================================
 
 * fixed docs formatting.
 
-0.4.0 (2019-11-06)
-==================
+`0.4.0 <https://github.com/bird-house/threddsclient/tree/v0.4.0>`_ (2019-11-06)
+==========================================================================================
 
 * drop Python 2.7 (#5)
 * fix pip install (#4)
 
-0.3.5 (2018-10-05)
-==================
+`0.3.5 <https://github.com/bird-house/threddsclient/tree/v0.3.5>`_ (2018-10-05)
+==========================================================================================
 
 * support for Python 3.x (#1)
 
-0.3.4 (2015-10-25)
-==================
+`0.3.4 <https://github.com/bird-house/threddsclient/tree/v0.3.4>`_ (2015-10-25)
+==========================================================================================
 
 * fixed travis build/tests
 * updated docs
 
 0.3.3 (2015-10-24)
-==================
+==========================================================================================
 
 * converted docs to rst.
 * MANIFEST.in added.
 
 0.3.2 (2015-07-15)
-==================
+==========================================================================================
 
 *  append catalog.xml to catalog url if missing
 *  crawl method added
 
 0.3.1 (2015-06-14)
-==================
+==========================================================================================
 
 *  fixed catalog.follow()
 *  using dataset.download_url()
 *  added ipython example
 *  cleaned up Readme
 
 0.3.0 (2015-06-13)
-==================
+==========================================================================================
 
 *  Refactored
 *  added catalog.opendap_urls()
 
 0.2.0 (2015-06-08)
-==================
+==========================================================================================
 
 *  Refactored
 *  using CollectionDataset
 *  added catalog.download_urls()
 
 0.1.1 (2015-06-05)
-==================
+==========================================================================================
 
 *  Fixed catalog generation.
 *  added pytest dependency.
 
 0.1.0 (2015-03-13)
-==================
+==========================================================================================
 
 *  Version by https://github.com/ScottWales/threddsclient.
```

### Comparing `threddsclient-0.4.3/threddsclient.egg-info/SOURCES.txt` & `threddsclient-0.4.4/threddsclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

