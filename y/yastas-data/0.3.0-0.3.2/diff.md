# Comparing `tmp/yastas-data-0.3.0.tar.gz` & `tmp/yastas-data-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.3.0.tar", last modified: Mon Jul 10 21:09:03 2023, max compression
+gzip compressed data, was "yastas-data-0.3.2.tar", last modified: Wed Jul 12 19:55:22 2023, max compression
```

## Comparing `yastas-data-0.3.0.tar` & `yastas-data-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.640427 yastas-data-0.3.0/
--rw-rw-rw-   0        0        0      583 2023-07-10 21:09:03.631727 yastas-data-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.466417 yastas-data-0.3.0/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.0/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.478759 yastas-data-0.3.0/data_code/beam/
--rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.0/data_code/beam/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-07-10 21:03:38.000000 yastas-data-0.3.0/data_code/beam/database.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.548075 yastas-data-0.3.0/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.0/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.0/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.0/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.0/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     3555 2023-07-10 20:36:32.000000 yastas-data-0.3.0/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.0/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.581602 yastas-data-0.3.0/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.0/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.0/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.0/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-10 21:09:03.642066 yastas-data-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-10 21:05:58.000000 yastas-data-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.623598 yastas-data-0.3.0/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      583 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.588673 yastas-data-0.3.2/
+-rw-rw-rw-   0        0        0      583 2023-07-12 19:55:22.574527 yastas-data-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.325414 yastas-data-0.3.2/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.2/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.345452 yastas-data-0.3.2/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.2/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-07-12 18:48:22.000000 yastas-data-0.3.2/data_code/beam/database.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.445880 yastas-data-0.3.2/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.2/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.2/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.2/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.2/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     3558 2023-07-12 19:35:01.000000 yastas-data-0.3.2/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.2/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.484738 yastas-data-0.3.2/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.2/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.2/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.2/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:55:22.589668 yastas-data-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-12 19:54:32.000000 yastas-data-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:55:22.558858 yastas-data-0.3.2/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-07-12 19:55:22.000000 yastas-data-0.3.2/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-12 19:55:22.000000 yastas-data-0.3.2/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:55:22.000000 yastas-data-0.3.2/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 19:55:22.000000 yastas-data-0.3.2/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.3.0/PKG-INFO` & `yastas-data-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.0
+Version: 0.3.2
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

### Comparing `yastas-data-0.3.0/data_code/beam/database.py` & `yastas-data-0.3.2/data_code/beam/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,24 @@
         self.database=database
         self.query = query
         self.string_conn = string_conn
         self.project_id = project_id
         self.secret_user = secret_user
         self.secret_password = secret_password
         self.postgres = Database(self.host,self.port,self.database,self.secret_user,self.secret_password, self.project_id)
-        self.conn = self.postgres.get_connection()
 
     def setup(self):
+        self.conn = self.postgres.get_connection()
         self.postgres.raise_proxy(self.string_conn)
-
-    def process(self, element, *args, **kwargs):
-        
         
+
+    def process(self, element):
         query_result=self.postgres.execute_query(self.conn, query=self.query)
+        self.postgres.close_connection(self.conn)
+        self.postgres.shut_down_proxy()
+        return query_result
         
-        yield query_result
 
     def teardown(self):
-        self.postgres.close_connection(self.conn)
-        self.postgres.shut_down_proxy()
-        return super().teardown()
+        # Investigate functionality
+        pass
```

### Comparing `yastas-data-0.3.0/data_code/gcp/bq.py` & `yastas-data-0.3.2/data_code/gcp/bq.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.0/data_code/gcp/sql.py` & `yastas-data-0.3.2/data_code/gcp/sql.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         logging.info(msg)
         print(msg)
 
     def raise_proxy(self, string_connection:str):
         self.logprint_i("Inicia levantacion del proxy.....")
         PROXYUP_COMMANDS = [
             f"rm -fr DTF && mkdir DTF && cd DTF && \
-            wget https://dl.google.com/cloudsql/cloud_sql_proxy.linux.amd64 -O cloud_sql_proxy && ls -la cloud_sql_proxy && \
+            wget --progress=bar:force:noscrol https://dl.google.com/cloudsql/cloud_sql_proxy.linux.amd64 -O cloud_sql_proxy && ls -la cloud_sql_proxy && \
             chmod 755 cloud_sql_proxy && ls -la cloud_sql_proxy && pwd && ls -latrh && \
             nohup ./{string_connection} -ip_address_types=PRIVATE  & \&& \
             sleep 5 ",
         ]
 
         self.logprint_i("Inicia descarga proxy")
         for command in PROXYUP_COMMANDS:
@@ -54,15 +54,15 @@
             port=self.port, 
             database=self.database_name,
             user=self.user,
             password=self.password
         )
         return connection
     
-    def get_tables(self, connection:psycopg2):
+    def get_tables(self, connection):
 
         # Crear un cursor para ejecutar consultas
         cursor = connection.cursor()
         
 
         # Obtener los nombres de las tablas
         cursor.execute("""
@@ -81,17 +81,17 @@
         print("~~~~~~~~~~~~~~~~~~~~~~~~")
         
         for fila in filas:
             print(f"| {fila[0]:^20} |")
             print("________________________")
         print("\n")
         # Cerrar el cursor y la conexión
-        cursor.close()
+        #cursor.close()
         
-    def execute_query(self, connection:psycopg2, query:str):
+    def execute_query(self, connection, query:str):
 
         # Crear un cursor para ejecutar consultas
         cursor = connection.cursor()
 
         # Ejecutar una consulta de ejemplo
         cursor.execute(query)
 
@@ -102,11 +102,11 @@
         # for fila in filas:
         #     print(fila)
 
         # Cerrar el cursor y la conexión
         cursor.close()
         return query_result
 
-    def close_connection(self, connection:psycopg2):
+    def close_connection(self, connection):
         # Cerrar el cursor y la conexión
         connection.close()
```

### Comparing `yastas-data-0.3.0/data_code/parquets/parquet2csv.py` & `yastas-data-0.3.2/data_code/parquets/parquet2csv.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.0/setup.py` & `yastas-data-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.3.0',
+    version='0.3.2',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

### Comparing `yastas-data-0.3.0/yastas_data.egg-info/PKG-INFO` & `yastas-data-0.3.2/yastas_data.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.0
+Version: 0.3.2
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

