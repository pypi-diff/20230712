# Comparing `tmp/st_pandas_text_editor-0.0.2.tar.gz` & `tmp/st_pandas_text_editor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pandas_text_editor-0.0.2.tar", last modified: Tue Jul 11 10:02:39 2023, max compression
+gzip compressed data, was "st_pandas_text_editor-0.0.3.tar", last modified: Wed Jul 12 15:38:19 2023, max compression
```

## Comparing `st_pandas_text_editor-0.0.2.tar` & `st_pandas_text_editor-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,18 @@
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
+drwxrwxrwx   0        0        0        0 2023-07-12 15:38:19.962395 st_pandas_text_editor-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      287 2023-07-12 15:38:19.961265 st_pandas_text_editor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:38:19.962395 st_pandas_text_editor-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-07-12 15:38:00.000000 st_pandas_text_editor-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:38:19.923989 st_pandas_text_editor-0.0.3/st_pandas_text_editor/
+-rw-rw-rw-   0        0        0     5120 2023-07-12 15:37:56.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:38:19.900693 st_pandas_text_editor-0.0.3/st_pandas_text_editor/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:38:19.960269 st_pandas_text_editor-0.0.3/st_pandas_text_editor/frontend/build/
+-rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor/frontend/build/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-07-12 15:38:19.950775 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-12 15:38:19.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-12 15:38:19.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:38:19.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 15:38:19.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-12 15:38:19.000000 st_pandas_text_editor-0.0.3/st_pandas_text_editor.egg-info/top_level.txt
```

### Comparing `st_pandas_text_editor-0.0.2/LICENSE` & `st_pandas_text_editor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/README.md` & `st_pandas_text_editor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.2/setup.py` & `st_pandas_text_editor-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_pandas_text_editor",
-    version="0.0.2",
+    version="0.0.3",
     author="Elias",
     author_email="eli.mue@gmx.de",
     description="Rich Text Editor with customizable Dropdown Options for Streamlit",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/__init__.py` & `st_pandas_text_editor-0.0.3/st_pandas_text_editor/__init__.py`

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

### Comparing `st_pandas_text_editor-0.0.2/st_pandas_text_editor/frontend/build/bootstrap.min.css` & `st_pandas_text_editor-0.0.3/st_pandas_text_editor/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

