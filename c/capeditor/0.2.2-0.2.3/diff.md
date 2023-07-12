# Comparing `tmp/capeditor-0.2.2.tar.gz` & `tmp/capeditor-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.2.tar", last modified: Fri Jul  7 23:30:25 2023, max compression
+gzip compressed data, was "capeditor-0.2.3.tar", last modified: Wed Jul 12 09:24:13 2023, max compression
```

## Comparing `capeditor-0.2.2.tar` & `capeditor-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.128951 capeditor-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 23:30:14.000000 capeditor-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 23:30:25.128951 capeditor-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-07 23:30:14.000000 capeditor-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.120951 capeditor-0.2.2/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0002_alter_alertinfo_language.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0003_alter_alert_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/css/cap_style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/js/hide_attributes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_filter_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_item_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_list_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/latest_alert_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/pagination_include.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/widgets/basemap_polygon.html
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/widgets/polygon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.128951 capeditor-0.2.2/capeditor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templatetags/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.120951 capeditor-0.2.2/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:30:25.128951 capeditor-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-07 23:30:14.000000 capeditor-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 09:23:59.000000 capeditor-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 09:24:13.896660 capeditor-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 09:23:59.000000 capeditor-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0002_alter_alertinfo_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0002_capsetting_audience_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0003_alter_alert_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0003_alter_capsetting_audience_types_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0004_countryboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0005_delete_countryboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/0006_remove_capsetting_contact_capsetting_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/cap_detail_page.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/cap_accordion.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.888660 capeditor-0.2.3/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/icons/cap-alert.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.896660 capeditor-0.2.3/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 09:23:59.000000 capeditor-0.2.3/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:24:13.892660 capeditor-0.2.3/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:24:13.000000 capeditor-0.2.3/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 09:23:59.000000 capeditor-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-12 09:24:13.900660 capeditor-0.2.3/setup.cfg
```

### Comparing `capeditor-0.2.2/PKG-INFO` & `capeditor-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.2
-Summary: Wagtail CAP Editor can be run as standalone or integrated into website
+Version: 0.2.3
+Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
-Author: Grace Amondi
-Author-email: miswa.grace@gmail.com
-License: MIT License
+Author: Grace Amondi, Erick Otenyo
+Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
```

### Comparing `capeditor-0.2.2/README.md` & `capeditor-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.2/capeditor/migrations/0002_alter_alertinfo_language.py` & `capeditor-0.2.3/capeditor/migrations/0002_alter_alertinfo_language.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.2/capeditor/migrations/0003_alter_alert_sender.py` & `capeditor-0.2.3/capeditor/migrations/0003_alter_alert_sender.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.2/capeditor/models.py` & `capeditor-0.2.3/capeditor/blocks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,258 +1,448 @@
-import uuid
-import hashlib
+import json
 
+import shapely
+from django import forms
+from django.contrib.gis.geos import GEOSGeometry
 from django.utils.functional import cached_property
-from django.contrib.gis.db import models
-from django.core.validators import MaxValueValidator, MinValueValidator
-from wagtail.models import Page
-from wagtail.models import Orderable
-from modelcluster.fields import ParentalKey
-from wagtail.fields import RichTextField
-from modelcluster.models import ClusterableModel
-from datetime import datetime
-from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
-# from Inlinepanel.edit_handlers import InlinePanel
-from django.utils.text import slugify
-from capeditor.utils import  paginate, query_param_to_list
-
-from wagtail.admin.panels import MultiFieldPanel, FieldPanel, InlinePanel,FieldRowPanel
-from capeditor.widgets import  BasemapPolygonWidget
-        
-            
-# Create your models here.
-class AlertList(Page):
-    template = "capeditor/alert_index.html"
-    ajax_template = 'capeditor/alert_list_include.html'
-
-    subpage_types = [
-        'capeditor.Alert',  # appname.ModelName
-    ]
-    parent_page_type = [
-        # 'wagtailcore.Page'  # appname.ModelName
-    ]
-    max_count = 1
-
-    alerts_per_page = models.PositiveIntegerField(default=6, validators=[
-        MinValueValidator(6),
-        MaxValueValidator(20),
-    ], help_text=_("How many of this products should be visible on the landing page filter section ?"),
-    verbose_name=_("Alerts Per Page")
-    )
+from shapely import Point
+from shapely.geometry import shape
+from wagtail import blocks
+from wagtail.blocks import FieldBlock, StructValue
+from wagtail.documents.blocks import DocumentChooserBlock
+from wagtail.models import Site
+from wagtailiconchooser.blocks import IconChooserBlock
+
+from .forms.fields import PolygonField, BoundaryPolygonField
+from .forms.widgets import CircleWidget
+from .utils import file_path_mime
+
+
+class BoundaryFieldBlock(FieldBlock):
+    def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
+        self.field_options = {
+            "required": required,
+            "help_text": help_text,
+            "srid": srid
+        }
+
+        super().__init__(**kwargs)
+
+    @cached_property
+    def field(self):
+        return BoundaryPolygonField(**self.field_options)
+
+    def value_from_form(self, value):
+        if isinstance(value, GEOSGeometry):
+            value = value.json
+        return value
+
+
+class PolygonFieldBlock(FieldBlock):
+    def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
+        self.field_options = {
+            "required": required,
+            "help_text": help_text,
+            "srid": srid
+        }
+
+        super().__init__(**kwargs)
+
+    @cached_property
+    def field(self):
+        return PolygonField(**self.field_options)
+
+    def value_from_form(self, value):
+        if isinstance(value, GEOSGeometry):
+            value = value.json
+        return value
+
+
+class CircleFieldBlock(blocks.TextBlock):
+    @cached_property
+    def field(self):
+        field_kwargs = {"widget": CircleWidget()}
+        field_kwargs.update(self.field_options)
+        return forms.CharField(**field_kwargs)
+
 
