# Comparing `tmp/SquirroClient-3.7.1.tar.gz` & `tmp/SquirroClient-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SquirroClient-3.7.1.tar", last modified: Mon Jan 23 22:44:59 2023, max compression
+gzip compressed data, was "SquirroClient-3.8.2.tar", last modified: Wed Jul 12 18:44:23 2023, max compression
```

## Comparing `SquirroClient-3.7.1.tar` & `SquirroClient-3.8.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 22:44:59.043904 SquirroClient-3.7.1/
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-23 22:44:59.043904 SquirroClient-3.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 22:44:59.028904 SquirroClient-3.7.1/SquirroClient.egg-info/
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/SquirroClient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1889 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/SquirroClient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/SquirroClient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/SquirroClient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/SquirroClient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-23 22:44:59.043904 SquirroClient-3.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1144 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 22:44:59.031904 SquirroClient-3.7.1/squirro_client/
--rw-r--r--   0 root         (0) root         (0)      336 2023-01-23 22:44:58.000000 SquirroClient-3.7.1/squirro_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17137 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/base.py
--rw-r--r--   0 root         (0) root         (0)    11589 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/document_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2049 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/internal.py
--rw-r--r--   0 root         (0) root         (0)    26763 2022-09-28 18:40:03.000000 SquirroClient-3.7.1/squirro_client/item_uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 22:44:59.043904 SquirroClient-3.7.1/squirro_client/topic/
--rw-r--r--   0 root         (0) root         (0)    71049 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/topic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11655 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/topic/communities.py
--rw-r--r--   0 root         (0) root         (0)     4488 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/topic/community_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8573 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/community_types.py
--rw-r--r--   0 root         (0) root         (0)    14510 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/contributingrecords.py
--rw-r--r--   0 root         (0) root         (0)    27838 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/topic/dashboards.py
--rw-r--r--   0 root         (0) root         (0)     2306 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/email_templates.py
--rw-r--r--   0 root         (0) root         (0)     6644 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/enrichments.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/entities.py
--rw-r--r--   0 root         (0) root         (0)     8146 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/facets.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/globaltemp.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/guidefiles.py
--rw-r--r--   0 root         (0) root         (0)    17842 2022-10-17 05:12:00.000000 SquirroClient-3.7.1/squirro_client/topic/machinelearning.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/ml_candidate_set.py
--rw-r--r--   0 root         (0) root         (0)    15257 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/ml_groundtruth.py
--rw-r--r--   0 root         (0) root         (0)     7079 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/ml_model.py
--rw-r--r--   0 root         (0) root         (0)     7259 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/ml_publish.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/ml_sentence_splitter.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/ml_template.py
--rw-r--r--   0 root         (0) root         (0)     6529 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/ml_user_feedback.py
--rw-r--r--   0 root         (0) root         (0)    10022 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/objects.py
--rw-r--r--   0 root         (0) root         (0)      850 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/pipeline_sections.py
--rw-r--r--   0 root         (0) root         (0)     2556 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/pipeline_status.py
--rw-r--r--   0 root         (0) root         (0)    14290 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/pipeline_workflows.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/project_translations.py
--rw-r--r--   0 root         (0) root         (0)    37653 2022-11-28 13:55:15.000000 SquirroClient-3.7.1/squirro_client/topic/projects.py
--rw-r--r--   0 root         (0) root         (0)     9185 2022-11-11 12:30:00.000000 SquirroClient-3.7.1/squirro_client/topic/savedsearches.py
--rw-r--r--   0 root         (0) root         (0)      886 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/smart_answers.py
--rw-r--r--   0 root         (0) root         (0)    16304 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/smartfilters.py
--rw-r--r--   0 root         (0) root         (0)    29496 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/sources.py
--rw-r--r--   0 root         (0) root         (0)     9472 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/topic/suggest_images.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/synonyms.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/themes.py
--rw-r--r--   0 root         (0) root         (0)    20886 2023-01-11 18:47:07.000000 SquirroClient-3.7.1/squirro_client/topic/trenddetection.py
--rw-r--r--   0 root         (0) root         (0)    11086 2022-10-17 05:12:00.000000 SquirroClient-3.7.1/squirro_client/topic/widgets_assets.py
--rw-r--r--   0 root         (0) root         (0)    27333 2022-09-02 15:29:04.000000 SquirroClient-3.7.1/squirro_client/user.py
--rw-r--r--   0 root         (0) root         (0)     1448 2022-09-28 18:40:03.000000 SquirroClient-3.7.1/squirro_client/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 18:44:23.677322 SquirroClient-3.8.2/
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-12 18:44:23.676322 SquirroClient-3.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 18:44:23.668321 SquirroClient-3.8.2/SquirroClient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/SquirroClient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/SquirroClient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/SquirroClient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/SquirroClient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/SquirroClient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 18:44:23.677322 SquirroClient-3.8.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 18:44:23.670322 SquirroClient-3.8.2/squirro_client/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-12 18:44:23.000000 SquirroClient-3.8.2/squirro_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17134 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/base.py
+-rw-r--r--   0 root         (0) root         (0)    11588 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/document_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2022-11-11 15:50:29.000000 SquirroClient-3.8.2/squirro_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/internal.py
+-rw-r--r--   0 root         (0) root         (0)    26763 2022-09-28 19:42:06.000000 SquirroClient-3.8.2/squirro_client/item_uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 18:44:23.676322 SquirroClient-3.8.2/squirro_client/topic/
+-rw-r--r--   0 root         (0) root         (0)    71735 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12149 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/communities.py
+-rw-r--r--   0 root         (0) root         (0)     4696 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/community_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8837 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/community_types.py
+-rw-r--r--   0 root         (0) root         (0)    15030 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/contributingrecords.py
+-rw-r--r--   0 root         (0) root         (0)    27838 2022-11-11 15:50:29.000000 SquirroClient-3.8.2/squirro_client/topic/dashboards.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/squirro_client/topic/email_templates.py
+-rw-r--r--   0 root         (0) root         (0)     6644 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/enrichments.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/entities.py
+-rw-r--r--   0 root         (0) root         (0)     8146 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/facets.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/globaltemp.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/guidefiles.py
+-rw-r--r--   0 root         (0) root         (0)    17842 2022-10-17 06:40:19.000000 SquirroClient-3.8.2/squirro_client/topic/machinelearning.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_candidate_set.py
+-rw-r--r--   0 root         (0) root         (0)    15956 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_groundtruth.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_model.py
+-rw-r--r--   0 root         (0) root         (0)     7258 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_publish.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_sentence_splitter.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_template.py
+-rw-r--r--   0 root         (0) root         (0)     6528 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/ml_user_feedback.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/notes.py
+-rw-r--r--   0 root         (0) root         (0)    10022 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/objects.py
+-rw-r--r--   0 root         (0) root         (0)      850 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/pipeline_sections.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/squirro_client/topic/pipeline_status.py
+-rw-r--r--   0 root         (0) root         (0)    15743 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/pipeline_workflows.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/project_translations.py
+-rw-r--r--   0 root         (0) root         (0)    37651 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/projects.py
+-rw-r--r--   0 root         (0) root         (0)     9185 2022-11-11 15:50:29.000000 SquirroClient-3.8.2/squirro_client/topic/savedsearches.py
+-rw-r--r--   0 root         (0) root         (0)      886 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/squirro_client/topic/smart_answers.py
+-rw-r--r--   0 root         (0) root         (0)    16304 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/smartfilters.py
+-rw-r--r--   0 root         (0) root         (0)    29495 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/sources.py
+-rw-r--r--   0 root         (0) root         (0)     9472 2023-01-11 22:15:35.000000 SquirroClient-3.8.2/squirro_client/topic/subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2022-09-02 17:52:25.000000 SquirroClient-3.8.2/squirro_client/topic/suggest_images.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/synonyms.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2023-01-23 22:44:30.000000 SquirroClient-3.8.2/squirro_client/topic/themes.py
+-rw-r--r--   0 root         (0) root         (0)    20885 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/trenddetection.py
+-rw-r--r--   0 root         (0) root         (0)    11085 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/topic/widgets_assets.py
+-rw-r--r--   0 root         (0) root         (0)    28210 2023-07-12 18:41:04.000000 SquirroClient-3.8.2/squirro_client/user.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2022-09-28 19:42:06.000000 SquirroClient-3.8.2/squirro_client/util.py
```

### Comparing `SquirroClient-3.7.1/PKG-INFO` & `SquirroClient-3.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SquirroClient
-Version: 3.7.1
+Version: 3.8.2
 Summary: Python client for the Squirro API
 Home-page: http://dev.squirro.com/docs/tools/python/index.html
 Author: Squirro Team
 Author-email: support@squirro.com
 License: Commercial
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SquirroClient-3.7.1/SquirroClient.egg-info/PKG-INFO` & `SquirroClient-3.8.2/SquirroClient.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SquirroClient
-Version: 3.7.1
+Version: 3.8.2
 Summary: Python client for the Squirro API
 Home-page: http://dev.squirro.com/docs/tools/python/index.html
 Author: Squirro Team
 Author-email: support@squirro.com
 License: Commercial
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SquirroClient-3.7.1/SquirroClient.egg-info/SOURCES.txt` & `SquirroClient-3.8.2/SquirroClient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 squirro_client/topic/ml_candidate_set.py
 squirro_client/topic/ml_groundtruth.py
 squirro_client/topic/ml_model.py
 squirro_client/topic/ml_publish.py
 squirro_client/topic/ml_sentence_splitter.py
 squirro_client/topic/ml_template.py
 squirro_client/topic/ml_user_feedback.py
