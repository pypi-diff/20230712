# Comparing `tmp/unogenerator-0.8.0.tar.gz` & `tmp/unogenerator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unogenerator-0.8.0.tar", last modified: Mon Oct 18 15:56:33 2021, max compression
+gzip compressed data, was "unogenerator-0.9.0.tar", last modified: Thu Oct 28 20:12:51 2021, max compression
```

## Comparing `unogenerator-0.8.0.tar` & `unogenerator-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.487403 unogenerator-0.8.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2021-09-16 16:04:16.000000 unogenerator-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      267 2021-10-03 15:33:40.000000 unogenerator-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      713 2021-10-18 15:56:33.487403 unogenerator-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3529 2021-10-11 04:56:56.000000 unogenerator-0.8.0/PROBLEMS.md
--rw-r--r--   0 root         (0) root         (0)     3606 2021-10-18 15:45:20.000000 unogenerator-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.484403 unogenerator-0.8.0/doc/
--rw-r--r--   0 root         (0) root         (0)   106603 2021-10-18 15:48:07.000000 unogenerator-0.8.0/doc/Doxyfile
--rw-r--r--   0 root         (0) root         (0)      471 2021-10-03 15:23:41.000000 unogenerator-0.8.0/doc/index.dox
--rw-r--r--   0 root         (0) root         (0)    21000 2021-10-03 15:31:20.000000 unogenerator-0.8.0/doc/unogenerator_doxygen.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.484403 unogenerator-0.8.0/locale/
--rw-r--r--   0 root         (0) root         (0)      738 2021-10-04 03:30:11.000000 unogenerator-0.8.0/locale/en.po
--rw-r--r--   0 root         (0) root         (0)    15539 2021-10-18 15:47:08.000000 unogenerator-0.8.0/locale/es.po
--rw-r--r--   0 root         (0) root         (0)     6843 2021-10-18 15:47:11.000000 unogenerator-0.8.0/locale/unogenerator.pot
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-18 15:56:33.487403 unogenerator-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6808 2021-10-04 03:27:27.000000 unogenerator-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.485403 unogenerator-0.8.0/unogenerator/
--rw-r--r--   0 root         (0) root         (0)      211 2021-10-04 03:12:59.000000 unogenerator-0.8.0/unogenerator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15197 2021-10-18 15:42:54.000000 unogenerator-0.8.0/unogenerator/commons.py
--rw-r--r--   0 root         (0) root         (0)    20465 2021-10-18 15:50:23.000000 unogenerator-0.8.0/unogenerator/demo.py
--rw-r--r--   0 root         (0) root         (0)     9774 2021-10-07 02:03:00.000000 unogenerator-0.8.0/unogenerator/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.486403 unogenerator-0.8.0/unogenerator/images/
--rw-r--r--   0 root         (0) root         (0)     8836 2021-09-17 12:13:28.000000 unogenerator-0.8.0/unogenerator/images/crown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.483403 unogenerator-0.8.0/unogenerator/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.483403 unogenerator-0.8.0/unogenerator/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.486403 unogenerator-0.8.0/unogenerator/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      424 2021-10-18 15:47:11.000000 unogenerator-0.8.0/unogenerator/locale/en/LC_MESSAGES/unogenerator.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.483403 unogenerator-0.8.0/unogenerator/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.486403 unogenerator-0.8.0/unogenerator/locale/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4425 2021-10-18 15:47:11.000000 unogenerator-0.8.0/unogenerator/locale/es/LC_MESSAGES/unogenerator.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.487403 unogenerator-0.8.0/unogenerator/reusing/
--rw-r--r--   0 root         (0) root         (0)       76 2021-09-18 17:14:27.000000 unogenerator-0.8.0/unogenerator/reusing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9136 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/casts.py
--rw-r--r--   0 root         (0) root         (0)     5191 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/currency.py
--rw-r--r--   0 root         (0) root         (0)    17302 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/datetime_functions.py
--rw-r--r--   0 root         (0) root         (0)     3178 2021-10-07 16:56:36.000000 unogenerator-0.8.0/unogenerator/reusing/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2588 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/github.py
--rw-r--r--   0 root         (0) root         (0)    24834 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/libmanagers.py
--rw-r--r--   0 root         (0) root         (0)     3414 2021-09-17 14:28:32.000000 unogenerator-0.8.0/unogenerator/reusing/percentage.py
--rw-r--r--   0 root         (0) root         (0)     2752 2021-10-07 18:01:23.000000 unogenerator-0.8.0/unogenerator/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.487403 unogenerator-0.8.0/unogenerator/templates/
--rw-r--r--   0 root         (0) root         (0)     8395 2021-10-02 09:46:12.000000 unogenerator-0.8.0/unogenerator/templates/standard.ods
--rw-r--r--   0 root         (0) root         (0)    25897 2021-10-13 05:27:55.000000 unogenerator-0.8.0/unogenerator/templates/standard.odt
--rw-r--r--   0 root         (0) root         (0)    30897 2021-10-13 05:11:06.000000 unogenerator-0.8.0/unogenerator/unogenerator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-18 15:56:33.486403 unogenerator-0.8.0/unogenerator.egg-info/
--rw-r--r--   0 root         (0) root         (0)      713 2021-10-18 15:56:33.000000 unogenerator-0.8.0/unogenerator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1017 2021-10-18 15:56:33.000000 unogenerator-0.8.0/unogenerator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-18 15:56:33.000000 unogenerator-0.8.0/unogenerator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      233 2021-10-18 15:56:33.000000 unogenerator-0.8.0/unogenerator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-17 12:14:43.000000 unogenerator-0.8.0/unogenerator.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       13 2021-10-18 15:56:33.000000 unogenerator-0.8.0/unogenerator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3054 2021-10-02 05:53:06.000000 unogenerator-0.8.0/unogenerator.epj
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.701847 unogenerator-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2021-09-16 16:04:16.000000 unogenerator-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      267 2021-10-03 15:33:40.000000 unogenerator-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      713 2021-10-28 20:12:51.701847 unogenerator-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3529 2021-10-11 04:56:56.000000 unogenerator-0.9.0/PROBLEMS.md
+-rw-r--r--   0 root         (0) root         (0)     3774 2021-10-28 20:10:16.000000 unogenerator-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.698847 unogenerator-0.9.0/doc/
+-rw-r--r--   0 root         (0) root         (0)   106603 2021-10-28 20:10:56.000000 unogenerator-0.9.0/doc/Doxyfile
+-rw-r--r--   0 root         (0) root         (0)      471 2021-10-03 15:23:41.000000 unogenerator-0.9.0/doc/index.dox
+-rw-r--r--   0 root         (0) root         (0)    21000 2021-10-03 15:31:20.000000 unogenerator-0.9.0/doc/unogenerator_doxygen.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.698847 unogenerator-0.9.0/locale/
+-rw-r--r--   0 root         (0) root         (0)      738 2021-10-04 03:30:11.000000 unogenerator-0.9.0/locale/en.po
+-rw-r--r--   0 root         (0) root         (0)    16196 2021-10-28 20:10:22.000000 unogenerator-0.9.0/locale/es.po
+-rw-r--r--   0 root         (0) root         (0)     7459 2021-10-28 20:10:22.000000 unogenerator-0.9.0/locale/unogenerator.pot
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-28 20:12:51.701847 unogenerator-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7022 2021-10-28 18:56:48.000000 unogenerator-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.698847 unogenerator-0.9.0/unogenerator/
+-rw-r--r--   0 root         (0) root         (0)      211 2021-10-04 03:12:59.000000 unogenerator-0.9.0/unogenerator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15841 2021-10-28 20:08:33.000000 unogenerator-0.9.0/unogenerator/commons.py
+-rw-r--r--   0 root         (0) root         (0)    20465 2021-10-18 15:50:23.000000 unogenerator-0.9.0/unogenerator/demo.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2021-10-07 02:03:00.000000 unogenerator-0.9.0/unogenerator/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.699847 unogenerator-0.9.0/unogenerator/images/
+-rw-r--r--   0 root         (0) root         (0)     8836 2021-09-17 12:13:28.000000 unogenerator-0.9.0/unogenerator/images/crown.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.696847 unogenerator-0.9.0/unogenerator/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.696847 unogenerator-0.9.0/unogenerator/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.699847 unogenerator-0.9.0/unogenerator/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      424 2021-10-28 20:10:22.000000 unogenerator-0.9.0/unogenerator/locale/en/LC_MESSAGES/unogenerator.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.696847 unogenerator-0.9.0/unogenerator/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.699847 unogenerator-0.9.0/unogenerator/locale/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4379 2021-10-28 20:10:22.000000 unogenerator-0.9.0/unogenerator/locale/es/LC_MESSAGES/unogenerator.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.700847 unogenerator-0.9.0/unogenerator/reusing/
+-rw-r--r--   0 root         (0) root         (0)       76 2021-09-18 17:14:27.000000 unogenerator-0.9.0/unogenerator/reusing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9138 2021-10-28 05:19:45.000000 unogenerator-0.9.0/unogenerator/reusing/casts.py
+-rw-r--r--   0 root         (0) root         (0)     5191 2021-09-17 14:28:32.000000 unogenerator-0.9.0/unogenerator/reusing/currency.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2021-09-17 14:28:32.000000 unogenerator-0.9.0/unogenerator/reusing/datetime_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2021-10-07 16:56:36.000000 unogenerator-0.9.0/unogenerator/reusing/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2021-09-17 14:28:32.000000 unogenerator-0.9.0/unogenerator/reusing/github.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2021-09-17 14:28:32.000000 unogenerator-0.9.0/unogenerator/reusing/libmanagers.py
+-rw-r--r--   0 root         (0) root         (0)     6635 2021-10-28 05:18:35.000000 unogenerator-0.9.0/unogenerator/reusing/listdict_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2021-09-17 14:28:32.000000 unogenerator-0.9.0/unogenerator/reusing/percentage.py
+-rw-r--r--   0 root         (0) root         (0)     5857 2021-10-28 20:06:16.000000 unogenerator-0.9.0/unogenerator/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.700847 unogenerator-0.9.0/unogenerator/templates/
+-rw-r--r--   0 root         (0) root         (0)     8395 2021-10-02 09:46:12.000000 unogenerator-0.9.0/unogenerator/templates/standard.ods
+-rw-r--r--   0 root         (0) root         (0)    25897 2021-10-13 05:27:55.000000 unogenerator-0.9.0/unogenerator/templates/standard.odt
+-rw-r--r--   0 root         (0) root         (0)    31365 2021-10-28 15:45:25.000000 unogenerator-0.9.0/unogenerator/unogenerator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 20:12:51.699847 unogenerator-0.9.0/unogenerator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      713 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-17 12:14:43.000000 unogenerator-0.9.0/unogenerator.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-10-28 20:12:51.000000 unogenerator-0.9.0/unogenerator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3054 2021-10-02 05:53:06.000000 unogenerator-0.9.0/unogenerator.epj
```

### Comparing `unogenerator-0.8.0/LICENSE` & `unogenerator-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/PKG-INFO` & `unogenerator-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unogenerator
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to read and write LibreOffice and MS Office files
 Home-page: https://github.com/turulomio/unogenerator
 Author: Turulomio
 Author-email: turulomio@yahoo.es
 License: GPL-3
 Keywords: office generator uno pyuno libreoffice
 Platform: UNKNOWN
