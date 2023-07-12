# Comparing `tmp/skillsnetwork-authoring-extension-0.5.6rc1.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.5.7rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork-authoring-extension-0.5.6rc1.tar", last modified: Wed Apr 19 14:41:47 2023, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.5.7rc4.tar", last modified: Wed Jul 12 17:55:36 2023, max compression
```

## Comparing `skillsnetwork-authoring-extension-0.5.6rc1.tar` & `skillsnetwork-authoring-extension-0.5.7rc4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.738331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-19 14:40:32.000000 skillsnetwork-authoring-extension-0.5.6rc1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 14:41:45.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:04.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/button/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/style/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   218440 2023-04-19 14:41:34.000000 skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock
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

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/LICENSE` & `skillsnetwork-authoring-extension-0.5.7rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.7rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.6rc1
+Version: 0.5.7rc4
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/README.md` & `skillsnetwork-authoring-extension-0.5.7rc4/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/RELEASE.md` & `skillsnetwork-authoring-extension-0.5.7rc4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/package.json` & `skillsnetwork-authoring-extension-0.5.7rc4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9299242424242425%*

 * *Differences: {"'dependencies'": "{'jwt-decode': '^3.1.2'}",*

 * * "'resolutions'": "OrderedDict([('@lumino/widgets', '1.37.2')])",*

 * * "'version'": "'0.5.7-rc4'"}*

```diff
@@ -13,15 +13,16 @@
         "@jupyterlab/docregistry": "^3.3.0",
         "@jupyterlab/mainmenu": "^3.4.2",
         "@jupyterlab/nbformat": "^3.3.3",
         "@jupyterlab/notebook": "^3.3.0",
         "@jupyterlab/services": "^6.4.3",
         "@lumino/disposable": "^1.4.3",
         "axios": "^0.21.2",
-        "buffer": "^6.0.3"
+        "buffer": "^6.0.3",
+        "jwt-decode": "^3.1.2"
     },
     "description": "JupyterLab/JupyterLite extension for Skills Network Authoring",
     "devDependencies": {
         "@jupyterlab/builder": "^3.3.0",
         "@types/node": "^17.0.29",
         "@types/signale": "^1.4.4",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
@@ -71,14 +72,17 @@
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/ibm-skills-network/skillsnetwork-authoring-extension.git"
     },
+    "resolutions": {
+        "@lumino/widgets": "1.37.2"
+    },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
@@ -103,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.6-rc1"
+    "version": "0.5.7-rc4"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml` & `skillsnetwork-authoring-extension-0.5.7rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/setup.py` & `skillsnetwork-authoring-extension-0.5.7rc4/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,19 @@
         help="The base URL for the lab file version management service (AKA Atlas)"
   )
   sn_file_library_url = Unicode(
         default_value=os.environ.get("SN_FILE_LIBRARY_URL", "https://author-ide.skills.network/file-library"),
         config=True,
         help="The URL for the sn-file-library ui"
   )
-
+  awb_base_url = Unicode(
+        default_value=os.environ.get("AWB_BASE_URL", "https://author.skills.network"),
+        config=True,
+        help="The URL for Author Workbench"
+  )
 
 def _load_jupyter_server_extension(server_app):
     """Registers the API handler to receive HTTP requests from the frontend extension.
     Parameters
     ----------
     server_app: jupyterlab.labapp.LabApp
         JupyterLab application instance
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   """
   Route handler for the /skillsnetwork-authoring-extension/config endpoint.
 
   A single endpoint that returns the Atlas base URL.
   """
   def get(self) -> None:
     print('test', type(self.config))
-    self.finish({"ATLAS_BASE_URL": self.config.atlas_base_url, "SN_FILE_LIBRARY_URL": self.config.sn_file_library_url})
+    self.finish({"ATLAS_BASE_URL": self.config.atlas_base_url, "SN_FILE_LIBRARY_URL": self.config.sn_file_library_url, "AWB_BASE_URL": self.config.awb_base_url})
 
 
 def setup_handlers(web_app, url_path: str) -> None:
   """Setup handlers in the jupyter server web app.
 
   Args:
     - web_app: Jupyter server web application instance to add handlers to.
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9294507575757577%*

 * *Differences: {"'dependencies'": "{'jwt-decode': '^3.1.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9e7c06ac94a6b92bf5ef.js'}}",*

 * * "'resolutions'": "OrderedDict([('@lumino/widgets', '1.37.2')])",*

 * * "'version'": "'0.5.7-rc4'"}*

```diff
@@ -13,15 +13,16 @@
         "@jupyterlab/docregistry": "^3.3.0",
         "@jupyterlab/mainmenu": "^3.4.2",
         "@jupyterlab/nbformat": "^3.3.3",
         "@jupyterlab/notebook": "^3.3.0",
         "@jupyterlab/services": "^6.4.3",
         "@lumino/disposable": "^1.4.3",
         "axios": "^0.21.2",
-        "buffer": "^6.0.3"
+        "buffer": "^6.0.3",
+        "jwt-decode": "^3.1.2"
     },
     "description": "JupyterLab/JupyterLite extension for Skills Network Authoring",
     "devDependencies": {
         "@jupyterlab/builder": "^3.3.0",
         "@types/node": "^17.0.29",
         "@types/signale": "^1.4.4",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
@@ -54,15 +55,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1ebb17cfc896e2585599.js",
+            "load": "static/remoteEntry.9e7c06ac94a6b92bf5ef.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -76,14 +77,17 @@
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/ibm-skills-network/skillsnetwork-authoring-extension.git"
     },
+    "resolutions": {
+        "@lumino/widgets": "1.37.2"
+    },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
@@ -108,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.6-rc1"
+    "version": "0.5.7-rc4"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,190 +1,217 @@
 "use strict";
 (self.webpackChunkskillsnetwork_authoring_extension = self.webpackChunkskillsnetwork_authoring_extension || []).push([
     [568], {
         7953: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        Z: () => m
+                        Z: () => _
                     });
-                    var a = o(7986),
-                        l = o(3033),
-                        i = o(5923),
-                        s = o(5344),
+                    var a = o(931),
+                        i = o(6303),
+                        l = o(5923),
+                        s = o(8535),
                         r = o(8623),
                         c = o(3311),
                         u = o(6973),
                         d = o(3619),
-                        h = o(1123),
-                        b = o(5449),
-                        w = t([d, r, c, b]);
-                    [d, r, c, b] = w.then ? (await w)() : w;
-                    const p = {
-                        activate: g,
+                        h = o(3191),
+                        b = o.n(h),
+                        w = o(127),
+                        p = o(5449),
+                        g = t([d, r, c, p]);
+                    [d, r, c, p] = g.then ? (await g)() : g;
+                    const y = {
+                        activate: f,
                         id: "skillsnetwork-authoring-extension:plugin",
                         autoStart: !0,
-                        requires: [s.IMainMenu, h.INotebookTracker, a.IDocumentManager]
+                        requires: [s.IMainMenu, w.INotebookTracker, a.IDocumentManager]
                     };
-                    class y {
+                    class m {
                         createNew(t, e) {
-                            if (d.OH.SHOW_PUBLISH_BUTTON_FOR !== e.path) return new i.DisposableDelegate((() => {})); {
+                            if (d.OH.SHOW_PUBLISH_BUTTON_FOR !== e.path) return new l.DisposableDelegate((() => {})); {
                                 const o = async () => {
                                     const o = await (0, r.nu)(t, e),
                                         n = d.OH.TOKENS.get(t.id);
-                                    void 0 !== n ? (0, c.nK)((0, c.SJ)(n), o) : console.log("No atlas token found for id", t.id)
+                                    void 0 !== n ? "version_id" in b()(n) ? (0, c.Wk)((0, c.So)(n), o, n) : (0, c.nK)((0, c.SJ)(n), o) : console.log("No atlas or awb token found for id", t.id)
                                 }, n = async () => {
                                     const o = await (0, r.nu)(t, e),
                                         n = new Blob([o], {
                                             type: "application/x-ipynb+json"
                                         }),
                                         a = URL.createObjectURL(n),
-                                        l = document.createElement("a");
-                                    l.setAttribute("download", e.path), l.setAttribute("href", a), document.body.appendChild(l), l.click(), document.body.removeChild(l), URL.revokeObjectURL(a)
-                                }, a = new l.ToolbarButton({
+                                        i = document.createElement("a");
+                                    i.setAttribute("download", e.path), i.setAttribute("href", a), document.body.appendChild(i), i.click(), document.body.removeChild(i), URL.revokeObjectURL(a)
+                                }, a = new i.ToolbarButton({
                                     className: "download-lab-button",
-                                    label: "Download",
+                                    label: "Download Notebook",
                                     onClick: n,
-                                    tooltip: "Download Lab"
-                                }), s = new l.ToolbarButton({
+                                    tooltip: "Download the current notebook ipynb file to your local system"
+                                }), s = new i.ToolbarButton({
                                     className: "publish-lab-button",
                                     label: "Publish on SN",
                                     onClick: o,
                                     tooltip: "Publish Lab"
-                                }), u = new l.ToolbarButton({
+                                }), u = new i.ToolbarButton({
                                     className: "sn-file-library-button",
                                     label: "SN File Library",
-                                    onClick: () => new b.E(t.id).launch(),
+                                    onClick: () => new p.E(t.id).launch(),
                                     tooltip: "Skills Network File Library"
                                 });
-                                return t.toolbar.insertItem(8, "download", a), t.toolbar.insertItem(9, "sn-file-library", u), t.toolbar.insertItem(10, "publish", s), new i.DisposableDelegate((() => {
+                                return t.toolbar.insertItem(8, "download", a), t.toolbar.insertItem(9, "sn-file-library", u), t.toolbar.insertItem(10, "publish", s), new l.DisposableDelegate((() => {
                                     a.dispose(), s.dispose(), u.dispose()
                                 }))
                             }
                         }
                     }
-                    async function g(t, e, o, n) {
+                    async function f(t, e, o, n) {
                         if (console.log("Activated skillsnetwork-authoring-extension button plugin!"), "learn" == await (0, d.IK)()) return;
                         const a = await (0, d.Nz)(),
-                            i = await (0, d.D2)();
-                        console.log("Using default kernel: ", d.OH.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new y), t.restored.then((async () => {
-                            if ("NO_TOKEN" !== a && "local" !== i) try {
+                            l = await (0, d.fe)(),
+                            s = await (0, d.D2)();
+                        console.log("Using default kernel: ", d.OH.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new m), t.restored.then((async () => {
+                            if ("NO_TOKEN" !== a && "local" !== s) try {
                                 await (0, r._Y)(a, n)
                             } catch (t) {
-                                l.Dialog.flush(), (0, u.YZ)(), console.log(t)
+                                i.Dialog.flush(), (0, u.YZ)(), console.log(t)
+                            } else if ("NO_TOKEN" !== l && "local" !== s) try {
+                                await (0, r.Ps)(l, n)
+                            } catch (t) {
+                                i.Dialog.flush(), (0, u.YZ)(), console.log(t)
                             }
                         }))
                     }
-                    const m = p;
+                    const _ = y;
                     n()
-                } catch (f) {
-                    n(f)
+                } catch (k) {
+                    n(k)
                 }
             }))
         },
         3619: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        CC: () => i,
-                        D2: () => c,
-                        IK: () => s,
-                        Nz: () => r,
-                        OH: () => d,
-                        XM: () => l
+                        CC: () => s,
+                        D2: () => d,
+                        DO: () => l,
+                        IK: () => r,
+                        Nz: () => c,
+                        OH: () => b,
+                        XM: () => i,
+                        fe: () => u
                     });
-                    var a = o(8820);
+                    var a = o(5139);
                     const t = t => {
                             let e = t.baseUrl;
                             return e.endsWith("/") || (e += "/"), e
                         },
-                        l = await (async () => {
+                        i = await (async () => {
                             const e = window.location.href,
                                 o = new URL(e).searchParams.get("atlas_base_url");
                             if (null === o) {
                                 const e = {
                                         method: "GET"
                                     },
                                     o = a.ServerConnection.makeSettings(),
                                     n = t(o) + "skillsnetwork-authoring-extension/config",
-                                    l = await a.ServerConnection.makeRequest(n, e, o);
-                                return (await l.json()).ATLAS_BASE_URL
+                                    i = await a.ServerConnection.makeRequest(n, e, o);
+                                return (await i.json()).ATLAS_BASE_URL
                             }
                             return decodeURIComponent(o)
                         })(),
-                        i = await (async () => {
+                        l = await (async () => {
+                            const e = window.location.href,
+                                o = new URL(e).searchParams.get("awb_base_url");
+                            if (null === o) {
+                                const e = {
+                                        method: "GET"
+                                    },
+                                    o = a.ServerConnection.makeSettings(),
+                                    n = t(o) + "skillsnetwork-authoring-extension/config",
+                                    i = await a.ServerConnection.makeRequest(n, e, o);
+                                return (await i.json()).AWB_BASE_URL
+                            }
+                            return decodeURIComponent(o)
+                        })(),
+                        s = await (async () => {
                             const e = window.location.href,
                                 o = new URL(e).searchParams.get("sn_file_library_url");
                             if (null === o) {
                                 const e = {
                                         method: "GET"
                                     },
                                     o = a.ServerConnection.makeSettings(),
                                     n = t(o) + "skillsnetwork-authoring-extension/config",
-                                    l = await a.ServerConnection.makeRequest(n, e, o);
-                                return (await l.json()).SN_FILE_LIBRARY_URL
+                                    i = await a.ServerConnection.makeRequest(n, e, o);
+                                return (await i.json()).SN_FILE_LIBRARY_URL
                             }
                             return decodeURIComponent(o)
                         })(),
-                        s = async () => {
+                        r = async () => {
                             const t = window.location.href;
                             let e = new URL(t).searchParams.get("mode");
                             return "learn" == e ? e : "author"
-                        }, r = async () => {
+                        }, c = async () => {
                             const t = window.location.href,
                                 e = new URL(t).searchParams.get("atlas_token");
                             return null !== e ? e : "NO_TOKEN"
-                        }, c = async () => {
+                        }, u = async () => {
+                            const t = window.location.href,
+                                e = new URL(t).searchParams.get("awb_token");
+                            return null !== e ? e : "NO_TOKEN"
+                        }, d = async () => {
                             const t = window.location.href;
                             let e = new URL(t).searchParams.get("env_type");
-                            return "jupyterlab" !== e && "jupyterlite" !== e && (e = "local"), console.log("Env type: ", e), "jupyterlab" === e || "local" === e ? (d.PY_KERNEL_NAME = await u(), d.DEFAULT_LAB_NAME = "lab.ipynb") : "jupyterlite" === e && (d.PY_KERNEL_NAME = "python", d.DEFAULT_LAB_NAME = "lab.jupyterlite.ipynb"), e
-                        }, u = async () => {
+                            return "jupyterlab" !== e && "jupyterlite" !== e && (e = "local"), console.log("Env type: ", e), "jupyterlab" === e || "local" === e ? (b.PY_KERNEL_NAME = await h(), b.DEFAULT_LAB_NAME = "lab.ipynb") : "jupyterlite" === e && (b.PY_KERNEL_NAME = "python", b.DEFAULT_LAB_NAME = "lab.jupyterlite.ipynb"), e
+                        }, h = async () => {
                             let t = await (await a.KernelSpecAPI.getSpecs()).kernelspecs,
                                 e = Object.keys(t).filter((function(t) {
                                     return t.includes("python")
                                 })).sort();
                             return e[e.length - 1]
                         };
-                    class d {}
-                    d.TOKENS = new Map, d.SHOW_PUBLISH_BUTTON_FOR = void 0, n()
+                    class b {}
+                    b.TOKENS = new Map, b.SHOW_PUBLISH_BUTTON_FOR = void 0, n()
                 } catch (t) {
                     n(t)
                 }
             }), 1)
         },
         6973: (t, e, o) => {
             o.d(e, {
-                Up: () => i,
+                Up: () => l,
                 YZ: () => d,
                 fP: () => u,
                 ql: () => r,
                 wW: () => c,
                 wj: () => s
             });
             var n = o(8832),
-                a = o(3033);
-            class l extends n.Widget {
+                a = o(6303);
+            class i extends n.Widget {
                 constructor() {
                     const t = document.createElement("div"),
                         e = new a.Spinner;
                     t.appendChild(e.node), t.style.padding = "15px", super({
                         node: t
                     })
                 }
             }
-            const i = t => {
-                    const e = new l;
+            const l = t => {
+                    const e = new i;
                     (0, a.showDialog)({
                         title: t,
                         body: e,
                         buttons: [a.Dialog.cancelButton()]
                     })
                 },
                 s = t => {
-                    const e = new l;
+                    const e = new i;
                     return (0, a.showDialog)({
                         title: t,
                         body: e,
                         buttons: []
                     })
                 },
                 r = t => (0, a.showDialog)({
@@ -216,45 +243,87 @@
                     }).then((t => {})).catch((t => {}))
                 }
         },
         3311: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        B4: () => d,
-                        SJ: () => u,
-                        nK: () => h
+                        B4: () => g,
+                        RZ: () => w,
+                        SJ: () => h,
+                        So: () => b,
+                        Wk: () => p,
+                        nK: () => y
                     });
                     var a = o(6973),
-                        l = o(3033),
-                        i = o(3619),
+                        i = o(6303),
+                        l = o(3619),
                         s = o(9581),
                         r = o.n(s),
-                        c = t([i]);
-                    i = (c.then ? (await c)() : c)[0];
-                    const u = t => r().create({
-                            baseURL: i.XM,
+                        c = o(3191),
+                        u = o.n(c),
+                        d = t([l]);
+                    l = (d.then ? (await d)() : d)[0];
+                    const h = t => r().create({
+                            baseURL: l.XM,
                             headers: {
                                 Authorization: `Bearer ${t}`,
                                 "Content-Type": "application/json",
                                 "Access-Control-Allow-Origin": "*",
                                 Accept: "application/json"
                             }
                         }),
-                        d = t => t.get("v1/labs").then((t => (l.Dialog.flush(), t.data))).catch((t => {
+                        b = t => r().create({
+                            baseURL: l.DO,
+                            headers: {
+                                Authorization: `Bearer ${t}`,
+                                "Content-Type": "application/json",
+                                "Access-Control-Allow-Origin": "*",
+                                Accept: "application/json"
+                            }
+                        }),
+                        w = async (t, e) => {
+                            try {
+                                const o = u()(e),
+                                    n = o.version_id,
+                                    a = o.lab_id,
+                                    l = await t.get(`api/v1/labs/${a}`).then((t => `${t.data.name}.ipynb`)),
+                                    s = await t.get(`api/v1/labs/${a}/lab_versions/${n}/download`).then((t => t.data));
+                                return i.Dialog.flush(), {
+                                    labFilename: l,
+                                    body: s
+                                }
+                            } catch (t) {
+                                throw console.log(t), "Failed to fetch notebook"
+                            }
+                        }, p = async (t, e, o) => {
+                            if (!await (0, a.ql)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return;
+                            (0, a.wj)("Publishing your changes...");
+                            const n = u()(o),
+                                l = n.version_id,
+                                s = n.lab_id;
+                            return new Promise((async (o, n) => {
+                                await t.patch(`api/v1/labs/${s}/lab_versions/${l}/update_source_file`, {
+                                    file: e
+                                }).then((t => {
+                                    console.log("SUCCESSFULLY PUSHED", t), i.Dialog.flush(), (0, a.wW)()
+                                })).catch((t => {
+                                    console.log(t), i.Dialog.flush(), (0, a.fP)()
+                                }))
+                            }))
+                        }, g = t => t.get("v1/labs").then((t => (i.Dialog.flush(), t.data))).catch((t => {
                             throw console.log(t), "Failed to fetch notebook"
-                        })),
-                        h = async (t, e) => {
+                        })), y = async (t, e) => {
                             if (await (0, a.ql)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return (0, a.wj)("Publishing your changes..."), new Promise((async (o, n) => {
                                 await t.post("v1/labs", {
                                     body: e
                                 }).then((t => {
-                                    console.log("SUCCESSFULLY PUSHED", t), l.Dialog.flush(), (0, a.wW)()
+                                    console.log("SUCCESSFULLY PUSHED", t), i.Dialog.flush(), (0, a.wW)()
                                 })).catch((t => {
-                                    console.log(t), l.Dialog.flush(), (0, a.fP)()
+                                    console.log(t), i.Dialog.flush(), (0, a.fP)()
                                 }))
                             }))
                         };
                     n()
                 } catch (t) {
                     n(t)
                 }
@@ -263,153 +332,159 @@
         1568: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.r(e), o.d(e, {
                         default: () => s
                     });
                     var a = o(4822),
-                        l = o(7953),
-                        i = t([l, a]);
-                    [l, a] = i.then ? (await i)() : i;
-                    const s = [l.Z, a.G];
+                        i = o(7953),
+                        l = t([i, a]);
+                    [i, a] = l.then ? (await l)() : l;
+                    const s = [i.Z, a.G];
                     n()
                 } catch (t) {
                     n(t)
                 }
             }))
         },
         4822: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        G: () => b
+                        G: () => p
                     });
-                    var a = o(5344),
-                        l = o(8832),
-                        i = o(3033),
-                        s = o(1123),
-                        r = o(7986),
+                    var a = o(8535),
+                        i = o(8832),
+                        l = o(6303),
+                        s = o(127),
+                        r = o(931),
                         c = o(6973),
                         u = o(3619),
                         d = o(8623),
-                        h = t([u, d]);
-                    [u, d] = h.then ? (await h)() : h;
-                    const b = {
+                        h = o(3191),
+                        b = o.n(h),
+                        w = t([u, d]);
+                    [u, d] = w.then ? (await w)() : w;
+                    const p = {
                         id: "skillsnetwork-authoring-extension:menu",
                         autoStart: !0,
                         requires: [a.IMainMenu, s.INotebookTracker, r.IDocumentManager],
                         activate: async (t, e, o, n) => {
                             if (console.log("Activated skillsnetwork-authoring-extension menu plugin!"), "learn" == await (0, u.IK)()) return;
                             const a = "edit-lab-from-token";
                             t.commands.addCommand(a, {
                                 label: "Edit a Lab",
                                 execute: () => {
                                     h(o, n)
                                 }
                             });
                             const {
                                 commands: s
-                            } = t, r = new l.Menu({
+                            } = t, r = new i.Menu({
                                 commands: s
                             });
                             r.title.label = "Skills Network", e.addMenu(r, {
                                 rank: 80
                             }), r.addItem({
                                 command: a,
                                 args: {}
                             });
                             const h = (t, e) => {
                                 let o = document.createElement("div"),
                                     n = document.createElement("label");
-                                n.textContent = "Enter your authorization token: ";
+                                n.textContent = "Enter your authorization token";
                                 let a = document.createElement("input");
-                                a.className = "jp-mod-styled", o.appendChild(n), o.appendChild(a), (0, i.showDialog)({
+                                a.className = "jp-mod-styled", o.appendChild(n), o.appendChild(a), (0, l.showDialog)({
                                     title: "Edit a Lab",
-                                    body: new l.Widget({
+                                    body: new i.Widget({
                                         node: o
                                     }),
-                                    buttons: [i.Dialog.cancelButton(), i.Dialog.okButton()]
+                                    buttons: [l.Dialog.cancelButton(), l.Dialog.okButton()]
                                 }).then((async t => {
                                     if (t.button.accept) {
                                         (0, c.Up)("Loading up your lab...");
                                         const t = a.value;
-                                        await (0, d._Y)(t, e)
+                                        "version_id" in b()(t) ? await (0, d.Ps)(t, e) : await (0, d._Y)(t, e)
                                     }
                                 })).catch((t => {
-                                    i.Dialog.flush(), (0, c.YZ)(), console.log(t)
+                                    l.Dialog.flush(), (0, c.YZ)(), console.log(t)
                                 }))
                             }
                         }
                     };
                     n()
                 } catch (t) {
                     n(t)
                 }
             }))
         },
         5449: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        E: () => d
+                        E: () => b
                     });
                     var a = o(8832),
-                        l = o(3033),
-                        i = o(3619),
-                        s = t([i]);
-                    i = (s.then ? (await s)() : s)[0];
-                    var r, c = function(t, e) {
+                        i = o(6303),
+                        l = o(3619),
+                        s = o(3191),
+                        r = o.n(s),
+                        c = t([l]);
+                    l = (c.then ? (await c)() : c)[0];
+                    var u, d = function(t, e) {
                         if (!e.has(t)) throw new TypeError("attempted to get private field on non-instance");
                         return e.get(t)
                     };
-                    class u extends a.Widget {
+                    class h extends a.Widget {
                         constructor(t) {
-                            const e = document.createElement("iframe");
-                            e.src = `${i.CC}?atlas_token=${i.OH.TOKENS.get(t)}`, e.setAttribute("frameborder", "0"), e.setAttribute("allow", "clipboard-read; clipboard-write"), e.classList.add("sn-file-library-frame"), super({
+                            const e = document.createElement("iframe"),
+                                o = l.OH.TOKENS.get(t);
+                            "project_id" in (o ? r()(o) : {}) && (e.src = `${l.CC}?atlas_token=${o}`), e.setAttribute("frameborder", "0"), e.setAttribute("allow", "clipboard-read; clipboard-write"), e.classList.add("sn-file-library-frame"), super({
                                 node: e
                             })
                         }
                     }
-                    class d {
+                    class b {
                         constructor(t) {
-                            r.set(this, void 0),
+                            u.set(this, void 0),
                                 function(t, e, o) {
                                     if (!e.has(t)) throw new TypeError("attempted to set private field on non-instance");
                                     e.set(t, o)
-                                }(this, r, t)
+                                }(this, u, t)
                         }
                         launch() {
-                            const t = new l.Dialog({
+                            const t = new i.Dialog({
                                     title: "Skills Network File Library",
-                                    body: new u(c(this, r)),
+                                    body: new h(d(this, u)),
                                     hasClose: !0,
                                     buttons: []
                                 }),
                                 e = t.node.querySelector(".jp-Dialog-content");
                             e && e.classList.add("sn-file-library-dialog"), t.launch()
                         }
                     }
-                    r = new WeakMap, n()
+                    u = new WeakMap, n()
                 } catch (t) {
                     n(t)
                 }
             }))
         },
         8623: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        _Y: () => u,
+                        Ps: () => u,
+                        _Y: () => d,
                         nu: () => c
                     });