+squirro_client/topic/notes.py
 squirro_client/topic/objects.py
 squirro_client/topic/pipeline_sections.py
 squirro_client/topic/pipeline_status.py
 squirro_client/topic/pipeline_workflows.py
 squirro_client/topic/project_translations.py
 squirro_client/topic/projects.py
 squirro_client/topic/savedsearches.py
```

### Comparing `SquirroClient-3.7.1/setup.py` & `SquirroClient-3.8.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import find_packages, setup
 
 install_requires = open("requirements.txt").read().splitlines()
 
 setup(
     name="SquirroClient",
     # Version number also needs to be updated in squirro_client/__init__.py
-    version="3.7.1",
+    version="3.8.2",
     description="Python client for the Squirro API",
     long_description=open("README").read(),
     author="Squirro Team",
     author_email="support@squirro.com",
     url="http://dev.squirro.com/docs/tools/python/index.html",
     packages=find_packages(),
     install_requires=install_requires,
```

### Comparing `SquirroClient-3.7.1/squirro_client/base.py` & `SquirroClient-3.8.2/squirro_client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         ...                        cluster='http://squirro.example.com')
         >>> client = SquirroClient(None, None,
         ...                        cluster='http://squirro.example.com',
         ...                        retry_total=10)
     """
 
     def __init__(self, client_id, client_secret, **kwargs):
-
         # assign authentication class state
         self.client_id = client_id
         self.client_secret = client_secret
         self.tenant = kwargs.get("tenant", None)
 
         self._access_token = None
         self._refresh_token = None
@@ -123,15 +122,14 @@
             self.topic_api_url = topic_api_url.rstrip("/")
 
         # retry default options, use values provided by the caller to update
         # the default retry options
         self.retry = copy.deepcopy(RETRY)
         for k, v in kwargs.items():
             if k.startswith("retry_"):
-
                 # `method_whitelist` has been deprecated
                 if k == "retry_method_whitelist":
                     k = "retry_allowed_methods"
 
                 self.retry[k.replace("retry_", "")] = v
 
         # default timeout
@@ -366,15 +364,14 @@
             except self._requests.exceptions.RetryError as ex:
                 raise RetryError(None, ex.args[0])
             except self._requests.exceptions.ConnectionError as ex:
                 raise ConnectionError(None, ex) from ex
 
             # check for failed authorization
             if retry_count == 0 and res.status_code == 401:
-
                 # try to refresh the tokens, if that fails we return the
                 # previous response
                 successful = self._refresh_tokens()
                 if not successful:
                     break
 
                 log.debug("retrying request %r %r", method, url)
```

### Comparing `SquirroClient-3.7.1/squirro_client/document_uploader.py` & `SquirroClient-3.8.2/squirro_client/document_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         metadata_mapping=None,
         batch_size=10,
         batch_size_mb=150,
         default_mime_type_keyword=True,
         timeout_secs=TIMEOUT_SECS,
         **kwargs
     ):
-
         # assemble steps_config configuration
         source_id = kwargs.pop("source_id", None)
         pipeline_workflow_id = kwargs.pop("pipeline_workflow_id", None)
         pipeline_workflow_name = kwargs.pop("pipeline_workflow_name", None)
         steps_config = kwargs.pop("steps_config", None)
 
         # deprecation warning for an explicit processing config
```

### Comparing `SquirroClient-3.7.1/squirro_client/exceptions.py` & `SquirroClient-3.8.2/squirro_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/internal.py` & `SquirroClient-3.8.2/squirro_client/internal.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/item_uploader.py` & `SquirroClient-3.8.2/squirro_client/item_uploader.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/__init__.py` & `SquirroClient-3.8.2/squirro_client/topic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .ml_candidate_set import MLCandidateSetMixin
 from .ml_groundtruth import MLGroundTruthMixin
 from .ml_model import MLModelsMixin
 from .ml_publish import MLPublishMixin
 from .ml_sentence_splitter import MLSentenceSplitterMixin
 from .ml_template import MLTemplatesMixin
 from .ml_user_feedback import MLUserFeedbackMixin
+from .notes import NotesMixin
 from .objects import ObjectsMixin
 from .pipeline_sections import PipelineSectionsMixin
 from .pipeline_status import PipelineStatusMixin
 from .pipeline_workflows import PipelineWorkflowMixin
 from .project_translations import ProjectTranslationsMixin
 from .projects import ProjectsMixin
 from .savedsearches import SavedSearchesMixin
@@ -322,14 +323,15 @@
 
         :param project_id: Project identifier.
         :param query: Optional query to run.
         :param query_context: Dictionary with more context of the user's input / intent:
 
                 - `searchbar_query` : Terms that user typed in a searchbar.
                 - `dashboard_filters` : Additional filter-queries provided via dashboard or widget configuration.
+                - `community_query` : Selected community in the Community 360 dashboard.
                 - `like` : Additional input to perform approximate search on.
                          For now `like` is considered to be a long string (e.g. paragraphs)
                 - `parsed` : The parsed, analysed and enriched representation of the `searchbar_query` (response of the configured `query-processing workflow <https://go.squirro.com/libnlp-query-processing>`_)
 
         :param start: Zero based starting point.
         :param count: Maximum number of items to return.
         :param child_count: Maximum number of entities to return with items.
@@ -1281,21 +1283,18 @@
             ...                         count=500, scroll='1m', preserve_scroll_order=True):
                     # process matched item
         """
         assert scroll, "`scroll` cannot be empty for scan."
         if options:
             assert "fold_near_duplicate" not in options
 