-    content_panels = Page.content_panels +[
-        FieldPanel('alerts_per_page'),
-    ]
+class AlertAddress(blocks.StructBlock):
+    name = blocks.TextBlock(label=_("Name"), help_text=_("Name of the recipient"))
+    address = blocks.TextBlock(label=_("Address"), help_text=_("Address Information of the recipient"))
 
+
+class AlertReferenceStructValue(StructValue):
     @property
-    def filters(self):
+    def ref_alert_identifier(self):
+        alert_page = self.get("ref_alert").specific
+
+        if hasattr(alert_page, "cap_reference_id"):
+            return alert_page.cap_reference_id
+
+        return None
+
+
+class AlertReference(blocks.StructBlock):
+    class Meta:
+        value_class = AlertReferenceStructValue
+
+    ref_alert = blocks.PageChooserBlock(label=_("Reference Alert"),
+                                        help_text=_("Earlier alert referenced by this alert"))
+
+
+class AlertIncident(blocks.StructBlock):
+    incident = blocks.TextBlock(label=_("Incident"), help_text=_("Referent incident to this alert message"))
+
 
-        URGENCIES = {
-            'Immediate':_('Immediate'),
-            'Expected':_('Expected'),
-            'Future':_('Future'),
-            'Past':_('Past'),
-            'Unknown':_('Unknown'),
+class AlertInfoParameter(blocks.StructBlock):
+    valueName = blocks.TextBlock(label=_("Name"))
+    value = blocks.TextBlock(label=_("Value"))
+
+
+class AlertResponseType(blocks.StructBlock):
+    RESPONSE_TYPE_CHOICES = (
+        ("Shelter", _("Shelter - Take shelter in place or per instruction")),
+        ("Evacuate", _("Evacuate - Relocate as instructed in the instruction")),
+        ("Prepare", _("Prepare - Relocate as instructed in the instruction")),
+        ("Execute", _("Execute - Execute a pre-planned activity identified in instruction")),
+        ("Avoid", _("Avoid - Avoid the subject event as per the instruction")),
+        ("Monitor", _("Monitor - Attend to information sources as described in instruction")),
+        ("Assess", _("Assess - Evaluate the information in this message - DONT USE FOR PUBLIC ALERTS")),
+        ("AllClear", _("All Clear - The subject event no longer poses a threat or concern and any follow "
+                       "on action is described in instruction")),
+        ("None", _("No action recommended")),
+    )
+
+    response_type = blocks.ChoiceBlock(choices=RESPONSE_TYPE_CHOICES, label=_("Response type"),
+                                       help_text=_("The code denoting the type of action recommended for the "
+                                                   "target audience"))
+
+
+class AlertAreaBoundaryStructValue(StructValue):
+    @cached_property
+    def area(self):
+        polygon_geojson_str = self.get("boundary")
+        polygon_geojson_dict = json.loads(polygon_geojson_str)
+
+        polygon = shape(polygon_geojson_dict)
+        coords = " ".join(["{},{}".format(x, y) for x, y in list(polygon.exterior.coords)])
+
+        area_data = {
+            "areaDesc": self.get("areaDesc"),
+            "polygon": coords,
         }
-        
-        SEVERITIES = {
-            'Extreme': _("Extreme - Extraordinary threat to life or property"),
-            'Severe': _("Severe - Significant threat to life or property"),
-            'Moderate': _("Moderate - Possible threat to life or property"),
-            'Minor': _("Minor - Minimal to no known threat to life or property"),
-            'Unknown': _("Unknown - Severity unknown"),
+
+        if self.get("altitude"):
+            area_data.update({"altitude": self.get("altitude")})
+            if self.get("ceiling"):
+                area_data.update({"ceiling": self.get("ceiling")})
+
+        return area_data
+
+    @cached_property
+    def geojson(self):
+        polygon = self.get("boundary")
+        return json.loads(polygon)
+
+
+class AlertAreaBoundaryBlock(blocks.StructBlock):
+    class Meta:
+        value_class = AlertAreaBoundaryStructValue
+
+    ADMIN_LEVEL_CHOICES = (
+        (1, "Level 1"),
+        (2, "Level 2"),
+        (3, "Level 3")
+    )
+
+    areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
+                                help_text=_("The text describing the affected area of the alert message"))
+    admin_level = blocks.ChoiceBlock(choices=ADMIN_LEVEL_CHOICES, default=1, label=_("Administrative Level"))
+    boundary = BoundaryFieldBlock(label=_("Boundary"),
+                                  help_text=_("The paired values of points defining a polygon that delineates "
+                                              "the affected area of the alert message"))
+
+    altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
+                                help_text=_("The specific or minimum altitude of the affected "
+                                            "area of the alert message"))
+    ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
+                               help_text=_("The maximum altitude of the affected area of the alert message."
+                                           "MUST NOT be used except in combination with the altitude element. "))
+
+
+class AlertAreaPolygonStructValue(StructValue):
+    @cached_property
+    def area(self):
+        polygon_geojson_str = self.get("polygon")
+        polygon_geojson_dict = json.loads(polygon_geojson_str)
+
+        polygon = shape(polygon_geojson_dict)
+        coords = " ".join(["{},{}".format(x, y) for x, y in list(polygon.exterior.coords)])
+
+        area_data = {
+            "areaDesc": self.get("areaDesc"),
+            "polygon": coords,
         }
 
