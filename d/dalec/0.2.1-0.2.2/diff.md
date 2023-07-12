# Comparing `tmp/dalec-0.2.1.tar.gz` & `tmp/dalec-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalec-0.2.1.tar", last modified: Wed Jul  5 11:32:49 2023, max compression
+gzip compressed data, was "dalec-0.2.2.tar", last modified: Wed Jul 12 13:02:45 2023, max compression
```

## Comparing `dalec-0.2.1.tar` & `dalec-0.2.2.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 11:32:40.000000 dalec-0.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 11:32:40.000000 dalec-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 11:32:40.000000 dalec-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 11:32:49.424842 dalec-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-05 11:32:40.000000 dalec-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/dalek/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/static/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/static/dalec/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/static/dalec/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/templates/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/templates/dalec/default/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templates/dalec/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templates/dalec/default/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templatetags/dalec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_example/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec_example/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec_example/templates/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_example/templates/dalec/example/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/templates/dalec/example/french_educ-item.html
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/templates/dalec/example/quarter-item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_prime/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_prime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0002_auto_20211109_1546.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0003_auto_20211109_1615.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 11:32:49.424842 dalec-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 11:32:40.000000 dalec-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/tests/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/adiposian.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/bad_wolf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/empty_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/nice_dalek.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.755679 dalec-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 13:02:36.000000 dalec-0.2.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 13:02:36.000000 dalec-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 13:02:36.000000 dalec-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-12 13:02:45.755679 dalec-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-12 13:02:36.000000 dalec-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/locale/dalek/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/locale/dalek/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/dalek/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/dalek/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/static/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/static/dalec/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/static/dalec/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec/templates/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/templates/dalec/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/templates/dalec/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/templates/dalec/default/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/templatetags/dalec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:02:45.000000 dalec-0.2.2/dalec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_example/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_example/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec_example/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.747679 dalec-0.2.2/dalec_example/templates/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec_example/templates/dalec/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_example/templates/dalec/example/french_educ-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_example/templates/dalec/example/quarter-item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.751679 dalec-0.2.2/dalec_prime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/migrations/0002_auto_20211109_1546.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/migrations/0003_auto_20211109_1615.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 13:02:36.000000 dalec-0.2.2/dalec_prime/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-12 13:02:36.000000 dalec-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-12 13:02:45.755679 dalec-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 13:02:36.000000 dalec-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.755679 dalec-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:45.755679 dalec-0.2.2/tests/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/proxies/adiposian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/proxies/bad_wolf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/proxies/empty_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/proxies/nice_dalek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21461 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 13:02:36.000000 dalec-0.2.2/tests/urls.py
```

### Comparing `dalec-0.2.1/LICENSE` & `dalec-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/PKG-INFO` & `dalec-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalec
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extendable app to retrieve external contents from various external sources.
 Home-page: https://github.com/webu/dalec
 Author: Webu
 Author-email: contact@webu.coop
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/webu/dalec
 Project-URL: Tracker, https://github.com/webu/dalec/issues
