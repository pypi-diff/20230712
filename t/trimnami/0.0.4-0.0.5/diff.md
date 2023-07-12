# Comparing `tmp/trimnami-0.0.4.tar.gz` & `tmp/trimnami-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.0.4.tar", last modified: Wed Jul 12 01:25:11 2023, max compression
+gzip compressed data, was "trimnami-0.0.5.tar", last modified: Wed Jul 12 04:46:08 2023, max compression
```

## Comparing `trimnami-0.0.4.tar` & `trimnami-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 01:25:00.000000 trimnami-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 01:25:11.966557 trimnami-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-12 01:25:00.000000 trimnami-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:25:11.966557 trimnami-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 01:25:00.000000 trimnami-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-12 01:25:00.000000 trimnami-0.0.4/tests/test_skipHostRm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-12 01:25:00.000000 trimnami-0.0.4/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/scripts/skipHostRm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.958557 trimnami-0.0.4/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.962557 trimnami-0.0.4/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/fastqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/multiqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/envs/rasusa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.966557 trimnami-0.0.4/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/fastqc.smk
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/nanopore.smk
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/notrim.smk
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/rasusa.smk
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-12 01:25:00.000000 trimnami-0.0.4/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:25:11.950556 trimnami-0.0.4/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:25:11.000000 trimnami-0.0.4/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.337880 trimnami-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 04:45:58.000000 trimnami-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 04:46:08.337880 trimnami-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-12 04:45:58.000000 trimnami-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 04:46:08.337880 trimnami-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 04:45:58.000000 trimnami-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.321880 trimnami-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-12 04:45:58.000000 trimnami-0.0.5/tests/test_skipHostRm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-12 04:45:58.000000 trimnami-0.0.5/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.321880 trimnami-0.0.5/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.321880 trimnami-0.0.5/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.321880 trimnami-0.0.5/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/scripts/skipHostRm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.329880 trimnami-0.0.5/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.333880 trimnami-0.0.5/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.333880 trimnami-0.0.5/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.333880 trimnami-0.0.5/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.337880 trimnami-0.0.5/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/multiqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/envs/rasusa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.337880 trimnami-0.0.5/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/fastqc.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/nanopore.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/rasusa.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-12 04:45:58.000000 trimnami-0.0.5/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:46:08.321880 trimnami-0.0.5/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 04:46:08.000000 trimnami-0.0.5/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.0.4/PKG-INFO` & `trimnami-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trimnami-0.0.4/README.md` & `trimnami-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/setup.py` & `trimnami-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/tests/test_skipHostRm.py` & `trimnami-0.0.5/tests/test_skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/tests/test_trimnami.py` & `trimnami-0.0.5/tests/test_trimnami.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,10 +40,12 @@
     exec_command("trimnami -v")
     exec_command("trimnami -h")
     exec_command("trimnami run -h")
     exec_command("trimnami config -h")
 
 
 def test_trimnami_commands(tmp_dir):
-    exec_command("trimnami test --threads 1 --fastqc -n prinseq fastp roundAB nanopore notrim")
+    exec_command("trimnami test --threads 1 --fastqc -n --subsample 1k prinseq fastp roundAB notrim")
+    exec_command("trimnami testhost --threads 1 --fastqc -n --subsample 1k prinseq fastp roundAB notrim")
+    exec_command("trimnami testnp --threads 1 --fastqc -n --subsample 1k")
     exec_command("trimnami config")
     exec_command("trimnami citation")
```

### Comparing `trimnami-0.0.4/trimnami/__main__.py` & `trimnami-0.0.5/trimnami/__main__.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/config/config.yaml` & `trimnami-0.0.5/trimnami/config/config.yaml`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/config/system_config.yaml` & `trimnami-0.0.5/trimnami/config/system_config.yaml`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/scripts/skipHostRm.py` & `trimnami-0.0.5/trimnami/scripts/skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.0.5/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.0.5/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/test_data/ref.fna` & `trimnami-0.0.5/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/trimnami.LICENSE` & `trimnami-0.0.5/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/Snakefile` & `trimnami-0.0.5/trimnami/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.0.5/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/databases/primerB.fa` & `trimnami-0.0.5/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.0.5/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.0.5/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/fastp.smk` & `trimnami-0.0.5/trimnami/workflow/rules/fastp.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/fastqc.smk` & `trimnami-0.0.5/trimnami/workflow/rules/fastqc.smk`

 * *Files 14% similar despite different names*

```diff
@@ -73,40 +73,40 @@
         mv {params.z1} {output.z1}
         rm {params.r1}
         """
 
 
 rule fastqc_paired_trimmed:
     input:
-        r1 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R1.fastq.gz"),
-        r2 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R2.fastq.gz"),
-        rs = os.path.join(dir.out, "{trimmer}", "{sample}.paired.S.fastq.gz"),
+        r1 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R1{subsampled}.fastq.gz"),
+        r2 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R2{subsampled}.fastq.gz"),
+        rs = os.path.join(dir.out, "{trimmer}", "{sample}.paired.S{subsampled}.fastq.gz"),
     output:
-        r1 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1_fastqc.html")),
-        r2 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2_fastqc.html")),
-        rs = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.S_fastqc.html")),
-        z1 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R1_fastqc.zip")),
-        z2 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R2_fastqc.zip")),
-        zs = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.S_fastqc.zip")),
+        r1 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.html")),
+        r2 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.html")),
+        rs = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.html")),
+        z1 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.zip")),
+        z2 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.zip")),
+        zs = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.zip")),
     params:
         dir = os.path.join(dir.temp,"{trimmer}"),
-        z1 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1_fastqc.zip"),
-        z2 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2_fastqc.zip"),
-        zs = os.path.join(dir.temp,"{trimmer}","{sample}.paired.S_fastqc.zip"),
+        z1 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.zip"),
+        z2 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.zip"),
+        zs = os.path.join(dir.temp,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.zip"),
     conda:
         os.path.join(dir.env, "fastqc.yaml")
     resources:
         mem_mb=resources.med.mem,
         time=resources.med.time
     threads:
         resources.med.cpu
     log:
-        os.path.join(dir.log, "fastqc_paired_trimmed.{sample}.{trimmer}.log")
+        os.path.join(dir.log, "fastqc_paired_trimmed.{sample}.{trimmer}{subsampled}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_paired_trimmed.{sample}.{trimmer}.txt")
+        os.path.join(dir.bench,"fastqc_paired_trimmed.{sample}.{trimmer}{subsampled}.txt")
     shell:
         """
         fastqc {input.r1} {input.r2} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
         
