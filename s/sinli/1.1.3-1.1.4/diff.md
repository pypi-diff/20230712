# Comparing `tmp/sinli-1.1.3.tar.gz` & `tmp/sinli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.3.tar", last modified: Tue Jun 27 10:59:01 2023, max compression
+gzip compressed data, was "sinli-1.1.4.tar", last modified: Wed Jul 12 10:34:27 2023, max compression
```

## Comparing `sinli-1.1.3.tar` & `sinli-1.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2023-06-27 10:41:00.000000 sinli-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45669 2023-06-27 10:59:01.585718 sinli-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5445 2023-06-27 10:58:52.000000 sinli-1.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-27 10:58:52.000000 sinli-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 10:59:01.585718 sinli-1.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     5491 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7392 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45669 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-27 10:41:00.000000 sinli-1.1.3/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.306263 sinli-1.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2023-07-12 10:33:18.000000 sinli-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45669 2023-07-12 10:34:27.306263 sinli-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5445 2023-07-12 10:33:18.000000 sinli-1.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-12 10:34:17.000000 sinli-1.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:34:27.306263 sinli-1.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     7418 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45669 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-12 10:33:18.000000 sinli-1.1.4/tests/test_document.py
```

### Comparing `sinli-1.1.3/LICENSE` & `sinli-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/PKG-INFO` & `sinli-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.3
+Version: 1.1.4
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.3/README.md` & `sinli-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/pyproject.toml` & `sinli-1.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.1.3"
+version = "1.1.4"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.1.3/src/sinli/common/encoded_values.py` & `sinli-1.1.4/src/sinli/common/encoded_values.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/__init__.py` & `sinli-1.1.4/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/envio/v8.py` & `sinli-1.1.4/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/factul/v1.py` & `sinli-1.1.4/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/libros/v8.py` & `sinli-1.1.4/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/libros/v9.py` & `sinli-1.1.4/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/mensaj/v1.py` & `sinli-1.1.4/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/doctype/pedido/v7.py` & `sinli-1.1.4/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/document.py` & `sinli-1.1.4/src/sinli/document.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.3/src/sinli/line.py` & `sinli-1.1.4/src/sinli/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
             return str(v)
         return str(v)
 
 class LongIdentificationLine(Line):
     def __post_init__(self):
         super().__post_init__()
         self.TYPE = "I"
+        self.FORMAT = "N"
 
     class Field(Enum):
         TYPE = (0, 1, t.STR, "Tipo de registro (I)")
         FORMAT = (1, 1, t.STR, "Tipo de formato (N=Normalizado ; ?=Libre)")
         DOCTYPE = (2, 6, t.STR, "Nombre del tipo de documento")
         VERSION = (8, 2, t.STR, "Versión del tipo de documento")
         FROM = (10, 8, t.STR, "Identificador ESFANDE del remitente")
```

### Comparing `sinli-1.1.3/src/sinli.egg-info/PKG-INFO` & `sinli-1.1.4/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.3
+Version: 1.1.4
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.3/src/sinli.egg-info/SOURCES.txt` & `sinli-1.1.4/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