-        CERTAINTIES = {
-            'Observed': _("Observed - Determined to have occurred or to be ongoing"),
-            'Likely': _("Likely - Likely (percentage > ~50%)"),
-            'Possible': _("Possible - Possible but not likely (percentage <= ~50%)"),
-            'Unlikely': _("Unlikely - Not expected to occur (percentage ~ 0)"),
-            'Unknown': _("Unknown - Certainty unknown"),
+        if self.get("altitude"):
+            area_data.update({"altitude": self.get("altitude")})
+            if self.get("ceiling"):
+                area_data.update({"ceiling": self.get("ceiling")})
+
+        return area_data
+
+    @cached_property
+    def geojson(self):
+        polygon = self.get("polygon")
+        return json.loads(polygon)
+
+
+class AlertAreaPolygonBlock(blocks.StructBlock):
+    class Meta:
+        value_class = AlertAreaPolygonStructValue
+
+    areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
+                                help_text=_("The text describing the affected area of the alert message"))
+    polygon = PolygonFieldBlock(label=_("Polygon"),
+                                help_text=_("The paired values of points defining a polygon that delineates "
+                                            "the affected area of the alert message"))
+    altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
+                                help_text=_("The specific or minimum altitude of the affected "
+                                            "area of the alert message"))
+    ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
+                               help_text=_("The maximum altitude of the affected area of the alert message."
+                                           "MUST NOT be used except in combination with the altitude element. "))
+
+
+class AlertAreaCircleStructValue(StructValue):
+    @cached_property
+    def area(self):
+        area_data = {
+            "areaDesc": self.get("areaDesc"),
+            "circle": self.get("circle"),
         }
-        return {'urgency': URGENCIES, 'severity':SEVERITIES, 'certainty': CERTAINTIES}
 
-    @property
-    def all_alerts(self):
-        return Alert.objects.live().exclude(status='Draft').filter(scope='Public').order_by('-alert_info__effective')
+        if self.get("altitude"):
+            area_data.update({"altitude": self.get("altitude")})
+            if self.get("ceiling"):
+                area_data.update({"ceiling": self.get("ceiling")})
 
-    def filter_alerts(self, request):
-        alerts = self.all_alerts
+        return area_data
 
-        
-        urgency = query_param_to_list(request.GET.get("urgency"), as_int=False)
-        severity = query_param_to_list(request.GET.get("severity"), as_int=False)
-        certainty = query_param_to_list(request.GET.get("certainty"), as_int=False)
+    @cached_property
+    def geojson(self):
+        circle_str = self.get("circle")
+        parts = circle_str.split()
+        coords = parts[0].split(',')
 
-        filters = models.Q()
+        # Extract the longitude, latitude, and radius
+        longitude, latitude, radius_km = float(coords[0]), float(coords[1]), float(parts[1])
 
-        if urgency:
-            filters &= models.Q(alert_info__urgency__in=urgency)
-        if severity:
-            filters &= models.Q(alert_info__severity__in=severity)
-        if certainty:
-            filters &= models.Q(alert_info__certainty__in=certainty)
+        # Convert radius to degrees (approximation for small distances)
+        radius_deg = radius_km / 111.12
 
-        return alerts.filter(filters)
+        # Create a point for the center
+        center_point = Point(longitude, latitude)
 
-    def filter_and_paginate_alerts(self, request):
-        page = request.GET.get('page')
+        circle = center_point.buffer(radius_deg)
 
-        filtered_alerts = self.filter_alerts(request)
+        return shapely.geometry.mapping(circle)
 
-        paginated_alerts = paginate(filtered_alerts, page, self.alerts_per_page)
 
-        return paginated_alerts
+class AlertAreaCircleBlock(blocks.StructBlock):
+    class Meta:
+        value_class = AlertAreaCircleStructValue
 
+    areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
+                                help_text=_("The text describing the affected area of the alert message"))
+    circle = CircleFieldBlock(label=_("Circle"), help_text=_("Drag the marker to change position"))
 
-    def get_context(self, request, *args, **kwargs):
-        context = super(AlertList,
-                        self).get_context(request, *args, **kwargs)
+    altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
+                                help_text=_("The specific or minimum altitude of the affected "
+                                            "area of the alert message"))
+    ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
+                               help_text=_("The maximum altitude of the affected area of the alert message."
+                                           "MUST NOT be used except in combination with the altitude element. "))
 
-        context['alerts'] = self.filter_and_paginate_alerts(request)
-        context['latest_alert'] = self.all_alerts[0]
 
-        return context
-    
+class AlertAreaGeocodeStructValue(StructValue):
+    @cached_property
+    def area(self):
+        area_data = {
+            "areaDesc": self.get("areaDesc"),
+            "geocode": {"valueName": self.get("valueName"), "value": self.get("value")},
+        }
 
