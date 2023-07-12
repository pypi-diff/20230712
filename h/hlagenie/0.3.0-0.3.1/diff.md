# Comparing `tmp/hlagenie-0.3.0.tar.gz` & `tmp/hlagenie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.3.0.tar", last modified: Wed Jul 12 19:43:28 2023, max compression
+gzip compressed data, was "hlagenie-0.3.1.tar", last modified: Wed Jul 12 21:24:37 2023, max compression
```

## Comparing `hlagenie-0.3.0.tar` & `hlagenie-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 19:43:17.000000 hlagenie-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 19:43:17.000000 hlagenie-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 19:43:28.228502 hlagenie-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-12 19:43:17.000000 hlagenie-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 19:43:17.000000 hlagenie-0.3.0/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 19:43:28.000000 hlagenie-0.3.0/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 19:43:17.000000 hlagenie-0.3.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 19:43:17.000000 hlagenie-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:43:28.228502 hlagenie-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-12 19:43:17.000000 hlagenie-0.3.0/scripts/hlagenie
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-12 19:43:17.000000 hlagenie-0.3.0/scripts/hlagenie-match
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 19:43:28.232502 hlagenie-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-12 19:43:17.000000 hlagenie-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:24:37.831121 hlagenie-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 21:24:20.000000 hlagenie-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 21:24:20.000000 hlagenie-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 21:24:37.831121 hlagenie-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-12 21:24:20.000000 hlagenie-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:24:37.831121 hlagenie-0.3.1/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 21:24:20.000000 hlagenie-0.3.1/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:24:37.831121 hlagenie-0.3.1/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 21:24:37.000000 hlagenie-0.3.1/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 21:24:20.000000 hlagenie-0.3.1/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 21:24:20.000000 hlagenie-0.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:24:37.831121 hlagenie-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-12 21:24:20.000000 hlagenie-0.3.1/scripts/hlagenie
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-12 21:24:20.000000 hlagenie-0.3.1/scripts/hlagenie-match
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 21:24:37.831121 hlagenie-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-12 21:24:20.000000 hlagenie-0.3.1/setup.py
```

### Comparing `hlagenie-0.3.0/LICENSE` & `hlagenie-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/PKG-INFO` & `hlagenie-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hlagenie-0.3.0/README.md` & `hlagenie-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/hlagenie/configs.py` & `hlagenie-0.3.1/hlagenie/configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,13 +64,10 @@
 config["gapped_tables"] = [f"{locus}_gapped" for locus in config["loci"]]
 config["gapped_mature_tables"] = [f"{locus}_gapped_mature" for locus in config["loci"]]
 # TODO: rename ungapped_tables to ungapped_tables_prot
 config["ungapped_tables"] = [f"{locus}_ungapped" for locus in config["loci"]]
 config["ungapped_mature_tables"] = [
     f"{locus}_ungapped_mature" for locus in config["loci"]
 ]
-config["completed_tables"] = [f"{locus}_completed" for locus in config["loci"]]
-config["incomplete_tables"] = [f"{locus}_incomplete" for locus in config["loci"]]
-config["extended_tables"] = [f"{locus}_extended" for locus in config["loci"]]
 config["ungapped_nuc_tables"] = [f"{locus}_ungapped_nuc" for locus in config["loci"]]
 config["gapped_nuc_tables"] = [f"{locus}_gapped_nuc" for locus in config["loci"]]
 config["position_tables"] = [f"{locus}_position" for locus in config["loci"]]
```

### Comparing `hlagenie-0.3.0/hlagenie/data_repository.py` & `hlagenie-0.3.1/hlagenie/data_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -166,29 +166,33 @@
 
         # update overall dictionary
         ungapped_seqs.update(loc_seqs)
 
     return ungapped_seqs
 
 
-def generate_completed_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+def generate_completed_table(
+    db_conn: sqlite3.Connection, locus: str, seqtype: str, seqs: dict
+):
     """
     Create table with list of allele with completed sequences
 
     :param db_conn: SQLite3 database connection object to HLAGenie database
     :type db_conn: sqlite3.Connection
     :param locus: HLA locus to generate completed table for
     :type locus: str
+    :param seqtype: sequence type to generate completed table for
+    :type seqtype: str
     :param seqs: dictionary of sequences
     :type seqs: dict
     :return: list of alleles with completed sequences
     """
 
-    if db.table_exists(db_conn, f"{locus}_completed"):
-        return db.load_set(db_conn, f"{locus}_completed", ("allele"))
+    if db.table_exists(db_conn, f"{locus}_completed_{seqtype}"):
+        return db.load_set(db_conn, f"{locus}_completed_{seqtype}", ("allele"))
 
     # get the reference sequence
     ref_allele = config["refseq"][locus]
 
     # get the reference sequence
     ref_seq = seqs[ref_allele]
 
