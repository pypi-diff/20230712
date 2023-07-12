# Comparing `tmp/clp_ffi_py-0.0.0b0.tar.gz` & `tmp/clp_ffi_py-0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clp_ffi_py-0.0.0b0.tar", last modified: Thu Jul  6 04:00:54 2023, max compression
+gzip compressed data, was "clp_ffi_py-0.0.0b1.tar", last modified: Wed Jul 12 04:55:19 2023, max compression
```

## Comparing `clp_ffi_py-0.0.0b0.tar` & `clp_ffi_py-0.0.0b1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.190492 clp_ffi_py-0.0.0b0/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      853 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/.clang-format
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1402 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/.clang-tidy
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.138491 clp_ffi_py-0.0.0b0/.github/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.138491 clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1113 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       27 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      557 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      283 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.138491 clp_ffi_py-0.0.0b0/.github/workflows/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      758 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/.github/workflows/build_wheels.yml
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      122 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/.gitignore
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       80 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b0/.gitmodules
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    11356 2023-06-14 03:19:32.000000 clp_ffi_py-0.0.0b0/LICENSE
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      296 2023-06-14 03:44:48.000000 clp_ffi_py-0.0.0b0/MANIFEST.in
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4278 2023-07-06 04:00:54.190492 clp_ffi_py-0.0.0b0/PKG-INFO
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3795 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/README.md
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.142491 clp_ffi_py-0.0.0b0/clp_ffi_py/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      303 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/CLPFourByteEncoder.pyi
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      930 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/CLPIRDecoder.pyi
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2765 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/FileReader.py
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/__init__.py
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/py.typed
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1079 2023-07-02 19:45:23.000000 clp_ffi_py-0.0.0b0/clp_ffi_py/utils.py
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.142491 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4278 2023-07-06 04:00:54.000000 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/PKG-INFO
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8478 2023-07-06 04:00:54.000000 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/SOURCES.txt
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)        1 2023-07-06 04:00:54.000000 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/dependency_links.txt
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       66 2023-07-06 04:00:54.000000 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/requires.txt
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       11 2023-07-06 04:00:54.000000 clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/top_level.txt
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      945 2023-07-06 04:00:41.000000 clp_ffi_py-0.0.0b0/pyproject.toml
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      166 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/requirements-dev.txt
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       38 2023-07-06 04:00:54.190492 clp_ffi_py-0.0.0b0/setup.cfg
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2752 2023-07-06 03:50:51.000000 clp_ffi_py-0.0.0b0/setup.py
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.130491 clp_ffi_py-0.0.0b0/src/clp/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.130491 clp_ffi_py-0.0.0b0/src/clp/components/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/clp/components/core/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.158492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5498 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ArrayBackedPosIntSet.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      914 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/CommandLineArgumentsBase.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1025 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryEntry.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8995 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9605 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryWriter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5003 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/EncodedVariableInterpreter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      613 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ErrorCode.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3611 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/FileReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2681 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/FileWriter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2463 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMetadataDB.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1506 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMetadataDBConfig.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3405 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMySQLMetadataDB.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3184 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalSQLiteMetadataDB.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4847 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Grep.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3297 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/LibarchiveFileReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5050 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/LibarchiveReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5344 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/LogTypeDictionaryEntry.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      423 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/LogTypeDictionaryReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1203 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/LogTypeDictionaryWriter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2112 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/MessageParser.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3173 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLDB.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1427 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLParamBindings.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1657 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLPreparedStatement.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8341 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/PageAllocatedVector.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1764 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ParsedMessage.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1752 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Platform.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6593 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Profiler.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     7759 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Query.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5235 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ReaderInterface.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1222 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/SQLiteDB.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2338 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/SQLitePreparedStatement.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      474 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Stopwatch.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2960 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/StringReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1511 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Thread.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5288 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/TimestampPattern.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       34 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/TraceableException.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1148 2023-06-03 03:52:34.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/TraceableException.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3517 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Utils.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2247 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/VariableDictionaryEntry.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      432 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/VariableDictionaryReader.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1095 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/VariableDictionaryWriter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1476 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/Writer.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2044 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/WriterInterface.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.158492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clg/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2130 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clg/CommandLineArguments.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.158492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clo/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1842 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clo/CommandLineArguments.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      780 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clo/ControllerMonitoringThread.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.162492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3152 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/CommandLineArguments.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4115 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileCompressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1193 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileDecompressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      935 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileToCompress.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      918 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/StructuredFileToCompress.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1605 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/compression.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      568 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/decompression.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      126 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/run.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3632 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/utils.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.162492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1303 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Constants.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13827 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LALR1Parser.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    32949 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LALR1Parser.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6708 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Lexer.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    24628 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Lexer.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2496 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LogParser.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3627 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/SchemaParser.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1718 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Token.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.166492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    15948 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    10255 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2433 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1438 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4122 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8484 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5239 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8505 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      608 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/utils.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2239 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/database_utils.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      782 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/dictionary_utils.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.166492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3955 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13102 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    24981 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.tpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.170492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      323 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/byteswap.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    21845 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/decoding_methods.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5894 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/decoding_methods.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    12961 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/encoding_methods.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3080 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/encoding_methods.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2127 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/protocol_constants.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.170492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3645 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/CompositeWildcardToken.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1929 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/ExactVariableToken.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      805 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryMethodFailed.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1553 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryToken.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2512 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryWildcard.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1905 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/Subquery.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3281 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/WildcardToken.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1559 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/fmtlib_specializations.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      584 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/query_methods.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.174492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/networking/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      656 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/networking/SocketOperationFailed.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1542 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/networking/socket_utils.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.174492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2467 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/Constants.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5475 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/MetadataDB.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.174492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5228 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Archive.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5376 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/File.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1042 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Message.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2329 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Segment.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1733 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/SegmentManager.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.174492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13234 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/Archive.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8361 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/File.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3011 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/Segment.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.174492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1883 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/Compressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      324 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/Constants.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2217 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/Decompressor.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.178492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/passthrough/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2389 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/passthrough/Compressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4064 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/passthrough/Decompressor.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.178492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2908 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/Compressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      310 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/Constants.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5363 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/Decompressor.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9576 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/string_utils.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3995 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/string_utils.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      446 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/string_utils.tpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1989 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/type_utils.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/clp/components/core/src/utils/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.178492 clp_ffi_py-0.0.0b0/src/clp/components/core/src/utils/make_dictionaries_readable/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      986 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/utils/make_dictionaries_readable/CommandLineArguments.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)       99 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/src/version.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/json/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.134491 clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/json/single_include/
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.178492 clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/json/single_include/nlohmann/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)   914657 2023-06-01 22:18:57.000000 clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/json/single_include/nlohmann/json.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.182492 clp_ffi_py-0.0.0b0/src/clp_ffi_py/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1758 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/ErrorMessage.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      653 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/ExceptionFFI.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      395 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/PyObjectDeleter.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1594 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/Py_utils.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      338 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/Py_utils.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      346 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/Python.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.186493 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Message.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2777 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Message.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2250 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Metadata.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1299 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Metadata.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6068 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyDecoderBuffer.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1158 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyDecoderBuffer.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13262 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMessage.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1201 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMessage.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6076 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMetadata.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      708 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMetadata.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    10717 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyQuery.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      461 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyQuery.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      570 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Query.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2663 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Query.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9671 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/decoding_methods.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      524 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/decoding_methods.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.186493 clp_ffi_py-0.0.0b0/src/clp_ffi_py/encoder/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4981 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/encoder/encoding_methods.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      572 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/encoder/encoding_methods.hpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.186493 clp_ffi_py-0.0.0b0/src/clp_ffi_py/modules/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3997 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/modules/clp_four_byte_encoder.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2425 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/modules/clp_ir_decoder.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2458 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.cpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1052 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.hpp
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)      960 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.tpp
-drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-06 04:00:54.186493 clp_ffi_py-0.0.0b0/tests/
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)    11209 2023-07-06 03:47:46.000000 clp_ffi_py-0.0.0b0/tests/TestCase.py
--rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1174 2023-07-03 02:57:46.000000 clp_ffi_py-0.0.0b0/tests/__init__.py
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      853 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/.clang-format
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1402 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/.clang-tidy
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.146940 clp_ffi_py-0.0.0b1/.github/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.146940 clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1113 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       27 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      557 2023-06-14 03:44:36.000000 clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      283 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.146940 clp_ffi_py-0.0.0b1/.github/workflows/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      758 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/.github/workflows/build_wheels.yml
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      122 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/.gitignore
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       80 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/.gitmodules
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    11356 2023-06-14 03:19:32.000000 clp_ffi_py-0.0.0b1/LICENSE
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      296 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/MANIFEST.in
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4278 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/PKG-INFO
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3795 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/README.md
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.146940 clp_ffi_py-0.0.0b1/clp_ffi_py/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      303 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/CLPFourByteEncoder.pyi
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      930 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/CLPIRDecoder.pyi
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2765 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/FileReader.py
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/__init__.py
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-06-14 03:05:42.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/py.typed
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1079 2023-07-02 19:45:23.000000 clp_ffi_py-0.0.0b1/clp_ffi_py/utils.py
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.150940 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4278 2023-07-12 04:55:19.000000 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/PKG-INFO
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8478 2023-07-12 04:55:19.000000 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/SOURCES.txt
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)        1 2023-07-12 04:55:19.000000 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/dependency_links.txt
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       66 2023-07-12 04:55:19.000000 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/requires.txt
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       11 2023-07-12 04:55:19.000000 clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/top_level.txt
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      945 2023-07-12 04:54:44.000000 clp_ffi_py-0.0.0b1/pyproject.toml
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      166 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/requirements-dev.txt
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       38 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/setup.cfg
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2752 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/setup.py
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.138940 clp_ffi_py-0.0.0b1/src/clp/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.138940 clp_ffi_py-0.0.0b1/src/clp/components/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/clp/components/core/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.158940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5498 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ArrayBackedPosIntSet.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      914 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/CommandLineArgumentsBase.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1025 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryEntry.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8995 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9605 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryWriter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5003 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/EncodedVariableInterpreter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      613 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ErrorCode.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3611 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/FileReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2681 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/FileWriter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2463 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMetadataDB.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1506 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMetadataDBConfig.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3405 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMySQLMetadataDB.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3184 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalSQLiteMetadataDB.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4847 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Grep.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3297 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/LibarchiveFileReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5050 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/LibarchiveReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5344 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/LogTypeDictionaryEntry.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      423 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/LogTypeDictionaryReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1203 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/LogTypeDictionaryWriter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2112 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/MessageParser.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3173 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLDB.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1427 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLParamBindings.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1657 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLPreparedStatement.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8341 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/PageAllocatedVector.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1764 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ParsedMessage.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1752 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Platform.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6593 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Profiler.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     7759 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Query.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5235 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ReaderInterface.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1222 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/SQLiteDB.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2338 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/SQLitePreparedStatement.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      474 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Stopwatch.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2960 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/StringReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1511 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Thread.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5288 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/TimestampPattern.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       34 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/TraceableException.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1148 2023-06-03 03:52:34.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/TraceableException.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3517 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Utils.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2247 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/VariableDictionaryEntry.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      432 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/VariableDictionaryReader.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1095 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/VariableDictionaryWriter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1476 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/Writer.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2044 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/WriterInterface.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.158940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clg/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2130 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clg/CommandLineArguments.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.158940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clo/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1842 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clo/CommandLineArguments.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      780 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clo/ControllerMonitoringThread.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.162940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3152 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/CommandLineArguments.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4115 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileCompressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1193 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileDecompressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      935 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileToCompress.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      918 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/StructuredFileToCompress.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1605 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/compression.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      568 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/decompression.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      126 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/run.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3632 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/utils.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.162940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1303 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Constants.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13827 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LALR1Parser.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    32949 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LALR1Parser.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6708 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Lexer.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    24628 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Lexer.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2496 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LogParser.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3627 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/SchemaParser.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1718 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Token.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.162940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    15948 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    10255 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2433 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1438 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4122 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8484 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5239 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8505 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      608 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/utils.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2239 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/database_utils.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      782 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/dictionary_utils.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.162940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3955 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13102 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    24981 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.tpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.166940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      323 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/byteswap.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    21845 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/decoding_methods.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5894 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/decoding_methods.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    12961 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/encoding_methods.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3080 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/encoding_methods.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2127 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/protocol_constants.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.166940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3645 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/CompositeWildcardToken.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1929 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/ExactVariableToken.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      805 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryMethodFailed.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1553 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryToken.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2512 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryWildcard.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1905 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/Subquery.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3281 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/WildcardToken.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1559 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/fmtlib_specializations.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      584 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/query_methods.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.166940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/networking/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      656 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/networking/SocketOperationFailed.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1542 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/networking/socket_utils.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.166940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2467 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/Constants.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5475 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/MetadataDB.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5228 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Archive.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5376 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/File.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1042 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Message.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2329 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Segment.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1733 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/SegmentManager.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13234 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/Archive.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     8361 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/File.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3011 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/Segment.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1883 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/Compressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      324 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/Constants.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2217 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/Decompressor.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/passthrough/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2389 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/passthrough/Compressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4064 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/passthrough/Decompressor.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2908 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/Compressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      310 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/Constants.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     5363 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/Decompressor.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9576 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/string_utils.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3995 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/string_utils.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      446 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/string_utils.tpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1989 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/type_utils.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/utils/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/src/utils/make_dictionaries_readable/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      986 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/utils/make_dictionaries_readable/CommandLineArguments.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)       99 2023-05-24 22:29:59.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/src/version.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/json/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.142940 clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/json/single_include/
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.170940 clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/json/single_include/nlohmann/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)   914657 2023-06-01 22:18:57.000000 clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/json/single_include/nlohmann/json.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.174940 clp_ffi_py-0.0.0b1/src/clp_ffi_py/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1758 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/ErrorMessage.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      653 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/ExceptionFFI.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      395 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/PyObjectDeleter.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1594 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/Py_utils.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      338 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/Py_utils.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      346 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/Python.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Message.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2777 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Message.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2250 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Metadata.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1299 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Metadata.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6068 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyDecoderBuffer.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1158 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyDecoderBuffer.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    13262 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMessage.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1201 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMessage.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     6076 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMetadata.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      708 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMetadata.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    10717 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyQuery.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      461 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyQuery.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      570 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Query.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2663 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Query.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     9671 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/decoding_methods.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      524 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/decoding_methods.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/src/clp_ffi_py/encoder/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     4981 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/encoder/encoding_methods.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      572 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/encoder/encoding_methods.hpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/src/clp_ffi_py/modules/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     3997 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/modules/clp_four_byte_encoder.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2425 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/modules/clp_ir_decoder.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     2458 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.cpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1052 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.hpp
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)      960 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.tpp
+drwxr-xr-x   0 lzh      (1000046) lzh      (1000000)        0 2023-07-12 04:55:19.178941 clp_ffi_py-0.0.0b1/tests/
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)    11209 2023-07-12 04:39:07.000000 clp_ffi_py-0.0.0b1/tests/TestCase.py
+-rw-r--r--   0 lzh      (1000046) lzh      (1000000)     1174 2023-07-03 02:57:46.000000 clp_ffi_py-0.0.0b1/tests/__init__.py
```

### Comparing `clp_ffi_py-0.0.0b0/.clang-format` & `clp_ffi_py-0.0.0b1/.clang-format`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/.clang-tidy` & `clp_ffi_py-0.0.0b1/.clang-tidy`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/bug-report.yml` & `clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/.github/ISSUE_TEMPLATE/feature-request.yml` & `clp_ffi_py-0.0.0b1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/.github/workflows/build_wheels.yml` & `clp_ffi_py-0.0.0b1/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/LICENSE` & `clp_ffi_py-0.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/PKG-INFO` & `clp_ffi_py-0.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clp_ffi_py
-Version: 0.0.0b0
+Version: 0.0.0b1
 Summary: Python interface to the CLP Core Features through CLP's FFI
 Author-email: zhihao lin <lin.zhihao@yscope.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/y-scope/clp-ffi-py
 Project-URL: Bug Tracker, https://github.com/y-scope/clp-ffi-py/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
