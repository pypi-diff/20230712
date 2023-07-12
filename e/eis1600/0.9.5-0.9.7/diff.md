# Comparing `tmp/eis1600-0.9.5.tar.gz` & `tmp/eis1600-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.5.tar", last modified: Wed Jun 21 13:43:08 2023, max compression
+gzip compressed data, was "eis1600-0.9.7.tar", last modified: Wed Jul 12 09:03:52 2023, max compression
```

## Comparing `eis1600-0.9.5.tar` & `eis1600-0.9.7.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.5/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-21 13:43:08.048154 eis1600-0.9.5/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-06-08 08:10:00.000000 eis1600-0.9.5/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.5/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.5/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.5/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.5/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.5/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3476 2023-06-14 10:59:59.000000 eis1600-0.9.5/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.5/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.032154 eis1600-0.9.5/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.5/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.5/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-14 10:40:04.000000 eis1600-0.9.5/eis1600/gazetteers/data/toponyms_gazetteer.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.036154 eis1600-0.9.5/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.5/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.5/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.5/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.5/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.036154 eis1600-0.9.5/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.5/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.5/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.5/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.5/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.5/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.5/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3152 2023-06-16 13:52:38.000000 eis1600-0.9.5/eis1600/helper/md_tags_to_bio.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.5/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11212 2023-06-08 08:03:01.000000 eis1600-0.9.5/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.5/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.5/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.040154 eis1600-0.9.5/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.5/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.5/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.5/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.5/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.5/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.5/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.040154 eis1600-0.9.5/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.5/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.5/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.5/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.5/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9595 2023-06-08 09:08:43.000000 eis1600-0.9.5/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.5/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8824 2023-06-14 10:59:59.000000 eis1600-0.9.5/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.5/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2935 2023-06-08 07:49:05.000000 eis1600-0.9.5/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.5/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6543 2023-06-08 07:58:41.000000 eis1600-0.9.5/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.5/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.5/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.5/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.5/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.5/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.5/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.5/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.5/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.5/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/eis1600/toponyms/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.5/eis1600/toponyms/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.5/eis1600/toponyms/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2959 2023-06-08 09:06:21.000000 eis1600-0.9.5/eis1600/toponyms/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      903 2023-06-20 14:15:34.000000 eis1600-0.9.5/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2083 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      852 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-21 13:43:08.048154 eis1600-0.9.5/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2445 2023-06-16 10:55:21.000000 eis1600-0.9.5/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.829389 eis1600-0.9.7/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.7/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-07-12 09:03:52.829389 eis1600-0.9.7/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-07-03 10:37:00.000000 eis1600-0.9.7/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.7/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.7/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6116 2023-07-10 10:56:25.000000 eis1600-0.9.7/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5111 2023-07-07 07:47:22.000000 eis1600-0.9.7/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.7/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3476 2023-06-14 10:59:59.000000 eis1600-0.9.7/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.7/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.7/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.7/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-14 10:40:04.000000 eis1600-0.9.7/eis1600/gazetteers/data/toponyms_gazetteer.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.7/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      393 2023-07-12 08:58:30.000000 eis1600-0.9.7/eis1600/helper/EvalResultsEncoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.7/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.7/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.7/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.7/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.7/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6547 2023-07-12 09:00:06.000000 eis1600-0.9.7/eis1600/helper/eval_date_model.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.7/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.7/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.7/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3915 2023-07-06 08:53:43.000000 eis1600-0.9.7/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.7/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11325 2023-07-12 07:09:47.000000 eis1600-0.9.7/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2746 2023-07-12 07:01:24.000000 eis1600-0.9.7/eis1600/helper/top_tags_to_bio.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.7/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1667 2023-06-23 09:40:16.000000 eis1600-0.9.7/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.7/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.7/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.7/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2945 2023-07-10 10:38:20.000000 eis1600-0.9.7/eis1600/markdown/md_to_bio.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.7/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.7/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.7/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.7/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7927 2023-06-23 09:37:32.000000 eis1600-0.9.7/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.7/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.7/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9846 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.7/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10503 2023-06-23 07:37:45.000000 eis1600-0.9.7/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.7/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3560 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.7/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7565 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.7/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.7/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.7/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.7/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.7/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5019 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.7/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.7/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.7/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.829389 eis1600-0.9.7/eis1600/toponyms/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.7/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2371 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/toponyms/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3153 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/toponyms/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1076 2023-07-12 07:17:22.000000 eis1600-0.9.7/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2185 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      915 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      108 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-07-12 09:03:52.829389 eis1600-0.9.7/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2562 2023-07-12 09:02:05.000000 eis1600-0.9.7/setup.py
```

### Comparing `eis1600-0.9.5/LICENSE` & `eis1600-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/PKG-INFO` & `eis1600-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.5
+Version: 0.9.7
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -245,7 +245,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7, <3.9
 Description-Content-Type: text/markdown
 Provides-Extra: NER
+Provides-Extra: EVAL
```

### Comparing `eis1600-0.9.5/README.md` & `eis1600-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/dates/Date.py` & `eis1600-0.9.7/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/dates/date_patterns.py` & `eis1600-0.9.7/eis1600/dates/date_patterns.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from eis1600.helper.ar_normalization import normalize_dict
 from eis1600.helper.markdown_patterns import WORD
 
 ONES = {
         'واحد': 1, 'احدى': 1, 'احد': 1, 'اثنين': 2, 'اثنتين': 2, 'اثنتي': 2, 'ثلاث': 3, 'ثلث': 3, 'اربع': 4, 'خمس': 5,
         'ست': 6, 'سبع': 7, 'ثماني': 8, 'ثمان': 8, 'تسع': 9
 }
+# TODO integrate
+INDETERMINATES = ['بضع', 'في حدود', 'نيف']
+
 ONES_NOR = normalize_dict(ONES)
 TEN = {
         'عشرة': 10, 'عشري': 10, 'عشر': 10, 'عشرين': 20, 'ثلاثين': 30, 'اربعين': 40, 'خمسين': 50, 'ستين': 60,
         'سبعين': 70,
         'ثمانين': 80, 'تسعين': 90
 }
 TEN_NOR = normalize_dict(TEN)
@@ -62,22 +65,31 @@
 AR_ONES_DAY = '|'.join([denormalize(key) for key in DAY_ONES.keys()])
 AR_TEN_DAY = '|'.join([denormalize(key) for key in DAY_TEN.keys()])
 AR_WEEKDAY = '|'.join(['(?:' + r'\s'.join(key.split()) + ')' for key in WEEKDAYS.keys()])
 DATE = r'(?P<context>' + WORD + r'{0,10}?' + r'(?:\s(?:ف[يى]|تقريبا))?' + WORD + r'{0,9}?)' + \
        r'(?:\s(?P<weekday>' + AR_WEEKDAY + r'))?' + \
        r'(?:\s(:?ال)?(?P<day_ones>' + AR_ONES_DAY + r'))?(?:\s(:?و)?(:?ال)?(?P<day_ten>' + AR_TEN_DAY + r'))?' + \
        r'(?:\s(?:(?:من\s)?(?:شهر\s)?)?(?:ال)?(?P<month>' + AR_MONTHS + r')(?:\s(?:من|ف[يى])(?:\sشهور)?)?)?' + \
