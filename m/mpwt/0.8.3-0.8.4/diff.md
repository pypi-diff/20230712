# Comparing `tmp/mpwt-0.8.3.tar.gz` & `tmp/mpwt-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpwt-0.8.3.tar", last modified: Fri Jan 13 16:37:14 2023, max compression
+gzip compressed data, was "dist/mpwt-0.8.4.tar", last modified: Wed Jul 12 09:53:43 2023, max compression
```

## Comparing `mpwt-0.8.3.tar` & `mpwt-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:37:14.000000 mpwt-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    56659 2023-01-13 16:37:14.000000 mpwt-0.8.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    48064 2023-01-13 16:36:53.000000 mpwt-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt/
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13655 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24784 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/mpwt_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31319 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/pathologic_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17620 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/pwt_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12443 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/results_check.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22273 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/to_pathologic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11465 2023-01-13 16:36:53.000000 mpwt-0.8.3/mpwt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56659 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-13 16:37:14.000000 mpwt-0.8.3/mpwt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-13 16:37:14.000000 mpwt-0.8.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1896 2023-01-13 16:36:53.000000 mpwt-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:37:14.000000 mpwt-0.8.3/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2622 2023-01-13 16:36:53.000000 mpwt-0.8.3/test/test_mpwt_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-01-13 16:36:53.000000 mpwt-0.8.3/test/test_mpwt_pathway_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:53:43.000000 mpwt-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-12 09:53:43.000000 mpwt-0.8.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48050 2023-07-12 09:53:26.000000 mpwt-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:53:43.000000 mpwt-0.8.4/mpwt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13655 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24784 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/mpwt_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31787 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/pathologic_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17620 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/pwt_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12443 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/results_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22273 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/to_pathologic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11465 2023-07-12 09:53:26.000000 mpwt-0.8.4/mpwt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:53:43.000000 mpwt-0.8.4/mpwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 09:53:42.000000 mpwt-0.8.4/mpwt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-12 09:53:43.000000 mpwt-0.8.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1896 2023-07-12 09:53:26.000000 mpwt-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:53:43.000000 mpwt-0.8.4/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2622 2023-07-12 09:53:26.000000 mpwt-0.8.4/test/test_mpwt_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-07-12 09:53:26.000000 mpwt-0.8.4/test/test_mpwt_pathway_tools.py
```

### Comparing `mpwt-0.8.3/PKG-INFO` & `mpwt-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: mpwt
-Version: 0.8.3
+Version: 0.8.4
 Summary: Multiprocessing for Pathway Tools
 Home-page: https://github.com/AuReMe/mpwt
 Author: AuReMe
 License: GPLv3
 Description: .. image:: https://img.shields.io/pypi/v/mpwt.svg
             :target: https://pypi.python.org/pypi/mpwt
         
         .. image:: https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg
             :target: https://doi.org/10.7554/eLife.61968
         
-        .. image:: https://img.shields.io/badge/Pathway%20Tools-26.5-brightgreen
+        .. image:: https://img.shields.io/badge/Pathway%20Tools-27.0-brightgreen
             :target: https://bioinformatics.ai.sri.com/ptools/release-notes.html
         
         mpwt: Multiprocessing Pathway Tools
         ===================================
         
         mpwt is a python package for running Pathway Tools [PathwayToolsarXiv]_ on multiple genomes using multiprocessing. More precisely, it launches one PathoLogic [Karp2011]_ process for each organism (PathoLogic and Pathway Tools pathway prediction are described in this `blog entry <http://pathwaytools.blogspot.com/2020/10/how-does-metabolic-pathway-prediction.html>`__). This allows to increase the speed of draft metabolic network reconstruction when working on multiple organisms.
         
@@ -34,15 +34,15 @@
         
         Installation
         ------------
         
         Requirements
         ~~~~~~~~~~~~
         
