# Comparing `tmp/ttb-0.2.tar.gz` & `tmp/ttb-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttb-0.2.tar", last modified: Wed Jul 12 11:56:10 2023, max compression
+gzip compressed data, was "ttb-0.3.tar", last modified: Wed Jul 12 11:59:14 2023, max compression
```

## Comparing `ttb-0.2.tar` & `ttb-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:56:10.000327 ttb-0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-12 10:58:03.000000 ttb-0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-12 10:58:03.000000 ttb-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)      734 2023-07-12 11:56:10.000327 ttb-0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      379 2023-07-12 11:53:31.000000 ttb-0.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 11:56:10.000327 ttb-0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      540 2023-07-12 11:55:28.000000 ttb-0.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:56:09.996327 ttb-0.2/ttb/
--rw-r--r--   0 runner    (1000) runner    (1000)     1040 2023-07-12 11:53:30.000000 ttb-0.2/ttb/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:56:10.000327 ttb-0.2/ttb.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      734 2023-07-12 11:56:09.000000 ttb-0.2/ttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-07-12 11:56:09.000000 ttb-0.2/ttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:56:09.000000 ttb-0.2/ttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:56:09.000000 ttb-0.2/ttb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)        4 2023-07-12 11:56:09.000000 ttb-0.2/ttb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:59:14.020136 ttb-0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-12 10:58:03.000000 ttb-0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-12 10:58:03.000000 ttb-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-07-12 11:59:14.020136 ttb-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      399 2023-07-12 11:58:48.000000 ttb-0.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 11:59:14.024136 ttb-0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      540 2023-07-12 11:58:55.000000 ttb-0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:59:14.016136 ttb-0.3/ttb/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1040 2023-07-12 11:53:30.000000 ttb-0.3/ttb/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:59:14.020136 ttb-0.3/ttb.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-07-12 11:59:13.000000 ttb-0.3/ttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-07-12 11:59:13.000000 ttb-0.3/ttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:59:13.000000 ttb-0.3/ttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:59:13.000000 ttb-0.3/ttb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        4 2023-07-12 11:59:13.000000 ttb-0.3/ttb.egg-info/top_level.txt
```

### Comparing `ttb-0.2/LICENSE` & `ttb-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttb-0.2/PKG-INFO` & `ttb-0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ttb
-Version: 0.2
+Version: 0.3
 Summary: Библиотека со всякимим полезностями
 Author: Neso Hiroshi
 Author-email: neso_hoshi_official@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 # Библиотека со всякими полезностями
 
 Здесь есть функции:
-loading(delay) - Прогрессбар, вместо delay ввести задержку
-test(text) - Можно оставить аргумент пустым или ввести текст
-collatz(number) - Теория 3N + 1, вместо number ввести число
+- `loading(delay)`: Прогрессбар. Вместо `delay` введите задержку.
+- `test(text)`: Можно оставить аргумент пустым или ввести текст.
+- `collatz(number)`: Теория 3N + 1. Вместо `number` введите число.
```

### Comparing `ttb-0.2/setup.py` & `ttb-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ttb',
-      version='0.2',
+      version='0.3',
       description='Библиотека со всякимим полезностями',
       long_description=long_description,
       author_email='neso_hoshi_official@mail.ru',
       zip_safe=False,
       author='Neso Hiroshi',
       classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ttb-0.2/ttb/__init__.py` & `ttb-0.3/ttb/__init__.py`

 * *Files identical despite different names*

### Comparing `ttb-0.2/ttb.egg-info/PKG-INFO` & `ttb-0.3/ttb.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ttb
-Version: 0.2
+Version: 0.3
 Summary: Библиотека со всякимим полезностями
 Author: Neso Hiroshi
 Author-email: neso_hoshi_official@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 # Библиотека со всякими полезностями
 
 Здесь есть функции:
-loading(delay) - Прогрессбар, вместо delay ввести задержку
-test(text) - Можно оставить аргумент пустым или ввести текст
-collatz(number) - Теория 3N + 1, вместо number ввести число
+- `loading(delay)`: Прогрессбар. Вместо `delay` введите задержку.
+- `test(text)`: Можно оставить аргумент пустым или ввести текст.
+- `collatz(number)`: Теория 3N + 1. Вместо `number` введите число.
```

