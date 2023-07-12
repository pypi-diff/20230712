# Comparing `tmp/voila-vuetify-template-tuwien-0.6.1.tar.gz` & `tmp/voila-vuetify-template-tuwien-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-template-tuwien-0.6.1.tar", last modified: Mon Jul 10 10:20:55 2023, max compression
+gzip compressed data, was "voila-vuetify-template-tuwien-0.6.2.tar", last modified: Wed Jul 12 08:23:31 2023, max compression
```

## Comparing `voila-vuetify-template-tuwien-0.6.1.tar` & `voila-vuetify-template-tuwien-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,40 @@
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/LICENSE
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/MANIFEST.in
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/README.md
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/setup.cfg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3303 2023-07-10 10:20:43.000000 voila-vuetify-template-tuwien-0.6.1/setup.py
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6381 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-10 10:18:15.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-07-10 10:19:21.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      828 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/requires.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.143580 voila-vuetify-template-tuwien-0.6.2/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/LICENSE
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/MANIFEST.in
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-12 08:23:31.143580 voila-vuetify-template-tuwien-0.6.2/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      720 2023-07-12 07:59:22.000000 voila-vuetify-template-tuwien-0.6.2/README.md
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-07-12 08:23:31.147580 voila-vuetify-template-tuwien-0.6.2/setup.cfg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3311 2023-07-12 08:23:24.000000 voila-vuetify-template-tuwien-0.6.2/setup.py
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.135579 voila-vuetify-template-tuwien-0.6.2/share/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.139579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.135579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.135579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.139579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.139579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     5875 2023-07-11 21:46:35.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.143580 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)    15256 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   174112 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)    18663 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/logo.svg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   141851 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   181109 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     5000 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/tu_alone_white.svg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     8936 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/voila_alone_white.svg
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.139579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.139579 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.143580 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3141 2023-07-11 11:40:37.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/base.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1766 2023-07-12 07:33:53.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1473 2023-07-11 11:40:00.000000 voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/tree.html
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 08:23:31.143580 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-12 08:23:31.000000 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1512 2023-07-12 08:23:31.000000 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-12 08:23:31.000000 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-12 08:23:31.000000 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-07-12 08:23:31.000000 voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/top_level.txt
```

### Comparing `voila-vuetify-template-tuwien-0.6.1/LICENSE` & `voila-vuetify-template-tuwien-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.1/setup.py` & `voila-vuetify-template-tuwien-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-template-tuwien',
-    version="0.6.1",
-    description="A vuetify template for Voila",
+    version="0.6.2",
+    description="A TU Wien vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5'],
     include_package_data=True,
     url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-vuetify-tu-wien-template',
     keywords=[
         'ipython',
         'jupyter',
```

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 {% raw -%}
+
+</style>
 <div id="app" style="display: none">
     <v-app>
         <v-slide-y-transition>
             <v-layout v-show="loading" align-center justify-center>
                 <v-card style="min-width: 600px">
                     <v-progress-linear
                             :indeterminate="loadingPercentage < 0"
@@ -18,49 +20,46 @@
         </v-slide-y-transition>
         <v-slide-y-transition>
             <v-layout v-show="!loading">
                 <v-navigation-drawer v-model="showNavBar" app>
                     <v-toolbar flat>
                         <v-list>
                             <v-list-item>
-                                <v-list-item-title class="title">
-                                    <jupyter-widget-mount-point mount-id="content-title">
-                                        Navigation
+                               <v-list-item-title class="title">
+                                    <jupyter-widget-mount-point mount-id="content-title" style="color: #006699;">
+                                        TU VoilaVuetify
                                     </jupyter-widget-mount-point>
-                                </v-list-item-title>
+                               </v-list-item-title>
                             </v-list-item>
                         </v-list>
                     </v-toolbar>
 
                     <v-divider></v-divider>
                     <jupyter-widget-mount-point mount-id="content-nav">
-                        <v-container>
-                            Placeholder for widget with mount id <i>content-nav</i>.
-                        </v-container>
                         <v-list dense class="pt-0">
                             <v-list-item v-for="item in items" :key="item.title" :href="item.url"
                                          target="_blank">
                                 <v-list-item-action>
                                     <v-icon>{{ item.icon }}</v-icon>
                                 </v-list-item-action>
 
                                 <v-list-item-content>
                                     <v-list-item-title>{{ item.title }}</v-list-item-title>
                                 </v-list-item-content>
                             </v-list-item>
                         </v-list>
                     </jupyter-widget-mount-point>
                 </v-navigation-drawer>
-                <v-app-bar app>
+                <v-app-bar style="background-color: #006699;" app>
                     <v-app-bar-nav-icon
                         v-if="!showNavBar"
                         @click.stop="showNavBar = !showNavBar">
                     </v-app-bar-nav-icon>
                     <jupyter-widget-mount-point mount-id="content-bar">
-                        <v-toolbar-title>{{ title }}</v-toolbar-title>
+                        <v-toolbar-title  style="color:white; font-weight: bold;">{{ title }}</v-toolbar-title>
                     </jupyter-widget-mount-point>
                 </v-app-bar>
 
                 <v-content>
                     <jupyter-widget-mount-point mount-id="content-main">
                             <v-container>
                                     Placeholder for widget with mount id <i>content-main</i>.
@@ -118,20 +117,16 @@
             loading_text: "Loading page",
             loadingPercentage: -1,
             showNavBar: null,
             loading: true,
             right: null,
             url: 'https://www.w3schools.com/',
             items: [
-                {icon: "dashboard", title: "voila", url: "https://github.com/voila-dashboards/voila"},
-                {icon: "touch_app", title: "voila-vuetify", url: "https://github.com/voila-dashboards/voila-vuetify"},
-                {icon: "web", title: "ipvuetify", url: "https://github.com/mariobuikhuizen/ipyvuetify"},
-                {icon: "web", title: "vuetify", url: "https://v15.vuetifyjs.com/en/"},
-                {icon: "widgets", title: "jupyter widgets", url: "https://github.com/jupyter-widgets/ipywidgets"},
-                {icon: "bar_chart", title: "bqplot", url: "https://github.com/bloomberg/bqplot/"},
+                {icon: "static/TU-logo.svg"},
+                {icon: "dashboard", title: "TU Wien Voilà gallery", url: "https://voila-gallery.jupyter.hpc.tuwien.ac.at/"}
             ],
             title: 'Voila vuetify',
             debug: false,
             voilaDebugMessages: [],
         }
     }
 });
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-template-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
         {
             "baseUrl": "{{resources.base_url}}",
             "kernelId": "{{kernel_id}}"
         }
     </script>
 {% endblock notebook_execute %}
 
+
+
 {% block cell_generator %}
     <script>
     app.title = "{{nb_title}}"
         
         var voila_process = function(cell_index, cell_count) {
             const loading_text = `Executing cell ${cell_index} of ${cell_count}`
             console.log(loading_text)
```

### Comparing `voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/SOURCES.txt` & `voila-vuetify-template-tuwien-0.6.2/voila_vuetify_template_tuwien.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,13 +6,22 @@
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
 share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
 share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/logo.svg
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/tu_alone_white.svg
+share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/voila_alone_white.svg
+share/jupyter/voila/templates/vuetify-base-tuwien/base.html
 share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+share/jupyter/voila/templates/vuetify-base-tuwien/tree.html
 voila_vuetify_template_tuwien.egg-info/PKG-INFO
 voila_vuetify_template_tuwien.egg-info/SOURCES.txt
 voila_vuetify_template_tuwien.egg-info/dependency_links.txt
 voila_vuetify_template_tuwien.egg-info/requires.txt
 voila_vuetify_template_tuwien.egg-info/top_level.txt
```

