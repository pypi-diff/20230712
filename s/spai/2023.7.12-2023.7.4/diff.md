# Comparing `tmp/spai-2023.7.12.tar.gz` & `tmp/spai-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.7.12.tar", max compression
+gzip compressed data, was "spai-2023.7.4.tar", max compression
```

## Comparing `spai-2023.7.12.tar` & `spai-2023.7.4.tar`

### file list

```diff
@@ -1,67 +1,64 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.7.12/README.md
--rw-r--r--   0        0        0      378 2023-07-12 07:54:35.780331 spai-2023.7.12/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.7.12/spai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.7.12/spai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.7.12/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.7.12/spai/cli/commands/auth.py
--rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.7.12/spai/cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.7.12/spai/cli/src/errors/auth.py
--rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.7.12/spai/cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.7.12/spai/cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.7.12/spai/cli/src/repos/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.7.12/spai/cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-09 08:55:33.898583 spai-2023.7.12/spai/cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.7.12/spai/cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.7.12/spai/cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.7.12/spai/cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.7.12/spai/cli/src/usecases/project/GetLogs.py
--rw-r--r--   0        0        0      669 2023-07-04 12:57:35.512652 spai-2023.7.12/spai/cli/src/usecases/project/GetServices.py
--rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.7.12/spai/cli/src/usecases/project/RunService.py
--rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.7.12/spai/cli/src/usecases/project/ScheduleService.py
--rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.7.12/spai/cli/src/usecases/project/StopService.py
--rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.7.12/spai/cli/src/usecases/project/__init__.py
--rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.7.12/spai/cli/src/usecases/project/init_project.py
--rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.7.12/spai/cli/src/usecases/project/main.py
--rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.7.12/spai/cli/src/usecases/project/project-template/README.md
--rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.7.12/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.7.12/spai/cli/src/usecases/project/project-template/spai.config.yml
--rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.7.12/spai/cli/src/usecases/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.7.12/spai/cli/src/usecases/run/__init__.py
--rw-r--r--   0        0        0     3660 2023-07-12 07:05:42.949086 spai-2023.7.12/spai/cli/src/usecases/run/cloud.py
--rw-r--r--   0        0        0     3458 2023-07-12 07:21:02.211592 spai-2023.7.12/spai/cli/src/usecases/run/local.py
--rw-r--r--   0        0        0     3780 2023-07-12 06:51:07.529211 spai-2023.7.12/spai/cli/src/usecases/run/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.7.12/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.7.12/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0      897 2023-07-11 07:19:41.711206 spai-2023.7.12/spai/data/satellite/download.py
--rw-r--r--   0        0        0      356 2023-07-11 07:28:45.016498 spai-2023.7.12/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3447 2023-07-11 07:19:41.715206 spai-2023.7.12/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.7.12/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.7.12/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.7.12/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.7.12/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.7.12/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.7.12/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7130 2023-07-11 07:37:52.082017 spai-2023.7.12/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.7.12/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.7.12/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.7.12/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.7.12/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.7.12/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.7.12/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.7.12/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     2298 2023-07-04 14:28:43.830331 spai-2023.7.12/spai/main.py
--rw-r--r--   0        0        0        0 2023-07-10 11:09:54.127903 spai-2023.7.12/spai/pulses/__init__.py
--rw-r--r--   0        0        0       41 2023-07-10 11:10:22.811986 spai-2023.7.12/spai/pulses/forest-monitoring.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.7.12/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.7.12/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.7.12/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.7.12/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.7.12/spai/storage/minio.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 spai-2023.7.12/setup.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 spai-2023.7.12/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.7.4/README.md
+-rw-r--r--   0        0        0      378 2023-07-04 15:45:54.547735 spai-2023.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.7.4/spai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.7.4/spai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.7.4/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.7.4/spai/cli/commands/auth.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.7.4/spai/cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.7.4/spai/cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.7.4/spai/cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.7.4/spai/cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.7.4/spai/cli/src/repos/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.7.4/spai/cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.7.4/spai/cli/src/usecases/project/GetLogs.py
+-rw-r--r--   0        0        0      669 2023-07-04 12:57:35.512652 spai-2023.7.4/spai/cli/src/usecases/project/GetServices.py
+-rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.7.4/spai/cli/src/usecases/project/RunService.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.7.4/spai/cli/src/usecases/project/ScheduleService.py
+-rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.7.4/spai/cli/src/usecases/project/StopService.py
+-rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.7.4/spai/cli/src/usecases/project/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.7.4/spai/cli/src/usecases/project/init_project.py
+-rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.7.4/spai/cli/src/usecases/project/main.py
+-rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.7.4/spai/cli/src/usecases/project/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.7.4/spai/cli/src/usecases/run/__init__.py
+-rw-r--r--   0        0        0     3591 2023-06-09 12:16:07.390164 spai-2023.7.4/spai/cli/src/usecases/run/cloud.py
+-rw-r--r--   0        0        0     3143 2023-06-09 10:29:07.730004 spai-2023.7.4/spai/cli/src/usecases/run/local.py
+-rw-r--r--   0        0        0     3698 2023-07-04 10:07:01.300284 spai-2023.7.4/spai/cli/src/usecases/run/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.7.4/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.7.4/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.7.4/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.7.4/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.7.4/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.7.4/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.7.4/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.7.4/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.7.4/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.7.4/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.7.4/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.7.4/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     2298 2023-07-04 14:28:43.830331 spai-2023.7.4/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.7.4/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.7.4/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.7.4/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.7.4/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.7.4/spai/storage/minio.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 spai-2023.7.4/setup.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 spai-2023.7.4/PKG-INFO
```

### Comparing `spai-2023.7.12/spai/cli/commands/auth.py` & `spai-2023.7.4/spai/cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/repos/APIRepo.py` & `spai-2023.7.4/spai/cli/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/repos/AuthRepo.py` & `spai-2023.7.4/spai/cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/auth/Auth.py` & `spai-2023.7.4/spai/cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/auth/main.py` & `spai-2023.7.4/spai/cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/GetServices.py` & `spai-2023.7.4/spai/cli/src/usecases/project/GetServices.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/README.md` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/apis/analytics/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/apis/xyz/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/spai.config.yml` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/spai.config.yml`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/project/project-template/uis/map/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/cli/src/usecases/run/cloud.py` & `spai-2023.7.4/spai/cli/src/usecases/run/cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import json
+import requests
 
 from ..project import get_services, stop_service, run_service, schedule_service
 
 
 def setup_files(item_type, dir):
     files = {
         item_type: open(
@@ -26,16 +26,14 @@
         "rebuild": rebuild,
         "command": item.command,
     }
     if item_type == "api" or item_type == "ui":
         data["port"] = item.port
     if item_type == "ui":
         data["command"] = item.command
-        if item.env:
-            data["env_vars"] = json.dumps(item.env)
     if item_type != "ui":
         data["storage"] = item.storage
     files = setup_files(item_type, item_dir)
     return run_service(user, item_type, files, data)
 
 
 def schedule_item(user, item, dir, typer, config, rebuild, item_type):
```

