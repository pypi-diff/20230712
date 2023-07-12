# Comparing `tmp/iCount-Mini-3.0.0.tar.gz` & `tmp/iCount-Mini-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iCount-Mini-3.0.0.tar", last modified: Fri Jul  7 07:14:36 2023, max compression
+gzip compressed data, was "iCount-Mini-3.0.1.tar", last modified: Wed Jul 12 11:54:16 2023, max compression
```

## Comparing `iCount-Mini-3.0.0.tar` & `iCount-Mini-3.0.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.134516 iCount-Mini-3.0.0/
--rw-r--r--   0 capitac    (501) staff       (20)     9787 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/.pylintrc
--rw-r--r--   0 capitac    (501) staff       (20)     7715 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/CLA
--rw-r--r--   0 capitac    (501) staff       (20)     2181 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/Dockerfile
--rw-r--r--   0 capitac    (501) staff       (20)     1580 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/Dockerfile_test
--rw-r--r--   0 capitac    (501) staff       (20)     1145 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/LICENSE
--rw-r--r--   0 capitac    (501) staff       (20)      600 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/MANIFEST.in
--rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-07 07:14:36.134648 iCount-Mini-3.0.0/PKG-INFO
--rw-r--r--   0 capitac    (501) staff       (20)     2484 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/README.md
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.890162 iCount-Mini-3.0.0/docs/
--rw-r--r--   0 capitac    (501) staff       (20)     3267 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/Makefile
--rwxr-xr-x   0 capitac    (501) staff       (20)      559 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/changelog.sh
--rwxr-xr-x   0 capitac    (501) staff       (20)      200 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/pack_testupload.sh
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.953925 iCount-Mini-3.0.0/docs/source/
--rw-r--r--   0 capitac    (501) staff       (20)     1302 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/cite.rst
--rw-r--r--   0 capitac    (501) staff       (20)     5836 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/conf.py
--rw-r--r--   0 capitac    (501) staff       (20)    10629 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/contributing.rst
--rw-r--r--   0 capitac    (501) staff       (20)      520 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/faq.rst
--rw-r--r--   0 capitac    (501) staff       (20)      240 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/index.rst
--rw-r--r--   0 capitac    (501) staff       (20)     3071 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/installation.rst
--rw-r--r--   0 capitac    (501) staff       (20)       78 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/license.rst
--rw-r--r--   0 capitac    (501) staff       (20)       86 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref.rst
--rw-r--r--   0 capitac    (501) staff       (20)       99 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref_CLI.rst
--rw-r--r--   0 capitac    (501) staff       (20)    39672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/docs/source/ref_CLI.txt
--rw-r--r--   0 capitac    (501) staff       (20)      565 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref_python.rst
--rw-r--r--   0 capitac    (501) staff       (20)       55 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/revisions.rst
--rw-r--r--   0 capitac    (501) staff       (20)    12384 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/tutorial.rst
--rw-r--r--   0 capitac    (501) staff       (20)       92 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/versions.rst
--rw-r--r--   0 capitac    (501) staff       (20)      230 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/testdownload_install.sh
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.969457 iCount-Mini-3.0.0/iCount/
--rw-r--r--   0 capitac    (501) staff       (20)      836 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/iCount/__about__.py
--rw-r--r--   0 capitac    (501) staff       (20)     2281 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/__init__.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.993350 iCount-Mini-3.0.0/iCount/analysis/
--rw-r--r--   0 capitac    (501) staff       (20)      638 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/analysis/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)     4092 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/annotate.py
--rw-r--r--   0 capitac    (501) staff       (20)      346 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/group.py
--rw-r--r--   0 capitac    (501) staff       (20)    40612 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/kmers.py
--rw-r--r--   0 capitac    (501) staff       (20)    10210 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/analysis/metagene.py
--rw-r--r--   0 capitac    (501) staff       (20)     4252 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/peaks.py
--rw-r--r--   0 capitac    (501) staff       (20)    22815 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/sigxls.py
--rw-r--r--   0 capitac    (501) staff       (20)     5385 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/summary.py
--rwxr-xr-x   0 capitac    (501) staff       (20)    18226 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/cli.py
--rw-r--r--   0 capitac    (501) staff       (20)    11127 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/demultiplex.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.014030 iCount-Mini-3.0.0/iCount/examples/
--rw-r--r--   0 capitac    (501) staff       (20)     1709 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/__init__.py
--rwxr-xr-x   0 capitac    (501) staff       (20)     3310 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/hnRNPC.sh
--rwxr-xr-x   0 capitac    (501) staff       (20)     3348 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/hnRNPC_reduced.sh
--rwxr-xr-x   0 capitac    (501) staff       (20)     1962 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/tutorial.sh
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.025751 iCount-Mini-3.0.0/iCount/externals/
--rw-r--r--   0 capitac    (501) staff       (20)      324 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)     2941 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/cutadapt.py
--rw-r--r--   0 capitac    (501) staff       (20)     7465 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/star.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.038664 iCount-Mini-3.0.0/iCount/files/
--rw-r--r--   0 capitac    (501) staff       (20)     3781 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)     3591 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/bed.py
--rw-r--r--   0 capitac    (501) staff       (20)     3183 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/bedgraph.py
--rw-r--r--   0 capitac    (501) staff       (20)      762 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/fasta.py
--rw-r--r--   0 capitac    (501) staff       (20)     3221 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/fastq.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.049187 iCount-Mini-3.0.0/iCount/genomes/
--rw-r--r--   0 capitac    (501) staff       (20)     5143 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)    10859 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/ensembl.py
--rw-r--r--   0 capitac    (501) staff       (20)     7089 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/gencode.py
--rw-r--r--   0 capitac    (501) staff       (20)    40516 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/genomes/segment.py
--rw-r--r--   0 capitac    (501) staff       (20)     6994 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/logger.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.058885 iCount-Mini-3.0.0/iCount/mapping/
--rw-r--r--   0 capitac    (501) staff       (20)      377 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)      925 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/filters.py
--rw-r--r--   0 capitac    (501) staff       (20)      197 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/indexstar.py
--rw-r--r--   0 capitac    (501) staff       (20)      218 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/mapstar.py
--rw-r--r--   0 capitac    (501) staff       (20)    22429 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/xlsites.py
--rw-r--r--   0 capitac    (501) staff       (20)     1558 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/metrics.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.067181 iCount-Mini-3.0.0/iCount/plotting/
--rw-r--r--   0 capitac    (501) staff       (20)      160 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)     2204 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_combined.py
--rw-r--r--   0 capitac    (501) staff       (20)     4460 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_metagene.py
--rw-r--r--   0 capitac    (501) staff       (20)     5435 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_rnaheatmap.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.112433 iCount-Mini-3.0.0/iCount/tests/
--rw-r--r--   0 capitac    (501) staff       (20)       20 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/__init__.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.126426 iCount-Mini-3.0.0/iCount/tests/functional/
--rw-r--r--   0 capitac    (501) staff       (20)      367 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/__init__.py
--rw-r--r--   0 capitac    (501) staff       (20)     9158 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/gtf_variations.py
--rw-r--r--   0 capitac    (501) staff       (20)    29055 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt
--rw-r--r--   0 capitac    (501) staff       (20)     3308 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.py
--rw-r--r--   0 capitac    (501) staff       (20)      278 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/segments_count.out.txt
--rw-r--r--   0 capitac    (501) staff       (20)     4366 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/segments_count.py
--rw-r--r--   0 capitac    (501) staff       (20)     6912 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_annotate.py
--rw-r--r--   0 capitac    (501) staff       (20)     2696 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_bed.py
--rw-r--r--   0 capitac    (501) staff       (20)    16194 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_cli.py
--rw-r--r--   0 capitac    (501) staff       (20)     2580 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_clusters.py
--rw-r--r--   0 capitac    (501) staff       (20)     1081 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_data.py
--rw-r--r--   0 capitac    (501) staff       (20)    14672 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_demultiplex.py
--rw-r--r--   0 capitac    (501) staff       (20)     6817 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_e2e.py
--rw-r--r--   0 capitac    (501) staff       (20)     1012 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_examples.py
--rw-r--r--   0 capitac    (501) staff       (20)     4604 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_externals.py
--rw-r--r--   0 capitac    (501) staff       (20)     9046 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_files.py
--rw-r--r--   0 capitac    (501) staff       (20)    10194 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_genomes.py
--rw-r--r--   0 capitac    (501) staff       (20)     4109 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_peaks.py
--rw-r--r--   0 capitac    (501) staff       (20)     3672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_plotting.py
--rw-r--r--   0 capitac    (501) staff       (20)     9700 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_rnamaps.py
--rw-r--r--   0 capitac    (501) staff       (20)    42560 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_segment.py
--rw-r--r--   0 capitac    (501) staff       (20)     6056 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_summary.py
--rw-r--r--   0 capitac    (501) staff       (20)    14112 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_xlsites.py
--rw-r--r--   0 capitac    (501) staff       (20)    11519 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/utils.py
-drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.134316 iCount-Mini-3.0.0/iCount_Mini.egg-info/
--rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/PKG-INFO
--rw-r--r--   0 capitac    (501) staff       (20)     2564 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/SOURCES.txt
--rw-r--r--   0 capitac    (501) staff       (20)        1 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/dependency_links.txt
--rw-r--r--   0 capitac    (501) staff       (20)       48 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/entry_points.txt
--rw-r--r--   0 capitac    (501) staff       (20)      266 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/requires.txt
--rw-r--r--   0 capitac    (501) staff       (20)        7 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/top_level.txt
--rw-r--r--   0 capitac    (501) staff       (20)      111 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/requirements-rtd.txt
--rw-r--r--   0 capitac    (501) staff       (20)      242 2023-07-07 07:14:36.136873 iCount-Mini-3.0.0/setup.cfg
--rwxr-xr-x   0 capitac    (501) staff       (20)     2546 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/setup.py
--rw-r--r--   0 capitac    (501) staff       (20)     1108 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/tox.ini
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.542661 iCount-Mini-3.0.1/
+-rw-r--r--   0 capitac    (501) staff       (20)     9787 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/.pylintrc
+-rw-r--r--   0 capitac    (501) staff       (20)     7715 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/CLA
+-rw-r--r--   0 capitac    (501) staff       (20)     2181 2023-07-07 07:08:15.000000 iCount-Mini-3.0.1/Dockerfile
+-rw-r--r--   0 capitac    (501) staff       (20)     1580 2023-07-07 07:08:15.000000 iCount-Mini-3.0.1/Dockerfile_test
+-rw-r--r--   0 capitac    (501) staff       (20)     1145 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/LICENSE
+-rw-r--r--   0 capitac    (501) staff       (20)      600 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/MANIFEST.in
+-rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-12 11:54:16.542789 iCount-Mini-3.0.1/PKG-INFO
+-rw-r--r--   0 capitac    (501) staff       (20)     2484 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/README.md
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.410526 iCount-Mini-3.0.1/docs/
+-rw-r--r--   0 capitac    (501) staff       (20)     3267 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/Makefile
+-rwxr-xr-x   0 capitac    (501) staff       (20)      559 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/changelog.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)      200 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/pack_testupload.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.476270 iCount-Mini-3.0.1/docs/source/
+-rw-r--r--   0 capitac    (501) staff       (20)     1302 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/cite.rst
+-rw-r--r--   0 capitac    (501) staff       (20)     5836 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/conf.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10629 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/contributing.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      520 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/faq.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      240 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/index.rst
+-rw-r--r--   0 capitac    (501) staff       (20)     3071 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/installation.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       78 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/license.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       86 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/ref.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       99 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/ref_CLI.rst
+-rw-r--r--   0 capitac    (501) staff       (20)    39672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/docs/source/ref_CLI.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      565 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/ref_python.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       55 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/revisions.rst
+-rw-r--r--   0 capitac    (501) staff       (20)    12384 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/tutorial.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       92 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/source/versions.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      230 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/docs/testdownload_install.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.478658 iCount-Mini-3.0.1/iCount/
+-rw-r--r--   0 capitac    (501) staff       (20)      836 2023-07-12 11:46:01.000000 iCount-Mini-3.0.1/iCount/__about__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2281 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/__init__.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.488994 iCount-Mini-3.0.1/iCount/analysis/
+-rw-r--r--   0 capitac    (501) staff       (20)      638 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/analysis/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4092 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/annotate.py
+-rw-r--r--   0 capitac    (501) staff       (20)      346 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/group.py
+-rw-r--r--   0 capitac    (501) staff       (20)    40612 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/kmers.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10210 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/analysis/metagene.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4252 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/peaks.py
+-rw-r--r--   0 capitac    (501) staff       (20)    22815 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/sigxls.py
+-rw-r--r--   0 capitac    (501) staff       (20)     5385 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/analysis/summary.py
+-rwxr-xr-x   0 capitac    (501) staff       (20)    18226 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/cli.py
+-rw-r--r--   0 capitac    (501) staff       (20)    11127 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/demultiplex.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.490327 iCount-Mini-3.0.1/iCount/examples/
+-rw-r--r--   0 capitac    (501) staff       (20)     1709 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/examples/__init__.py
+-rwxr-xr-x   0 capitac    (501) staff       (20)     3310 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/examples/hnRNPC.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)     3348 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/examples/hnRNPC_reduced.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)     1962 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/examples/tutorial.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.491869 iCount-Mini-3.0.1/iCount/externals/
+-rw-r--r--   0 capitac    (501) staff       (20)      324 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/externals/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2941 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/externals/cutadapt.py
+-rw-r--r--   0 capitac    (501) staff       (20)     7465 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/externals/star.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.493812 iCount-Mini-3.0.1/iCount/files/
+-rw-r--r--   0 capitac    (501) staff       (20)     3781 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/files/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3591 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/files/bed.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3183 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/files/bedgraph.py
+-rw-r--r--   0 capitac    (501) staff       (20)      762 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/files/fasta.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3221 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/files/fastq.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.495396 iCount-Mini-3.0.1/iCount/genomes/
+-rw-r--r--   0 capitac    (501) staff       (20)     5143 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/genomes/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10859 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/genomes/ensembl.py
+-rw-r--r--   0 capitac    (501) staff       (20)     7089 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/genomes/gencode.py
+-rw-r--r--   0 capitac    (501) staff       (20)    40516 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/genomes/segment.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6994 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/logger.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.501280 iCount-Mini-3.0.1/iCount/mapping/
+-rw-r--r--   0 capitac    (501) staff       (20)      377 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/mapping/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)      925 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/mapping/filters.py
+-rw-r--r--   0 capitac    (501) staff       (20)      197 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/mapping/indexstar.py
+-rw-r--r--   0 capitac    (501) staff       (20)      218 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/mapping/mapstar.py
+-rw-r--r--   0 capitac    (501) staff       (20)    22429 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/mapping/xlsites.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1558 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/metrics.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.502759 iCount-Mini-3.0.1/iCount/plotting/
+-rw-r--r--   0 capitac    (501) staff       (20)      160 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/plotting/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2204 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/plotting/plot_combined.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4466 2023-07-12 11:45:00.000000 iCount-Mini-3.0.1/iCount/plotting/plot_metagene.py
+-rw-r--r--   0 capitac    (501) staff       (20)     5435 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/plotting/plot_rnaheatmap.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.517372 iCount-Mini-3.0.1/iCount/tests/
+-rw-r--r--   0 capitac    (501) staff       (20)       20 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/__init__.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.527242 iCount-Mini-3.0.1/iCount/tests/functional/
+-rw-r--r--   0 capitac    (501) staff       (20)      367 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9158 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/gtf_variations.py
+-rw-r--r--   0 capitac    (501) staff       (20)    29055 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt
+-rw-r--r--   0 capitac    (501) staff       (20)     3308 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/pipeline_examples.py
+-rw-r--r--   0 capitac    (501) staff       (20)      278 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/segments_count.out.txt
+-rw-r--r--   0 capitac    (501) staff       (20)     4366 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/functional/segments_count.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6912 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_annotate.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2696 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_bed.py
+-rw-r--r--   0 capitac    (501) staff       (20)    16194 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/tests/test_cli.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2580 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_clusters.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1081 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_data.py
+-rw-r--r--   0 capitac    (501) staff       (20)    14672 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_demultiplex.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6817 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/tests/test_e2e.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1012 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_examples.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4604 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_externals.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9046 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_files.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10194 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_genomes.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4109 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_peaks.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/tests/test_plotting.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9700 2023-05-17 05:53:23.000000 iCount-Mini-3.0.1/iCount/tests/test_rnamaps.py
+-rw-r--r--   0 capitac    (501) staff       (20)    42560 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_segment.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6056 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_summary.py
+-rw-r--r--   0 capitac    (501) staff       (20)    14112 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/test_xlsites.py
+-rw-r--r--   0 capitac    (501) staff       (20)    11519 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/iCount/tests/utils.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-12 11:54:16.542331 iCount-Mini-3.0.1/iCount_Mini.egg-info/
+-rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/PKG-INFO
+-rw-r--r--   0 capitac    (501) staff       (20)     2564 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/SOURCES.txt
+-rw-r--r--   0 capitac    (501) staff       (20)        1 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/dependency_links.txt
+-rw-r--r--   0 capitac    (501) staff       (20)       48 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/entry_points.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      266 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/requires.txt
+-rw-r--r--   0 capitac    (501) staff       (20)        7 2023-07-12 11:54:16.000000 iCount-Mini-3.0.1/iCount_Mini.egg-info/top_level.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      111 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/requirements-rtd.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      242 2023-07-12 11:54:16.543957 iCount-Mini-3.0.1/setup.cfg
+-rwxr-xr-x   0 capitac    (501) staff       (20)     2546 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/setup.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1108 2023-05-15 06:53:41.000000 iCount-Mini-3.0.1/tox.ini
```

### Comparing `iCount-Mini-3.0.0/.pylintrc` & `iCount-Mini-3.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/CLA` & `iCount-Mini-3.0.1/CLA`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/Dockerfile` & `iCount-Mini-3.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/Dockerfile_test` & `iCount-Mini-3.0.1/Dockerfile_test`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/LICENSE` & `iCount-Mini-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/MANIFEST.in` & `iCount-Mini-3.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/PKG-INFO` & `iCount-Mini-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCount-Mini
-Version: 3.0.0
+Version: 3.0.1
 Summary: Computational pipeline for analysis of iCLIP data
 Home-page: https://github.com/ulelab/iCount-Mini
 Author: Ule Group, The Francis Crick Institute, London
 Author-email: jernej.ule@crick.ac.uk
 License: MIT
 Keywords: iCLIP protein-RNA
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iCount-Mini-3.0.0/README.md` & `iCount-Mini-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/Makefile` & `iCount-Mini-3.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/changelog.sh` & `iCount-Mini-3.0.1/docs/changelog.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/cite.rst` & `iCount-Mini-3.0.1/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/conf.py` & `iCount-Mini-3.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/contributing.rst` & `iCount-Mini-3.0.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/faq.rst` & `iCount-Mini-3.0.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/installation.rst` & `iCount-Mini-3.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/ref_CLI.txt` & `iCount-Mini-3.0.1/docs/source/ref_CLI.txt`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/ref_python.rst` & `iCount-Mini-3.0.1/docs/source/ref_python.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/docs/source/tutorial.rst` & `iCount-Mini-3.0.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/__about__.py` & `iCount-Mini-3.0.1/iCount/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #       interfere with a global variable __name__ denoting object's name.
 __title__ = 'iCount-Mini'
 __summary__ = 'Computational pipeline for analysis of iCLIP data'
 __url__ = 'https://github.com/ulelab/iCount-Mini'
 
 # Semantic versioning is used. For more information see:
 # https://packaging.python.org/en/latest/distributing/#semantic-versioning-preferred
-__version__ = '3.0.0'
+__version__ = '3.0.1'
 
 __author__ = 'Ule Group, The Francis Crick Institute, London'
 __email__ = 'jernej.ule@crick.ac.uk'
 
 __license__ = 'MIT'
 __copyright__ = '2016-2017, University of Ljubljana, Bioinformatics Laboratory'
```