-        mpwt needs at least **Python 3.6**. It has been tested on Ubuntu and macOS but it is not working on Windows.
+        mpwt needs at least **Python 3.7**. It has been tested on Ubuntu and macOS but it is not working on Windows.
         mpwt requires three python depedencies (`biopython <https://github.com/biopython/biopython>`__ , `chardet <https://github.com/chardet/chardet>`__ and `gffutils <https://github.com/daler/gffutils>`__) and **Pathway Tools**. For the multiprocessing, mpwt uses the `multiprocessing library of Python 3 <https://docs.python.org/3/library/multiprocessing.html>`__.
         
         You must have an environment where Pathway Tools is installed. Pathway Tools can be obtained `here <http://bioinformatics.ai.sri.com/ptools/>`__.
         
         Pathway Tools needs **Blast**, so it must be install on your system. Depending on your system, Pathway Tools needs a file named **.ncbirc** to locate Blast, for more informations look at `this page <http://bioinformatics.ai.sri.com/ptools/installation-guide/released/blast.html>`__.
         
         /!\\ For all OS, Pathway-Tools must be in ``$PATH``.
@@ -52,18 +52,18 @@
         Consider adding Pathway Tools in ``$PATH`` permanently by using the following command and then sourcing bashrc:
         
         .. code:: sh
         
             echo 'export PATH="$PATH:/your/install/directory/pathway-tools:"' >> ~/.bashrc
             source ~/.bashrc
         
-        If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/ArnaudBelcour/mpwt-docker>`__.
+        If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/AuReMe/mpwt-docker>`__.
         It is a dockerfile that will create a container with Pathway Tools, its dependencies and this package. You just need to give a Pathway Tools installer as input.
         
-        You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/ArnaudBelcour/mpwt-singularity>`__.
+        You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/AuReMe/mpwt-singularity>`__.
         More manipulations are required compared to Docker but with this you can create a Singularity image.
         
         Using pip
         ~~~~~~~~~
         
         .. code:: sh
```

### Comparing `mpwt-0.8.3/README.rst` & `mpwt-0.8.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. image:: https://img.shields.io/pypi/v/mpwt.svg
     :target: https://pypi.python.org/pypi/mpwt
 
 .. image:: https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg
     :target: https://doi.org/10.7554/eLife.61968
 
-.. image:: https://img.shields.io/badge/Pathway%20Tools-26.5-brightgreen
+.. image:: https://img.shields.io/badge/Pathway%20Tools-27.0-brightgreen
     :target: https://bioinformatics.ai.sri.com/ptools/release-notes.html
 
 mpwt: Multiprocessing Pathway Tools
 ===================================
 
 mpwt is a python package for running Pathway Tools [PathwayToolsarXiv]_ on multiple genomes using multiprocessing. More precisely, it launches one PathoLogic [Karp2011]_ process for each organism (PathoLogic and Pathway Tools pathway prediction are described in this `blog entry <http://pathwaytools.blogspot.com/2020/10/how-does-metabolic-pathway-prediction.html>`__). This allows to increase the speed of draft metabolic network reconstruction when working on multiple organisms.
 
@@ -27,15 +27,15 @@
 
 Installation
 ------------
 
 Requirements
 ~~~~~~~~~~~~
 
-mpwt needs at least **Python 3.6**. It has been tested on Ubuntu and macOS but it is not working on Windows.
+mpwt needs at least **Python 3.7**. It has been tested on Ubuntu and macOS but it is not working on Windows.
 mpwt requires three python depedencies (`biopython <https://github.com/biopython/biopython>`__ , `chardet <https://github.com/chardet/chardet>`__ and `gffutils <https://github.com/daler/gffutils>`__) and **Pathway Tools**. For the multiprocessing, mpwt uses the `multiprocessing library of Python 3 <https://docs.python.org/3/library/multiprocessing.html>`__.
 
 You must have an environment where Pathway Tools is installed. Pathway Tools can be obtained `here <http://bioinformatics.ai.sri.com/ptools/>`__.
 
 Pathway Tools needs **Blast**, so it must be install on your system. Depending on your system, Pathway Tools needs a file named **.ncbirc** to locate Blast, for more informations look at `this page <http://bioinformatics.ai.sri.com/ptools/installation-guide/released/blast.html>`__.
 
 /!\\ For all OS, Pathway-Tools must be in ``$PATH``.
@@ -45,18 +45,18 @@
 Consider adding Pathway Tools in ``$PATH`` permanently by using the following command and then sourcing bashrc:
 
 .. code:: sh
 
     echo 'export PATH="$PATH:/your/install/directory/pathway-tools:"' >> ~/.bashrc
     source ~/.bashrc
 