```

### Comparing `unogenerator-0.8.0/PROBLEMS.md` & `unogenerator-0.9.0/PROBLEMS.md`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/README.md` & `unogenerator-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 - [LibreOffice API](https://api.libreoffice.org/docs/idl/ref/index.html)
 - [LibreOffice Forums](https://forum.openoffice.org/en/forum/viewforum.php?f=20)
 - [UnoGenerator API](http://turulomio.users.sourceforge.net/doxygen/unogenerator/)
 
 
 ## Changelog
 
+### 0.9.0 (2021-10-28)
+- Added monitor to restart server when needed.
+- Find and Replace method improved.
+- Automatically creates directories to save or export files.
+
 ### 0.8.0 (2021-10-18)
 - Added statistics and timing withd --debug DEBUG.
 - Process migrate to other port if there's a problem creating it.
 - Page breaks improved.
 - Tables improved.
 - Added method LoadStylesFromFile.
 - Added deleteAll method to delete all document content.
```

### Comparing `unogenerator-0.8.0/doc/Doxyfile` & `unogenerator-0.9.0/doc/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = UnoGenerator
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER         = 0.8.0
+PROJECT_NUMBER         = 0.9.0
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          = "Python module to read and write LibreOffice and MS Office files with predefined styles"
```

### Comparing `unogenerator-0.8.0/doc/unogenerator_doxygen.png` & `unogenerator-0.9.0/doc/unogenerator_doxygen.png`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/locale/en.po` & `unogenerator-0.9.0/locale/en.po`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/locale/es.po` & `unogenerator-0.9.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # root <turulomio@yahoo.es>, 2015, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: TooManyFiles\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-10-18 17:45+0200\n"
+"POT-Creation-Date: 2021-10-28 22:10+0200\n"
 "PO-Revision-Date: 2020-04-03 08:54+0200\n"
 "Last-Translator: trabajo <turulomio@yahoo.es>\n"
 "Language-Team: Spanish <kde-i18n-doc@kde.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -40,17 +40,14 @@
 msgid "Number of workers to process this script. Default 4"
 msgstr ""
 
 #, python-brace-format
 msgid "Launching concurrent demo with {args.workers} workers to a daemon with {num_instances} instances from {first_port} port"
 msgstr ""
 