### Comparing `spai-2023.7.12/spai/cli/src/usecases/run/local.py` & `spai-2023.7.4/spai/cli/src/usecases/run/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,22 +31,17 @@
 
 
 def run_api(api, dir, port, host):
     os.chdir(dir)
     os.system(f"python apis/{api.name}/main.py --port {port} --host {host}")
 
 
-def run_ui(ui, dir, api_urls):
+def run_ui(ui, dir):
     os.chdir(dir)
-    cmd = ""
-    for name, value in ui.env.items():
-        if value in api_urls:
-            cmd += f"export {name}={api_urls[value]}; "
-    cmd += ui.command
-    os.system(cmd)
+    os.system(ui.command)
 
 
 def run_schdule():
     while True:
         schedule.run_pending()
         time.sleep(1)
 
@@ -74,33 +69,30 @@
             if notebook.run_on_start:
                 run_notebook((notebook, dir, typer))
             if notebook.run_every:
                 keep_alive = True
                 schedule.every(notebook.run_every).minutes.do(
                     run_notebook, (notebook, dir, typer)
                 )
-    api_urls = {}
     if config.apis:
         typer.echo(f"Deploying apis...")
         for api in config.apis:
             typer.echo(f"Running api '{api.name}'...")
             # TODO: reqs, env
             # load_dotenv(f"{dir}/apis/{api.name}/.env")
             p = Process(target=run_api, args=(api, dir, api.port, api.host))
             p.start()
             processes.append(p)