-class Alert(Page):
+        if self.get("altitude"):
+            area_data.update({"altitude": self.get("altitude")})
+            if self.get("ceiling"):
+                area_data.update({"ceiling": self.get("ceiling")})
+
+        return area_data
+
+    @cached_property
+    def geojson(self):
+        return {}
+
+
+class AlertAreaGeocodeBlock(blocks.StructBlock):
+    class Meta:
+        value_class = AlertAreaGeocodeStructValue
+
+    areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
+                                help_text=_("The text describing the affected area of the alert message"))
+    valueName = blocks.TextBlock(label="Name")
+    value = blocks.TextBlock(label=_("Value"))
+
+    altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
+                                help_text=_("The specific or minimum altitude of the affected "
+                                            "area of the alert message"))
+    ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
+                               help_text=_("The maximum altitude of the affected area of the alert message."
+                                           "MUST NOT be used except in combination with the altitude element. "))
 
-    subpage_types = [
-    ]
-    parent_page_type = [
-        'capeditor.AlertList'  # appname.ModelName
-    ]
 
-    template = "capeditor/alert_detail.html"
+SENDER_NAME_HELP_TEXT = _("The human-readable name of the agency or authority issuing this alert.")
+CONTACT_HELP_TEXT = _("The text describing the contact for follow-up and confirmation of the alert message")
+EVENT_HELP_TEXT = _("The text denoting the type of the subject event of the alert message")
+AUDIENCE_HELP_TEXT = _("The text describing the intended audience of the alert message")
 
-    STATUS_CHOICES = (
-        ("Draft", _("Draft - A preliminary template or draft, not actionable in its current form")),
-        ("Actual", _("Actual - Actionable by all targeted recipients")),
-        ("Test", _("Test - Technical testing only, all recipients disregard")),
-        ("Exercise",
-         _("Exercise - Actionable only by designated exercise participants; exercise identifier SHOULD appear in note")),
-        ("system", _("System - For messages that support alert network internal functions")),
-    )
 
-    MESSAGE_TYPE_CHOICES = (
-        ('Alert', _("Alert - Initial information requiring attention by targeted recipients")),
-        ('Update', _("Update - Updates and supercedes the earlier message(s) identified in referenced alerts")),
-        ('Cancel', _("Cancel - Cancels the earlier message(s) identified in references")),
-        ('Ack', _("Acknowledge - Acknowledges receipt and acceptance of the message(s) identified in references field")),
-        ('Error',
-         _("Error -  Indicates rejection of the message(s) identified in references; explanation SHOULD "
-         "appear in note field")),
-    )
+class FileResourceStructValue(StructValue):
+    @property
+    def mime_type(self):
+        doc = self.get('file')
 
-    SCOPE_CHOICES = (
-        ('Public', _("Public - For general dissemination to unrestricted audiences")),
-        ('Restricted',
-         _("Restricted - For dissemination only to users with a known operational requirement as in the restriction field")),
-        ('Private', _("Private - For dissemination only to specified addresses as in the addresses field in the alert")),
-    )
+        try:
+            doc_file = doc.file.path
+            mimetype = file_path_mime(doc_file)
+            return mimetype
+        except Exception:
+            return None
 