-                    var a = o(1123),
-                        l = o(3619),
-                        i = o(3311),
-                        s = t([i, l]);
-                    [i, l] = s.then ? (await s)() : s;
+                    var a = o(127),
+                        i = o(3619),
+                        l = o(3311),
+                        s = t([l, i]);
+                    [l, i] = s.then ? (await s)() : s;
                     const r = t => ({
                             cell_type: t.model.type,
                             id: t.model.id,
                             metadata: {},
                             outputs: [],
                             source: [t.model.value.text]
                         }),
@@ -417,39 +492,50 @@
                             const o = [];
                             t.content.widgets.forEach((t => {
                                 const e = r(t);
                                 o.push(e)
                             }));
                             const n = e.model.metadata.toJSON(),
                                 a = e.model.nbformat,
-                                l = e.model.nbformatMinor,
-                                i = {
+                                i = e.model.nbformatMinor,
+                                l = {
                                     cells: o,
                                     metadata: n,
                                     nbformat: a,
-                                    nbformat_minor: l
+                                    nbformat_minor: i
                                 };
-                            return JSON.stringify(i, null, 2)
+                            return JSON.stringify(l, null, 2)
                         },
                         u = async (t, e) => {
                             let {
+                                labFilename: o,
+                                body: n
+                            } = await (0, l.RZ)((0, l.So)(t), t);
+                            i.OH.SHOW_PUBLISH_BUTTON_FOR = o;
+                            const a = e.createNew(o, "notebook", {
+                                name: i.OH.PY_KERNEL_NAME
+                            });
+                            if (i.OH.SHOW_PUBLISH_BUTTON_FOR = void 0, i.OH.TOKENS.set(a.id, t), void 0 === a) throw Error("Error loading lab");
+                            return h(a, n), a
+                        }, d = async (t, e) => {
+                            let {
                                 instructions_file_path: o,
                                 body: n
-                            } = await (0, i.B4)((0, i.SJ)(t));
-                            const a = h(o);
-                            l.OH.SHOW_PUBLISH_BUTTON_FOR = a;
+                            } = await (0, l.B4)((0, l.SJ)(t));
+                            const a = b(o);
+                            i.OH.SHOW_PUBLISH_BUTTON_FOR = a;
                             const s = e.createNew(a, "notebook", {
-                                name: l.OH.PY_KERNEL_NAME
+                                name: i.OH.PY_KERNEL_NAME
                             });