-msgid "My language is "
-msgstr "Mi idioma es "
-
 msgid "UnoGenerator ODS example"
 msgstr "Ejemplo ODS con UnoGenerator"
 
 msgid "Demo with ODS class"
 msgstr "Demostración de la clase ODS"
 
 #, python-brace-format
@@ -271,15 +268,15 @@
 msgid "No data to show"
 msgstr "No hay datos para mostrar"
 
 msgid "Launches libreoffice server to run unogenerator code"
 msgstr ""
 
 #, python-brace-format
-msgid "Preparing {args.instances} libreoffice server instances from port {args.first_port}:"
+msgid "Preparing {instances} libreoffice server instances from port {first_port}:"
 msgstr ""
 
 msgid "You can see instances output in /var/log/unogenerator"
 msgstr ""
 
 #, python-brace-format
 msgid "  - Launched instance in port {port}"
@@ -287,14 +284,50 @@
 
 msgid "Stops libreoffice server to finish using unogenerator code"
 msgstr ""
 
 msgid "  - Server was stopped killing {s.stdout.decode('UTF-8').strip()} processes"
 msgstr ""
 
+msgid "Monitor unogenerator statistics"
+msgstr ""
+
+msgid "Instances: {green(instances)}"
+msgstr ""
+
+msgid "Ports used: {green(list2string(list_ports))}"
+msgstr ""
+
+#, python-brace-format
+msgid "Memory used: {str_mem_total}"
+msgstr ""
+
+msgid "Max memory recommended: {green(naturalsize(max_mem_recommended))}"
+msgstr ""
+
+#, python-brace-format
+msgid "CPU percentage: {str_cpu_percentage}"
+msgstr ""
+
+#, python-brace-format
+msgid "Connections: {str_connections}"
+msgstr ""
+
+msgid "Restarting server"
+msgstr ""
+
+msgid "Server restarted"
+msgstr ""
+
+msgid "Server wasn't restarted because it's busy"
+msgstr ""
+
+msgid "Server doesn't need to be restarted"
+msgstr ""
+
 #, python-brace-format
 msgid "Changing port {old} to {self.loserver_port} {i} times"
 msgstr ""
 
 msgid "This process died"
 msgstr ""
 
