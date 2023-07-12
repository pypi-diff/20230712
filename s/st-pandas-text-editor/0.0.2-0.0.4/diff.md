# Comparing `tmp/st_pandas_text_editor-0.0.2.tar.gz` & `tmp/st_pandas_text_editor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pandas_text_editor-0.0.2.tar", last modified: Tue Jul 11 10:02:39 2023, max compression
+gzip compressed data, was "st_pandas_text_editor-0.0.4.tar", last modified: Wed Jul 12 15:48:32 2023, max compression
```

## Comparing `st_pandas_text_editor-0.0.2.tar` & `st_pandas_text_editor-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.867062 st_pandas_text_editor-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      287 2023-07-11 10:02:39.865732 st_pandas_text_editor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 10:02:39.867062 st_pandas_text_editor-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-07-11 10:01:48.000000 st_pandas_text_editor-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.523803 st_pandas_text_editor-0.0.2/st_pandas_text_editor/
--rw-rw-rw-   0        0        0     5088 2023-07-11 09:57:38.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.504650 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.581967 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/
--rw-rw-rw-   0        0        0     1078 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2232 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.505839 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.611569 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/
--rw-rw-rw-   0        0        0    17207 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
--rw-rw-rw-   0        0        0    30841 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
--rw-rw-rw-   0        0        0      348 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
--rw-rw-rw-   0        0        0      788 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.862958 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/
--rw-rw-rw-   0        0        0  1051761 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js
--rw-rw-rw-   0        0        0     2322 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  3774473 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map
--rw-rw-rw-   0        0        0     5245 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js
--rw-rw-rw-   0        0        0    15132 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-11 10:00:45.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:39.547005 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/
--rw-rw-rw-   0        0        0      287 2023-07-11 10:02:39.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-07-11 10:02:39.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:02:39.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 10:02:39.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-11 10:02:39.000000 st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:32.129812 st_pandas_text_editor-0.0.4/
+-rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      287 2023-07-12 15:48:32.129812 st_pandas_text_editor-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:48:32.131106 st_pandas_text_editor-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-07-12 15:46:13.000000 st_pandas_text_editor-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.888527 st_pandas_text_editor-0.0.4/st_pandas_text_editor/
+-rw-rw-rw-   0        0        0     5120 2023-07-12 15:42:32.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.879169 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.906899 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/
+-rw-rw-rw-   0        0        0     1078 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2232 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.880612 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.924185 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/
+-rw-rw-rw-   0        0        0    17207 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
+-rw-rw-rw-   0        0        0    30841 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
+-rw-rw-rw-   0        0        0      348 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
+-rw-rw-rw-   0        0        0      788 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:32.128633 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/
+-rw-rw-rw-   0        0        0  1051761 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js
+-rw-rw-rw-   0        0        0     2322 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  3774473 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map
+-rw-rw-rw-   0        0        0     5292 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js
+-rw-rw-rw-   0        0        0    15354 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.895428 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/top_level.txt
```

### Comparing `st_pandas_text_editor-0.0.2/LICENSE` & `st_pandas_text_editor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/README.md` & `st_pandas_text_editor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/setup.py` & `st_pandas_text_editor-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_pandas_text_editor",
-    version="0.0.2",
+    version="0.0.4",
     author="Elias",
     author_email="eli.mue@gmx.de",
     description="Rich Text Editor with customizable Dropdown Options for Streamlit",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/__init__.py` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,12 +110,13 @@
     # component instance. By default, when a component's arguments change,
     # it is considered a new instance and will be re-mounted on the frontend
     # and lose its current state. In this case, we want to vary the component's
     # "name" argument without having it get recreated.
     response = st_pandas_text_editor(
         columns=df.columns.tolist(), key="foo", placeholder="This is ...\n a story"
     )
-    st.button("Hello")
     if response:
+        print(response)
         st.write(response)
         # use eval to dynamically evaluate the string (unsafe --> minimze risks)
         st.write(eval(f'f"""{response[1]}"""'))
+        st.write(response[2])
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/asset-manifest.json` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/asset-manifest.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8958333333333333%*

 * *Differences: {"'entrypoints'": "{insert: [(4, 'static/js/main.baa131a3.chunk.js')], delete: [4]}",*

 * * "'files'": "{'main.js': './static/js/main.baa131a3.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.baa131a3.chunk.js.map'}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "entrypoints": [
         "static/js/runtime-main.624f085e.js",
         "static/css/2.9b7094a5.chunk.css",
         "static/js/2.ecfcc7a3.chunk.js",
         "static/css/main.c21eaae6.chunk.css",
-        "static/js/main.168a4d94.chunk.js"
+        "static/js/main.baa131a3.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.c21eaae6.chunk.css",
-        "main.js": "./static/js/main.168a4d94.chunk.js",
-        "main.js.map": "./static/js/main.168a4d94.chunk.js.map",
+        "main.js": "./static/js/main.baa131a3.chunk.js",
+        "main.js.map": "./static/js/main.baa131a3.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.624f085e.js",
         "runtime-main.js.map": "./static/js/runtime-main.624f085e.js.map",
         "static/css/2.9b7094a5.chunk.css": "./static/css/2.9b7094a5.chunk.css",
         "static/css/2.9b7094a5.chunk.css.map": "./static/css/2.9b7094a5.chunk.css.map",
         "static/css/main.c21eaae6.chunk.css.map": "./static/css/main.c21eaae6.chunk.css.map",
         "static/js/2.ecfcc7a3.chunk.js": "./static/js/2.ecfcc7a3.chunk.js",
         "static/js/2.ecfcc7a3.chunk.js.LICENSE.txt": "./static/js/2.ecfcc7a3.chunk.js.LICENSE.txt",
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/bootstrap.min.css` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/index.html` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.9b7094a5.chunk.css" rel="stylesheet"><link href="./static/css/main.c21eaae6.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.ecfcc7a3.chunk.js"></script><script src="./static/js/main.168a4d94.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.9b7094a5.chunk.css" rel="stylesheet"><link href="./static/css/main.c21eaae6.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.ecfcc7a3.chunk.js"></script><script src="./static/js/main.baa131a3.chunk.js"></script></body></html>
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -14,16 +14,16 @@
                 d = n(3),
                 u = n(45),
                 p = n(28),
                 b = n(109),
                 j = (n(215), n(216), n(22)),
                 h = n(110),
                 m = n.n(h),
-                v = n(7),
-                g = function(e) {
+                g = n(7),
+                v = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n() {
                         var e;
                         Object(i.a)(this, n);
                         for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
@@ -36,41 +36,41 @@
                         }, e
                     }
                     return Object(s.a)(n, [{
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = this.props.column;
-                            return Object(v.jsx)("div", {
+                            return Object(g.jsx)("div", {
                                 style: {
                                     padding: "0 3px"
                                 },
-                                children: Object(v.jsxs)(j.a, {
-                                    children: [Object(v.jsx)(j.a.Toggle, {
+                                children: Object(g.jsxs)(j.a, {
+                                    children: [Object(g.jsx)(j.a.Toggle, {
                                         variant: "primary",
                                         id: "dropdown-basic",
                                         children: "Select Variable"
-                                    }), Object(v.jsxs)(j.a.Menu, {
+                                    }), Object(g.jsxs)(j.a.Menu, {
                                         style: {
                                             maxHeight: "150px",
                                             overflowY: "auto",
                                             columnCount: 2
                                         },
-                                        children: [Object(v.jsx)("div", {
+                                        children: [Object(g.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 0 ? Object(v.jsx)(j.a.Item, {
+                                                return n % 2 === 0 ? Object(g.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
-                                        }), Object(v.jsx)("div", {
+                                        }), Object(g.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 1 ? Object(v.jsx)(j.a.Item, {
+                                                return n % 2 === 1 ? Object(g.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
                                         })]
@@ -97,41 +97,41 @@
                         }, e
                     }
                     return Object(s.a)(n, [{
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = this.props.agg;
-                            return Object(v.jsx)("div", {
+                            return Object(g.jsx)("div", {
                                 style: {
                                     padding: "0 3px"
                                 },
-                                children: Object(v.jsxs)(j.a, {
-                                    children: [Object(v.jsx)(j.a.Toggle, {
+                                children: Object(g.jsxs)(j.a, {
+                                    children: [Object(g.jsx)(j.a.Toggle, {
                                         variant: "primary",
                                         id: "dropdown-basic",
                                         children: "Select Aggregate"
-                                    }), Object(v.jsxs)(j.a.Menu, {
+                                    }), Object(g.jsxs)(j.a.Menu, {
                                         style: {
                                             maxHeight: "150px",
                                             overflowY: "auto",
                                             columnCount: 2
                                         },
-                                        children: [Object(v.jsx)("div", {
+                                        children: [Object(g.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 0 ? Object(v.jsx)(j.a.Item, {
+                                                return n % 2 === 0 ? Object(g.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
-                                        }), Object(v.jsx)("div", {
+                                        }), Object(g.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 1 ? Object(v.jsx)(j.a.Item, {
+                                                return n % 2 === 1 ? Object(g.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
                                         })]
@@ -149,16 +149,17 @@
                         var e;
                         Object(i.a)(this, n);
                         for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
                         return (e = t.call.apply(t, [this].concat(o))).state = {
                             isHovered: !1
                         }, e.onButtonClicked = function() {
                             var t = e.props.editorState,
-                                n = m()(Object(p.convertToRaw)(t.getCurrentContent()));
-                            u.a.setComponentValue([!0, n])
+                                n = m()(Object(p.convertToRaw)(t.getCurrentContent())),
+                                r = t.getCurrentContent().getPlainText("\x01");
+                            u.a.setComponentValue([!0, n, r])
                         }, e.handleMouseEnter = function() {
                             e.setState({
                                 isHovered: !0
                             })
                         }, e.handleMouseLeave = function() {
                             e.setState({
                                 isHovered: !1
@@ -173,19 +174,19 @@
                                     backgroundColor: "initial",
                                     color: e ? "#FF4B4B" : "black",
                                     border: "1px solid ".concat(e ? "red" : "#F0F2F6"),
                                     borderRadius: "5px",
                                     padding: "5px 8px",
                                     transition: "background-color 0.1s ease"
                                 };
-                            return Object(v.jsx)("div", {
+                            return Object(g.jsx)("div", {
                                 style: {
                                     marginTop: "10px"
                                 },
-                                children: Object(v.jsx)("button", {
+                                children: Object(g.jsx)("button", {
                                     style: t,
                                     onMouseEnter: this.handleMouseEnter,
                                     onMouseLeave: this.handleMouseLeave,
                                     onClick: this.onButtonClicked,
                                     children: "Confirm Text"
                                 })
                             })
@@ -228,27 +229,27 @@
                         key: "render",
                         value: function() {
                             var e = this.props.args,
                                 t = this.state.editorState,
                                 n = e.placeholder,
                                 r = e.columns,
                                 o = e.agg;
-                            return Object(v.jsxs)("div", {
+                            return Object(g.jsxs)("div", {
                                 style: {
                                     position: "relative"
                                 },
-                                children: [Object(v.jsx)(b.Editor, {
+                                children: [Object(g.jsx)(b.Editor, {
                                     editorState: t,
                                     onEditorStateChange: this.handleEditorChange,
                                     wrapperClassName: "wrapper-class",
                                     editorClassName: "editor-class",
                                     toolbarClassName: "toolbar-class",
-                                    toolbarCustomButtons: [Object(v.jsx)(g, {
+                                    toolbarCustomButtons: [Object(g.jsx)(v, {
                                         column: r
-                                    }), Object(v.jsx)(f, {
+                                    }), Object(g.jsx)(f, {
                                         agg: o
                                     })],
                                     placeholder: n,
                                     toolbar: {
                                         options: ["inline", "blockType", "colorPicker"],
                                         inline: {
                                             options: ["bold", "italic", "underline"],
@@ -270,25 +271,25 @@
                                         },
                                         colorPicker: {
                                             component: void 0,
                                             popupClassName: void 0,
                                             colors: ["rgb(0, 0, 0)", "rgb(255, 0, 0)", "rgb(0, 255, 0)", "rgb(0, 0, 255)", "rgb(255, 255, 0)", "rgb(255, 255, 255)"]
                                         }
                                     }
-                                }), Object(v.jsx)(O, {
+                                }), Object(g.jsx)(O, {
                                     editorState: t
                                 })]
                             })
                         }
                     }]), n
                 }(u.b),
                 C = Object(u.c)(x);
-            c.a.render(Object(v.jsx)(o.a.StrictMode, {
-                children: Object(v.jsx)(C, {})
+            c.a.render(Object(g.jsx)(o.a.StrictMode, {
+                children: Object(g.jsx)(C, {})
             }), document.getElementById("root"))
         }
     },
     [
         [218, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.168a4d94.chunk.js.map
+//# sourceMappingURL=main.baa131a3.chunk.js.map
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js.map` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8084656084656084%*

 * *Differences: {"'file'": "'static/js/main.baa131a3.chunk.js'",*

 * * "'mappings'": "'sTAeMA,EAAmB,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAgBrB,OAhBqBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KAOvBM,QAAU,SAACC,GACT,IAAAC,EAAkCb,EAAKc,MAA/BC,EAAWF,EAAXE,YAAaC,EAAQH,EAARG,SACfC,EAAeC,WAASC,YAC5BJ,EAAYK,oBACZL,EAAYM,eAAe,QAADX,OAClBE,EAAU,MAClBG,EAAYO,yBAEdN,EAASO,cAAYC,KAAKT,EAAaE,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.168a4d94.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.baa131a3.chunk.js",
+    "mappings": "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",
     "names": [
         "FirstDropdownOption",
         "_Component",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -74,14 +74,16 @@
         "_key3",
         "state",
         "isHovered",
         "onButtonClicked",
         "content",
         "draftToHtml",
         "convertToRaw",
+        "contentPlainText",
+        "getPlainText",
         "Streamlit",
         "setComponentValue",
         "handleMouseEnter",
         "setState",
         "handleMouseLeave",
         "buttonStyle",
         "backgroundColor",
@@ -138,12 +140,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "PandasTextEditor.js",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\";\r\nimport React, { Component } from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport { EditorState, Modifier, convertToRaw } from 'draft-js';\r\nimport { Editor } from 'react-draft-wysiwyg';\r\nimport \"react-draft-wysiwyg/dist/react-draft-wysiwyg.css\";\r\nimport './app.css';\r\nimport Dropdown from 'react-bootstrap/Dropdown';\r\nimport draftToHtml from \"draftjs-to-html\";\r\n\r\n// first choice dropdown\r\nclass FirstDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    column: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (columnName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `{df['${columnName}']`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { column } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Variable\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// second dropdown choice\r\nclass SecondDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    agg: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (aggName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `.${aggName}()}`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { agg } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Aggregate\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// my custom react button to emulate the streamlit button\r\nclass Button extends React.Component {\r\n  state = {\r\n    isHovered: false\r\n  };\r\n\r\n  onButtonClicked = () => {\r\n    const { editorState } = this.props;\r\n    const content = draftToHtml(convertToRaw(editorState.getCurrentContent()));\r\n    Streamlit.setComponentValue([true, content]);\r\n  };\r\n\r\n  handleMouseEnter = () => {\r\n    this.setState({ isHovered: true });\r\n  };\r\n\r\n  handleMouseLeave = () => {\r\n    this.setState({ isHovered: false });\r\n  };\r\n\r\n  render() {\r\n    const { isHovered } = this.state;\r\n    const buttonContainerStyle = {\r\n      marginTop: '10px', // Adjust the value as needed\r\n    };\r\n    const buttonStyle = {\r\n      backgroundColor: 'initial',\r\n      color: isHovered ? '#FF4B4B' : 'black',\r\n      border: `1px solid ${isHovered ? 'red' : '#F0F2F6'}`,\r\n      borderRadius: '5px',\r\n      padding: '5px 8px',\r\n      transition: 'background-color 0.1s ease',\r\n      // Add other styles here\r\n    };\r\n\r\n    return (\r\n      <div style={buttonContainerStyle}>\r\n        <button\r\n          style={buttonStyle}\r\n          onMouseEnter={this.handleMouseEnter}\r\n          onMouseLeave={this.handleMouseLeave}\r\n          onClick={this.onButtonClicked}\r\n        >\r\n          Confirm Text\r\n        </button>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// main component\r\nclass PandasTextEditor extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props);\r\n\r\n    this.state = {\r\n      numClicks: 0,\r\n      isFocused: false,\r\n      editorState: EditorState.createEmpty(), // Initialize the editor state\r\n    };\r\n  }\r\n\r\n  onClicked = () => {\r\n    this.setState(\r\n      (prevState) => ({ numClicks: prevState.numClicks + 1 }),\r\n      () => Streamlit.setComponentValue(this.state.numClicks)\r\n    );\r\n  };\r\n\r\n  onFocus = () => {\r\n    this.setState({ isFocused: true });\r\n  };\r\n\r\n  onBlur = () => {\r\n    this.setState({ isFocused: false });\r\n  };\r\n\r\n  handleEditorChange = (editorState) => {\r\n    this.setState({ editorState });\r\n  };\r\n\r\n  render() {\r\n    const { args } = this.props;\r\n    const { editorState } = this.state;\r\n    const placeholder = args[\"placeholder\"];\r\n\r\n    const columns = args[\"columns\"];\r\n    const agg = args[\"agg\"];\r\n\r\n    return (\r\n      <div style={{ position: \"relative\" }}>\r\n        <Editor\r\n          editorState={editorState}\r\n          onEditorStateChange={this.handleEditorChange}\r\n          wrapperClassName=\"wrapper-class\"\r\n          editorClassName=\"editor-class\"\r\n          toolbarClassName=\"toolbar-class\"\r\n          toolbarCustomButtons={[<FirstDropdownOption column={columns} />, <SecondDropdownOption agg={agg} />]}\r\n          placeholder={placeholder}\r\n          toolbar={{\r\n            options: ['inline', 'blockType', 'colorPicker'],\r\n            inline: {\r\n              options: ['bold', 'italic', 'underline'],\r\n              bold: { className: 'bordered-option-classname' },\r\n              italic: { className: 'bordered-option-classname' },\r\n              underline: { className: 'bordered-option-classname' },\r\n            },\r\n            blockType: {\r\n              inDropdown: true,\r\n              maxHeight: \"100px\", overflowY: \"auto\", columnCount: 2\r\n            },\r\n            colorPicker: {\r\n              component: undefined,\r\n              popupClassName: undefined,\r\n              colors: ['rgb(0, 0, 0)',\r\n                'rgb(255, 0, 0)',   // Red\r\n                'rgb(0, 255, 0)',   // Green\r\n                'rgb(0, 0, 255)',   // Blue\r\n                'rgb(255, 255, 0)', // Yellow\r\n                'rgb(255, 255, 255)']\r\n            }\r\n          }}\r\n        />\r\n        <Button editorState={editorState} />\r\n      </div>\r\n\r\n\r\n    );\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(PandasTextEditor);",
+        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\";\r\nimport React, { Component } from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport { EditorState, Modifier, convertToRaw } from 'draft-js';\r\nimport { Editor } from 'react-draft-wysiwyg';\r\nimport \"react-draft-wysiwyg/dist/react-draft-wysiwyg.css\";\r\nimport './app.css';\r\nimport Dropdown from 'react-bootstrap/Dropdown';\r\nimport draftToHtml from \"draftjs-to-html\";\r\n\r\n// first choice dropdown\r\nclass FirstDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    column: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (columnName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `{df['${columnName}']`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { column } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Variable\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// second dropdown choice\r\nclass SecondDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    agg: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (aggName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `.${aggName}()}`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { agg } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Aggregate\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// my custom react button to emulate the streamlit button\r\nclass Button extends React.Component {\r\n  state = {\r\n    isHovered: false\r\n  };\r\n\r\n  onButtonClicked = () => {\r\n    const { editorState } = this.props;\r\n    const content = draftToHtml(convertToRaw(editorState.getCurrentContent()));\r\n    const contentState = editorState.getCurrentContent()\r\n    const contentPlainText = contentState.getPlainText('\\u0001');\r\n    Streamlit.setComponentValue([true, content, contentPlainText]);\r\n  };\r\n\r\n  handleMouseEnter = () => {\r\n    this.setState({ isHovered: true });\r\n  };\r\n\r\n  handleMouseLeave = () => {\r\n    this.setState({ isHovered: false });\r\n  };\r\n\r\n  render() {\r\n    const { isHovered } = this.state;\r\n    const buttonContainerStyle = {\r\n      marginTop: '10px', // Adjust the value as needed\r\n    };\r\n    const buttonStyle = {\r\n      backgroundColor: 'initial',\r\n      color: isHovered ? '#FF4B4B' : 'black',\r\n      border: `1px solid ${isHovered ? 'red' : '#F0F2F6'}`,\r\n      borderRadius: '5px',\r\n      padding: '5px 8px',\r\n      transition: 'background-color 0.1s ease',\r\n      // Add other styles here\r\n    };\r\n\r\n    return (\r\n      <div style={buttonContainerStyle}>\r\n        <button\r\n          style={buttonStyle}\r\n          onMouseEnter={this.handleMouseEnter}\r\n          onMouseLeave={this.handleMouseLeave}\r\n          onClick={this.onButtonClicked}\r\n        >\r\n          Confirm Text\r\n        </button>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// main component\r\nclass PandasTextEditor extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props);\r\n\r\n    this.state = {\r\n      numClicks: 0,\r\n      isFocused: false,\r\n      editorState: EditorState.createEmpty(), // Initialize the editor state\r\n    };\r\n  }\r\n\r\n  onClicked = () => {\r\n    this.setState(\r\n      (prevState) => ({ numClicks: prevState.numClicks + 1 }),\r\n      () => Streamlit.setComponentValue(this.state.numClicks)\r\n    );\r\n  };\r\n\r\n  onFocus = () => {\r\n    this.setState({ isFocused: true });\r\n  };\r\n\r\n  onBlur = () => {\r\n    this.setState({ isFocused: false });\r\n  };\r\n\r\n  handleEditorChange = (editorState) => {\r\n    this.setState({ editorState });\r\n  };\r\n\r\n  render() {\r\n    const { args } = this.props;\r\n    const { editorState } = this.state;\r\n    const placeholder = args[\"placeholder\"];\r\n\r\n    const columns = args[\"columns\"];\r\n    const agg = args[\"agg\"];\r\n\r\n    return (\r\n      <div style={{ position: \"relative\" }}>\r\n        <Editor\r\n          editorState={editorState}\r\n          onEditorStateChange={this.handleEditorChange}\r\n          wrapperClassName=\"wrapper-class\"\r\n          editorClassName=\"editor-class\"\r\n          toolbarClassName=\"toolbar-class\"\r\n          toolbarCustomButtons={[<FirstDropdownOption column={columns} />, <SecondDropdownOption agg={agg} />]}\r\n          placeholder={placeholder}\r\n          toolbar={{\r\n            options: ['inline', 'blockType', 'colorPicker'],\r\n            inline: {\r\n              options: ['bold', 'italic', 'underline'],\r\n              bold: { className: 'bordered-option-classname' },\r\n              italic: { className: 'bordered-option-classname' },\r\n              underline: { className: 'bordered-option-classname' },\r\n            },\r\n            blockType: {\r\n              inDropdown: true,\r\n              maxHeight: \"100px\", overflowY: \"auto\", columnCount: 2\r\n            },\r\n            colorPicker: {\r\n              component: undefined,\r\n              popupClassName: undefined,\r\n              colors: ['rgb(0, 0, 0)',\r\n                'rgb(255, 0, 0)',   // Red\r\n                'rgb(0, 255, 0)',   // Green\r\n                'rgb(0, 0, 255)',   // Blue\r\n                'rgb(255, 255, 0)', // Yellow\r\n                'rgb(255, 255, 255)']\r\n            }\r\n          }}\r\n        />\r\n        <Button editorState={editorState} />\r\n      </div>\r\n\r\n\r\n    );\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(PandasTextEditor);",
         "import React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport PandasTextEditor from \"./PandasTextEditor\"\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <PandasTextEditor />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor.egg-info/SOURCES.txt` & `st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
 st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
 st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
 st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
 st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js
 st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt
 st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map
-st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js
-st_pandas_text_editor/frontend/build/static/js/main.168a4d94.chunk.js.map
+st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js
+st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map
 st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
 st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
```