-       r'\s(?P<sana>سن[ةه]|عام)(?:\s(?P<ones>' + AR_ONES + r'))?' + \
-       r'(?:\s[و]?(?P<ten>' + AR_TEN + r'))?' + \
-       r'(?:\s[و]?(?P<hundred>' + AR_HUNDRED + r'))?(?=(?:' + WORD + r'|[\s\.,]|$))'
+       r'\s(?P<sana>سن[ةه]|عام)' + \
+       r'(?P<year>' + \
+              r'(?:\s(?P<ones>' + AR_ONES + r'))?' + \
+              r'(?:\s[و]?(?P<ten>' + AR_TEN + r'))?' + \
+              r'(?:\s[و]?(?P<hundred>' + AR_HUNDRED + r'))?' + \
+       r')' + \
+       r'(?=(?:' + WORD + r'|[\s\.,]|$))'
 
 DATE_PATTERN = compile(DATE)
 MONTH_PATTERN = compile(AR_MONTHS)
 
-DATE_CATEGORIES = {
-        'ولد': 'B', 'مولد': 'B', 'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D', 'حج': 'P',
-        'سمع': 'K', 'قرا': 'K', 'استقر': 'O', 'اجاز': 'K', 'انفصل': 'O', 'لقي': 'M'
+DATE_CATEGORIES_DICT = {
+        'ولد': 'B', 'مولد': 'B',
+        'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D',
+        'حج': 'P',
+        'سمع': 'K', 'قرا': 'K', 'اجاز': 'K',
+        'استقر': 'O', 'انفصل': 'O'
 }
-DATE_CATEGORIES_NOR = normalize_dict(DATE_CATEGORIES)
+DATE_CATEGORIES_NOR = normalize_dict(DATE_CATEGORIES_DICT)
 
-AR_DATE_CATEGORIES = '|'.join([denormalize(key) for key in DATE_CATEGORIES.keys()])
+AR_DATE_CATEGORIES = '|'.join([denormalize(key) for key in DATE_CATEGORIES_DICT.keys()])
 DATE_CATEGORY_PATTERN = compile(r'\s[وف]?(?P<date_category>' + AR_DATE_CATEGORIES + r')')
+
+DATE_CATEGORIES = list(set(DATE_CATEGORIES_DICT.values())) + ["X"]
```

### Comparing `eis1600-0.9.5/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.7/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/gazetteers/Toponyms.py` & `eis1600-0.9.7/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.7/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.7/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-0.9.7/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/EntityTags.py` & `eis1600-0.9.7/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/Singleton.py` & `eis1600-0.9.7/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/ar_normalization.py` & `eis1600-0.9.7/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.7/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/markdown_methods.py` & `eis1600-0.9.7/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.7/eis1600/helper/markdown_patterns.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,17 @@
 TAG_AND_TEXT_SAME_LINE = r'([$@]+' + NOR_DIGIT_NOR_AR_STR + r'\d*' + NOR_DIGIT_NOR_AR_STR + r') ?((?:[(\[] ?)?' + AR_STR + r')'
 UID_TAG_AND_TEXT_SAME_LINE_PATTERN = compile(
         r'(_ء_#=\d{12}= )' + TAG_AND_TEXT_SAME_LINE)
 MIU_TAG_AND_TEXT_PATTERN = compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
 
 # MIU entity tags
 entity_tags = '|'.join(EntityTags.instance().get_entity_tags())
-ENTITY_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:[A-Z0-9]+)?')
-YEAR_PATTERN = compile(r'Ü?Y\d{1,2}(?P<cat>[A-Z])(?P<written>\d{4})(?P<i>I)?Y(?P<real>\d{4})?')
+ENTITY_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:(?P<sub_cat>[A-Z]+)|['
+                                                               r'A-Z0-9]+)?\b')
+YEAR_PATTERN = compile(r'Ü?Y(?P<num_tokens>\d{1,2})(?P<cat>[A-Z])(?P<written>\d{4}|None)(?P<i>I)?Y(?P<real>\d{4})?')
 AGE_PATTERN = compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
 nasab_tags = '|'.join(EntityTags.instance().get_nasab_tags())
 NASAB_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + nasab_tags + r')(?P<length>\d{1,2})')
 
 # EIS1600 light mARkdown
 HEADING_OR_BIO_PATTERN = compile(r'# [|$]+')
 MIU_LIGHT_OR_EIS1600_PATTERN = compile(r'#|_ء_#')
```

### Comparing `eis1600-0.9.5/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.7/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/helper/repo.py` & `eis1600-0.9.7/eis1600/helper/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 
 from eis1600.helper.markdown_patterns import FIXED_POETRY_OLD_PATH_PATTERN
 
 # Path variables
 MIU_REPO = 'EIS1600_MIUs/'
 TEXT_REPO = 'OpenITI_EIS1600_Texts/'
 TRAINING_DATA_REPO = 'Training_Data/'
+TRAINING_RESULTS_REPO = 'Training_Results/'
 GAZETTEERS_REPO = 'gazetteers/'
 MC_REPO = 'MasterChronicle/'
