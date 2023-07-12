# Comparing `tmp/skillsnetwork-authoring-extension-0.5.7.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.5.7rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork-authoring-extension-0.5.7.tar", last modified: Wed Jul 12 18:24:22 2023, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.5.7rc4.tar", last modified: Wed Jul 12 17:55:36 2023, max compression
```

## Comparing `skillsnetwork-authoring-extension-0.5.7.tar` & `skillsnetwork-authoring-extension-0.5.7rc4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 18:22:59.000000 skillsnetwork-authoring-extension-0.5.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:22:59.000000 skillsnetwork-authoring-extension-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 18:22:59.000000 skillsnetwork-authoring-extension-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-12 18:22:59.000000 skillsnetwork-authoring-extension-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 18:22:59.000000 skillsnetwork-authoring-extension-0.5.7/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.346242 skillsnetwork-authoring-extension-0.5.7/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/remoteEntry.014a9b1f9cac9a0a27bc.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 18:24:20.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.350242 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:23:36.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 18:24:22.000000 skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/src/button/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/src/menu/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:24:22.354242 skillsnetwork-authoring-extension-0.5.7/style/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 18:23:00.000000 skillsnetwork-authoring-extension-0.5.7/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   219982 2023-07-12 18:24:08.000000 skillsnetwork-authoring-extension-0.5.7/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.246301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/server-config/skillsnetwork_authoring_extension.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-12 17:54:03.000000 skillsnetwork-authoring-extension-0.5.7rc4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 17:55:33.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:54:45.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/button/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/button/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/dialog.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/menu/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/sn-file-library.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219982 2023-07-12 17:55:19.000000 skillsnetwork-authoring-extension-0.5.7rc4/yarn.lock
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/LICENSE` & `skillsnetwork-authoring-extension-0.5.7rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.7rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.7
+Version: 0.5.7rc4
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/README.md` & `skillsnetwork-authoring-extension-0.5.7rc4/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/RELEASE.md` & `skillsnetwork-authoring-extension-0.5.7rc4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/package.json` & `skillsnetwork-authoring-extension-0.5.7rc4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.5.7-rc4'"}*

```diff
@@ -107,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.7"
+    "version": "0.5.7-rc4"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/pyproject.toml` & `skillsnetwork-authoring-extension-0.5.7rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/setup.py` & `skillsnetwork-authoring-extension-0.5.7rc4/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767992424242423%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9e7c06ac94a6b92bf5ef.js'}}",*

 * * "'version'": "'0.5.7-rc4'"}*

```diff
@@ -55,15 +55,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.014a9b1f9cac9a0a27bc.js",
+            "load": "static/remoteEntry.9e7c06ac94a6b92bf5ef.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -112,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.7"
+    "version": "0.5.7-rc4"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/remoteEntry.014a9b1f9cac9a0a27bc.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -151,15 +151,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => j.e(669).then((() => () => j(9669))))), u("jwt-decode", "3.1.2", (() => j.e(245).then((() => () => j(6245))))), u("skillsnetwork-authoring-extension", "0.5.7", (() => j.e(568).then((() => () => j(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "0.21.4", (() => j.e(669).then((() => () => j(9669))))), u("jwt-decode", "3.1.2", (() => j.e(245).then((() => () => j(6245))))), u("skillsnetwork-authoring-extension", "0.5.7-rc4", (() => j.e(568).then((() => () => j(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.7
+Version: 0.5.7rc4
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
 skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
 skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
 skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
 skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.014a9b1f9cac9a0a27bc.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/button/index.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/button/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/button/sample.json` & `skillsnetwork-authoring-extension-0.5.7rc4/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/config.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/dialog.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/handler.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/src/tools.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/tools.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/tsconfig.json` & `skillsnetwork-authoring-extension-0.5.7rc4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7/yarn.lock` & `skillsnetwork-authoring-extension-0.5.7rc4/yarn.lock`

 * *Files identical despite different names*