-If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/ArnaudBelcour/mpwt-docker>`__.
+If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/AuReMe/mpwt-docker>`__.
 It is a dockerfile that will create a container with Pathway Tools, its dependencies and this package. You just need to give a Pathway Tools installer as input.
 
-You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/ArnaudBelcour/mpwt-singularity>`__.
+You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/AuReMe/mpwt-singularity>`__.
 More manipulations are required compared to Docker but with this you can create a Singularity image.
 
 Using pip
 ~~~~~~~~~
 
 .. code:: sh
```

### Comparing `mpwt-0.8.3/mpwt/__init__.py` & `mpwt-0.8.4/mpwt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
 from mpwt.pwt_wrapper import run_pwt, run_pwt_flat
 from mpwt.mpwt_workflow import multiprocess_pwt
 from mpwt.utils import cleaning, cleaning_input, find_ptools_path, list_pgdb, pubmed_citations, remove_pgdbs
 from mpwt.to_pathologic import create_pathologic_file
 
-__version__='0.8.3'
+__version__='0.8.4'
```

### Comparing `mpwt-0.8.3/mpwt/__main__.py` & `mpwt-0.8.4/mpwt/__main__.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt/mpwt_workflow.py` & `mpwt-0.8.4/mpwt/mpwt_workflow.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt/pathologic_input.py` & `mpwt-0.8.4/mpwt/pathologic_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,26 +410,31 @@
             except StopIteration:
                 logger.critical('Issue with the genbank {0}, it can be empty or malformatted.'.format(input_path))
                 return None
 
             try:
                 species_name = first_seq_record.annotations['organism']
             except KeyError:
-                logger.critical('No organism in the Genbank {0} In the SOURCE you must have: ORGANISM  Species name'.format(pgdb_id))
+                logger.critical('No organism in the Genbank {0}. In field SOURCE, you must have: ORGANISM  Species name'.format(pgdb_id))
                 return None
 
             # Take the source feature of the first record.
             # This feature contains the taxon ID in the db_xref qualifier.
             src_features = [feature for feature in first_seq_record.features if feature.type == "source"]
-            for src_feature in src_features:
-                if 'db_xref' in src_feature.qualifiers:
-                    src_dbxref_qualifiers = src_feature.qualifiers['db_xref']
-                    for src_dbxref_qualifier in src_dbxref_qualifiers:
-                        if 'taxon:' in src_dbxref_qualifier:
-                            taxon_id = src_dbxref_qualifier.replace('taxon:', '')
+            if len(src_features) == 0:
+                logger.info('No FEATURES source in the Genbank {0}, you must have: /db_xref="taxon:taxonid" Where taxonid is the Id of your organism. You can find it on the NCBI.'.format(gbk_pathname))
+                logger.info('Try to look in the taxon_id.tsv file')
+                taxon_error, taxon_id, taxon_datas = extract_taxon_id(run_folder, pgdb_id, taxon_id, taxon_file)
+            else:
+                for src_feature in src_features:
+                    if 'db_xref' in src_feature.qualifiers:
+                        src_dbxref_qualifiers = src_feature.qualifiers['db_xref']
+                        for src_dbxref_qualifier in src_dbxref_qualifiers:
+                            if 'taxon:' in src_dbxref_qualifier:
+                                taxon_id = src_dbxref_qualifier.replace('taxon:', '')
                 if not taxon_id:
                     logger.info('No taxon ID in the Genbank {0} In the FEATURES source you must have: /db_xref="taxon:taxonid" Where taxonid is the Id of your organism. You can find it on the NCBI.'.format(gbk_pathname))
                     logger.info('Try to look in the taxon_id.tsv file')
                     taxon_error, taxon_id, taxon_datas = extract_taxon_id(run_folder, pgdb_id, taxon_id, taxon_file)
             if taxon_file:
                 taxon_error, taxon_id, taxon_datas = extract_taxon_id(run_folder, pgdb_id, taxon_id, taxon_file)
