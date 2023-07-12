# Comparing `tmp/scutls-0.3.0.tar.gz` & `tmp/scutls-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.3.0.tar", max compression
+gzip compressed data, was "scutls-0.3.1.tar", max compression
```

## Comparing `scutls-0.3.0.tar` & `scutls-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      601 2023-07-08 04:36:59.598732 scutls-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-08 04:37:16.305738 scutls-0.3.0/scutls/__init__.py
--rw-r--r--   0        0        0     7561 2023-07-08 04:25:06.015042 scutls-0.3.0/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.0/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.0/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.0/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.0/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.0/scutls/bam.py
--rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.0/scutls/barcode.py
--rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.0/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.0/scutls/download.py
--rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.0/scutls/fastq.py
--rw-r--r--   0        0        0    14058 2023-07-08 03:33:01.924697 scutls-0.3.0/scutls/util.py
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.0/setup.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-07-12 18:14:59.152132 scutls-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-12 18:15:20.548026 scutls-0.3.1/scutls/__init__.py
+-rw-r--r--   0        0        0     7560 2023-07-12 14:28:04.640198 scutls-0.3.1/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.1/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.1/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.1/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.1/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.1/scutls/bam.py
+-rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.1/scutls/barcode.py
+-rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.1/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.1/scutls/download.py
+-rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.1/scutls/fastq.py
+-rw-r--r--   0        0        0    14108 2023-07-12 18:14:00.283583 scutls-0.3.1/scutls/util.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.1/setup.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.1/PKG-INFO
```

### Comparing `scutls-0.3.0/pyproject.toml` & `scutls-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.3.0"
+version = "0.3.1"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.3.0/scutls/arguments.py` & `scutls-0.3.1/scutls/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from argparse import ArgumentParser
 from scutls import cli
 from scutls.__init__ import __version__
 
-parser = ArgumentParser(description = "Single-cell sequencing utility tools")
+parser = ArgumentParser(description = "Single-cell sequencing utility tool")
 parser.add_argument("-v", "--version", action="version", version="%(prog)s " + str(__version__))
 
 subparsers = parser.add_subparsers(title = "Subcommands")
 
 # subcommand: download
 parser_download = subparsers.add_parser(
     "download", description = "download genome/annotation file from UCSC/ENSEMBL")
```

### Comparing `scutls-0.3.0/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.3.1/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.3.1/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/assets/genome_ucsc.json` & `scutls-0.3.1/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/bam.py` & `scutls-0.3.1/scutls/bam.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/barcode.py` & `scutls-0.3.1/scutls/barcode.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/cli.py` & `scutls-0.3.1/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/download.py` & `scutls-0.3.1/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/fastq.py` & `scutls-0.3.1/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.0/scutls/util.py` & `scutls-0.3.1/scutls/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     _open = partial(gzip.open, mode='rt') if encoding == 'gzip' else open
     return(_open(filename))
 # _open_out function that can handle SeqIO writing to gz or fastq
 def _open_out(filename):
     encoding = guess_type(filename)[1]
     _open_out = partial(gzip.open, mode='wt') if encoding == 'gzip' else open
     return(_open_out(filename))
-    
+
 # find the closing number for chunking fastq file
 def closest_number(n, m):
     """
     Find the closest number to n that is no less than n and also divisible by m.
     Ref: https://www.geeksforgeeks.org/find-number-closest-n-divisible-m/
     """
     q = int(n / m)
@@ -172,17 +172,20 @@
         if n1 < n:
             n1 += m
         return n1
     if n2 < n:
         n2 += m
     return n2
 
-# ensure chunk_size is a fold of 4
 def chunks(lst, n):
     """Yield successive n-sized chunks from lst."""
+    # handle edge case: zero lst
+    if len(lst) == 0:
+        return(lst)
+    
     for i in range(0, len(lst), n):
         yield lst[i:i + n]
 
 # obtain the chunk intervals for given fastq and nproc
 def fastq_chunk_interval(fastq, nproc = 1):
     with _open(fastq) as f:
         n1 = sum(1 for record in SeqIO.parse(f, "fastq"))
@@ -298,14 +301,15 @@
 # obtain bam chunk intervals for multiprocessing
 def bam_chunk_interval(bam, nproc = 1):
     index_file_path = bam + '.bai'
     if not os.path.exists(index_file_path):
         pysam.index(bam)
     with pysam.AlignmentFile(bam, 'rb') as bam_file:
         n1 = sum(1 for alignment in bam_file)
+        
     chunk_size = math.ceil(n1 / nproc)
     intervals = list(chunks(range(0, n1), chunk_size))
     intervals = {i: intervals[i] for i in range(0, len(intervals))}
     return(intervals)
 
 # locate the read site position for given ref coordinate for each interval
 def bam_locate_pos_in_read(interval, bam, ref_coordinate):
```

### Comparing `scutls-0.3.0/setup.py` & `scutls-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.3.0/PKG-INFO` & `scutls-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.3.0
+Version: 0.3.1
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