-  
-    identifier = models.UUIDField(default=uuid.uuid4, editable=False,
-                                  help_text=_("Unique ID. Auto generated on creation."), verbose_name=_("Identifier"))
-    sender = models.EmailField(max_length=255,
-                              help_text=_(" Identifies the originator of an alert. "
-                                        "This can be an email of the institution for example"), verbose_name=_("Sender"))
-    sent = models.DateTimeField(help_text=_("Time and date of origination of the alert"), default=timezone.now, verbose_name=_("Sent"))
-    status = models.CharField(max_length=50, choices=STATUS_CHOICES,
-                              help_text=_("The code denoting the appropriate handling of the alert"), default='Actual', verbose_name=_("Status"))
-    msgType = models.CharField(max_length=100, choices=MESSAGE_TYPE_CHOICES,
-                                    help_text=_("The code denoting the nature of the alert message"),  default='Alert', verbose_name=_("Message Type"))
-    scope = models.CharField(max_length=100,
-                             choices=SCOPE_CHOICES,
-                             help_text=_("The code denoting the intended distribution of the alert message"),  default='Public', verbose_name=_("Scope"))
-    source = models.TextField(blank=True, null=True, help_text=_("The text identifying the source of the alert message"), verbose_name=_("Source"))
-    restriction = models.TextField(blank=True, null=True,
-                                   help_text=_("The text describing the rule for limiting distribution of the "
-                                             "restricted alert message. Used when scope value is Restricted"), verbose_name=_("Restriction"))
-    code = models.CharField(max_length=100, blank=True, null=True,
-                            help_text=_("The code denoting the special handling of the alert message"), verbose_name=_("Code"))
-    note = models.TextField(blank=True, null=True,
-                            help_text=_("The text describing the purpose or significance of the alert message."
-                                      "The message note is primarily intended for use with "
-                                      "<status> 'Exercise' and <msgType> 'Error'"), verbose_name=_("Note"))
-                                                         
-    content_panels = Page.content_panels + [
-
-        MultiFieldPanel([
-            FieldRowPanel([
-            FieldPanel('sender'),
-            FieldPanel('sent'),
-            ]),
-            FieldPanel('source'),
-            
-            FieldPanel('status',),
-            FieldPanel('msgType', classname="message"),
-            InlinePanel('references', heading=_("Earlier Reference Alerts -  If applicable"), label=_("Alert"), classname="references"),
-
-            FieldPanel('note', classname='note'),
-
-            FieldPanel('scope'),
-            FieldPanel('restriction',classname="restriction" ),
-            InlinePanel('addresses', heading=_("Intended Recipients (If scope is Private) "), label=_("Recipient"), classname="addresses"),
-
-
-        ], heading=_("Alert Identification (Sender, Message Type, Scope)")),
-
-        MultiFieldPanel([
-            InlinePanel('alert_info', label=_("Alert Information"),  classname="collapsed")
-        ], heading=_("Alert Info"))
-    ]
-
-    subpage_types = [
-        # 'capeditor.Alert',  # appname.ModelName
-    ]
-    parent_page_type = [
-        'wagtailcore.Page'  # appname.ModelName
-    ]
-
-class AlertAddress(Orderable):
-    alert = ParentalKey('Alert', related_name="addresses", verbose_name=_("Alert"))
-    name = models.TextField(help_text=_("Name of the recipient"))
-    address = models.EmailField(blank=True, null=True, help_text=_("Email"), verbose_name=_("Email address"))
-
-    def __str__(self):
-        return self.name
-
-
-class AlertReference(Orderable):
-    alert = ParentalKey('Alert', related_name='references', verbose_name=_("Alert"))
-    ref_alert = models.ForeignKey('Alert', blank=True, null=True, on_delete=models.PROTECT,
-                                  help_text=_("Earlier alert referenced by this alert"), verbose_name=_("Reference Alert"))
-
-    def __str__(self):
-        return f'{self.ref_alert.sender},{self.ref_alert.identifier},{self.ref_alert.sent}'
-    
     @property
-    def reference(self):
-        return f'{self.ref_alert.sender},{self.ref_alert.identifier},{self.ref_alert.sent}'
+    def uri(self):
+        doc = self.get('file')
+        return doc.url
 
+    @property
+    def resource(self):
+        return {
+            "type": "doc",
+            "resourceDesc": self.get("resourceDesc"),
+            "mimeType": self.mime_type,
+            "uri": self.uri
+        }
+
+
+class ExternalResourceStructValue(StructValue):
+    @property
+    def resource(self):
+        return {
+            "type": "external",
+            "resourceDesc": self.get("resourceDesc"),
+            "mimeType": "text/uri-list",
+            "uri": self.get('external_url')
+        }
 
 
-class AlertIncident(Orderable):
-    alert = ParentalKey('Alert', related_name='incidents', on_delete=models.CASCADE, verbose_name=_("Alert"))
-    title = models.CharField(max_length=255, help_text=_("Title of the incident referent of the alert"), verbose_name=_("Title"))
-    description = models.TextField(help_text=_("Description of the incident"), verbose_name=_("Description"))
+class FileResource(blocks.StructBlock):
+    resourceDesc = blocks.TextBlock(label=_("Resource Description"),
+                                    help_text=_("The text describing the type and content of the resource file"))
+    file = DocumentChooserBlock()
+
+    class Meta:
+        value_class = FileResourceStructValue
+
+
+class ExternalResource(blocks.StructBlock):
+    resourceDesc = blocks.TextBlock(label=_("Resource Description"),
+                                    help_text=_("The text describing the type and content of the resource file"))
+    external_url = blocks.URLBlock(verbose_name=_("External Resource Link"),
+                                   help_text=_("Link to external resource. "
+                                               "This can be for example a link to related websites. "))
+
+    class Meta:
+        value_class = ExternalResourceStructValue
+
+
+class AlertEventCode(blocks.StructBlock):
+    valueName = blocks.TextBlock(label=_("Name"), help_text=_("Name for the event code"))
+    value = blocks.TextBlock(label=_("Value"), help_text=_("Value of the event code"), )
+
+
+class AlertInfoStructValue(StructValue):
+    @cached_property
+    def event_icon(self):
+        from .models import CapSetting
+        event = self.get("event")
+        try:
+            site = Site.objects.get(is_default_site=True)
+            if site:
+                cap_setting = CapSetting.for_site(site)
+
+                if cap_setting.hazard_types:
+                    for hazard in cap_setting.hazard_types:
+                        event_name = hazard.value.get("hazard")
+                        if event_name == event:
+                            return hazard.value.get("icon")
+        except Exception:
+            pass
 
-    def __str__(self):
-        return self.title
+        return None
+
+    @cached_property
+    def resource(self):
+        resource = self.get("resource")
+        resources = []
+        if resource:
+            for res in resource:
+                resources.append(res.value.resource)
+            return resources
+        return None
 