-        url = "%(ep)s/%(version)s/%(tenant)s" "/projects/%(project_id)s/items/query"
-        url = url % {
-            "ep": self.topic_api_url,
-            "version": self.version,
-            "tenant": self.tenant,
-            "project_id": project_id,
-        }
+        url = (
+            f"{self.topic_api_url}/{self.version}/{self.tenant}/"
+            f"projects/{project_id}/items/query"
+        )
 
         if preserve_order:
             logging.warning(
                 "The `preserve_order` parameter is deprecated. "
                 "Use the `preserve_scroll_order` instead."
             )
             preserve_scroll_order = preserve_order
@@ -1313,26 +1312,41 @@
             "options": options,
             "created_before": created_before,
             "created_after": created_after,
         }
         data = {k: v for k, v in args.items() if v is not None}
 
         items = True
-        while items:
-            res = self._process_response(
-                self._perform_request(
-                    "post", url, data=json.dumps(data), headers=headers
+        res = None
+        try:
+            while items:
+                res = self._process_response(
+                    self._perform_request(
+                        "post", url, data=json.dumps(data), headers=headers
+                    )
                 )
-            )
-            items = res.get("items", [])
-            yield from items
-            if not res.get("eof"):
-                data["next_params"] = res.get("next_params")
-            else:
-                break
+                items = res.get("items", [])
+                yield from items
+                if not res.get("eof"):
+                    data["next_params"] = res.get("next_params")
+                else:
+                    break
+        except GeneratorExit:
+            logging.warning("Scanning of items was interrupted")
+        except Exception as ex:
+            logging.exception(f"Could not process the response: {ex}")
+            raise
+        finally:
+            if res is not None:
+                scroll_id = res.get("next_params").get("scroll_id")
+                url = (
+                    f"{self.topic_api_url}/{self.version}/{self.tenant}/"
+                    f"projects/{project_id}/scan_artifacts/scroll_context/{scroll_id}"
+                )
+                res = self._perform_request("delete", url)
 
     def get_items(self, project_id, **kwargs):
         """Returns items for the provided project.
 
         DEPRECATED. The `query` method is more powerful.
 
         :param project_id: Project identifier.
@@ -1864,9 +1878,10 @@
     MLGroundTruthMixin,
     MLTemplatesMixin,
     MLModelsMixin,
     MLPublishMixin,
     MLUserFeedbackMixin,
     MLSentenceSplitterMixin,
     SmartAnswersMixin,
+    NotesMixin,
 ):
     pass
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/communities.py` & `SquirroClient-3.8.2/squirro_client/topic/communities.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,30 @@
                 "community_type_id": community_type_id,
                 "community_id": community_id,
                 "query": query or "",
             }
         res = self._perform_request("get", url)
         return self._process_response(res)
 
+    def get_project_communities(self, project_id):
+        """Return all communities for the given `project_id`.
+
+        :param project_id: Project identifier
+
+        :returns: A list of communities.
+
+        """
+        url = "{ep}/v0/{tenant}/projects/{project_id}/communities".format(
+            ep=self.topic_api_url,
+            tenant=self.tenant,
+            project_id=project_id,
+        )
+        res = self._perform_request("get", url)
+        return self._process_response(res)
+
     def create_community(self, project_id, community_type_id, name, photo, facet_value):
         """Create a new community.
 
         :param project_id: Project identifier
         :param community_type_id: Community type identifier
         :param name: Name of the community
         :param photo: Address to the photo of the community
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/community_subscription.py` & `SquirroClient-3.8.2/squirro_client/topic/community_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,24 @@
 
     def new_community_subscriptions(
         self,
         project_id,
         community_ids,
         remove_existing_subscriptions=False,
         user_id=None,
+        include_count_of_items=False,
     ):
         """Creates a new community subscription for a project
         given the community_id
 
         :param project_id: Project Identifier
         :param community_ids: Ids of the communities to subscribe to
         :param remove_existing_subscriptions: Boolean flag to remove existing subscriptions
         :param user_id: Id of the user subscribing to the community ids
+        :param include_count_of_items: Boolean flag to add total count of items for a community subscription
 
         Example::
 
             >>> client.new_community_subscription(
                     'Xh9CeyQtTYe2cv5F11e6nQ',
                     ['mNDkc6q9QvuL8EVMWA3cgg','otCTwaF9Qs-66MFGLCtyKQ']
                     remove_existing_subscriptions = True
@@ -91,22 +93,22 @@
         url = (
             "%(ep)s/v0/%(tenant)s/projects/%(project_id)s/community_subscriptions"
         ) % {"ep": self.topic_api_url, "tenant": self.tenant, "project_id": project_id}
         data = {
             "community_ids": community_ids,
             "remove_existing_subscriptions": remove_existing_subscriptions,
             "user_id": user_id,
+            "include_count_of_items": include_count_of_items,
         }
 
         headers = {"Content-Type": "application/json"}
         res = self._perform_request("post", url, data=json.dumps(data), headers=headers)
         return self._process_response(res, [201])
 
     def delete_community_subscription(self, project_id, subscription_id):
-
         """Deletes a community subscription
 
         :param project_id: Project Identifier
         :param subscription_id: Community subscription Identifier
 
         Example::
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/community_types.py` & `SquirroClient-3.8.2/squirro_client/topic/community_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,53 +100,57 @@
             "count": count,
             "community_partial_name": community_partial_name,
             "include_count_of_items": include_count_of_items,
         }
         res = self._perform_request("get", url, params=params)
         return self._process_response(res)
 
