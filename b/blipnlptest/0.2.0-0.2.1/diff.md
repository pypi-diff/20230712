# Comparing `tmp/blipnlptest-0.2.0.tar.gz` & `tmp/blipnlptest-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.2.0.tar", max compression
+gzip compressed data, was "blipnlptest-0.2.1.tar", max compression
```

## Comparing `blipnlptest-0.2.0.tar` & `blipnlptest-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-06-23 18:18:09.432166 blipnlptest-0.2.0/blipnlptest/__init__.py
--rw-r--r--   0        0        0     6589 2023-06-23 18:18:09.503090 blipnlptest-0.2.0/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-06-23 18:18:09.712227 blipnlptest-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-06-23 18:18:09.752286 blipnlptest-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3177 2023-06-23 18:18:09.791777 blipnlptest-0.2.0/README.md
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 blipnlptest-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-07-12 15:30:30.519732 blipnlptest-0.2.1/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     6901 2023-07-12 15:30:30.535356 blipnlptest-0.2.1/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-07-12 15:30:30.441607 blipnlptest-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-07-12 15:30:30.472864 blipnlptest-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3232 2023-07-12 15:37:40.896034 blipnlptest-0.2.1/README.md
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 blipnlptest-0.2.1/PKG-INFO
```

### Comparing `blipnlptest-0.2.0/blipnlptest/blipnlptest.py` & `blipnlptest-0.2.1/blipnlptest/blipnlptest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 import pandas as pd
 import warnings
 
 warnings.filterwarnings("ignore", category=pd.core.common.SettingWithCopyWarning)
 
 class contentchecker:
 
-  def __init__(self, key, data=None, resource=None, threshold=0.5):
-
+  def __init__(self, key, data=None, resource=None, threshold=0.5, contract_id=None):
+      
+      self.contract_id = contract_id
       self.threshold = threshold
       self.resource = resource
       self.data = data
       self.key = key
-      self.url = 'https://http.msging.net/commands'
+      
+      if contract_id == None:
+          self.url = 'https://http.msging.net/commands'
+      else:
+          self.url = f'https://{contract_id}.http.msging.net/commands'
+
       self.header = {
             'content-type': 'application/json',
             'Authorization': self.key
             }
       """  
         if isinstance(data, None) == False:
           if isinstance(data, pd.DataFrame) == False:
@@ -78,36 +84,39 @@
     for i in range(len(df.Text)):
         try:
           ent.append(pd.json_normalize(df.Entities[i]).value.tolist())
         except AttributeError:
           ent.append('')
 
     df.loc[:, 'Content'] = [self.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
-    df = df.sort_values(by='Content',ascending=False)
-    
+        
     return(self.check_threshold(df))
 
   def byresource(self):
 
     body ={  
             "id": "{{$guid}}",
             "method": "get",
             "uri": f"/resources/{self.resource}"
           }        
     
+    
     r = requests.post(self.url, json=body,headers=self.header).json()
+    
     try:
-      if r['reason']['code'] == 67:
-        print("o recurso teste-modelo não foi encontrado, confira a existência e o nome do seu recurso.")
+      df = pd.DataFrame({'Text':r['resource'].split(',')})
+      return(self.sentences(df))
     except KeyError:
-        if r['resource']:
-          df = pd.DataFrame({'Text':r['resource'].split(',')})
-          return(self.sentences(df))
-        else:
-          print('Erro inesperado com o ser recurso.')
+      if r['code'] == 13:
+        print("Verifique se o contract_id e/ou a key estão corretos.")
+      elif r['code'] == 67:
+        print("o recurso teste-modelo não foi encontrado, confira a existência e o nome do seu recurso.")
+      else:
+        print(f"Ops, algo de errado aconteceu. - {r['code']}")
+
 
   def test(self, model, text=None, intention=None, entities=None):
 
     if model == 'y':
 
       body =  {
                 "id": "{{$guid}}",
@@ -134,18 +143,23 @@
       print('O parâmetro model deve ter o valor de y ou n.')
 
     return(result)
 
   def test_content(self, intention, entities):
 
     if isinstance(entities, str):
-        entities = [entities]
+        if entities == '':
+          entities = []
+        else:
+          entities = [entities]
     elif isinstance(entities, list):
         pass
 
+    print(entities)
+
     body =  {
               "id": "46544651",
               "to": "postmaster@ai.msging.net",
               "method": "set",
               "uri": "/content/analysis",
               "resource": {
                 "intent": intention,
```

### Comparing `blipnlptest-0.2.0/LICENSE.txt` & `blipnlptest-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.2.0/pyproject.toml` & `blipnlptest-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.2.0/README.md` & `blipnlptest-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
 - data (opcional) : Dataframe de entrada
 - resource (opcional) : Nome do recurso com o texto de tests
 - threshold (opcional) : float referente ao threshold do provedor com valores entre 0.1 (10%) a 1.0 (100%). (default: 0.5)
-- key : chave do bot.
+- key: chave do bot
+- contract_id: id do contrato.
 
 Exemplo do código:
 
 
 Caso a análise seja de dados já analisados pelo provedor (envie um dataframe que tenha no mínimo as colunas Text, Intentions, Entities e Score), use:
 
 <pre><code>
 
 import blipnlptest as bnt
 
-cc = bnt.contentchecker(key, data=df)
+cc = bnt.contentchecker(key, data=df, contract_id="cliente_x")
 cc.identityanalysis()
 </code></pre>
 
 Se a análise for feita com dados que não foram analisados (envie um dataframe que a coluna de texto tenha o nome Text), use:
 
 <pre><code>
 import blipnlptest as bnt
```

### Comparing `blipnlptest-0.2.0/PKG-INFO` & `blipnlptest-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.2.0
+Version: 0.2.1
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,26 +35,27 @@
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
 - data (opcional) : Dataframe de entrada
 - resource (opcional) : Nome do recurso com o texto de tests
 - threshold (opcional) : float referente ao threshold do provedor com valores entre 0.1 (10%) a 1.0 (100%). (default: 0.5)
-- key : chave do bot.
+- key: chave do bot
+- contract_id: id do contrato.
 
 Exemplo do código:
 
 
 Caso a análise seja de dados já analisados pelo provedor (envie um dataframe que tenha no mínimo as colunas Text, Intentions, Entities e Score), use:
 
 <pre><code>
 
 import blipnlptest as bnt
 
-cc = bnt.contentchecker(key, data=df)
+cc = bnt.contentchecker(key, data=df, contract_id="cliente_x")
 cc.identityanalysis()
 </code></pre>
 
 Se a análise for feita com dados que não foram analisados (envie um dataframe que a coluna de texto tenha o nome Text), use:
 
 <pre><code>
 import blipnlptest as bnt
```