```

### Comparing `dalec-0.2.1/README.md` & `dalec-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.mo` & `dalec-0.2.2/dalec/locale/dalek/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.po` & `dalec-0.2.2/dalec/locale/dalek/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.mo` & `dalec-0.2.2/dalec/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.po` & `dalec-0.2.2/dalec/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.mo` & `dalec-0.2.2/dalec/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.po` & `dalec-0.2.2/dalec/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/models.py` & `dalec-0.2.2/dalec/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     Stores fetch queries history for a specific dalec's app [+ channel [+ channel obj]]
     """
 
     last_fetch_dt = models.DateTimeField(
         _("last fetch datetime"), auto_now=True, blank=False, null=False
     )
     app = models.CharField(_("dalec app"), max_length=50, null=False, blank=False)
-    content_type = models.CharField(
-        _("content type"), max_length=50, null=True, blank=True
-    )
+    content_type = models.CharField(_("content type"), max_length=50, null=True, blank=True)
     channel = models.CharField(_("channel"), max_length=50, null=True, blank=True)
     channel_object = models.CharField(
         _("channel app object id"), max_length=255, null=True, blank=True
     )
 
     class Meta:
         verbose_name = _("Content fetch history line")
@@ -57,17 +55,15 @@
         auto_now=False,
         auto_now_add=False,
         blank=False,
         null=False,
         db_index=True,
     )
     app = models.CharField(_("dalec app"), max_length=50, null=False, blank=False)
-    content_type = models.CharField(
-        _("content type"), max_length=50, null=True, blank=True
-    )
+    content_type = models.CharField(_("content type"), max_length=50, null=True, blank=True)
     channel = models.CharField(_("channel"), max_length=50, null=True, blank=True)
     channel_object = models.CharField(
         _("channel app object id"), max_length=255, null=True, blank=True
     )
     dj_channel_content_type = models.ForeignKey(
         ContentType, on_delete=models.CASCADE, blank=True, null=True, related_name="+"
     )
```

### Comparing `dalec-0.2.1/dalec/proxy.py` & `dalec-0.2.2/dalec/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+# Future imports
 from __future__ import annotations
 
+# Standard libs
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Dict, Union, Type, Optional, Tuple
     from typing_extensions import Literal
     from django.db.models import Model
     from django.db.models.query import QuerySet
     from dalec.models import ContentBase, FetchHistoryBase
 
+# Standard libs
 from datetime import timedelta
 from importlib import import_module
 
+# Django imports
 from django.apps import apps
 from django.utils import timezone
 
 try:
+    # Django imports
     from django.utils.decorators import classproperty  # type: ignore
 except ImportError:
     from django.utils.functional import classproperty  # type: ignore
 
+# DALEC imports
 from dalec import settings as app_settings
 
 __all__ = ["ProxyPool", "Proxy"]
 
 
 class ProxyPool:
     """
@@ -48,22 +54,16 @@
         """
         if isinstance(proxy, type):
             proxy = proxy()
         if not isinstance(proxy, Proxy):
             raise ValueError("Your proxy must extends `dalec.proxy.Proxy`")
         if not proxy.app:
             raise ValueError("Your proxy must set it's app name in its `app` attribute")
-        if (
-            proxy.app in cls._proxies
-            and not override
-            and cls._proxies[proxy.app] != proxy
-        ):
-            raise ValueError(
-                'A proxy is already registered for app "{app}"'.format(app=proxy.app)
-            )
+        if proxy.app in cls._proxies and not override and cls._proxies[proxy.app] != proxy:
+            raise ValueError('A proxy is already registered for app "{app}"'.format(app=proxy.app))
         cls._proxies[proxy.app] = proxy
 
     @classmethod
     def get(cls, app: str, autoload: bool = True) -> Proxy:
         """
         Return the proxy registered for the given app.
         If it does not exists, the default behaviour is to try to autoload it
@@ -93,17 +93,15 @@
 
 
 class ProxyMeta(type):
     """
     Meta class to autoregister Proxy class when an app inherit from our Proxy abstact class.
     """
 
-    def __new__(
-        cls: Type[ProxyMeta], name: str, bases: tuple, attrs: dict
-    ) -> ProxyMeta:
+    def __new__(cls: Type[ProxyMeta], name: str, bases: tuple, attrs: dict) -> ProxyMeta:
         """
         Build the new Proxy and auto-register it in the pool
         Auto register
         """
         if not bases:
             return super().__new__(cls, name, bases, attrs)
         proxy_class = super().__new__(cls, name, bases, attrs)
@@ -136,31 +134,27 @@
     def refresh(
         self,
         content_type: str,
         channel: Optional[str] = None,
         channel_object: Optional[str] = None,
         force: Optional[bool] = False,
         dj_channel_obj: Optional[Model] = None,
-    ) -> Union[
-        Tuple[int, int, int], Tuple[Literal[False], Literal[False], Literal[False]]
-    ]:
+    ) -> Union[Tuple[int, int, int], Tuple[Literal[False], Literal[False], Literal[False]]]:
         """
         Fetch updated contents from the source and update/create it into the DB.
         Then, if some contents has been created, delete oldests contents which are not anymore
         required
         returns number of created, updated and deleted objects or False if cache not yet expired
         """
         dalec_kwargs = {
             "content_type": content_type,
             "channel": channel,
             "channel_object": channel_object,
         }