+BACKEND_REPO = 'backend/'
+TOPO_TRAINING_REPO = 'topo_training/data/'
 
 
 def get_entry(file_name: str, checked_entry: bool) -> str:
     """Formats README entry for that file_name.
 
     Only used internally.
     :param str file_name: The name of the file whose entry is added to the README
```

### Comparing `eis1600-0.9.5/eis1600/helper/yml_to_json.py` & `eis1600-0.9.7/eis1600/helper/yml_to_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from sys import argv
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from pathlib import Path
 import jsonpickle
 from p_tqdm import p_uimap
 
 from eis1600.processing.preprocessing import get_yml
-from eis1600.helper.repo import MC_REPO, TRAINING_DATA_REPO
+from eis1600.helper.repo import BACKEND_REPO, TRAINING_DATA_REPO
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to generate JSON from MIU YAMLHeaders.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
     args = arg_parser.parse_args()
 
     debug = args.debug
     with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
-    infiles = [TRAINING_DATA_REPO + 'gold_standard_nasab/' + file for file in files_txt if Path(
-            TRAINING_DATA_REPO + 'gold_standard_nasab/' + file
+    infiles = [TRAINING_DATA_REPO + 'gold_standard_topo/' + file for file in files_txt if Path(
+            TRAINING_DATA_REPO + 'gold_standard_topo/' + file
     ).exists()]
 
     res = []
     if debug:
         for file in infiles[:10]:
             print(file)
             res.append(get_yml(file))
@@ -34,13 +34,13 @@
     yml_dict = []
     for path, yml in res:
         key = path.replace(TRAINING_DATA_REPO + 'gold_standard_nasab/', '').replace('.EIS1600', '')
         author, text, version, UID = key.split('.')
         yml_init = {'author': author, 'text': text, 'version': version, 'UID': UID}
         yml_dict.append(yml.to_json(yml_init))
 
-    with open(MC_REPO + 'masterchronicleapp/src/data.json', 'w', encoding='utf-8') as fh:
+    with open(BACKEND_REPO + 'data.json', 'w', encoding='utf-8') as fh:
         jsonpickle.set_encoder_options('json', indent=4, ensure_ascii=False)
         json_str = jsonpickle.encode(yml_dict, unpicklable=False)
         fh.write(json_str)
 
     print('Done')
```

### Comparing `eis1600-0.9.5/eis1600/markdown/UIDs.py` & `eis1600-0.9.7/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/markdown/insert_uids.py` & `eis1600-0.9.7/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/markdown/methods.py` & `eis1600-0.9.7/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/markdown/update_uids.py` & `eis1600-0.9.7/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.7/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.7/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.7/eis1600/miu/YAMLHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     :ivar List[str] dates_headings: List of dates tags contained in headings.
     :ivar List[int] dates: List of dates contained in the text.
     :ivar Dict onomstics: contains onomastic elements by category.
     :ivar str category: String categorising the type of the entry, bio, chr, dict, etc.
     """
     # Only attributes named in the following list are allowed to be added to the YAMLHeader - add any new attribute
     # to that list
-    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambigious_toponyms', 'toponyms',
-                              'settlements', 'provinces', 'edges_settlements', 'edges_provinces']
+    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambiguous_toponyms', 'toponyms',
+                              'settlements', 'provinces', 'edges_settlements', 'edges_provinces', 'books', 'miscs']
 
     @staticmethod
-    def __parse_yml_val(val: str, key: Optional[str] = None) -> Any:
+    def __parse_yml_val(val: str) -> Any:
         if val.isdigit():
             return int(val)
         if len(val.split('.')) == 2 and val.split('.')[0].isdigit() and val.split('.')[1].isdigit():
             return float(val)
         elif val == 'True':
             return True
         elif val == 'False':
@@ -81,21 +81,21 @@
                     else:
                         yml[dict_key] = dict_val
                     level.pop()
 
                 if intend and intend == len(level) and val != '':
                     # Stay on level and add key, val to the respective dict
                     curr_dict = level[-1][1]
-                    curr_dict[key] = YAMLHandler.__parse_yml_val(val, key)
+                    curr_dict[key] = YAMLHandler.__parse_yml_val(val)
                 elif val == '':
                     # Go one level deeper, add key and empty dict for that new level
                     level.append((key, {}))
                 else:
                     # Add key, val to the top level
-                    yml[key] = YAMLHandler.__parse_yml_val(val, key)
+                    yml[key] = YAMLHandler.__parse_yml_val(val)
 
         if len(level):
             dict_key = level[-1][0]
             dict_val = level[-1][1]
             yml[dict_key] = dict_val
 
         return yml
@@ -104,72 +104,66 @@
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
         self.category = None
         self.headings = None
         self.dates_headings = None
 
         for key in YAMLHandler.__attr_from_annotation:
-            if key == 'ambigious_toponyms':
+            if key == 'ambiguous_toponyms':
                 self.__setattr__(key, False)
             else:
                 self.__setattr__(key, None)
 
         if yml:
             for key, val in yml.items():
                 if key == 'headings':
                     val = HeadingTracker(val)
+                if key == 'ambigious':
+                    # Fix typo
+                    key = 'ambiguous'
                 self.__setattr__(key, val)
 
     @classmethod
     def from_yml_str(cls, yml_str: str) -> YAMLHandler:
         """Return instance with attr set from the yml_str."""
         return cls(YAMLHandler.__parse_yml(yml_str))
 
     def set_category(self, category: str) -> None:
         self.category = category
 
-    def set_ambigious_toponyms(self) -> None:
-        self.ambigious_toponyms = True
+    def set_ambiguous_toponyms(self) -> None:
+        self.ambiguous_toponyms = True
 
     def set_headings(self, headings: HeadingTracker) -> None:
         self.headings = headings
 
     def unset_reviewed(self) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
 
     def get_yamlfied(self) -> str:
         yaml_str = MIU_HEADER + 'Begin#\n\n'
         for key, val in vars(self).items():
             if val:
                 if key == 'category':
                     yaml_str += key + '    : \'' + val + '\'\n'
-                # elif key == 'settlements' or key == 'provinces':
-                #     yaml_str += f'{key}    : {[toponym.as_dict() for toponym in val]}\n'
-                # elif key.startswith('edges'):
-                #     yaml_str += f'{key}    : {[[edge[0].as_dict(), edge[1].as_dict()] for edge in val]}\n'
                 elif hasattr(val, 'get_yamlfied'):
                     yaml_str += f'{key}    : {val.get_yamlfied()}\n'
                 elif isinstance(val, dict):
                     yaml_str += f'{key}    :\n{dict_to_yaml(val, 1)}\n'
                 else:
                     yaml_str += key + '    : ' + str(val) + '\n'
         yaml_str += '\n' + MIU_HEADER + 'End#\n\n'
 
         return yaml_str
 
     def to_json(self, init) -> Dict:
         json_dict = init
         for key, val in vars(self).items():
-            if key != 'toponyms' and val:
-                # Toponym is only to control the entity and how it was identified
-                # if key == 'settlements' or key == 'provinces':
-                #     json_dict[key] = [elem.to_json() for elem in val]
-                # elif key.startswith('edges'):
-                #     json_dict[key] = [[edge[0].to_json(), edge[1].to_json()] for edge in val]
+            if val:
                 if hasattr(val, 'to_json'):
                     json_dict[key] = val.to_json()
                 else:
                     json_dict[key] = val
         return json_dict
 
     def is_bio(self) -> bool:
@@ -184,16 +178,18 @@
                 self.dates_headings.append(date)
         else:
             self.dates_headings = [date]
 
     def add_tagged_entities(self, entities_dict: dict) -> None:
         for key in YAMLHandler.__attr_from_annotation:
             # Clear old entities
-            if key != 'ambigious_toponyms':
+            if key != 'ambiguous_toponyms':
                 self.__setattr__(key, None)
+            elif hasattr(self, 'ambiguous_toponyms'):
+                self.__delattr__('ambiguous_toponyms')
         for key in YAMLHandler.__attr_from_annotation:
             # Set new entities in same order
             if key in entities_dict.keys():
                 self.__setattr__(key, entities_dict.get(key))
 
     def __setitem__(self, key: str, value: Any) -> None:
         super().__setattr__(key, value)