### Comparing `iCount-Mini-3.0.0/iCount/__init__.py` & `iCount-Mini-3.0.1/iCount/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/__init__.py` & `iCount-Mini-3.0.1/iCount/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/annotate.py` & `iCount-Mini-3.0.1/iCount/analysis/annotate.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/kmers.py` & `iCount-Mini-3.0.1/iCount/analysis/kmers.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/metagene.py` & `iCount-Mini-3.0.1/iCount/analysis/metagene.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/peaks.py` & `iCount-Mini-3.0.1/iCount/analysis/peaks.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/sigxls.py` & `iCount-Mini-3.0.1/iCount/analysis/sigxls.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/analysis/summary.py` & `iCount-Mini-3.0.1/iCount/analysis/summary.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/cli.py` & `iCount-Mini-3.0.1/iCount/cli.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/demultiplex.py` & `iCount-Mini-3.0.1/iCount/demultiplex.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/examples/__init__.py` & `iCount-Mini-3.0.1/iCount/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/examples/hnRNPC.sh` & `iCount-Mini-3.0.1/iCount/examples/hnRNPC.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/examples/hnRNPC_reduced.sh` & `iCount-Mini-3.0.1/iCount/examples/hnRNPC_reduced.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/examples/tutorial.sh` & `iCount-Mini-3.0.1/iCount/examples/tutorial.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/externals/cutadapt.py` & `iCount-Mini-3.0.1/iCount/externals/cutadapt.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/externals/star.py` & `iCount-Mini-3.0.1/iCount/externals/star.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/files/__init__.py` & `iCount-Mini-3.0.1/iCount/files/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/files/bed.py` & `iCount-Mini-3.0.1/iCount/files/bed.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/files/bedgraph.py` & `iCount-Mini-3.0.1/iCount/files/bedgraph.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/files/fasta.py` & `iCount-Mini-3.0.1/iCount/files/fasta.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/files/fastq.py` & `iCount-Mini-3.0.1/iCount/files/fastq.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/genomes/__init__.py` & `iCount-Mini-3.0.1/iCount/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/genomes/ensembl.py` & `iCount-Mini-3.0.1/iCount/genomes/ensembl.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/genomes/gencode.py` & `iCount-Mini-3.0.1/iCount/genomes/gencode.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/genomes/segment.py` & `iCount-Mini-3.0.1/iCount/genomes/segment.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/logger.py` & `iCount-Mini-3.0.1/iCount/logger.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/mapping/filters.py` & `iCount-Mini-3.0.1/iCount/mapping/filters.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/mapping/xlsites.py` & `iCount-Mini-3.0.1/iCount/mapping/xlsites.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/metrics.py` & `iCount-Mini-3.0.1/iCount/metrics.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/plotting/plot_combined.py` & `iCount-Mini-3.0.1/iCount/plotting/plot_combined.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/plotting/plot_metagene.py` & `iCount-Mini-3.0.1/iCount/plotting/plot_metagene.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,12 +145,12 @@
 
     ax.set_xlim((up_limit, down_limit))
     ax.set_xlabel('Position')
     if ylim:
         ax.set_ylim((0, ylim))
     ax.set_ylabel('Score [CPM]')
     ax.set_title('Metagene')
