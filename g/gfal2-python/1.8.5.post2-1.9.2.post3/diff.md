# Comparing `tmp/gfal2-python-1.8.5.post2.tar.gz` & `tmp/gfal2-python-1.9.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gfal2-python-1.8.5.post2.tar", last modified: Wed Jan 18 12:14:41 2017, max compression
+gzip compressed data, was "dist/gfal2-python-1.9.2.post3.tar", last modified: Thu May 18 13:00:07 2017, max compression
```

## Comparing `gfal2-python-1.8.5.post2.tar` & `gfal2-python-1.9.2.post3.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/
-drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/cmake/
-drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/cmake/modules/
--rw-r--r--   0 aalvarez (32489) it        (2763)     1176 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/CMakeCXX11Support.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     4051 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/CMakeGeneratePkgConfig.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1077 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/CMakeMacroParseArguments.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1700 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/CMakeStringHelpers.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     4466 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/DefineInstallationPaths.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2111 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindCGSI_GSOAP.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1933 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindDCAP.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2667 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindDPM.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2960 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindDavix.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2570 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGFAL2.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2025 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGLIB2.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1736 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGRIDFTP_IFCE.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2041 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGTEST.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1959 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGTHREAD2.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2620 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_COMMON.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2796 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_FTP_CLIENT.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2704 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GASS_COPY.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2968 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSI_CERT_UTILS.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2969 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSI_CREDENTIAL.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2785 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSSAPI_GSI.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2754 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSS_ASSIST.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2090 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindLFC.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1624 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindPugiXML.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     6230 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/cmake/modules/FindPythonEasy.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2407 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindSRM_IFCE.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1884 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindUUID.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2126 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindVOMS.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     2153 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindXROOTD.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1892 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/FindZLIB.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     4052 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/cmake/modules/FindgSOAP.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)      561 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/MacroAddDoxygen.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)     1957 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/MacroAddepydoc.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)      972 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/MacroCopyFile.cmake
--rw-r--r--   0 aalvarez (32489) it        (2763)      400 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/cmake/modules/ReleaseDebugAutoFlags.cmake
-drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/
--rw-r--r--   0 aalvarez (32489) it        (2763)      676 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/PKG-INFO
--rw-r--r--   0 aalvarez (32489) it        (2763)     1721 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/SOURCES.txt
--rw-r--r--   0 aalvarez (32489) it        (2763)        1 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/dependency_links.txt
--rw-r--r--   0 aalvarez (32489) it        (2763)        1 2017-01-18 12:11:03.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/not-zip-safe
--rw-r--r--   0 aalvarez (32489) it        (2763)        6 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/gfal2_python.egg-info/top_level.txt
-drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/src/
--rw-r--r--   0 aalvarez (32489) it        (2763)      850 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/CMakeLists.txt
--rw-r--r--   0 aalvarez (32489) it        (2763)     1803 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/Directory.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     1132 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/src/Directory.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     2297 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/src/Dirent.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     3341 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/File.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     1544 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/src/File.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     5013 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/GErrorWrapper.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     1679 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/src/GErrorWrapper.h
--rw-r--r--   0 aalvarez (32489) it        (2763)    22739 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/Gfal2Context.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     6233 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/Gfal2Context.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     7444 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/GfaltParams.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     3808 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/GfaltParams.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     1725 2015-10-12 07:50:00.000000 gfal2-python-1.8.5.post2/src/LoggingHelper.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)      893 2015-10-12 07:50:00.000000 gfal2-python-1.8.5.post2/src/LoggingHelper.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     2264 2015-10-12 07:50:00.000000 gfal2-python-1.8.5.post2/src/Stat.h
--rw-r--r--   0 aalvarez (32489) it        (2763)    17858 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/src/gfal2.cpp
--rw-r--r--   0 aalvarez (32489) it        (2763)     1297 2015-10-12 07:50:00.000000 gfal2-python-1.8.5.post2/src/pyGIL.h
--rw-r--r--   0 aalvarez (32489) it        (2763)     1874 2017-01-18 08:06:24.000000 gfal2-python-1.8.5.post2/CMakeLists.txt
--rw-r--r--   0 aalvarez (32489) it        (2763)      103 2015-10-12 07:49:59.000000 gfal2-python-1.8.5.post2/MANIFEST.in
--rw-r--r--   0 aalvarez (32489) it        (2763)      231 2015-04-02 07:01:57.000000 gfal2-python-1.8.5.post2/README
--rwxr-xr-x   0 aalvarez (32489) it        (2763)     3312 2017-01-18 12:13:58.000000 gfal2-python-1.8.5.post2/setup.py
--rw-r--r--   0 aalvarez (32489) it        (2763)      676 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/PKG-INFO
--rw-r--r--   0 aalvarez (32489) it        (2763)       59 2017-01-18 12:14:41.000000 gfal2-python-1.8.5.post2/setup.cfg
+drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/
+drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/cmake/
+drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/cmake/modules/
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1176 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/CMakeCXX11Support.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     4051 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/CMakeGeneratePkgConfig.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1077 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/CMakeMacroParseArguments.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1700 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/CMakeStringHelpers.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     4466 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/DefineInstallationPaths.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2111 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindCGSI_GSOAP.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1933 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindDCAP.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2667 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindDPM.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2960 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindDavix.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2570 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGFAL2.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2025 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGLIB2.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1736 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGRIDFTP_IFCE.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2041 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGTEST.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1959 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGTHREAD2.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2620 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_COMMON.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2796 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_FTP_CLIENT.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2704 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GASS_COPY.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2968 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSI_CERT_UTILS.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2969 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSI_CREDENTIAL.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2785 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSSAPI_GSI.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2754 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSS_ASSIST.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2674 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_OPENSSL.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2090 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindLFC.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1624 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindPugiXML.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     5184 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindPythonEasy.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2407 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindSRM_IFCE.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1884 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindUUID.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2126 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindVOMS.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2153 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindXROOTD.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1892 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindZLIB.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     4452 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/cmake/modules/FindgSOAP.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)      561 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/MacroAddDoxygen.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1957 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/MacroAddepydoc.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)      972 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/MacroCopyFile.cmake
+-rw-r--r--   0 aalvarez (32489) it        (2763)      400 2017-02-06 10:11:17.000000 gfal2-python-1.9.2.post3/cmake/modules/ReleaseDebugAutoFlags.cmake
+drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/
+-rw-r--r--   0 aalvarez (32489) it        (2763)      676 2017-05-18 13:00:06.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/PKG-INFO
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1760 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/SOURCES.txt
+-rw-r--r--   0 aalvarez (32489) it        (2763)        1 2017-05-18 13:00:06.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/dependency_links.txt
+-rw-r--r--   0 aalvarez (32489) it        (2763)        1 2017-01-18 12:11:03.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/not-zip-safe
+-rw-r--r--   0 aalvarez (32489) it        (2763)        6 2017-05-18 13:00:06.000000 gfal2-python-1.9.2.post3/gfal2_python.egg-info/top_level.txt
+drwxr-xr-x   0 aalvarez (32489) it        (2763)        0 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/src/
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1617 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/src/CMakeLists.txt
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1795 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/src/Directory.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1132 2015-10-12 07:49:59.000000 gfal2-python-1.9.2.post3/src/Directory.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2297 2015-10-12 07:49:59.000000 gfal2-python-1.9.2.post3/src/Dirent.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     3327 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/src/File.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1544 2015-10-12 07:49:59.000000 gfal2-python-1.9.2.post3/src/File.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     5234 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/src/GErrorWrapper.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1679 2015-10-12 07:49:59.000000 gfal2-python-1.9.2.post3/src/GErrorWrapper.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)    22800 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/src/Gfal2Context.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     6690 2017-03-20 08:13:18.000000 gfal2-python-1.9.2.post3/src/Gfal2Context.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     9126 2017-03-20 08:13:18.000000 gfal2-python-1.9.2.post3/src/GfaltParams.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     3952 2017-03-20 08:13:18.000000 gfal2-python-1.9.2.post3/src/GfaltParams.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2908 2017-05-18 12:55:07.000000 gfal2-python-1.9.2.post3/src/LoggingHelper.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1837 2017-05-18 12:55:07.000000 gfal2-python-1.9.2.post3/src/LoggingHelper.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2264 2015-10-12 07:50:00.000000 gfal2-python-1.9.2.post3/src/Stat.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)    19821 2017-05-18 12:55:07.000000 gfal2-python-1.9.2.post3/src/gfal2.cpp
+-rw-r--r--   0 aalvarez (32489) it        (2763)     1297 2015-10-12 07:50:00.000000 gfal2-python-1.9.2.post3/src/pyGIL.h
+-rw-r--r--   0 aalvarez (32489) it        (2763)     2465 2017-03-20 08:13:17.000000 gfal2-python-1.9.2.post3/CMakeLists.txt
+-rw-r--r--   0 aalvarez (32489) it        (2763)      103 2015-10-12 07:49:59.000000 gfal2-python-1.9.2.post3/MANIFEST.in
+-rw-r--r--   0 aalvarez (32489) it        (2763)      231 2015-04-02 07:01:57.000000 gfal2-python-1.9.2.post3/README
+-rwxr-xr-x   0 aalvarez (32489) it        (2763)     3344 2017-05-18 12:59:44.000000 gfal2-python-1.9.2.post3/setup.py
+-rw-r--r--   0 aalvarez (32489) it        (2763)      676 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/PKG-INFO
+-rw-r--r--   0 aalvarez (32489) it        (2763)       59 2017-05-18 13:00:07.000000 gfal2-python-1.9.2.post3/setup.cfg
```

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/CMakeCXX11Support.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/CMakeCXX11Support.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/CMakeGeneratePkgConfig.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/CMakeGeneratePkgConfig.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/CMakeMacroParseArguments.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/CMakeMacroParseArguments.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/CMakeStringHelpers.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/CMakeStringHelpers.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/DefineInstallationPaths.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/DefineInstallationPaths.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindCGSI_GSOAP.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindCGSI_GSOAP.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindDCAP.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindDCAP.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindDPM.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindDPM.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindDavix.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindDavix.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGFAL2.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGFAL2.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGLIB2.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGLIB2.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGRIDFTP_IFCE.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGRIDFTP_IFCE.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGTEST.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGTEST.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGTHREAD2.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGTHREAD2.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_COMMON.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_COMMON.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_FTP_CLIENT.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_FTP_CLIENT.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GASS_COPY.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GASS_COPY.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSI_CERT_UTILS.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSI_CERT_UTILS.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSI_CREDENTIAL.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSI_CREDENTIAL.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSSAPI_GSI.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSSAPI_GSI.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindGlobus_GSS_ASSIST.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindGlobus_GSS_ASSIST.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindLFC.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindLFC.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindPugiXML.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindPugiXML.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindSRM_IFCE.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindSRM_IFCE.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindUUID.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindUUID.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindVOMS.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindVOMS.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindXROOTD.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindXROOTD.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindZLIB.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindZLIB.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/FindgSOAP.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/FindgSOAP.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -88,16 +88,25 @@
 
 # -----------------------------------------------------
 # GSOAP_276_COMPAT_FLAGS and GSOAPVERSION
 # try to determine the flagfor the 2.7.6 compatiblity, break with 2.7.13 and re-break with 2.7.16
 # ----------------------------------------------------
 message(STATUS " - wsdlh : ${GSOAP_WSDL2H}")
 message(STATUS " - SOAPCPP2 : ${GSOAP_SOAPCPP2}")
-execute_process(COMMAND ${GSOAP_SOAPCPP2}  "-v"   OUTPUT_VARIABLE GSOAP_STRING_VERSION ERROR_VARIABLE GSOAP_STRING_VERSION )
+
+# some versions of soapcpp2 interpret "-v" as verbose, and hang while waiting for input
+# try "-help" first, and if it fails, do "-v"
+execute_process(COMMAND ${GSOAP_SOAPCPP2}  "-help"   OUTPUT_VARIABLE GSOAP_STRING_VERSION ERROR_VARIABLE GSOAP_STRING_VERSION )
 string(REGEX MATCH "[0-9]*\\.[0-9]*\\.[0-9]*" GSOAP_VERSION ${GSOAP_STRING_VERSION})
+
+if( "${GSOAP_VERSION}" STREQUAL "..")
+  execute_process(COMMAND ${GSOAP_SOAPCPP2}  "-v"   OUTPUT_VARIABLE GSOAP_STRING_VERSION ERROR_VARIABLE GSOAP_STRING_VERSION )
+  string(REGEX MATCH "[0-9]*\\.[0-9]*\\.[0-9]*" GSOAP_VERSION ${GSOAP_STRING_VERSION})
+endif()
+
 message(STATUS " - GSOAP VERSION : ${GSOAP_VERSION}")
 if( "${GSOAP_VERSION}"  VERSION_LESS "2.7.6")
 	set(GSOAP_276_COMPAT_FLAGS "")
 elseif ( "${GSOAP_VERSION}"  VERSION_LESS "2.7.14") 
 	set(GSOAP_276_COMPAT_FLAGS "-z")	
 else ( "${GSOAP_VERSION}"  VERSION_LESS "2.7.14") 
 	set(GSOAP_276_COMPAT_FLAGS "-z1 -z2")
```

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/MacroAddDoxygen.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/MacroAddDoxygen.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/MacroAddepydoc.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/MacroAddepydoc.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/cmake/modules/MacroCopyFile.cmake` & `gfal2-python-1.9.2.post3/cmake/modules/MacroCopyFile.cmake`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/gfal2_python.egg-info/PKG-INFO` & `gfal2-python-1.9.2.post3/gfal2_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gfal2-python
-Version: 1.8.5.post2
+Version: 1.9.2.post3
 Summary: Python bindings for gfal2
 Home-page: https://dmc.web.cern.ch/
 Author: DMC Devel
 Author-email: dmc-devel@cern.ch
 License: Apache 2
 Download-URL: https://gitlab.cern.ch/dmc/gfal2-bindings
 Description: Python bindings for gfal2
```