```

### Comparing `eis1600-0.9.5/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.7/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/miu/methods.py` & `eis1600-0.9.7/eis1600/miu/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from pathlib import Path
 
 from eis1600.dates.methods import date_annotate_miu_text
 from eis1600.helper.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_PATTERN, PAGE_TAG_PATTERN
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
-from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text, insert_nasab_tag, insert_onomastic_tags
+from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text, insert_nasab_tag, insert_onomastic_tags,\
+    aggregate_STFCON_classes, merge_ner_with_person_classes
 from eis1600.onomastics.methods import nasab_annotate_miu
 from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.processing.preprocessing import get_yml_and_miu_df
 from eis1600.toponyms.methods import toponym_category_annotate_miu
 
 
 def disassemble_text(infile: str, out_path: str, verbose: Optional[bool] = None) -> None:
@@ -165,18 +166,20 @@
         return
 
     with open(path, 'r+', encoding='utf-8') as miu_file_object:
         # 1. open miu file and disassemble the file to its parts
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
 
         # 2. annotate NEs and lemmatize
-        df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'] = annotate_miu_text(df)
+        df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'], ST_labels, FCO_labels = annotate_miu_text(df)
 
         # 3. convert cameltools labels format to markdown format
-        df['NER_TAGS'] = camel2md_as_list(df['NER_LABELS'].tolist())
+        aggregated_stfco_labels = aggregate_STFCON_classes(ST_labels, FCO_labels)
+        ner_tags = camel2md_as_list(df['NER_LABELS'].tolist())
+        df['NER_TAGS'] = merge_ner_with_person_classes(ner_tags, aggregated_stfco_labels)
 
         # 4. annotate dates
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], yml_handler)
 
         # 5. insert BNASAB and ENASAB tags with the pretrained transformer model
         df['NASAB_TAGS'] = insert_nasab_tag(df)
```

### Comparing `eis1600-0.9.5/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.7/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/miu/yml_handling.py` & `eis1600-0.9.7/eis1600/miu/yml_handling.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,24 +64,25 @@
         if not is_header:
             text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
 
     return miu_yml_header, text
 
 
 def add_to_entities_dict(
-        entities_dict: Dict, cat: str,
+        entities_dict: Dict,
+        cat: str,
         entity: Union[str, Tuple[str, Union[int, str]], List[Tuple[str, str]], List[str], Tuple[int, str], Dict],
         tag: Optional[str] = None
 ) -> None:
     """Add a tagged entity to the respective list in the entities_dict.
 
     :param Dict entities_dict: Dict containing previous tagged entities.
     :param str cat: Category of the entity.
     :param Union[str|int] entity: Entity - might be int if entity is a date, otherwise str.
-    :param str tag: Onomastic classification, used to differentiate between onomastic elements, optional.
+    :param str tag: Optional, onomastic classification used to differentiate between onomastic elements, defaults to None.
     """
     cat = cat.lower() + 's'
     if tag:
         tag = tag.lower()
     if cat in entities_dict.keys():
         if cat == 'onomastics' and tag:
             if tag in entities_dict[cat].keys():
@@ -103,68 +104,83 @@
 def add_annotated_entities_to_yml(
         text_with_tags: str,
         yml_handler: YAMLHandler,
         file_path: str,
 ) -> None:
     """Populates YAMLHeader with annotated entities.
 
+    Extract annotated entities as metadata. While doing so, identify toponyms and calculate active period for the
+    biographee.
     :param str text_with_tags: Text with inserted tags of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param str file_path: Filename of the current MIU (used in error msg).
     """
     # We do not need to differentiate between automated and manual tags
     text_with_tags = text_with_tags.replace('Ü', '')
     tg = Toponyms.instance()
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     nas_dict = {}
+    nas_counter = 0
     settlements_set: Set[str] = set()
     provinces_set: Set[str] = set()
-    nas_counter = 0
+    ambiguous_toponyms = False
 
     m = ENTITY_TAGS_PATTERN.search(text_with_tags)
     while m:
         tag = m.group('entity')
         length = int(m.group('length'))
+        sub_cat = None
+        if m.group('sub_cat'):
+            # Person, toponyms and books are sub-classified based on their relation to the biographee
+            sub_cat = m.group('sub_cat')
         entity = ' '.join(text_with_tags[m.end():].split(maxsplit=length)[:length])
 
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
         if cat == 'DATE' or cat == 'AGE':
             try:
                 val, e_cat = get_yrs_tag_value(m.group(0))
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {file_path}')
                 return
         elif cat == 'TOPONYM':
-            place, tag, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
-            add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': tag})
+            # Identify toponym
+            place, uris_tag, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
+            if sub_cat:
+                add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uris_tag, 'cat': sub_cat})
+            else:
+                add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uris_tag})
             if len(list_of_uris) == 0:
                 path, uri = split(file_path)
                 uri, ext = splitext(uri)
                 LOGGER_TOPONYMS_UNKNOWN.info(f'{uri},{entity}')
             else:
                 if len(list_of_provinces) > 0:
                     settlements_set.update(list_of_uris)
                     provinces_set.update(list_of_provinces)
                 else:
                     # if there is no province URI that means the toponym is a province and should therefore be added
                     # to provinces and not settlements
                     provinces_set.update(list_of_uris)
                 if len(list_of_uris) > 1:
-                    yml_handler.set_ambigious_toponyms()
+                    # The toponym is ambiguous and matched multiple entries in our gazetteer
+                    ambiguous_toponyms = True
         elif cat == 'ONOMASTIC':
             if tag.startswith('SHR') and entity.startswith('ب'):
                 entity = entity[1:]
                 add_to_entities_dict(entities_dict, cat, entity, tag)
             elif tag.startswith('NAS'):
                 nas_dict['nas_' + str(nas_counter)] = entity
                 nas_counter += 1
             add_to_entities_dict(entities_dict, cat, entity, tag)
             LOGGER_NASAB_KNOWN.info(f'{tag},{entity}')
+        elif cat == 'BOOK':
+            if sub_cat:
+                add_to_entities_dict(entities_dict, cat, {'entity': entity, 'cat': sub_cat}, tag)
         else:
             add_to_entities_dict(entities_dict, cat, entity, tag)
 
         m = ENTITY_TAGS_PATTERN.search(text_with_tags, m.end())
 
     if nas_dict != {}:
         if 'onomastics' in entities_dict.keys():
@@ -172,32 +188,50 @@
         else:
             entities_dict['onomastics'] = {'nas': nas_dict}
 
     if 'onomastics' in entities_dict.keys():
         # Sort dict by keys
         entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
 
+    # Generate edges
     if settlements_set:
         entities_dict['settlements'] = list(settlements_set)
         entities_dict['edges_settlements'] = [[a, b] for a, b in combinations(settlements_set, 2) if a != b]
     if provinces_set:
         entities_dict['provinces'] = list(provinces_set)
         entities_dict['edges_provinces'] = [[a, b] for a, b in combinations(provinces_set, 2) if a != b]
 