@@ -318,14 +351,17 @@
 
 msgid "Filename extension must be 'ods'."
 msgstr ""
 
 msgid "Filename extension must be 'xlsx'."
 msgstr ""
 
+#~ msgid "My language is "
+#~ msgstr "Mi idioma es "
+
 #~ msgid "Hello World example"
 #~ msgstr "Ejemplo Hola Mundo"
 
 #~ msgid "We can create tables too, for example with size 11pt:"
 #~ msgstr "También podemos crear tablas, por ejemplo con tamaño 11pt:"
 
 #~ msgid "OfficeGenerator predefined paragraph styles"
```

### Comparing `unogenerator-0.8.0/locale/unogenerator.pot` & `unogenerator-0.9.0/locale/unogenerator.pot`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-10-18 17:47+0200\n"
+"POT-Creation-Date: 2021-10-28 22:10+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -38,17 +38,14 @@
 msgid "Number of workers to process this script. Default 4"
 msgstr ""
 
 #, python-brace-format
 msgid "Launching concurrent demo with {args.workers} workers to a daemon with {num_instances} instances from {first_port} port"
 msgstr ""
 
-msgid "My language is "
-msgstr ""
-
 msgid "UnoGenerator ODS example"
 msgstr ""
 
 msgid "Demo with ODS class"
 msgstr ""
 
 #, python-brace-format
@@ -269,15 +266,15 @@
 msgid "No data to show"
 msgstr ""
 
 msgid "Launches libreoffice server to run unogenerator code"
 msgstr ""
 
 #, python-brace-format
-msgid "Preparing {args.instances} libreoffice server instances from port {args.first_port}:"
+msgid "Preparing {instances} libreoffice server instances from port {first_port}:"
 msgstr ""
 
 msgid "You can see instances output in /var/log/unogenerator"
 msgstr ""
 
 #, python-brace-format
 msgid "  - Launched instance in port {port}"
@@ -285,14 +282,50 @@
 
 msgid "Stops libreoffice server to finish using unogenerator code"
 msgstr ""
 
 msgid "  - Server was stopped killing {s.stdout.decode('UTF-8').strip()} processes"
 msgstr ""
 
+msgid "Monitor unogenerator statistics"
+msgstr ""
+
+msgid "Instances: {green(instances)}"
+msgstr ""
+
+msgid "Ports used: {green(list2string(list_ports))}"
+msgstr ""
+
+#, python-brace-format
+msgid "Memory used: {str_mem_total}"
+msgstr ""
+
+msgid "Max memory recommended: {green(naturalsize(max_mem_recommended))}"
+msgstr ""
+
+#, python-brace-format
+msgid "CPU percentage: {str_cpu_percentage}"
+msgstr ""
+
+#, python-brace-format
+msgid "Connections: {str_connections}"
+msgstr ""
+
+msgid "Restarting server"
+msgstr ""
+
+msgid "Server restarted"
+msgstr ""
+
+msgid "Server wasn't restarted because it's busy"
+msgstr ""
+
+msgid "Server doesn't need to be restarted"
+msgstr ""
+
 #, python-brace-format
 msgid "Changing port {old} to {self.loserver_port} {i} times"
 msgstr ""
 
 msgid "This process died"
 msgstr ""
```

