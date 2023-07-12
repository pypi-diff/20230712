# Comparing `tmp/renderg-sdk-0.1.3.tar.gz` & `tmp/renderg-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\renderg-sdk-0.1.3.tar", last modified: Wed Jul 12 02:18:23 2023, max compression
+gzip compressed data, was "dist\renderg-sdk-0.1.5.tar", last modified: Wed Jul 12 07:53:13 2023, max compression
```

## Comparing `renderg-sdk-0.1.3.tar` & `renderg-sdk-0.1.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/
--rw-rw-rw-   0        0        0     3207 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2826 2023-06-20 07:08:22.000000 renderg-sdk-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/analyze_houdini/
--rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.3/analyze_houdini/__init__.py
--rw-rw-rw-   0        0        0     4248 2023-06-20 06:09:58.000000 renderg-sdk-0.1.3/analyze_houdini/analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:19.000000 renderg-sdk-0.1.3/analyze_houdini/houdini/
--rw-rw-rw-   0        0        0   942080 2023-05-22 08:30:57.000000 renderg-sdk-0.1.3/analyze_houdini/houdini/HoudiniAnalyze.pyd
--rw-rw-rw-   0        0        0  1128448 2023-05-22 08:30:57.000000 renderg-sdk-0.1.3/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
--rw-rw-rw-   0        0        0   820224 2023-05-22 08:30:57.000000 renderg-sdk-0.1.3/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
--rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.3/analyze_houdini/houdini/run.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:19.000000 renderg-sdk-0.1.3/ascp/
--rw-rw-rw-   0        0        0        0 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/ascp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/ascp/bin/
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-file-l1-2-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-file-l2-1-0.dll
--rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
--rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
--rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
--rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
--rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
--rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
--rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
--rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
--rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/ascp.exe
--rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/ascp4.exe
--rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.3/ascp/bin/aspera-scp-transfer.0.log
--rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/aspera-scp-transfer.log
--rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/aspera.exe
--rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/concrt140.dll
--rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/fasp3_shared.dll
--rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/libeay32.dll
--rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/msvcp100.dll
--rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/msvcp140.dll
--rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/msvcr100.dll
--rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/ssleay32.dll
--rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/ucrtbase.dll
--rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/vccorlib140.dll
--rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/bin/vcruntime140.dll
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/ascp/etc/
--rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/aspera-license
--rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/aspera.conf
--rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/aspera_tokenauth_id_rsa
--rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/asperaweb_id_dsa.openssh
--rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/asperaweb_id_dsa.putty
--rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/ascp/etc/curl-ca-bundle.crt
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_api/
--rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.3/renderg_api/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-06-16 01:07:50.000000 renderg-sdk-0.1.3/renderg_api/connect.py
--rw-rw-rw-   0        0        0      518 2023-06-20 07:08:22.000000 renderg-sdk-0.1.3/renderg_api/constants.py
--rw-rw-rw-   0        0        0     1183 2023-06-15 06:53:33.000000 renderg-sdk-0.1.3/renderg_api/core.py
--rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.3/renderg_api/exception.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_api/operators/
--rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.3/renderg_api/operators/__init__.py
--rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.3/renderg_api/operators/env.py
--rw-rw-rw-   0        0        0     2496 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_api/operators/job.py
--rw-rw-rw-   0        0        0      103 2023-06-15 02:27:45.000000 renderg-sdk-0.1.3/renderg_api/operators/project.py
--rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.3/renderg_api/operators/task.py
--rw-rw-rw-   0        0        0     1059 2023-06-15 08:52:48.000000 renderg-sdk-0.1.3/renderg_api/operators/transfer.py
--rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.3/renderg_api/operators/user.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_api/param_check/
--rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.3/renderg_api/param_check/__init__.py
--rw-rw-rw-   0        0        0     2428 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_api/param_check/check.py
--rw-rw-rw-   0        0        0      728 2023-06-16 01:12:35.000000 renderg-sdk-0.1.3/renderg_api/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/
--rw-rw-rw-   0        0        0     3207 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2652 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       62 2023-07-12 02:18:18.000000 renderg-sdk-0.1.3/renderg_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_upload/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/renderg_upload/__init__.py
--rw-rw-rw-   0        0        0      159 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/renderg_upload/asperaTransfer.py
--rw-rw-rw-   0        0        0     1474 2023-06-16 07:10:02.000000 renderg-sdk-0.1.3/renderg_upload/asperaTransferHelper.py
--rw-rw-rw-   0        0        0     3920 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_upload/assetsPathHelper.py
--rw-rw-rw-   0        0        0     2309 2023-07-12 02:16:37.000000 renderg-sdk-0.1.3/renderg_upload/rgUpload.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/renderg_utils/
--rw-rw-rw-   0        0        0      113 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_utils/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_utils/constants.py
--rw-rw-rw-   0        0        0     1131 2023-06-20 06:09:18.000000 renderg-sdk-0.1.3/renderg_utils/exception.py
--rw-rw-rw-   0        0        0     2655 2023-06-20 06:09:58.000000 renderg-sdk-0.1.3/renderg_utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-12 02:18:23.000000 renderg-sdk-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-07-12 02:17:17.000000 renderg-sdk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/
+-rw-rw-rw-   0        0        0     3341 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/analyze_houdini/
+-rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.5/analyze_houdini/__init__.py
+-rw-rw-rw-   0        0        0     4084 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/analyze_houdini/analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/
+-rw-rw-rw-   0        0        0   942080 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze.pyd
+-rw-rw-rw-   0        0        0  1128448 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
+-rw-rw-rw-   0        0        0   820224 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
+-rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/ascp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/bin/
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l2-1-0.dll
+-rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
+-rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
+-rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
+-rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
+-rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
+-rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
+-rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
+-rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ascp.exe
+-rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ascp4.exe
+-rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.0.log
+-rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.log
+-rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/aspera.exe
+-rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/concrt140.dll
+-rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/fasp3_shared.dll
+-rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/libeay32.dll
+-rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcp100.dll
+-rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcp140.dll
+-rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcr100.dll
+-rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ssleay32.dll
+-rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ucrtbase.dll
+-rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/vccorlib140.dll
+-rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/vcruntime140.dll
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/etc/
+-rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera-license
+-rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera.conf
+-rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera_tokenauth_id_rsa
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.openssh
+-rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.putty
+-rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/curl-ca-bundle.crt
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/
+-rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.5/renderg_api/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-06-16 01:07:50.000000 renderg-sdk-0.1.5/renderg_api/connect.py
+-rw-rw-rw-   0        0        0      518 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_api/constants.py
+-rw-rw-rw-   0        0        0     1183 2023-06-15 06:53:33.000000 renderg-sdk-0.1.5/renderg_api/core.py
+-rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.5/renderg_api/exception.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/operators/
+-rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.5/renderg_api/operators/__init__.py
+-rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.5/renderg_api/operators/env.py
+-rw-rw-rw-   0        0        0     2496 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_api/operators/job.py
+-rw-rw-rw-   0        0        0      103 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/project.py
+-rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/task.py
+-rw-rw-rw-   0        0        0     1059 2023-06-15 08:52:48.000000 renderg-sdk-0.1.5/renderg_api/operators/transfer.py
+-rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/user.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/param_check/
+-rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.5/renderg_api/param_check/__init__.py
+-rw-rw-rw-   0        0        0     3195 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/renderg_api/param_check/check.py
+-rw-rw-rw-   0        0        0      728 2023-06-16 01:12:35.000000 renderg-sdk-0.1.5/renderg_api/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3341 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2652 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       62 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_upload/
+-rw-rw-rw-   0        0        0        0 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/asperaTransfer.py
+-rw-rw-rw-   0        0        0     1474 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/asperaTransferHelper.py
+-rw-rw-rw-   0        0        0     3920 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_upload/assetsPathHelper.py
+-rw-rw-rw-   0        0        0     2309 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_upload/rgUpload.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_utils/
+-rw-rw-rw-   0        0        0      113 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/constants.py
+-rw-rw-rw-   0        0        0     1131 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/exception.py
+-rw-rw-rw-   0        0        0     2655 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/setup.py
```

### Comparing `renderg-sdk-0.1.3/PKG-INFO` & `renderg-sdk-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.3
+Version: 0.1.5
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -78,14 +78,19 @@
     "ChunkSize": 1,  # 一机多帧
     "Mark": "",  # 任务备注信息
     "PriorityFrames": "010:",  # 优先渲染帧 例：101:100-108x2 代表渲染首尾帧和100-108步长为2的帧
 
     "zone_id": config["ZONE_ID"],  # CPU 配置信息
     "ram_limit": config["RAM_LIMIT"],  # 内存配置
 }
