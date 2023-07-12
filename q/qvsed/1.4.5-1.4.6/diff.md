# Comparing `tmp/qvsed-1.4.5.tar.gz` & `tmp/qvsed-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.4.5.tar", last modified: Wed Jul 12 15:20:09 2023, max compression
+gzip compressed data, was "qvsed-1.4.6.tar", last modified: Wed Jul 12 15:24:00 2023, max compression
```

## Comparing `qvsed-1.4.5.tar` & `qvsed-1.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:20:09.743756 qvsed-1.4.5/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-12 15:20:09.740757 qvsed-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     7228 2023-07-11 10:35:02.000000 qvsed-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:20:09.713788 qvsed-1.4.5/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.5/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.4.5/qvsed/config_default.py
--rw-rw-rw-   0        0        0    22683 2023-07-12 15:19:35.000000 qvsed-1.4.5/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.5/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-12 15:20:09.738739 qvsed-1.4.5/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 15:20:09.000000 qvsed-1.4.5/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:20:09.751285 qvsed-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-12 15:19:49.000000 qvsed-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.641591 qvsed-1.4.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-12 15:24:00.641591 qvsed-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7228 2023-07-11 10:35:02.000000 qvsed-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.621207 qvsed-1.4.6/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.6/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.4.6/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    22683 2023-07-12 15:23:21.000000 qvsed-1.4.6/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.6/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.639592 qvsed-1.4.6/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:24:00.642610 qvsed-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-12 15:23:46.000000 qvsed-1.4.6/setup.py
```

### Comparing `qvsed-1.4.5/LICENSE.txt` & `qvsed-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.5/PKG-INFO` & `qvsed-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.5
+Version: 1.4.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.5/README.md` & `qvsed-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.5/qvsed/config_default.py` & `qvsed-1.4.6/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.5/qvsed/qvsed.py` & `qvsed-1.4.6/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
     def set_up_fonts(self):
         """
         Set up the fonts for the QVSED window.
         """
         text_area = self.textArea
         font = QFont()
         font.setFamilies(self.font_family)
-        if sys.platform == "Darwin":
+        if sys.platform == "darwin":
             # macOS fonts should be bigger
             self.font_size += 4
         font.setPointSize(self.font_size)
         text_area.setTabStopWidth(4 * text_area.fontMetrics().width(' '))
         QApplication.instance().setFont(font)
         self.update_widget_fonts(self)
```

### Comparing `qvsed-1.4.5/qvsed/qvsed.ui` & `qvsed-1.4.6/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.5/qvsed.egg-info/PKG-INFO` & `qvsed-1.4.6/qvsed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.5
+Version: 1.4.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.5/setup.py` & `qvsed-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.4.5',
+    version='1.4.6',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