### Comparing `unogenerator-0.8.0/setup.py` & `unogenerator-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def run(self):
         from sys import path
         path.append("unogenerator/reusing")
         from github import download_from_github
         download_from_github('turulomio','reusingcode','python/github.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/casts.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/datetime_functions.py', 'unogenerator/reusing/')
+        download_from_github('turulomio','reusingcode','python/listdict_functions.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/decorators.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/libmanagers.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/percentage.py', 'unogenerator/reusing/')
         download_from_github('turulomio','reusingcode','python/currency.py', 'unogenerator/reusing/')
 
 ## Class to define doc command
 class Translate(Command):
@@ -159,20 +160,21 @@
                  ], 
      keywords='office generator uno pyuno libreoffice',
      url='https://github.com/turulomio/unogenerator',
      author='Turulomio',
      author_email='turulomio@yahoo.es',
      license='GPL-3',
      packages=['unogenerator'],
-     install_requires=[],
+     install_requires=["humanize", "colorama"],
      entry_points = {'console_scripts': [
                             'unogenerator_demo=unogenerator.demo:main',
                             'unogenerator_demo_concurrent=unogenerator.demo:main_concurrent',
                             'unogenerator_start=unogenerator.server:server_start',
                             'unogenerator_stop=unogenerator.server:server_stop',
+                            'unogenerator_monitor=unogenerator.server:monitor',
                         ],
                     },
      cmdclass={'doxygen': Doxygen,
                'uninstall':Uninstall, 
                'translate': Translate,
                'documentation': Documentation,
                'procedure': Procedure,
```

### Comparing `unogenerator-0.8.0/unogenerator/commons.py` & `unogenerator-0.9.0/unogenerator/commons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ## @namespace unogenerator.commons
-## @brief Common code to odfpy and openpyxl wrappers
+from colorama import Fore, Style
 from datetime import datetime, date
 from gettext import translation
 from logging import info, ERROR, WARNING, INFO, DEBUG, CRITICAL, basicConfig, error
 from pkg_resources import resource_filename
 from psutil import process_iter
 from uno import createUnoStruct
+from unogenerator.reusing.listdict_functions import listdict_min
 
-__version__ = '0.8.0'
-__versiondatetime__=datetime(2021, 10, 18, 17, 41)
+__version__ = '0.9.0'
+__versiondatetime__=datetime(2021, 10, 28, 22, 8)
 __versiondate__=__versiondatetime__.date()
 
 try:
     t=translation('unogenerator',resource_filename("unogenerator","locale"))
     _=t.gettext
 except:
     _=str
@@ -431,21 +432,39 @@
         len_rows=len(o)-1
         len_columns=len(o[0])-1
     else:
         len_rows=0
         len_columns=len(o)-1
     return Range(f"{coord_start.string()}:{coord_start.addRowCopy(len_rows).addColumnCopy(len_columns).string()}")
 
-def get_from_process_numinstances_and_firstport():        
+## Returns a dictt with process info
+def get_from_process_info(cpu_percentage=False):    
     try:
-        instances=0
-        ports=[]
+        r=[]
         for p in process_iter(['name','cmdline', 'pid']): 
+            d={}
             if p.info['name']=='soffice.bin':
                 if  'file:///tmp/unogenerator'  in ' '.join(p.info['cmdline']):
-                    instances=instances+1
-                    ports.append(int(p.info['cmdline'][1][-4:]))
-        first_port=min(ports)
-        return instances, first_port
+                    d["port"]=int(p.info['cmdline'][1][-4:])
+                    d["pid"]=p.pid
+                    vms=p.memory_info().vms
+                    d["mem"]=vms
+                    if cpu_percentage is True:
+                        d["cpu_percentage"]=p.cpu_percent(interval=0.01)
+                        d["object"]=p
+                    r.append(d)
+        return r
     except:
         print(_("Have you launched unogenerator instances?. Please run unogenerator_start"))
-        return None, None
+        return []
+    
+
+def get_from_process_numinstances_and_firstport():        
+    ld=get_from_process_info()
+    return len(ld), listdict_min(ld,"port")
+   
+def red(s):
+    return Style.BRIGHT + Fore.RED + str(s) + Style.RESET_ALL
+def green(s):
+    return Style.BRIGHT + Fore.GREEN + str(s) + Style.RESET_ALL
+def magenta(s):
+    return Style.BRIGHT + Fore.MAGENTA + str(s) + Style.RESET_ALL
```

### Comparing `unogenerator-0.8.0/unogenerator/demo.py` & `unogenerator-0.9.0/unogenerator/demo.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/helpers.py` & `unogenerator-0.9.0/unogenerator/helpers.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/images/crown.png` & `unogenerator-0.9.0/unogenerator/images/crown.png`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/locale/es/LC_MESSAGES/unogenerator.mo` & `unogenerator-0.9.0/unogenerator/locale/es/LC_MESSAGES/unogenerator.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -75,17 +75,14 @@
 
 msgid "Introduction"
 msgstr "Introducción"
 
 msgid "Lists and numbered lists"
 msgstr "Listas y listas numeradas"
 
-msgid "My language is "
-msgstr "Mi idioma es "
-
 msgid "No data to show"
 msgstr "No hay datos para mostrar"
 
 msgid "Number with 2 decimals"
 msgstr "Número con 2 decimales"
 
 msgid "Number with 6 decimals"
```

### Comparing `unogenerator-0.8.0/unogenerator/reusing/casts.py` & `unogenerator-0.9.0/unogenerator/reusing/casts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## THIS IS FILE IS FROM https://github.com/turulomio/reusingcode IF YOU NEED TO UPDATE IT PLEASE MAKE A PULL REQUEST IN THAT PROJECT
 ## DO NOT UPDATE IT IN YOUR CODE IT WILL BE REPLACED USING FUNCTION IN README
 
 from decimal import Decimal
 from json import dumps
 from logging import warning
-from currency import Currency
-from percentage import Percentage
+from .currency import Currency
+from .percentage import Percentage
 
 def valueORempty(v):
     return "" if v is None else v
 
 def list2string(lista):
         """Covierte lista a string"""
         if  len(lista)==0:
```

### Comparing `unogenerator-0.8.0/unogenerator/reusing/currency.py` & `unogenerator-0.9.0/unogenerator/reusing/currency.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/reusing/datetime_functions.py` & `unogenerator-0.9.0/unogenerator/reusing/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/reusing/decorators.py` & `unogenerator-0.9.0/unogenerator/reusing/decorators.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/reusing/github.py` & `unogenerator-0.9.0/unogenerator/reusing/github.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/reusing/libmanagers.py` & `unogenerator-0.9.0/unogenerator/reusing/libmanagers.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/reusing/percentage.py` & `unogenerator-0.9.0/unogenerator/reusing/percentage.py`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/templates/standard.ods` & `unogenerator-0.9.0/unogenerator/templates/standard.ods`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/templates/standard.odt` & `unogenerator-0.9.0/unogenerator/templates/standard.odt`

 * *Files identical despite different names*

### Comparing `unogenerator-0.8.0/unogenerator/unogenerator.py` & `unogenerator-0.9.0/unogenerator/unogenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## @namespace unogenerator.unogenerator
 ## @brief Package that allows to read and write Libreoffice ods and odt files
 
 from datetime import datetime
-from os import path
+from os import path, makedirs
 from uno import getComponentContext, createUnoStruct, systemPathToFileUrl
 from com.sun.star.beans import PropertyValue
 from com.sun.star.text import ControlCharacter
 from com.sun.star.awt import Size
 from com.sun.star.style.ParagraphAdjust import RIGHT,  LEFT
 from com.sun.star.style.BreakType import PAGE_BEFORE, PAGE_AFTER
 from gettext import translation
@@ -143,14 +143,15 @@
             PropertyValue('Overwrite',0,True,0),
         )
     
 
         with TemporaryDirectory() as tmpdirname:
                 tempfile=f"{tmpdirname}/{path.basename(filename)}"
                 self.document.storeAsURL(systemPathToFileUrl(tempfile), args)