-                            if (l.OH.SHOW_PUBLISH_BUTTON_FOR = void 0, l.OH.TOKENS.set(s.id, t), void 0 === s) throw Error("Error loading lab");
-                            return d(s, JSON.parse(n)), s
-                        }, d = (t, e, o) => {
+                            if (i.OH.SHOW_PUBLISH_BUTTON_FOR = void 0, i.OH.TOKENS.set(s.id, t), void 0 === s) throw Error("Error loading lab");
+                            return h(s, JSON.parse(n)), s
+                        }, h = (t, e, o) => {
                             const n = new a.NotebookModel;
                             "local" !== o && n.fromJSON(e), t.content.model = n
-                        }, h = t => (null != t ? t : l.OH.DEFAULT_LAB_NAME).replace(/^.*[\\\/]/, "");
+                        }, b = t => (null != t ? t : i.OH.DEFAULT_LAB_NAME).replace(/^.*[\\\/]/, "");
                     n()
                 } catch (t) {
                     n(t)
                 }
             }))
         }
     }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, m, g, y, w, k, _ = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, b, m, g, y, w, k, _, S = {
             5367: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -21,36 +21,36 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        S = {};
+        x = {};
 
-    function x(e) {
-        var r = S[e];
+    function j(e) {
+        var r = x[e];
         if (void 0 !== r) return r.exports;
-        var t = S[e] = {
+        var t = x[e] = {
             id: e,
             exports: {}
         };
-        return _[e](t, t.exports, x), t.exports
+        return S[e](t, t.exports, j), t.exports
     }
-    x.m = _, x.c = S, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
-        e && !e.d && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
-    }, x.a = (o, a, i) => {
+    j.m = S, j.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
+        e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
+    }, j.a = (o, a, i) => {
         var u;
-        i && ((u = []).d = 1);
+        i && ((u = []).d = -1);
         var l, s, f, d = new Set,
-            p = o.exports,
-            c = new Promise(((e, r) => {
+            c = o.exports,
+            p = new Promise(((e, r) => {
                 f = r, s = e
             }));
-        c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
+        p[r] = c, p[e] = e => (u && e(u), d.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
             var a;
             l = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
                         var a = [];
                         a.d = 0, o.then((e => {
@@ -71,105 +71,108 @@
                 })),
                 s = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
             return a.r ? s : i()
-        }), (e => (e ? f(c[t] = e) : s(p), n(u)))), u && (u.d = 0)
-    }, x.n = e => {
+        }), (e => (e ? f(p[t] = e) : s(c), n(u)))), u && u.d < 0 && (u.d = 0)
+    }, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return x.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, x.d = (e, r) => {
-        for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        568: "d23144daea3f495050cb",
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        245: "74d5f0c3fbdb9413b03b",
+        568: "51d4a727ea85f89ce2e1",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e] + ".js?v=" + {
-        568: "d23144daea3f495050cb",
+        245: "74d5f0c3fbdb9413b03b",
+        568: "51d4a727ea85f89ce2e1",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
-    } [e], x.g = function() {
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork-authoring-extension:", x.l = (e, r, t, n) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork-authoring-extension:", j.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
                     if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, x.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        x.S = {};
+        j.S = {};
         var e = {},
             r = {};
-        x.I = (t, n) => {
+        j.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                x.o(x.S, t) || (x.S[t] = {});
-                var a = x.S[t],
+                j.o(j.S, t) || (j.S[t] = {});
+                var a = j.S[t],
                     i = "skillsnetwork-authoring-extension",
                     u = (e, r, t, n) => {
                         var o = a[e] = a[e] || {},
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => x.e(669).then((() => () => x(9669))))), u("skillsnetwork-authoring-extension", "0.5.6-rc1", (() => x.e(568).then((() => () => x(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "0.21.4", (() => j.e(669).then((() => () => j(9669))))), u("jwt-decode", "3.1.2", (() => j.e(245).then((() => () => j(6245))))), u("skillsnetwork-authoring-extension", "0.5.7-rc4", (() => j.e(568).then((() => () => j(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        x.g.importScripts && (e = x.g.location + "");
-        var r = x.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), x.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), i = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, u = (e, r) => {
         e = i(e), r = i(r);
@@ -227,101 +230,104 @@
                     u = !1, a--
                 } else {
                     if (a <= t || f < d != n) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? s(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? s(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, f = (e, r) => {
-        var t = x.S[e];
-        if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
-    }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
+    }, c = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", p = (e, r, t, n) => {
         var o = d(e, t);
-        return s(n, o) || "undefined" != typeof console && console.warn && console.warn(p(e, t, o, n)), v(e[t][o])
+        return s(n, o) || v(c(e, t, o, n)), b(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, n, o) {
-        var a = x.I(r);
-        return a && a.then ? a.then(e.bind(e, r, x.S[r], t, n, o)) : e(r, x.S[r], t, n, o)
-    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
-        var a = r && x.o(r, t) && h(r, t, n);
-        return a ? v(a) : o()
-    })), y = {}, w = {
-        1123: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        3033: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        5344: () => m("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
-        5923: () => m("default", "@lumino/disposable", [1, 1, 10, 0]),
-        7986: () => m("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
-        8820: () => m("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        8832: () => m("default", "@lumino/widgets", [1, 1, 37, 2]),
-        9581: () => g("default", "axios", [2, 0, 21, 2], (() => x.e(669).then((() => () => x(9669)))))
-    }, k = {
-        568: [1123, 3033, 5344, 5923, 7986, 8820, 8832, 9581]
-    }, x.f.consumes = (e, r) => {
-        x.o(k, e) && k[e].forEach((e => {
-            if (x.o(y, e)) return r.push(y[e]);
+    }, v = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, b = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (f(e, t), p(r, 0, t, n)))), y = m(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && h(r, t, n);
+        return a ? b(a) : o()
+    })), w = {}, k = {
+        127: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
+        931: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 5]),
+        3191: () => y("default", "jwt-decode", [1, 3, 1, 2], (() => j.e(245).then((() => () => j(6245))))),
+        5139: () => g("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        5923: () => g("default", "@lumino/disposable", [1, 1, 10, 0]),
+        6303: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        8535: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
+        8832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
+        9581: () => y("default", "axios", [2, 0, 21, 2], (() => j.e(669).then((() => () => j(9669)))))
+    }, _ = {
+        568: [127, 931, 3191, 5139, 5923, 6303, 8535, 8832, 9581]
+    }, j.f.consumes = (e, r) => {
+        j.o(_, e) && _[e].forEach((e => {
+            if (j.o(w, e)) return r.push(w[e]);
             var t = r => {
-                    y[e] = 0, x.m[e] = t => {
-                        delete x.c[e], t.exports = r()
+                    w[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete y[e], x.m[e] = t => {
-                        throw delete x.c[e], r
+                    delete w[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
-                var o = w[e]();
-                o.then ? r.push(y[e] = o.then(t).catch(n)) : t(o)
+                var o = k[e]();
+                o.then ? r.push(w[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             340: 0
         };
-        x.f.j = (r, t) => {
-            var n = x.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = x.p + x.u(r),
+                    var a = j.p + j.u(r),
                         i = new Error;
-                    x.l(a, (t => {
-                        if (x.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    j.l(a, (t => {
+                        if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) x.o(i, n) && (x.m[n] = i[n]);
-                    u && u(x)
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    u && u(j)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkskillsnetwork_authoring_extension = self.webpackChunkskillsnetwork_authoring_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), x.nc = void 0;
-    var E = x(5367);
+    })(), j.nc = void 0;
+    var E = j(5367);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["skillsnetwork-authoring-extension"] = E
 })();
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'packages'": "{insert: [(2, OrderedDict([('name', 'jwt-decode'), ('versionInfo', '3.1.2'), "*

 * *               "('licenseId', 'MIT'), ('extractedText', 'The MIT License (MIT)\\n \\nCopyright (c) "*

 * *               '2015 Auth0, Inc. <support@auth0.com> (http://auth0.com)\\n \\nPermission is hereby '*

 * *               'granted, free of charge, to any person obtaining a copy\\nof this software and '*

 * *               'associated documentation files (the "Software"), to deal\\nin the Software without '*

 * *               'r […]*

```diff
@@ -9,14 +9,20 @@
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "5.2.7"
         },
         {
+            "extractedText": "The MIT License (MIT)\n \nCopyright (c) 2015 Auth0, Inc. <support@auth0.com> (http://auth0.com)\n \nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n \nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n \nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "jwt-decode",
+            "versionInfo": "3.1.2"
+        },
+        {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "process",
             "versionInfo": "0.11.10"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.6rc1
+Version: 0.5.7rc4
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 yarn.lock
 jupyter-config/nb-config/skillsnetwork_authoring_extension.json
 jupyter-config/server-config/skillsnetwork_authoring_extension.json
 skillsnetwork-authoring-extension/__init__.py
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
-skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
+skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
+skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
 skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
 skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/button/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 /* eslint-disable @typescript-eslint/explicit-module-boundary-types */
 /* eslint-disable @typescript-eslint/ban-types */
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { Dialog, ToolbarButton } from '@jupyterlab/apputils';
 import { IDisposable, DisposableDelegate } from '@lumino/disposable';
 import { IMainMenu } from '@jupyterlab/mainmenu';
-import { getFileContents, openLab } from '../tools';
-import { axiosHandler, postLabModel,} from '../handler';
+import { getFileContents, openLab, openIndependentLab } from '../tools';
+import { axiosHandler, postLabModel, awbAxiosHandler, postIndependentLabModel } from '../handler';
 import { showFailureImportLabDialog } from '../dialog';
 import { Globals } from '../config';
-import { extractAtlasTokenFromQuery, SET_DEFAULT_LAB_NAME_AND_KERNEL, MODE } from '../config';
+import { extractAtlasTokenFromQuery, extractAwbTokenFromQuery, SET_DEFAULT_LAB_NAME_AND_KERNEL, MODE } from '../config';
+import jwt_decode from 'jwt-decode';
 
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import {
@@ -59,19 +60,25 @@
       // This is a Skills Network Lab notebook so add the publish button
       const start = async () => {
         // Get the current file contents
         const file = await getFileContents(panel, context);
         // POST to Atlas the file contents/lab model
         const token = Globals.TOKENS.get(panel.id)
         if (token === undefined) {
-          console.log('No atlas token found for id', panel.id);
+          console.log('No atlas or awb token found for id', panel.id);
           return;
         }
 
-        postLabModel(axiosHandler(token), file);
+        const token_info = jwt_decode(token) as { [key: string]: any };
+
+        if ("version_id" in token_info) {
+          postIndependentLabModel(awbAxiosHandler(token), file, token);
+        } else {
+          postLabModel(axiosHandler(token), file);
+        }
       };
 
       const download = async () => {
         const file = await getFileContents(panel, context);
         const blob = new Blob([file], { type: 'application/x-ipynb+json' });
         const url = URL.createObjectURL(blob);
 
@@ -84,17 +91,17 @@
 
         document.body.removeChild(link);
         URL.revokeObjectURL(url);
       };
 
       const downloadButton = new ToolbarButton({
         className: 'download-lab-button',
-        label: 'Download',
+        label: 'Download Notebook',
         onClick: download,
-        tooltip: 'Download Lab'
+        tooltip: 'Download the current notebook ipynb file to your local system'
       });
 
       const publishButton = new ToolbarButton({
         className: 'publish-lab-button',
         label: 'Publish on SN',
         onClick: start,
         tooltip: 'Publish Lab'
@@ -129,14 +136,16 @@
   console.log("Activated skillsnetwork-authoring-extension button plugin!");
 
   if (await MODE() == "learn") return
 
   // init the token
   const token = await extractAtlasTokenFromQuery();
 
+  const awb_token = await extractAwbTokenFromQuery();
+
   //init globals
   const env_type = await SET_DEFAULT_LAB_NAME_AND_KERNEL()
 
   console.log('Using default kernel: ', Globals.PY_KERNEL_NAME);
 
   // Add the Publish widget to the lab environment
   app.docRegistry.addWidgetExtension('Notebook', new ButtonExtension());
@@ -148,14 +157,23 @@
         await openLab(token, docManager);
       }
       catch (e){
         Dialog.flush() // remove spinner
         showFailureImportLabDialog();
         console.log(e)
       }
+    } else if (awb_token !== 'NO_TOKEN' && env_type !== "local"){
+      try{
+        await openIndependentLab(awb_token, docManager);
+      }
+      catch (e){
+        Dialog.flush() // remove spinner
+        showFailureImportLabDialog();
+        console.log(e)
+      }
     }
   })
 }
 
 /**
  * Export the plugin as default.
  */
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json` & `skillsnetwork-authoring-extension-0.5.7rc4/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/config.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import {ServerConnection} from '@jupyterlab/services';
 import { KernelSpecAPI } from '@jupyterlab/services';
 
 interface Configuration {
 	ATLAS_BASE_URL: string;
   SN_FILE_LIBRARY_URL: string;
+  AWB_BASE_URL: string;
 }
 
 const getServerBaseUrl = (settings: ServerConnection.ISettings): string => {
   let baseUrl = settings.baseUrl;
   // Add the trailing slash if it is missing.
   if (!baseUrl.endsWith('/')) {
     baseUrl += '/';
@@ -35,14 +36,38 @@
       = (await response.json()) as Configuration;
 		return configuration.ATLAS_BASE_URL;
   } else {
     return decodeURIComponent(baseUrl)
   }
 })();
 
+export const AWB_BASE_URL = await (async (): Promise<string> => {
+	const currentUrl = window.location.href;
+
+	const parameters = new URL(currentUrl).searchParams;
+	const baseUrl: string | undefined = parameters.get('awb_base_url')!;
+	if (baseUrl === null) {
+		const init: RequestInit = {
+			method: 'GET',
+		};
+		const settings = ServerConnection.makeSettings();
+		const requestUrl = getServerBaseUrl(settings) + 'skillsnetwork-authoring-extension/config';
+    const response = await ServerConnection.makeRequest(
+			requestUrl,
+			init,
+			settings,
+		);
+		const configuration: Configuration
+      = (await response.json()) as Configuration;
+		return configuration.AWB_BASE_URL;
+  } else {
+    return decodeURIComponent(baseUrl)
+  }
+})();
+
 export const SN_FILE_LIBRARY_URL = await (async (): Promise<string> => {
 	const currentUrl = window.location.href;
 
 	const parameters = new URL(currentUrl).searchParams;
 	const snFileLibraryURL: string | undefined = parameters.get('sn_file_library_url')!;
 	if (snFileLibraryURL === null) {
 		const init: RequestInit = {
@@ -87,14 +112,22 @@
   const currentURL = window.location.href;
   const params = new URL(currentURL).searchParams;
   const token_from_query = params.get('atlas_token')
 
   return  (token_from_query !== null) ? token_from_query : 'NO_TOKEN';
 };
 
+export const extractAwbTokenFromQuery = async (): Promise<string> => {
+  const currentURL = window.location.href;
+  const params = new URL(currentURL).searchParams;
+  const token_from_query = params.get('awb_token')
+
+  return  (token_from_query !== null) ? token_from_query : 'NO_TOKEN';
+};
+
 export const SET_DEFAULT_LAB_NAME_AND_KERNEL = async (): Promise<string> => {
 const currentURL = window.location.href;
   const params = new URL(currentURL).searchParams;
   let env_type = params.get('env_type')
 
   if (env_type !== "jupyterlab" && env_type !== "jupyterlite"){
     env_type = "local"
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/menu/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import { IMainMenu } from '@jupyterlab/mainmenu';
 import { Menu, Widget } from '@lumino/widgets';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { show_spinner, showFailureImportLabDialog } from '../dialog';
 import { MODE } from '../config';
-import { openLab } from '../tools';
+import { openIndependentLab, openLab } from '../tools';
+import jwt_decode from 'jwt-decode';
 
 export const menu: JupyterFrontEndPlugin<void> = {
   id: 'skillsnetwork-authoring-extension:menu',
   autoStart: true,
   requires: [IMainMenu, INotebookTracker, IDocumentManager],
   activate: async (app: JupyterFrontEnd, mainMenu: IMainMenu, notebookTracker: INotebookTracker, docManager: IDocumentManager) => {
 
@@ -40,30 +41,37 @@
     });
 
     const showTokenDialog = (notebookTracker: INotebookTracker, docManager: IDocumentManager) => {
 
       // Generate Dialog body
       let bodyDialog = document.createElement('div');
       let nameLabel = document.createElement('label');
-      nameLabel.textContent = "Enter your authorization token: "
+      nameLabel.textContent = "Enter your authorization token"
       let tokenInput = document.createElement('input');
       tokenInput.className = "jp-mod-styled";
       bodyDialog.appendChild(nameLabel);
       bodyDialog.appendChild(tokenInput);
 
       showDialog({
         title: "Edit a Lab",
         body: new Widget({node: bodyDialog}),
         buttons: [Dialog.cancelButton(), Dialog.okButton()]
       }).then(async result => {
         if (result.button.accept){
           show_spinner('Loading up your lab...');
 
           const token = tokenInput.value
-          await openLab(token, docManager);
+
+          const token_info = jwt_decode(token) as { [key: string]: any };
+
+          if ("version_id" in token_info) {
+            await openIndependentLab(token, docManager);
+          } else {
+            await openLab(token, docManager);
+          }
         }
       })
       .catch((e) => {
         Dialog.flush(); //remove spinner
         showFailureImportLabDialog();
         console.log(e)
       });
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/sn-file-library.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import { Widget } from '@lumino/widgets';
 import { Dialog } from '@jupyterlab/apputils';
 import { Globals, SN_FILE_LIBRARY_URL } from './config';
+import jwt_decode from 'jwt-decode';
 
 export class SkillsNetworkFileLibraryWidget extends Widget {
     constructor(nbPanelId: string) {
       const frame = document.createElement('iframe');
-      frame.src = `${SN_FILE_LIBRARY_URL}?atlas_token=${Globals.TOKENS.get(nbPanelId)}`
+      const token = Globals.TOKENS.get(nbPanelId)
+      const token_info = token ? jwt_decode(token) as { [key: string]: any } : {};
+      if ("project_id" in token_info) frame.src = `${SN_FILE_LIBRARY_URL}?atlas_token=${token}`
       frame.setAttribute("frameborder", "0")
       frame.setAttribute("allow", "clipboard-read; clipboard-write")
       frame.classList.add("sn-file-library-frame");
       super({ node: frame });
     }
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts` & `skillsnetwork-authoring-extension-0.5.7rc4/src/tools.ts`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   NotebookPanel,
   NotebookModel
 } from '@jupyterlab/notebook';
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import * as nbformat from '@jupyterlab/nbformat';
 import { Globals } from './config';
-import { axiosHandler, getLabModel } from './handler';
+import { axiosHandler, getLabModel, awbAxiosHandler, getIndependentLabModel} from './handler';
 
 export interface ICellData {
   cell_type: string;
   id: string;
   metadata: {};
   outputs: [];
   source: string[];
@@ -70,14 +70,39 @@
     metadata: config_meta,
     nbformat: config_nbmajor,
     nbformat_minor: config_nbminor
   };
   return JSON.stringify(rawFile, null, 2);
 };
 
+export const openIndependentLab = async (awb_token: string, docManager: IDocumentManager): Promise<NotebookPanel> => {
+  let {labFilename, body: instructions_content} = await getIndependentLabModel(awbAxiosHandler(awb_token), awb_token)
+
+  // TODO: This is really hacky and should be replaced with a better solution
+  // Set the publish button to only show for the lab with title labFilename
+  Globals.SHOW_PUBLISH_BUTTON_FOR = labFilename;
+
+  // Attempt to open the lab
+  const nbPanel = docManager.createNew(labFilename, 'notebook', { name:  Globals.PY_KERNEL_NAME}) as NotebookPanel;
+
+  // Reset it back to undefind, meaning that the publish button will not be shown for any subsequent activation
+  // unless this variable is set again
+  Globals.SHOW_PUBLISH_BUTTON_FOR = undefined;
+
+  // Persist tokens
+  Globals.TOKENS.set(nbPanel.id, awb_token);
+
+  if (nbPanel === undefined) {
+    throw Error('Error loading lab')
+  }
+  loadLabContents(nbPanel, instructions_content as unknown as nbformat.INotebookContent);
+
+  return nbPanel;
+}
+
 export const openLab = async (token: string, docManager: IDocumentManager): Promise<NotebookPanel> => {
   let {instructions_file_path, body: instructions_content} = await getLabModel(axiosHandler(token))
   const labFilename = getLabFileName(instructions_file_path);
 
   // TODO: This is really hacky and should be replaced with a better solution
   // Set the publish button to only show for the lab with title labFilename
   Globals.SHOW_PUBLISH_BUTTON_FOR = labFilename;
```

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json` & `skillsnetwork-authoring-extension-0.5.7rc4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock` & `skillsnetwork-authoring-extension-0.5.7rc4/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 # THIS IS AN AUTOGENERATED FILE. DO NOT EDIT THIS FILE DIRECTLY.
 # yarn lockfile v1
 
 
+"@aashutoshrathi/word-wrap@^1.2.3":
+  version "1.2.6"
+  resolved "https://registry.yarnpkg.com/@aashutoshrathi/word-wrap/-/word-wrap-1.2.6.tgz#bd9154aec9983f77b3a034ecaa015c2e4201f6cf"
+  integrity sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==
+
 "@babel/code-frame@7.12.11":
   version "7.12.11"
   resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.12.11.tgz#f4ad435aa263db935b8f10f2c552d23fb716a63f"
   integrity sha512-Zt1yodBx1UcyiePMSkWnU4hPqhwq7hGi2nFL1LeA3EUl+q2LQx16MISgJ0+z7dnmgvP9QtIleuETGOiOH1RcIw==
   dependencies:
     "@babel/highlight" "^7.10.4"
 
 "@babel/code-frame@^7.0.0":
-  version "7.21.4"
-  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.21.4.tgz#d0fa9e4413aca81f2b23b9442797bda1826edb39"
-  integrity sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==
-  dependencies:
-    "@babel/highlight" "^7.18.6"
-
-"@babel/helper-validator-identifier@^7.18.6":
-  version "7.19.1"
-  resolved "https://registry.yarnpkg.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz#7eea834cf32901ffdc1a7ee555e2f9c27e249ca2"
-  integrity sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==
-
-"@babel/highlight@^7.10.4", "@babel/highlight@^7.18.6":
-  version "7.18.6"
-  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.18.6.tgz#81158601e93e2563795adcbfbdf5d64be3f2ecdf"
-  integrity sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==
+  version "7.22.5"
+  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.22.5.tgz#234d98e1551960604f1246e6475891a570ad5658"
+  integrity sha512-Xmwn266vad+6DAqEB2A6V/CcZVp62BbwVmcOJc2RPuwih1kw02TjQvWVWlcKGbBPd+8/0V5DEkOcizRGYsspYQ==
+  dependencies:
+    "@babel/highlight" "^7.22.5"
+
+"@babel/helper-validator-identifier@^7.22.5":
+  version "7.22.5"
+  resolved "https://registry.yarnpkg.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.22.5.tgz#9544ef6a33999343c8740fa51350f30eeaaaf193"
+  integrity sha512-aJXu+6lErq8ltp+JhkJUfk1MTGyuA4v7f3pA+BJ5HLfNC6nAQ0Cpi9uOquUj8Hehg0aUiHzWQbOVJGao6ztBAQ==
+
+"@babel/highlight@^7.10.4", "@babel/highlight@^7.22.5":
+  version "7.22.5"
+  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.22.5.tgz#aa6c05c5407a67ebce408162b7ede789b4d22031"
+  integrity sha512-BSKlD1hgnedS5XRnGOljZawtag7H1yPfQp0tdNJCHoH6AZ+Pcm9VvkrK59/Yy593Ypg0zMxH2BxD1VPYUQ7UIw==
   dependencies:
-    "@babel/helper-validator-identifier" "^7.18.6"
+    "@babel/helper-validator-identifier" "^7.22.5"
     chalk "^2.0.0"
     js-tokens "^4.0.0"
 
 "@babel/runtime@^7.1.2":
-  version "7.21.0"
-  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.21.0.tgz#5b55c9d394e5fcf304909a8b00c07dc217b56673"
-  integrity sha512-xwII0//EObnq89Ji5AKYQaRYiW/nZ3llSv29d49IuxPhKbtJoLP+9QUUZ4nVragQVtaVGeZrpB+ZtG/Pdy/POw==
+  version "7.22.6"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.22.6.tgz#57d64b9ae3cff1d67eb067ae117dac087f5bd438"
+  integrity sha512-wDb5pWm4WDdF6LFUde3Jl8WzPA+3ZbxYqkC6xAXuD3irdEHN1k0NfTRrJD8ZD378SJ61miMLCqIOXYhd8x+AJQ==
   dependencies:
     regenerator-runtime "^0.13.11"
 
 "@blueprintjs/colors@^4.0.0-alpha.3":
-  version "4.1.21"
-  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.1.21.tgz#622c56ac7f9af466680eafcdbaf26e5c9152ad3b"
-  integrity sha512-5csitaTn1xyHktMRyXAcvWzsbrgtP9pK7ZmYX9f0TGjB1UG5zNaTGLexX0aFqop44SpfsSP5mbA8xGBniy8nZA==
+  version "4.2.1"
+  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.2.1.tgz#603b2512caee84feddcb3dbd536534c140b9a1f3"
+  integrity sha512-Cx7J2YnUuxn+fi+y5XtXnBB7+cFHN4xBrRkaAetp78i3VTCXjUk+d1omrOr8TqbRucUXTdrhbZOUHpzRLFcJpQ==
+  dependencies:
+    tslib "~2.5.0"
 
 "@blueprintjs/core@^3.36.0", "@blueprintjs/core@^3.54.0":
   version "3.54.0"
   resolved "https://registry.yarnpkg.com/@blueprintjs/core/-/core-3.54.0.tgz#7269f34eccdf0d2874377c5ad973ca2a31562221"
   integrity sha512-u2c1s6MNn0ocxhnC6CuiG5g3KV6b4cKUvSobznepA9SC3/AL1s3XOvT7DLWoHRv2B/vBOHFYEDzLw2/vlcGGZg==
   dependencies:
     "@blueprintjs/colors" "^4.0.0-alpha.3"
@@ -149,18 +156,18 @@
   integrity sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==
 
 "@jridgewell/set-array@^1.0.1":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.1.2.tgz#7c6cf998d6d20b914c0a55a91ae928ff25965e72"
   integrity sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==
 
-"@jridgewell/source-map@^0.3.2":
-  version "0.3.3"
-  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.3.tgz#8108265659d4c33e72ffe14e33d6cc5eb59f2fda"
-  integrity sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==
+"@jridgewell/source-map@^0.3.3":
+  version "0.3.5"
+  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.5.tgz#a3bb4d5c6825aab0d281268f47f6ad5853431e91"
+  integrity sha512-UTYAUj/wviwdsMfzoSJspJxbkH5o1snzwX0//0ENX1u/55kkZZkcTZP6u9bwKGkv+dkk9at4m1Cpt0uY80kcpQ==
   dependencies:
     "@jridgewell/gen-mapping" "^0.3.0"
     "@jridgewell/trace-mapping" "^0.3.9"
 
 "@jridgewell/sourcemap-codec@1.4.14":
   version "1.4.14"
   resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz#add4c98d341472a289190b424efbdb096991bb24"
@@ -180,64 +187,64 @@
     "@jridgewell/sourcemap-codec" "1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
-"@jupyter/ydoc@~0.2.3":
+"@jupyter/ydoc@~0.2.4":
   version "0.2.4"
   resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.4.tgz#bc312f171777b58e286aadca62dadeca3a894dd1"
   integrity sha512-QACcB4bF+Ew4UJmJP+3OyiyQm3vwRYF6iZCQK9q0nE2U5uAosQkfLyT6Bx71jPUXe4G9lEF6m9fjpZvSUX7Lyw==
   dependencies:
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
     "@lumino/signaling" "^1.10.0 || ^2.0.0-alpha.6"
     y-protocols "^1.0.5"
     yjs "^13.5.40"
 
 "@jupyterlab/application@^3.3.0":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.3.tgz#7e199f77a4536bc7429fbecf9ba1850f51d9de52"
-  integrity sha512-G0tR6sUSCuHB8vGQnaB5lfihKNJVHtqYNoMlsZYF9rYpZEhW1TRD4uE5rg4RfDDR+GghjckQlP3rRNB2Vn4tMA==
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.5.tgz#44679f48ad6485e96e6ce5cd6401cafa8c1d911c"
+  integrity sha512-T9pjZbIB26HBkssG1bLVZqwUXjSMCobYGRwNvit0GiJ4BF1I2GxuVF4Hd2tNIqqFreRVEyvobN+w+DGZWFLxfw==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docregistry" "^3.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/rendermime-interfaces" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/docregistry" "^3.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/rendermime-interfaces" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/statedb" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/apputils@^3.3.0", "@jupyterlab/apputils@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.3.tgz#bc37683142b281e21d22a2f4698634563658298e"
-  integrity sha512-um2Aaa5fOUwHFpAqKTDA+MFpnAldzOILIi5QsKOWRxiJA2W8x+hlg5HvHbq+eSWuWEU3ah15M7htzBcL3g9d4Q==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/settingregistry" "^3.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/apputils@^3.3.0", "@jupyterlab/apputils@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.5.tgz#cc4fbc811c797dee71d1ecff0fde15b4ca6750e6"
+  integrity sha512-cJ4FnsnEMwhcrh/27Z7q04hYRPYWgFRrBylw10SBHWzOryiFc9chg8LqzUOL0CNjmBRui6hS6w5R/Z7YmINpTg==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/settingregistry" "^3.6.5"
+    "@jupyterlab/statedb" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
@@ -247,30 +254,30 @@
     "@lumino/widgets" "^1.37.2"
     "@types/react" "^17.0.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     sanitize-html "~2.7.3"
     url "^0.11.0"
 
-"@jupyterlab/attachments@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.3.tgz#f2e52c3518d3f84cb7a7cc7c8a113f49dfdde4f1"
-  integrity sha512-ZYDJjcoExmojsGkX5f1WVFfW39XJcb7CtfzFcNz3AbytebRK13S1xqCRlef/TFW+XT6BG7hjMSJlpW3GdkCV1Q==
-  dependencies:
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+"@jupyterlab/attachments@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.5.tgz#ad8600dfe26b7036b6e1b2f1ad066fe10e36d2ef"
+  integrity sha512-Gtam8zzgL3/hkBiHHBAS3nW2EsrBiA+X9SeM+A0CmKq0JHDFlf8boR54HqU3zGZv6Cc313RfVuHtoBsX2hQIcQ==
+  dependencies:
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/rendermime-interfaces" "^3.6.5"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/builder@^3.3.0":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.3.tgz#a4b22efe34e9598b84122ff10509d3d890017b6a"
-  integrity sha512-oY1a/r75RMoPzhSmuVu+DfjL0cKk1ceHTniZsM2wPuhjjyoF875u6CDzArJatpOOuTgLm7CY5OcU3LCIK1OAgg==
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.5.tgz#17e103ff13a135e3df8cf03bf7c592fae87b97ec"
+  integrity sha512-J9WO50gxjJ1bUo7BCix0fSxpRySCwaR8AaWNQ5QdYT1ARSGuSnfM9ZyeUOS61DvL3+h7IqsPTQQr5tbhIWv91Q==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
@@ -300,379 +307,393 @@
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
     webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/cells@^3.3.3", "@jupyterlab/cells@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.3.tgz#ac8191f99923a004211725435d25280347794cff"
-  integrity sha512-o3Uydof6bZ6HGSRgSm6isuAhaqYVmv+ozsmADYNmIGbwwwC+eb391Cv+rC3kuPZX/+2UhhO6s7fqFxW8aHUDkg==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/attachments" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/codemirror" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/filebrowser" "^3.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/outputarea" "^3.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/cells@^3.3.3", "@jupyterlab/cells@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.5.tgz#44b87fd4e8cf645be45f862eb006d28cc780a448"
+  integrity sha512-oxo2jjKwrLlWkH8kNk64LdOoUowd+iBQuY9/5fyk5U2YswV4x1GUtOlBAzFYiBFK4Nq+NvwjXoZjVaYAxTs6pA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/attachments" "^3.6.5"
+    "@jupyterlab/codeeditor" "^3.6.5"
+    "@jupyterlab/codemirror" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/filebrowser" "^3.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/outputarea" "^3.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
     marked "^4.0.17"
     react "^17.0.1"
 
-"@jupyterlab/codeeditor@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.3.tgz#a889c1821001888af7b60f66b1ee91e15797c0bb"
-  integrity sha512-SnVo5KDhyRkK/o1SDRX9nehLEAMaOBFf+GUx2jeXBTfr6wTKcwDBnJAUwlOfncwRlMV79aUIqTIcS861FSXDyA==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/codeeditor@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.5.tgz#1101ada956f6e983c6bd9101db3674bf53165975"
+  integrity sha512-Wp81WZaUg3cJh/cKhoB/RemDOxE6hyEx0kvNu8BRTTYobKMqMQWahKTEWRoHxTCoeQzb/tJUSEJQV8u7d0vr1Q==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/codemirror@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.3.tgz#7cb19faae58d4fc26bc37064f029c4b17098c20a"
-  integrity sha512-VU5bInzSqsyPGZkEd/w6HtJ9PSw7U5twoyrQSpSM+E2SEYWskaBZOHJf8XNunVoRRKwSvDLyxSs07Ot6zUlA0w==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/statusbar" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
+"@jupyterlab/codemirror@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.5.tgz#36189e2764979a7e93b9a10ee8232e21ca86d2bd"
+  integrity sha512-BonbNpBxOn4CDPuyl2JtkruwgiA8ANsIAuzrZMoTnglOScHLGxmddnF5BhsjuvatG2cDM/PZtY+KaQqcaJQBQQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/codeeditor" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/statusbar" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     codemirror "~5.61.0"
     react "^17.0.1"
     y-codemirror "^3.0.1"
 
-"@jupyterlab/coreutils@^5.6.3":
-  version "5.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.3.tgz#3b0b5d481b14596158b560336833c89be509e84e"
-  integrity sha512-jRVTpwGzP9wBNYuaZTip89FS1qbeSYrEO2qdNVdW2rs0mQHcIlu3Fkv5muMFmKYGi0XHhG3UhZiWQ7qiPw2svQ==
+"@jupyterlab/coreutils@^5.6.5":
+  version "5.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.5.tgz#113b95fe106fc2be69c7a523f916ac25d2d413c2"
+  integrity sha512-nQ0eY9rv8bj0KoFHAwR4dDJY033XZsSDH5EV/E5m5/0f/oyLxWmKI3L/C1alXrltgdivh3nudbDX7VzQRoZPHA==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/docmanager@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.3.tgz#df2c5b45c5e9b38e2a48eb703ff5e3a9b4b7860c"
-  integrity sha512-4d5zGE3SGbg58wsFJtyskUxK7dEvl8d5Wh90hTlmsFNmr+nh5duTWcqTQ/a+d76YxYbGhH5vqOsNm5ORZq4Umw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docprovider" "^3.6.3"
-    "@jupyterlab/docregistry" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/statusbar" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
+"@jupyterlab/docmanager@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.5.tgz#a0ce3bfc73748fc128b99588ebea64c4643f1f1c"
+  integrity sha512-BBu03OJrtst+2zAxq4NJpaizIfDCZRL7G736o2bn5LSTNuUmg3gVbAtUG7beqUX/oKrCO/ALlgPI8zL+5vS9lQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/docprovider" "^3.6.5"
+    "@jupyterlab/docregistry" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/statusbar" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/docprovider@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.3.tgz#90fbf07214b6c3e98055787fc351a68e9d83470c"
-  integrity sha512-M5IoyykDpWnUFNePHz3+fi/RNvV92UNbQGfAvsaCMSn+fl48rD4rHB9EZGceOisb3m1U+E4SntKYI3pl49yUEg==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/translation" "^3.6.3"
+"@jupyterlab/docprovider@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.5.tgz#4e296d4f117a545fd7b33dd3dca52f0f39c312b3"
+  integrity sha512-jPFI2hKt1D/9ZpDH7iB9XDoKj8HYSNAFFENWOlRaEXCHL3S3lZA9b2G+T1XunQRefYxdyDZlY2JUSXojdgV2mA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     y-protocols "^1.0.5"
     y-websocket "^1.4.6"
 
-"@jupyterlab/docregistry@^3.3.0", "@jupyterlab/docregistry@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.3.tgz#4a03fbb704449bda7a94df7a4bd63078c11aef58"
-  integrity sha512-unDMrtCSGKPqX9uvYCkI7zGTvskuC9odAPIHPsYSVMcHL/o5M7lQkHmRZCoSIezfe5OvPGXbYT2boQrBKXqCFw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/codemirror" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docprovider" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/rendermime-interfaces" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/docregistry@^3.3.0", "@jupyterlab/docregistry@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.5.tgz#8744c794c711454224d036e78cdb750e67b58ddf"
+  integrity sha512-/QYkpDyqmDFeB12fjr0ANbSuJ2CRGk3O4yVft58pUsQHcWTZLXMG23XMMt9SaFjlr5LcYjhAbIfPzR8NYwGU9Q==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/codeeditor" "^3.6.5"
+    "@jupyterlab/codemirror" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/docprovider" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/rendermime-interfaces" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/filebrowser@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.3.tgz#169b880e19a8686f9a669a750027c2817b4b6cef"
-  integrity sha512-Qu+Mtx3d0QY7qCMIxg5nQtkQYh+kZ2kGO7tgS+yfKjo0cluPsxo+Zr56KtJU6zyDYjylVCtLYIK2RflwRKhdng==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docmanager" "^3.6.3"
-    "@jupyterlab/docregistry" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
-    "@jupyterlab/statusbar" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/filebrowser@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.5.tgz#2a87f7cfe74f653b6caeece72a22490c6ca2dfcc"
+  integrity sha512-jDNy3UHKNbEEW1tuUnWaae9dgK3PvyyJRnYWou7Tiz1uk/aqyoYEcvfyEP0xJ87bh8mw4D8XHaEgfEOufZwyMg==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/docmanager" "^3.6.5"
+    "@jupyterlab/docregistry" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/statedb" "^3.6.5"
+    "@jupyterlab/statusbar" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
 "@jupyterlab/mainmenu@^3.4.2":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz#5d322db9b8d742b7042109ab7e8c733696ae38fc"
-  integrity sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.5.tgz#a101260d8c60347ef61f6c7b59e94f7260bbd1a5"
+  integrity sha512-E7vJqh50tGmuZMRBb0XTqky3eINGFLO2ak2oj8xekLZX1hstLp6LHzlJy5ygSABD6AmxcyrXSbwvITHReH8PXQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
-  integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
+"@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15":
+  version "4.0.2"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.2.tgz#a735304dfcd3ac5214bc6e471cd24f7e198a01b3"
+  integrity sha512-K83wDb1iUViTk4mj228SR4E0GPASiykXcD/tVYAOvxWv8TsaZ2UK/dcX4ZtBEZpVqI5enRrq8Z7xISMR+3CRBg==
+  dependencies:
+    "@lumino/coreutils" "^2.1.1"
+
+"@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.5.tgz#dfb957d1297b2f319690df326e2ecc1eee99edfa"
+  integrity sha512-yyyNniuzxycsF+kHvjpAIjZ+qrt3G/HEViZN+FJA3vFpg6e2n/nqa7BgzlxINS5SH4FnBG6rM/u45bwih38VkA==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
 "@jupyterlab/notebook@^3.3.0":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.3.tgz#1584be72184d67d59291e2b22f55bc257afde436"
-  integrity sha512-id1KD5/9IDPr/IZFCl/YX4Vc+Q198LZshhFNEcVJZcRdjD7Vh+LGvWcLOh80OAv86J4XSTTAsp3gHPr4iSwPDg==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/cells" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docregistry" "^3.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/settingregistry" "^3.6.3"
-    "@jupyterlab/statusbar" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.5.tgz#6d3c4fecb4c95dfacf4ea68335518aaca73f7fa3"
+  integrity sha512-+Tb/kvFeI5hCzt60wdfxFncquhrkX2C3eoOPAfiabqWkCL52oZfYDRYVmrXTJzvuhmVVupRPKjvusFPDoBN8/g==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/cells" "^3.6.5"
+    "@jupyterlab/codeeditor" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/docregistry" "^3.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/settingregistry" "^3.6.5"
+    "@jupyterlab/shared-models" "^3.6.5"
+    "@jupyterlab/statusbar" "^3.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/observables@^4.6.3":
-  version "4.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
-  integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
+"@jupyterlab/observables@^4.6.5":
+  version "4.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.5.tgz#dea28b8048769adaad1376cb3bcb34a35a10c8df"
+  integrity sha512-k6x7kLou+1EPtVlrQ6OFoujFj1jlvsKMcnap83Omjqj1DIkzSBGat3Y7Yf5OS7lrdyERJGYbtV9vfeSkwdjkjA==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/outputarea@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.3.tgz#acf7a604eb352109d096d2a9fdd1fbbddbf80af1"
-  integrity sha512-SSmkDWS8MhdXl7+rQoLu/5wJBKTq1YEkxlQcKh1Z0VN4VjYDCA/bKFGjOmKN7wMmoVP/zRmWvUwl/DLJCHx/Tw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/rendermime-interfaces" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
+"@jupyterlab/outputarea@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.5.tgz#9833ec040f90aa96a7b045e2c1e05197890920ae"
+  integrity sha512-CmsemQDwpO4RbxbmWgcwP7Pgq/3cJV6zpJSv4c172C3Nq82xXYPa+3XDbTV+cVFmZe+f1e3FJFw+i3uyT/Ad1Q==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/rendermime" "^3.6.5"
+    "@jupyterlab/rendermime-interfaces" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
-"@jupyterlab/rendermime-interfaces@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.3.tgz#80009705d5ded65a4b27c4b826b295f40f126902"
-  integrity sha512-VHZVnqB0K1nmoQMOhFGHwvSYMQmxqcOC3wWDRFeUOv8S+tejTYfbrKXPOZJvhdGB52Jn8XNIesXOuNpLhl4HmQ==
-  dependencies:
-    "@jupyterlab/translation" "^3.6.3"
-    "@lumino/coreutils" "^1.11.0"
-    "@lumino/widgets" "^1.37.2"
-
-"@jupyterlab/rendermime@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.3.tgz#48d83c70493b0356d4dac6d89a863d8a5a84f68e"
-  integrity sha512-w3e38OddJin9fbfe7EWsKiiup/0ayvHPrAsacde8PqGLvi/sLeAXT98PqihsKt8EAlOgXSkSO0Ivjbd0JzgGgA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/codemirror" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime-interfaces" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/translation" "^3.6.3"
+"@jupyterlab/rendermime-interfaces@^3.6.5":
+  version "3.8.2"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.8.2.tgz#115d70f1dd064784cd5816785c94b7c36e605fd5"
+  integrity sha512-IOnzA/ccfwXGO/RaWysYn74ojJ7PaH5igTnS0sjo4qIprFZ6tCORTrKF594BA7Qz6PpW2+GpdUVMUnnYdU5R9Q==
+  dependencies:
+    "@lumino/coreutils" "^1.11.0 || ^2.1.1"
+    "@lumino/widgets" "^1.37.2 || ^2.1.1"
+
+"@jupyterlab/rendermime@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.5.tgz#95e49172914118ea5ca2d5037659ee2baf1c132a"
+  integrity sha512-ln0UgKJo+2qS4FehCQUR5W/SDbnwiUHX+zdKEViNI6NHK2oAeXtD4BbuxfS3ZfJyEKZcB6hMj+OVqO7opL/fvw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/codemirror" "^3.6.5"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/rendermime-interfaces" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/translation" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     lodash.escape "^4.0.1"
     marked "^4.0.17"
 
-"@jupyterlab/services@^6.4.3", "@jupyterlab/services@^6.6.3":
-  version "6.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.3.tgz#303938e5dc5aebce7a86324a64ed89c25c61c9e7"
-  integrity sha512-BxEOMRl9X18T5wY7iV6ZJhARnibFghpD3OruqeSbnGdbRv6XJi8prsRbCQQ6Mf9agvf81B20KmDvYKikPHC0xQ==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/settingregistry" "^3.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
+"@jupyterlab/services@^6.4.3", "@jupyterlab/services@^6.6.5":
+  version "6.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.5.tgz#81ca9d1f13789541055ebee870e9a67c929f7933"
+  integrity sha512-ReTi7r8nAzop1u65Jc4HDlyERcyV8ebjTGmXUohRWEqMbgjrFH8rz4rV8iQnobg5GZ2Kyf2RBdSTKwEttj2Ghg==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/nbformat" "^3.6.5"
+    "@jupyterlab/observables" "^4.6.5"
+    "@jupyterlab/settingregistry" "^3.6.5"
+    "@jupyterlab/statedb" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
-  integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
+"@jupyterlab/settingregistry@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.5.tgz#9bf56db9bc85ffd06d2ed39ddfa5888c81e34f5f"
+  integrity sha512-PLg6E7j9x5otTnsTntFHwhbd+SacSsjiTP5krVq1WwTV6FrqrfT29ttxTCgV5+y7j91YmnEaHhZD+TXx5bQqIQ==
   dependencies:
-    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.5"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.3.tgz#6ba2166af9232c9a185cf0077cf1272f24cc9a69"
-  integrity sha512-A36L+0NN8f0WOES2GdtZjp9uFuC7IBjhKiO/RlKRX5AFjNxoJ9oO3PZtoxJQYPnGBljMqVdRa+m9aYEfvKhYyQ==
+"@jupyterlab/shared-models@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/shared-models/-/shared-models-3.6.5.tgz#f7ccc174222b53ab19005425b20f241e231b28c4"
+  integrity sha512-5ZsX5Kt9n3tVvTSNDnV8vKKpQFDZ/zdUifwClx1gy5ZLMc0rtjXyIC10UKk0l8fIFSFGj7EN2ZR6pIAF0TRDZg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.4"
+    "@jupyterlab/nbformat" "^3.6.5"
+
+"@jupyterlab/statedb@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.5.tgz#4a651e4c97f7f89b852bb9e96409b07d55ad436f"
+  integrity sha512-Ah6pwJiU0XDI41iH+Ihw1lONBNDUrM4h58HwXD5qMvEPIWw5IxQn7QKt5XuaQWpTagXfUeuHrNpbekgdEImMog==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/statusbar@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.3.tgz#29c24427a2d6b205349b94583de0ccb8b9435d88"
-  integrity sha512-m59NLR0Zghm53PU6hDzRF4XVORnJx/YRx0svcjj/TGLk8LSffpQbUDBy24dl3tOuChk4D5cCdgeDH1X30TzCaA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
+"@jupyterlab/statusbar@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.5.tgz#dfb52b563c46fac0617db54fcfc5c2e8eaffb2c2"
+  integrity sha512-+kSW6ZgpXOfbfH9727JBYtx+lmgPiJCfFDKqlZfTbxYfvFx9j0C7eWfHZm6sL1WFYv5lB0iCUEY3GfL7X4LjHQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.5"
+    "@jupyterlab/codeeditor" "^3.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/translation" "^3.6.5"
+    "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/translation@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.3.tgz#3fd95f726316762bc1799a7b7be0243d5465932a"
-  integrity sha512-m+wwBv/hiN5Y6Sb7Ij150ZhPXZdhN5wI8CT3afnzARwKr2Aww5AIURO3upmMwnKaPVQTrWqsS3+7bZS/21JuJA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
+"@jupyterlab/translation@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.5.tgz#3f308e421cb8e5d8d3739269e20c01103c1871e4"
+  integrity sha512-avk96gOFuWqZWywCezeXvvjNnib4xQv5VY4rvvhTrz0unAeo8CtQ3L3ZBdLtWLq+aA470WfdhneLwtv3n6JYdw==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/services" "^6.6.5"
+    "@jupyterlab/statedb" "^3.6.5"
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/ui-components@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.3.tgz#36555036b383c5d80346f409a7a168d13c9d8c85"
-  integrity sha512-XzseUo2IXclPlYcGxCIz8evjWF+dCBMmbJlvoE5OF29BYBvI5N/DUaTem8bHN5kmQwHIXX6BImHu7rbC9Xjl6w==
+"@jupyterlab/ui-components@^3.6.5":
+  version "3.6.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.5.tgz#0092b5d6f606d53541450f089835fd58133bc138"
+  integrity sha512-yEkC/MLxalEJ9PvZs7AQo/IJDxqAToBBWvqC57t8lGEEkwNBG4hNDv8bmQMtfVv9BMvooQzhac5wJiaEj0T6sg==
   dependencies:
     "@blueprintjs/core" "^3.36.0"
     "@blueprintjs/select" "^3.15.0"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.5"
+    "@jupyterlab/translation" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
@@ -721,33 +742,33 @@
     "@lumino/virtualdom" "^1.14.3"
 
 "@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
   version "1.12.1"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
-"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.0":
-  version "2.1.0"
-  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.0.tgz#291ed11a1bd143bfd5a2f2638cfb27aefd1bd9ba"
-  integrity sha512-1pF3gaTxZY6P+Tixs2rd1aj5HgFOdH3RNupgsMaq0sFmxuvuSxaYhiK5/LB9evDN8a6HqHFeS6wVhVajSOJfDQ==
+"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^1.11.0 || ^2.1.1", "@lumino/coreutils@^2.1.1":
+  version "2.1.1"
+  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.1.tgz#e867a501f3564987a757005c81aa4b0d4ea5ff4c"
+  integrity sha512-OmEzvphZC/EVpFfwBkmcuzNwKXvkij6gJo1mbf4/tZMC1/8NO3aVnjK1FsgC0TlaGwMD1BLIFgGay2mC/I/cyQ==
 
 "@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4", "@lumino/disposable@^1.4.3":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
 
 "@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6":
-  version "2.1.0"
-  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.0.tgz#54dfd2e8f361570b08751784b80751056816c66f"
-  integrity sha512-BFSNoNKxdX/qpN8cvL+5/I3MErzBUZYlqLuURSp4aTnqkVg4fYVOUo3E8fD/V9zQRu9pX0WzgTl8H0w0uVK6Gg==
+  version "2.1.1"
+  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.1.tgz#9c6dace68320538532ebd4fb91b159c532baf62e"
+  integrity sha512-zGl5hDDgDgPlrCN8b37gmNRjmYrTXnVq4WaseRtEgjj/en+gHLQW7sgTzkLgPj5rFaVETPkyrDTQ5uZVewFOAw==
   dependencies:
-    "@lumino/signaling" "^2.1.0"
+    "@lumino/signaling" "^2.1.1"
 
 "@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
 "@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.5":
@@ -789,30 +810,30 @@
   version "1.11.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
   integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/properties" "^1.8.2"
 
-"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.0":
-  version "2.1.0"
-  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.0.tgz#82bddad7e074e757b5c9b5e0822278115f81beec"
-  integrity sha512-Vk2qPmuYn7TdEiqn/bmIrLNBaLmcuB09s+cI8FOxyEZvuW92fGP5P5H2C0rgqy9OT1mvZqobhkEvcCav8HdxxA==
+"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.1":
+  version "2.1.1"
+  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.1.tgz#aae22e4cfb8f99baaa54cefaf1555be2c4148f0f"
+  integrity sha512-EUPJlC/kis5DEPA4UxsJRPidGk4qcgS+rfQlYfGfA4Z6vR8nzcwU9WE0UIWdqo6GN7cLWR8lGLzZzyIGY3+qiA==
   dependencies:
     "@lumino/algorithm" "^2.0.0"
-    "@lumino/coreutils" "^2.1.0"
+    "@lumino/coreutils" "^2.1.1"
 
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
 
-"@lumino/widgets@^1.37.2":
+"@lumino/widgets@1.37.2", "@lumino/widgets@^1.37.2", "@lumino/widgets@^1.37.2 || ^2.1.1":
   version "1.37.2"
   resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.2.tgz#b408fae221ecec2f1b028607782fbe1e82588bce"
   integrity sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
@@ -887,40 +908,40 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
   integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.37.0"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.37.0.tgz#29cebc6c2a3ac7fea7113207bf5a828fdf4d7ef1"
-  integrity sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==
+  version "8.44.0"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.44.0.tgz#55818eabb376e2272f77fbf5c96c43137c3c1e53"
+  integrity sha512-gsF+c/0XOguWgaOgvFs+xnnRqt9GwgTvIks36WpE6ueeI4KCEHHd8K/CKHqhOqrJKsYH8m27kRzQEvWXAwXUTw==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*", "@types/estree@^1.0.0":
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
   integrity sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==
 
 "@types/json-schema@*", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.7", "@types/json-schema@^7.0.8":
-  version "7.0.11"
-  resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.11.tgz#d421b6c527a3037f7c84433fd2c4229e016863d3"
-  integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
+  version "7.0.12"
+  resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.12.tgz#d70faba7039d5fca54c83c7dbab41051d2b6f6cb"
+  integrity sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "18.15.11"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-18.15.11.tgz#b3b790f09cb1696cffcec605de025b088fa4225f"
-  integrity sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==
+  version "20.4.1"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.1.tgz#a6033a8718653c50ac4962977e14d0f984d9527d"
+  integrity sha512-JIzsAvJeA/5iY6Y/OxZbv1lUcc8dNSE77lb2gnBH+/PJ3lFR1Ccvgwl5JWnHAkNHcRsT0TbpVOsiMKZ1F/yyJg==
 
 "@types/node@^17.0.29":
   version "17.0.45"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-17.0.45.tgz#2c0fafd78705e7a18b7906b5201a522719dc5190"
   integrity sha512-w+tIMs3rq2afQdsPJlODhoUEKzFP1ayaoyl1CcnwtIlsVe7K7bA1NGm4s3PraqTLlXnbIN84zuBlxBWo1u9BLw==
 
 "@types/normalize-package-data@^2.4.0":
@@ -935,17 +956,17 @@
 
 "@types/prop-types@*":
   version "15.7.5"
   resolved "https://registry.yarnpkg.com/@types/prop-types/-/prop-types-15.7.5.tgz#5f19d2b85a98e9558036f6a3cacc8819420f05cf"
   integrity sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==
 
 "@types/react@^17.0.0":
-  version "17.0.58"
-  resolved "https://registry.yarnpkg.com/@types/react/-/react-17.0.58.tgz#c8bbc82114e5c29001548ebe8ed6c4ba4d3c9fb0"
-  integrity sha512-c1GzVY97P0fGxwGxhYq989j4XwlcHQoto6wQISOC2v6wm3h0PORRWJFHlkRjfGsiG3y1609WdQ+J+tKxvrEd6A==
+  version "17.0.62"
+  resolved "https://registry.yarnpkg.com/@types/react/-/react-17.0.62.tgz#2efe8ddf8533500ec44b1334dd1a97caa2f860e3"
+  integrity sha512-eANCyz9DG8p/Vdhr0ZKST8JV12PhH2ACCDYlFw6DIO+D+ca+uP4jtEDEpVqXZrh/uZdXQGwk7whJa3ah5DtyLw==
   dependencies:
     "@types/prop-types" "*"
     "@types/scheduler" "*"
     csstype "^3.0.2"
 
 "@types/scheduler@*":
   version "0.16.3"
@@ -1039,133 +1060,133 @@
   version "4.33.0"
   resolved "https://registry.yarnpkg.com/@typescript-eslint/visitor-keys/-/visitor-keys-4.33.0.tgz#2a22f77a41604289b7a186586e9ec48ca92ef1dd"
   integrity sha512-uqi/2aSz9g2ftcHWf8uLPJA70rUv6yuMW5Bohw+bwcuzaxQIHaKFZCKGoGXIrc9vkTJ3+0txM73K0Hq3d5wgIg==
   dependencies:
     "@typescript-eslint/types" "4.33.0"
     eslint-visitor-keys "^2.0.0"
 
-"@webassemblyjs/ast@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.1.tgz#2bfd767eae1a6996f432ff7e8d7fc75679c0b6a7"
-  integrity sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==
+"@webassemblyjs/ast@1.11.6", "@webassemblyjs/ast@^1.11.5":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.6.tgz#db046555d3c413f8966ca50a95176a0e2c642e24"
+  integrity sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==
+  dependencies:
+    "@webassemblyjs/helper-numbers" "1.11.6"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
+
+"@webassemblyjs/floating-point-hex-parser@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz#dacbcb95aff135c8260f77fa3b4c5fea600a6431"
+  integrity sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==
+
+"@webassemblyjs/helper-api-error@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz#6132f68c4acd59dcd141c44b18cbebbd9f2fa768"
+  integrity sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==
+
+"@webassemblyjs/helper-buffer@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz#b66d73c43e296fd5e88006f18524feb0f2c7c093"
+  integrity sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==
+
+"@webassemblyjs/helper-numbers@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz#cbce5e7e0c1bd32cf4905ae444ef64cea919f1b5"
+  integrity sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==
   dependencies:
-    "@webassemblyjs/helper-numbers" "1.11.1"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
-
-"@webassemblyjs/floating-point-hex-parser@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz#f6c61a705f0fd7a6aecaa4e8198f23d9dc179e4f"
-  integrity sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==
-
-"@webassemblyjs/helper-api-error@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz#1a63192d8788e5c012800ba6a7a46c705288fd16"
-  integrity sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==
-
-"@webassemblyjs/helper-buffer@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz#832a900eb444884cde9a7cad467f81500f5e5ab5"
-  integrity sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==
-
-"@webassemblyjs/helper-numbers@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz#64d81da219fbbba1e3bd1bfc74f6e8c4e10a62ae"
-  integrity sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==
-  dependencies:
-    "@webassemblyjs/floating-point-hex-parser" "1.11.1"
-    "@webassemblyjs/helper-api-error" "1.11.1"
+    "@webassemblyjs/floating-point-hex-parser" "1.11.6"
+    "@webassemblyjs/helper-api-error" "1.11.6"
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/helper-wasm-bytecode@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz#f328241e41e7b199d0b20c18e88429c4433295e1"
-  integrity sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==
-
-"@webassemblyjs/helper-wasm-section@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz#21ee065a7b635f319e738f0dd73bfbda281c097a"
-  integrity sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/helper-buffer" "1.11.1"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
-    "@webassemblyjs/wasm-gen" "1.11.1"
-
-"@webassemblyjs/ieee754@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz#963929e9bbd05709e7e12243a099180812992614"
-  integrity sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==
+"@webassemblyjs/helper-wasm-bytecode@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz#bb2ebdb3b83aa26d9baad4c46d4315283acd51e9"
+  integrity sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==
+
+"@webassemblyjs/helper-wasm-section@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz#ff97f3863c55ee7f580fd5c41a381e9def4aa577"
+  integrity sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/helper-buffer" "1.11.6"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
+    "@webassemblyjs/wasm-gen" "1.11.6"
+
+"@webassemblyjs/ieee754@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz#bb665c91d0b14fffceb0e38298c329af043c6e3a"
+  integrity sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==
   dependencies:
     "@xtuc/ieee754" "^1.2.0"
 
-"@webassemblyjs/leb128@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.1.tgz#ce814b45574e93d76bae1fb2644ab9cdd9527aa5"
-  integrity sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==
+"@webassemblyjs/leb128@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.6.tgz#70e60e5e82f9ac81118bc25381a0b283893240d7"
+  integrity sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==
   dependencies:
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/utf8@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.1.tgz#d1f8b764369e7c6e6bae350e854dec9a59f0a3ff"
-  integrity sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==
-
-"@webassemblyjs/wasm-edit@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz#ad206ebf4bf95a058ce9880a8c092c5dec8193d6"
-  integrity sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/helper-buffer" "1.11.1"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
-    "@webassemblyjs/helper-wasm-section" "1.11.1"
-    "@webassemblyjs/wasm-gen" "1.11.1"
-    "@webassemblyjs/wasm-opt" "1.11.1"
-    "@webassemblyjs/wasm-parser" "1.11.1"
-    "@webassemblyjs/wast-printer" "1.11.1"
-
-"@webassemblyjs/wasm-gen@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz#86c5ea304849759b7d88c47a32f4f039ae3c8f76"
-  integrity sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
-    "@webassemblyjs/ieee754" "1.11.1"
-    "@webassemblyjs/leb128" "1.11.1"
-    "@webassemblyjs/utf8" "1.11.1"
-
-"@webassemblyjs/wasm-opt@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz#657b4c2202f4cf3b345f8a4c6461c8c2418985f2"
-  integrity sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/helper-buffer" "1.11.1"
-    "@webassemblyjs/wasm-gen" "1.11.1"
-    "@webassemblyjs/wasm-parser" "1.11.1"
-
-"@webassemblyjs/wasm-parser@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz#86ca734534f417e9bd3c67c7a1c75d8be41fb199"
-  integrity sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==
+"@webassemblyjs/utf8@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.6.tgz#90f8bc34c561595fe156603be7253cdbcd0fab5a"
+  integrity sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==
+
+"@webassemblyjs/wasm-edit@^1.11.5":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz#c72fa8220524c9b416249f3d94c2958dfe70ceab"
+  integrity sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/helper-buffer" "1.11.6"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
+    "@webassemblyjs/helper-wasm-section" "1.11.6"
+    "@webassemblyjs/wasm-gen" "1.11.6"
+    "@webassemblyjs/wasm-opt" "1.11.6"
+    "@webassemblyjs/wasm-parser" "1.11.6"
+    "@webassemblyjs/wast-printer" "1.11.6"
+
+"@webassemblyjs/wasm-gen@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz#fb5283e0e8b4551cc4e9c3c0d7184a65faf7c268"
+  integrity sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
+    "@webassemblyjs/ieee754" "1.11.6"
+    "@webassemblyjs/leb128" "1.11.6"
+    "@webassemblyjs/utf8" "1.11.6"
+
+"@webassemblyjs/wasm-opt@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz#d9a22d651248422ca498b09aa3232a81041487c2"
+  integrity sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/helper-buffer" "1.11.6"
+    "@webassemblyjs/wasm-gen" "1.11.6"
+    "@webassemblyjs/wasm-parser" "1.11.6"
+
+"@webassemblyjs/wasm-parser@1.11.6", "@webassemblyjs/wasm-parser@^1.11.5":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz#bb85378c527df824004812bbdb784eea539174a1"
+  integrity sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/helper-api-error" "1.11.6"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
+    "@webassemblyjs/ieee754" "1.11.6"
+    "@webassemblyjs/leb128" "1.11.6"
+    "@webassemblyjs/utf8" "1.11.6"
+
+"@webassemblyjs/wast-printer@1.11.6":
+  version "1.11.6"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz#a7bf8dd7e362aeb1668ff43f35cb849f188eff20"
+  integrity sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==
   dependencies:
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/helper-api-error" "1.11.1"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
-    "@webassemblyjs/ieee754" "1.11.1"
-    "@webassemblyjs/leb128" "1.11.1"
-    "@webassemblyjs/utf8" "1.11.1"
-
-"@webassemblyjs/wast-printer@1.11.1":
-  version "1.11.1"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz#d0c73beda8eec5426f10ae8ef55cee5e7084c2f0"
-  integrity sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/ast" "1.11.6"
     "@xtuc/long" "4.2.2"
 
 "@webpack-cli/configtest@^1.2.0":
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/@webpack-cli/configtest/-/configtest-1.2.0.tgz#7b20ce1c12533912c3b217ea68262365fa29a6f5"
   integrity sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==
 
@@ -1214,33 +1235,33 @@
   dependencies:
     buffer "^5.5.0"
     immediate "^3.2.3"
     level-concat-iterator "~2.0.0"
     level-supports "~1.0.0"
     xtend "~4.0.0"
 
-acorn-import-assertions@^1.7.6:
-  version "1.8.0"
-  resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz#ba2b5939ce62c238db6d93d81c9b111b29b855e9"
-  integrity sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==
+acorn-import-assertions@^1.9.0:
+  version "1.9.0"
+  resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz#507276249d684797c84e0734ef84860334cfb1ac"
+  integrity sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==
 
 acorn-jsx@^5.3.1:
   version "5.3.2"
   resolved "https://registry.yarnpkg.com/acorn-jsx/-/acorn-jsx-5.3.2.tgz#7ed5bb55908b3b2f1bc55c6af1653bada7f07937"
   integrity sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==
 
 acorn@^7.4.0:
   version "7.4.1"
   resolved "https://registry.yarnpkg.com/acorn/-/acorn-7.4.1.tgz#feaed255973d2e77555b83dbc08851a6c63520fa"
   integrity sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==
 
-acorn@^8.5.0, acorn@^8.7.1:
-  version "8.8.2"
-  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.2.tgz#1b2f25db02af965399b9776b0c2c391276d37c4a"
-  integrity sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==
+acorn@^8.7.1, acorn@^8.8.2:
+  version "8.10.0"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.10.0.tgz#8be5b3907a67221a81ab23c7889c4c5526b62ec5"
+  integrity sha512-F0SAmZ8iUtS//m8DmCTA0jlh6TDKkHQyK6xc6V4KDTyZKA9dnvX9/3sRTVQrWm79glUAZbnmmNcdYwUIHWVybw==
 
 aggregate-error@^3.0.0:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/aggregate-error/-/aggregate-error-3.1.0.tgz#92670ff50f5359bdb7a3e0d40d0ec30c5737687a"
   integrity sha512-4I7Td01quW/RpocfNayFdFVk1qSuoh0E7JrbRJ16nH01HhKFQ88INq9Sd+nd72zqRySlr9BmDA8xlEJ6vJMrYA==
   dependencies:
     clean-stack "^2.0.0"
@@ -1379,22 +1400,22 @@
   version "3.0.2"
   resolved "https://registry.yarnpkg.com/braces/-/braces-3.0.2.tgz#3454e1a462ee8d599e236df336cd9ea4f8afe107"
   integrity sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==
   dependencies:
     fill-range "^7.0.1"
 
 browserslist@^4.14.5:
-  version "4.21.5"
-  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.5.tgz#75c5dae60063ee641f977e00edd3cfb2fb7af6a7"
-  integrity sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==
-  dependencies:
-    caniuse-lite "^1.0.30001449"
-    electron-to-chromium "^1.4.284"
-    node-releases "^2.0.8"
-    update-browserslist-db "^1.0.10"
+  version "4.21.9"
+  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.9.tgz#e11bdd3c313d7e2a9e87e8b4b0c7872b13897635"
+  integrity sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==
+  dependencies:
+    caniuse-lite "^1.0.30001503"
+    electron-to-chromium "^1.4.431"
+    node-releases "^2.0.12"
+    update-browserslist-db "^1.0.11"
 
 buffer-from@^1.0.0:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
 buffer@^5.5.0, buffer@^5.6.0:
@@ -1460,18 +1481,18 @@
     quick-lru "^4.0.1"
 
 camelcase@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-5.3.1.tgz#e3c9b31569e106811df242f715725a1f4c494320"
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
-caniuse-lite@^1.0.30001449:
-  version "1.0.30001480"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001480.tgz#9bbd35ee44c2480a1e3a3b9f4496f5066817164a"
-  integrity sha512-q7cpoPPvZYgtyC4VaBSN0Bt+PJ4c4EYRf0DrduInOz2SkFpHD5p3LnvEpqBp7UnJn+8x1Ogl1s38saUxe+ihQQ==
+caniuse-lite@^1.0.30001503:
+  version "1.0.30001515"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001515.tgz#418aefeed9d024cd3129bfae0ccc782d4cb8f12b"
+  integrity sha512-eEFDwUOZbE24sb+Ecsx3+OvNETqjWIdabMy52oOkIgcUtAsQifjUG9q4U9dgTHJM2mfk4uEPxc0+xuFdJ629QA==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -1595,17 +1616,17 @@
 
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
   integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
 core-js-pure@^3.6.5:
-  version "3.30.1"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.30.1.tgz#7d93dc89e7d47b8ef05d7e79f507b0e99ea77eec"
-  integrity sha512-nXBEVpmUnNRhz83cHd9JRQC52cTMcuXAmR56+9dSMpRdpeA4I1PX6yjmhd71Eyc/wXNsdBdUDIj1QTIeZpU5Tg==
+  version "3.31.1"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.31.1.tgz#73d154958881873bc19381df80bddb20c8d0cdb5"
+  integrity sha512-w+C62kvWti0EPs4KPMCMVv9DriHSXfQOCQ94bGGBiEW5rrbtt/Rz8n5Krhfw9cpFyzXBjf3DB3QnPdEzGDY4Fw==
 
 cosmiconfig@^7.1.0:
   version "7.1.0"
   resolved "https://registry.yarnpkg.com/cosmiconfig/-/cosmiconfig-7.1.0.tgz#1443b9afa596b670082ea46cbd8f6a62b84635f6"
   integrity sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==
   dependencies:
     "@types/parse-json" "^4.0.0"
@@ -1631,17 +1652,17 @@
   integrity sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==
   dependencies:
     path-key "^3.1.0"
     shebang-command "^2.0.0"
     which "^2.0.1"
 
 css-functions-list@^3.1.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/css-functions-list/-/css-functions-list-3.1.0.tgz#cf5b09f835ad91a00e5959bcfc627cd498e1321b"
-  integrity sha512-/9lCvYZaUbBGvYUgYGFJ4dcYiyqdhSjG7IPVluoV8A1ILjkF7ilmhp1OGUz8n+nmBcu0RNrQAzgD8B6FJbrt2w==
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/css-functions-list/-/css-functions-list-3.2.0.tgz#8290b7d064bf483f48d6559c10e98dc4d1ad19ee"
+  integrity sha512-d/jBMPyYybkkLVypgtGv12R+pIFw4/f/IHtCTxWpZc8ofTYOPigIgmA6vu5rMHartZC+WuXhBUHfnyNUIQSYrg==
 
 css-loader@^5.0.1:
   version "5.2.7"
   resolved "https://registry.yarnpkg.com/css-loader/-/css-loader-5.2.7.tgz#9b9f111edf6fb2be5dc62525644cbc9c232064ae"
   integrity sha512-Q7mOvpBNBG7YrVGMxRxcBJZFL75o+cH2abNASdibkj/fffYD8qWbInZrD0S9ccI6vZclF3DsHE7njGlLtaHbhg==
   dependencies:
     icss-utils "^5.1.0"
@@ -1804,18 +1825,18 @@
   integrity sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
-electron-to-chromium@^1.4.284:
-  version "1.4.368"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.368.tgz#75901f97d3e23da2e66feb1e61fbb8e70ac96430"
-  integrity sha512-e2aeCAixCj9M7nJxdB/wDjO6mbYX+lJJxSJCXDzlr5YPGYVofuJwGN9nKg2o6wWInjX6XmxRinn3AeJMK81ltw==
+electron-to-chromium@^1.4.431:
+  version "1.4.457"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.457.tgz#3fdc7b4f97d628ac6b51e8b4b385befb362fe343"
+  integrity sha512-/g3UyNDmDd6ebeWapmAoiyy+Sy2HyJ+/X8KyvNeHfKRFfHaA2W8oF5fxD5F3tjBDcjpwo0iek6YNgxNXDBoEtA==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
@@ -1829,18 +1850,18 @@
   integrity sha512-QKrV0iKR6MZVJV08QY0wp1e7vF6QbhnbQhb07bwpEyuz4uZiZgPlEGdkCROuFkUwdxlFaiPIhjyarH1ee/3vhw==
   dependencies:
     abstract-leveldown "^6.2.1"
     inherits "^2.0.3"
     level-codec "^9.0.0"
     level-errors "^2.0.0"
 
-enhanced-resolve@^5.10.0:
-  version "5.12.0"
-  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz#300e1c90228f5b570c4d35babf263f6da7155634"
-  integrity sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==
+enhanced-resolve@^5.15.0:
+  version "5.15.0"
+  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz#1af946c7d93603eb88e9896cee4904dc012e9c35"
+  integrity sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 enquirer@^2.3.5:
   version "2.3.6"
   resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.3.6.tgz#2a7fe5dd634a1e4125a975ec994ff5456dc3734d"
@@ -1850,17 +1871,17 @@
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-2.2.0.tgz#098dc90ebb83d8dffa089d55256b351d34c4da55"
   integrity sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==
 
 envinfo@^7.7.3:
-  version "7.8.1"
-  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.8.1.tgz#06377e3e5f4d379fea7ac592d5ad8927e0c4d475"
-  integrity sha512-/o+BXHmB7ocbHEAs6F2EnG0ogybVVUdkRunTT2glZU9XAaGmhqskrvKwqXuDfNjEO0LZKWdejEEpnq8aM0tOaw==
+  version "7.10.0"
+  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.10.0.tgz#55146e3909cc5fe63c22da63fb15b05aeac35b13"
+  integrity sha512-ZtUjZO6l5mwTHvc1L9+1q5p/R3wTopcfqMW8r5t8SJSKqeVI/LtajORwRFEKpEFuekjD0VBjwu1HMxL4UalIRw==
 
 errno@~0.1.1:
   version "0.1.8"
   resolved "https://registry.yarnpkg.com/errno/-/errno-0.1.8.tgz#8bb3e9c7d463be4976ff888f76b4809ebc2e811f"
   integrity sha512-dJ6oBr5SQ1VSd9qkk7ByRgb/1SH4JZjCHSW/mr63/QcXO9zLVxvJ6Oy13nio03rxpSnVDDjFor75SjVeZWPW/A==
   dependencies:
     prr "~1.0.1"
@@ -1909,17 +1930,17 @@
     string.prototype.trimend "^1.0.6"
     string.prototype.trimstart "^1.0.6"
     typed-array-length "^1.0.4"
     unbox-primitive "^1.0.2"
     which-typed-array "^1.1.9"
 
 es-module-lexer@^1.2.1:
-  version "1.2.1"
-  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.2.1.tgz#ba303831f63e6a394983fde2f97ad77b22324527"
-  integrity sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==
+  version "1.3.0"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.3.0.tgz#6be9c9e0b4543a60cd166ff6f8b4e9dae0b0c16f"
+  integrity sha512-vZK7T0N2CBmBOixhmjdqx2gWVbFZ4DXZ/NyRMZVlJXPa7CyFS+/a4QQsDGDQy9ZfEzxFuNEsMLeQJnKP2p5/JA==
 
 es-set-tostringtag@^2.0.1:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/es-set-tostringtag/-/es-set-tostringtag-2.0.1.tgz#338d502f6f674301d710b80c8592de8a15f09cd8"
   integrity sha512-g3OMbtlwY3QewlqAiMLI47KywjWZoEytKr8pf6iTC8uJq5bIAH52Z9pnQ8pVL6whrCto53JZDuUIsifGeLorTg==
   dependencies:
     get-intrinsic "^1.1.3"
@@ -2092,22 +2113,22 @@
 
 fast-deep-equal@^3.1.1, fast-deep-equal@^3.1.3:
   version "3.1.3"
   resolved "https://registry.yarnpkg.com/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz#3a7d56b559d6cbc3eb512325244e619a65c6c525"
   integrity sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==
 
 fast-diff@^1.1.2:
-  version "1.2.0"
-  resolved "https://registry.yarnpkg.com/fast-diff/-/fast-diff-1.2.0.tgz#73ee11982d86caaf7959828d519cfe927fac5f03"
-  integrity sha512-xJuoT5+L99XlZ8twedaRf6Ax2TgQVxvgZOYoPKqZufmJib0tL2tegPBOZb1pVNgIhlqDlA0eO0c3wBvQcmzx4w==
+  version "1.3.0"
+  resolved "https://registry.yarnpkg.com/fast-diff/-/fast-diff-1.3.0.tgz#ece407fa550a64d638536cd727e129c61616e0f0"
+  integrity sha512-VxPP4NqbUjj6MaAOafWeUn2cXWLcCtljklUtZf0Ind4XQ+QPtmA0b18zZy0jIQx+ExRVCR/ZQpBmik5lXshNsw==
 
 fast-glob@^3.2.12, fast-glob@^3.2.9:
-  version "3.2.12"
-  resolved "https://registry.yarnpkg.com/fast-glob/-/fast-glob-3.2.12.tgz#7f39ec99c2e6ab030337142da9e0c18f37afae80"
-  integrity sha512-DVj4CQIYYow0BlaelwK1pHl5n5cRSJfM60UA0zK891sVInoPri2Ekj7+e1CT3/3qxXenpI+nBBmQAcJPJgaj4w==
+  version "3.3.0"
+  resolved "https://registry.yarnpkg.com/fast-glob/-/fast-glob-3.3.0.tgz#7c40cb491e1e2ed5664749e87bfb516dbe8727c0"
+  integrity sha512-ChDuvbOypPuNjO8yIDf36x7BlZX1smcUMTTcyoIjycexOxd6DFsKsg21qVBzEmr3G7fUKIRy2/psii+CIUt7FA==
   dependencies:
     "@nodelib/fs.stat" "^2.0.2"
     "@nodelib/fs.walk" "^1.2.3"
     glob-parent "^5.1.2"
     merge2 "^1.3.0"
     micromatch "^4.0.4"
 
@@ -2251,20 +2272,21 @@
 
 functions-have-names@^1.2.2, functions-have-names@^1.2.3:
   version "1.2.3"
   resolved "https://registry.yarnpkg.com/functions-have-names/-/functions-have-names-1.2.3.tgz#0404fe4ee2ba2f607f0e0ec3c80bae994133b834"
   integrity sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==
 
 get-intrinsic@^1.0.2, get-intrinsic@^1.1.1, get-intrinsic@^1.1.3, get-intrinsic@^1.2.0:
-  version "1.2.0"
-  resolved "https://registry.yarnpkg.com/get-intrinsic/-/get-intrinsic-1.2.0.tgz#7ad1dc0535f3a2904bba075772763e5051f6d05f"
-  integrity sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==
+  version "1.2.1"
+  resolved "https://registry.yarnpkg.com/get-intrinsic/-/get-intrinsic-1.2.1.tgz#d295644fed4505fc9cde952c37ee12b477a83d82"
+  integrity sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==
   dependencies:
     function-bind "^1.1.1"
     has "^1.0.3"
+    has-proto "^1.0.1"
     has-symbols "^1.0.3"
 
 get-stdin@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/get-stdin/-/get-stdin-6.0.0.tgz#9e09bf712b360ab9225e812048f71fde9c89657b"
   integrity sha512-jp4tHawyV7+fkkSKyvjuLZswblUtz+SQKzSWnBbii16BuZksJlU1wuBYXY75r+duh/llF1ur6oNwi+2ZzjKZ7g==
 
@@ -2593,17 +2615,17 @@
 
 is-callable@^1.1.3, is-callable@^1.1.4, is-callable@^1.2.7:
   version "1.2.7"
   resolved "https://registry.yarnpkg.com/is-callable/-/is-callable-1.2.7.tgz#3bc2a85ea742d9e36205dcacdd72ca1fdc51b055"
   integrity sha512-1BC0BVFhS/p0qtw6enp8e+8OD0UrK0oFLztSjNzhcKA3WDuJxxAPXzPuPtKkjEY9UUoEWlX/8fgKeu2S8i9JTA==
 
 is-core-module@^2.11.0, is-core-module@^2.5.0:
-  version "2.12.0"
-  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.12.0.tgz#36ad62f6f73c8253fd6472517a12483cf03e7ec4"
-  integrity sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==
+  version "2.12.1"
+  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.12.1.tgz#0c0b6885b6f80011c71541ce15c8d66cf5a4f9fd"
+  integrity sha512-Q4ZuBAe2FUsKtyQJoQHlvP8OvBERxO3jEmy1I7hcRXcJBGGHFh/aJBswbXuS9sgrDH2QUO8ilkwNPHvHMd8clg==
   dependencies:
     has "^1.0.3"
 
 is-date-object@^1.0.1:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/is-date-object/-/is-date-object-1.0.5.tgz#0841d5536e724c25597bf6ea62e1bd38298df31f"
   integrity sha512-9YQaSxsAiSwcvS33MBk3wTCVnWK+HhF8VZR2jRxehM16QcVOdHqPn4VPHmRK4lSr38n9JriurInLcP90xsYNfQ==
@@ -2817,14 +2839,19 @@
     graceful-fs "^4.1.6"
 
 jsonpointer@^5.0.0:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/jsonpointer/-/jsonpointer-5.0.1.tgz#2110e0af0900fd37467b5907ecd13a7884a1b559"
   integrity sha512-p/nXbhSEcu3pZRdkW1OfJhpsVtW1gd4Wa1fnQc9YLiTfAjn0312eMKimbdIQzuZl9aa9xUGaRlP9T/CJE/ditQ==
 
+jwt-decode@^3.1.2:
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/jwt-decode/-/jwt-decode-3.1.2.tgz#3fb319f3675a2df0c2895c8f5e9fa4b67b04ed59"
+  integrity sha512-UfpWE/VZn0iP50d8cz9NrZLM9lSWhcJ+0Gt/nm4by88UL+J1SiKN8/5dkjMmbEzwL2CAe+67GsegCbIKtbp75A==
+
 kind-of@^6.0.2, kind-of@^6.0.3:
   version "6.0.3"
   resolved "https://registry.yarnpkg.com/kind-of/-/kind-of-6.0.3.tgz#07c05034a6c349fa06e24fa35aa76db4580ce4dd"
   integrity sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==
 
 known-css-properties@^0.26.0:
   version "0.26.0"
@@ -2917,18 +2944,18 @@
   version "0.4.1"
   resolved "https://registry.yarnpkg.com/levn/-/levn-0.4.1.tgz#ae4562c007473b932a6200d403268dd2fffc6ade"
   integrity sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==
   dependencies:
     prelude-ls "^1.2.1"
     type-check "~0.4.0"
 
-lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52, lib0@^0.2.72:
-  version "0.2.73"
-  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.73.tgz#af7d7ce9ad523fa3e241d437cc3ab1862f9a1f29"
-  integrity sha512-aJJIElCLWnHMcYZPtsM07QoSfHwpxCy4VUzBYGXFYEmh/h2QS5uZNbCCfL0CqnkOE30b7Tp9DVfjXag+3qzZjQ==
+lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52, lib0@^0.2.74:
+  version "0.2.78"
+  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.78.tgz#9aa34733075caafb3edf228da6e609d15ada0088"
+  integrity sha512-SV2nU43/6eaYnGH3l0lg2wg1ziB/TH3sAd2E8quXPGwrqo+aX98SNT2ZKucpUr5B8A52jD7ZMjAl+r87Fa/bLQ==
   dependencies:
     isomorphic.js "^0.2.4"
 
 license-webpack-plugin@^2.3.14:
   version "2.3.21"
   resolved "https://registry.yarnpkg.com/license-webpack-plugin/-/license-webpack-plugin-2.3.21.tgz#152f5e82d5f51f8bab78905731f2b8042aa5691b"
   integrity sha512-rVaYU9TddZN3ao8M/0PrRSCdTp2EW6VQymlgsuScld1vef0Ou7fALx3ePe83KLP3xAEDcPK5fkqUVqGBnbz1zQ==
@@ -3164,18 +3191,18 @@
 minipass@^3.0.0, minipass@^3.1.1:
   version "3.3.6"
   resolved "https://registry.yarnpkg.com/minipass/-/minipass-3.3.6.tgz#7bba384db3a1520d18c9c0e5251c3444e95dd94a"
   integrity sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==
   dependencies:
     yallist "^4.0.0"
 
-minipass@^4.0.0:
-  version "4.2.8"
-  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.8.tgz#f0010f64393ecfc1d1ccb5f582bcaf45f48e1a3a"
-  integrity sha512-fNzuVyifolSLFL4NzpF+wEF4qrgqaaKX0haXPQEdQ7NKAN+WecoKMHV09YcuL/DHxrUsYQOK3MiuDf7Ip2OXfQ==
+minipass@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-5.0.0.tgz#3e9788ffb90b694a5d0ec94479a45b5d8738133d"
+  integrity sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==
 
 minizlib@^2.1.1:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/minizlib/-/minizlib-2.1.2.tgz#e90d3466ba209b932451508a11ce3d3632145931"
   integrity sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==
   dependencies:
     minipass "^3.0.0"
@@ -3218,29 +3245,29 @@
 
 nice-try@^1.0.4:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/nice-try/-/nice-try-1.0.5.tgz#a3378a7696ce7d223e88fc9b764bd7ef1089e366"
   integrity sha512-1nh45deeb5olNY7eX82BkPO7SSxR5SSYJiPTrTdFUVYwAl8CKMA5N9PjTYkHiRjisVcxcQ1HXdLhx2qxxJzLNQ==
 
 node-fetch@^2.6.0:
-  version "2.6.9"
-  resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.9.tgz#7c7f744b5cc6eb5fd404e0c7a9fec630a55657e6"
-  integrity sha512-DJm/CJkZkRjKKj4Zi4BsKVZh3ValV5IR5s7LVZnW+6YMh0W1BfNA8XSs6DLMGYlId5F3KnA70uu2qepcR08Qqg==
+  version "2.6.12"
+  resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.12.tgz#02eb8e22074018e3d5a83016649d04df0e348fba"
+  integrity sha512-C/fGU2E8ToujUivIO0H+tpQ6HWo4eEmchoPIoXtxCrVghxdKq+QOHqEZW7tuP3KlV3bC8FRMO5nMCC7Zm1VP6g==
   dependencies:
     whatwg-url "^5.0.0"
 
 node-gyp-build@~4.1.0:
   version "4.1.1"
   resolved "https://registry.yarnpkg.com/node-gyp-build/-/node-gyp-build-4.1.1.tgz#d7270b5d86717068d114cc57fff352f96d745feb"
   integrity sha512-dSq1xmcPDKPZ2EED2S6zw/b9NKsqzXRE6dVr8TVQnI3FJOTteUMuqF3Qqs6LZg+mLGYJWqQzMbIjMtJqTv87nQ==
 
-node-releases@^2.0.8:
-  version "2.0.10"
-  resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.10.tgz#c311ebae3b6a148c89b1813fd7c4d3c024ef537f"
-  integrity sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==
+node-releases@^2.0.12:
+  version "2.0.13"
+  resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.13.tgz#d5ed1627c23e3461e819b02e57b75e4899b1c81d"
+  integrity sha512-uYr7J37ae/ORWdZeQ1xxMJe3NtdmqMC/JZK+geofDrkLUApKRHPd18/TxtBOJ4A0/+uUIliorNrfYV6s1b02eQ==
 
 normalize-package-data@^2.3.2, normalize-package-data@^2.5.0:
   version "2.5.0"
   resolved "https://registry.yarnpkg.com/normalize-package-data/-/normalize-package-data-2.5.0.tgz#e66db1838b200c1dfc233225d12cb36520e234a8"
   integrity sha512-/5CMN3T0R4XTj4DcGaexo+roZSdSFW/0AOOTROrjxzCG1wrWXEsGbRKevjlIL+ZDE4sZlJr5ED4YW0yqmkK+eA==
   dependencies:
     hosted-git-info "^2.1.4"
@@ -3320,24 +3347,24 @@
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/once/-/once-1.4.0.tgz#583b1aa775961d4b113ac17d9c50baef9dd76bd1"
   integrity sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==
   dependencies:
     wrappy "1"
 
 optionator@^0.9.1:
-  version "0.9.1"
-  resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.9.1.tgz#4f236a6373dae0566a6d43e1326674f50c291499"
-  integrity sha512-74RlY5FCnhq4jRxVUPKDaRwrVNXMqsGsiW6AJw4XK8hmtm10wC0ypZBLw5IIp85NZMr91+qd1RvvENwg7jjRFw==
+  version "0.9.3"
+  resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.9.3.tgz#007397d44ed1872fdc6ed31360190f81814e2c64"
+  integrity sha512-JjCoypp+jKn1ttEFExxhetCKeJt9zhAgAve5FXHixTvFDW/5aEktX9bufBKLRRMdU7bNtpLfcGu94B3cdEJgjg==
   dependencies:
+    "@aashutoshrathi/word-wrap" "^1.2.3"
     deep-is "^0.1.3"
     fast-levenshtein "^2.0.6"
     levn "^0.4.1"
     prelude-ls "^1.2.1"
     type-check "^0.4.0"
-    word-wrap "^1.2.3"
 
 p-limit@^2.2.0:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/p-limit/-/p-limit-2.3.0.tgz#3dd33c647a214fdfffd835933eb086da0dc21db1"
   integrity sha512-//88mFWSJx8lxCzwdAABTJL2MyWB12+eIY7MDL2SqLmAkeKU9qxRvWuSyTjm3FUmpBEMuFfckAIqEaVGUDxb6w==
   dependencies:
     p-try "^2.0.0"
@@ -3479,17 +3506,17 @@
 
 postcss-modules-extract-imports@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.0.0.tgz#cda1f047c0ae80c97dbe28c3e76a43b88025741d"
   integrity sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==
 
 postcss-modules-local-by-default@^4.0.0:
-  version "4.0.0"
-  resolved "https://registry.yarnpkg.com/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.0.tgz#ebbb54fae1598eecfdf691a02b3ff3b390a5a51c"
-  integrity sha512-sT7ihtmGSF9yhm6ggikHdV0hlziDTX7oFoXtuVWeDd3hHObNkcHRo9V3yg7vCAY7cONyxJC/XXCmmiHHcvX7bQ==
+  version "4.0.3"
+  resolved "https://registry.yarnpkg.com/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.3.tgz#b08eb4f083050708998ba2c6061b50c2870ca524"
+  integrity sha512-2/u2zraspoACtrbFRnTijMiQtb4GW4BvatjaG/bCjYQo8kLTdevCUlwuBHx2sCnSyrI3x3qj4ZK1j5LQBgzmwA==
   dependencies:
     icss-utils "^5.0.0"
     postcss-selector-parser "^6.0.2"
     postcss-value-parser "^4.1.0"
 
 postcss-modules-scope@^3.0.0:
   version "3.0.0"
@@ -3512,30 +3539,30 @@
 
 postcss-safe-parser@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/postcss-safe-parser/-/postcss-safe-parser-6.0.0.tgz#bb4c29894171a94bc5c996b9a30317ef402adaa1"
   integrity sha512-FARHN8pwH+WiS2OPCxJI8FuRJpTVnn6ZNFiqAM2aeW2LwTHWWmWgIyKC6cUo0L8aeKiF/14MNvnpls6R2PBeMQ==
 
 postcss-selector-parser@^6.0.11, postcss-selector-parser@^6.0.2, postcss-selector-parser@^6.0.4:
-  version "6.0.11"
-  resolved "https://registry.yarnpkg.com/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz#2e41dc39b7ad74046e1615185185cd0b17d0c8dc"
-  integrity sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==
+  version "6.0.13"
+  resolved "https://registry.yarnpkg.com/postcss-selector-parser/-/postcss-selector-parser-6.0.13.tgz#d05d8d76b1e8e173257ef9d60b706a8e5e99bf1b"
+  integrity sha512-EaV1Gl4mUEV4ddhDnv/xtj7sxwrwxdetHdWUGnT4VJQf+4d05v6lHYZr8N573k5Z0BViss7BDhfWtKS3+sfAqQ==
   dependencies:
     cssesc "^3.0.0"
     util-deprecate "^1.0.2"
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11, postcss@^8.4.19:
-  version "8.4.22"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.22.tgz#c29e6776b60ab3af602d4b513d5bd2ff9aa85dc1"
-  integrity sha512-XseknLAfRHzVWjCEtdviapiBtfLdgyzExD50Rg2ePaucEesyh8Wv4VPdW0nbyDa1ydbrAxV19jvMT4+LFmcNUA==
+  version "8.4.25"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.25.tgz#4a133f5e379eda7f61e906c3b1aaa9b81292726f"
+  integrity sha512-7taJ/8t2av0Z+sQEvNzCkpDynl0tX3uJMCODi6nT3PfASC7dYCWV9aQ+uiCf+KBD4SEFcu+GvJdGdwzQ6OSjCw==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
@@ -3546,17 +3573,17 @@
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/prettier-linter-helpers/-/prettier-linter-helpers-1.0.0.tgz#d23d41fe1375646de2d0104d3454a3008802cf7b"
   integrity sha512-GbK2cP9nraSSUF9N2XwUwqfzlAFlMNYYl+ShE/V+H8a9uNl/oUqB1w2EL54Jh0OlyRSd8RfWYJ3coVS4TROP2w==
   dependencies:
     fast-diff "^1.1.2"
 
 prettier@^2.1.1:
-  version "2.8.7"
-  resolved "https://registry.yarnpkg.com/prettier/-/prettier-2.8.7.tgz#bb79fc8729308549d28fe3a98fce73d2c0656450"
-  integrity sha512-yPngTo3aXUUmyuTjeTUT75txrf+aMh9FiD7q9ZE/i6r0bPb22g4FsE6Y338PQX1bmfy08i9QQCB7/rcUAVntfw==
+  version "2.8.8"
+  resolved "https://registry.yarnpkg.com/prettier/-/prettier-2.8.8.tgz#e8c5d7e98a4305ffe3de2e1fc4aca1a71c28b1da"
+  integrity sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==
 
 process@^0.11.10:
   version "0.11.10"
   resolved "https://registry.yarnpkg.com/process/-/process-0.11.10.tgz#7332300e840161bda3e69a1d1d91a7d4bc16f182"
   integrity sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==
 
 progress@^2.0.0:
@@ -3579,28 +3606,30 @@
     react-is "^16.13.1"
 
 prr@~1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/prr/-/prr-1.0.1.tgz#d3fc114ba06995a45ec6893f484ceb1d78f5f476"
   integrity sha512-yPw4Sng1gWghHQWj0B3ZggWUm4qVbPwPFcRG8KyxiU7J2OHFSoEHKS+EZ3fv5l1t9CyCiop6l/ZYeWbrgoQejw==
 
-punycode@1.3.2:
-  version "1.3.2"
-  resolved "https://registry.yarnpkg.com/punycode/-/punycode-1.3.2.tgz#9653a036fb7c1ee42342f2325cceefea3926c48d"
-  integrity sha512-RofWgt/7fL5wP1Y7fxE7/EmTLzQVnB0ycyibJ0OOHIlJqTNzglYFxVwETOcIoJqJmpDXJ9xImDv+Fq34F/d4Dw==
+punycode@^1.4.1:
+  version "1.4.1"
+  resolved "https://registry.yarnpkg.com/punycode/-/punycode-1.4.1.tgz#c0d5a63b2718800ad8e1eb0fa5269c84dd41845e"
+  integrity sha512-jmYNElW7yvO7TV33CjSmvSiE2yco3bV2czu/OzDKdMNVZQWfxCblURLhf+47syQRBntjfLdd/H0egrzIG+oaFQ==
 
 punycode@^2.1.0, punycode@^2.1.1:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/punycode/-/punycode-2.3.0.tgz#f67fa67c94da8f4d0cfff981aee4118064199b8f"
   integrity sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==
 
-querystring@0.2.0:
-  version "0.2.0"
-  resolved "https://registry.yarnpkg.com/querystring/-/querystring-0.2.0.tgz#b209849203bb25df820da756e747005878521620"
-  integrity sha512-X/xY82scca2tau62i9mDyU9K+I+djTMUsvwf7xnUX5GLvVzgJybOJf4Y6o9Zx3oJK/LSXg5tTZBjwzqVPaPO2g==
+qs@^6.11.0:
+  version "6.11.2"
+  resolved "https://registry.yarnpkg.com/qs/-/qs-6.11.2.tgz#64bea51f12c1f5da1bc01496f48ffcff7c69d7d9"
+  integrity sha512-tDNIz22aBzCDxLtVH++VnTfzxlfeK5CbqohpSqpJgj1Wg/cQbStNAz3NuqCs5vV+pjBsK4x4pN9HlVh7rcYRiA==
+  dependencies:
+    side-channel "^1.0.4"
 
 querystringify@^2.1.1:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/querystringify/-/querystringify-2.2.0.tgz#3345941b4153cb9d082d8eee4cda2016a9aef7f6"
   integrity sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==
 
 queue-microtask@^1.2.2:
@@ -3853,37 +3882,37 @@
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-2.7.1.tgz#1ca4f32d1b24c590c203b8e7a50bf0ea4cd394d7"
   integrity sha512-SHiNtMOUGWBQJwzISiVYKu82GiV4QYGePp3odlY1tuKO7gPtphAT5R/py0fA6xtbgLL/RvtJZnU9b8s0F1q0Xg==
   dependencies:
     "@types/json-schema" "^7.0.5"
     ajv "^6.12.4"
     ajv-keywords "^3.5.2"
 
-schema-utils@^3.0.0, schema-utils@^3.1.0, schema-utils@^3.1.1:
-  version "3.1.2"
-  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.2.tgz#36c10abca6f7577aeae136c804b0c741edeadc99"
-  integrity sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==
+schema-utils@^3.0.0, schema-utils@^3.1.1, schema-utils@^3.2.0:
+  version "3.3.0"
+  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.3.0.tgz#f50a88877c3c01652a15b622ae9e9795df7a60fe"
+  integrity sha512-pN/yOAvcC+5rQ5nERGuwrjLlYvLTbCibnZ1I7B1LaiAz9BRBlE9GMgE/eqV30P7aJQUf7Ddimy/RsbYO/GrVGg==
   dependencies:
     "@types/json-schema" "^7.0.8"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
 
 "semver@2 || 3 || 4 || 5", semver@^5.4.1, semver@^5.5.0:
-  version "5.7.1"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.1.tgz#a954f931aeba508d307bbf069eff0c01c96116f7"
-  integrity sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==
+  version "5.7.2"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.2.tgz#48d55db737c3287cd4835e17fa13feace1c41ef8"
+  integrity sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==
 
 semver@^6.0.0:
-  version "6.3.0"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.0.tgz#ee0a64c8af5e8ceea67687b133761e1becbd1d3d"
-  integrity sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==
+  version "6.3.1"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.1.tgz#556d2ef8689146e46dcea4bfdd095f3434dffcb4"
+  integrity sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==
 
 semver@^7.2.1, semver@^7.3.4, semver@^7.3.5:
-  version "7.5.0"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.0.tgz#ed8c5dc8efb6c629c88b23d41dc9bf40c1d96cd0"
-  integrity sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==
+  version "7.5.4"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.4.tgz#483986ec4ed38e1c6c48c34894a9182dbff68a6e"
+  integrity sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==
   dependencies:
     lru-cache "^6.0.0"
 
 serialize-javascript@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-5.0.1.tgz#7886ec848049a462467a97d3d918ebb2aaf934f4"
   integrity sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==
@@ -4250,21 +4279,21 @@
 
 tapable@^2.1.1, tapable@^2.2.0:
   version "2.2.1"
   resolved "https://registry.yarnpkg.com/tapable/-/tapable-2.2.1.tgz#1967a73ef4060a82f12ab96af86d52fdb76eeca0"
   integrity sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==
 
 tar@^6.0.2:
-  version "6.1.13"
-  resolved "https://registry.yarnpkg.com/tar/-/tar-6.1.13.tgz#46e22529000f612180601a6fe0680e7da508847b"
-  integrity sha512-jdIBIN6LTIe2jqzay/2vtYLlBHa3JF42ot3h1dW8Q0PaAG4v8rm0cvpVePtau5C6OKXGGcgO9q2AMNSWxiLqKw==
+  version "6.1.15"
+  resolved "https://registry.yarnpkg.com/tar/-/tar-6.1.15.tgz#c9738b0b98845a3b344d334b8fa3041aaba53a69"
+  integrity sha512-/zKt9UyngnxIT/EAGYuxaMYgOIJiP81ab9ZfkILq4oNLPFX50qyYmu7jRj9qeXoxmJHjGlbH0+cm2uy1WCs10A==
   dependencies:
     chownr "^2.0.0"
     fs-minipass "^2.0.0"
-    minipass "^4.0.0"
+    minipass "^5.0.0"
     minizlib "^2.1.1"
     mkdirp "^1.0.3"
     yallist "^4.0.0"
 
 terser-webpack-plugin@^4.1.0:
   version "4.2.3"
   resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-4.2.3.tgz#28daef4a83bd17c1db0297070adc07fc8cfc6a9a"
@@ -4277,31 +4306,31 @@
     schema-utils "^3.0.0"
     serialize-javascript "^5.0.1"
     source-map "^0.6.1"
     terser "^5.3.4"
     webpack-sources "^1.4.3"
 
 terser-webpack-plugin@^5.3.7:
-  version "5.3.7"
-  resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz#ef760632d24991760f339fe9290deb936ad1ffc7"
-  integrity sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==
+  version "5.3.9"
+  resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz#832536999c51b46d468067f9e37662a3b96adfe1"
+  integrity sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
-    terser "^5.16.5"
+    terser "^5.16.8"
 
-terser@^5.16.5, terser@^5.3.4:
-  version "5.17.1"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.17.1.tgz#948f10830454761e2eeedc6debe45c532c83fd69"
-  integrity sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==
+terser@^5.16.8, terser@^5.3.4:
+  version "5.19.0"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.19.0.tgz#7b3137b01226bdd179978207b9c8148754a6da9c"
+  integrity sha512-JpcpGOQLOXm2jsomozdMDpd5f8ZHh1rR48OFgWUH3QsyZcfPgv2qDCYbcDEAYNd4OZRj2bWYKpwdll/udZCk/Q==
   dependencies:
-    "@jridgewell/source-map" "^0.3.2"
-    acorn "^8.5.0"
+    "@jridgewell/source-map" "^0.3.3"
+    acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 text-table@^0.2.0:
   version "0.2.0"
   resolved "https://registry.yarnpkg.com/text-table/-/text-table-0.2.0.tgz#7f5ee823ae805207c00af2df4a84ec3fcfa570b4"
   integrity sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==
@@ -4343,14 +4372,19 @@
   integrity sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==
 
 tslib@~2.3.1:
   version "2.3.1"
   resolved "https://registry.yarnpkg.com/tslib/-/tslib-2.3.1.tgz#e8a335add5ceae51aa261d32a490158ef042ef01"
   integrity sha512-77EbyPPpMz+FRFRuAFlWMtmgUWGe9UOG2Z25NqCwiIjRhOf5iKGuzSe5P2w1laq+FkRy4p+PCuVkJSGkzTEKVw==
 
+tslib@~2.5.0:
+  version "2.5.3"
+  resolved "https://registry.yarnpkg.com/tslib/-/tslib-2.5.3.tgz#24944ba2d990940e6e982c4bea147aba80209913"
+  integrity sha512-mSxlJJwl3BMEQCUNnxXBU9jP4JBktcEGhURcPR6VQVlnP0FdDEsIaz0C35dXNGLyRfrATNofF0F5p2KPxQgB+w==
+
 tsutils@^3.21.0:
   version "3.21.0"
   resolved "https://registry.yarnpkg.com/tsutils/-/tsutils-3.21.0.tgz#b48717d394cea6c1e096983eed58e9d61715b623"
   integrity sha512-mHKK3iUXL+3UF6xL5k0PEhKRUBKPBCv/+RkEOpjRWxxx27KKRBmmA60A9pgOUvMi8GKhRMPEmjBRPzs2W7O1OA==
   dependencies:
     tslib "^1.8.1"
 
@@ -4433,15 +4467,15 @@
     imurmurhash "^0.1.4"
 
 universalify@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/universalify/-/universalify-2.0.0.tgz#75a4984efedc4b08975c5aeb73f530d02df25717"
   integrity sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==
 
-update-browserslist-db@^1.0.10:
+update-browserslist-db@^1.0.11:
   version "1.0.11"
   resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz#9a2a641ad2907ae7b3616506f4b977851db5b940"
   integrity sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
 
@@ -4466,20 +4500,20 @@
   resolved "https://registry.yarnpkg.com/url-parse/-/url-parse-1.5.10.tgz#9d3c2f736c1d75dd3bd2be507dcc111f1e2ea9c1"
   integrity sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==
   dependencies:
     querystringify "^2.1.1"
     requires-port "^1.0.0"
 
 url@^0.11.0:
-  version "0.11.0"
-  resolved "https://registry.yarnpkg.com/url/-/url-0.11.0.tgz#3838e97cfc60521eb73c525a8e55bfdd9e2e28f1"
-  integrity sha512-kbailJa29QrtXnxgq+DdCEGlbTeYM2eJUxsz6vjZavrCYPMIFHMKQmSKYAIuUK2i7hgPm28a8piX5NTUtM/LKQ==
+  version "0.11.1"
+  resolved "https://registry.yarnpkg.com/url/-/url-0.11.1.tgz#26f90f615427eca1b9f4d6a28288c147e2302a32"
+  integrity sha512-rWS3H04/+mzzJkv0eZ7vEDGiQbgquI1fGfOad6zKvgYQi1SzMmhl7c/DdRGxhaWrVH6z0qWITo8rpnxK/RfEhA==
   dependencies:
-    punycode "1.3.2"
-    querystring "0.2.0"
+    punycode "^1.4.1"
+    qs "^6.11.0"
 
 util-deprecate@^1.0.1, util-deprecate@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/util-deprecate/-/util-deprecate-1.0.2.tgz#450d4dc9fa70de732762fbd2d4a28981419a0ccf"
   integrity sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==
 
 v8-compile-cache@^2.0.3, v8-compile-cache@^2.3.0:
@@ -4565,17 +4599,17 @@
     fastest-levenshtein "^1.0.12"
     import-local "^3.0.2"
     interpret "^2.2.0"
     rechoir "^0.7.0"
     webpack-merge "^5.7.3"
 
 webpack-merge@^5.1.2, webpack-merge@^5.7.3:
-  version "5.8.0"
-  resolved "https://registry.yarnpkg.com/webpack-merge/-/webpack-merge-5.8.0.tgz#2b39dbf22af87776ad744c390223731d30a68f61"
-  integrity sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==
+  version "5.9.0"
+  resolved "https://registry.yarnpkg.com/webpack-merge/-/webpack-merge-5.9.0.tgz#dc160a1c4cf512ceca515cc231669e9ddb133826"
+  integrity sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==
   dependencies:
     clone-deep "^4.0.1"
     wildcard "^2.0.0"
 
 webpack-sources@^1.1.0, webpack-sources@^1.2.0, webpack-sources@^1.4.3:
   version "1.4.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-1.4.3.tgz#eedd8ec0b928fbf1cbfe994e22d2d890f330a933"
@@ -4586,38 +4620,38 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.41.1:
-  version "5.79.0"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.79.0.tgz#8552b5da5a26e4e25842c08a883e08fc7740547a"
-  integrity sha512-3mN4rR2Xq+INd6NnYuL9RC9GAmc1ROPKJoHhrZ4pAjdMFEkJJWrsPw8o2JjCIyQyTu7rTXYn4VG6OpyB3CobZg==
+  version "5.88.1"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.88.1.tgz#21eba01e81bd5edff1968aea726e2fbfd557d3f8"
+  integrity sha512-FROX3TxQnC/ox4N+3xQoWZzvGXSuscxR32rbzjpXgEzWudJFEJBpdlkkob2ylrv5yzzufD1zph1OoFsLtm6stQ==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^1.0.0"
-    "@webassemblyjs/ast" "1.11.1"
-    "@webassemblyjs/wasm-edit" "1.11.1"
-    "@webassemblyjs/wasm-parser" "1.11.1"
+    "@webassemblyjs/ast" "^1.11.5"
+    "@webassemblyjs/wasm-edit" "^1.11.5"
+    "@webassemblyjs/wasm-parser" "^1.11.5"
     acorn "^8.7.1"
-    acorn-import-assertions "^1.7.6"
+    acorn-import-assertions "^1.9.0"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.10.0"
+    enhanced-resolve "^5.15.0"
     es-module-lexer "^1.2.1"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.2.9"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
-    schema-utils "^3.1.0"
+    schema-utils "^3.2.0"
     tapable "^2.1.1"
     terser-webpack-plugin "^5.3.7"
     watchpack "^2.4.0"
     webpack-sources "^3.2.3"
 
 whatwg-mimetype@^2.3.0:
   version "2.3.0"
@@ -4649,17 +4683,17 @@
     is-bigint "^1.0.1"
     is-boolean-object "^1.1.0"
     is-number-object "^1.0.4"
     is-string "^1.0.5"
     is-symbol "^1.0.3"
 
 which-typed-array@^1.1.9:
-  version "1.1.9"
-  resolved "https://registry.yarnpkg.com/which-typed-array/-/which-typed-array-1.1.9.tgz#307cf898025848cf995e795e8423c7f337efbde6"
-  integrity sha512-w9c4xkx6mPidwp7180ckYWfMmvxpjlZuIudNtDf4N/tTAUB8VJbX25qZoAsrtGuYNnGw3pa0AXgbGKRB8/EceA==
+  version "1.1.10"
+  resolved "https://registry.yarnpkg.com/which-typed-array/-/which-typed-array-1.1.10.tgz#74baa2789991905c2076abb317103b866c64e69e"
+  integrity sha512-uxoA5vLUfRPdjCuJ1h5LlYdmTLbYfums398v3WLkM+i/Wltl2/XyZpQWKbN++ck5L64SR/grOHqtXCUKmlZPNA==
   dependencies:
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
     for-each "^0.3.3"
     gopd "^1.0.1"
     has-tostringtag "^1.0.0"
     is-typed-array "^1.1.10"
@@ -4675,22 +4709,17 @@
   version "2.0.2"
   resolved "https://registry.yarnpkg.com/which/-/which-2.0.2.tgz#7c6a8dd0a636a0327e10b59c9286eee93f3f51b1"
   integrity sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==
   dependencies:
     isexe "^2.0.0"
 
 wildcard@^2.0.0:
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.0.tgz#a77d20e5200c6faaac979e4b3aadc7b3dd7f8fec"
-  integrity sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==
-
-word-wrap@^1.2.3:
-  version "1.2.3"
-  resolved "https://registry.yarnpkg.com/word-wrap/-/word-wrap-1.2.3.tgz#610636f6b1f703891bd34771ccb17fb93b47079c"
-  integrity sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==
+  version "2.0.1"
+  resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.1.tgz#5ab10d02487198954836b6349f74fff961e10f67"
+  integrity sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==
 
 worker-loader@^3.0.2:
   version "3.0.8"
   resolved "https://registry.yarnpkg.com/worker-loader/-/worker-loader-3.0.8.tgz#5fc5cda4a3d3163d9c274a4e3a811ce8b60dbb37"
   integrity sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==
   dependencies:
     loader-utils "^2.0.0"
@@ -4772,17 +4801,17 @@
 
 yargs-parser@^20.2.3:
   version "20.2.9"
   resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-20.2.9.tgz#2eb7dc3b0289718fc295f362753845c41a0c94ee"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
 yjs@^13.5.40:
-  version "13.5.53"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.53.tgz#6531378981b89cfadd107145f7fb9f65f708a01f"
-  integrity sha512-B4UUycEK8BcYf195HL4LN4Az4Sg2+QzTHnabFHjQwLvGn96v/G+4CS52xNZk/0QWNXhLRCb+2GK3JmcX5fiCEQ==
+  version "13.6.6"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.6.tgz#586b2dd25121a8cdb55ba85bb8760ec8904e037c"
+  integrity sha512-VTvezMeMuOra9jKG1Ym5XuQ2H4xXOubIIIupv/B5oygasa9IqDE7Ufv93QTSe9uz69J5VZGMQb2WTEmJv4kJFQ==
   dependencies:
-    lib0 "^0.2.72"
+    lib0 "^0.2.74"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

