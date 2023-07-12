# Comparing `tmp/nef_pipelines-0.1.42.tar.gz` & `tmp/nef_pipelines-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.42.tar", last modified: Sun Jun  4 15:55:22 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.43.tar", last modified: Wed Jul 12 10:12:13 2023, max compression
```

## Comparing `nef_pipelines-0.1.42.tar` & `nef_pipelines-0.1.43.tar`

### file list

```diff
@@ -1,396 +1,396 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.364850 nef_pipelines-0.1.42/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.107114 nef_pipelines-0.1.42/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.221578 nef_pipelines-0.1.42/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.242321 nef_pipelines-0.1.42/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.42/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.42/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.248021 nef_pipelines-0.1.42/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.42/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.42/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.42/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.42/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3974 2023-06-04 15:54:43.000000 nef_pipelines-0.1.42/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.42/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.42/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-06-04 15:55:22.365936 nef_pipelines-0.1.42/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.42/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.42/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.42/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.272098 nef_pipelines-0.1.42/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.42/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.42/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.42/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.42/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-06-04 15:55:22.370751 nef_pipelines-0.1.42/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.42/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.108391 nef_pipelines-0.1.42/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.297602 nef_pipelines-0.1.42/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.351028 nef_pipelines-0.1.42/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.414313 nef_pipelines-0.1.42/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15025 2023-05-24 21:08:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    23324 2023-06-04 15:15:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4191 2023-05-21 10:59:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10315 2023-06-04 10:57:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.417723 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    24946 2023-05-24 21:08:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5335 2023-05-20 12:46:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.418104 nef_pipelines-0.1.42/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.451920 nef_pipelines-0.1.42/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.463766 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.468343 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.475773 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.481781 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rwxrwxrwx   0 garythompson   (501) staff       (20)      315 2023-05-28 10:49:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     3065 2023-05-28 10:49:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.483400 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.487728 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.489197 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.507508 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.522798 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.527488 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_tabulate.py
--rwxr--r--   0 garythompson   (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_unassign.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.547622 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.558240 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
--rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
--rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_all.out
--rw-r--r--   0 garythompson   (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5489 2023-05-24 21:22:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.588092 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.643595 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.674506 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.716590 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.724282 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.729450 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.731312 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.743593 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.745115 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.756683 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.773945 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.837902 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.850342 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garythompson   (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.852061 nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.892384 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.898994 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garythompson   (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3392 2023-05-21 11:56:45.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8984 2023-05-21 14:27:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.912340 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.969737 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.003330 nef_pipelines-0.1.42/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.019260 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.026904 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.049161 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      700 2023-06-04 15:15:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8977 2023-05-21 15:22:30.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/unassign.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.056586 nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.061250 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-21 16:48:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.064846 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.065378 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.076138 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16493 2023-05-28 10:49:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.079062 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.083583 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.086102 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.089089 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.092400 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.095891 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.133047 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5933 2023-05-24 21:29:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.142334 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11115 2023-05-24 21:25:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.154233 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.168738 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.173606 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.189912 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.214559 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.216766 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.221906 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.224655 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.226742 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.230970 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.237257 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.239984 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.259334 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.269052 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.274424 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-21 16:37:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.292371 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7995 2023-05-24 21:20:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-05-24 21:17:30.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17287 2023-05-24 21:17:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.302598 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.309013 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.317524 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garythompson   (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.330114 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     2925 2023-05-21 12:09:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2852 2023-05-21 11:00:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1899 2023-05-21 14:30:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    22539 2023-05-21 14:29:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.341735 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.348385 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.361227 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.316404 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    15289 2023-06-04 15:55:21.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.984212 nef_pipelines-0.1.43/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:11.826670 nef_pipelines-0.1.43/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:11.953071 nef_pipelines-0.1.43/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.43/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:11.988006 nef_pipelines-0.1.43/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.43/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.43/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.43/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:11.992359 nef_pipelines-0.1.43/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.43/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.43/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.43/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.43/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.43/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.43/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.43/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     4106 2023-07-12 10:10:49.000000 nef_pipelines-0.1.43/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.43/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.43/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-07-12 10:12:13.984514 nef_pipelines-0.1.43/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.43/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.43/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.43/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.025058 nef_pipelines-0.1.43/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.43/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.43/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.43/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.43/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-07-12 10:12:13.987938 nef_pipelines-0.1.43/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.43/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:11.827959 nef_pipelines-0.1.43/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.057081 nef_pipelines-0.1.43/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.43/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.155015 nef_pipelines-0.1.43/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.270628 nef_pipelines-0.1.43/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15025 2023-05-24 21:08:05.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    23324 2023-06-04 15:15:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4216 2023-07-09 14:27:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10315 2023-06-04 10:57:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.273187 nef_pipelines-0.1.43/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    24946 2023-05-24 21:08:07.000000 nef_pipelines-0.1.43/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5335 2023-05-20 12:46:21.000000 nef_pipelines-0.1.43/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.277142 nef_pipelines-0.1.43/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.309795 nef_pipelines-0.1.43/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.330711 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.347393 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.360376 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.388407 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxrwxrwx   0 garythompson   (501) staff       (20)      315 2023-05-28 10:49:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     3065 2023-05-28 10:49:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.394753 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.404341 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.410416 nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.419776 nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.445458 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.465622 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.499959 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.578363 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garythompson   (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5489 2023-05-24 21:22:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.648317 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.842450 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.871142 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.969706 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.980391 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.996851 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.003202 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.044448 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.051249 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.056262 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.077453 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.204190 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.268715 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.274494 nef_pipelines-0.1.43/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.306077 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.321543 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garythompson   (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3392 2023-05-21 11:56:45.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8984 2023-05-21 14:27:42.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.349524 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.437165 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.491608 nef_pipelines-0.1.43/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.511952 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.519755 nef_pipelines-0.1.43/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.601328 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      700 2023-06-04 15:15:37.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8977 2023-05-21 15:22:30.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.605990 nef_pipelines-0.1.43/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.614977 nef_pipelines-0.1.43/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-21 16:48:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.43/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.619177 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.625497 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.638168 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16493 2023-05-28 10:49:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.646016 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.651700 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.655846 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.659699 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.664003 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6210 2023-07-09 14:27:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.668825 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.695334 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5933 2023-05-24 21:29:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.706303 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11115 2023-05-24 21:25:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.714514 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.740033 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.747249 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.762979 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.810626 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.814033 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.821724 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.824499 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.827996 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.830882 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.837309 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.840583 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.846665 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.865083 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.871216 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-21 16:37:56.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.892752 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7995 2023-05-24 21:20:29.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-05-24 21:17:30.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17287 2023-05-24 21:17:28.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.896490 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.900558 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.907561 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.924582 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2925 2023-05-21 12:09:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2852 2023-05-21 11:00:00.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1899 2023-05-21 14:30:07.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22539 2023-05-21 14:29:12.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.940182 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.968009 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:13.981589 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2895 2023-07-11 09:22:19.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    39903 2023-07-09 14:27:25.000000 nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-07-12 10:12:12.072036 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    15289 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-07-12 10:12:11.000000 nef_pipelines-0.1.43/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.43/tox.ini
```

### Comparing `nef_pipelines-0.1.42/.github/workflows/ci.yml` & `nef_pipelines-0.1.43/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.43/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/.pre-commit-config.yaml` & `nef_pipelines-0.1.43/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/CHANGELOG.md` & `nef_pipelines-0.1.43/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -159,7 +159,11 @@
 a  number of bug fixes in the sparky and echidna tools
 
 ## version 0.1.42
 
 add the ability to unassign frames in general with support for different sequence_code
 unassignment strategies and the ability to choose what is unassigned (chain_code, sequence_code
 residue_name atom_name)
+
+## version 0.1.43
+fasta input tool can read RNA/DNA sequences
+improvemenets to the xplor distance restraint reader to suppport CNS
```

### Comparing `nef_pipelines-0.1.42/CONTRIBUTING.md` & `nef_pipelines-0.1.43/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/LICENSE.txt` & `nef_pipelines-0.1.43/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/PKG-INFO` & `nef_pipelines-0.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.42
+Version: 0.1.43
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.42/README.md` & `nef_pipelines-0.1.43/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/TODO.md` & `nef_pipelines-0.1.43/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.43/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.43/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/release_to_pypi.sh` & `nef_pipelines-0.1.43/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/setup.cfg` & `nef_pipelines-0.1.43/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/setup.py` & `nef_pipelines-0.1.43/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.43/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     atom_list_1: List[AtomLabel]
     atom_list_2: List[AtomLabel]
 
     target_distance: float
     distance_minus: float
     distance_plus: float
 
+    comment: str = None
+
 
 @dataclass
 class DihedralRestraint:
     atom_1: AtomLabel
     atom_2: AtomLabel
     atom_3: AtomLabel
     atom_4: AtomLabel
```

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.43/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/main.py` & `nef_pipelines-0.1.43/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_unassign.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/frames/test_unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/unassign.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/frames/unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.43/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,135 @@
-from itertools import chain, cycle, islice, zip_longest
+import warnings
+from argparse import Namespace
 from pathlib import Path
-from typing import Iterable, List
+from typing import List
 
 import typer
-from Bio.SeqIO.FastaIO import SimpleFastaParser
-from ordered_set import OrderedSet
 
-from nef_pipelines.lib.sequence_lib import (
-    chain_code_iter,
-    offset_chain_residues,
-    sequence_3let_to_res,
-    sequence_to_nef_frame,
-    translate_1_to_3,
-)
+from nef_pipelines.lib.sequence_lib import sequence_to_nef_frame
 from nef_pipelines.lib.structures import SequenceResidue
 from nef_pipelines.lib.typer_utils import get_args
 from nef_pipelines.lib.util import (
     exit_error,
     parse_comma_separated_options,
     process_stream_and_add_frames,
 )
-from nef_pipelines.transcoders.fasta import import_app
+from nef_pipelines.transcoders.pdbx import import_app
 
 app = typer.Typer()
 
+CHAINS_HELP = """chains [or segid] to read', metavar='<CHAIN-CODE>, multiple chains can be added as a comma joined list
+                [eg A.B.C] ] or by calling this option mutiple times"""
 NO_CHAIN_START_HELP = """don't include the start chain link type on a chain for the first residue [linkage will be
                          middle] for the named chains. Either use a comma joined list of chains [e.g. A,B] or call this
                          option multiple times to set chain starts for multiple chains"""
 NO_CHAIN_END_HELP = """don't include the end chain link type on a chain for the last residue [linkage will be
                        middle] for the named chains. Either use a comma joined list of chains [e.g. A,B] or call this
                        option multiple times to set chain ends for multiple chains"""
 
 
-# todo add comment to other sequences etc
-@import_app.command()
+# noinspection PyUnusedLocal
+@import_app.command(no_args_is_help=True)
 def sequence(
-    chain_codes: List[str] = typer.Option(
-        [],
-        "--chains",
-        help="chain codes to use for the imported chains, can be a a comma separated list or can be called "
-        "multiple times",
-        metavar="<CHAIN-CODES>",
-    ),
-    starts: List[str] = typer.Option(
-        [],
-        "--starts",
-        help="first residue number of sequences can be a comma separated list or ",
-        metavar="<START>",
+    chain_codes: List[str] = typer.Option(None, "-c", "--chains", help=CHAINS_HELP),
+    use_segids: bool = typer.Option(
+        False, "-s", "--segid", help="use segid instead of chain"
     ),
     no_chain_starts: List[str] = typer.Option(
         [], "--no-chain-start", help=NO_CHAIN_START_HELP
     ),
     no_chain_ends: List[str] = typer.Option(
         [], "--no-chain-end", help=NO_CHAIN_END_HELP
     ),
-    entry_name: str = typer.Option("fasta", help="a name for the entry if required"),
-    pipe: List[Path] = typer.Option(
-        None,
-        metavar="|PIPE|",
-        help="pipe to read NEF data from, for testing [overrides stdin !use stdin instead!]",
-    ),
-    file_names: List[Path] = typer.Argument(
-        ..., help="the file to read", metavar="<FASTA-FILE>"
+    entry_name: str = typer.Option(
+        "pdb", help="a name for the nef entry if not updating an existing entry"
     ),
+    file_name: Path = typer.Argument(..., help="input pdb file", metavar="<PDB-FILE>"),
 ):
-    """- convert fasta sequence to nef"""
+    """extracts a sequence from a pdb file"""
 
     chain_codes = parse_comma_separated_options(chain_codes)
-    if not chain_codes:
-        chain_codes = ["A"]
-
     no_chain_starts = parse_comma_separated_options(no_chain_starts)
-    if not no_chain_starts:
-        no_chain_starts = [False]
-
     no_chain_ends = parse_comma_separated_options(no_chain_ends)
-    if no_chain_ends:
-        no_chain_ends = [False]
-
-    starts = [int(elem) for elem in parse_comma_separated_options(starts)]
-    if not starts:
-        starts = [1]
-
-    args = get_args()
-
-    args.chain_codes = chain_codes
-    args.no_chain_starts = no_chain_starts
-    args.no_chain_ends = no_chain_ends
-    args.starts = starts
-
-    process_sequences(args)
 
+    try:
+        args = get_args()
 
-def process_sequences(args):
-    fasta_frames = []
+        process_sequence(args)
 
-    chain_code_iterator = chain_code_iter(args.chain_codes)
-    fasta_sequences = OrderedSet()
-    for file_path in args.file_names:
-        fasta_sequences.update(read_sequences(file_path, chain_code_iterator))
+    except Exception as e:
+        exit_error(f"reading sequence failed because {e}", e)
 
-    read_chain_codes = residues_to_chain_codes(fasta_sequences)
 
-    offsets = _get_sequence_offsets(read_chain_codes, args.starts)
+def process_sequence(args: Namespace):
 
-    fasta_sequences = offset_chain_residues(fasta_sequences, offsets)
+    pdb_sequences = read_sequences(
+        args.file_name, args.chain_codes, use_segids=args.use_segids
+    )
 
-    fasta_sequences = sorted(fasta_sequences)
+    if len(pdb_sequences) == 0:
+        exit_error(f"no chains read from {args.file_name}")
 
-    fasta_frames.append(sequence_to_nef_frame(fasta_sequences))
+    pdb_frame = sequence_to_nef_frame(
+        pdb_sequences, set(args.no_chain_starts), set(args.no_chain_ends)
+    )
 
-    entry = process_stream_and_add_frames(fasta_frames, args)
+    # TODO: need a a warning if the sequence already exists in a molecular system and ability to merge
+    entry = process_stream_and_add_frames(
+        [
+            pdb_frame,
+        ],
+        args,
+    )
 
     print(entry)
 
 
-def _get_sequence_offsets(chain_codes: List[str], starts: List[int]):
+def read_sequences(path, target_chain_codes, use_segids=False):
 
-    offsets = [start - 1 for start in starts]
-    cycle_starts = chain(
-        offsets,
-        cycle(
-            [
-                0,
-            ]
-        ),
-    )
-    offsets = list(islice(cycle_starts, len(chain_codes)))
+    from Bio.PDB.PDBExceptions import PDBConstructionWarning
 
-    return {chain_code: offset for chain_code, offset in zip(chain_codes, offsets)}
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", PDBConstructionWarning)
 
+        from Bio.PDB.PDBParser import PDBParser
 
-def residues_to_chain_codes(residues: List[SequenceResidue]) -> List[str]:
-    return list(OrderedSet([residue.chain_code for residue in residues]))
+        parser = PDBParser(PERMISSIVE=1)
+        structure = parser.get_structure("pdb", path)
+        model = structure[0]
 
+        sequences = []
 
-# could do with taking a list of offsets
-# noinspection PyUnusedLocal
-def read_sequences(path: Path, chain_codes: Iterable[str]) -> List[SequenceResidue]:
-
-    residues = OrderedSet()
-    try:
-        with open(path) as handle:
-            try:
-                sequences = list(SimpleFastaParser(handle))
-            except Exception as e:
-                # check if relative to os.getcwd
-                exit_error(f"Error reading fasta file {str(path)}", e)
-
-            number_sequences = len(sequences)
+        if not use_segids:
+            for chain in model:
+                id = chain.id.strip()
+                if len(id) == 0:
+                    use_segids = True
 
-            # read as many chain codes as there are sequences
-            # https://stackoverflow.com/questions/16188270/get-a-fixed-number-of-items-from-a-generator
+        all_chains = len(target_chain_codes) == 0
 
-            chain_codes = list(islice(chain_codes, number_sequences))
+        for chain in model:
+            for residue in chain:
+                chain_code = residue.segid if use_segids else chain.id
+                chain_code = chain_code.strip()
 
-            for (meta_data, sequence), chain_code in zip_longest(
-                sequences, chain_codes
-            ):
+                if not all_chains and chain_code not in target_chain_codes:
+                    continue
 
-                sequence_3_let = translate_1_to_3(sequence)
-                chain_residues = sequence_3let_to_res(sequence_3_let, chain_code)
+                hetero_atom_flag, sequence_code, _ = residue.get_id()
 
-                residues.update(chain_residues)
+                if len(hetero_atom_flag.strip()) != 0:
+                    continue
 
-    except IOError as e:
-        exit_error(f"couldn't open {path} because:\n{e}", e)
+                if chain_code == "":
+                    exit_error(
+                        f"residue with no chain code found for file {path} sequence_code is {sequence_code} \
+                        residue_name is {residue.get_resname()}"
+                    )
+                residue = SequenceResidue(
+                    chain_code=chain_code,
+                    sequence_code=sequence_code,
+                    residue_name=residue.get_resname(),
+                )
+                sequences.append(residue)
 
-    return residues
+    return sequences
```

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from argparse import Namespace
 from itertools import zip_longest
 from pathlib import Path
 from typing import List
 
 import typer
 
-from nef_pipelines.lib.nef_lib import file_name_path_to_frame_name
+from nef_pipelines.lib.nef_lib import (
+    add_frames_to_entry,
+    file_name_path_to_frame_name,
+    read_entry_from_file_or_stdin_or_exit_error,
+)
 from nef_pipelines.lib.sequence_lib import (
     ANY_CHAIN,
-    get_sequence_or_exit,
     residues_to_residue_name_lookup,
+    sequence_from_entry_or_exit,
 )
-from nef_pipelines.lib.util import (
-    parse_comma_separated_options,
-    process_stream_and_add_frames,
-)
+from nef_pipelines.lib.util import parse_comma_separated_options
 from nef_pipelines.transcoders.xplor import import_app
 from nef_pipelines.transcoders.xplor.xplor_lib import (
     _exit_if_chains_and_filenames_dont_match,
     distance_restraints_to_nef,
     read_distance_restraints_or_exit_error,
 )
 
@@ -48,17 +48,19 @@
     use_chains: bool = typer.Option(False, "--use-chains", help=USE_CHAINS_HELP),
     file_names: List[Path] = typer.Argument(
         ..., help="input distance restraint tables", metavar="<DIHEDRALS-TBL>"
     ),
 ):
     """- read xplor distance restraints [note: currently limited to 'single' atom selections]"""
 
-    chains = parse_comma_separated_options(chains)
+    entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
-    sequence = get_sequence_or_exit(input)
+    sequence = sequence_from_entry_or_exit(entry)
+
+    chains = parse_comma_separated_options(chains)
 
     residue_name_lookup = residues_to_residue_name_lookup(sequence)
 
     distance_restraints = []
 
     _exit_if_chains_and_filenames_dont_match(chains, file_names)
 
@@ -72,12 +74,10 @@
         )
 
     for i, (restraint_list, frame_name) in enumerate(
         zip(distance_restraints, frame_names)
     ):
         nef_restraints = distance_restraints_to_nef(restraint_list, frame_name)
 
-    entry = process_stream_and_add_frames(
-        [nef_restraints], Namespace(pipe=None, entry_name="xplor_distance_restraints")
-    )
+    entry = add_frames_to_entry(entry, [nef_restraints])
 
     print(entry)
```

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.43/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     ParseResults,
     Regex,
     Suppress,
     Word,
     ZeroOrMore,
     alphanums,
     nums,
+    rest_of_line,
 )
 from pyparsing.common import pyparsing_common as ppc
 
 from nef_pipelines.lib.nef_lib import UNUSED, PotentialTypes
 from nef_pipelines.lib.sequence_lib import ANY_CHAIN, replace_chain_in_atom_labels
 from nef_pipelines.lib.structures import (
     AtomLabel,
@@ -65,14 +66,17 @@
 #
 #   SEGIdentifier <*segment-name*> selects all atoms that match the specified segment name (Section 3.7)
 #                                  or a wildcard (Section 2.6) of it.
 
 LEFT_PARENTHESIS = "("
 RIGHT_PARENTHESIS = ")"
 
+SINGLE_QUOTE = "'"
+DOUBLE_QUOTE = '"'
+
 ASSIGN = "assign"
 NEF_DIHEDRAL_RESTRAINT = "nef_dihedral_restraint"
 XPLOR_COMMENT_TOKEN = "!"
 DISTANCE_PLUS = "d_plus"
 DISTANCE_MINUS = "d_minus"
 DISTANCE = "d"
 EXPONENT = "exponent"
@@ -129,14 +133,16 @@
 SEQUENCE_CODE_4 = "sequence_code_4"
 RESIDUE_NAME_4 = "residue_name_4"
 ATOM_4 = "atom_name_4"
 WEIGHT = "weight"
 TARGET_VALUE = "target_value"
 LOWER_LIMIT = "lower_limit"
 UPPER_LIMIT = "upper_limit"
+EXTRA_INFO = "extra_info"
+CCPN_COMMENT = "ccpn_comment"
 
 DISTANCE_RESTRAINT_TAGS = [
     INDEX,
     RESTRAINT_ID,
     RESTRAINT_COMBINATION_ID,
     CHAIN_CODE_1,
     SEQUENCE_CODE_1,
@@ -272,17 +278,17 @@
 _residue_factor = (_residue_literal + _residue_number)(RESIDUE_FACTOR)
 
 _named_resid = partial(_as_named_single_token, RESID)
 _residue_factor.set_parse_action(_named_resid)
 
 # atom factor
 _atom_literal = Suppress(CaselessLiteral(ATOM_NAME_LITERAL))
-_atom_label = Word(alphanums + ATOM_WILDCARDS).set_results_name(
-    ATOM, list_all_matches=True
-)
+_atom_label = Word(
+    alphanums + ATOM_WILDCARDS + SINGLE_QUOTE + DOUBLE_QUOTE
+).set_results_name(ATOM, list_all_matches=True)
 _atom_factor = (_atom_literal + _atom_label)(ATOM_FACTOR)
 
 _named_atom = partial(_as_named_single_token, ATOM)
 _atom_factor.set_parse_action(_named_atom)
 
 # segment factor
 _segid_literal = Suppress(_expand_literal(SEGIMENT_IDENTIFIER_LITERAL))
@@ -330,14 +336,15 @@
 _distance_restraint = Group(
     Suppress(_expand_literal(ASSIGN))
     + _selection.set_results_name(ATOMS_1)
     + _selection.set_results_name(ATOMS_2)
     + ppc.number.set_results_name(DISTANCE).setParseAction(ppc.convertToFloat)
     + ppc.number.set_results_name(DISTANCE_MINUS).setParseAction(ppc.convertToFloat)
     + ppc.number.set_results_name(DISTANCE_PLUS).setParseAction(ppc.convertToFloat)
+    + rest_of_line.set_results_name(EXTRA_INFO)
 )
 
 _distance_restraints = OneOrMore(_distance_restraint)
 
 
 def _remove_xplor_comments(data_lines: List[str]) -> List[str]:
     result = []
@@ -403,23 +410,25 @@
     if valid:
         residue_type_key = chain_code, str(sequence_code)
         if residue_type_key in residue_types:
             residue_type = residue_types[residue_type_key]
         else:
             valid = False
             residue_type = None
-            invalid_reason = f"the residue type for chain code: {chain_code} sequence code {sequence_code} is not known"
+            # TODO print out sequence...
+            invalid_reason = f"""the residue type for chain code: {chain_code} sequence code {sequence_code} is not
+                                 known, check this residue is present in you input sequence!"""
 
     if valid:
         residue = SequenceResidue(chain_code, sequence_code, residue_type)
         result = AtomLabel(residue, atom_name)
 
     if not valid:
         raise XPLORParseException(
-            f"Couldn't get a single restraint from {parsed} because {invalid_reason}"
+            f"Couldn't get a single restraint from {parsed} \n because {invalid_reason}"
         )
 
     return result
 
 
 def read_distance_restraints_or_exit_error(
     file_path: Path,
@@ -439,21 +448,24 @@
 
     restraint_text = read_from_file_or_exit(
         file_path, f"xplor distance restraints from {file_path}"
     )
 
     file_path_display_name = get_display_file_name(file_path)
 
-    restraints = parse_distance_restraints(
-        restraint_text,
-        residue_name_lookup,
-        file_path_display_name,
-        chain_code,
-        use_chains,
-    )
+    try:
+        restraints = parse_distance_restraints(
+            restraint_text,
+            residue_name_lookup,
+            file_path_display_name,
+            chain_code,
+            use_chains,
+        )
+    except XPLORParseException as e:
+        exit_error("there was an error", e)
 
     return restraints
 
 
 def distance_restraints_to_nef(
     restraints: List[DistanceRestraint], frame_name: str
 ) -> Saveframe:
@@ -461,40 +473,56 @@
     convert a list of DistanceRestraints to a new distance restraint save frame
     :param restraints: the restraints
     :param frame_name: the name of the new save frame
     :return: a new save frame
     """
     loop = Loop.from_scratch(category="nef_distance_restraint")
 
+    have_comments = False
+    for restraint in restraints:
+        if restraint.comment is not None:
+            have_comments = True
+            break
+
     for tag in DISTANCE_RESTRAINT_TAGS:
         loop.add_tag(tag)
 
+    if have_comments:
+        loop.add_tag(CCPN_COMMENT)
+
     for i, restraint in enumerate(restraints, start=1):
         selection_1 = restraint.atom_list_1[0]
         selection_2 = restraint.atom_list_2[0]
         d = restraint.target_distance
         d_minus = restraint.distance_minus
         d_plus = restraint.distance_plus
-
+        comment = (
+            restraint.comment
+            if restraint.comment is not None or restraint.comment != ""
+            else UNUSED
+        )
         row = {
             INDEX: i,
             RESTRAINT_ID: i,
             RESTRAINT_COMBINATION_ID: UNUSED,
             CHAIN_CODE_1: selection_1.residue.chain_code,
             SEQUENCE_CODE_1: selection_1.residue.sequence_code,
             ATOM_1: selection_1.atom_name,
             CHAIN_CODE_2: selection_2.residue.chain_code,
             SEQUENCE_CODE_2: selection_2.residue.sequence_code,
             ATOM_2: selection_2.atom_name,
             WEIGHT: 1.0,
             TARGET_VALUE: round(d, DEFAULT_PRECISION),
-            LOWER_LIMIT: round(d - d_minus, DEFAULT_PRECISION),
-            UPPER_LIMIT: round(d + d_plus, DEFAULT_PRECISION),
+            LOWER_LIMIT: round(d_minus, DEFAULT_PRECISION),
+            UPPER_LIMIT: round(d_plus, DEFAULT_PRECISION),
         }
 
+        if have_comments:
+            row[CCPN_COMMENT] = comment
+
         loop.add_data([row])
 
     save_frame_name = f"nef_distance_restraint_list_{frame_name}"
 
     save_frame = Saveframe.from_scratch(save_frame_name, "nef_distance_restraint")
 
     save_frame.add_tag("sf_category", "nef_distance_restraint_list")
@@ -575,15 +603,15 @@
             if len(new_line.strip()) > 0:
                 new_lines.append(new_line)
         else:
             new_lines.append(line)
 
     new_lines = "\n".join(new_lines)
 
-    restraints = new_lines.split(ASSIGN)
+    restraints = list(_expand_literal(ASSIGN).split(new_lines))
 
     if restraints[0] == "":
         restraints = restraints[1:]
 
     return [f"{ASSIGN} {restraint}" for restraint in restraints]
 
 
@@ -765,21 +793,25 @@
 
         if use_chains and chain_code != ANY_CHAIN:
             atom_selections = replace_chain_in_atom_labels(atom_selections, chain_code)
 
         target_distance = restraint.get(DISTANCE)
         distance_minus = restraint.get(DISTANCE_MINUS)
         distance_plus = restraint.get(DISTANCE_PLUS)
+        comment = restraint.get(EXTRA_INFO).strip()
+        if comment == "":
+            comment = None
 
         atom_selections = [[atom_selection] for atom_selection in atom_selections]
         restraint = DistanceRestraint(
             *atom_selections,
             target_distance=target_distance,
             distance_minus=target_distance - distance_minus,
             distance_plus=target_distance + distance_plus,
+            comment=comment,
         )
 
         restraints.append(restraint)
 
     return restraints
```

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.43/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.42
+Version: 0.1.43
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.42/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.43/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.42/tox.ini` & `nef_pipelines-0.1.43/tox.ini`

 * *Files identical despite different names*