+                makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
                 copyfile(tempfile, filename)
         
                 
     def export_pdf(self, filename):
         if filename.endswith(".pdf") is False:
             print(_("Filename extension must be 'pdf'."))
             print(_("Document hasn't been saved."))
@@ -158,14 +159,16 @@
         args=(
             PropertyValue('FilterName',0,'writer_pdf_Export',0),
             PropertyValue('Overwrite',0,True,0),
         )
         with TemporaryDirectory() as tmpdirname:
             tempfile=f"{tmpdirname}/{path.basename(filename)}"
             self.document.storeToURL(systemPathToFileUrl(tempfile), args)
+            
+            makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
             copyfile(tempfile, filename)
          
     def export_docx(self, filename):
         if filename.endswith(".docx") is False:
             print(_("Filename extension must be 'docx'."))
             print(_("Document hasn't been saved."))
             return
@@ -173,28 +176,30 @@
             PropertyValue('FilterName',0,'MS Word 2007 XML',0),
             PropertyValue('Overwrite',0,True,0),
         )
 
         with TemporaryDirectory() as tmpdirname:
             tempfile=f"{tmpdirname}/{path.basename(filename)}"
             self.document.storeToURL(systemPathToFileUrl(tempfile), args)
+            makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
             copyfile(tempfile, filename)
