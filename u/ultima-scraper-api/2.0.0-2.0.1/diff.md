# Comparing `tmp/ultima_scraper_api-2.0.0.tar.gz` & `tmp/ultima_scraper_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-2.0.0.tar", max compression
+gzip compressed data, was "ultima_scraper_api-2.0.1.tar", max compression
```

## Comparing `ultima_scraper_api-2.0.0.tar` & `ultima_scraper_api-2.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1214 2023-07-11 11:46:57.031789 ultima_scraper_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.0.0/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2532 2023-07-11 07:31:18.304539 ultima_scraper_api-2.0.0/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.0.0/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6913 2023-06-01 15:05:27.454325 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     3377 2023-07-11 02:37:00.259116 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0     1306 2023-06-15 08:27:10.520823 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/auth_streamliner.py
--rw-r--r--   0        0        0      635 2023-07-11 11:18:35.577703 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2890 2023-07-11 11:19:18.696746 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    13795 2023-07-10 03:49:56.772912 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6562 2023-07-09 22:21:57.158649 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/comment_model.py
--rw-r--r--   0        0        0    14991 2023-07-10 03:22:18.901274 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6479 2023-07-08 08:28:30.959843 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     7348 2023-07-09 22:27:49.103017 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0     1102 2023-07-09 22:28:09.345831 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27699 2023-07-10 03:52:55.262488 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     6353 2023-07-11 07:36:55.711368 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2774 2023-07-08 03:39:16.755488 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      191 2023-06-01 22:07:45.846163 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    14098 2023-07-06 20:59:41.959524 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0      727 2023-07-06 21:08:54.518835 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
--rw-r--r--   0        0        0    17169 2023-07-08 05:22:05.900713 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2986 2023-07-09 22:29:54.823123 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3675 2023-07-09 22:31:18.494304 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1374 2023-07-09 22:31:37.387150 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1705 2023-07-08 03:21:45.085840 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    28663 2023-07-10 03:53:41.051494 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     6760 2023-07-11 07:31:38.247375 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2899 2023-06-21 10:24:55.083858 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0     1493 2023-07-11 08:03:54.563941 ultima_scraper_api-2.0.0/ultima_scraper_api/config.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    10870 2023-07-11 07:36:36.651955 ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     2318 2023-06-23 10:17:35.539928 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      781 2023-06-23 10:13:00.135609 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2977 2023-07-08 03:26:53.352487 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    18493 2023-07-11 09:31:06.300816 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.0.0/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-2.0.0/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.0.0/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 ultima_scraper_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1214 2023-07-12 02:16:21.840443 ultima_scraper_api-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.0.1/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2532 2023-07-11 07:31:18.304539 ultima_scraper_api-2.0.1/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.0.1/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6913 2023-06-01 15:05:27.454325 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     3377 2023-07-11 02:37:00.259116 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0     1306 2023-06-15 08:27:10.520823 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/auth_streamliner.py
+-rw-r--r--   0        0        0      635 2023-07-11 11:18:35.577703 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2890 2023-07-11 11:19:18.696746 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    13795 2023-07-10 03:49:56.772912 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6562 2023-07-09 22:21:57.158649 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/comment_model.py
+-rw-r--r--   0        0        0    14897 2023-07-12 00:02:33.358033 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6479 2023-07-08 08:28:30.959843 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     7348 2023-07-09 22:27:49.103017 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0     1102 2023-07-09 22:28:09.345831 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27699 2023-07-10 03:52:55.262488 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     6353 2023-07-11 07:36:55.711368 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2774 2023-07-08 03:39:16.755488 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-01 22:07:45.846163 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    14098 2023-07-06 20:59:41.959524 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0      727 2023-07-06 21:08:54.518835 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
+-rw-r--r--   0        0        0    17169 2023-07-12 00:02:37.331458 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2986 2023-07-09 22:29:54.823123 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3675 2023-07-09 22:31:18.494304 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1374 2023-07-09 22:31:37.387150 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1705 2023-07-08 03:21:45.085840 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28663 2023-07-10 03:53:41.051494 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     6760 2023-07-11 07:31:38.247375 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2899 2023-06-21 10:24:55.083858 ultima_scraper_api-2.0.1/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.0.1/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.0.1/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.1/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-2.0.1/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.1/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0     1493 2023-07-11 08:03:54.563941 ultima_scraper_api-2.0.1/ultima_scraper_api/config.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.1/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.1/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.0.1/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-2.0.1/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.0.1/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.0.1/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    10870 2023-07-11 07:36:36.651955 ultima_scraper_api-2.0.1/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     2318 2023-06-23 10:17:35.539928 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      781 2023-06-23 10:13:00.135609 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2977 2023-07-08 03:26:53.352487 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    18706 2023-07-12 00:01:51.627075 ultima_scraper_api-2.0.1/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.0.1/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-2.0.1/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.0.1/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 ultima_scraper_api-2.0.1/PKG-INFO
```

### Comparing `ultima_scraper_api-2.0.0/pyproject.toml` & `ultima_scraper_api-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "2.0.0"
+version = "2.0.1"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/__init__.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/auth_streamliner.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/auth_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/comment_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
-from user_agent import generate_user_agent
-
 from ultima_scraper_api.managers.session_manager import SessionManager