-    def new_community_type(self, project_id, name, facet=None):
+    def new_community_type(self, project_id, name, facet=None, photo=None):
         """Creates a new community type
 
         :param project_id: Project Identifier
         :param name: community type name
         :param facet: facet name associated with the community
+        :param photo: Address to the photo of the community
 
         Example::
 
             >>> client.new_community_type(
                     'Xh9CeyQtTYe2cv5F11e6nQ',
                     'Community_type_1',
-                    facet='Company'
+                    facet='Company',
+                    photo='https://twitter.com/MarcusRashford/photo',
                     )
             {
                 "id": "LB5Q-GmBSbaNvJhUxXfUaA",
                 "created_at": "2020-09-09T15:15:42",
                 "modified_at": "2020-09-09T15:15:42",
                 "project_id": "Xh9CeyQtTYe2cv5F11e6nQ",
                 "name": "Community_type_1",
-                "facet": "Company"
+                "facet": "Company",
+                "photo": "https://twitter.com/MarcusRashford/photo",
             }
         """
 
         url = ("%(ep)s/v0/%(tenant)s/projects/%(project_id)s/" "community_types") % {
             "ep": self.topic_api_url,
             "tenant": self.tenant,
             "project_id": project_id,
         }
         data = {"name": name}
         if facet:
             data["facet"] = facet