-    ax.grid(b=True, which='major', axis='both')
+    ax.grid(visible=True, which='major', axis='both')
     ax.legend()
 
     if is_independent:
         fig.savefig(outfile)
```

### Comparing `iCount-Mini-3.0.0/iCount/plotting/plot_rnaheatmap.py` & `iCount-Mini-3.0.1/iCount/plotting/plot_rnaheatmap.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/functional/gtf_variations.py` & `iCount-Mini-3.0.1/iCount/tests/functional/gtf_variations.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt` & `iCount-Mini-3.0.1/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.py` & `iCount-Mini-3.0.1/iCount/tests/functional/pipeline_examples.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/functional/segments_count.py` & `iCount-Mini-3.0.1/iCount/tests/functional/segments_count.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_annotate.py` & `iCount-Mini-3.0.1/iCount/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_bed.py` & `iCount-Mini-3.0.1/iCount/tests/test_bed.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_cli.py` & `iCount-Mini-3.0.1/iCount/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_clusters.py` & `iCount-Mini-3.0.1/iCount/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_data.py` & `iCount-Mini-3.0.1/iCount/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_demultiplex.py` & `iCount-Mini-3.0.1/iCount/tests/test_demultiplex.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_e2e.py` & `iCount-Mini-3.0.1/iCount/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_examples.py` & `iCount-Mini-3.0.1/iCount/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_externals.py` & `iCount-Mini-3.0.1/iCount/tests/test_externals.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_files.py` & `iCount-Mini-3.0.1/iCount/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_genomes.py` & `iCount-Mini-3.0.1/iCount/tests/test_genomes.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_peaks.py` & `iCount-Mini-3.0.1/iCount/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_plotting.py` & `iCount-Mini-3.0.1/iCount/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_rnamaps.py` & `iCount-Mini-3.0.1/iCount/tests/test_rnamaps.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_segment.py` & `iCount-Mini-3.0.1/iCount/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_summary.py` & `iCount-Mini-3.0.1/iCount/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/test_xlsites.py` & `iCount-Mini-3.0.1/iCount/tests/test_xlsites.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount/tests/utils.py` & `iCount-Mini-3.0.1/iCount/tests/utils.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/iCount_Mini.egg-info/PKG-INFO` & `iCount-Mini-3.0.1/iCount_Mini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCount-Mini
-Version: 3.0.0
+Version: 3.0.1
 Summary: Computational pipeline for analysis of iCLIP data
 Home-page: https://github.com/ulelab/iCount-Mini
 Author: Ule Group, The Francis Crick Institute, London
 Author-email: jernej.ule@crick.ac.uk
 License: MIT
 Keywords: iCLIP protein-RNA
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iCount-Mini-3.0.0/iCount_Mini.egg-info/SOURCES.txt` & `iCount-Mini-3.0.1/iCount_Mini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/setup.py` & `iCount-Mini-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-3.0.0/tox.ini` & `iCount-Mini-3.0.1/tox.ini`

 * *Files identical despite different names*