+    # Extrapolate active period for the biographee
+    # TODO dates_headings are not analysed yet
     if entities_dict.get('dates'):
         dates = entities_dict.get('dates')
         birth_date = [d.get('date') for d in dates if d.get('cat') == 'B']
         death_date = [d.get('date') for d in dates if d.get('cat') == 'D']
-        alternative_death_date = [d.get('date') for d in dates if d.get('cat') == 'B']
+        alternative_dates = [d.get('date') for d in dates]
+        age_at_death = None
+        if entities_dict.get('ages') and [a.get('age') for a in entities_dict.get('ages') if a.get('cat') == 'D']:
+            age_at_death = max([a.get('age') for a in entities_dict.get('ages') if a.get('cat') == 'D'])
+
         if death_date:
             entities_dict['max_date'] = max(death_date)
-        elif alternative_death_date:
-            entities_dict['max_date'] = max(alternative_death_date)
         elif birth_date:
-            entities_dict['max_date'] = min(birth_date) + 70
+            if age_at_death:
+                entities_dict['max_date'] = min(birth_date) + age_at_death
+            else:
+                # TODO better approximation for active period
+                entities_dict['max_date'] = min(birth_date) + 70
+        elif alternative_dates:
+            entities_dict['max_date'] = max(alternative_dates)
 
         if birth_date:
             entities_dict['min_date'] = min(birth_date)
         elif entities_dict.get('max_date'):
-            entities_dict['min_date'] = entities_dict.get('max_date') - 70
+            if type(age_at_death) == 'int':
+                entities_dict.get('max_date') - age_at_death
+            else:
+                # TODO better approximation for active period
+                entities_dict['min_date'] = entities_dict.get('max_date') - 70
 
+    # Entities, which are not listed in 'YAMLHandler.__attr_from_annotation' are ignored
     yml_handler.add_tagged_entities(entities_dict)
+    if ambiguous_toponyms:
+        yml_handler.set_ambiguous_toponyms()
```

### Comparing `eis1600-0.9.5/eis1600/nlp/cameltools.py` & `eis1600-0.9.7/eis1600/nlp/cameltools.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,31 @@
 class CamelToolsModels:
     __pos_tagger = None
     __mled_disambiguator = None
     __lemmatizer = None
     __ner_tagger = None
     __nasab_tagger = None
     __onomastic_tagger = None
+    __st_tagger = None
+    __fco_tagger = None
+
     __NASAB_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_nasab/"
     __NER_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_ner/"
     __ONOMASTIC_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
+    __STN_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
+    __FCON_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
+
 
     @staticmethod
     def getInstance():
         """ Static access method. """
         if CamelToolsModels.__ner_tagger is None or CamelToolsModels.__lemmatizer is None:
             CamelToolsModels()
-        return CamelToolsModels.__ner_tagger, CamelToolsModels.__lemmatizer, CamelToolsModels.__pos_tagger
+        return CamelToolsModels.__ner_tagger, CamelToolsModels.__lemmatizer, CamelToolsModels.__pos_tagger,\
+            CamelToolsModels.__st_tagger, CamelToolsModels.__fco_tagger
 
     @staticmethod
     def getNasabModel():
         """ Static access method. """
         if CamelToolsModels.__nasab_tagger is None:
             CamelToolsModels.__nasab_tagger = NERecognizer(CamelToolsModels.__NASAB_MODEL_PATH)
         return CamelToolsModels.__nasab_tagger
@@ -43,24 +50,27 @@
         if CamelToolsModels.__ner_tagger is not None:
             raise Exception("This class is a singleton!")
         else:
             CamelToolsModels.__mled_disambiguator = MLEDisambiguator.pretrained()
             CamelToolsModels.__lemmatizer = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'lex')
             CamelToolsModels.__pos_tagger = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'pos')
             CamelToolsModels.__ner_tagger = NERecognizer(CamelToolsModels.__NER_MODEL_PATH) # .pretrained
-
+            CamelToolsModels.__st_tagger = NERecognizer(CamelToolsModels.__STN_MODEL_PATH)
+            CamelToolsModels.__fco_tagger = NERecognizer(CamelToolsModels.__FCON_MODEL_PATH)
 
 def lemmatize_and_tag_ner(tokens: Union[str, list]) -> list:
     """Lemmatize the text and annotate named-entities.
 
         Lemmatize the text and annotated named-entities using Camel Tools models.
         :param tokens: a  string or a list of tokens to be annotated
         """
-    ner_tagger, lemmatizer, pos_tagger = CamelToolsModels.getInstance()
+    ner_tagger, lemmatizer, pos_tagger, st_tager, fco_tagger = CamelToolsModels.getInstance()
     # if tokens is a string, then tokenize it
     if isinstance(tokens, str):
         tokens = simple_word_tokenize(tokens)
     ner_labels = ner_tagger.predict_sentence(tokens)
+    st_labels = st_tager.predict_sentence(tokens)
+    fco_labels = fco_tagger.predict_sentence(tokens)
     lemmas = lemmatizer.tag(tokens)
     pos_tags = pos_tagger.tag(tokens)
     dediac_lemmas = [dediac_ar(lemma) for lemma in lemmas]
-    return list(zip(tokens, ner_labels, lemmas, dediac_lemmas, pos_tags))
+    return list(zip(tokens, ner_labels, lemmas, dediac_lemmas, pos_tags, st_labels, fco_labels))
```

### Comparing `eis1600-0.9.5/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.7/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/nlp/utils.py` & `eis1600-0.9.7/eis1600/nlp/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,98 @@
 from typing import List
 import string
 
 from eis1600.nlp.cameltools import lemmatize_and_tag_ner, CamelToolsModels
 
 
 def annotate_miu_text(df):
-    lemmas, ner_tags, pos_tags = ['_'], ['_'], ['_']
+    lemmas, ner_tags, pos_tags, st_tags, fco_tags = ['_'], ['_'], ['_'], ['_'], ['_']
     section_id, temp_tokens = None, []
     for entry in list(zip(df['SECTIONS'].to_list(), df['TOKENS'].fillna('').to_list()))[1:]:
         _section, _token = entry[0], entry[1]
         if _section is not None:
             # Start a new section
             if len(temp_tokens) > 0:
                 # 1. process the previous section
                 _labels = lemmatize_and_tag_ner(temp_tokens)
-                _, _ner_tags, _lemmas, _dediac_lemmas, _pos_tags = zip(*_labels)
+                _, _ner_tags, _lemmas, _dediac_lemmas, _pos_tags, _st_tags, _fco_tags = zip(*_labels)
                 ner_tags.extend(_ner_tags)
                 lemmas.extend(_dediac_lemmas)
                 pos_tags.extend(_pos_tags)
