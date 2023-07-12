# Comparing `tmp/yastas-data-0.3.3.tar.gz` & `tmp/yastas-data-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.3.3.tar", last modified: Wed Jul 12 20:06:25 2023, max compression
+gzip compressed data, was "yastas-data-0.3.4.tar", last modified: Wed Jul 12 21:36:25 2023, max compression
```

## Comparing `yastas-data-0.3.3.tar` & `yastas-data-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.986858 yastas-data-0.3.3/
--rw-rw-rw-   0        0        0      583 2023-07-12 20:06:24.971421 yastas-data-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.721863 yastas-data-0.3.3/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.3/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.739665 yastas-data-0.3.3/data_code/beam/
--rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.3/data_code/beam/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-07-12 18:48:22.000000 yastas-data-0.3.3/data_code/beam/database.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.844360 yastas-data-0.3.3/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.3/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.3/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.3/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.3/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     3559 2023-07-12 19:58:48.000000 yastas-data-0.3.3/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.3/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.889310 yastas-data-0.3.3/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.3/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.3/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.3/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-12 20:06:24.988070 yastas-data-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-12 20:06:17.000000 yastas-data-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:06:24.959656 yastas-data-0.3.3/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      583 2023-07-12 20:06:24.000000 yastas-data-0.3.3/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-12 20:06:24.000000 yastas-data-0.3.3/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:06:24.000000 yastas-data-0.3.3/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 20:06:24.000000 yastas-data-0.3.3/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:25.014628 yastas-data-0.3.4/
+-rw-rw-rw-   0        0        0      583 2023-07-12 21:36:25.003700 yastas-data-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.752498 yastas-data-0.3.4/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.4/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.775649 yastas-data-0.3.4/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.4/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-07-12 21:01:11.000000 yastas-data-0.3.4/data_code/beam/database.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.882716 yastas-data-0.3.4/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.4/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.4/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.4/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.4/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     3597 2023-07-12 21:35:49.000000 yastas-data-0.3.4/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.4/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.927109 yastas-data-0.3.4/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.4/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.4/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.4/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-07-12 21:36:25.015699 yastas-data-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-12 21:36:01.000000 yastas-data-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.991840 yastas-data-0.3.4/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.3.3/PKG-INFO` & `yastas-data-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.3
+Version: 0.3.4
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

### Comparing `yastas-data-0.3.3/data_code/beam/database.py` & `yastas-data-0.3.4/data_code/beam/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import apache_beam as beam
 from data_code.gcp.sql import Database
-
+import time
 class GetQuery(beam.DoFn):
     def __init__(self, host, port, database, query, string_conn, project_id, secret_user, secret_password):
         self.host=host
         self.port=port
         self.database=database
         self.query = query
         self.string_conn = string_conn
```

### Comparing `yastas-data-0.3.3/data_code/gcp/bq.py` & `yastas-data-0.3.4/data_code/gcp/bq.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.3/data_code/gcp/sql.py` & `yastas-data-0.3.4/data_code/gcp/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from data_code.gcp.secrets import get_secret
 import psycopg2
 import logging
 import os
-
+import time
 class Proxy():
     """Funcionalidades relacionadas al proxy para lograr comunicación con bases de datos.
     """
     def logprint_i(self,msg):
         logging.info(msg)
         print(msg)
 
@@ -19,14 +19,15 @@
             nohup ./{string_connection} -ip_address_types=PRIVATE  & \&& \
             sleep 5 ",
         ]
 
         self.logprint_i("Inicia descarga proxy")
         for command in PROXYUP_COMMANDS:
             os.system(command)
+            time.sleep(3)
         self.logprint_i("termina levantacion del proxy.....")
 
         self.logprint_i("proxy_up_executed")
     
     def shut_down_proxy(self):
         #TODO: Crear la baja del proxy para evitar vulnerabilidades.
         os.system("rm -fr DTF")
```

### Comparing `yastas-data-0.3.3/data_code/parquets/parquet2csv.py` & `yastas-data-0.3.4/data_code/parquets/parquet2csv.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.3/setup.py` & `yastas-data-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.3.3',
+    version='0.3.4',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

### Comparing `yastas-data-0.3.3/yastas_data.egg-info/PKG-INFO` & `yastas-data-0.3.4/yastas_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.3
+Version: 0.3.4
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