-        last_fetch = (
-            None if force else self.get_last_fetch(**dalec_kwargs)  # type: ignore
-        )
+        last_fetch = None if force else self.get_last_fetch(**dalec_kwargs)  # type: ignore
         if last_fetch:
             too_old = timezone.now() - timedelta(seconds=app_settings.TTL)
             if last_fetch.last_fetch_dt > too_old:
                 # last request is still too recent: we do not spam the external app
                 return False, False, False
         nb = app_settings.get_for("NB_CONTENTS_KEPT", self.app, content_type)
         contents = self._fetch(nb, **dalec_kwargs)  # type: ignore
@@ -184,17 +178,15 @@
                 content=new_content,
                 dj_channel_obj=dj_channel_obj,
                 **dalec_kwargs,  # type: ignore
             )
             if res:
                 nb_created += 1
         # exterminate the oldest ones if some new contents have been created
-        nb_deleted = (
-            0 if not nb_created else self.exterminate(**dalec_kwargs)  # type: ignore
-        )
+        nb_deleted = 0 if not nb_created else self.exterminate(**dalec_kwargs)  # type: ignore
 
         return nb_created, nb_updated, nb_deleted
 
     def create_content(
         self,
         content_type: str,
         channel: str,
```

### Comparing `dalec-0.2.1/dalec/settings.py` & `dalec-0.2.2/dalec/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+# Future imports
 from __future__ import annotations
+
+# Standard libs
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any, Optional
 
+# Standard libs
 import sys
+
+# Django imports
 from django.conf import settings
 
 
 def get_setting(
     setting: str, default: Optional[Any] = None, raise_if_not_set: bool = False
 ) -> Any:
     """
     Return a DALEC_<setting> or it's default Value if not set or raise an Exception
     """
     setting = "DALEC_" + setting
     if not hasattr(settings, setting):
         if raise_if_not_set:
-            raise ValueError(
-                "{setting} is required in your settings.py".format(setting=setting)
-            )
+            raise ValueError("{setting} is required in your settings.py".format(setting=setting))
         return default
     return getattr(settings, setting)
 
 
 def get_for(
     setting: str,
     app: Optional[str] = None,
```

### Comparing `dalec-0.2.1/dalec/static/dalec/js/main.js` & `dalec-0.2.2/dalec/static/dalec/js/main.js`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/templates/dalec/default/list.html` & `dalec-0.2.2/dalec/templates/dalec/default/list.html`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec/templatetags/dalec.py` & `dalec-0.2.2/dalec/templatetags/dalec.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     {% dalec "gitlab" "issue" channel="project" channel_objects='["42", "443"]' %}
 
     Retrieves recent gitlab issues for multiple projects and order them by descending
     issue internal ID (default is `last_update_dt`):
     {% dalec "gitlab" "issue" channel="project" channel_object='42' ordered_by="-iid" %}
     """
     if channel_object and channel_objects:
-        raise ValueError(
-            "You can not use channel_object AND channel_objects at the same time"
-        )
+        raise ValueError("You can not use channel_object AND channel_objects at the same time")
     dalec_view = FetchContentView(_dalec_template=template)
     if channel_objects:
         list_channel_objects = json.loads(channel_objects)
     elif channel_object:
         list_channel_objects = [channel_object]
     else:
         list_channel_objects = None
```

### Comparing `dalec-0.2.1/dalec/tests_utils.py` & `dalec-0.2.2/dalec/tests_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# Standard libs
 from importlib import reload
 
+# Django imports
 from django.apps import apps
 
+# DALEC imports
 from dalec import settings as app_settings
 from dalec.proxy import ProxyPool
 
 
 class DalecTestCaseMixin:
     def tearDown(self) -> None:
         """
```

### Comparing `dalec-0.2.1/dalec/views.py` & `dalec-0.2.2/dalec/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+# Future imports
 from __future__ import annotations
 
-import json
+# Standard libs
 from copy import copy
+import json
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Union, List, Type
     from dalec.models import ContentBase
     from django.http import HttpRequest
     from django.db.models.query import QuerySet
 
+# Standard libs
 import hashlib
 import urllib.parse
 
+# Django imports
 from django.apps import apps
 from django.http import HttpResponse
 from django.template.loader import select_template
 from django.urls import reverse
 
 try:
+    # Django imports
     from django.utils.decorators import classproperty  # type: ignore
 except ImportError:
     from django.utils.functional import classproperty  # type: ignore
 
+# Django imports
 from django.utils.decorators import method_decorator
 from django.utils.functional import cached_property
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic import ListView
 
+# DALEC imports
 from dalec import settings as app_settings
 from dalec.proxy import ProxyPool
 
 __all__ = ["FetchContentView"]
 
 
 @method_decorator(csrf_exempt, name="dispatch")
@@ -76,34 +83,30 @@
             else self.request.GET.get("template", None)
         )
 
     def get_paginate_by(self, queryset: QuerySet) -> int:
         """
         Get the number of items to paginate by, or ``None`` for no pagination.
         """
-        return app_settings.get_for(
-            "NB_CONTENTS_KEPT", self.dalec_app, self.content_type
-        )
+        return app_settings.get_for("NB_CONTENTS_KEPT", self.dalec_app, self.content_type)
 
     def post(self, request: HttpRequest, *args: tuple, **kwargs: dict) -> HttpResponse:
         if request.body:
             data = json.loads(self.request.body)
             self.dalec_channel_objects = data.get("channelObjects", None)
             self.ordered_by = data.get("orderedBy", None)
         return self.get(request, *args, **kwargs)
 
     def get(self, request: HttpRequest, *args: tuple, **kwargs: dict) -> HttpResponse:
         """
         Return a TemplateResponse with HTML for the last X elements wanted
         or a 204 response if nothing need an update (cache used or still the same contents)
         """
         if self.kwargs.get("channel_object", None):
-            self.dalec_channel_objects = [
-                urllib.parse.unquote(self.kwargs["channel_object"])
-            ]
+            self.dalec_channel_objects = [urllib.parse.unquote(self.kwargs["channel_object"])]
         refreshed = self.refresh_contents()
         if not refreshed:
             # nothing to refresh, our content is already the updated one
             # note this is not quite True, because TTL could have expired between the moment
             # we display contents and this request BUT in the same time, another
             # request refreshed the cache and set a new TTL:
             # when we process "our" request, a new TTL is valid, so refresh_content will
@@ -150,34 +153,30 @@
             "app": self.dalec_app,
             "content_type": self.dalec_content_type,
             "type": template_type,
         }
         tpl_names = []
         if self.dalec_channel:
             kwargs["channel"] = self.dalec_channel