-            # save api_urls in case UIs need them
-            api_urls[f"api.{api.name}"] = f"http://{api.host}:{api.port}"
     if config.uis:
         typer.echo(f"Deploying uis...")
         for ui in config.uis:
             typer.echo(f"Running ui '{ui.name}'...")
             # TODO: reqs, env
             # load_dotenv(f"{dir}/apis/{api.name}/.env")
-            p = Process(target=run_ui, args=(ui, dir, api_urls))
+            p = Process(target=run_ui, args=(ui, dir))
             p.start()
             processes.append(p)
     typer.echo(f"Project '{config.project}' deployed.")
     if keep_alive:
         p = Process(target=run_schdule)
         p.start()
         processes.append(p)
```

### Comparing `spai-2023.7.12/spai/cli/src/usecases/run/validate.py` & `spai-2023.7.4/spai/cli/src/usecases/run/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     storage: Union[str, None] = None  # folder to bind in cloud
 
 
 class UIConfig(BaseModel):
     name: str
     command: str  # steamlit, javascript, ...
     port: int = 3000
-    env: dict = {}  # can accept the name of another service as a url placeholder
 
 
 class Config(BaseModel):
     project: Union[str, None] = None
     scripts: Union[List[ScriptConfig], None] = None
     notebooks: Union[List[NotebookConfig], None] = None
     apis: Union[List[APIConfig], None] = None
```

### Comparing `spai-2023.7.12/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         date_next_day = date_next_day.strftime("%Y-%m-%d")
         self.time_interval = (date_day_before, date_next_day)
 
     def download(self, gdf, date):
         self.prepare_time_interval(date)
         self.compute_image_size(gdf)
         if self.bbox_size[0] > 2500 or self.bbox_size[1] > 2500:
-            # return self.download_large_area(gdf)
-            raise Exception("Area too large")
+            return self.download_large_area(gdf)
         return self.download_small_area(self.bbox)
 
     def request_bands(self, bbox):
         return SentinelHubRequest(
             data_folder=self.download_folder,
             evalscript=self.script,
             input_data=[
@@ -85,8 +84,8 @@
         for i, bbox in enumerate(bbox_list):
             request_bands = self.request_bands(bbox)
             request_bands.save_data()
         downloaded_files = glob.glob(f"{self.download_folder}/*/response.tiff")
         dst_path = self.download_folder + "/output.tiff"
         command = f"gdal_merge.py -o {dst_path} " + " ".join(downloaded_files)
         os.system(command)
-        return dst_path
+        return dst_path
```

### Comparing `spai-2023.7.12/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/image/utils.py` & `spai-2023.7.4/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/image/xyz/cache.py` & `spai-2023.7.4/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/image/xyz/errors.py` & `spai-2023.7.4/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/image/xyz/get_image_tile.py` & `spai-2023.7.4/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/image/xyz/image_utils.py` & `spai-2023.7.4/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/main.py` & `spai-2023.7.4/spai/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/storage/BaseStorage.py` & `spai-2023.7.4/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/storage/CloudStorage.py` & `spai-2023.7.4/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/storage/Storage.py` & `spai-2023.7.4/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/spai/storage/minio.py` & `spai-2023.7.4/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.12/setup.py` & `spai-2023.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
  'spai.cli.src.usecases.project.project-template.uis.map',
  'spai.cli.src.usecases.run',
  'spai.data',
  'spai.data.satellite',
  'spai.data.satellite.sentinelhub',
  'spai.image',
  'spai.image.xyz',
- 'spai.pulses',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
  'spai.cli.src.usecases.project': ['project-template/*',
                                    'project-template/notebooks/analytics/*']}
 
@@ -32,15 +31,15 @@
 ['minio>=7.1.15,<8.0.0', 'pandas>=2.0.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.7.12',
+    'version': '2023.7.4',
     'description': '',
     'long_description': '# SPAI CLI\n\n## Create new project\n\n```bash\nspai init\n```\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spai-2023.7.12/PKG-INFO` & `spai-2023.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2023.7.12
+Version: 2023.7.4
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