-class AlertInfo(ClusterableModel):
+    @cached_property
+    def area(self):
+        area_blocks = self.get("area")
+        areas = []
+
+        if area_blocks:
+            for area in area_blocks:
+                areas.append(area.value.area)
+            return areas
+
+    @cached_property
+    def geojson(self):
+        area_blocks = self.get("area")
+        features = []
+        if area_blocks:
+            for area in area_blocks:
+                features.append(area.value.geojson)
+            return features
+
+    @cached_property
+    def features(self):
+        area_blocks = self.get("area")
+        features = []
+
+        if area_blocks:
+            for feature in area_blocks:
+                if feature.value.geojson:
+                    features.append({"type": "Feature", "geometry": feature.value.geojson})
+
+        return features
+
+
+class AlertInfo(blocks.StructBlock):
+    class Meta:
+        value_class = AlertInfoStructValue
 
     LANGUAGE_CHOICES = (
         ('en', _("English")),
-        ('fr', _("French")),
-        ('ar', _("Arabic")),
-        ('am', _("Amharic")),
-        ('sw', _("Swahili")),
     )
 
     CATEGORY_CHOICES = (
         ('Geo', _("Geophysical")),
         ('Met', _("Meteorological")),
         ('Safety', _("General emergency and public safety")),
         ('Security', _("Law enforcement, military, homeland and local/private security")),
@@ -286,216 +476,79 @@
         ('Observed', _("Observed - Determined to have occurred or to be ongoing")),
         ('Likely', _("Likely - Likely (percentage > ~50%)")),
         ('Possible', _("Possible - Possible but not likely (percentage <= ~50%)")),
         ('Unlikely', _("Unlikely - Not expected to occur (percentage ~ 0)")),
         ('Unknown', _("Unknown - Certainty unknown")),
     )
 