+        if photo:
+            data["photo"] = photo
 
         headers = {"Content-Type": "application/json"}
         res = self._perform_request("post", url, data=json.dumps(data), headers=headers)
         return self._process_response(res, [201])
 
     def modify_community_type(self, project_id, community_type_id, name, facet=None):
-
         """Modifies a community type
 
         :param project_id: Project Identifier
         :param community_type_id: Community type Identifier
         :param name: community type name
         :param facet: facet name associated with the community
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/configuration.py` & `SquirroClient-3.8.2/squirro_client/topic/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,17 @@
                 'scope': None,
                 'config': {
                     'user.create': {
                         'value': False,
                         'default_value': True,
                         'type': 'boolean',
                         'delete': 'reset',
-                        'help': 'Whether new users can be created on this sytemn.'
+                        'help': 'Whether new users can be created on this sytemn.',
+                        'schema': None,
+                        'schema_model': None
                     },
                 },
                 # …
             }
         """
         # Build URL
         url = "{ep}/v0/{tenant}/configuration".format(
@@ -105,15 +107,17 @@
                 'namespace': 'server',
                 'scope': None,
                 'key': 'user.create',
                 'value': False,
                 'default_value': True,
                 'type': 'boolean',
                 'help': 'Whether new users can be created on this system.',
-                'delete': 'reset'
+                'delete': 'reset',
+                'schema': None,
+                'schema_model': None
             }
         """
         # Build URL
         url = "{ep}/v0/{tenant}/configuration/{key}".format(
             ep=self.topic_api_url,
             tenant=self.tenant,
             key=key,
@@ -144,26 +148,30 @@
             {
                 'key': 'topic.custom-locator',
                 'value': False,
                 'default_value': False,
                 'type': 'boolean',
                 'help': 'Whether custom index locators can be defined on Squirro projects.',
                 'delete': 'noop',
+                'schema': None,
+                'schema_model': None
             }
 
             >>> c.set_server_configuration(key='user.create', value=False)
             {
                 'namespace': 'server',
                 'scope': None,
                 'key': 'user.create',
                 'value': False,
                 'default_value': True,
                 'type': 'boolean',
                 'help': 'Whether new users can be created on this system.',
-                'delete': 'reset'
+                'delete': 'reset',
+                'schema': None,
+                'schema_model': None
             }
         """
 
         # Build URL
         url = "{ep}/v0/{tenant}/configuration/{key}".format(
             ep=self.topic_api_url,
             tenant=self.tenant,
@@ -215,15 +223,17 @@
                 'scope': 'd_GZJjMiVgKHHf6-pFWzNQ',
                 'config': {
                     'topic.typeahead.popular.scope': {
                         'value': 'user',
                         'default_value': 'user',
                         'type': 'string',
                         'delete': 'reset',
-                        'help': 'A scope for popular queries (user/project).'
+                        'help': 'A scope for popular queries (user/project).',
+                        'schema': None,
+                        'schema_model': None
                     },
                 },
                 # …
             }
         """
         url = (
             f"{self.topic_api_url}/v0/{self.tenant}/projects/{project_id}/configuration"
@@ -279,15 +289,17 @@
                 'namespace': 'project',
                 'scope': 'd_GZJjMiVgKHHf6-pFWzNQ',
                 'key': 'topic.typeahead.popular.scope',
                 'value': 'project',
                 'default_value': 'user',
                 'type': 'string',
                 'help': 'A scope for popular queries (user/project).',
-                'delete': 'reset'
+                'delete': 'reset',
+                'schema': None,
+                'schema_model': None
             }
         """
         url = f"{self.topic_api_url}/v0/{self.tenant}/projects/{project_id}/configuration/{key}"
         headers = {"Content-Type": "application/json"}
         post_data = {"value": value, "type": type}
         res = self._perform_request(
             "put", url, data=json.dumps(post_data), headers=headers
@@ -316,14 +328,16 @@
             {
                 'key': 'topic.typeahead.popular.scope',
                 'value': 'user',
                 'default_value': 'user,
                 'type': 'string',
                 'help': 'A scope for popular queries (user/project).',
                 'delete': 'noop',
+                'schema': None,
+                'schema_model': None
             }
         """
         url = f"{self.topic_api_url}/v0/{self.tenant}/projects/{project_id}/configuration/{key}"
         res = self._perform_request("delete", url)
         return self._process_response(res, [200, 204])
 
     def interpolate_project_configuration(self, project_id: str, value: Any):
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/contributingrecords.py` & `SquirroClient-3.8.2/squirro_client/topic/contributingrecords.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/dashboards.py` & `SquirroClient-3.8.2/squirro_client/topic/dashboards.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/email_templates.py` & `SquirroClient-3.8.2/squirro_client/topic/email_templates.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/enrichments.py` & `SquirroClient-3.8.2/squirro_client/topic/enrichments.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/entities.py` & `SquirroClient-3.8.2/squirro_client/topic/entities.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/facets.py` & `SquirroClient-3.8.2/squirro_client/topic/facets.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/file_upload.py` & `SquirroClient-3.8.2/squirro_client/topic/file_upload.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/globaltemp.py` & `SquirroClient-3.8.2/squirro_client/topic/globaltemp.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,29 @@
         """
         if not os.path.exists(filename):
             raise ValueError(f"Can not find file {filename}")
 
         data = open(filename, "rb").read()
         return self.new_tempfile(data=data)
 
-    def new_tempfile(self, data):
+    def new_tempfile(self, data, filename=None):
         """Stores the `data` in a temp file.
 
         :param data: data to be stored in the temp file
+        :param filename: optional filename, serving as metadata of the temp file.
         """
 
         url = "{ep}/v0/{tenant}/temp".format(
             ep=self.topic_api_url,
             tenant=self.tenant,
         )
         headers = {}
+        if filename is not None:
+            headers["X-Filename"] = filename
+
         res = self._perform_request("post", url, files={"file": data}, headers=headers)
         return self._process_response(res, [201])
 
     def get_tempfile(self, filename, file_type=None):
         """Returns the content of the temp file with the name `filename`.
 
         :param filename: File name
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/guidefiles.py` & `SquirroClient-3.8.2/squirro_client/topic/guidefiles.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/machinelearning.py` & `SquirroClient-3.8.2/squirro_client/topic/machinelearning.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_candidate_set.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_candidate_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLCandidateSetMixin:
-
     #
     #  ML Candidate Set (CS)
     #
     def get_candidate_sets(self, project_id):
         """Return all Candidate Sets for a project.
 
         :param project_id: Id of the Squirro project.
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_groundtruth.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_groundtruth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLGroundTruthMixin:
-
     #
     #  ML Groundtruth (GT)
     #
     def get_groundtruths(self, project_id):
         """Return all ground truth for a project in a list.
 
         :param project_id: Id of the Squirro project.
@@ -30,14 +29,31 @@
         return self._process_response(res)
 
     def get_groundtruth(self, project_id, groundtruth_id):
         """Get a single Ground Truth.
 
         :param project_id: Id of the Squirro project.
         :param groundtruth_id: Id of the GroundTruth
+
+        **Examples**
+
+        *Get a single groundtruth*::
+
+            >>> client.get_groundtruth(
+                        project_id="DSuNrcnlSc6x5SJZh02IyQ",
+                        groundtruth_id="n57sJlpcTLy4_XxdvHvx5g")
+            {'bulk_labeling_status': 'no bulk labelings',
+            'config': {'candidatesets': [], 'labels': ['yes', 'no']},
+            'created_at': '1996-03-13T00:00:00',
+            'id': 'n57sJlpcTLy4_XxdvHvx5g',
+            'modified_at': '2015-06-09T00:00:00',
+            'name': 'Commercial final fly share white focus voice.',
+            'project_id': 'DSuNrcnlSc6x5SJZh02IyQ',
+            'bulk_labeling_status': 'no bulk labelings'
+            'rules': {}}
         """
         base_url = "{}/v0/{}/projects/{}/groundtruths/{}"
         headers = {"Content-Type": "application/json"}
 
         url = base_url.format(
             self.topic_api_url, self.tenant, project_id, groundtruth_id
         )
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_model.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLModelsMixin:
-
     #
     #  ML Model
     #
     def get_ml_models(self, project_id):
         """Return all ML Models for a project.
 
         :param project_id: Id of the Squirro project.
@@ -151,14 +150,15 @@
 
     def get_bulk_labeling(
         self,
         project_id,
         groundtruth_id,
         ml_workflow_fields: Optional[List[str]] = None,
         ml_job_fields: Optional[List[str]] = None,
+        job_count: Optional[int] = None,
     ):
         """Get new bulk labeling status.
 
         :param project_id: Id of the Squirro project.
         :param groundtruth_id: id of the grountruth.
         :param ml_workflow_fields: list of fields of ML workflows
         :param ml_job_fields: list of fields of ML jobs
@@ -171,14 +171,15 @@
             groundtruth_id=groundtruth_id,
         )
         headers = {"Content-Type": "application/json"}
 
         params = {
             "ml_workflow_fields": ml_workflow_fields,
             "ml_job_fields": ml_job_fields,
+            "job_count": job_count,
         }
 
         res = self._perform_request(
             "get", url, data=json.dumps(params), headers=headers
         )
         return self._process_response(res, [200])
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_publish.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLPublishMixin:
-
     #
     #  ML Publish
     #
     def get_ml_published_models(self, project_id):
         """Returns all the publishing model for a given project.
 
         :param project_id: Id of the Squirro project.
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_sentence_splitter.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_sentence_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLSentenceSplitterMixin:
-
     #
     #  ML Sentence Splitter
     #
     def get_sentence_splitters(self, project_id):
         """Return all available Sentence Splitter.
 
         :param project_id: Id of the Squirro project.
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_template.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_template.py`

 * *Files identical despite different names*

```diff
@@ -7,15 +7,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job"""
 
     pass
 
 
 class MLTemplatesMixin:
-
     #
     #  ML Templates
     #
     def get_templates(self, project_id, groundtruth_id=None):
         """Return all available Templates.
 
         :param project_id: Id of the Squirro project.
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/ml_user_feedback.py` & `SquirroClient-3.8.2/squirro_client/topic/ml_user_feedback.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class ExecutionError(Exception):
     """Error in executing a machine learning job."""
 
     pass
 
 
 class MLUserFeedbackMixin:
-
     #
     #  User Feedback
     #
     def get_feedbacks(
         self,
         project_id,
         user_name=None,
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/objects.py` & `SquirroClient-3.8.2/squirro_client/topic/objects.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/pipeline_sections.py` & `SquirroClient-3.8.2/squirro_client/topic/pipeline_sections.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/pipeline_status.py` & `SquirroClient-3.8.2/squirro_client/topic/pipeline_status.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/pipeline_workflows.py` & `SquirroClient-3.8.2/squirro_client/topic/pipeline_workflows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from typing import List, Optional, Union
 
 
 class PipelineWorkflowMixin:
-
     #
     # Pipeline Workflows
     #
 
     def get_pipeline_workflows(self, project_id, omit_steps=False, omit_sources=False):
         """Return all pipeline workflows for project with `project_id`.
 
@@ -375,7 +374,53 @@
         )
 
         res = self._perform_request(
             "post", url, params=params, data=json.dumps(data), headers=headers
         )
 
         return self._process_response(res)