+from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 
 from ultima_scraper_api.apis import api_helper
 
 
@@ -333,16 +332,14 @@
     link: str = "https://onlyfans.com/",
 ):
     headers: dict[str, Any] = {}
     headers["user-agent"] = user_agent
     headers["referer"] = link
     headers["user-id"] = str(auth_id)
     headers["x-bc"] = ""
-    for remove_header in dynamic_rules["remove_headers"]:
-        headers.pop(remove_header)
     return headers
 
 
 def handle_refresh(object_: object, name: str):
     final_argument = getattr(object_, name)
     return final_argument
```

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/comment_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/config.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/config.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-2.0.1/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-2.0.1/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/managers/session_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 from random import randint
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 import aiohttp
 import python_socks
 import requests
+import ultima_scraper_api
+import ultima_scraper_api.apis.api_helper as api_helper
 from aiohttp import ClientResponse, ClientSession
 from aiohttp.client_exceptions import (
     ClientConnectorError,
     ClientOSError,
     ClientPayloadError,
     ClientResponseError,
     ContentTypeError,
     ServerDisconnectedError,
 )
 from aiohttp_socks import ProxyConnectionError, ProxyConnector, ProxyError, ProxyInfo
 
-import ultima_scraper_api
-import ultima_scraper_api.apis.api_helper as api_helper
-
 if TYPE_CHECKING:
     auth_types = ultima_scraper_api.auth_types
 EXCEPTION_TEMPLATE = (
     ClientPayloadError,
     ContentTypeError,
     ClientOSError,
     ServerDisconnectedError,
@@ -88,17 +87,23 @@
         self.kill = False
         self.headers = headers
         self.proxies: list[str] = (
             proxies if proxies else auth.api.config.settings.network.proxies
         )
         self.proxy_manager = ProxyManager(self)
         site_settings = auth.api.config.site_apis.get_settings(auth.api.site_name)
-        dynamic_rules_url = getattr(site_settings, "dynamic_rules_url")
-        dynamic_rules = requests.get(dynamic_rules_url).json()  # type: ignore
-        self.dynamic_rules = dynamic_rules
+        self.dynamic_rules = None
+        from ultima_scraper_api.apis.onlyfans.classes.extras import (
+            OnlyFansAuthenticator,
+        )
+
+        if isinstance(auth, OnlyFansAuthenticator):
+            dynamic_rules_url = getattr(site_settings, "dynamic_rules_url")
+            dynamic_rules = requests.get(dynamic_rules_url).json()  # type: ignore
+            self.dynamic_rules = dynamic_rules
         self.auth = auth
         self.use_cookies: bool = use_cookies
         self.active_session = self.create_client_session()
         self.request_count = 0
         # self.last_request_time: float | None = None
         # self.rate_limit_wait_minutes = 6
         self.rate_limit_check = False
```

### Comparing `ultima_scraper_api-2.0.0/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-2.0.1/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.0.0/PKG-INFO` & `ultima_scraper_api-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