@@ -205,34 +209,38 @@
         allele for allele, seq in loc_seqs.items() if set(find_gaps(seq)) == gaps
     ]
 
     # remove null alleles
     completed = [allele for allele in completed if not allele[-1].isalpha()]
 
     # save the list to the database
-    db.save_set(db_conn, f"{locus}_completed", set(completed), ("allele"))
+    db.save_set(db_conn, f"{locus}_completed_{seqtype}", set(completed), ("allele"))
 
     return completed
 
 
-def generate_incomplete_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+def generate_incomplete_table(
+    db_conn: sqlite3.Connection, locus: str, seqtype: str, seqs: dict
+):
     """
     Create table with list of allele with incomplete sequences
 
     :param db_conn: SQLite3 database connection object to HLAGenie database
     :type db_conn: sqlite3.Connection
     :param locus: HLA locus to generate incomplete table for
     :type locus: str
+    :param seqtype: sequence type to generate incomplete table for
+    :type seqtype: str
     :param seqs: dictionary of sequences
     :type seqs: dict
     :return: list of alleles with incomplete sequences
     """
 
-    if db.table_exists(db_conn, f"{locus}_incomplete"):
-        return db.load_set(db_conn, f"{locus}_incomplete", ("allele"))
+    if db.table_exists(db_conn, f"{locus}_incomplete_{seqtype}"):
+        return db.load_set(db_conn, f"{locus}_incomplete_{seqtype}", ("allele"))
 
     # get the reference sequence
     ref_allele = config["refseq"][locus]
 
     # get the reference sequence
     ref_seq = seqs[ref_allele]
 
@@ -249,56 +257,69 @@
         allele for allele, seq in loc_seqs.items() if len(find_gaps(seq)) > gaps
     ]
 
     # remove null alleles
     incomplete = [allele for allele in incomplete if not allele[-1].isalpha()]
 
     # save the list to the database
-    db.save_set(db_conn, f"{locus}_incomplete", set(incomplete), ("allele"))
+    db.save_set(db_conn, f"{locus}_incomplete_{seqtype}", set(incomplete), ("allele"))
 
     return incomplete
 
 
-def generate_extended_table(db_conn: sqlite3.Connection, locus: str, seqs: dict):
+def generate_extended_table(
+    db_conn: sqlite3.Connection, locus: str, seqtype: str, ungap: bool, seqs: dict
+):
     """
     Create table with list of allele with extended sequences
 
     :param db_conn: SQLite3 database connection object to HLAGenie database
     :type db_conn: sqlite3.Connection
     :param locus: HLA locus to generate extended table for
     :type locus: str
+    :param seqtype: sequence type to generate extended table for
+    :type seqtype: str
+    :param ungap: whether ungapped sequences were used
+    :type ungap: bool
     :param seqs: dictionary of sequences
     :type seqs: dict
     :return: list of alleles with extended sequences
     """
 
-    if db.table_exists(db_conn, f"{locus}_extended"):
-        return db.load_set(db_conn, f"{locus}_extended", ("allele"))
+    if db.table_exists(db_conn, f"{locus}_extended_{seqtype}"):
+        return db.load_set(db_conn, f"{locus}_extended_{seqtype}", ("allele"))
 
     # get the reference sequence
     ref_allele = config["refseq"][locus]
 
     # get the reference sequence
     ref_seq = seqs[ref_allele]
 
-    # get the gaps in the reference sequence
-    gaps = len(find_gaps(ref_seq))
-
     # limit to alleles in locus
     loc_seqs = {
         allele: seq for allele, seq in seqs.items() if allele.split("*")[0] == locus
     }
 
-    # initialize list to store extended alleles
-    extended = [
-        allele for allele, seq in loc_seqs.items() if len(find_gaps(seq)) < gaps
-    ]
+    # check if ungap=True was used
+    if ungap:
+        # get the length of the reference sequence
+        ref_len = len(ref_seq)
+
+        # initialize list to store extended alleles
+        extended = [allele for allele, seq in loc_seqs.items() if len(seq) > ref_len]
+    else:
+        # get the gaps in the reference sequence
+        gaps = len(find_gaps(ref_seq))
+        # initialize list to store extended alleles
+        extended = [
+            allele for allele, seq in loc_seqs.items() if len(find_gaps(seq)) < gaps
+        ]
 
     # save the list to the database