-            tpl_names.append(
-                "dalec/{app}/{content_type}-{channel}-{type}.html".format(**kwargs)
-            )
+            tpl_names.append("dalec/{app}/{content_type}-{channel}-{type}.html".format(**kwargs))
         tpl_names += [
             "dalec/{app}/{content_type}-{type}.html".format(**kwargs),
             "dalec/{app}/{type}.html".format(**kwargs),
             "dalec/default/{type}.html".format(**kwargs),
         ]
         css_framework = app_settings.CSS_FRAMEWORK
         if css_framework:
             for i, tpl_name in enumerate(copy(tpl_names)):
                 parts = tpl_name.rsplit("/", 1)
                 parts.insert(1, css_framework)
                 tpl_names.insert(i, "/".join(parts))
         if self.dalec_template:
             tpl_names.insert(
                 0,
-                "dalec/{app}/{tpl}-{type}.html".format(
-                    **{**kwargs, "tpl": self.dalec_template}
-                ),
+                "dalec/{app}/{tpl}-{type}.html".format(**{**kwargs, "tpl": self.dalec_template}),
             )
         return tpl_names
 
     def get_item_template(self) -> str:
         """
         Return the template name to use to display an item in the list, depending the
         custom template, app, content_type, channel and css_framework if used.
@@ -203,17 +202,15 @@
                 "ordered_by": self.ordered_by,
                 "url": reverse("dalec_fetch_content", kwargs=url_kwargs),
                 "ajax_refresh": app_settings.AJAX_REFRESH,
                 "is_fetch": self.request
                 and self.request.headers.get("content-type") == "application/json",
             }
         )
-        temp_id = "{app}-{content_type}-{channel}-{json_channel_objects}".format(
-            **context
-        )
+        temp_id = "{app}-{content_type}-{channel}-{json_channel_objects}".format(**context)
         context["id"] = hashlib.md5(temp_id.encode("utf-8")).hexdigest()
         if self.dalec_template:
             context["url"] += "?template=%s" % self.dalec_template
         return context
 
     def refresh_contents(self) -> bool:
         """