```

### Comparing `mpwt-0.8.3/mpwt/pwt_wrapper.py` & `mpwt-0.8.4/mpwt/pwt_wrapper.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt/results_check.py` & `mpwt-0.8.4/mpwt/results_check.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt/to_pathologic.py` & `mpwt-0.8.4/mpwt/to_pathologic.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt/utils.py` & `mpwt-0.8.4/mpwt/utils.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/mpwt.egg-info/PKG-INFO` & `mpwt-0.8.4/mpwt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: mpwt
-Version: 0.8.3
+Version: 0.8.4
 Summary: Multiprocessing for Pathway Tools
 Home-page: https://github.com/AuReMe/mpwt
 Author: AuReMe
 License: GPLv3
 Description: .. image:: https://img.shields.io/pypi/v/mpwt.svg
             :target: https://pypi.python.org/pypi/mpwt
         
         .. image:: https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg
             :target: https://doi.org/10.7554/eLife.61968
         
-        .. image:: https://img.shields.io/badge/Pathway%20Tools-26.5-brightgreen
+        .. image:: https://img.shields.io/badge/Pathway%20Tools-27.0-brightgreen
             :target: https://bioinformatics.ai.sri.com/ptools/release-notes.html
         
         mpwt: Multiprocessing Pathway Tools
         ===================================
         
         mpwt is a python package for running Pathway Tools [PathwayToolsarXiv]_ on multiple genomes using multiprocessing. More precisely, it launches one PathoLogic [Karp2011]_ process for each organism (PathoLogic and Pathway Tools pathway prediction are described in this `blog entry <http://pathwaytools.blogspot.com/2020/10/how-does-metabolic-pathway-prediction.html>`__). This allows to increase the speed of draft metabolic network reconstruction when working on multiple organisms.
         
@@ -34,15 +34,15 @@
         
         Installation
         ------------
         
         Requirements
         ~~~~~~~~~~~~
         
-        mpwt needs at least **Python 3.6**. It has been tested on Ubuntu and macOS but it is not working on Windows.
+        mpwt needs at least **Python 3.7**. It has been tested on Ubuntu and macOS but it is not working on Windows.
         mpwt requires three python depedencies (`biopython <https://github.com/biopython/biopython>`__ , `chardet <https://github.com/chardet/chardet>`__ and `gffutils <https://github.com/daler/gffutils>`__) and **Pathway Tools**. For the multiprocessing, mpwt uses the `multiprocessing library of Python 3 <https://docs.python.org/3/library/multiprocessing.html>`__.
         
         You must have an environment where Pathway Tools is installed. Pathway Tools can be obtained `here <http://bioinformatics.ai.sri.com/ptools/>`__.
         
         Pathway Tools needs **Blast**, so it must be install on your system. Depending on your system, Pathway Tools needs a file named **.ncbirc** to locate Blast, for more informations look at `this page <http://bioinformatics.ai.sri.com/ptools/installation-guide/released/blast.html>`__.
         
         /!\\ For all OS, Pathway-Tools must be in ``$PATH``.
@@ -52,18 +52,18 @@
         Consider adding Pathway Tools in ``$PATH`` permanently by using the following command and then sourcing bashrc:
         
         .. code:: sh
         
             echo 'export PATH="$PATH:/your/install/directory/pathway-tools:"' >> ~/.bashrc
             source ~/.bashrc
         
-        If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/ArnaudBelcour/mpwt-docker>`__.
+        If your OS doesn't support Pathway Tools, you can use a docker container. If it's your case, look at `Pathway Tools Multiprocessing Docker <https://github.com/AuReMe/mpwt-docker>`__.
         It is a dockerfile that will create a container with Pathway Tools, its dependencies and this package. You just need to give a Pathway Tools installer as input.
         
-        You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/ArnaudBelcour/mpwt-singularity>`__.
+        You can also look at `Pathway Tools Multiprocessing Singularity <https://github.com/AuReMe/mpwt-singularity>`__.
         More manipulations are required compared to Docker but with this you can create a Singularity image.
         
         Using pip
         ~~~~~~~~~
         
         .. code:: sh
```

### Comparing `mpwt-0.8.3/setup.py` & `mpwt-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/test/test_mpwt_functions.py` & `mpwt-0.8.4/test/test_mpwt_functions.py`

 * *Files identical despite different names*

### Comparing `mpwt-0.8.3/test/test_mpwt_pathway_tools.py` & `mpwt-0.8.4/test/test_mpwt_pathway_tools.py`

 * *Files identical despite different names*