-    alert = ParentalKey('Alert', related_name="alert_info", )
-
-    language = models.CharField(max_length=100, choices=LANGUAGE_CHOICES, default='en', blank=True, null=True,
-                                help_text=_("The code denoting the language of the alert message"), verbose_name=_("Language"))
-    category = models.CharField(max_length=100,  default='Met',
-                                choices=CATEGORY_CHOICES,
-                                help_text=_("The code denoting the category of the subject event of the alert message"), verbose_name=_("Category"))
-    event = models.CharField(max_length=100,
-                             help_text=_("The text denoting the type of the subject event of the alert message"), blank=True, null=True, verbose_name=_("Event"))
-    urgency = models.CharField(max_length=100,
-                               choices=URGENCY_CHOICES,
-                               verbose_name=_("Urgency"),
-                               help_text=_("The code denoting the urgency of the subject event of the alert message"), default="Immediate")
-    severity = models.CharField(max_length=100,
-                                choices=SEVERITY_CHOICES,
-                                verbose_name=_("Severity"),
-                                help_text=_("The code denoting the severity of the subject event of the alert message"), default="Extreme")
-    certainty = models.CharField(max_length=100,
-                                 choices=CERTAINTY_CHOICES,
-                                 verbose_name=_("Certainty"),
-                                 help_text=_("The code denoting the certainty of the subject event of the alert message"), default="Likely")
-    audience = models.TextField(blank=True, null=True,
-                                verbose_name=_("Audience"),
-                                help_text=_("The text describing the intended audience of the alert message"))
-
-    effective = models.DateTimeField(blank=True, null=True,
-                                     verbose_name=_("Effective"),
-                                     help_text=_("The effective time of the information of the alert message"))
-    onset = models.DateTimeField(blank=True, null=True,
-                                 verbose_name=_("Onset"),
-                                 help_text=_("The expected time of the beginning of the subject event "
-                                           "of the alert message"))
-    expires = models.DateTimeField(blank=True, null=True,
-                                   verbose_name=_("Expires"),
-                                   help_text=_("The expiry time of the information of the alert message"))
-    headline = models.TextField(blank=True, null=True,verbose_name=_("Headline"), help_text=_("The text headline of the alert message"))
-    description = models.TextField(blank=True, null=True,verbose_name=_("Description"),
-                                   help_text=_("The text describing the subject event of the alert message"))
-    instruction = models.TextField(blank=True, null=True,verbose_name=_("Instruction"),
+    language = blocks.ChoiceBlock(choices=LANGUAGE_CHOICES, default="en", required=False, label=_("Language"),
+                                  help_text=_("The code denoting the language of the alert message"), )
+    category = blocks.ChoiceBlock(choices=CATEGORY_CHOICES, default="Met", label=_("Category"),
+                                  help_text=_("The code denoting the category of the subject"
+                                              " event of the alert message"))
+    event = blocks.CharBlock(max_length=255, label=_("Event"), help_text=EVENT_HELP_TEXT)
+    urgency = blocks.ChoiceBlock(choices=URGENCY_CHOICES, label=_("Urgency"),
+                                 help_text=_("The code denoting the urgency of the subject "
+                                             "event of the alert message"))
+    severity = blocks.ChoiceBlock(choices=SEVERITY_CHOICES, label=_("Severity"),
+                                  help_text=_("The code denoting the severity of the subject "
+                                              "event of the alert message"))
+    certainty = blocks.ChoiceBlock(choices=CERTAINTY_CHOICES, label=_("Certainty"),
+                                   help_text=_("The code denoting the certainty of the subject "
+                                               "event of the alert message"))
+    headline = blocks.CharBlock(max_length=160, required=False, label=_("Headline"),
+                                help_text=_("The text headline of the alert message. "
+                                            "Make it direct and actionable as possible while remaining short"))
+    description = blocks.TextBlock(required=True, label=_("Description"),
+                                   help_text=_(
+                                       "The text describing the subject event of the alert message. "
+                                       "An extended description of the hazard or event that occasioned this message"))
+    instruction = blocks.TextBlock(required=False, label=_("Instruction"),
                                    help_text=_("The text describing the recommended action to be taken by "
-                                             "recipients of the alert message"))
-    web = models.URLField(blank=True, null=True,verbose_name=_("Web"),
-                          help_text=_("The identifier of the hyperlink associating "
-                                    "additional information with the alert message"))
-    contact = models.TextField(blank=True, null=True,verbose_name=_("Contact"),
-                               help_text=_("The text describing the contact for follow-up and "
-                                         "confirmation of the alert message"))
-
-    
-    panels = [
-
-        MultiFieldPanel([
-            FieldRowPanel([
-            FieldPanel('language'),
-            FieldPanel('event'),
-
-            ]),
-            FieldPanel('category'),
-            FieldPanel('urgency'),
-            FieldPanel('severity'),
-            FieldPanel('certainty'),
-            InlinePanel('response_types', heading="Response Types ", label="Response Type"),        
-            FieldPanel('audience'),
-            # FieldPanel('event_codes'),
-            FieldRowPanel([
-                FieldPanel('effective'),
-                FieldPanel('onset'),
-            ]),
-            FieldPanel('expires'),
-
-            
-        ], heading=_("Alert Categorization (Category, Urgency, Severity, Certainity, Response & Dates)"), classname="collapsed"),
-
-        MultiFieldPanel([
-            FieldPanel('headline'),
-            FieldPanel('description'),
-            FieldPanel('instruction'),
-
-            FieldRowPanel([
-                FieldPanel('web'),
-                FieldPanel('contact'),
-            ])
-        ], heading =_("Alert Delivery Message (Headline, Description, Intsructions, Contact & Website)"), classname="collapsed"),
-
-
-        MultiFieldPanel([
-        InlinePanel('resources', heading=_("Alert Resources "), label=_("Resource")),
-        ],  classname="collapsed"),
-
-        MultiFieldPanel([
-            InlinePanel('alert_areas',  heading=_("Alert Areas "),label=_("Alert Area")),
-        ], classname="collapsed"),
-
-        
-    ]
-
-    @property
-    def is_expired(self):
-        difference = (timezone.now() - self.expires).days
-        if difference >= 0:
-            return True
-        return False
-
+                                               "recipients of the alert message"))
+    effective = blocks.DateTimeBlock(required=False, label=_("Effective"),
+                                     help_text=_("The effective time of the information of the alert message. "
+                                                 "If not set, the sent date will be used"))
+    onset = blocks.DateTimeBlock(required=False, label=_("Onset"),
+                                 help_text=_("The expected time of the beginning of the subject event "
+                                             "of the alert message"))
+    expires = blocks.DateTimeBlock(required=True, label=_("Expires"),
+                                   help_text=_("The expiry time of the information of the alert message. "
+                                               "If not set, each recipient is free to set its own policy as to when the"
+                                               " message is no longer in effect."))
+    responseType = blocks.ListBlock(AlertResponseType(label="Response Type"), label=_("Response Types"), default=[])
+
+    senderName = blocks.CharBlock(max_length=255, label=_("Sender name"), required=False,
+                                  help_text=SENDER_NAME_HELP_TEXT)
+    contact = blocks.CharBlock(max_length=255, required=False, label=_("Contact"), help_text=CONTACT_HELP_TEXT)
+    audience = blocks.CharBlock(max_length=255, required=False, label=_("Audience"),
+                                help_text=AUDIENCE_HELP_TEXT)
+    area = blocks.StreamBlock([
+        ("boundary_block", AlertAreaBoundaryBlock(label=_("Admin Boundary"))),
+        ("polygon_block", AlertAreaPolygonBlock(label=_("Draw Polygon"))),
+        ("circle_block", AlertAreaCircleBlock(label=_("Circle"))),
+        ("geocode_block", AlertAreaGeocodeBlock(label=_("Geocode"))),
+    ], label=_("Alert Area"), help_text=_("Admin Boundary, Polygon, Circle or Geocode"))
+
+    resource = blocks.StreamBlock([
+        ("file_resource", FileResource()),
+        ("external_resource", ExternalResource()),
+    ], required=False, label=_("Resources"), help_text=_("Additional file with supplemental information "
+                                                         "related to this alert information"))
+
+    parameter = blocks.ListBlock(AlertInfoParameter(label=_("Parameter")), label=_("Parameters"), default=[])
+    eventCode = blocks.ListBlock(AlertEventCode(label=_("Event Code")), label=_("Event codes"), default=[])
+
+    # NOTE: web attribute is obtained from the url of the page
+
+
+class HazardTypeBlock(blocks.StructBlock):
+    hazard = blocks.CharBlock(max_length=255, label=_("Hazard"), help_text="Name of Hazard")
+    icon = IconChooserBlock(required=False)
 