### Comparing `gfal2-python-1.8.5.post2/gfal2_python.egg-info/SOURCES.txt` & `gfal2-python-1.9.2.post3/gfal2_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 cmake/modules/FindGlobus_COMMON.cmake
 cmake/modules/FindGlobus_FTP_CLIENT.cmake
 cmake/modules/FindGlobus_GASS_COPY.cmake
 cmake/modules/FindGlobus_GSI_CERT_UTILS.cmake
 cmake/modules/FindGlobus_GSI_CREDENTIAL.cmake
 cmake/modules/FindGlobus_GSSAPI_GSI.cmake
 cmake/modules/FindGlobus_GSS_ASSIST.cmake
+cmake/modules/FindGlobus_OPENSSL.cmake
 cmake/modules/FindLFC.cmake
 cmake/modules/FindPugiXML.cmake
 cmake/modules/FindPythonEasy.cmake
 cmake/modules/FindSRM_IFCE.cmake
 cmake/modules/FindUUID.cmake
 cmake/modules/FindVOMS.cmake
 cmake/modules/FindXROOTD.cmake
```

### Comparing `gfal2-python-1.8.5.post2/src/Directory.cpp` & `gfal2-python-1.9.2.post3/src/Directory.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -24,36 +24,36 @@
 
 
 Directory::Directory(const Gfal2Context & context, const std::string & path) :
         cont(context.getContext()), path(path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    d = gfal2_opendir(cont->context, path.c_str(), &tmp_err);
+    d = gfal2_opendir(cont->get(), path.c_str(), &tmp_err);
     if (d == NULL)
         GErrorWrapper::throwOnError(&tmp_err);
 }
 
 
 Directory::~Directory()
 {
     ScopedGILRelease unlock;
-    (void) gfal2_closedir(cont->context, d, NULL);
+    (void) gfal2_closedir(cont->get(), d, NULL);
 }
 
 
 boost::python::tuple Directory::readpp()
 {
     GError* tmp_err = NULL;
     Dirent dirent;
     Stat stat;
 
     {
         ScopedGILRelease unlock;
-        dirent = gfal2_readdirpp(cont->context, d, &stat._st, &tmp_err);
+        dirent = gfal2_readdirpp(cont->get(), d, &stat._st, &tmp_err);
     }
 
     if (dirent.isValid() == false) {
         GErrorWrapper::throwOnError(&tmp_err);
         return boost::python::make_tuple(boost::python::object(), boost::python::object());
     }
 
@@ -62,11 +62,11 @@
 
 
 Dirent Directory::read()
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
 
-    Dirent dirent(gfal2_readdir(cont->context, d, &tmp_err));
+    Dirent dirent(gfal2_readdir(cont->get(), d, &tmp_err));
     GErrorWrapper::throwOnError(&tmp_err);
     return dirent;
 }