+param_check_obj.set_houdini_render_node({
+    "/node/path/to/render": "1001-1100",
+    "/node/path/to/render/1": "100-1100",
+})
+
 param_check_obj.execute(**render_params)
 
 # ========上传任务并提交==========
 # 1. 获取 info.cfg 和 任务 ID 信息
 info_path = analyze_obj.info_path
 job_id = analyze_obj.job_id
```

### Comparing `renderg-sdk-0.1.3/README.md` & `renderg-sdk-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,19 @@
     "ChunkSize": 1,  # 一机多帧
     "Mark": "",  # 任务备注信息
     "PriorityFrames": "010:",  # 优先渲染帧 例：101:100-108x2 代表渲染首尾帧和100-108步长为2的帧
 
     "zone_id": config["ZONE_ID"],  # CPU 配置信息
     "ram_limit": config["RAM_LIMIT"],  # 内存配置
 }
+param_check_obj.set_houdini_render_node({
+    "/node/path/to/render": "1001-1100",
+    "/node/path/to/render/1": "100-1100",
+})
+
 param_check_obj.execute(**render_params)
 
 # ========上传任务并提交==========
 # 1. 获取 info.cfg 和 任务 ID 信息
 info_path = analyze_obj.info_path
 job_id = analyze_obj.job_id
