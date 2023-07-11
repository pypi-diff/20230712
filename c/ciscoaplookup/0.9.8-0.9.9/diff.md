# Comparing `tmp/ciscoaplookup-0.9.8.tar.gz` & `tmp/ciscoaplookup-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ciscoaplookup-0.9.8.tar", last modified: Thu Oct 17 08:19:04 2019, max compression
+gzip compressed data, was "dist/ciscoaplookup-0.9.9.tar", last modified: Fri Nov  8 08:58:56 2019, max compression
```

## Comparing `ciscoaplookup-0.9.8.tar` & `ciscoaplookup-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/
-drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/test/
--rw-r--r--   0 stsmr      (501) staff       (20)       49 2019-04-23 21:18:44.000000 ciscoaplookup-0.9.8/test/__init__.py
--rw-r--r--   0 stsmr      (501) staff       (20)     1133 2019-10-08 10:24:47.000000 ciscoaplookup-0.9.8/test/test_ciscoaplookup.py
-drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/
--rw-r--r--   0 stsmr      (501) staff       (20)     2896 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/PKG-INFO
--rw-r--r--   0 stsmr      (501) staff       (20)       14 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/requires.txt
--rw-r--r--   0 stsmr      (501) staff       (20)       19 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/top_level.txt
--rw-r--r--   0 stsmr      (501) staff       (20)      295 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/SOURCES.txt
--rw-r--r--   0 stsmr      (501) staff       (20)        1 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup.egg-info/dependency_links.txt
--rw-r--r--   0 stsmr      (501) staff       (20)     2896 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/PKG-INFO
--rw-r--r--   0 stsmr      (501) staff       (20)      941 2019-10-17 08:18:16.000000 ciscoaplookup-0.9.8/setup.py
--rw-r--r--   0 stsmr      (501) staff       (20)     2073 2019-09-12 12:09:45.000000 ciscoaplookup-0.9.8/README.md
--rw-r--r--   0 stsmr      (501) staff       (20)       38 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/setup.cfg
-drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-10-17 08:19:04.000000 ciscoaplookup-0.9.8/ciscoaplookup/
--rw-r--r--   0 stsmr      (501) staff       (20)      133 2019-09-12 12:11:26.000000 ciscoaplookup-0.9.8/ciscoaplookup/__init__.py
--rw-r--r--   0 stsmr      (501) staff       (20)     5900 2019-10-17 08:18:09.000000 ciscoaplookup-0.9.8/ciscoaplookup/logic.py
+drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/
+drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/test/
+-rw-r--r--   0 stsmr      (501) staff       (20)       49 2019-04-23 21:18:44.000000 ciscoaplookup-0.9.9/test/__init__.py
+-rw-r--r--   0 stsmr      (501) staff       (20)     1133 2019-10-08 10:24:47.000000 ciscoaplookup-0.9.9/test/test_ciscoaplookup.py
+drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/
+-rw-r--r--   0 stsmr      (501) staff       (20)     2896 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/PKG-INFO
+-rw-r--r--   0 stsmr      (501) staff       (20)       14 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/requires.txt
+-rw-r--r--   0 stsmr      (501) staff       (20)       19 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/top_level.txt
+-rw-r--r--   0 stsmr      (501) staff       (20)      295 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/SOURCES.txt
+-rw-r--r--   0 stsmr      (501) staff       (20)        1 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup.egg-info/dependency_links.txt
+-rw-r--r--   0 stsmr      (501) staff       (20)     2896 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/PKG-INFO
+-rw-r--r--   0 stsmr      (501) staff       (20)      941 2019-11-08 08:55:39.000000 ciscoaplookup-0.9.9/setup.py
+-rw-r--r--   0 stsmr      (501) staff       (20)     2073 2019-09-12 12:09:45.000000 ciscoaplookup-0.9.9/README.md
+-rw-r--r--   0 stsmr      (501) staff       (20)       38 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/setup.cfg
+drwxr-xr-x   0 stsmr      (501) staff       (20)        0 2019-11-08 08:58:56.000000 ciscoaplookup-0.9.9/ciscoaplookup/
+-rw-r--r--   0 stsmr      (501) staff       (20)      133 2019-09-12 12:11:26.000000 ciscoaplookup-0.9.9/ciscoaplookup/__init__.py
+-rw-r--r--   0 stsmr      (501) staff       (20)     5979 2019-11-08 08:55:19.000000 ciscoaplookup-0.9.9/ciscoaplookup/logic.py
```

### Comparing `ciscoaplookup-0.9.8/test/test_ciscoaplookup.py` & `ciscoaplookup-0.9.9/test/test_ciscoaplookup.py`

 * *Files identical despite different names*

### Comparing `ciscoaplookup-0.9.8/ciscoaplookup.egg-info/PKG-INFO` & `ciscoaplookup-0.9.9/ciscoaplookup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscoaplookup
-Version: 0.9.8
+Version: 0.9.9
 Summary: The Cisco Wireless LAN Compliance Lookup library
 Home-page: https://github.com/steffenschumacher/ciscoaplookup.git
 Author: Steffen Schumacher
 Author-email: ssch@wheel.dk
 License: UNKNOWN
 Description: # Introduction 
         Tiny python library to determine actual available Cisco AP models, and their full name, specific to the regulatory
```

### Comparing `ciscoaplookup-0.9.8/PKG-INFO` & `ciscoaplookup-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscoaplookup
-Version: 0.9.8
+Version: 0.9.9
 Summary: The Cisco Wireless LAN Compliance Lookup library
 Home-page: https://github.com/steffenschumacher/ciscoaplookup.git
 Author: Steffen Schumacher
 Author-email: ssch@wheel.dk
 License: UNKNOWN
 Description: # Introduction 
         Tiny python library to determine actual available Cisco AP models, and their full name, specific to the regulatory
```

### Comparing `ciscoaplookup-0.9.8/README.md` & `ciscoaplookup-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ciscoaplookup-0.9.8/ciscoaplookup/logic.py` & `ciscoaplookup-0.9.9/ciscoaplookup/logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,15 +122,16 @@
                     h[model] = col
                     break
             except IndexError:
                 raise ValueError('Unable to find the model {} in the {} platform?'.format(model, platform))
         for row_no in range(1, sheet.nrows):
             row = parse_row(row_no, h, sheet)
             if not row: continue
-            if not country or row['Country'].lower() == country.lower():
+            # this way we also match United States in United States of America
+            if not country or country.lower() in row['Country'].lower():
                 found_country = True
                 if row[model] == 'x':
                     valid_domains.add(row['Regulatory Domain'])
 
     if valid_domains:
         return list(valid_domains)
     elif found_country:
```

