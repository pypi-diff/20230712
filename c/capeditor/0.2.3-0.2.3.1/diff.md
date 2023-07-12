# Comparing `tmp/capeditor-0.2.3.tar.gz` & `tmp/capeditor-0.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.3.tar", last modified: Wed Jul 12 09:24:13 2023, max compression
+gzip compressed data, was "capeditor-0.2.3.1.tar", last modified: Wed Jul 12 10:08:33 2023, max compression
```

## Comparing `capeditor-0.2.3.tar` & `capeditor-0.2.3.1.tar`

### file list

```diff
@@ -1,90 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 09:23:59.000000 capeditor-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 09:24:13.896660 capeditor-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 09:23:59.000000 capeditor-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0002_alter_alertinfo_language.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0002_capsetting_audience_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0003_alter_alert_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0003_alter_capsetting_audience_types_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0004_countryboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0005_delete_countryboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0006_remove_capsetting_contact_capsetting_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/cap_detail_page.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/cap_accordion.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 09:23:59.000000 capeditor-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-12 09:24:13.900660 capeditor-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/css/cap_detail_page.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/cap_accordion.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.501629 capeditor-0.2.3.1/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/icons/cap-alert.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:08:33.505630 capeditor-0.2.3.1/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-12 10:08:33.000000 capeditor-0.2.3.1/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-12 10:08:33.000000 capeditor-0.2.3.1/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:08:33.000000 capeditor-0.2.3.1/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 10:08:33.000000 capeditor-0.2.3.1/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 10:08:33.000000 capeditor-0.2.3.1/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 10:08:19.000000 capeditor-0.2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 10:08:33.509630 capeditor-0.2.3.1/setup.cfg
```

### Comparing `capeditor-0.2.3/PKG-INFO` & `capeditor-0.2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.2.3/README.md` & `capeditor-0.2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/blocks.py` & `capeditor-0.2.3.1/capeditor/blocks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/forms/widgets.py` & `capeditor-0.2.3.1/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.2.3.1/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.2.3.1/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/migrations/0001_initial.py` & `capeditor-0.2.3.1/capeditor/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.2 on 2023-06-26 10:23
+# Generated by Django 4.1.7 on 2023-07-12 09:55
 
 from django.db import migrations, models
 import django.db.models.deletion
 import wagtail.blocks
 import wagtail.fields
 import wagtailiconchooser.blocks
 
@@ -16,18 +16,19 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='CapSetting',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sender', models.CharField(blank=True, max_length=255, null=True, verbose_name='CAP Sender')),
-                ('sender_name', models.CharField(blank=True, max_length=255, null=True, verbose_name='CAP Sender Name')),
-                ('contact', models.CharField(blank=True, max_length=255, null=True, verbose_name='CAP Sender Contact')),
-                ('hazard_types', wagtail.fields.StreamField([('hazard_type', wagtail.blocks.StructBlock([('hazard', wagtail.blocks.CharBlock(help_text='Name of Hazard', label='Hazard', max_length=255)), ('icon', wagtailiconchooser.blocks.IconChooserBlock(required=False))], label='Hazard Type'))], blank=True, null=True, use_json_field=True, verbose_name='Hazard Types')),
+                ('sender', models.CharField(blank=True, help_text='Can be the website link or email of the sending institution', max_length=255, null=True, verbose_name='CAP Sender Identifier')),
+                ('sender_name', models.CharField(blank=True, help_text='Name of the sending institution', max_length=255, null=True, verbose_name='CAP Sender Name')),
+                ('contacts', wagtail.fields.StreamField([('contact', wagtail.blocks.StructBlock([('contact', wagtail.blocks.CharBlock(label='Contact Detail', max_length=255))], label='Contact'))], blank=True, help_text='Contact for follow-up and confirmation of the alert message', null=True, use_json_field=True, verbose_name='Contact Details')),
+                ('hazard_types', wagtail.fields.StreamField([('hazard_type', wagtail.blocks.StructBlock([('hazard', wagtail.blocks.CharBlock(help_text='Name of Hazard', label='Hazard', max_length=255)), ('icon', wagtailiconchooser.blocks.IconChooserBlock(required=False))], label='Hazard Type'))], blank=True, help_text='Hazards monitored by the institution', null=True, use_json_field=True, verbose_name='Hazard Types')),
+                ('audience_types', wagtail.fields.StreamField([('audience_type', wagtail.blocks.StructBlock([('audience', wagtail.blocks.CharBlock(help_text='Intended audience', label='Audience', max_length=255))], label='Audience Type'))], blank=True, help_text='Target audiences for published alerts', null=True, use_json_field=True, verbose_name='Audience Types')),
                 ('site', models.OneToOneField(editable=False, on_delete=django.db.models.deletion.CASCADE, to='wagtailcore.site')),
             ],
             options={
                 'abstract': False,
             },
         ),
     ]
```

### Comparing `capeditor-0.2.3/capeditor/models.py` & `capeditor-0.2.3.1/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/renderers.py` & `capeditor-0.2.3.1/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/serializers.py` & `capeditor-0.2.3.1/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.2.3.1/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.2.3.1/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/conditional_fields.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.2.3.1/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.2.3.1/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.2.3.1/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.2.3.1/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.2.3.1/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.3/capeditor.egg-info/PKG-INFO` & `capeditor-0.2.3.1/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.2.3/capeditor.egg-info/SOURCES.txt` & `capeditor-0.2.3.1/capeditor.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,14 @@
 capeditor/locale/es/LC_MESSAGES/django.mo
 capeditor/locale/es/LC_MESSAGES/django.po
 capeditor/locale/fr/LC_MESSAGES/django.mo
 capeditor/locale/fr/LC_MESSAGES/django.po
 capeditor/locale/sw/LC_MESSAGES/django.mo
 capeditor/locale/sw/LC_MESSAGES/django.po
 capeditor/migrations/0001_initial.py
-capeditor/migrations/0002_alter_alertinfo_language.py
-capeditor/migrations/0002_capsetting_audience_types.py
-capeditor/migrations/0003_alter_alert_sender.py
-capeditor/migrations/0003_alter_capsetting_audience_types_and_more.py
-capeditor/migrations/0004_countryboundary.py
-capeditor/migrations/0005_delete_countryboundary.py
-capeditor/migrations/0006_remove_capsetting_contact_capsetting_contacts.py
 capeditor/migrations/__init__.py
 capeditor/static/capeditor/css/cap_detail_page.css
 capeditor/static/capeditor/css/widget/boundary-widget.css
 capeditor/static/capeditor/css/widget/circle-widget.css
 capeditor/static/capeditor/css/widget/polygon-widget.css
 capeditor/static/capeditor/js/cap_accordion.js
 capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
```

### Comparing `capeditor-0.2.3/setup.cfg` & `capeditor-0.2.3.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.2.3
+version = 0.2.3.1
 description = Wagtail based CAP Editor
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-editor
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
@@ -23,15 +23,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 	djangorestframework-xml
-	python-magic
+	python-magic-bin
 	shapely>=2.0.1
 	wagtail-icon-chooser>=0.0.4
 	adm-boundary-manager>=0.0.3
 	wagtail-humanitarian-icons>=2.0.0
 
 [egg_info]
 tag_build =
```