```

### Comparing `renderg-sdk-0.1.3/analyze_houdini/analyze.py` & `renderg-sdk-0.1.5/analyze_houdini/analyze.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,28 +79,22 @@
             except BaseException as err:
                 print(err.__str__())
         if not dcc_exe_path or not os.path.isfile(dcc_exe_path):
             raise DCCExeNotFoundError(ErrorCode.DCCExeNotFoundError, dcc_exe_path)
 
         return dcc_exe_path
 
-    def analyze(self):
+    def analyze(self, cmd=None):
         self.check_file_version()
         if not self.dcc_exe_path:
             self.dcc_exe_path = self.find_dcc_exe()
 
         self._update_analyze_status(JobStatus.STATUS_ANALYZE_DOING)
         script_path = os.path.join(os.path.dirname(__file__), "houdini/run.py")
-        cmd = '"{exe_path}" "{script_path}" -input "{dcc_file}" -output "{info_file}"'.format(
-            exe_path=self.dcc_exe_path,
-            script_path=script_path,
-            dcc_file=self.dcc_file,
-            info_file=self.info_path
-        )
-        print(cmd)
+        cmd = cmd or [self.dcc_exe_path, script_path, "-input", self.dcc_file, "-output", self.info_path]
         code = renderg_utils.run_cmd(cmd, shell=True)
         if code != 0:
             self._update_analyze_status(JobStatus.STATUS_ANALYZE_FAILED)
             raise AnalyzeFailError(ErrorCode.AnalyzeFailError, "analyze exits unexpectedly")
 
         if not os.path.isfile(self.info_path):
             self._update_analyze_status(JobStatus.STATUS_ANALYZE_FAILED)
```

### Comparing `renderg-sdk-0.1.3/analyze_houdini/houdini/run.py` & `renderg-sdk-0.1.5/analyze_houdini/houdini/run.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-file-l1-2-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-file-l2-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-localization-l1-2-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-localization-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-synch-l1-2-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-synch-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-math-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-math-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-private-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-private-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-process-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-process-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-string-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-string-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-time-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-time-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll` & `renderg-sdk-0.1.5/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/ascp.exe` & `renderg-sdk-0.1.5/ascp/bin/ascp.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/ascp4.exe` & `renderg-sdk-0.1.5/ascp/bin/ascp4.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/aspera-scp-transfer.0.log` & `renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.0.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/aspera-scp-transfer.log` & `renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/aspera.exe` & `renderg-sdk-0.1.5/ascp/bin/aspera.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/concrt140.dll` & `renderg-sdk-0.1.5/ascp/bin/concrt140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/fasp3_shared.dll` & `renderg-sdk-0.1.5/ascp/bin/fasp3_shared.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/libeay32.dll` & `renderg-sdk-0.1.5/ascp/bin/libeay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/msvcp100.dll` & `renderg-sdk-0.1.5/ascp/bin/msvcp100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/msvcp140.dll` & `renderg-sdk-0.1.5/ascp/bin/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/msvcr100.dll` & `renderg-sdk-0.1.5/ascp/bin/msvcr100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/ssleay32.dll` & `renderg-sdk-0.1.5/ascp/bin/ssleay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/ucrtbase.dll` & `renderg-sdk-0.1.5/ascp/bin/ucrtbase.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/vccorlib140.dll` & `renderg-sdk-0.1.5/ascp/bin/vccorlib140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/bin/vcruntime140.dll` & `renderg-sdk-0.1.5/ascp/bin/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/etc/aspera-license` & `renderg-sdk-0.1.5/ascp/etc/aspera-license`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/etc/aspera_tokenauth_id_rsa` & `renderg-sdk-0.1.5/ascp/etc/aspera_tokenauth_id_rsa`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/etc/asperaweb_id_dsa.openssh` & `renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.openssh`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/etc/asperaweb_id_dsa.putty` & `renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.putty`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/ascp/etc/curl-ca-bundle.crt` & `renderg-sdk-0.1.5/ascp/etc/curl-ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/connect.py` & `renderg-sdk-0.1.5/renderg_api/connect.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/constants.py` & `renderg-sdk-0.1.5/renderg_api/constants.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/core.py` & `renderg-sdk-0.1.5/renderg_api/core.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/operators/env.py` & `renderg-sdk-0.1.5/renderg_api/operators/env.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/operators/job.py` & `renderg-sdk-0.1.5/renderg_api/operators/job.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/operators/transfer.py` & `renderg-sdk-0.1.5/renderg_api/operators/transfer.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_api/param_check/check.py` & `renderg-sdk-0.1.5/renderg_api/param_check/check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 import os.path
 
 import renderg_utils
 from renderg_utils import RenderGException
 
 
 class RenderGParamChecker(object):