+
 ##def insertTextIntoCell( table, cellName, text, color ):
 ##    tableText = table.getCellByName( cellName )
 ##    cursor = tableText.createTextCursor()
 ##    cursor.setPropertyValue( "CharColor", color )
 ##    tableText.setString( text )
     def find_and_replace(self, find, replace=""):
         search=self.document.createSearchDescriptor()
         search.SearchString=find
         found=self.document.findFirst(search)
         if found is not None:
             found.setString("")
             self.cursor=found
-            self.document.Text.insertString(self.cursor, replace, False)
+            found.Text.insertString(self.cursor, replace, False)
         else:
             warning(f"'{find}' was not found in the document'")
 
         
     def addParagraph(self,  text,  style):
         self.cursor.setPropertyValue("ParaStyleName", style)
         self.document.Text.insertString(self.cursor, text, False)
@@ -649,14 +654,15 @@
         args=(
             PropertyValue('FilterName', 0, 'calc8', 0),
             PropertyValue('Overwrite', 0, True, 0),
         )
         with TemporaryDirectory() as tmpdirname:
                 tempfile=f"{tmpdirname}/{path.basename(filename)}"
                 self.document.storeAsURL(systemPathToFileUrl(tempfile), args)
+                makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
                 copyfile(tempfile, filename)
         self.showStatistics()
 
     def export_pdf(self, filename):
         if filename.endswith(".pdf") is False:
             print(_("Filename extension must be 'pdf'."))
             print(_("Document hasn't been saved."))