-    db.save_set(db_conn, f"{locus}_extended", set(extended), ("allele"))
+    db.save_set(db_conn, f"{locus}_extended_{seqtype}", set(extended), ("allele"))
 
     return extended
 
 
 def generate_ungapped_mature_tables(db_conn: sqlite3.Connection):
     """
     Create tables with ungapped mature sequences for every allele in the IMGT/HLA database for each locus
```

### Comparing `hlagenie-0.3.0/hlagenie/db.py` & `hlagenie-0.3.1/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/hlagenie/genie.py` & `hlagenie-0.3.1/hlagenie/genie.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,23 +21,24 @@
         imgt_version: str = "Latest",
         data_dir: str = None,
         cache_size: int = config["DEFAULT_CACHE_SIZE"],
         ungap: bool = True,
     ):
         # set values for needed variables
         self._data_dir = data_dir
+        self.ungap = ungap
 
         # add an ard object
         self.ard = pyard.init(imgt_version)
 
         # create database connection to SQLite database
         self.db_connection = db.create_db_connection(data_dir, imgt_version)
 
         # load sequence data from database
-        if ungap:
+        if self.ungap:
             self.full_seqs = dr.generate_ungapped_tables(
                 self.db_connection, imgt_version
             )
             self.nuc_seqs = dr.generate_ungapped_nuc_tables(
                 self.db_connection, imgt_version
             )
             self.seqs = dr.generate_ungapped_mature_tables(self.db_connection)
@@ -239,36 +240,66 @@
 
         # get locus
         locus = allele.split("*")[0]
 
         # get the ARD sequence
         return self.seqs[allele][: self.xrds[locus]]
 
-    def listIncompletes(self, locus: str):
+    def listIncompletes(self, locus: str, seqtype: str = "prot"):
         """
         List the incomplete alleles in the database
 
         :param locus: The locus to list the incomplete alleles from
+        :param seqtype: The sequence type to list the incomplete alleles for (prot or nuc)
         :return: A list of incomplete alleles
         """
 
-        return dr.generate_incomplete_table(self.db_connection, locus, self.seqs)
+        if seqtype == "prot":
+            return dr.generate_incomplete_table(
+                self.db_connection, locus, seqtype, self.seqs
+            )
+        elif seqtype == "nuc":
+            return dr.generate_incomplete_table(
+                self.db_connection, locus, seqtype, self.nuc_seqs
+            )
+        else:
+            print("Invalid sequence type specified")
 
-    def listCompletes(self, locus: str):
+    def listCompletes(self, locus: str, seqtype: str = "prot"):
         """
         List the complete alleles in the database
 
         :param locus: The locus to list the complete alleles from
+        :param seqtype: The sequence type to list the complete alleles for (prot or nuc)
         :return: A list of complete alleles
         """
 
-        return dr.generate_completed_table(self.db_connection, locus, self.seqs)
+        if seqtype == "prot":
+            return dr.generate_completed_table(
+                self.db_connection, locus, seqtype, self.seqs
+            )
+        elif seqtype == "nuc":
+            return dr.generate_completed_table(
+                self.db_connection, locus, seqtype, self.nuc_seqs
+            )
+        else:
+            print("Invalid sequence type specified")
 
-    def listExtendeds(self, locus: str):
+    def listExtendeds(self, locus: str, seqtype: str = "prot"):
         """
         List the extended alleles in the database
 
         :param locus: The locus to list the extended alleles from
+        :param seqtype: The sequence type to list the extended alleles for (prot or nuc)
         :return: A list of extended alleles
         """
 
-        return dr.generate_extended_table(self.db_connection, locus, self.seqs)
+        if seqtype == "prot":
+            return dr.generate_extended_table(
+                self.db_connection, locus, seqtype, self.ungap, self.seqs
+            )
+        elif seqtype == "nuc":
+            return dr.generate_extended_table(
+                self.db_connection, locus, seqtype, self.ungap, self.nuc_seqs
+            )
+        else:
+            print("Invalid sequence type specified")
```

### Comparing `hlagenie-0.3.0/hlagenie/load.py` & `hlagenie-0.3.1/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/hlagenie/misc.py` & `hlagenie-0.3.1/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/hlagenie/smart_sort.py` & `hlagenie-0.3.1/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.3.1/hlagenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hlagenie-0.3.0/scripts/hlagenie` & `hlagenie-0.3.1/scripts/hlagenie`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/scripts/hlagenie-match` & `hlagenie-0.3.1/scripts/hlagenie-match`

 * *Files identical despite different names*

### Comparing `hlagenie-0.3.0/setup.py` & `hlagenie-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.3.0",
+    version="0.3.1",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
```