```

### Comparing `gfal2-python-1.8.5.post2/src/Directory.h` & `gfal2-python-1.9.2.post3/src/Directory.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/src/Dirent.h` & `gfal2-python-1.9.2.post3/src/Dirent.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/src/File.cpp` & `gfal2-python-1.9.2.post3/src/File.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -40,84 +40,84 @@
 File::File(const Gfal2Context & context, const std::string & path,
         const std::string & flag) :
         cont(context.getContext()), path(path), flag(flag)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     int flags_i = convert_open_flag_py_to_cpp(flag);
-    fd = gfal2_open(cont->context, path.c_str(), flags_i, &tmp_err);
+    fd = gfal2_open(cont->get(), path.c_str(), flags_i, &tmp_err);
     if (fd <= 0)
         GErrorWrapper::throwOnError(&tmp_err);
 }
 
 
 File::~File()
 {
     ScopedGILRelease unlock;
-    (void) gfal2_close(cont->context, fd, NULL);
+    (void) gfal2_close(cont->get(), fd, NULL);
 }
 
 
 std::string File::read(size_t count)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     std::vector<char> buf(count + 1); // vector on the heap for massive buffer size
-    ssize_t ret = gfal2_read(cont->context, fd, &(buf.front()), count, &tmp_err);
+    ssize_t ret = gfal2_read(cont->get(), fd, &(buf.front()), count, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
 
     buf[ret] = '\0';
     return std::string(&(buf.front()), ret);
 }
 
 
 std::string File::pread(off_t offset, size_t count)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     std::vector<char> buf(count + 1); // vector on the heap for massive buffer size
-    ssize_t ret = gfal2_pread(cont->context, fd, &(buf.front()), count, offset, &tmp_err);
+    ssize_t ret = gfal2_pread(cont->get(), fd, &(buf.front()), count, offset, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
 
     buf[ret] = '\0';
     return std::string(&(buf.front()), ret);
 }
 
 
 ssize_t File::write(const std::string & str)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     const size_t s_str = str.size();
 