@@ -223,16 +220,12 @@
         proxy = ProxyPool.get(self.dalec_app)
         something_changed = False
         if self.dalec_channel_objects:
             for channel_object in self.dalec_channel_objects:
                 created, updated, deleted = proxy.refresh(
                     self.dalec_content_type, self.dalec_channel, channel_object
                 )
-                something_changed = something_changed or bool(
-                    created or updated or deleted
-                )
+                something_changed = something_changed or bool(created or updated or deleted)
         else:
-            created, updated, deleted = proxy.refresh(
-                self.dalec_content_type, self.dalec_channel
-            )
+            created, updated, deleted = proxy.refresh(self.dalec_content_type, self.dalec_channel)
             something_changed = bool(created or updated or deleted)
         return something_changed
```

### Comparing `dalec-0.2.1/dalec.egg-info/PKG-INFO` & `dalec-0.2.2/dalec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalec
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extendable app to retrieve external contents from various external sources.
 Home-page: https://github.com/webu/dalec
 Author: Webu
 Author-email: contact@webu.coop
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/webu/dalec
 Project-URL: Tracker, https://github.com/webu/dalec/issues
```

### Comparing `dalec-0.2.1/dalec.egg-info/SOURCES.txt` & `dalec-0.2.2/dalec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 dalec/__init__.py
 dalec/apps.py
 dalec/models.py
 dalec/proxy.py
 dalec/settings.py
```

### Comparing `dalec-0.2.1/dalec_example/proxy.py` & `dalec-0.2.2/dalec_example/proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+# Future imports
 from __future__ import annotations
+
+# Standard libs
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional, Dict
 
-from datetime import timedelta, datetime
-
-import requests
+# Standard libs
+from datetime import datetime
+from datetime import timedelta
 
+# Django imports
 from django.utils.dateparse import parse_datetime
 from django.utils.timezone import make_aware
 from django.utils.timezone import now
 
+# DALEC imports
 from dalec.proxy import Proxy