+
+    def add_model_to_pipeline_workflow(
+        self,
+        project_id,
+        workflow_id,
+        model_id,
+    ):
+        """Updates a pipeline workflow with a published model from AI Studio.
+
+        :param project_id: project id
+        :param workflow_id: pipeline workflow id
+        :param model_id: id of published model in AI Studio
+
+        Example::
+
+            >>> client.add_model_to_pipeline_workflow(
+            >>>     project_id='project_id_1',
+            >>>     workflow_id='pipeline_workflow_id_1',
+            >>>     model_id="model_id_1",
+        """
+        headers = {"Content-Type": "application/json"}
+        url = "{ep}/v0/{tenant}/projects/{project_id}/pipeline_sections".format(
+            ep=self.topic_api_url,
+            tenant=self.tenant,
+            project_id=project_id,
+        )
+
+        res = self._perform_request("get", url, headers=headers)
+
+        url = (
+            "%(ep)s/v0/%(tenant)s/projects/%(project_id)s/"
+            "pipeline_workflows/%(workflow_id)s/model/%(model_id)s"
+            % {
+                "ep": self.topic_api_url,
+                "tenant": self.tenant,
+                "project_id": project_id,
+                "workflow_id": workflow_id,
+                "model_id": model_id,
+            }
+        )
+
+        res = self._perform_request(
+            "put", url, data=json.dumps(res.json()), headers=headers
+        )
+
+        return self._process_response(res, [201])
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/project_translations.py` & `SquirroClient-3.8.2/squirro_client/topic/project_translations.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/projects.py` & `SquirroClient-3.8.2/squirro_client/topic/projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import re
 
 log = logging.getLogger(__name__)
 
 
 class ProjectsMixin:
-
     PROJECT_ATTRIBUTES = {
         "default_search",
         "title",
         "description",
         "default_sort",
         "locator",
         "guide_completed_steps",
@@ -719,15 +718,14 @@
         import_sources=True,
         import_sources_dataloader_plugins=True,
         import_trends=True,
         import_items=True,
         import_guide_file=True,
         import_ais_published_models=True,
     ):
-
         """Imports parts or all configuration and metadata of a project.
 
         The following entities can be imported:
             - dashboards
                 - optionally include dashboard loaders
                 - optionally include custom widgets
             - email_templates
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/savedsearches.py` & `SquirroClient-3.8.2/squirro_client/topic/savedsearches.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/smart_answers.py` & `SquirroClient-3.8.2/squirro_client/topic/smart_answers.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/smartfilters.py` & `SquirroClient-3.8.2/squirro_client/topic/smartfilters.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/sources.py` & `SquirroClient-3.8.2/squirro_client/topic/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -772,15 +772,14 @@
             "source_id": source_id,
         }
         data = {"data": {"max_inc_value": max_inc_value}}
         res = self._perform_request("put", url, data=json.dumps(data))
         self._process_response(res, [200, 204])
 
     def get_preview(self, project_id, config):
-
         """Preview the source configuration.
 
         :param project_id: Project identifier.
         :param config: Provider configuration.
         :returns: A dictionary which contains the source preview items.
 
         Example::
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/subscriptions.py` & `SquirroClient-3.8.2/squirro_client/topic/subscriptions.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/suggest_images.py` & `SquirroClient-3.8.2/squirro_client/topic/suggest_images.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/synonyms.py` & `SquirroClient-3.8.2/squirro_client/topic/synonyms.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/tasks.py` & `SquirroClient-3.8.2/squirro_client/topic/tasks.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/themes.py` & `SquirroClient-3.8.2/squirro_client/topic/themes.py`

 * *Files identical despite different names*

### Comparing `SquirroClient-3.7.1/squirro_client/topic/trenddetection.py` & `SquirroClient-3.8.2/squirro_client/topic/trenddetection.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,14 @@
         )
 
         # TODO: remove the logic for getting the historical data once the
         # trends-service store the historical data itself
         # get first & last timestamp of thresholds data, in order to filter the
         # historical data with the same time stamps
         if include_historical_data:
-
             # return empty historical data if we get back no thresholds data
             if len(ret["thresholds"]) < 2:
                 ret["historical_values"] = {"values": []}
 
             else:
                 interval = (
                     datetime.strptime(
```

### Comparing `SquirroClient-3.7.1/squirro_client/topic/widgets_assets.py` & `SquirroClient-3.8.2/squirro_client/topic/widgets_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from tarfile import TarInfo
 
 import hjson
 import tarsafe
 
 
 class WidgetsAndAssetsMixin:
-
     #
     # Dashboard Custom Widgets
     #
 
     def get_dashboard_widgets(self):
         """Return all dashboard widgets (for tenant).
```

### Comparing `SquirroClient-3.7.1/squirro_client/user.py` & `SquirroClient-3.8.2/squirro_client/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import re
 
+from squirro_client.util import deprecation
+
 
 class UserApiMixin:
     """Mixin class which encapsulates the functionality of the user API
     service.
 
     All the methods of this class are made available in the
     [[SquirroClient]] class.
@@ -486,17 +488,40 @@
             >>> client.get_token_from_msexchuid('89edf14d-90c4-834d-9efc-cd20a93fc74b')
             {
                 u'oauth2_token': u'5ad37930dda85a7...6c066b2253dba8d19',
                 u'user_id': u'vP7h4g7EThuJKIfMorHTUQ',
             }
         """
 
-        url = ("%(ep)s/msexchange/oauth2_token") % {"ep": self.user_api_url}
-        params = {}
-        params["msexchuid"] = msexchuid
+        msg = (
+            "The `get_token_from_msexchuid` method is obsolete. It has been replaced by"
+            " the `get_token_from_msexchuid_token` method."
+        )
+        deprecation(msg)
+        raise NotImplementedError(msg)
+
+    def get_token_from_msexchuid_token(self, msexchuid_token):
+        """
+        Retrieves an OAUTH2 authentication token based on the provided MS Exchange user
+        identity token.
+
+        :param msexchuid_token: a Microsoft Exchange user identity token (JWT).
+        :return: A dictionary containing the OAUTH2 token and the Squirro user id.
+
+        Example::
+
+            >>> client.get_token_from_msexchuid_token("<your.jwt.token>")
+            {
+                u'oauth2_token': u'5ad37930dda85a7...6c066b2253dba8d19',
+                u'user_id': u'vP7h4g7EThuJKIfMorHTUQ',
+            }
+        """
+        url = f"{self.user_api_url}/msexchange/oauth2_token"
+
+        params = {"msexchuid_token": msexchuid_token}
 
         res = self._perform_request("get", url, params=params)
         return self._process_response(res, [200])
 
     def add_project_member(self, project_id, role, user_id=None, group_id=None):
         """Adds a user or group to a project as a member.
```

### Comparing `SquirroClient-3.7.1/squirro_client/util.py` & `SquirroClient-3.8.2/squirro_client/util.py`

 * *Files identical despite different names*