@@ -124,32 +124,32 @@
         mv {params.z2} {output.z2}
         mv {params.zs} {output.zs}
         """
 
 
 rule fastqc_single_trimmed:
     input:
-        os.path.join(dir.out,"{trimmer}","{sample}.single.fastq.gz"),
+        os.path.join(dir.out,"{trimmer}","{sample}.single{subsampled}.fastq.gz"),
     output:
-        r=temp(os.path.join(dir.temp,"{trimmer}","{sample}.single_fastqc.html")),
-        z=temp(os.path.join(dir.reports,"{trimmer}","{sample}.single_fastqc.zip")),
+        r=temp(os.path.join(dir.temp,"{trimmer}","{sample}.single{subsampled}_fastqc.html")),
+        z=temp(os.path.join(dir.reports,"{trimmer}","{sample}.single{subsampled}_fastqc.zip")),
     params:
         dir=os.path.join(dir.temp,"{trimmer}"),
-        z=os.path.join(dir.temp,"{trimmer}","{sample}.single_fastqc.zip"),
+        z=os.path.join(dir.temp,"{trimmer}","{sample}.single{subsampled}_fastqc.zip"),
     conda:
         os.path.join(dir.env,"fastqc.yaml")
     resources:
         mem_mb=resources.med.mem,
         time=resources.med.time
     threads:
         resources.med.cpu
     log:
-        os.path.join(dir.log,"fastqc_single_trimmed.{sample}.{trimmer}.log")
+        os.path.join(dir.log,"fastqc_single_trimmed.{sample}.{trimmer}{subsampled}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_single_trimmed.{sample}.{trimmer}.txt")
+        os.path.join(dir.bench,"fastqc_single_trimmed.{sample}.{trimmer}{subsampled}.txt")
     shell:
         """
         fastqc {input} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
```

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.0.5/trimnami/workflow/rules/hostRemoval.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/nanopore.smk` & `trimnami-0.0.5/trimnami/workflow/rules/nanopore.smk`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     params:
         params=config.qc.nanopore.filtlong
     log:
         os.path.join(dir.log, "filtlong_{file}.log")
     shell:
         """
             export LC_ALL=en_US.UTF-8
-            filtlong {params.params} {input.i} > {output.o} 2> {log}
+            filtlong {params.params} {input.i} | gzip -1 > {output.o} 2> {log}
         """
 
 
 rule nanopore_paired:
     """This rule should never be run"""
     input:
         r1=os.path.join(dir.temp,"{file}.R1.fastq.gz"),
```

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/notrim.smk` & `trimnami-0.0.5/trimnami/workflow/rules/notrim.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/preflight.smk` & `trimnami-0.0.5/trimnami/workflow/rules/preflight.smk`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 for sample_name in samples.names:
     if samples.reads[sample_name]["R2"] is not None:
         samples.reads[sample_name]["trimmed_targets"] = expand(
             sample_name + config.args.hostStr + ".paired" + "{R12}" + config.args.subsampleStr + ".fastq.gz",
             R12 = [".R1", ".R2", ".S"]
         )
         samples.reads[sample_name]["fastqc_targets"] = expand(
-            sample_name + config.args.hostStr + config.args.subsampleStr + ".paired" + "{R12}" + config.args.subsampleStr + "_fastqc.zip",
+            sample_name + config.args.hostStr + ".paired" + "{R12}" + config.args.subsampleStr + "_fastqc.zip",
             R12 = [".R1", ".R2", ".S"]
         )
         samples.reads[sample_name]["fastqc_untrimmed"] = expand(
             sample_name + ".paired" + "{R12}_fastqc.zip",
             R12=[".R1", ".R2"]
         )
     else:
```

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/prinseq.smk` & `trimnami-0.0.5/trimnami/workflow/rules/prinseq.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/rasusa.smk` & `trimnami-0.0.5/trimnami/workflow/rules/rasusa.smk`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,19 @@
             -i {input.r2} \
             -o {output.r1} \
             -o {output.r2} \
             -O g \
             --bases {params.bases} \
             2> {log}
         
-        rasusa \
-            -i {input.rs} \
-            -o {output.rs} \
-            -O g \
-            --bases {params.bases} \
-            2> {log}
+        if (( $(wc -c {input.rs} | awk '{{print$1}}') > 100 ))
+        then
+            rasusa \
+                -i {input.rs} \
+                -o {output.rs} \
+                -O g \
+                --bases {params.bases} \
+                2> {log}
+        else
+            touch {output.rs}
+        fi
         """
```

### Comparing `trimnami-0.0.4/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.0.5/trimnami/workflow/rules/roundAB.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.4/trimnami.egg-info/PKG-INFO` & `trimnami-0.0.5/trimnami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trimnami-0.0.4/trimnami.egg-info/SOURCES.txt` & `trimnami-0.0.5/trimnami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

