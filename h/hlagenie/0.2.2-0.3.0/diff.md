# Comparing `tmp/hlagenie-0.2.2.tar.gz` & `tmp/hlagenie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.2.2.tar", last modified: Fri Jul  7 19:50:36 2023, max compression
+gzip compressed data, was "hlagenie-0.3.0.tar", last modified: Wed Jul 12 19:43:28 2023, max compression
```

## Comparing `hlagenie-0.2.2.tar` & `hlagenie-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 19:50:26.000000 hlagenie-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 19:50:26.000000 hlagenie-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 19:50:36.008402 hlagenie-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-07 19:50:26.000000 hlagenie-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 19:50:36.000000 hlagenie-0.2.2/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 19:50:26.000000 hlagenie-0.2.2/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 19:50:26.000000 hlagenie-0.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 19:50:26.000000 hlagenie-0.2.2/scripts/hlagenie
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 19:50:26.000000 hlagenie-0.2.2/scripts/hlagenie-match
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 19:50:36.008402 hlagenie-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 19:50:26.000000 hlagenie-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 19:43:17.000000 hlagenie-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 19:43:17.000000 hlagenie-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 19:43:28.228502 hlagenie-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-12 19:43:17.000000 hlagenie-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 19:43:17.000000 hlagenie-0.3.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 19:43:17.000000 hlagenie-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-12 19:43:17.000000 hlagenie-0.3.0/scripts/hlagenie
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-12 19:43:17.000000 hlagenie-0.3.0/scripts/hlagenie-match
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 19:43:28.232502 hlagenie-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-12 19:43:17.000000 hlagenie-0.3.0/setup.py
```

### Comparing `hlagenie-0.2.2/LICENSE` & `hlagenie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.2/PKG-INFO` & `hlagenie-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.2.2
+Version: 0.3.0
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
@@ -27,16 +27,16 @@
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
     - [Initialize `hlagenie`](#initialize-hlagenie)
-    - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
-    - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
+    - [Accessing sequence dictionaries for HLA alleles](#accessing-sequence-dictionaries-for-hla-alleles)
+    - [Retrieve amino acid or nucleotide position from mature protein sequence](#retrieve-amino-acid-or-nucleotide-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
@@ -92,33 +92,35 @@
 import hlagenie
 
 genie = hlagenie.init("3510", ungap = False)
 ```
 
 The first time an object is instantiated with a given IMGT/HLA database version, the package will download the appropriate MSF files from the IMGT/HLA GitHub repository and create a SQLite database in the `/tmp` folder.
 
-#### Accessing amino acid sequence dictionaries for HLA alleles
+#### Accessing sequence dictionaries for HLA alleles
 
-The `GENIE` object contains dictionaries of amino acid sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the amino acid sequences for the full or mature protein sequence dictionary.
+The `GENIE` object contains dictionaries of amino acid and nucleotide sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the genetic sequences.
 
 All of the keys are two-field alleles given the shared protein sequence of these alleles.
 
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
+genie.nuc_seqs # full nucleotide sequences
 ```
 
-#### Retrieve amino acid position from mature protein sequence
+#### Retrieve amino acid or nucleotide position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid (or nucleotide) position from a given HLA allele, you can use the `getAA` or `getNuc` functions. These functions are 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
 genie.getAA("A*01:01",1) # returns "G"
+genie.getNuc("A*01:01",1) # returns "A"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
 To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
```

### Comparing `hlagenie-0.2.2/README.md` & `hlagenie-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
     - [Initialize `hlagenie`](#initialize-hlagenie)
-    - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
-    - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
+    - [Accessing sequence dictionaries for HLA alleles](#accessing-sequence-dictionaries-for-hla-alleles)
+    - [Retrieve amino acid or nucleotide position from mature protein sequence](#retrieve-amino-acid-or-nucleotide-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
@@ -73,33 +73,35 @@
 import hlagenie
 
 genie = hlagenie.init("3510", ungap = False)
 ```
 
 The first time an object is instantiated with a given IMGT/HLA database version, the package will download the appropriate MSF files from the IMGT/HLA GitHub repository and create a SQLite database in the `/tmp` folder.
 
-#### Accessing amino acid sequence dictionaries for HLA alleles
+#### Accessing sequence dictionaries for HLA alleles
 
-The `GENIE` object contains dictionaries of amino acid sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the amino acid sequences for the full or mature protein sequence dictionary.
+The `GENIE` object contains dictionaries of amino acid and nucleotide sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the genetic sequences.
 
 All of the keys are two-field alleles given the shared protein sequence of these alleles.
 
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
+genie.nuc_seqs # full nucleotide sequences
 ```
 
-#### Retrieve amino acid position from mature protein sequence
+#### Retrieve amino acid or nucleotide position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid (or nucleotide) position from a given HLA allele, you can use the `getAA` or `getNuc` functions. These functions are 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
 genie.getAA("A*01:01",1) # returns "G"
+genie.getNuc("A*01:01",1) # returns "A"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
 To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
```

### Comparing `hlagenie-0.2.2/hlagenie/configs.py` & `hlagenie-0.3.0/hlagenie/configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,17 +56,21 @@
 }
 config["expression_chars"] = [
     "N",
     "Q",
     "L",
     "S",
 ]
+# TODO: rename gapped_tables to gapped_tables_prot
 config["gapped_tables"] = [f"{locus}_gapped" for locus in config["loci"]]
 config["gapped_mature_tables"] = [f"{locus}_gapped_mature" for locus in config["loci"]]
+# TODO: rename ungapped_tables to ungapped_tables_prot
 config["ungapped_tables"] = [f"{locus}_ungapped" for locus in config["loci"]]
 config["ungapped_mature_tables"] = [
     f"{locus}_ungapped_mature" for locus in config["loci"]
 ]
 config["completed_tables"] = [f"{locus}_completed" for locus in config["loci"]]
 config["incomplete_tables"] = [f"{locus}_incomplete" for locus in config["loci"]]
 config["extended_tables"] = [f"{locus}_extended" for locus in config["loci"]]
+config["ungapped_nuc_tables"] = [f"{locus}_ungapped_nuc" for locus in config["loci"]]
+config["gapped_nuc_tables"] = [f"{locus}_gapped_nuc" for locus in config["loci"]]
 config["position_tables"] = [f"{locus}_position" for locus in config["loci"]]
```

### Comparing `hlagenie-0.2.2/hlagenie/data_repository.py` & `hlagenie-0.3.0/hlagenie/data_repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import functools
 import sqlite3
 import hlagenie.load
-from .load import load_sequence_alignment
+from .load import load_sequence_alignment, load_nucleotide_alignment
 from hlagenie.configs import config
 from hlagenie.smart_sort import smart_sort_comparator
 from . import db
 from .misc import find_gaps, regex_gen, coordinate, coordinate_end
 import pyard  # for HLA nomenclature
 
 
@@ -166,14 +166,143 @@
 
         # update overall dictionary
         ungapped_seqs.update(loc_seqs)
 
     return ungapped_seqs
 
 
+def generate_completed_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+    """
+    Create table with list of allele with completed sequences
+
+    :param db_conn: SQLite3 database connection object to HLAGenie database
+    :type db_conn: sqlite3.Connection
+    :param locus: HLA locus to generate completed table for
+    :type locus: str
+    :param seqs: dictionary of sequences
+    :type seqs: dict
+    :return: list of alleles with completed sequences
+    """
+
+    if db.table_exists(db_conn, f"{locus}_completed"):
+        return db.load_set(db_conn, f"{locus}_completed", ("allele"))
+
+    # get the reference sequence
+    ref_allele = config["refseq"][locus]
+
+    # get the reference sequence
+    ref_seq = seqs[ref_allele]
+
+    # get the gaps in the reference sequence
+    gaps = set(find_gaps(ref_seq))
+
+    # get the sequences for the locus
+    loc_seqs = {
+        allele: seq for allele, seq in seqs.items() if allele.split("*")[0] == locus
+    }
+
+    # initialize list to store completed alleles
+    completed = [
+        allele for allele, seq in loc_seqs.items() if set(find_gaps(seq)) == gaps
+    ]
+
+    # remove null alleles
+    completed = [allele for allele in completed if not allele[-1].isalpha()]
+
+    # save the list to the database
+    db.save_set(db_conn, f"{locus}_completed", set(completed), ("allele"))
+
+    return completed
+
+
+def generate_incomplete_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+    """
+    Create table with list of allele with incomplete sequences
+
+    :param db_conn: SQLite3 database connection object to HLAGenie database
+    :type db_conn: sqlite3.Connection
+    :param locus: HLA locus to generate incomplete table for
+    :type locus: str
+    :param seqs: dictionary of sequences
+    :type seqs: dict
+    :return: list of alleles with incomplete sequences
+    """
+
+    if db.table_exists(db_conn, f"{locus}_incomplete"):
+        return db.load_set(db_conn, f"{locus}_incomplete", ("allele"))
+
+    # get the reference sequence
+    ref_allele = config["refseq"][locus]
+
+    # get the reference sequence
+    ref_seq = seqs[ref_allele]
+
+    # get the gaps in the reference sequence
+    gaps = len(find_gaps(ref_seq))
+
+    # limit to alleles in locus
+    loc_seqs = {
+        allele: seq for allele, seq in seqs.items() if allele.split("*")[0] == locus
+    }
+
+    # initialize list to store incomplete alleles
+    incomplete = [
+        allele for allele, seq in loc_seqs.items() if len(find_gaps(seq)) > gaps
+    ]
+
+    # remove null alleles
+    incomplete = [allele for allele in incomplete if not allele[-1].isalpha()]
+
+    # save the list to the database
+    db.save_set(db_conn, f"{locus}_incomplete", set(incomplete), ("allele"))
+
+    return incomplete
+
+
+def generate_extended_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+    """
+    Create table with list of allele with extended sequences
+
+    :param db_conn: SQLite3 database connection object to HLAGenie database
+    :type db_conn: sqlite3.Connection
+    :param locus: HLA locus to generate extended table for
+    :type locus: str
+    :param seqs: dictionary of sequences
+    :type seqs: dict
+    :return: list of alleles with extended sequences
+    """
+
+    if db.table_exists(db_conn, f"{locus}_extended"):
+        return db.load_set(db_conn, f"{locus}_extended", ("allele"))
+
+    # get the reference sequence
+    ref_allele = config["refseq"][locus]
+
+    # get the reference sequence
+    ref_seq = seqs[ref_allele]
+
+    # get the gaps in the reference sequence
+    gaps = len(find_gaps(ref_seq))
+
+    # limit to alleles in locus
+    loc_seqs = {
+        allele: seq for allele, seq in seqs.items() if allele.split("*")[0] == locus
+    }
+
+    # initialize list to store extended alleles
+    extended = [
+        allele for allele, seq in loc_seqs.items() if len(find_gaps(seq)) < gaps
+    ]
+
+    # save the list to the database
+    db.save_set(db_conn, f"{locus}_extended", set(extended), ("allele"))
+
+    return extended
+
+
 def generate_ungapped_mature_tables(db_conn: sqlite3.Connection):
     """
     Create tables with ungapped mature sequences for every allele in the IMGT/HLA database for each locus
 
     :return: dictionary of ungapped mature sequences
     """
 
@@ -380,7 +509,117 @@
         # add to dictionary
         xrd_ends[locus] = int(end_coords)
 
     # save the dictionary to the database
     db.save_dict(db_conn, "ungapped_xrd", xrd_ends, ("locus", "xrd_end"))
 
     return xrd_ends
+
+
+def generate_ungapped_nuc_tables(db_conn: sqlite3.Connection, imgt_version):
+    """Generate a table with ungapped nucleotide sequences for every locus
+
+    :param db_conn: The database connection object
+    :type db_conn: sqlite3.Connection
+    :return: dictionary of ungapped nucleotide sequences
+    """
+    # check if the tables exist so as to not rebuild if unnecessary
+    if db.tables_exist(db_conn, config["ungapped_nuc_tables"]):
+        return db.load_ungapped_nuc_tables(db_conn)
+
+    # initialize pyard object
+    ard = pyard.init(imgt_version)
+
+    # initialize the dictionary to store all sequences
+    ungapped_seqs = {}
+
+    # retrieve multiple sequence alignment for each locus
+    for locus in config["loci"]:
+        # load the nucleotide sequence alignment
+        multi_seq = load_nucleotide_alignment(imgt_version, locus)
+
+        # get the reference sequence
+        ref_allele = config["refseq"][locus]
+        for record in multi_seq:
+            if ard.redux(record.id, "U2") == ref_allele:
+                ref_seq = str(record.seq)
+                break
+
+        # get the gaps in the reference sequence
+        gaps = find_gaps(ref_seq)
+
+        # turn the sequence alignment into a dictionary
+
+        ## initialize a per-locus dictionary
+        loc_seqs = {}
+
+        ## iterate through the sequence alignment
+        for record in multi_seq:
+            ### use py-ard to get two-field allele
+            allele = ard.redux(record.id, "U2")
+
+            ### only add allele if not already present to avoid overwriting with less complete sequence
+            if allele not in loc_seqs.keys():
+                #### remove gaps from the sequence (if actually a gap)
+                sequence = "".join(
+                    [
+                        char
+                        for i, char in enumerate(str(record.seq))
+                        if ((i not in gaps) or (char != "-"))
+                    ]
+                )
+
+                loc_seqs[allele] = sequence
+
+        # save the sequence alignment to the database
+        db.save_dict(db_conn, f"{locus}_ungapped_nuc", loc_seqs, ("allele", "seq"))
+
+        # update overall dictionary
+        ungapped_seqs.update(loc_seqs)
+
+    return ungapped_seqs
+
+
+def generate_gapped_nuc_tables(db_conn: sqlite3.Connection, imgt_version):
+    """
+    Create tables with gapped nucleotide sequences for every allele in the IMGT/HLA database for each locus
+
+    :param db_conn: The database connection object
+    :return: dictionary of gapped sequences
+    """
+
+    # check if the tables exist so as to not rebuild if unnecessary
+    if db.tables_exist(db_conn, config["gapped_nuc_tables"]):
+        return db.load_gapped_nuc_tables(db_conn)
+
+    # initialize pyard object
+    ard = pyard.init(imgt_version)
+
+    # initialize the dictionary to store all sequences
+    gapped_seqs = {}
+
+    # retrieve multiple sequence alignment for each locus
+    for locus in config["loci"]:
+        # load the sequence alignment
+        multi_seq = load_nucleotide_alignment(imgt_version, locus)
+
+        # turn the sequence alignment into a dictionary
+
+        ## initialize a per-locus dictionary
+        loc_seqs = {}
+
+        ## iterate through the sequence alignment
+        for record in multi_seq:
+            ### use py-ard to get two-field allele
+            allele = ard.redux(record.id, "U2")
+
+            ### only add allele if not already present to avoid overwriting with less complete sequence
+            if allele not in loc_seqs.keys():
+                loc_seqs[allele] = str(record.seq)
+
+        # save the sequence alignment to the database
+        db.save_dict(db_conn, f"{locus}_gapped_nuc", loc_seqs, ("allele", "seq"))
+
+        # update overall dictionary
+        gapped_seqs.update(loc_seqs)
+
+    return gapped_seqs
```

### Comparing `hlagenie-0.2.2/hlagenie/db.py` & `hlagenie-0.3.0/hlagenie/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,14 +228,15 @@
     cursor = connection.execute(query)
     # commit transaction - writes to the db
     connection.commit()
     # close the cursor
     cursor.close()
 
 
+# TODO: combine load_gapped_tables and load_gapped_nuc_tables
 def load_gapped_tables(connection: sqlite3.Connection):
     """
     Return a dictionary of gapped sequence tables
 
     :param connection: db connection of type sqlite.Connection
     :return: dict of gapped sequence tables
     """
@@ -248,14 +249,36 @@
         gapped_seqs.update(
             load_dict(connection, table_name=f"{loc}_gapped", columns=("allele", "seq"))
         )
 
     return gapped_seqs
 
 
+def load_gapped_nuc_tables(connection: sqlite3.Connection):
+    """
+    Return a dictionary of gapped nucleotide tables
+
+    :param connection: db connection of type sqlite.Connection
+    :return: dict of gapped sequence tables
+    """
+
+    # initialize dictionary to store allele:seq key:value pairs
+    gapped_seqs = {}
+
+    for loc in config["loci"]:
+        # extend the dictionary with each locus
+        gapped_seqs.update(
+            load_dict(
+                connection, table_name=f"{loc}_gapped_nuc", columns=("allele", "seq")
+            )
+        )
+
+    return gapped_seqs
+
+
 def load_gapped_mature_tables(connection: sqlite3.Connection):
     """
     Return a dictionary of gapped mature sequence tables
 
     :param connection: db connection of type sqlite.Connection
     :return: dict of gapped mature sequence tables
     """
@@ -270,14 +293,15 @@
                 connection, table_name=f"{loc}_gapped_mature", columns=("allele", "seq")
             )
         )
 
     return gapped_seqs
 
 
+# TODO: combine load_ungapped_tables and load_ungapped_nuc_tables
 def load_ungapped_tables(connection: sqlite3.Connection):
     """
     Return a dictionary of ungapped sequence tables
 
     :param connection: db connection of type sqlite.Connection
     :return: dict of ungapped sequence tables
     """
@@ -292,14 +316,36 @@
                 connection, table_name=f"{loc}_ungapped", columns=("allele", "seq")
             )
         )
 
     return ungapped_seqs
 
 
+def load_ungapped_nuc_tables(connection: sqlite3.Connection):
+    """
+    Return a dictionary of ungapped nucleotide tables
+
+    :param connection: db connection of type sqlite.Connection
+    :return: dict of ungapped sequence tables
+    """
+
+    # initialize dictionary to store allele:seq key:value pairs
+    ungapped_seqs = {}
+
+    for loc in config["loci"]:
+        # extend the dictionary with each locus
+        ungapped_seqs.update(
+            load_dict(
+                connection, table_name=f"{loc}_ungapped_nuc", columns=("allele", "seq")
+            )
+        )
+
+    return ungapped_seqs
+
+
 def load_ungapped_mature_tables(connection: sqlite3.Connection):
     """
     Return a dictionary of ungapped mature sequence tables
 
     :param connection: db connection of type sqlite.Connection
     :return: dict of ungapped mature sequence tables
     """
```

### Comparing `hlagenie-0.2.2/hlagenie/genie.py` & `hlagenie-0.3.0/hlagenie/genie.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
 
     def __init__(
         self,
         imgt_version: str = "Latest",
         data_dir: str = None,
         cache_size: int = config["DEFAULT_CACHE_SIZE"],
-        ungap=True,
+        ungap: bool = True,
     ):
         # set values for needed variables
         self._data_dir = data_dir
 
         # add an ard object
         self.ard = pyard.init(imgt_version)
 
@@ -33,75 +33,101 @@
         self.db_connection = db.create_db_connection(data_dir, imgt_version)
 
         # load sequence data from database
         if ungap:
             self.full_seqs = dr.generate_ungapped_tables(
                 self.db_connection, imgt_version
             )
+            self.nuc_seqs = dr.generate_ungapped_nuc_tables(
+                self.db_connection, imgt_version
+            )
             self.seqs = dr.generate_ungapped_mature_tables(self.db_connection)
             self.ards = dr.generate_ungapped_ard_table(self.db_connection, self.seqs)
             self.xrds = dr.generate_ungapped_xrd_table(self.db_connection, self.seqs)
         else:
             self.full_seqs = dr.generate_gapped_tables(self.db_connection, imgt_version)
+            self.nuc_seqs = dr.generate_gapped_nuc_tables(
+                self.db_connection, imgt_version
+            )
             self.seqs = dr.generate_gapped_mature_tables(self.db_connection)
             self.ards = dr.generate_gapped_ard_table(self.db_connection, self.seqs)
             self.xrds = dr.generate_gapped_xrd_table(self.db_connection, self.seqs)
 
-    def getAA(self, allele, position):
+    def getAA(self, allele: str, position: int):
         """
         Get the amino acid at a specific position in an allele
 
         :param allele: The allele to get the amino acid from
         :param position: The position to get the amino acid from
+        :return: The amino acid at the specified position
         """
 
         if allele.count(":") > 1:
             allele = self.ard.redux(allele, "U2")
 
         # get the amino acid at the specified position
         return self.seqs[allele][position - 1]
 
-    def getPeptide(self, allele, start, stop):
+    def getNuc(self, allele: str, position: int):
+        """Get the nucleotide at a specific position in an allele
+
+        :param allele: The allele to get the nucleotide from
+        :type allele: str
+        :param position: The position to get the nucleotide from
+        :type position: int
+        :return: The nucleotide at the specified position
+        """
+
+        if allele.count(":") > 1:
+            allele = self.ard.redux(allele, "U2")
+
+        # get the nucleotide at the specified position
+        return self.nuc_seqs[allele][position - 1]
+
+    def getPeptide(self, allele: str, start: int, stop: int):
         """
         Get the amino acid substring from a specified position to another specified position
 
         :param allele: The allele to get the amino acid substring from
         :param start: The position to start the substring
         :param stop: The position to end the substring
+        :return: The amino acid substring from the specified positions
         """
 
         if allele.count(":") > 1:
             allele = self.ard.redux(allele, "U2")
 
         # get the amino acid substring
         return self.seqs[allele][start - 1 : stop]
 
-    def getEpitope(self, allele, positions):
+    def getEpitope(self, allele: str, positions: list[int]):
         """
         Get the epitope string from a list of positions
 
         :param allele: The allele to get the epitope from
         :param positions: A list of positions to retrieve the epitope from
+        :return: The epitope string from the specified positions
         """
 
         if allele.count(":") > 1:
             allele = self.ard.redux(allele, "U2")
 
         # get the epitope string
         return "_".join(
             [f"{position}{self.seqs[allele][position-1]}" for position in positions]
         )
 
-    def isPositionMismatched(self, allele1, allele2, position):
+    def isPositionMismatched(self, allele1: str, allele2: str, position: int):
         """
         Check if two alleles have a mismatch at a specified position
 
         :param allele1: The first allele to check
         :param allele2: The second allele to check
         :param position: The position to check
+        :return: True if the alleles have a mismatch at the specified position, False otherwise
         """
 
         if allele1.count(":") > 1:
             allele1 = self.ard.redux(allele1, "U2")
         if allele2.count(":") > 1:
             allele2 = self.ard.redux(allele2, "U2")
 
@@ -109,24 +135,30 @@
         aa1 = self.getAA(allele1, position)
         aa2 = self.getAA(allele2, position)
 
         # check if the amino acids are the same
         return not (aa1 == aa2)
 
     def countAAMismatchesAllele(
-        self, allele1donor, allele2donor, allele1recip, allele2recip, position
+        self,
+        allele1donor: str,
+        allele2donor: str,
+        allele1recip: str,
+        allele2recip: str,
+        position: int,
     ):
         """
         Count the number of amino acid mismatches between two alleles at a specified position, adjusting for donor homozygosity
 
         :param allele1donor: The first allele of the donor to check
         :param allele2donor: The second allele of the donor to check
         :param allele1recip: The first allele of the recipient to check
         :param allele2recip: The second allele of the recipient to check
         :param position: The position to check
+        :return: The number of amino acid mismatches between the two alleles at the specified position
         """
         if allele1donor.count(":") > 1:
             allele1donor = self.ard.redux(allele1donor, "U2")
         if allele2donor.count(":") > 1:
             allele2donor = self.ard.redux(allele2donor, "U2")
         if allele1recip.count(":") > 1:
             allele1recip = self.ard.redux(allele1recip, "U2")
@@ -149,15 +181,17 @@
 
         # adjust if donor is homozygous, due to mismatch being same AA
         if (mm_count == 2) and (donor_homozygous):
             mm_count = 1
 
         return mm_count
 
-    def countAAMismatches(self, aa1_donor, aa2_donor, aa1_recip, aa2_recip):
+    def countAAMismatches(
+        self, aa1_donor: str, aa2_donor: str, aa1_recip: str, aa2_recip: str
+    ):
         """
         Count the number of amino acid mismatches at a position bewteen donor and recipient
 
         :param aa1_donor: The first amino acid of the donor to check
         :param aa2_donor: The second amino acid of the donor to check
         :param aa1_recip: The first amino acid of the recipient to check
         :param aa2_recip: The second amino acid of the recipient to check
@@ -169,15 +203,15 @@
         if (aa1_donor != aa1_recip) and (aa1_donor != aa2_recip):
             mm_count += 1
         if (aa2_donor != aa2_recip) and (aa2_donor != aa1_recip):
             mm_count += 1
 
         return mm_count
 
-    def getARD(self, allele):
+    def getARD(self, allele: str):
         """
         Get the ARD sequence of an allele
 
         :param allele: The allele to get the ARD sequence from
         :return: The ARD sequence
         """
 
@@ -187,15 +221,15 @@
 
         # get locus
         locus = allele.split("*")[0]
 
         # get the ARD sequence
         return self.seqs[allele][: self.ards[locus]]
 
-    def getXRD(self, allele):
+    def getXRD(self, allele: str):
         """
         Get the XRD sequence of an allele
 
         :param allele: The allele to get the XRD sequence from
         :return: The XRD sequence
         """
 
@@ -204,7 +238,37 @@
             allele = self.ard.redux(allele, "U2")
 
         # get locus
         locus = allele.split("*")[0]
 
         # get the ARD sequence
         return self.seqs[allele][: self.xrds[locus]]
+
+    def listIncompletes(self, locus: str):
+        """
+        List the incomplete alleles in the database
+
+        :param locus: The locus to list the incomplete alleles from
+        :return: A list of incomplete alleles
+        """
+
+        return dr.generate_incomplete_table(self.db_connection, locus, self.seqs)
+
+    def listCompletes(self, locus: str):
+        """
+        List the complete alleles in the database
+
+        :param locus: The locus to list the complete alleles from
+        :return: A list of complete alleles
+        """
+
+        return dr.generate_completed_table(self.db_connection, locus, self.seqs)
+
+    def listExtendeds(self, locus: str):
+        """
+        List the extended alleles in the database
+
+        :param locus: The locus to list the extended alleles from
+        :return: A list of extended alleles
+        """
+
+        return dr.generate_extended_table(self.db_connection, locus, self.seqs)
```

### Comparing `hlagenie-0.2.2/hlagenie/load.py` & `hlagenie-0.3.0/hlagenie/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :param imgt_version: The version of the IMGT/HLA database to use
     :param loc: The HLA locus to retrieve the sequence alignment for
     :return: Bio.Align.MultipleSeqAlignment object
     """
     msf_p_url = f"{IMGT_HLA_URL}/{imgt_version}/msf/{loc}_prot.msf"
     try:
         # download the file data from the IMGT_HLA GitHub repository
-        request = requests.get(msf_p_url)
+        request = requests.get(msf_p_url, timeout=15)
 
         # create a Named Temporary File to store the file data
         tf = tempfile.NamedTemporaryFile()
 
         # write the file data to the Named Temporary File
         tf.write(request.content)
 
@@ -34,7 +34,39 @@
 
     except URLError as e:
         print(f"Error downloading {msf_p_url}", e, file=sys.stderr)
         sys.exit(1)
 
     # return the multiple sequence alignment object
     return multi_seq
+
+
+def load_nucleotide_alignment(imgt_version: str, loc: str):
+    """Retrieve nucleotide alignment from the IMGTHLA GitHub repository and store in a Named Temporary File until processed into the database
+
+    :param imgt_version: The version of the IMGT/HLA database to use
+    :param loc: The HLA locus to retrieve the sequence alignment for
+    :return: Bio.Align.MultipleSeqAlignment object
+    """
+    msf_n_url = f"{IMGT_HLA_URL}/{imgt_version}/msf/{loc}_nuc.msf"
+    try:
+        # download the file data from the IMGT_HLA GitHub repository
+        request = requests.get(msf_n_url, timeout=15)
+
+        # create a Named Temporary File to store the file data
+        tf = tempfile.NamedTemporaryFile()
+
+        # write the file data to the Named Temporary File
+        tf.write(request.content)
+
+        # read the data into a multiple sequence alignment object
+        multi_seq = AlignIO.read(tf.name, "msf")
+
+        # close the Named Temporary File, deleting it
+        tf.close()
+
+    except URLError as e:
+        print(f"Error downloading {msf_n_url}", e, file=sys.stderr)
+        sys.exit(1)
+
+    # return the multiple sequence alignment object
+    return multi_seq
```

### Comparing `hlagenie-0.2.2/hlagenie/misc.py` & `hlagenie-0.3.0/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.2/hlagenie/smart_sort.py` & `hlagenie-0.3.0/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.2/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.3.0/hlagenie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.2.2
+Version: 0.3.0
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
@@ -27,16 +27,16 @@
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
     - [Initialize `hlagenie`](#initialize-hlagenie)
-    - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
-    - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
+    - [Accessing sequence dictionaries for HLA alleles](#accessing-sequence-dictionaries-for-hla-alleles)
+    - [Retrieve amino acid or nucleotide position from mature protein sequence](#retrieve-amino-acid-or-nucleotide-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
@@ -92,33 +92,35 @@
 import hlagenie
 
 genie = hlagenie.init("3510", ungap = False)
 ```
 
 The first time an object is instantiated with a given IMGT/HLA database version, the package will download the appropriate MSF files from the IMGT/HLA GitHub repository and create a SQLite database in the `/tmp` folder.
 
-#### Accessing amino acid sequence dictionaries for HLA alleles
+#### Accessing sequence dictionaries for HLA alleles
 
-The `GENIE` object contains dictionaries of amino acid sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the amino acid sequences for the full or mature protein sequence dictionary.
+The `GENIE` object contains dictionaries of amino acid and nucleotide sequences for each HLA allele. The keys for the dictionaries are the HLA allele names. The values are the genetic sequences.
 
 All of the keys are two-field alleles given the shared protein sequence of these alleles.
 
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
+genie.nuc_seqs # full nucleotide sequences
 ```
 
-#### Retrieve amino acid position from mature protein sequence
+#### Retrieve amino acid or nucleotide position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid (or nucleotide) position from a given HLA allele, you can use the `getAA` or `getNuc` functions. These functions are 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
 genie.getAA("A*01:01",1) # returns "G"
+genie.getNuc("A*01:01",1) # returns "A"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
 To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
```

### Comparing `hlagenie-0.2.2/scripts/hlagenie` & `hlagenie-0.3.0/scripts/hlagenie`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.2/scripts/hlagenie-match` & `hlagenie-0.3.0/scripts/hlagenie-match`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.2/setup.py` & `hlagenie-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.2.2",
+    version="0.3.0",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
```