-    ssize_t ret = gfal2_write(cont->context, fd, str.c_str(), s_str, &tmp_err);
+    ssize_t ret = gfal2_write(cont->get(), fd, str.c_str(), s_str, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 ssize_t File::pwrite(const std::string & str, off_t offset)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     const size_t s_str = str.size();
 
-    ssize_t ret = gfal2_pwrite(cont->context, fd, str.c_str(), s_str, offset, &tmp_err);
+    ssize_t ret = gfal2_pwrite(cont->get(), fd, str.c_str(), s_str, offset, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 off_t File::lseek(off_t offset, int flag)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    off_t ret = gfal2_lseek(cont->context, fd, offset, flag, &tmp_err);
+    off_t ret = gfal2_lseek(cont->get(), fd, offset, flag, &tmp_err);
     if (ret == ((off_t) 0) - 1)
         GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
```

### Comparing `gfal2-python-1.8.5.post2/src/File.h` & `gfal2-python-1.9.2.post3/src/File.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/src/GErrorWrapper.cpp` & `gfal2-python-1.9.2.post3/src/GErrorWrapper.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,23 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include "GErrorWrapper.h"
 
+// Python3 compat
+#if PY_MAJOR_VERSION >= 3
+
+#define PyInt_FromLong PyLong_FromLong
+#define PyString_FromString PyUnicode_FromString
+
+#endif
+
+
 using namespace PyGfal2;
 
 
 PyObject *PyGfal2::GErrorPyType = NULL;
 
 
 GErrorWrapper::GErrorWrapper(const std::string &msg, int error):
@@ -132,16 +141,21 @@
 {
     PyObject* func   = NULL;
     PyObject* method = NULL;
 
     if (!(func = PyCFunction_NewEx(methodDef, NULL, NULL)))
         goto exception;
 
+#if PY_MAJOR_VERSION >= 3
+    if (!(method = PyInstanceMethod_New(func)))
+        goto exception;
+#else
     if (!(method = PyMethod_New(func, NULL, klass)))
         goto exception;
+#endif
 
     if (PyDict_SetItemString(dict, methodDef->ml_name, method) < 0)
         goto exception;
 
     Py_DECREF(method);
     Py_DECREF(func);
     return 0;
@@ -184,17 +198,16 @@
 
     Py_DECREF(attrs);
 
     scope.attr("GError") = boost::python::borrowed(typeObj);
     return typeObj;
 
 exception:
-    Py_XDECREF(typeObj);
-    Py_XDECREF(attrs);
-    return NULL;
+    PyErr_Print();
+    abort();
 }
 
 
 void PyGfal2::GError2PyError(boost::python::list& pyerrors, size_t nerrors, GError** g_errors)
 {
     if (g_errors != NULL) {
         for (size_t i = 0; i < nerrors; ++i) {
```

### Comparing `gfal2-python-1.8.5.post2/src/GErrorWrapper.h` & `gfal2-python-1.9.2.post3/src/GErrorWrapper.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/src/Gfal2Context.cpp` & `gfal2-python-1.9.2.post3/src/Gfal2Context.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -47,26 +47,26 @@
 }
 
 
 int Gfal2Context::filecopy(const std::string &src, const std::string &dst)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfalt_copy_file(cont->context, NULL, src.c_str(), dst.c_str(), &tmp_err);
+    int ret = gfalt_copy_file(cont->get(), NULL, src.c_str(), dst.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::filecopy(const GfaltParams & p, const std::string & src,
         const std::string & dst)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfalt_copy_file(cont->context, p.params, src.c_str(), dst.c_str(), &tmp_err);
+    int ret = gfalt_copy_file(cont->get(), p.params, src.c_str(), dst.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 boost::python::object Gfal2Context::filecopy(const boost::python::list& srcs,
         const boost::python::list& dsts)
@@ -118,19 +118,19 @@
         }
     }
 
     {
         ScopedGILRelease unlock;
 
         if (nbchksum == 0) {
-            ret = gfalt_copy_bulk(cont->context, p.params, nbfiles, sources_ptr,
+            ret = gfalt_copy_bulk(cont->get(), p.params, nbfiles, sources_ptr,
                     destinations_ptr, NULL, &op_error, &file_errors);
         }
         else {
-            ret = gfalt_copy_bulk(cont->context, p.params, nbfiles, sources_ptr,
+            ret = gfalt_copy_bulk(cont->get(), p.params, nbfiles, sources_ptr,
                     destinations_ptr, checksums_ptr, &op_error, &file_errors);
         }
 
         if (ret < 0 && op_error != NULL)
             GErrorWrapper::throwOnError(&op_error);
     }
 
@@ -142,60 +142,60 @@
 
 
 Stat Gfal2Context::lstat(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     Stat st;
-    const int ret = gfal2_lstat(cont->context, path.c_str(), &st._st, &tmp_err);
+    const int ret = gfal2_lstat(cont->get(), path.c_str(), &st._st, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return st;
 }
 
 
 Stat Gfal2Context::stat_c(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     Stat st;
-    const int ret = gfal2_stat(cont->context, path.c_str(), &st._st, &tmp_err);
+    const int ret = gfal2_stat(cont->get(), path.c_str(), &st._st, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return st;
 }
 
 
 int Gfal2Context::access(const std::string & path, int flag)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_access(cont->context, path.c_str(), flag, &tmp_err);
+    const int ret = gfal2_access(cont->get(), path.c_str(), flag, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::chmod(const std::string & path, mode_t mode)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_chmod(cont->context, path.c_str(), mode, &tmp_err);
+    const int ret = gfal2_chmod(cont->get(), path.c_str(), mode, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 int Gfal2Context::unlink(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_unlink(cont->context, path.c_str(), &tmp_err);
+    const int ret = gfal2_unlink(cont->get(), path.c_str(), &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 boost::python::list Gfal2Context::unlink_list(const boost::python::list& pyfiles)
@@ -211,80 +211,86 @@
     for (size_t i = 0; i < nbfiles; ++i) {
         files.push_back(boost::python::extract<std::string>(pyfiles[i]));
         files_ptr[i] = files.back().c_str();
     }
 
     {
 	ScopedGILRelease unlock;
-	gfal2_unlink_list(cont->context, nbfiles, files_ptr, errors.data());
+	gfal2_unlink_list(cont->get(), nbfiles, files_ptr, errors.data());
     }
 
     boost::python::list pyerrors;
     GError2PyError(pyerrors, nbfiles, errors.data());
     return pyerrors;
 }
 
 
 int Gfal2Context::mkdir(const std::string & path, mode_t mode)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_mkdir(cont->context, path.c_str(), mode, &tmp_err);
+    const int ret = gfal2_mkdir(cont->get(), path.c_str(), mode, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 int Gfal2Context::mkdir_rec(const std::string & path, mode_t mode)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_mkdir_rec(cont->context, path.c_str(), mode,
+    const int ret = gfal2_mkdir_rec(cont->get(), path.c_str(), mode,
             &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 int Gfal2Context::rmdir(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const int ret = gfal2_rmdir(cont->context, path.c_str(), &tmp_err);
+    const int ret = gfal2_rmdir(cont->get(), path.c_str(), &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 boost::python::list Gfal2Context::listdir(const std::string & path)
 {
     GError* tmp_err = NULL;
-    DIR* d = gfal2_opendir(cont->context, path.c_str(), &tmp_err);
+    DIR* d = NULL;
+    {
+        ScopedGILRelease unlock;
+        d = gfal2_opendir(cont->get(), path.c_str(), &tmp_err);
+    }
     if (d == NULL) {
         GErrorWrapper::throwOnError(&tmp_err);
     }
 
     // Do the listing outside Python scope
     // Creating Python objects even via boost require acquiring the GIL
     std::list<std::string> temporary;
-
     {
         ScopedGILRelease unlock;
         struct dirent *st;
 
-        while ((st = gfal2_readdir(cont->context, d, &tmp_err)) != NULL) {
+        while ((st = gfal2_readdir(cont->get(), d, &tmp_err)) != NULL) {
             temporary.push_back(std::string(st->d_name));
         }
     }
 
     GError* close_error = NULL;
-    gfal2_closedir(cont->context, d, &close_error);
+    {
+        ScopedGILRelease unlock;
+        gfal2_closedir(cont->get(), d, &close_error);
+    }
 
     GErrorWrapper::throwOnError(&tmp_err);
     GErrorWrapper::throwOnError(&close_error);
 
     // Convert to a Python list
     boost::python::list result;
     for (std::list<std::string>::const_iterator i = temporary.begin(); i != temporary.end(); ++i) {
@@ -294,40 +300,40 @@
 }
 
 
 int Gfal2Context::rename(const std::string & src, const std::string & dest)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    int ret = gfal2_rename(cont->context, src.c_str(), dest.c_str(), &tmp_err);
+    int ret = gfal2_rename(cont->get(), src.c_str(), dest.c_str(), &tmp_err);
     if (ret != 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 std::string Gfal2Context::readlink(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     char buffer[MAX_BUFFER_SIZE];
-    ssize_t ret = gfal2_readlink(cont->context, path.c_str(), buffer, MAX_BUFFER_SIZE, &tmp_err);
+    ssize_t ret = gfal2_readlink(cont->get(), path.c_str(), buffer, MAX_BUFFER_SIZE, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return buffer;
 }
 
 
 std::string Gfal2Context::checksum(const std::string & uri,
         const std::string & chk_type, off_t start_offset, size_t data_length)
 {
     ScopedGILRelease unlock;
     char buffer[MAX_BUFFER_SIZE];
     GError* tmp_err = NULL;
-    gfal2_checksum(cont->context, uri.c_str(), chk_type.c_str(), start_offset,
+    gfal2_checksum(cont->get(), uri.c_str(), chk_type.c_str(), start_offset,
             data_length, buffer, MAX_BUFFER_SIZE, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return buffer;
 }
 
 
 std::string Gfal2Context::checksum(const std::string & uri,
@@ -338,53 +344,53 @@
 
 
 int Gfal2Context::symlink(const std::string & oldpath,
         const std::string & newpath)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    int ret = gfal2_symlink(cont->context, oldpath.c_str(), newpath.c_str(), &tmp_err);
+    int ret = gfal2_symlink(cont->get(), oldpath.c_str(), newpath.c_str(), &tmp_err);
     if (ret != 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 std::string Gfal2Context::getxattr(const std::string & file, const std::string & key)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     char buffer[MAX_BUFFER_SIZE];
-    const ssize_t ret = gfal2_getxattr(cont->context, file.c_str(), key.c_str(), buffer,
+    const ssize_t ret = gfal2_getxattr(cont->get(), file.c_str(), key.c_str(), buffer,
             MAX_BUFFER_SIZE, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return std::string(buffer);
 }
 
 
 int Gfal2Context::setxattr(const std::string & file, const std::string & key,
         const std::string & value, int flag)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
-    const ssize_t ret = gfal2_setxattr(cont->context, file.c_str(), key.c_str(),
+    const ssize_t ret = gfal2_setxattr(cont->get(), file.c_str(), key.c_str(),
             value.c_str(), value.size() + 1, flag, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return 0;
 }
 
 
 boost::python::list Gfal2Context::listxattr(const std::string & file)
 {
     ScopedGILRelease unlock;
     GError* tmp_err = NULL;
     char buffer[MAX_BUFFER_SIZE];
-    const ssize_t ret = gfal2_listxattr(cont->context, file.c_str(), buffer,
+    const ssize_t ret = gfal2_listxattr(cont->get(), file.c_str(), buffer,
             MAX_BUFFER_SIZE, &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
 
     boost::python::list resu;
     ssize_t current = 0;
     while (current < ret) {
@@ -399,30 +405,30 @@
 boost::python::tuple Gfal2Context::bring_online(const std::string& path, time_t pintime,
         time_t timeout, bool async)
 {
     ScopedGILRelease unlock;
 
     GError* tmp_err = NULL;
     char token[128] = { 0 };
-    int ret = gfal2_bring_online(cont->context, path.c_str(), pintime, timeout, token,
+    int ret = gfal2_bring_online(cont->get(), path.c_str(), pintime, timeout, token,
             sizeof(token), async, &tmp_err);
 
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
 
     return boost::python::make_tuple(ret, std::string(token));
 }
 
 
 int Gfal2Context::bring_online_poll(const std::string& path, const std::string& token)
 {
     ScopedGILRelease unlock;
 
     GError* tmp_err = NULL;
-    int ret = gfal2_bring_online_poll(cont->context, path.c_str(), token.c_str(),
+    int ret = gfal2_bring_online_poll(cont->get(), path.c_str(), token.c_str(),
             &tmp_err);
     if (ret < 0 && tmp_err->code == EAGAIN) {
         g_error_free(tmp_err);
         ret = 0;
     }
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
@@ -431,15 +437,15 @@
 
 
 int Gfal2Context::release(const std::string& path, const std::string& token)
 {
     ScopedGILRelease unlock;
 
     GError* tmp_err = NULL;
-    int ret = gfal2_release_file(cont->context, path.c_str(), token.c_str(), &tmp_err);
+    int ret = gfal2_release_file(cont->get(), path.c_str(), token.c_str(), &tmp_err);
     if (ret < 0)
         GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 boost::python::tuple Gfal2Context::bring_online_list(const boost::python::list& pyfiles,
         time_t pintime, time_t timeout, bool async)
@@ -457,15 +463,15 @@
         files_ptr[i] = files.back().c_str();
     }
 
     char token[128] = { 0 };
 
     {
 	ScopedGILRelease unlock;
-	gfal2_bring_online_list(cont->context, nbfiles, files_ptr, pintime, timeout, token,
+	gfal2_bring_online_list(cont->get(), nbfiles, files_ptr, pintime, timeout, token,
 			sizeof(token), async, errors.data());
     }
 
     boost::python::list pyerrors;
     GError2PyError(pyerrors, nbfiles, errors.data());
     return boost::python::make_tuple(pyerrors, std::string(token));
 }
@@ -484,15 +490,15 @@
     for (size_t i = 0; i < nbfiles; ++i) {
         files.push_back(boost::python::extract<std::string>(pyfiles[i]));
         files_ptr[i] = files.back().c_str();
     }
 
     {
 	ScopedGILRelease unlock;
-	gfal2_bring_online_poll_list(cont->context, nbfiles, files_ptr, token.c_str(),
+	gfal2_bring_online_poll_list(cont->get(), nbfiles, files_ptr, token.c_str(),
 			errors.data());
     }
 
     boost::python::list pyerrors;
     GError2PyError(pyerrors, nbfiles, errors.data());
     return pyerrors;
 }
@@ -512,15 +518,15 @@
     for (size_t i = 0; i < nbfiles; ++i) {
         files.push_back(boost::python::extract<std::string>(pyfiles[i]));
         files_ptr[i] = files.back().c_str();
     }
 
     {
 	ScopedGILRelease unlock;
-	gfal2_release_file_list(cont->context, nbfiles, files_ptr, token.c_str(),
+	gfal2_release_file_list(cont->get(), nbfiles, files_ptr, token.c_str(),
 			errors.data());
     }
 
     boost::python::list pyerrors;
     GError2PyError(pyerrors, nbfiles, errors.data());
     return pyerrors;
 }
@@ -528,15 +534,15 @@
 
 int Gfal2Context::abort_bring_online(const std::string &path, const std::string& token)
 {
     GError* error = NULL;
     const char* file_ptr = path.c_str();
     int ret;
     ScopedGILRelease unlock;
-    ret = gfal2_abort_files(cont->context, 1, &file_ptr, token.c_str(), &error);
+    ret = gfal2_abort_files(cont->get(), 1, &file_ptr, token.c_str(), &error);
     if (ret < 0)
         GErrorWrapper::throwOnError(&error);
     return ret;
 }
 
 
 boost::python::list Gfal2Context::abort_bring_online_list(
@@ -553,15 +559,15 @@
     for (size_t i = 0; i < nbfiles; ++i) {
         files.push_back(boost::python::extract<std::string>(pyfiles[i]));
         files_ptr[i] = files.back().c_str();
     }
 
     {
 	ScopedGILRelease unlock;
-	gfal2_abort_files(cont->context, nbfiles, files_ptr, token.c_str(),
+	gfal2_abort_files(cont->get(), nbfiles, files_ptr, token.c_str(),
 			errors.data());
     }
 
     boost::python::list pyerrors;
     GError2PyError(pyerrors, nbfiles, errors.data());
     return pyerrors;
 }
@@ -591,38 +597,38 @@
 }
 
 
 int Gfal2Context::get_opt_integer(const std::string & nmspace, const std::string & key)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_get_opt_integer(cont->context, nmspace.c_str(), key.c_str(), &tmp_err);
+    int ret = gfal2_get_opt_integer(cont->get(), nmspace.c_str(), key.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 std::string Gfal2Context::get_opt_string(const std::string & nmspace,
         const std::string & key)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    char* p = gfal2_get_opt_string(cont->context, nmspace.c_str(), key.c_str(), &tmp_err);
+    char* p = gfal2_get_opt_string(cont->get(), nmspace.c_str(), key.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return std::string(p);
 }
 
 
 boost::python::list Gfal2Context::get_opt_string_list(const std::string & nmspace, const std::string & key)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
     gsize size = 0;
     boost::python::list result;
-    char** res = gfal2_get_opt_string_list(cont->context, nmspace.c_str(), key.c_str(),
+    char** res = gfal2_get_opt_string_list(cont->get(), nmspace.c_str(), key.c_str(),
             &size, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     if (res) {
         for (size_t i = 0; i < size; i++)
             result.append(std::string(res[i]));
         g_strfreev(res);
     }
@@ -630,37 +636,37 @@
 }
 
 
 bool Gfal2Context::get_opt_boolean(const std::string & nmspace, const std::string & key)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    const bool ret = gfal2_get_opt_boolean(cont->context, nmspace.c_str(), key.c_str(),
+    const bool ret = gfal2_get_opt_boolean(cont->get(), nmspace.c_str(), key.c_str(),
             &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::set_opt_integer(const std::string & nmspace, const std::string & key, int value)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_set_opt_integer(cont->context, nmspace.c_str(), key.c_str(), value, &tmp_err);
+    int ret = gfal2_set_opt_integer(cont->get(), nmspace.c_str(), key.c_str(), value, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::set_opt_string(const std::string & nmspace, const std::string & key,
         const std::string & value)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_set_opt_string(cont->context, nmspace.c_str(), key.c_str(), (char*) value.c_str(), &tmp_err);
+    int ret = gfal2_set_opt_string(cont->get(), nmspace.c_str(), key.c_str(), (char*) value.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::set_opt_string_list(const std::string & nmspace,
         const std::string & key, const boost::python::list &py_value)
@@ -673,47 +679,47 @@
     const int size_list = value.size();
     char* tab_ptr[size_list + 1];
     for (int i = 0; i < size_list; i++) {
         tab_ptr[i] = (char*) value[i].c_str();
     }
     tab_ptr[size_list] = NULL;
 
-    int ret = gfal2_set_opt_string_list(cont->context, nmspace.c_str(), key.c_str(),
+    int ret = gfal2_set_opt_string_list(cont->get(), nmspace.c_str(), key.c_str(),
             tab_ptr, size_list, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::set_opt_boolean(const std::string & nmspace, const std::string & key, bool val)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_set_opt_boolean(cont->context, nmspace.c_str(), key.c_str(), val,
+    int ret = gfal2_set_opt_boolean(cont->get(), nmspace.c_str(), key.c_str(), val,
             &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::load_opts_from_file(const std::string & path)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_load_opts_from_file(cont->context, path.c_str(), &tmp_err);
+    int ret = gfal2_load_opts_from_file(cont->get(), path.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 boost::python::list Gfal2Context::get_plugin_names(void)
 {
     ScopedGILRelease unlock;
     boost::python::list pyplugins;
-    gchar** plugins = gfal2_get_plugin_names(cont->context);
+    gchar** plugins = gfal2_get_plugin_names(cont->get());
     int nplugins = g_strv_length(plugins);
 
     for (int i = 0; i < nplugins; ++i) {
         pyplugins.append(std::string(plugins[i]));
     }
     g_strfreev(plugins);
 
@@ -721,83 +727,87 @@
 }
 
 
 int Gfal2Context::set_user_agent(const std::string & agent, const std::string & version)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_set_user_agent(cont->context, agent.c_str(), version.c_str(), &tmp_err);
+    int ret = gfal2_set_user_agent(cont->get(), agent.c_str(), version.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 boost::python::tuple Gfal2Context::get_user_agent(void)
 {
     ScopedGILRelease unlock;
     const char* agent, *version;
-    gfal2_get_user_agent(cont->context, &agent, &version);
+    gfal2_get_user_agent(cont->get(), &agent, &version);
     return boost::python::make_tuple(agent, version);
 }
 
 
 int Gfal2Context::add_client_info(const std::string& key, const std::string& value)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_add_client_info(cont->context, key.c_str(), value.c_str(), &tmp_err);
+    int ret = gfal2_add_client_info(cont->get(), key.c_str(), value.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::remove_client_info(const std::string& key)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_remove_client_info(cont->context, key.c_str(), &tmp_err);
+    int ret = gfal2_remove_client_info(cont->get(), key.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 int Gfal2Context::clear_client_info(void)
 {
     ScopedGILRelease unlock;
     GError * tmp_err = NULL;
-    int ret = gfal2_clear_client_info(cont->context, &tmp_err);
+    int ret = gfal2_clear_client_info(cont->get(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return ret;
 }
 
 
 boost::python::dict Gfal2Context::get_client_info(void)
 {
     ScopedGILRelease unlock;
     boost::python::dict dictionary;
 
     GError* tmp_err = NULL;
-    size_t nitems = gfal2_get_client_info_count(cont->context, &tmp_err);
+    size_t nitems = gfal2_get_client_info_count(cont->get(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 
     for (size_t i = 0; i < nitems; ++i) {
         const char *key, *value;
-        gfal2_get_client_info_pair(cont->context, i, &key, &value, &tmp_err);
+        gfal2_get_client_info_pair(cont->get(), i, &key, &value, &tmp_err);
         GErrorWrapper::throwOnError(&tmp_err);
         dictionary[key] = value;
     }
 
     return dictionary;
 }
 
+void Gfal2Context::free()
+{
+    cont->free();
+}
 
 int Gfal2Context::cancel()
 {
     ScopedGILRelease unlock;
-    return gfal2_cancel(cont->context);
+    return gfal2_cancel(cont->get());
 }
 
 
 int PyGfal2::gfal_set_verbose_enum(GLogLevelFlags lvls)
 {
     ScopedGILRelease unlock;
     gfal2_log_set_level(lvls);
```

### Comparing `gfal2-python-1.8.5.post2/src/Gfal2Context.h` & `gfal2-python-1.9.2.post3/src/Gfal2Context.h`

 * *Files 8% similar despite different names*

```diff
@@ -39,27 +39,47 @@
 #include "Stat.h"
 #include "pyGIL.h"
 
 namespace PyGfal2 {
 
 class GfalContextWrapper
 {
-public:
+private:
     gfal2_context_t context;
 
+public:
+
     GfalContextWrapper()
     {
         GError* tmp_err = NULL;
         context = gfal2_context_new(&tmp_err);
-        if (context == NULL)
+        if (context == NULL) {
             GErrorWrapper::throwOnError(&tmp_err);
+        }
     }
     ~GfalContextWrapper()
     {
+        if (context != NULL) {
+            gfal2_context_free(context);
+        }
+    }
+
+    gfal2_context_t get() {
+        if (context == NULL) {
+            throw GErrorWrapper("gfal2 context has been freed", EFAULT);
+        }
+        return context;
+    }
+
+    void free() {
+        if (context == NULL) {
+            throw GErrorWrapper("gfal2 context has been freed", EFAULT);
+        }
         gfal2_context_free(context);
+        context = NULL;
     }
 };
 
 
 class Gfal2Context
 {
 private:
@@ -78,14 +98,15 @@
         return PyGfal2::Gfal2Context();
     }
 
     boost::shared_ptr<GfalContextWrapper> getContext() const {
         return cont ;
     }
 
+    void free();
 
     int cancel();
 
     boost::shared_ptr<File> open(const std::string & path, const std::string &flag);
     boost::shared_ptr<File> file(const std::string & path, const std::string &flag);
 
     boost::shared_ptr<Directory> opendir(const std::string & path);
```

### Comparing `gfal2-python-1.8.5.post2/src/GfaltParams.cpp` & `gfal2-python-1.9.2.post3/src/GfaltParams.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,17 @@
  */
 
 #include "GfaltParams.h"
 #include "pyGIL.h"
 
 using namespace PyGfal2;
 
+#if PY_VERSION_HEX < 0x02060000
+#define PyErr_WarnEx(category, msg, level) PyErr_Warn(category, msg)
+#endif
 
 static void event_callback_wrapper(const gfalt_event_t e, gpointer user_data)
 {
 	ScopedGILLocker lock;
     CallbackObjs* callbacks = static_cast<CallbackObjs*>(user_data);
     if (callbacks->event_callback) {
         boost::python::call<void>(callbacks->event_callback.ptr(), GfaltEvent(e));
@@ -111,24 +114,33 @@
     GErrorWrapper::throwOnError(&tmp_err);
     return res;
 }
 
 
 void GfaltParams::set_checksum_check(bool checksum_check)
 {
-    GError * tmp_err = NULL;
-    gfalt_set_checksum_check(params, checksum_check, &tmp_err);
+    PyErr_WarnEx(PyExc_DeprecationWarning, "checksum_check is deprecated. Use set_checksum instead.", 1);
+
+    GError *tmp_err = NULL;
+    char type[64], buffer[512];
+
+    gfalt_get_checksum(params, type, sizeof(type), buffer, sizeof(buffer), &tmp_err);
+    GErrorWrapper::throwOnError(&tmp_err);
+
+    gfalt_set_checksum(params, checksum_check?GFALT_CHECKSUM_BOTH:GFALT_CHECKSUM_NONE, type, buffer, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 }
 
 
 bool GfaltParams::get_checksum_check()
 {
+    PyErr_WarnEx(PyExc_DeprecationWarning, "checksum_check is deprecated. Use get_checksum_mode instead.", 1);
+
     GError * tmp_err = NULL;
-    bool res = gfalt_get_checksum_check(params, &tmp_err);
+    bool res = gfalt_get_checksum_mode(params, &tmp_err) != GFALT_CHECKSUM_NONE;
     GErrorWrapper::throwOnError(&tmp_err);
     return res;
 }
 
 
 void GfaltParams::set_src_spacetoken(const std::string & token)
 {
@@ -163,27 +175,33 @@
     return (res) ? res : "";
 }
 
 
 void GfaltParams::set_user_defined_checksum(const std::string & chk_type,
         const std::string & checksum)
 {
+    PyErr_WarnEx(PyExc_DeprecationWarning, "set_user_defined_checksum is deprecated. Use set_checksum instead.", 1);
+
     GError * tmp_err = NULL;
-    gfalt_set_user_defined_checksum(params, chk_type.c_str(), checksum.c_str(), &tmp_err);
+    gfalt_checksum_mode_t current = gfalt_get_checksum_mode(params, &tmp_err);
+    GErrorWrapper::throwOnError(&tmp_err);
+
+    gfalt_set_checksum(params, current, chk_type.c_str(), checksum.c_str(), &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 }
 
 
 boost::python::tuple GfaltParams::get_user_defined_checksum()
 {
+    PyErr_WarnEx(PyExc_DeprecationWarning, "get_user_defined_checksum is deprecated. Use get_checksum instead.", 1);
+
     char buff_chktype[GFAL_URL_MAX_LEN];
     char buff_chk[GFAL_URL_MAX_LEN];
     GError * tmp_err = NULL;
-    gfalt_get_user_defined_checksum(params, buff_chktype, GFAL_URL_MAX_LEN, buff_chk,
-            GFAL_URL_MAX_LEN, &tmp_err);
+    gfalt_get_checksum(params, buff_chktype, GFAL_URL_MAX_LEN, buff_chk, GFAL_URL_MAX_LEN, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
     return boost::python::make_tuple<std::string, std::string>(buff_chktype, buff_chk);
 }
 
 
 void GfaltParams::set_overwrite(bool overwrite)
 {
@@ -248,19 +266,43 @@
 void GfaltParams::set_strict_copy(bool val)
 {
     GError * tmp_err = NULL;
     gfalt_set_strict_copy_mode(params, val, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 }
 
+
+void GfaltParams::set_checksum(gfalt_checksum_mode_t mode, const std::string &type, const std::string &value)
+{
+    GError *tmp_err = NULL;
+    gfalt_set_checksum(params, mode, type.c_str(), value.c_str(), &tmp_err);
+    GErrorWrapper::throwOnError(&tmp_err);
+}
+
+
+boost::python::tuple GfaltParams::get_checksum()
+{
+    char buff_chktype[GFAL_URL_MAX_LEN];
+    char buff_chk[GFAL_URL_MAX_LEN];
+    GError * tmp_err = NULL;
+    gfalt_checksum_mode_t mode = gfalt_get_checksum(params,
+        buff_chktype, GFAL_URL_MAX_LEN,
+        buff_chk, GFAL_URL_MAX_LEN,
+        &tmp_err);
+    GErrorWrapper::throwOnError(&tmp_err);
+
+    return boost::python::make_tuple<gfalt_checksum_mode_t, std::string, std::string>(mode, buff_chktype, buff_chk);
+}
+
+
 // Callbacks
 void GfaltParams::set_event_callback(PyObject* callable)
 {
     callback_objs.event_callback = boost::python::object(
-            boost::python::handle<>(callable));
+            boost::python::handle<>(boost::python::borrowed(callable)));
     GError *tmp_err = NULL;
     gfalt_add_event_callback(params, event_callback_wrapper,
             &callback_objs, NULL, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 }
 
 
@@ -269,15 +311,15 @@
     return callback_objs.event_callback.ptr();
 }
 
 
 void GfaltParams::set_monitor_callback(PyObject* callable)
 {
     callback_objs.monitor_callback = boost::python::object(
-            boost::python::handle<>(callable));
+            boost::python::handle<>(boost::python::borrowed(callable)));
     GError *tmp_err = NULL;
     gfalt_add_monitor_callback(params, monitor_callback_wrapper,
             &callback_objs, NULL, &tmp_err);
     GErrorWrapper::throwOnError(&tmp_err);
 }
 
 PyObject* GfaltParams::get_monitor_callback(void)
```

### Comparing `gfal2-python-1.8.5.post2/src/GfaltParams.h` & `gfal2-python-1.9.2.post3/src/GfaltParams.h`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,17 @@
     void                 set_create_parent(bool create_parent);
     bool                 get_create_parent(void);
     void                 set_tcp_buffersize(uint64_t buffersize);
     uint64_t             get_tcp_buffersize(void);
     bool                 get_strict_copy(void);
     void                 set_strict_copy(bool val);
 
+    void set_checksum(gfalt_checksum_mode_t mode, const std::string &type, const std::string &value);
+    boost::python::tuple get_checksum();
+
     // Callbacks
     void      set_event_callback(PyObject* callable);
     PyObject* get_event_callback(void);
     void      set_monitor_callback(PyObject* callable);
     PyObject* get_monitor_callback(void);
 
     friend class Gfal2Context;
```

### Comparing `gfal2-python-1.8.5.post2/src/Stat.h` & `gfal2-python-1.9.2.post3/src/Stat.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/src/gfal2.cpp` & `gfal2-python-1.9.2.post3/src/gfal2.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,27 @@
     boost::python::enum_<GLogLevelFlags>("verbose_level")
         .value("normal", G_LOG_LEVEL_CRITICAL)
         .value("warning", G_LOG_LEVEL_WARNING)
         .value("verbose", G_LOG_LEVEL_INFO)
         .value("debug", G_LOG_LEVEL_DEBUG)
         .value("trace", G_LOG_LEVEL_DEBUG);
 
+    boost::python::enum_<gfalt_checksum_mode_t>("checksum_mode")
+        .value("none", GFALT_CHECKSUM_NONE)
+        .value("source", GFALT_CHECKSUM_SOURCE)
+        .value("target", GFALT_CHECKSUM_TARGET)
+        .value("both", GFALT_CHECKSUM_BOTH);
+
     // register exception
     PyGfal2::GErrorPyType = PyGfal2::createGErrorExceptionType(gfal2Scope);
 
     boost::python::scope context_scope = boost::python::class_<PyGfal2::Gfal2Context>("Gfal2Context", "Gfal2 Context")
+        .def("free", &PyGfal2::Gfal2Context::free,
+            "Release internal resources used by the context. The instance can *not* be used after this"
+        )
         .def("open", &PyGfal2::Gfal2Context::open,
             "Opens a file and returns a file descriptor"
         )
         .def("file", &PyGfal2::Gfal2Context::file,
             "Synonym for open"
         )
         .def("opendir", &PyGfal2::Gfal2Context::opendir,
@@ -328,15 +337,21 @@
             &PyGfal2::GfaltParams::set_monitor_callback,
             "Callback for performance monitoring (i.e. throughput)"
         )
 
         .def("set_user_defined_checksum", &PyGfal2::GfaltParams::set_user_defined_checksum,
             "Specify manually the checksum type and value (optional)")
         .def("get_user_defined_checksum", &PyGfal2::GfaltParams::get_user_defined_checksum,
-            "Gets the user specified checksum");
+            "Get the user specified checksum")
+
+        .def("set_checksum", &PyGfal2::GfaltParams::set_checksum,
+            "Specify the checksum mode, type and value")
+        .def("get_checksum", &PyGfal2::GfaltParams::get_checksum,
+            "Get the user specified checksum mode, type and value")
+        ;
 
     boost::python::scope().attr("transfer_parameters") = boost::python::scope().attr("TransferParameters");
 
     // Callback types
     boost::python::enum_<gfal_event_side_t>("event_side")
         .value("event_source", GFAL_EVENT_SOURCE)
         .value("event_destination", GFAL_EVENT_DESTINATION)
@@ -373,8 +388,33 @@
         ("DirectoryType", "Directory descriptor", boost::python::init<PyGfal2::Gfal2Context, const std::string &>())
         .def("read", &PyGfal2::Directory::read,
             "Reads a directory entry from the directory")
         .def("readpp", &PyGfal2::Directory::readpp,
             "Reads a directory entry and its stat information");
 
     register_shared_ptr<PyGfal2::Directory>();
+
+    // Null log handler
+    boost::python::class_<PyGfal2::NullHandler> nullHandler("NullHandler");
+    nullHandler.def("emit", &PyGfal2::NullHandler::emit)
+        .def("createLock", &PyGfal2::NullHandler::createLock)
+        .def("acquire", &PyGfal2::NullHandler::acquire)
+        .def("release", &PyGfal2::NullHandler::release)
+        .def("setLevel", &PyGfal2::NullHandler::setLevel)
+        .def("setFormatter", &PyGfal2::NullHandler::setFormatter)
+        .def("addFilter", &PyGfal2::NullHandler::addFilter)
+        .def("removeFilter", &PyGfal2::NullHandler::removeFilter)
+        .def("filter", &PyGfal2::NullHandler::filter)
+        .def("flush", &PyGfal2::NullHandler::flush)
+        .def("close", &PyGfal2::NullHandler::close)
+        .def("handle", &PyGfal2::NullHandler::handle)
+        .def("handleError", &PyGfal2::NullHandler::handleError)
+        .def("format", &PyGfal2::NullHandler::format)
+        .def("emit", &PyGfal2::NullHandler::emit)
+        .add_property("level", &PyGfal2::NullHandler::level)
+        .add_property("filters", &PyGfal2::NullHandler::filters);
+
+    gfal2Scope.attr("NullHandler") = nullHandler;
+
+    // Register the null handler for gfal2 by default
+    PyGfal2::logging_register_handler("gfal2", boost::python::object(nullHandler)());
 }
```

### Comparing `gfal2-python-1.8.5.post2/src/pyGIL.h` & `gfal2-python-1.9.2.post3/src/pyGIL.h`

 * *Files identical despite different names*

### Comparing `gfal2-python-1.8.5.post2/CMakeLists.txt` & `gfal2-python-1.9.2.post3/CMakeLists.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,31 +17,49 @@
 set(Boost_NO_BOOST_CMAKE ON)
 
 find_package(Boost COMPONENTS python REQUIRED)
 find_package(PythonEasy REQUIRED)
 
 message("Python: ${PYTHON_EXECUTABLE}")
 
+if (PYTHON_EXECUTABLE_3)
+    message("Python 3 installed! ${PYTHON3_CURRENT_VERSION}")
+    message("Python 3: ${PYTHON_EXECUTABLE_3}")
+
+    string(REPLACE "." "" Boost_PYTHON_3_SUFFIX "${PYTHON3_CURRENT_VERSION}")
+
+    find_library(Boost_PYTHON_3_LIBRARY
+        NAMES boost_python3 boost_python-py${Boost_PYTHON_3_SUFFIX}
+        HINTS
+            ${Boost_LIBRARYDIR}
+            "/usr/lib"
+            "/usr/lib64"
+    )
+    if (Boost_PYTHON_3_LIBRARY)
+        message("Boost Python3 library found! ${Boost_PYTHON_3_LIBRARY}")
+    else()
+        message("Boost Python3 library not found")
+    endif ()
+endif ()
+
 #define PROJECT vars
 set(PROJECT_NAME_MAIN "gfal2-python")
-set(OUTPUT_NAME_MAIN "gfal2")
-
 
 # EPYDOC definition for EPEL5 support
 if (NOT SKIP_DOC)
-    set(EPYDOC_MODULE_PATH "${CMAKE_BINARY_DIR}/src/gfal2.so")
+    set(EPYDOC_MODULE_PATH "${CMAKE_BINARY_DIR}/src/python2/gfal2.so")
     set(EPYDOC_MODULE_URL  "http://dmc.web.cern.ch/projects/gfal2-python")
     set(EPYDOC_MODULE_NAME "gfal2")
 
     include(MacroAddepydoc REQUIRED)
 endif (NOT SKIP_DOC)
 
 set(VERSION_MAJOR 1)
-set(VERSION_MINOR 8)
-set(VERSION_PATCH 5)
+set(VERSION_MINOR 9)
+set(VERSION_PATCH 2)
 set(VERSION_STRING ${VERSION_MAJOR}.${VERSION_MINOR}.${VERSION_PATCH})
 add_definitions(-DGFAL2_PYTHON_VERSION="${VERSION_STRING}")
 
 # libs checks
 find_package (GLIB2 REQUIRED)
 find_package (GTHREAD2 REQUIRED)
```

### Comparing `gfal2-python-1.8.5.post2/setup.py` & `gfal2-python-1.9.2.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import distutils.command.build_ext as _build_ext
 import distutils.spawn
 import distutils.dir_util
 from glob import glob
 from setuptools import Extension, setup
 
 # Change this when there are changes in the setup.py or MANIFEST.in
-RELEASE = 2
+RELEASE = 3
 
 
 def get_version():
     ver_components = dict(VERSION_RELEASE=RELEASE)
     with open('CMakeLists.txt') as cmake:
         for line in cmake:
             line = line.strip()
@@ -42,15 +42,15 @@
     if len(ver_components) == 0:
         raise ValueError('Could not find the version')
     return "%(VERSION_MAJOR)s.%(VERSION_MINOR)s.%(VERSION_PATCH)s.post%(VERSION_RELEASE)s" % ver_components
 
 
 def validate():
     if distutils.spawn.find_executable('cmake') is None:
-        print 'Missing CMake executable'
+        print('Missing CMake executable')
         sys.exit(-1)
 
 
 def _run_make(build_dir, lib_path):
     validate()
 
     pwd = os.getcwd()
@@ -63,15 +63,15 @@
 
     try:
         distutils.spawn.spawn([
             'cmake', '-DSKIP_DOC=TRUE', '-DSKIP_TESTS=TRUE',
             source_dir
         ])
         distutils.spawn.spawn(['make'])
-        shutil.copy('src/gfal2.so', full_lib_path)
+        shutil.copy('src/python%d/gfal2.so' % sys.version_info[0], full_lib_path)
     finally:
         os.chdir(pwd)
 
 
 class build_ext(_build_ext.build_ext):
     def run(self):
         _run_make(self.build_temp, self.get_ext_fullpath('gfal2'))
```

### Comparing `gfal2-python-1.8.5.post2/PKG-INFO` & `gfal2-python-1.9.2.post3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gfal2-python
-Version: 1.8.5.post2
+Version: 1.9.2.post3
 Summary: Python bindings for gfal2
 Home-page: https://dmc.web.cern.ch/
 Author: DMC Devel
 Author-email: dmc-devel@cern.ch
 License: Apache 2
 Download-URL: https://gitlab.cern.ch/dmc/gfal2-bindings
 Description: Python bindings for gfal2
```