+    render_nodes = dict()
 
     def __init__(self, api, analyze_obj):
         self.api = api
         self.analyze_obj = analyze_obj
 
         self.info_path = self.analyze_obj.info_path
         self.warning_path = self.analyze_obj.warning_path
 
+    def set_houdini_render_node(self, nodes):
+        info_data = renderg_utils.read_json(self.info_path)
+        info_nodes = info_data.get("Nodes", {})
+        render_nodes = dict()
+        for node, frame in nodes.items():
+            if node in info_nodes:
+                render_nodes[node] = {
+                    "Frames": frame
+                }
+            else:
+                raise KeyError("Node {} Not Found.".format(node))
+        self.render_nodes = render_nodes
+        custom_params = info_data.get("CustomParams", {})
+        custom_params.update({"Nodes": render_nodes})
+        info_data["CustomParams"] = custom_params
+        renderg_utils.write_json(self.info_path, info_data)
+
     def execute(self, info_path=None, **kwargs):
         if info_path and os.path.isfile(info_path):
             self.info_path = info_path
 
         if "zone_id" not in kwargs:
             raise ValueError('Required "zone_id" not specified')
         if "ram_limit" not in kwargs:
@@ -34,15 +52,15 @@
             nodes = info_data.get("Nodes", {})
             custom_params = {
                     'ChunkSize': int(kwargs.get("ChunkSize", 1)),  # 一机多帧
                     'ForceRenderFrames': kwargs.get("ForceRenderFrames", ""),  # 帧范围
                     'Mark': kwargs.get("Mark", ""),  # 备注
                     'PriorityFrames':  kwargs.get("PriorityFrames", ""),  # 优先测试帧
                     'use_custom_params': 1,
-                    'Nodes': self.__get_houdini_render_nodes(nodes),
+                    'Nodes': self.render_nodes or self.__get_houdini_render_nodes(nodes),
                     'farm_envs': self.api.env.get_env_info_by_id(self.analyze_obj.env_id),
             }
         if not custom_params:
             raise ValueError('"CustomParams" is empty. please set it')
 
         info_data["CustomParams"] = custom_params
         renderg_utils.write_json(self.info_path, info_data)
```

### Comparing `renderg-sdk-0.1.3/renderg_api/urls.py` & `renderg-sdk-0.1.5/renderg_api/urls.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_sdk.egg-info/PKG-INFO` & `renderg-sdk-0.1.5/renderg_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.3
+Version: 0.1.5
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -78,14 +78,19 @@
     "ChunkSize": 1,  # 一机多帧
     "Mark": "",  # 任务备注信息
     "PriorityFrames": "010:",  # 优先渲染帧 例：101:100-108x2 代表渲染首尾帧和100-108步长为2的帧
 
     "zone_id": config["ZONE_ID"],  # CPU 配置信息
     "ram_limit": config["RAM_LIMIT"],  # 内存配置
 }
+param_check_obj.set_houdini_render_node({
+    "/node/path/to/render": "1001-1100",
+    "/node/path/to/render/1": "100-1100",
+})
+
 param_check_obj.execute(**render_params)
 
 # ========上传任务并提交==========
 # 1. 获取 info.cfg 和 任务 ID 信息
 info_path = analyze_obj.info_path
 job_id = analyze_obj.job_id
```

### Comparing `renderg-sdk-0.1.3/renderg_sdk.egg-info/SOURCES.txt` & `renderg-sdk-0.1.5/renderg_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_upload/asperaTransferHelper.py` & `renderg-sdk-0.1.5/renderg_upload/asperaTransferHelper.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_upload/assetsPathHelper.py` & `renderg-sdk-0.1.5/renderg_upload/assetsPathHelper.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_upload/rgUpload.py` & `renderg-sdk-0.1.5/renderg_upload/rgUpload.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_utils/exception.py` & `renderg-sdk-0.1.5/renderg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/renderg_utils/utils.py` & `renderg-sdk-0.1.5/renderg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.3/setup.py` & `renderg-sdk-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
 setup(
     name='renderg-sdk',
-    version='0.1.3',
+    version='0.1.5',
     url='https://github.com/renderg-repo/renderg-sdk.git',
     author='RenderG',
     author_email='support@renderg.com',
     description='www.renderg.com',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