-
+                fco_tags.extend(_fco_tags)
+                st_tags.extend(_st_tags)
                 # 2. reset variables
                 section_id, temp_tokens = None, []
 
         token = _token if _token not in ['', None] else '_'
         temp_tokens.append(token)
 
     if len(temp_tokens) > 0:
         _labels = lemmatize_and_tag_ner(temp_tokens)
-        _, _ner_tags, _lemmas, _dediac_lemmas, _pos_tags = zip(*_labels)
+        _, _ner_tags, _lemmas, _dediac_lemmas, _pos_tags, _st_tags, _fco_tags = zip(*_labels)
         ner_tags.extend(_ner_tags)
         lemmas.extend(_dediac_lemmas)
         pos_tags.extend(_pos_tags)
-    return ner_tags, lemmas, pos_tags
+        fco_tags.extend(_fco_tags)
+        st_tags.extend(_st_tags)
+
+    return ner_tags, lemmas, pos_tags, st_tags, fco_tags
+
+
+def aggregate_STFCON_classes(st_list: list, fco_list: list) -> List[str]:
+    label_dict = {
+        "B-FAMILY": "F",
+        "I-FAMILY": "F",
+        "B-CONTACT": "C",
+        "I-CONTACT": "C",
+        "B-OPINION": "O",
+        "I-OPINION": "O",
+        "O": "",
+        "_": "",
+        "B-TEACHER": "T",
+        "I-TEACHER": "T",
+        "B-STUDENT": "S",
+        "I-STUDENT": "S",
+        "I-NEUTRAL": "X",
+        "B-NEUTRAL": "X",
+    }
+    aggregated_labels = []
+    for a, b in zip(st_list, fco_list):
+        labels = f"{label_dict.get(a, '')}{label_dict.get(b, '')}"
+        if a == b:
+            labels = label_dict.get(a, '')
+        else:
+            labels = labels.replace("X", "")
+        aggregated_labels.append(labels)
+    return aggregated_labels
 
 
+def merge_ner_with_person_classes(ner_labels, aggregated_stfco_labels):
+    merged_labels = []
+    for a, b in zip(ner_labels, aggregated_stfco_labels):
+        if a[:2] == "ÜP":
+            postfix = "X"
+            if b.strip() != "":
+                postfix = b.strip()
+            a = a + postfix
+        merged_labels.append(a)
+    return merged_labels
+
 def camel2md(labels: list) -> List[str]:
     default_str = ''
 
     converted_tokens, temp_tokens, temp_class = [], [], None
     for _label in labels:
         if _label is None:
             converted_tokens.append(default_str)
         else:
             # Check if the first letter of the label is 'o' or 'B' a Begining of an NE
             if _label[0] in ['O', 'B', '_']:
                 if len(temp_tokens) > 0 and temp_class is not None:
-                    converted_tokens.append(f"{temp_class}{len(temp_tokens)}")  # e.g. ÜP3
+                    converted_tokens.append(f"Ü{temp_class}{len(temp_tokens)}")  # e.g. ÜP3
                     converted_tokens.extend([default_str] * (len(temp_tokens) - 1))
                     # reset temp variables
                     temp_tokens, temp_class = [], None
 
                 if _label in ['O', '_']:
                     converted_tokens.append(default_str)
                 else:
@@ -58,15 +101,15 @@
 
             else:
                 if temp_class is not None:
                     temp_tokens.append(_label)
                 else:
                     converted_tokens.append(default_str)
     if len(temp_tokens) > 0 and temp_class is not None:
