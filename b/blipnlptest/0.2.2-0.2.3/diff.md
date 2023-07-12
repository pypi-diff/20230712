# Comparing `tmp/blipnlptest-0.2.2.tar.gz` & `tmp/blipnlptest-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.2.2.tar", max compression
+gzip compressed data, was "blipnlptest-0.2.3.tar", max compression
```

## Comparing `blipnlptest-0.2.2.tar` & `blipnlptest-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-07-12 15:30:30.519732 blipnlptest-0.2.2/blipnlptest/__init__.py
--rw-r--r--   0        0        0     6879 2023-07-12 15:52:34.526305 blipnlptest-0.2.2/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-07-12 15:30:30.441607 blipnlptest-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-07-12 15:52:59.077550 blipnlptest-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3232 2023-07-12 15:37:40.896034 blipnlptest-0.2.2/README.md
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 blipnlptest-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-07-12 15:30:30.519732 blipnlptest-0.2.3/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     7033 2023-07-12 16:12:52.167594 blipnlptest-0.2.3/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-07-12 15:30:30.441607 blipnlptest-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-07-12 16:13:05.392213 blipnlptest-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3233 2023-07-12 16:13:56.304970 blipnlptest-0.2.3/README.md
+-rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 blipnlptest-0.2.3/PKG-INFO
```

### Comparing `blipnlptest-0.2.2/blipnlptest/blipnlptest.py` & `blipnlptest-0.2.3/blipnlptest/blipnlptest.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,20 +143,23 @@
       print('O parâmetro model deve ter o valor de y ou n.')
 
     return(result)
 
   def test_content(self, intention, entities):
 
     if isinstance(entities, str):
-        if entities == '':
+        if entities == '' or entities == '['']' or entities == ['']:
           entities = []
         else:
           entities = [entities]
     elif isinstance(entities, list):
-        pass
+        if entities == '' or entities == '['']' or entities == ['']:
+          entities = []
+        else:
+          pass
 
     body =  {
               "id": "46544651",
               "to": "postmaster@ai.msging.net",
               "method": "set",
               "uri": "/content/analysis",
               "resource": {
```

### Comparing `blipnlptest-0.2.2/LICENSE.txt` & `blipnlptest-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.2.2/pyproject.toml` & `blipnlptest-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.2.2/README.md` & `blipnlptest-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 Caso queira analisar com dados que não estejam na base de dados, utilize o recurso do bot. O recurso deverá ser do tipo texto, e as mensagens separadas por vírgula. Use:
 
 <pre><code>
 
 import blipnlptest as bnt
 
 cc = bnt.contentchecker(key, resource='nome_do_recurso')
-cc.sentences()
+cc.byresource()
 </code></pre>
 
 Em todos os casos, você pode colocar o valor do threshold personalizado, da seguinte forma:
 
 <pre><code>
 cc = bnt.contentchecker(key, data=df,threshold=0.6)
 cc.sentences()
```

### Comparing `blipnlptest-0.2.2/PKG-INFO` & `blipnlptest-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.2.2
+Version: 0.2.3
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 Caso queira analisar com dados que não estejam na base de dados, utilize o recurso do bot. O recurso deverá ser do tipo texto, e as mensagens separadas por vírgula. Use:
 
 <pre><code>
 
 import blipnlptest as bnt
 
 cc = bnt.contentchecker(key, resource='nome_do_recurso')
-cc.sentences()
+cc.byresource()
 </code></pre>
 
 Em todos os casos, você pode colocar o valor do threshold personalizado, da seguinte forma:
 
 <pre><code>
 cc = bnt.contentchecker(key, data=df,threshold=0.6)
 cc.sentences()
```