+import requests
 
 __all__ = ["ExampleProxy"]
 
 
 class ExampleProxy(Proxy):
     """
     Just a proxy example wich just fetch the last :
@@ -28,25 +34,21 @@
     app = "example"
 
     def _fetch(
         self, nb: int, content_type: str, channel: str, channel_object: str
     ) -> Dict[str, dict]:
         if content_type == "hour":
             if not channel or channel not in ("quarter", "half"):
-                raise ValueError(
-                    "%s requires a channel ('quarter' or 'half')" % content_type
-                )
+                raise ValueError("%s requires a channel ('quarter' or 'half')" % content_type)
             return self._fetch_hour(nb, channel, channel_object)
         if content_type == "french_educ":
             return self._fetch_french_educ(nb, channel, channel_object)
         raise ValueError("Invalid content_type %s" % content_type)
 
-    def _fetch_hour(
-        self, nb: int, channel: str, channel_object: str
-    ) -> Dict[str, dict]:
+    def _fetch_hour(self, nb: int, channel: str, channel_object: str) -> Dict[str, dict]:
         """
         Return the last N quarters or halfs of an hour from "now" or from a specific datetime
         """
         i = 0
         contents = {}
         if channel_object:
             if "/" in channel_object:
@@ -113,15 +115,11 @@
             record = record["record"]["fields"]
             id = record["identifiant_de_l_etablissement"]
             contents[id] = {
                 # set all fields
                 **record,
                 # and add our own required fields
                 "id": id,
-                "last_update_dt": parse_datetime(
-                    "%s 00:00:00Z" % record["date_maj_ligne"]
-                ),
-                "creation_dt": parse_datetime(
-                    "%s 00:00:00Z" % record["date_ouverture"]
-                ),
+                "last_update_dt": parse_datetime("%s 00:00:00Z" % record["date_maj_ligne"]),
+                "creation_dt": parse_datetime("%s 00:00:00Z" % record["date_ouverture"]),
             }
         return contents
```

### Comparing `dalec-0.2.1/dalec_example/templates/dalec/example/french_educ-item.html` & `dalec-0.2.2/dalec_example/templates/dalec/example/french_educ-item.html`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/dalec_prime/migrations/0001_initial.py` & `dalec-0.2.2/dalec_prime/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Generated by Django 2.2.24 on 2021-10-21 05:39
 
+# Django imports
 import django.core.serializers.json
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 
 try:
+    # Django imports
     from django.db.models import JSONField  # type: ignore
 except ImportError:
     from django_jsonfield_backport.models import JSONField  # type: ignore
+
+# Django imports
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [("contenttypes", "0002_remove_content_type_name")]
```

### Comparing `dalec-0.2.1/dalec_prime/migrations/0002_auto_20211109_1546.py` & `dalec-0.2.2/dalec_prime/migrations/0002_auto_20211109_1546.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Generated by Django 2.2.24 on 2021-11-09 14:46
 
-from django.db import migrations, models
+# Django imports
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
     dependencies = [("dalec_prime", "0001_initial")]
 
     operations = [
         migrations.AlterField(
```

### Comparing `dalec-0.2.1/dalec_prime/migrations/0003_auto_20211109_1615.py` & `dalec-0.2.2/dalec_prime/migrations/0003_auto_20211109_1615.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Generated by Django 2.2.24 on 2021-11-09 15:15
 
-from django.db import migrations, models
+# Django imports
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
     dependencies = [("dalec_prime", "0002_auto_20211109_1546")]
 
     operations = [
         migrations.AlterField(
```

### Comparing `dalec-0.2.1/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py` & `dalec-0.2.2/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Generated by Django 4.2 on 2023-06-21 08:54
 
-from django.db import migrations, models
+# Django imports
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("dalec_prime", "0003_auto_20211109_1615"),
     ]
```

### Comparing `dalec-0.2.1/setup.cfg` & `dalec-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dalec-0.2.1/tests/settings.py` & `dalec-0.2.2/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 ]
 
 if django.VERSION < (3, 2):
     INSTALLED_APPS.append("django_jsonfield_backport")
 
 ROOT_URLCONF = "tests.urls"
 
-TEMPLATES = [
-    {"BACKEND": "django.template.backends.django.DjangoTemplates", "APP_DIRS": True}
-]
+TEMPLATES = [{"BACKEND": "django.template.backends.django.DjangoTemplates", "APP_DIRS": True}]
 
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.sqlite3",
         "NAME": os.path.join(BASE_PATH, "tests.sqlite3"),
     }
 }
```

### Comparing `dalec-0.2.1/tests/tests.py` & `dalec-0.2.2/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,41 +30,31 @@
     def test_overrided_settings_app(self):
         """
         Test if settings overrided for a specific app is returned if set
         """
         reload(app_settings)
         self.assertEqual(app_settings.NB_CONTENTS_KEPT, 10)
         self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "example"), 15)
-        self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "example", "quarter"), 15
-        )
-        self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "example", "french_educ"), 20
-        )
-        self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "example", "content-type"), 30
-        )
+        self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "example", "quarter"), 15)
+        self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "example", "french_educ"), 20)
+        self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "example", "content-type"), 30)
 
     @override_settings(
         INSTALLED_APPS=[app for app in settings.INSTALLED_APPS if app != "dalec_prime"]
     )
     def test_missing_dalec_prime_content_model(self):
-        with self.assertRaisesRegex(
-            ValueError, "You must define a DALEC_CONTENT_MODEL"
-        ):
+        with self.assertRaisesRegex(ValueError, "You must define a DALEC_CONTENT_MODEL"):
             reload(app_settings)
 
     @override_settings(
         INSTALLED_APPS=[app for app in settings.INSTALLED_APPS if app != "dalec_prime"],
         DALEC_CONTENT_MODEL="tests.Content",
     )
     def test_missing_dalec_prime_history_model(self):
-        with self.assertRaisesRegex(
-            ValueError, "You must define a DALEC_FETCH_HISTORY_MODEL"
-        ):
+        with self.assertRaisesRegex(ValueError, "You must define a DALEC_FETCH_HISTORY_MODEL"):
             reload(app_settings)
 
     @override_settings(
         DALEC_CONTENT_MODEL="tests.Content",
         DALEC_FETCH_HISTORY_MODEL="tests.FetchHistory",
     )
     def test_specific_models(self):
@@ -215,17 +205,15 @@
         all_contents = self.content_model.objects.all()
         self.assertEqual(all_contents.count(), 20)
         self.assertEqual(all_contents.filter(channel_object=None).count(), 10)
         self.assertEqual(all_contents.filter(channel_object=channel_object).count(), 10)
 
     def test_ordering_and_latest(self):
         proxy = ProxyPool.get("example")
-        created, updated, deleted = proxy.refresh(
-            "hour", "quarter", "1985-07-02 21:45:00Z"
-        )
+        created, updated, deleted = proxy.refresh("hour", "quarter", "1985-07-02 21:45:00Z")
         first_ordered = self.content_model.objects.first()
         latest_chrono = self.content_model.objects.latest()
         self.assertEqual(first_ordered.pk, latest_chrono.pk)
         self.assertEqual(first_ordered.content_data["id"], "21h45")
 
     def test_proxy_extending_rules(self):
         from .proxies.empty_child import EmptyChildProxy
@@ -404,17 +392,15 @@
             "{% load dalec %}"
             "{% dalec 'example' 'hour' "
             "channel='quarter' channel_objects='[\"2021-12-24\", \"2021-12-25\"]' %}"
         )
         output = Template(html).render(Context({}))
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
-        self.assertEqual(
-            divs[0].attrs["data-channel-objects"], '["2021-12-24", "2021-12-25"]'
-        )
+        self.assertEqual(divs[0].attrs["data-channel-objects"], '["2021-12-24", "2021-12-25"]')
 
     def test_ordered_by_dalec_templatetags(self):
         # Let's query the external apps to fetch contents
         proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh(
             "hour", "half", channel_object="2021-12-24 12:00"
         )
@@ -449,26 +435,22 @@
         with self.assertRaisesRegexp(AttributeError, "MISSING_SETTING"):
             app_settings.get_for("MISSING_SETTING", "example", raise_if_not_set=True)
 
     @override_settings(
         INSTALLED_APPS=[app for app in settings.INSTALLED_APPS if app != "dalec_prime"]
     )
     def test_missing_history_model_and_dalec_prime(self):
-        with self.assertRaisesRegexp(
-            ValueError, "adding dalec_prime to your INSTALLED_APPS"
-        ):
+        with self.assertRaisesRegexp(ValueError, "adding dalec_prime to your INSTALLED_APPS"):
             reload(app_settings)
 
     @override_settings(DALEC_CSS_FRAMEWORK="bootstrap")
     def test_css_framework_template_names(self):
         reload(app_settings)
         dalec_view = FetchContentView(_dalec_template=None)
-        dalec_view.setup(
-            None, app="app", content_type="content_type", channel="channel", page=1
-        )
+        dalec_view.setup(None, app="app", content_type="content_type", channel="channel", page=1)
         template_names = dalec_view.get_template_names()
         expected = [
             "dalec/app/bootstrap/content_type-channel-list.html",
             "dalec/app/bootstrap/content_type-list.html",
             "dalec/app/bootstrap/list.html",
             "dalec/default/bootstrap/list.html",
             "dalec/app/content_type-channel-list.html",
```