-        converted_tokens.append(f"{temp_class}{len(temp_tokens)}")
+        converted_tokens.append(f"Ü{temp_class}{len(temp_tokens)}")
         converted_tokens.extend([default_str] * (len(temp_tokens) - 1))
     return converted_tokens
 
 def camel2md_as_list(labels: list) -> List[str]:
     default_str = ''
     types_mapping = {
         'LOC': 'ÜT',
@@ -105,48 +148,39 @@
 def insert_nasab_tag(df) -> list:
     tokens = df['TOKENS'].fillna('').to_list()
     nasab_tagger = CamelToolsModels.getNasabModel()
     shortend_list_of_tokens = tokens[1:]
     __shortend_list_limit = 120
     if len(tokens) > __shortend_list_limit:
         shortend_list_of_tokens = tokens[1:__shortend_list_limit]
-        # print(tokens[:__shortend_list_limit], tokens)
-        # for token in tokens[1:__shortend_list_limit]:
-        #     if token is not None:
-        #         shortend_list_of_tokens.append(token)
-        #     else:
-        #         shortend_list_of_tokens.append("_")
+    for idx, t in enumerate(shortend_list_of_tokens):
+        if t.strip() == "":
+            shortend_list_of_tokens[idx] = "-"
     nasab_labels = nasab_tagger.predict_sentence(shortend_list_of_tokens)
     punct = "..،_" + string.punctuation
     nasab = ['_']
     nasab_started = False
     for token, label in zip(shortend_list_of_tokens, nasab_labels):
         if label == "B-NASAB":
             # Start a new NASAB
             nasab.append("BNASAB")
             nasab_started = True
+        elif label == "I-NASAB":
+            nasab.append('')
         else:
-            if label == "I-NASAB":
-                nasab.append('')
+            if nasab_started:
+                nasab.append("ENASAB")
+                nasab_started = False
             else:
-                if nasab_started:
-                    if token.strip() in punct:
-                        nasab[-1] = "ENASAB"
-                        nasab.append("")
-                    else:
-                        nasab.append("ENASAB")
-                    nasab_started = False
-                else:
-                    nasab.append('')
+                nasab.append('')
     if nasab_started:
         nasab[-1] = "ENASAB"
     # merge the shortend list
     if len(tokens) > __shortend_list_limit:
         nasab.extend([''] * (len(tokens) - __shortend_list_limit))
-
     return nasab
 
 
 def insert_onomastic_tags(df):
     onomastic_tagger = CamelToolsModels.getOnomasticModel()
     onomastic_tags = [None] * len(df['TOKENS'])
     start_nasab_id, end_nasab_id = -1, -1
@@ -164,9 +198,8 @@
         onomastic_labels = onomastic_tagger.predict_sentence(nasab_tokens)
         ono_tags = camel2md(onomastic_labels)
 
         for i, tag in enumerate(ono_tags):
             onomastic_tags[start_nasab_id + i] = tag
 
     df['ONONMASTIC_TAGS'] = onomastic_tags
-
     return df['ONONMASTIC_TAGS']
```

### Comparing `eis1600-0.9.5/eis1600/onomastics/annotation.py` & `eis1600-0.9.7/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/onomastics/methods.py` & `eis1600-0.9.7/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.7/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/processing/postprocessing.py` & `eis1600-0.9.7/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/processing/preprocessing.py` & `eis1600-0.9.7/eis1600/processing/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from eis1600.miu.YAMLHandler import YAMLHandler
 
 from eis1600.miu.yml_handling import extract_yml_header_and_text
-from typing import Iterator, List, TextIO, Tuple, Union
+from typing import Iterator, List, Optional, TextIO, Tuple, Union
 
 from pandas import DataFrame, options
 
 from camel_tools.tokenizers.word import simple_word_tokenize
 from eis1600.helper.markdown_patterns import MIU_TAG_PATTERN, SECTION_PATTERN, SECTION_SPLITTER_PATTERN, TAG_PATTERN
 
 
@@ -28,20 +28,24 @@
             ar_tokens.append(t)
             tags.append(tag)
             tag = None
 
     return ar_tokens, tags
 
 
-def tokenize_miu_text(text: str) -> Iterator[Tuple[Union[str, None], Union[str, None], List[Union[str, None]]]]:
+def tokenize_miu_text(
+        text: str,
+        keep_automatic_tags: Optional[bool] = False
+) -> Iterator[Tuple[Union[str, None], Union[str, None], List[Union[str, None]]]]:
     """Returns the MIU text as zip object of three sparse columns: sections, tokens, lists of tags.
 
     Takes an MIU text and returns a zip object of three sparse columns: sections, tokens, lists of tags. Elements can
     be None because of sparsity.
-    :param text: MIU text content to process.
+    :param str text: MIU text content to process.
+    :param bool keep_automatic_tags: Optional, if True keep automatic annotation (Ü-tags), defaults to False.
     :return Iterator: Returns a zip object containing three sparse columns: sections, tokens, lists of tags. Elements
     can be None because of sparsity.
     """
     text_and_heading = MIU_TAG_PATTERN.split(text)
     # The indices are connected to the number of capturing group in MIU_TAG_PATTERN
     heading = text_and_heading[1]
     text_iter = SECTION_SPLITTER_PATTERN.split(text_and_heading[4][:-2]).__iter__()
@@ -60,15 +64,15 @@
             text_wo_new_lines = paragraph.replace('\n_ء_', ' NEWLINE ')
             text_wo_new_lines = text_wo_new_lines.replace('\n', ' NEWLINE ')
             text_wo_new_lines = text_wo_new_lines.replace('%~%', 'HEMISTICH')
             tokens = simple_word_tokenize(text_wo_new_lines)
             tag = None
             for t in tokens:
                 if TAG_PATTERN.match(t):
-                    if not t.startswith('Ü'):
+                    if not t.startswith('Ü') or keep_automatic_tags:
                         # Do not add automated tags to the list - they come from the csv anyway
                         # There might be multiple tags in front of a token - Page, NEWLINE, NER tag, ...
                         if tag:
                             tag.append(t)
                         else:
                             tag = [t]
                 else:
@@ -84,24 +88,28 @@
                 tags.append(tag)
 
         paragraph = next(text_iter, None)
 
     return zip(sections, ar_tokens, tags)
 
 
-def get_yml_and_miu_df(miu_file_object: TextIO) -> Tuple[YAMLHandler, DataFrame]:
+def get_yml_and_miu_df(
+        miu_file_object: TextIO,
+        keep_automatic_tags: Optional[bool] = False
+) -> Tuple[YAMLHandler, DataFrame]:
     """Returns YAMLHandler instance and MIU as a DataFrame containing the columns 'SECTIONS', 'TOKENS', 'TAGS_LISTS'.
 
     :param TextIO miu_file_object: File object of the MIU file.
+    :param bool keep_automatic_tags: Optional, if True keep automatic annotation (Ü-tags), defaults to False.
     :return Tuple[YAMLHandler, DataFrame]: YAMLHandler and DataFrame containing the columns 'SECTIONS', 'TOKENS',
     'TAGS_LISTS'.
     """
     yml_str, text = extract_yml_header_and_text(miu_file_object, False)
     yml_handler = YAMLHandler().from_yml_str(yml_str)
-    zipped = tokenize_miu_text(text)
+    zipped = tokenize_miu_text(text, keep_automatic_tags)
     df = DataFrame(zipped, columns=['SECTIONS', 'TOKENS', 'TAGS_LISTS'])
 
     df.mask(df == '', inplace=True)
 
     return yml_handler, df
```

### Comparing `eis1600-0.9.5/eis1600/stats/methods.py` & `eis1600-0.9.7/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/stats/miu_stats.py` & `eis1600-0.9.7/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.5/eis1600/toponyms/annotation.py` & `eis1600-0.9.7/eis1600/toponyms/annotation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,66 @@
-# Annotate hajja -> Mekka
-# Annotate jāwara -> Medina
-# Tag category of toponyms
 from glob import glob
 from pathlib import Path
 
 from sys import argv
-from argparse import ArgumentParser, RawDescriptionHelpFormatter
+from os.path import isfile, splitext
+from argparse import Action, ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 
 from p_tqdm import p_uimap
 
 from eis1600.helper.repo import TRAINING_DATA_REPO
 from eis1600.toponyms.methods import toponym_category_annotation
 
 
+class CheckFileEndingAction(Action):
+    def __call__(self, parser, namespace, input_arg, option_string=None):
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
+            if fileext != '.EIS1600':
+                parser.error('Input must be a single MIU file')
+            else:
+                setattr(namespace, self.dest, input_arg)
+        else:
+            setattr(namespace, self.dest, None)
+
+
 def main():
     arg_parser = ArgumentParser(
             prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
+    arg_parser.add_argument('-K', '--keep', action='store_true', help='Keep automatic tags (Ü-tags)')
     arg_parser.add_argument('-T', '--test', action='store_true')
+    arg_parser.add_argument(
+            'input', type=str, nargs='?',
+            help='IDs or MIU file to process',
+            action=CheckFileEndingAction
+    )
 
     args = arg_parser.parse_args()
     debug = args.debug
     test = args.test
+    keep = args.keep
 
-    if test:
-        with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
-            files_txt = fh.read().splitlines()
-
-        infiles = [TRAINING_DATA_REPO + 'gold_standard_nasab/' + file for file in files_txt if Path(
-                TRAINING_DATA_REPO + 'gold_standard_nasab/' + file).exists()]
-    else:
-        infiles = glob(TRAINING_DATA_REPO + 'training_data_nasab_ML2/*.EIS1600')
-
-    if debug:
-        for file in infiles[:20]:
-            print(file)
-            toponym_category_annotation(file, test)
+    if args.input:
+        toponym_category_annotation(args.input, test, keep)
     else:
-        res = []
-        res += p_uimap(partial(toponym_category_annotation, test=test), infiles)
+        if test:
+            with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
+                files_txt = fh.read().splitlines()
+
+            infiles = [TRAINING_DATA_REPO + 'gold_standard_nasab/' + file for file in files_txt if Path(
+                    TRAINING_DATA_REPO + 'gold_standard_nasab/' + file).exists()]
+        else:
+            infiles = glob(TRAINING_DATA_REPO + 'training_data_nasab_ML2/*.EIS1600')
+
+        if debug:
+            for file in infiles[:20]:
+                print(file)
+                toponym_category_annotation(file, test, keep)
+        else:
+            res = []
+            res += p_uimap(partial(toponym_category_annotation, test=test, keep_automatic_tags=keep), infiles)
 
     print('Done')
```

### Comparing `eis1600-0.9.5/eis1600/toponyms/methods.py` & `eis1600-0.9.7/eis1600/toponyms/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def add_category_to_tag(
         tag_or_tag_list: Union[str, List[str]],
         category: Literal['B', 'D', 'K', 'M', 'O', 'P', 'R', 'X'],
 ) -> Union[str, List[str]]:
     if isinstance(tag_or_tag_list, list):
-        return [t if not t.startswith('T') else t + category for t in tag_or_tag_list]
+        return [t if not t.startswith('T') else 'Ü' + t + category for t in tag_or_tag_list]
     else:
         return tag_or_tag_list + category
 
 
 def toponym_category_annotate_miu(s_tokens: Series, s_tags: Series) -> Series:
     """Categorize toponyms based on their context and add category to their tag.
 
@@ -48,22 +48,23 @@
 
         # Update tag
         s_new_tags.loc[idx] = add_category_to_tag(s_tags.loc[idx], category=toponym_category)
 
     return s_new_tags
 
 
-def toponym_category_annotation(file: str, test: Optional[bool] = False):
+def toponym_category_annotation(file: str, test: Optional[bool] = False, keep_automatic_tags: Optional[bool] = False):
     """Helper to run toponyms category annotation standalone as cmdline script.
 
     :param str file: Path of the miu file to annotate.
-    :param bool test: Indicating if the script is run with test data, defaults to false.
+    :param bool test: Optional, indicating if the script is run with test data, defaults to false.
+    :param bool keep_automatic_tags: Optional, if True keep automatic annotation (Ü-tags), defaults to False.
     """
     with open(file, 'r', encoding='utf-8') as miu_file_object:
-        yml_handler, df = get_yml_and_miu_df(miu_file_object)
+        yml_handler, df = get_yml_and_miu_df(miu_file_object, keep_automatic_tags)
 
     df['TAGS_LISTS'] = toponym_category_annotate_miu(df['TOKENS'], df['TAGS_LISTS'])
 
     if test:
         output_path = str(file).replace('gold_standard_nasab', 'gold_standard_topo')
     else:
         output_path = str(file)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eis1600-0.9.5/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.7/eis1600.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.5
+Version: 0.9.7
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -245,7 +245,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7, <3.9
 Description-Content-Type: text/markdown
 Provides-Extra: NER
+Provides-Extra: EVAL
```

### Comparing `eis1600-0.9.5/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.7/eis1600.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,35 @@
 eis1600/gazetteers/Toponyms.py
 eis1600/gazetteers/__init__.py
 eis1600/gazetteers/data/__init__.py
 eis1600/gazetteers/data/onomastic_gazetteer.csv
 eis1600/gazetteers/data/spelling_gazetteer.csv
 eis1600/gazetteers/data/toponyms_gazetteer.csv
 eis1600/helper/EntityTags.py
+eis1600/helper/EvalResultsEncoder.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
+eis1600/helper/eval_date_model.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
-eis1600/helper/md_tags_to_bio.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/repo.py
+eis1600/helper/top_tags_to_bio.py
 eis1600/helper/yml_methods.py
 eis1600/helper/yml_to_json.py
 eis1600/helper/data/__init__.py
 eis1600/helper/data/entity_tags.csv
 eis1600/markdown/UIDs.py
 eis1600/markdown/__init__.py
 eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
 eis1600/markdown/insert_uids.py
+eis1600/markdown/md_to_bio.py
 eis1600/markdown/methods.py
 eis1600/markdown/update_uids.py
 eis1600/markdown/update_uids_old_process.py
 eis1600/miu/HeadingTracker.py
 eis1600/miu/YAMLHandler.py
 eis1600/miu/__init__.py
 eis1600/miu/disassemble_into_miu_files.py
```

### Comparing `eis1600-0.9.5/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.7/eis1600.egg-info/entry_points.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [console_scripts]
 annotate_mius = eis1600.nlp.ner_annotate_mius:main [ner]
 convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main
 disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main
+eval_date_model = eis1600.helper.eval_date_model:main [eval]
 fix_miu_annotation = eis1600.helper.fix_miu_annotation:main
 insert_uids = eis1600.markdown.insert_uids:main
-md_tags_to_bio = eis1600.helper.md_tags_to_bio:main
 miu_random_revisions = eis1600.helper.miu_random_revisions:main
 miu_stats = eis1600.stats.miu_stats:main
 onomastic_annotation = eis1600.onomastics.annotation:main
 reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main
+top_tags_to_bio = eis1600.helper.top_tags_to_bio:main
 toponym_annotation = eis1600.toponyms.annotation:main
 update_uids = eis1600.markdown.update_uids:main
 xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main
 yml_to_json = eis1600.helper.yml_to_json:main
```

### Comparing `eis1600-0.9.5/setup.py` & `eis1600-0.9.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.5',
+      version='0.9.7',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
       packages=find_packages(include=['eis1600', 'eis1600.*'], exclude=['excluded']),
       package_data={'eis1600.gazetteers.data': ['*.csv'], 'eis1600.helper.data': ['*.csv']},
       entry_points={
           'console_scripts': [
                   'annotate_mius = eis1600.nlp.ner_annotate_mius:main [NER]',
                   'convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main',
                   'disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main',
+                  'eval_date_model = eis1600.helper.eval_date_model:main [EVAL]',
                   'fix_miu_annotation = eis1600.helper.fix_miu_annotation:main',
                   'insert_uids = eis1600.markdown.insert_uids:main',
-                  'md_tags_to_bio = eis1600.helper.md_tags_to_bio:main',
+                  'top_tags_to_bio = eis1600.helper.top_tags_to_bio:main',
                   'miu_random_revisions = eis1600.helper.miu_random_revisions:main',
                   'miu_stats = eis1600.stats.miu_stats:main',
                   'onomastic_annotation = eis1600.onomastics.annotation:main',
                   'toponym_annotation = eis1600.toponyms.annotation:main',
                   'reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main',
                   'update_uids = eis1600.markdown.update_uids:main',
                   'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main',
@@ -38,14 +39,14 @@
               'pandas',
               'numpy',
               'tqdm',
               'p_tqdm',
               'importlib_resources',
               'jsonpickle'
       ],
-      extras_require={'NER': ['camel-tools']},
+      extras_require={'NER': ['camel-tools'], 'EVAL': ['evaluate', 'seqeval']},
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent',
                    'Development Status :: 1 - Planning',
                    'Intended Audience :: Science/Research']
       )
```