@@ -664,14 +670,15 @@
         args=(
             PropertyValue('FilterName',0,'calc_pdf_Export',0),
             PropertyValue('Overwrite',0,True,0),
         )
         with TemporaryDirectory() as tmpdirname:
             tempfile=f"{tmpdirname}/{path.basename(filename)}"
             self.document.storeToURL(systemPathToFileUrl(tempfile), args)
+            makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
             copyfile(tempfile, filename)
 
 
     def export_xlsx(self, filename):
         if filename.endswith(".xlsx") is False:
             print(_("Filename extension must be 'xlsx'."))
             print(_("Document hasn't been saved."))
@@ -679,14 +686,15 @@
         args=(
             PropertyValue('FilterName',0,'Calc MS Excel 2007 XML',0),
             PropertyValue('Overwrite',0,True,0),
         )
         with TemporaryDirectory() as tmpdirname:
             tempfile=f"{tmpdirname}/{path.basename(filename)}"
             self.document.storeToURL(systemPathToFileUrl(tempfile), args)
+            makedirs(path.dirname(path.abspath(filename)), exist_ok=True)
             copyfile(tempfile, filename)
 
 
 class ODS_Standard(ODS):
     def __init__(self, loserver_port=2002):
         ODS.__init__(self, resource_filename(__name__, 'templates/standard.ods'), loserver_port)
```

### Comparing `unogenerator-0.8.0/unogenerator.egg-info/PKG-INFO` & `unogenerator-0.9.0/unogenerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unogenerator
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to read and write LibreOffice and MS Office files
 Home-page: https://github.com/turulomio/unogenerator
 Author: Turulomio
 Author-email: turulomio@yahoo.es
 License: GPL-3
 Keywords: office generator uno pyuno libreoffice
 Platform: UNKNOWN
```

### Comparing `unogenerator-0.8.0/unogenerator.egg-info/SOURCES.txt` & `unogenerator-0.9.0/unogenerator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 unogenerator/server.py
 unogenerator/unogenerator.py
 unogenerator.egg-info/PKG-INFO
 unogenerator.egg-info/SOURCES.txt
 unogenerator.egg-info/dependency_links.txt
 unogenerator.egg-info/entry_points.txt
 unogenerator.egg-info/not-zip-safe
+unogenerator.egg-info/requires.txt
 unogenerator.egg-info/top_level.txt
 unogenerator/images/crown.png
 unogenerator/locale/en/LC_MESSAGES/unogenerator.mo
 unogenerator/locale/es/LC_MESSAGES/unogenerator.mo
 unogenerator/reusing/__init__.py
 unogenerator/reusing/casts.py
 unogenerator/reusing/currency.py
 unogenerator/reusing/datetime_functions.py
 unogenerator/reusing/decorators.py
 unogenerator/reusing/github.py
 unogenerator/reusing/libmanagers.py
+unogenerator/reusing/listdict_functions.py
 unogenerator/reusing/percentage.py
 unogenerator/templates/standard.ods
 unogenerator/templates/standard.odt
```

### Comparing `unogenerator-0.8.0/unogenerator.epj` & `unogenerator-0.9.0/unogenerator.epj`

 * *Files identical despite different names*