-class AlertResponseType(Orderable):
-    RESPONSE_TYPE_CHOICES = (
-        ("Shelter", _("Shelter - Take shelter in place or per instruction")),
-        ("Evacuate", _("Evacuate - Relocate as instructed in the instruction")),
-        ("Prepare", _("Prepare - Relocate as instructed in the instruction")),
-        ("Execute", _("Execute - Execute a pre-planned activity identified in instruction")),
-        ("Avoid", _("Avoid - Avoid the subject event as per the instruction")),
-        ("Monitor", _("Monitor - Attend to information sources as described in instruction")),
-        ("Assess", _("Assess - Evaluate the information in this message - DONT USE FOR PUBLIC ALERTS")),
-        ("AllClear",
-         _("All Clear - The subject event no longer poses a threat or concern and any follow on action is described in instruction")),
-        ("None", _("No action recommended")),
-    )
 
-    alert = ParentalKey('AlertInfo', related_name='response_types', null=True)
-    response_type = models.CharField(max_length=100, choices=RESPONSE_TYPE_CHOICES,verbose_name=_("Response type"),
-                                     help_text=_("The code denoting the type of action recommended for the "
-                                               "target audience"))
-
-    def __str__(self) -> str:
-        return self.response_type
-
-
-class AlertResource(Orderable):
-    alert_info = ParentalKey('AlertInfo', related_name='resources', null=True)
-    mimeType = models.CharField(max_length=100, blank=True, null=True,
-                                     help_text=_("Resource type whether is image, file etc"))
-    resourceDesc = models.TextField(help_text=_("The text describing the type and content of the resource file"))
-    file = models.ForeignKey(
-        'wagtaildocs.Document',
-        help_text=_("File, Document etc"),
-        verbose_name=_("File"),
-        null=True,
-        blank=True,
-        on_delete=models.SET_NULL,
-        related_name='+',
-    )
-    uri = models.URLField(blank=True, null=True, help_text=_("The identifier of the hyperlink for the resource file"), verbose_name=_('Link'))
-    derefUri = models.TextField(blank=True, null=True,
-                                help_text=_("The base-64 encoded data content of the resource file"))
-    digest = models.TextField(blank=True, null=True,
-                              help_text=_("The code representing the digital digest ('hash') computed "
-                                        "from the resource file"))
-    
-    size = models.IntegerField(null=True, blank=True)
-
-    panels = [
-        FieldPanel('resourceDesc'),
-        FieldPanel('file'),
-    ]
+class AudienceTypeBlock(blocks.StructBlock):
+    audience = blocks.CharBlock(max_length=255, label=_("Audience"), help_text="Intended audience")
 
-    @property
-    def mime_type(self):
-        return None
 
-    
-    def save(self ,*args, **kwargs):
-        self.size = self.file.file.size
-        self.mimeType = self.file.content_type
-        self.uri = self.file.url
-        with open(self.file.file.path, 'rb') as file:
-            document_content = file.read()
-        self.digest = hashlib.sha256(document_content).hexdigest()
-
-        return super(AlertResource, self).save(*args, **kwargs)
-
-
-class AlertArea(ClusterableModel):
-    alert_info = ParentalKey('AlertInfo', related_name='alert_areas', null=True)
-    areaDesc = models.CharField(max_length=100, help_text=_("The text describing the affected area of the alert message"),
-                                 verbose_name=_("Affected areas / Regions"),null=True)
-   
-    area = models.PolygonField(help_text=_("The paired values of points defining a polygon that delineates the affected "
-                                         "area of the alert message"), verbose_name=_("Area"), null=True, srid=4326)
-
-    altitude = models.CharField(max_length=100,
-                                blank=True,
-                                null=True,
-                                help_text=_("The specific or minimum altitude of the affected area of the alert message"),
-                                verbose_name=_("Altitude"))
-    ceiling = models.CharField(max_length=100,
-                               blank=True,
-                               null=True,
-                               verbose_name=_("Ceiling"),
-                               help_text=_("The maximum altitude of the affected area of the alert message."
-                                         "MUST NOT be used except in combination with the altitude element. "))
-                          
-    panels = [
-        FieldPanel('areaDesc'),
-        FieldPanel('area', widget=BasemapPolygonWidget() ),
-        InlinePanel('geocodes', label="Geocode", heading="Geocodes "),
-        FieldPanel('altitude'),
-        FieldPanel('ceiling'),
-    ]   
-
-class AlertEventCode(Orderable):
-    alert_info = ParentalKey('AlertInfo', related_name='event_codes', null=True)
-    name = models.CharField(max_length=100, help_text=_("Name for the event code"), verbose_name=_("Name"))
-    value = models.CharField(max_length=255, help_text=_("Value of the event code"), verbose_name=_("Value"))
-
-
-class AlertGeocode(Orderable):
-    alert_info = ParentalKey('AlertArea', related_name='geocodes', null=True)
-    name = models.CharField(max_length=100, help_text=_("Name for the geocode"), verbose_name=_("Name"))
-    value = models.CharField(max_length=255, help_text=_("Value of the geocode"), verbose_name=_("Value"))
+class ContactBlock(blocks.StructBlock):
+    contact = blocks.CharBlock(max_length=255, label=_("Contact Detail"))
```

### Comparing `capeditor-0.2.2/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.2.3/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.2/capeditor.egg-info/PKG-INFO` & `capeditor-0.2.3/capeditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.2
-Summary: Wagtail CAP Editor can be run as standalone or integrated into website
+Version: 0.2.3
+Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
-Author: Grace Amondi
-Author-email: miswa.grace@gmail.com
-License: MIT License
+Author: Grace Amondi, Erick Otenyo
+Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
```

