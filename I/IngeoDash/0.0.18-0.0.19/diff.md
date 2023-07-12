# Comparing `tmp/IngeoDash-0.0.18.tar.gz` & `tmp/IngeoDash-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.18.tar", last modified: Wed Jul 12 19:23:53 2023, max compression
+gzip compressed data, was "IngeoDash-0.0.19.tar", last modified: Wed Jul 12 21:08:06 2023, max compression
```

## Comparing `IngeoDash-0.0.18.tar` & `IngeoDash-0.0.19.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:53.840925 IngeoDash-0.0.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:53.836925 IngeoDash-0.0.18/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:53.836925 IngeoDash-0.0.18/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/IngeoDash/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:53.836925 IngeoDash-0.0.18/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 19:23:53.000000 IngeoDash-0.0.18/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 19:23:53.000000 IngeoDash-0.0.18/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:23:53.000000 IngeoDash-0.0.18/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 19:23:53.000000 IngeoDash-0.0.18/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 19:23:53.000000 IngeoDash-0.0.18/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 19:23:53.840925 IngeoDash-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:23:53.840925 IngeoDash-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 19:21:58.000000 IngeoDash-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.790624 IngeoDash-0.0.19/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/setup.py
```

### Comparing `IngeoDash-0.0.18/IngeoDash/__init__.py` & `IngeoDash-0.0.19/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.18'
+__version__ = '0.0.19'
```

### Comparing `IngeoDash-0.0.18/IngeoDash/__main__.py` & `IngeoDash-0.0.19/IngeoDash/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.app import process_manager, download, progress
 from IngeoDash.config import CONFIG
 from IngeoDash.annotate import flip_label
+from EvoMSA.utils import MODEL_LANG
 from dash import dcc, Output, Input, callback, ctx, Dash, State, dash_table, html, Patch
 import dash_bootstrap_components as dbc
 
 
 @callback(
     Output('store', 'data'),
     Input(CONFIG.next, 'n_clicks'),
-    Input(CONFIG.upload, 'contents'),    
+    Input(CONFIG.upload, 'contents'),
+    State(CONFIG.lang, 'value'),
     State('store', 'data'),
     prevent_initial_call=True)
 def process_manager_callback(next,
                              content,
+                             lang,
                              mem):
     mem = CONFIG(mem)
     return process_manager(mem, ctx.triggered_id,
-                           next, content)
+                           next, content, lang)
 
 
 @callback(
     Output(CONFIG.center, 'children'),
     Input('store', 'data'),
     prevent_initial_call=True    
 )
@@ -81,34 +84,41 @@
           State('store', 'data'),
           prevent_initial_call=True)
 def download_callback(_, filename, mem):
     mem = CONFIG(mem)
     return download(mem, filename)
 
 
-if __name__ == '__main__':
+def run():
     app = Dash(external_stylesheets=[dbc.themes.BOOTSTRAP],
                suppress_callback_exceptions=True)
+    lang = dbc.Select(id=CONFIG.lang, value='es',
+                      options=[dict(label=x, value=x) for x in MODEL_LANG])
 
     download_grp = dbc.InputGroup([dbc.InputGroupText('Filename:'),
                                    dbc.Input(placeholder='output.json',
                                              value='output.json',
                                              type='text',
                                              id=CONFIG.filename),
                                    dbc.Button('Download',
                                               color='success',
                                               id=CONFIG.save)])
-    upload = dcc.Upload(id=CONFIG.upload, children=html.A('Upload'))
+    upload = dbc.InputGroup([lang, dcc.Upload(id=CONFIG.upload, 
+                                              children=dbc.Button('Upload'))])
     app.layout = dbc.Container([dcc.Loading(children=dcc.Store('store'),
                                             fullscreen=True), 
                                 dcc.Download(id=CONFIG.download),
                                 dbc.Row(dbc.Stack([dbc.Progress(value=0,
                                                                 id=CONFIG.progress),
                                                    html.Div(id=CONFIG.center,
                                                             children=create_table([{}])),
                                                    dbc.Button('Next', 
                                                               color='primary', 
                                                               id=CONFIG.next,
                                                               n_clicks=0)])),
                                 dbc.Row(download_grp),
                                 dbc.Row(upload)])
-    app.run_server(debug=True)
+    app.run_server(debug=True)
+
+
+if __name__ == '__main__':
+    run()
```

### Comparing `IngeoDash-0.0.18/IngeoDash/annotate.py` & `IngeoDash-0.0.19/IngeoDash/annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/IngeoDash/app.py` & `IngeoDash-0.0.19/IngeoDash/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     return [{'text': x['text']}
             for x in tweet_iterator(TWEETS) if x['klass'] in ['P', 'N']]
 
 
 def process_manager(mem,
                     triggered_id=None,
                     next=None,
-                    content=None):
+                    content=None,
+                    lang='es'):
     if triggered_id == mem.upload:
-        upload(mem, content)
+        upload(mem, content, lang=lang)
         return json.dumps(mem.mem)
     elif triggered_id == mem.next:
         store(mem)
         db = CONFIG.db[mem[mem.username]]
         init = mem[mem.n]
         data = db[mem.original]
         if len(data):
```

### Comparing `IngeoDash-0.0.18/IngeoDash/config.py` & `IngeoDash-0.0.19/IngeoDash/config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.0.19/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/IngeoDash/tests/test_app.py` & `IngeoDash-0.0.19/IngeoDash/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/IngeoDash/tests/test_config.py` & `IngeoDash-0.0.19/IngeoDash/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/LICENSE` & `IngeoDash-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/README.rst` & `IngeoDash-0.0.19/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.18/setup.py` & `IngeoDash-0.0.19/setup.py`

 * *Files identical despite different names*

