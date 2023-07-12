# Comparing `tmp/trimnami-0.0.3.tar.gz` & `tmp/trimnami-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.0.3.tar", last modified: Thu Jul  6 06:25:59 2023, max compression
+gzip compressed data, was "trimnami-0.0.4.tar", last modified: Wed Jul 12 01:25:11 2023, max compression
```

## Comparing `trimnami-0.0.3.tar` & `trimnami-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 06:25:50.000000 trimnami-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-06 06:25:59.980682 trimnami-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-06 06:25:50.000000 trimnami-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:25:59.980682 trimnami-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-06 06:25:50.000000 trimnami-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 06:25:50.000000 trimnami-0.0.3/tests/test_skipHostRm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 06:25:50.000000 trimnami-0.0.3/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/scripts/skipHostRm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.972682 trimnami-0.0.3/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/fastqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/multiqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/rasusa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/fastqc.smk
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/nanopore.smk
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/notrim.smk
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 01:25:00.000000 trimnami-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 01:25:11.966557 trimnami-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-12 01:25:00.000000 trimnami-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:25:11.966557 trimnami-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 01:25:00.000000 trimnami-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-12 01:25:00.000000 trimnami-0.0.4/tests/test_skipHostRm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-12 01:25:00.000000 trimnami-0.0.4/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/scripts/skipHostRm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.958557 trimnami-0.0.4/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/multiqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/rasusa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/fastqc.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/nanopore.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/rasusa.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.0.3/PKG-INFO` & `trimnami-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.3
+Version: 0.0.4
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trimnami-0.0.3/README.md` & `trimnami-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/setup.py` & `trimnami-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/tests/test_skipHostRm.py` & `trimnami-0.0.4/tests/test_skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/tests/test_trimnami.py` & `trimnami-0.0.4/tests/test_trimnami.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/__main__.py` & `trimnami-0.0.4/trimnami/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,20 @@
         click.option(
             "--fastqc/--no-fastqc",
             default=False,
             help="Run fastqc on trimmed and untrimmed reads",
             show_default=True,
         ),
         click.option(
+            "--subsample",
+            default=None,
+            help="Subsample reads to this many bases with rasusa, e.g. 1000, 1m, 1g, 1t",
+            show_default=False,
+        ),
+        click.option(
             "--use-conda/--no-use-conda",
             default=True,
             help="Use conda for Snakemake rules",
             show_default=True,
         ),
         click.option(
             "--conda-prefix",
@@ -168,14 +174,15 @@
     merge_config = {
         "trimnami": {
             "args": {
                 "reads": kwargs["reads"],
                 "output": kwargs["output"],
                 "host": kwargs["host"],
                 "fastqc": kwargs["fastqc"],
+                "subsample": kwargs["subsample"],
                 "minimap": kwargs["minimap"],
                 "log": kwargs["log"]
             }
         }
     }
 
     # run!
@@ -200,14 +207,15 @@
     # Config to add or update in configfile
     merge_config = {
         "trimnami": {
             "args": {
                 "reads": snake_base(os.path.join("test_data")),
                 "host": None,
                 "fastqc": kwargs["fastqc"],
+                "subsample": kwargs["subsample"],
                 "output": kwargs["output"],
                 "minimap": "sr",
                 "log": kwargs["log"]
             }
         }
     }
 
@@ -234,14 +242,15 @@
     merge_config = {
         "trimnami": {
             "args": {
                 "reads": snake_base(os.path.join("test_data")),
                 "host": snake_base(os.path.join("test_data", "ref.fna")),
                 "output": kwargs["output"],
                 "fastqc": kwargs["fastqc"],
+                "subsample": kwargs["subsample"],
                 "minimap": "sr",
                 "log": kwargs["log"]
             }
         }
     }
 
     # run!
@@ -267,14 +276,15 @@
     merge_config = {
         "trimnami": {
             "args": {
                 "reads": snake_base(os.path.join("test_data", "nanopore")),
                 "host": snake_base(os.path.join("test_data", "ref.fna")),
                 "output": kwargs["output"],
                 "fastqc": kwargs["fastqc"],
+                "subsample": kwargs["subsample"],
                 "minimap": "map-ont",
                 "log": kwargs["log"]
             }
         }
     }
 
     kwargs["snake_args"] = ["nanopore"]
```

### Comparing `trimnami-0.0.3/trimnami/config/config.yaml` & `trimnami-0.0.4/trimnami/config/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+resources:
+    med:
+        mem: 16000
+        cpu: 8
+        time: 240
 trimnami:
-    resources:
-        job:
-            cpu: 8
-            mem: 16000
-            time: 480
     qc:
         compression:
             1
         minimapIndex:
             -I 8G
         fastp:
             --qualified_quality_phred 15
```

### Comparing `trimnami-0.0.3/trimnami/config/system_config.yaml` & `trimnami-0.0.4/trimnami/config/system_config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 trimnami:
     args:
         reads:
         output:
         host:
         minimap:
         fastqc:
+        subsample:
         log:
     qc:
         bbduk:
             rm_5p:
                 k=16
                 hdist=1
                 mink=11
```

### Comparing `trimnami-0.0.3/trimnami/scripts/skipHostRm.py` & `trimnami-0.0.4/trimnami/scripts/skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.0.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/test_data/ref.fna` & `trimnami-0.0.4/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/trimnami.LICENSE` & `trimnami-0.0.4/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/Snakefile` & `trimnami-0.0.4/trimnami/workflow/Snakefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import glob
 import attrmap as ap
 import attrmap.utils as au
 
 
 configfile: os.path.join(workflow.basedir, '../', 'config', 'config.yaml')
 configfile: os.path.join(workflow.basedir, '../', 'config', 'system_config.yaml')
+resources = ap.AttrMap(config["resources"])
 config = ap.AttrMap(config["trimnami"])
 
 
 def copy_log_file():
     """Concatenate Snakemake's own logfile with the CLI logfile"""
     files = glob.glob(os.path.join(".snakemake", "log", "*.snakemake.log"))
     if files:
@@ -27,14 +28,15 @@
 include: os.path.join("rules", "hostRemoval.smk")
 include: os.path.join("rules", "fastqc.smk")
 include: os.path.join("rules", "fastp.smk")
 include: os.path.join("rules", "prinseq.smk")
 include: os.path.join("rules", "roundAB.smk")
 include: os.path.join("rules", "nanopore.smk")
 include: os.path.join("rules", "notrim.smk")
+include: os.path.join("rules", "rasusa.smk")
 include: os.path.join("rules", "reports.smk")
 
 
 # Mark target rules
 target_rules = []
 def targetRule(fn):
     assert fn.__name__.startswith('__')
```

### Comparing `trimnami-0.0.3/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.0.4/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/databases/primerB.fa` & `trimnami-0.0.4/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.0.4/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.0.4/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/fastp.smk` & `trimnami-0.0.4/trimnami/workflow/rules/fastp.smk`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         stats=temp(os.path.join(dir.fastp,"{file}.stats.json")),
         html=temp(os.path.join(dir.fastp,"{file}.stats.html"))
     benchmark:
         os.path.join(dir.bench,"fastp.{file}.txt")
     log:
         os.path.join(dir.log,"fastp.{file}.log")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"fastp.yaml")
     params:
         fastp=config.fastp,
         compression=config.qc.compression
     shell:
         """
@@ -68,18 +68,18 @@
         stats=temp(os.path.join(dir.fastp,"{file}.stats.json")),
         html=temp(os.path.join(dir.fastp,"{file}.stats.html"))
     benchmark:
         os.path.join(dir.bench,"fastp.{file}.txt")
     log:
         os.path.join(dir.log,"fastp.{file}.log")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"fastp.yaml")
     params:
         fastp=config.fastp,
         compression=config.qc.compression
     shell:
         """
```

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/fastqc.smk` & `trimnami-0.0.4/trimnami/workflow/rules/fastqc.smk`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         z1 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
             samples.reads[wildcards.sample]["R1"])) + "_fastqc.zip"),
         z2 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
             samples.reads[wildcards.sample]["R2"])) + "_fastqc.zip"),
     conda:
         os.path.join(dir.env, "fastqc.yaml")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     log:
         os.path.join(dir.log, "fastqc_paired_untrimmed.{sample}.log")
     benchmark:
         os.path.join(dir.bench,"fastqc_paired_untrimmed.{sample}.txt")
     shell:
         """
         fastqc {input} \
@@ -51,18 +51,18 @@
         r1=lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
             samples.reads[wildcards.sample]["R1"])) + "_fastqc.html"),
         z1=lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
             samples.reads[wildcards.sample]["R1"])) + "_fastqc.zip"),
     conda:
         os.path.join(dir.env,"fastqc.yaml")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     log:
         os.path.join(dir.log,"fastqc_unpaired_untrimmed.{sample}.log")
     benchmark:
         os.path.join(dir.bench,"fastqc_unpaired_untrimmed.{sample}.txt")
     shell:
         """
         fastqc {input} \
@@ -91,18 +91,18 @@
         dir = os.path.join(dir.temp,"{trimmer}"),
         z1 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1_fastqc.zip"),
         z2 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2_fastqc.zip"),
         zs = os.path.join(dir.temp,"{trimmer}","{sample}.paired.S_fastqc.zip"),
     conda:
         os.path.join(dir.env, "fastqc.yaml")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     log:
         os.path.join(dir.log, "fastqc_paired_trimmed.{sample}.{trimmer}.log")
     benchmark:
         os.path.join(dir.bench,"fastqc_paired_trimmed.{sample}.{trimmer}.txt")
     shell:
         """
         fastqc {input.r1} {input.r2} \
@@ -134,18 +134,18 @@
         z=temp(os.path.join(dir.reports,"{trimmer}","{sample}.single_fastqc.zip")),
     params:
         dir=os.path.join(dir.temp,"{trimmer}"),
         z=os.path.join(dir.temp,"{trimmer}","{sample}.single_fastqc.zip"),
     conda:
         os.path.join(dir.env,"fastqc.yaml")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     log:
         os.path.join(dir.log,"fastqc_single_trimmed.{sample}.{trimmer}.log")
     benchmark:
         os.path.join(dir.bench,"fastqc_single_trimmed.{sample}.{trimmer}.txt")
     shell:
         """
         fastqc {input} \
```

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.0.4/trimnami/workflow/rules/hostRemoval.smk`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     input:
         lambda wildcards: config.args.host if config.args.host else ""
     output:
         config.args.hostIndex
     params:
         params = config.qc.minimapIndex
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"minimap2.yaml")
     benchmark:
         os.path.join(dir.bench,"index_host_genome.txt")
     log:
         os.path.join(dir.log,"index_host_genome.log")
     shell:
@@ -37,18 +37,18 @@
     benchmark:
         os.path.join(dir.bench,"host_removal_mapping.{sample}.txt")
     log:
         mm=os.path.join(dir.log,"host_removal_mapping.{sample}.minimap.log"),
         sv=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsView.log"),
         fq=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsFastq.log"),
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"minimap2.yaml")
     shell:
         """
         minimap2 -ax sr -t {threads} --secondary=no {input.host} {input.r1} {input.r2} 2> {log.mm} \
             | samtools view -f 4 -h 2> {log.sv} \
             | samtools fastq -NO -c {params.compression} -1 {output.r1} -2 {output.r2} -0 {output.o} -s {output.s} 2> {log.fq}
@@ -71,18 +71,18 @@
     benchmark:
         os.path.join(dir.bench,"host_removal_mapping.{sample}.txt")
     log:
         mm=os.path.join(dir.log,"host_removal_mapping.{sample}.minimap.log"),
         sv=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsView.log"),
         fq=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsFastq.log")
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"minimap2.yaml")
     shell:
         """
         minimap2 -ax {params.minimap_mode} -t {threads} --secondary=no {input.host} {input.r1} 2> {log.mm} \
             | samtools view -f 4 -h 2> {log.sv} \
             | samtools fastq -nO -c {params.compression} -o {output.r1} -0 {output.o} -s {output.s} 2> {log.fq}
```

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/notrim.smk` & `trimnami-0.0.4/trimnami/workflow/rules/notrim.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/preflight.smk` & `trimnami-0.0.4/trimnami/workflow/rules/preflight.smk`

 * *Files 20% similar despite different names*

```diff
@@ -39,49 +39,51 @@
 
 """
 Define file intermediates
 """
 # Check if host removal
 config.args.hostStr = ""
 config.args.hostIndex = ""
+config.args.subsampleStr = ""
 if config.args.host is not None:
     # String to append to targets to signal host removal
     config.args.hostStr = ".host_rm"
     # Minimap2 index file for mapping
     config.args.hostIndex = os.path.join(
         dir.temp,
         os.path.splitext(
             os.path.basename(config.args.host)
         )[0] + ".idx"
     )
-
+if config.args.subsample is not None:
+    config.args.subsampleStr = ".subsampled"
 
 """
 Define targets
 """
 targets = ap.AttrMap()
 
 # generate target base names
 for sample_name in samples.names:
     if samples.reads[sample_name]["R2"] is not None:
         samples.reads[sample_name]["trimmed_targets"] = expand(
-            sample_name + config.args.hostStr + ".paired" + "{R12}.fastq.gz",
+            sample_name + config.args.hostStr + ".paired" + "{R12}" + config.args.subsampleStr + ".fastq.gz",
             R12 = [".R1", ".R2", ".S"]
         )
         samples.reads[sample_name]["fastqc_targets"] = expand(
-            sample_name + config.args.hostStr + ".paired" + "{R12}_fastqc.zip",
+            sample_name + config.args.hostStr + config.args.subsampleStr + ".paired" + "{R12}" + config.args.subsampleStr + "_fastqc.zip",
             R12 = [".R1", ".R2", ".S"]
         )
         samples.reads[sample_name]["fastqc_untrimmed"] = expand(
             sample_name + ".paired" + "{R12}_fastqc.zip",
             R12=[".R1", ".R2"]
         )
     else:
-        samples.reads[sample_name]["trimmed_targets"] = [sample_name + config.args.hostStr + ".single.fastq.gz"]
-        samples.reads[sample_name]["fastqc_targets"] = [sample_name + config.args.hostStr + ".single_fastqc.zip"]
+        samples.reads[sample_name]["trimmed_targets"] = [sample_name + config.args.hostStr + ".single" + config.args.subsampleStr + ".fastq.gz"]
+        samples.reads[sample_name]["fastqc_targets"] = [sample_name + config.args.hostStr + ".single" + config.args.subsampleStr + "_fastqc.zip"]
         samples.reads[sample_name]["fastqc_untrimmed"] = [sample_name + ".untrimmed.single_fastqc.zip"]
 
 
 # lock samples from further changes
 samples = au.convert_state(samples, read_only=True)
```

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/prinseq.smk` & `trimnami-0.0.4/trimnami/workflow/rules/prinseq.smk`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     output:
         r1=os.path.join(dir.prinseq,"{file}.R1.fastq.gz"),
         r2=os.path.join(dir.prinseq,"{file}.R2.fastq.gz"),
         s=os.path.join(dir.prinseq,"{file}.S.fastq.gz"),
         s1=temp(os.path.join(dir.prinseq,"{file}.S1.fastq.gz")),
         s2=temp(os.path.join(dir.prinseq,"{file}.S2.fastq.gz")),
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"prinseq.yaml")
     params:
         params = config.qc.prinseq
     log:
         os.path.join(dir.log, "prinseq.{file}.log")
     benchmark:
@@ -52,18 +52,18 @@
 
 rule prinseq_single:
     input:
         r1=os.path.join(dir.temp,"{file}.single.fastq.gz"),
     output:
         r1=os.path.join(dir.prinseq,"{file}.single.fastq.gz"),
     resources:
-        mem_mb=config.resources.job.mem,
-        time=config.resources.job.time
+        mem_mb=resources.med.mem,
+        time=resources.med.time
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     conda:
         os.path.join(dir.env,"prinseq.yaml")
     params:
         params = config.qc.prinseq
     log:
         os.path.join(dir.log, "prinseq.{file}.log")
     benchmark:
```

### Comparing `trimnami-0.0.3/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.0.4/trimnami/workflow/rules/roundAB.smk`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s1.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s1.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_5prime_primer.{file}.txt")
     log:
         os.path.join(dir.log,"remove_5prime_primer.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_5p
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -65,19 +65,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s2.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s2.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_3prime_contaminant.{file}.txt")
     log:
         os.path.join(dir.log,"remove_3prime_contaminant.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_3rt
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -120,19 +120,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s3.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s3.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_primer_free_adapter.{file}.txt")
     log:
         os.path.join(dir.log,"remove_primer_free_adapter.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.neb
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -175,19 +175,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s4.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s4.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_adapter_free_primer.{file}.txt")
     log:
         os.path.join(dir.log,"remove_adapter_free_primer.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_afp
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -230,19 +230,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s5.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s5.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_vector_contamination.{file}.txt")
     log:
         os.path.join(dir.log,"remove_vector_contamination.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_vc
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -284,19 +284,19 @@
         r2=temp(os.path.join(dir.temp,"{file}.R2.s6.fastq")),
         s=temp(os.path.join(dir.temp,"{file}.S.s6.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_low_quality.{file}.txt")
     log:
         os.path.join(dir.log,"remove_low_quality.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_lq
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
     shell:
@@ -336,19 +336,19 @@
         r2 = os.path.join(dir.roundAB,"{file}.R2.fastq.gz"),
         s = os.path.join(dir.roundAB,"{file}.S.fastq.gz")
     benchmark:
         os.path.join(dir.bench,"zip_roundAB.{file}.txt")
     log:
         os.path.join(dir.log,"zip_roundAB.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         compression = config.qc.compression
     conda:
         os.path.join(dir.env, "pigz.yaml")
     group:
         "roundAB"
     shell:
@@ -367,19 +367,19 @@
         r1=os.path.join(dir.roundAB,"{file}.single.fastq.gz"),
         tmp=temp(os.path.join(dir.roundAB,"{file}.single.fastq")),
     benchmark:
         os.path.join(dir.bench,"remove_low_quality.{file}.txt")
     log:
         os.path.join(dir.log,"remove_low_quality.{file}.log")
     resources:
-        mem_mb = config.resources.job.mem,
-        javaAlloc = int(0.9 * config.resources.job.mem),
-        time = int(0.5 * config.resources.job.time)
+        mem_mb = resources.med.mem,
+        javaAlloc = int(0.9 * resources.med.mem),
+        time = int(0.5 * resources.med.time)
     threads:
-        config.resources.job.cpu
+        resources.med.cpu
     params:
         params = config.qc.bbduk.rm_lq,
         compression = config.qc.compression
     conda:
         os.path.join(dir.env, "bbmap.yaml")
     group:
         "roundAB"
```

### Comparing `trimnami-0.0.3/trimnami.egg-info/PKG-INFO` & `trimnami-0.0.4/trimnami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.3
+Version: 0.0.4
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trimnami-0.0.3/trimnami.egg-info/SOURCES.txt` & `trimnami-0.0.4/trimnami.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -43,9 +43,10 @@
 trimnami/workflow/rules/fastp.smk
 trimnami/workflow/rules/fastqc.smk
 trimnami/workflow/rules/hostRemoval.smk
 trimnami/workflow/rules/nanopore.smk
 trimnami/workflow/rules/notrim.smk
 trimnami/workflow/rules/preflight.smk
 trimnami/workflow/rules/prinseq.smk
+trimnami/workflow/rules/rasusa.smk
 trimnami/workflow/rules/reports.smk
 trimnami/workflow/rules/roundAB.smk
```