```

### Comparing `clp_ffi_py-0.0.0b0/README.md` & `clp_ffi_py-0.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/clp_ffi_py/CLPIRDecoder.pyi` & `clp_ffi_py-0.0.0b1/clp_ffi_py/CLPIRDecoder.pyi`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/clp_ffi_py/FileReader.py` & `clp_ffi_py-0.0.0b1/clp_ffi_py/FileReader.py`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/clp_ffi_py/utils.py` & `clp_ffi_py-0.0.0b1/clp_ffi_py/utils.py`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/PKG-INFO` & `clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clp-ffi-py
-Version: 0.0.0b0
+Version: 0.0.0b1
 Summary: Python interface to the CLP Core Features through CLP's FFI
 Author-email: zhihao lin <lin.zhihao@yscope.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/y-scope/clp-ffi-py
 Project-URL: Bug Tracker, https://github.com/y-scope/clp-ffi-py/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
```

### Comparing `clp_ffi_py-0.0.0b0/clp_ffi_py.egg-info/SOURCES.txt` & `clp_ffi_py-0.0.0b1/clp_ffi_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/pyproject.toml` & `clp_ffi_py-0.0.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools >= 59.0", "setuptools_scm", "wheel"]
+requires = ["setuptools >= 57.0", "setuptools_scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clp_ffi_py"
-version = "0.0.0.beta.0"
+version = "0.0.0.beta.1"
 license = { text = "Apache License 2.0" }
 authors = [
     { name="zhihao lin", email="lin.zhihao@yscope.com" },
 ]
 description = "Python interface to the CLP Core Features through CLP's FFI"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `clp_ffi_py-0.0.0b0/setup.py` & `clp_ffi_py-0.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ArrayBackedPosIntSet.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ArrayBackedPosIntSet.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/CommandLineArgumentsBase.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/CommandLineArgumentsBase.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryEntry.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryEntry.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryReader.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryReader.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/DictionaryWriter.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/DictionaryWriter.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/EncodedVariableInterpreter.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/EncodedVariableInterpreter.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ErrorCode.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ErrorCode.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/FileReader.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/FileReader.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/FileWriter.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/FileWriter.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMetadataDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMetadataDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMetadataDBConfig.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMetadataDBConfig.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalMySQLMetadataDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalMySQLMetadataDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/GlobalSQLiteMetadataDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/GlobalSQLiteMetadataDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Grep.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Grep.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/LibarchiveFileReader.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/LibarchiveFileReader.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/LibarchiveReader.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/LibarchiveReader.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/LogTypeDictionaryEntry.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/LogTypeDictionaryEntry.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/LogTypeDictionaryWriter.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/LogTypeDictionaryWriter.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/MessageParser.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/MessageParser.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLParamBindings.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLParamBindings.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/MySQLPreparedStatement.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/MySQLPreparedStatement.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/PageAllocatedVector.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/PageAllocatedVector.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ParsedMessage.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ParsedMessage.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Platform.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Platform.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Profiler.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Profiler.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Query.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Query.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ReaderInterface.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ReaderInterface.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/SQLiteDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/SQLiteDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/SQLitePreparedStatement.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/SQLitePreparedStatement.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/StringReader.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/StringReader.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Thread.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Thread.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/TimestampPattern.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/TimestampPattern.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/TraceableException.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/TraceableException.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/VariableDictionaryEntry.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/VariableDictionaryEntry.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/VariableDictionaryWriter.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/VariableDictionaryWriter.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/Writer.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/Writer.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/WriterInterface.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/WriterInterface.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clg/CommandLineArguments.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clg/CommandLineArguments.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clo/CommandLineArguments.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clo/CommandLineArguments.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clo/ControllerMonitoringThread.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clo/ControllerMonitoringThread.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/CommandLineArguments.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/CommandLineArguments.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileCompressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileCompressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileDecompressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileDecompressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/FileToCompress.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/FileToCompress.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/StructuredFileToCompress.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/StructuredFileToCompress.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/compression.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/compression.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/decompression.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/decompression.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/clp/utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/clp/utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Constants.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Constants.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LALR1Parser.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LALR1Parser.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LALR1Parser.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LALR1Parser.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Lexer.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Lexer.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Lexer.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Lexer.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/LogParser.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/LogParser.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/SchemaParser.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/SchemaParser.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/Token.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/Token.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexAST.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexDFA.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/RegexNFA.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/finite_automata/UnicodeIntervalTree.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/compressor_frontend/utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/compressor_frontend/utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/database_utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/database_utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/dictionary_utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/dictionary_utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.cpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/encoding_methods.tpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/encoding_methods.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/decoding_methods.cpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/decoding_methods.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/decoding_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/decoding_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/encoding_methods.cpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/encoding_methods.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/encoding_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/encoding_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/ir_stream/protocol_constants.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/ir_stream/protocol_constants.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/CompositeWildcardToken.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/CompositeWildcardToken.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/ExactVariableToken.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/ExactVariableToken.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryMethodFailed.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryMethodFailed.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryToken.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryToken.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/QueryWildcard.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/QueryWildcard.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/Subquery.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/Subquery.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/WildcardToken.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/WildcardToken.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/fmtlib_specializations.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/fmtlib_specializations.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/ffi/search/query_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/ffi/search/query_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/networking/SocketOperationFailed.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/networking/SocketOperationFailed.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/networking/socket_utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/networking/socket_utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/Constants.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/Constants.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/MetadataDB.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/MetadataDB.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Archive.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Archive.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/File.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/File.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Message.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Message.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/Segment.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/Segment.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/reader/SegmentManager.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/reader/SegmentManager.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/Archive.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/Archive.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/File.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/File.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_archive/writer/Segment.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_archive/writer/Segment.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/Compressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/Compressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/Decompressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/Decompressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/passthrough/Compressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/passthrough/Compressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/passthrough/Decompressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/passthrough/Decompressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/Compressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/Compressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/streaming_compression/zstd/Decompressor.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/streaming_compression/zstd/Decompressor.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/string_utils.cpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/string_utils.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/string_utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/string_utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/type_utils.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/type_utils.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/src/utils/make_dictionaries_readable/CommandLineArguments.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/src/utils/make_dictionaries_readable/CommandLineArguments.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp/components/core/submodules/json/single_include/nlohmann/json.hpp` & `clp_ffi_py-0.0.0b1/src/clp/components/core/submodules/json/single_include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/ErrorMessage.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/ErrorMessage.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/ExceptionFFI.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/ExceptionFFI.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/Py_utils.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/Py_utils.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Message.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Message.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Metadata.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Metadata.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Metadata.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Metadata.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyDecoderBuffer.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyDecoderBuffer.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyDecoderBuffer.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyDecoderBuffer.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMessage.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMessage.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMessage.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMessage.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMetadata.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMetadata.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyMetadata.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyMetadata.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/PyQuery.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/PyQuery.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Query.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Query.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/Query.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/Query.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/decoding_methods.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/decoding_methods.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/decoder/decoding_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/decoder/decoding_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/encoder/encoding_methods.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/encoder/encoding_methods.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/encoder/encoding_methods.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/encoder/encoding_methods.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/modules/clp_four_byte_encoder.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/modules/clp_four_byte_encoder.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/modules/clp_ir_decoder.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/modules/clp_ir_decoder.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.cpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.cpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.hpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.hpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/src/clp_ffi_py/utilities.tpp` & `clp_ffi_py-0.0.0b1/src/clp_ffi_py/utilities.tpp`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/tests/TestCase.py` & `clp_ffi_py-0.0.0b1/tests/TestCase.py`

 * *Files identical despite different names*

### Comparing `clp_ffi_py-0.0.0b0/tests/__init__.py` & `clp_ffi_py-0.0.0b1/tests/__init__.py`

 * *Files identical despite different names*

