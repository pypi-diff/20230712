# Comparing `tmp/django-filer-3.0.0rc3.tar.gz` & `tmp/django-filer-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-3.0.0rc3.tar", last modified: Thu Jun 29 06:33:29 2023, max compression
+gzip compressed data, was "django-filer-3.0.1.tar", last modified: Wed Jul 12 19:11:53 2023, max compression
```

## Comparing `django-filer-3.0.0rc3.tar` & `django-filer-3.0.1.tar`

### file list

```diff
@@ -1,375 +1,378 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.683263 django-filer-3.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-29 06:33:29.683263 django-filer-3.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.599256 django-filer-3.0.0rc3/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 06:33:29.000000 django-filer-3.0.0rc3/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.599256 django-filer-3.0.0rc3/filer/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.603256 django-filer-3.0.0rc3/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.603256 django-filer-3.0.0rc3/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.603256 django-filer-3.0.0rc3/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.607257 django-filer-3.0.0rc3/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.607257 django-filer-3.0.0rc3/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.607257 django-filer-3.0.0rc3/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.571253 django-filer-3.0.0rc3/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.607257 django-filer-3.0.0rc3/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30202 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.571253 django-filer-3.0.0rc3/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.607257 django-filer-3.0.0rc3/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29699 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.571253 django-filer-3.0.0rc3/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36612 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.571253 django-filer-3.0.0rc3/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.571253 django-filer-3.0.0rc3/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37740 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.611257 django-filer-3.0.0rc3/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31609 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34181 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29585 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36506 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18114 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38077 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.575254 django-filer-3.0.0rc3/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.615257 django-filer-3.0.0rc3/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.619258 django-filer-3.0.0rc3/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.619258 django-filer-3.0.0rc3/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36760 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.619258 django-filer-3.0.0rc3/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37243 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.619258 django-filer-3.0.0rc3/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29586 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.619258 django-filer-3.0.0rc3/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29600 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37319 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.579254 django-filer-3.0.0rc3/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29889 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37299 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34818 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.623258 django-filer-3.0.0rc3/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37357 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.627258 django-filer-3.0.0rc3/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.627258 django-filer-3.0.0rc3/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37525 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.627258 django-filer-3.0.0rc3/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    41320 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.627258 django-filer-3.0.0rc3/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29828 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.583254 django-filer-3.0.0rc3/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.627258 django-filer-3.0.0rc3/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29585 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35015 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29599 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29600 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.631259 django-filer-3.0.0rc3/filer/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.635259 django-filer-3.0.0rc3/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.639259 django-filer-3.0.0rc3/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/0017_image__transparent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.643260 django-filer-3.0.0rc3/filer/models/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.643260 django-filer-3.0.0rc3/filer/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.647260 django-filer-3.0.0rc3/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.587255 django-filer-3.0.0rc3/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.591255 django-filer-3.0.0rc3/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.647260 django-filer-3.0.0rc3/filer/static/filer/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.cms.icons.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    91190 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.fa.icons.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.647260 django-filer-3.0.0rc3/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (123)    87123 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/css/maps/admin_filer.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.647260 django-filer-3.0.0rc3/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.655261 django-filer-3.0.0rc3/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/move-to-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/remove-selection.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/th-large.svg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/th-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/fonts/src/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.659261 django-filer-3.0.0rc3/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.663262 django-filer-3.0.0rc3/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.663262 django-filer-3.0.0rc3/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.667262 django-filer-3.0.0rc3/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/filer_popup_response.js
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.667262 django-filer-3.0.0rc3/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.591255 django-filer-3.0.0rc3/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.591255 django-filer-3.0.0rc3/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.671262 django-filer-3.0.0rc3/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.671262 django-filer-3.0.0rc3/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/file/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/file/popup_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.675263 django-filer-3.0.0rc3/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.679263 django-filer-3.0.0rc3/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:29.683263 django-filer-3.0.0rc3/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 06:33:29.683263 django-filer-3.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-29 06:33:18.000000 django-filer-3.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.461593 django-filer-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-12 19:11:40.000000 django-filer-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 19:11:40.000000 django-filer-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-12 19:11:53.461593 django-filer-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-12 19:11:40.000000 django-filer-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.413591 django-filer-3.0.1/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 19:11:53.000000 django-filer-3.0.1/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.417592 django-filer-3.0.1/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36871 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37978 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31970 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36774 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.421592 django-filer-3.0.1/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39279 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.405591 django-filer-3.0.1/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37572 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30912 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.425592 django-filer-3.0.1/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35169 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30709 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37766 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30834 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38041 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.429592 django-filer-3.0.1/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.433592 django-filer-3.0.1/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.409591 django-filer-3.0.1/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.433592 django-filer-3.0.1/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.433592 django-filer-3.0.1/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.433592 django-filer-3.0.1/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.437592 django-filer-3.0.1/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.437592 django-filer-3.0.1/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.437592 django-filer-3.0.1/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.437592 django-filer-3.0.1/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.413591 django-filer-3.0.1/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.413591 django-filer-3.0.1/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.441592 django-filer-3.0.1/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91190 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.441592 django-filer-3.0.1/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    87123 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/maps/admin_filer.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/css/maps/admin_filer.icons.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.445592 django-filer-3.0.1/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.445592 django-filer-3.0.1/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.449592 django-filer-3.0.1/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.449592 django-filer-3.0.1/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.449592 django-filer-3.0.1/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.453593 django-filer-3.0.1/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.453593 django-filer-3.0.1/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.413591 django-filer-3.0.1/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.413591 django-filer-3.0.1/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.453593 django-filer-3.0.1/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.453593 django-filer-3.0.1/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.457593 django-filer-3.0.1/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:53.461593 django-filer-3.0.1/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 19:11:40.000000 django-filer-3.0.1/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-12 19:11:53.461593 django-filer-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-12 19:11:40.000000 django-filer-3.0.1/setup.py
```

### Comparing `django-filer-3.0.0rc3/LICENSE` & `django-filer-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/PKG-INFO` & `django-filer-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.0rc3
+Version: 3.0.1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -35,14 +35,15 @@
 Classifier: Framework :: Django CMS :: 4.0
 Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
+Provides-Extra: heif
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
 |pypi| |python| |django| |coverage|
```

### Comparing `django-filer-3.0.0rc3/README.rst` & `django-filer-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/django_filer.egg-info/PKG-INFO` & `django-filer-3.0.1/django_filer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.0rc3
+Version: 3.0.1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -35,14 +35,15 @@
 Classifier: Framework :: Django CMS :: 4.0
 Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
+Provides-Extra: heif
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
 |pypi| |python| |django| |coverage|
```

### Comparing `django-filer-3.0.0rc3/django_filer.egg-info/SOURCES.txt` & `django-filer-3.0.1/django_filer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -152,15 +152,18 @@
 filer/server/backends/default.py
 filer/server/backends/nginx.py
 filer/server/backends/xsendfile.py
 filer/static/filer/css/admin_filer.cms.icons.css
 filer/static/filer/css/admin_filer.css
 filer/static/filer/css/admin_filer.fa.icons.css
 filer/static/filer/css/admin_folderpermissions.css
+filer/static/filer/css/maps/admin_filer.cms.icons.css.map
 filer/static/filer/css/maps/admin_filer.css.map
+filer/static/filer/css/maps/admin_filer.fa.icons.css.map
+filer/static/filer/css/maps/admin_filer.icons.css.map
 filer/static/filer/fonts/FontAwesome.otf
 filer/static/filer/fonts/django-filer-iconfont.eot
 filer/static/filer/fonts/django-filer-iconfont.svg
 filer/static/filer/fonts/django-filer-iconfont.ttf
 filer/static/filer/fonts/django-filer-iconfont.woff
 filer/static/filer/fonts/django-filer-iconfont.woff2
 filer/static/filer/fonts/fontawesome-webfont.eot
```

### Comparing `django-filer-3.0.0rc3/filer/__init__.py` & `django-filer-3.0.1/filer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '3.0.0rc3'
+__version__ = '3.0.1'
 
 default_app_config = 'filer.apps.FilerConfig'
```

### Comparing `django-filer-3.0.0rc3/filer/admin/__init__.py` & `django-filer-3.0.1/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/clipboardadmin.py` & `django-filer-3.0.1/filer/admin/clipboardadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/fileadmin.py` & `django-filer-3.0.1/filer/admin/fileadmin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from django import forms
 from django.contrib.admin.utils import unquote
+from django.contrib.staticfiles.storage import staticfiles_storage
 from django.http import Http404, HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 
+from easy_thumbnails.exceptions import InvalidImageFormatError
 from easy_thumbnails.files import get_thumbnailer
 from easy_thumbnails.options import ThumbnailOptions
 
 from .. import settings
 from ..models import BaseImage, File
 from ..settings import DEFERRED_THUMBNAIL_SIZES
 from .permissions import PrimitivePermissionAwareModelAdmin
@@ -170,14 +172,17 @@
         if size not in DEFERRED_THUMBNAIL_SIZES:
             # Only allow icon sizes relevant for the admin
             raise Http404
         file = get_object_or_404(File, pk=file_id)
         if not isinstance(file, BaseImage):
             raise Http404()
 
-        thumbnailer = get_thumbnailer(file)
-        thumbnail_options = ThumbnailOptions({'size': (size, size), "crop": True})
-        thumbnail = thumbnailer.get_thumbnail(thumbnail_options, generate=True)
-        return HttpResponseRedirect(thumbnail.url)
+        try:
+            thumbnailer = get_thumbnailer(file)
+            thumbnail_options = ThumbnailOptions({'size': (size, size), "crop": True})
+            thumbnail = thumbnailer.get_thumbnail(thumbnail_options, generate=True)
+            return HttpResponseRedirect(thumbnail.url)
+        except InvalidImageFormatError:
+            return HttpResponseRedirect(staticfiles_storage.url('filer/icons/file-missing.svg'))
 
 
 FileAdmin.fieldsets = FileAdmin.build_fieldsets()
```

### Comparing `django-filer-3.0.0rc3/filer/admin/folderadmin.py` & `django-filer-3.0.1/filer/admin/folderadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/forms.py` & `django-filer-3.0.1/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/imageadmin.py` & `django-filer-3.0.1/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/patched/admin_utils.py` & `django-filer-3.0.1/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/permissionadmin.py` & `django-filer-3.0.1/filer/admin/permissionadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/permissions.py` & `django-filer-3.0.1/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/tools.py` & `django-filer-3.0.1/filer/admin/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/admin/views.py` & `django-filer-3.0.1/filer/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/apps.py` & `django-filer-3.0.1/filer/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,39 @@
+import mimetypes
+
 from django.apps import AppConfig
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.translation import gettext_lazy as _
 
 
 class FilerConfig(AppConfig):
     default_auto_field = 'django.db.models.AutoField'
     name = 'filer'
     verbose_name = _("Filer")
 
-    def ready(self):
+    def register_optional_heif_supprt(self):
+        try:  # pragma:  no cover
+            from pillow_heif import register_heif_opener
+
+            from .settings import IMAGE_EXTENSIONS, IMAGE_MIME_TYPES
+
+            # Register with easy_thumbnails
+            register_heif_opener()
+            HEIF_EXTENSIONS = [".heic", ".heics", ".heif", ".heifs", ".hif"]
+            # Add extensions to python mimetypes which filer uses
+            for ext in HEIF_EXTENSIONS:
+                mimetypes.add_type("image/heic", ext)
+            # Mark them as images
+            IMAGE_EXTENSIONS += HEIF_EXTENSIONS
+            IMAGE_MIME_TYPES.append("heic")
+        except (ModuleNotFoundError, ImportError):
+            # No heif support installed
+            pass
+
+    def resolve_validators(self):
         """Resolve dotted path file validators"""
 
         import importlib
 
         from filer.settings import FILE_VALIDATORS, FILER_MIME_TYPE_WHITELIST
 
         if (
@@ -33,7 +54,14 @@
                     split = item.rsplit(".", 1)
                     try:
                         module = importlib.import_module(split[0])
                         functions.append(getattr(module, split[-1]))
                     except (ImportError, ModuleNotFoundError, AttributeError):
                         raise ImproperlyConfigured(f"""filer: could not import validator "{item}".""")
             self.FILE_VALIDATORS[mime_type] = functions
+
+    def ready(self):
+        # Make webp mime type known to python (needed for python < 3.11)
+        mimetypes.add_type("image/webp", ".webp")
+        #
+        self.resolve_validators()
+        self.register_optional_heif_supprt()
```

### Comparing `django-filer-3.0.0rc3/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.0.1/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/fields/file.py` & `django-filer-3.0.1/filer/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/fields/folder.py` & `django-filer-3.0.1/filer/fields/folder.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/fields/multistorage_file.py` & `django-filer-3.0.1/filer/fields/multistorage_file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: django Filer*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0300 0000 2c00 0000 0000 0000  $.......,.......
-00000020: 3800 0000 c601 0000 3900 0000 0100 0000  8.......9.......
+00000020: 3800 0000 ce01 0000 3900 0000 0100 0000  8.......9.......
 00000030: 0000 0000 0000 0000 0050 726f 6a65 6374  .........Project
 00000040: 2d49 642d 5665 7273 696f 6e3a 2064 6a61  -Id-Version: dja
 00000050: 6e67 6f20 4669 6c65 720a 5265 706f 7274  ngo Filer.Report
 00000060: 2d4d 7367 6964 2d42 7567 732d 546f 3a20  -Msgid-Bugs-To: 
 00000070: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
-00000080: 653a 2032 3031 382d 3034 2d30 3920 3036  e: 2018-04-09 06
-00000090: 3a35 382b 3030 3030 0a4c 6173 742d 5472  :58+0000.Last-Tr
-000000a0: 616e 736c 6174 6f72 3a20 7961 6b6b 7920  anslator: yakky 
-000000b0: 3c69 2e73 7061 6c6c 6574 7469 406e 6570  <i.spalletti@nep
-000000c0: 6869 6c61 2e69 743e 0a4c 616e 6775 6167  hila.it>.Languag
-000000d0: 652d 5465 616d 3a20 4172 6162 6963 2028  e-Team: Arabic (
-000000e0: 6874 7470 3a2f 2f77 7777 2e74 7261 6e73  http://www.trans
-000000f0: 6966 6578 2e63 6f6d 2f64 6976 696f 2f64  ifex.com/divio/d
-00000100: 6a61 6e67 6f2d 6669 6c65 722f 6c61 6e67  jango-filer/lang
-00000110: 7561 6765 2f61 722f 290a 4c61 6e67 7561  uage/ar/).Langua
-00000120: 6765 3a20 6172 0a4d 494d 452d 5665 7273  ge: ar.MIME-Vers
-00000130: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
-00000140: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
-00000150: 6e3b 2063 6861 7273 6574 3d55 5446 2d38  n; charset=UTF-8
-00000160: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
-00000170: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
-00000180: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
-00000190: 706c 7572 616c 733d 363b 2070 6c75 7261  plurals=6; plura
-000001a0: 6c3d 6e3d 3d30 203f 2030 203a 206e 3d3d  l=n==0 ? 0 : n==
-000001b0: 3120 3f20 3120 3a20 6e3d 3d32 203f 2032  1 ? 1 : n==2 ? 2
-000001c0: 203a 206e 2531 3030 3e3d 3320 2626 206e   : n%100>=3 && n
-000001d0: 2531 3030 3c3d 3130 203f 2033 203a 206e  %100<=10 ? 3 : n
-000001e0: 2531 3030 3e3d 3131 2026 2620 6e25 3130  %100>=11 && n%10
-000001f0: 303c 3d39 3920 3f20 3420 3a20 353b 0a00  0<=99 ? 4 : 5;..
+00000080: 653a 2032 3031 322d 3037 2d31 3320 3135  e: 2012-07-13 15
+00000090: 3a35 302b 3030 3030 0a4c 6173 742d 5472  :50+0000.Last-Tr
+000000a0: 616e 736c 6174 6f72 3a20 416e 6765 6c6f  anslator: Angelo
+000000b0: 2044 696e 6920 3c66 696e 616c 616e 6765   Dini <finalange
+000000c0: 6c6a 7040 686f 746d 6169 6c2e 636f 6d3e  ljp@hotmail.com>
+000000d0: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
+000000e0: 4172 6162 6963 2028 6874 7470 3a2f 2f61  Arabic (http://a
+000000f0: 7070 2e74 7261 6e73 6966 6578 2e63 6f6d  pp.transifex.com
+00000100: 2f64 6976 696f 2f64 6a61 6e67 6f2d 6669  /divio/django-fi
+00000110: 6c65 722f 6c61 6e67 7561 6765 2f61 722f  ler/language/ar/
+00000120: 290a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ).MIME-Version: 
+00000130: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
+00000140: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
+00000150: 6172 7365 743d 5554 462d 380a 436f 6e74  arset=UTF-8.Cont
+00000160: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
+00000170: 6f64 696e 673a 2038 6269 740a 4c61 6e67  oding: 8bit.Lang
+00000180: 7561 6765 3a20 6172 0a50 6c75 7261 6c2d  uage: ar.Plural-
+00000190: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+000001a0: 363b 2070 6c75 7261 6c3d 6e3d 3d30 203f  6; plural=n==0 ?
+000001b0: 2030 203a 206e 3d3d 3120 3f20 3120 3a20   0 : n==1 ? 1 : 
+000001c0: 6e3d 3d32 203f 2032 203a 206e 2531 3030  n==2 ? 2 : n%100
+000001d0: 3e3d 3320 2626 206e 2531 3030 3c3d 3130  >=3 && n%100<=10
+000001e0: 203f 2033 203a 206e 2531 3030 3e3d 3131   ? 3 : n%100>=11
+000001f0: 2026 2620 6e25 3130 303c 3d39 3920 3f20   && n%100<=99 ? 
+00000200: 3420 3a20 353b 0a00                      4 : 5;..
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Arabic (http://www.transifex.com/divio/django-filer/language/"
-"ar/)\n"
-"Language: ar\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Arabic (http://app.transifex.com/divio/django-filer/language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Language: ar\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -444,14 +445,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -462,26 +464,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -530,14 +534,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -658,16 +663,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -734,16 +739,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -934,19 +939,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1000,18 +1007,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1073,14 +1082,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1128,14 +1138,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1153,14 +1164,44 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Bulgarian (http://www.transifex.com/divio/django-filer/"
-"language/bg/)\n"
-"Language: bg\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Bulgarian (http://app.transifex.com/divio/django-filer/language/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -439,14 +441,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -457,26 +460,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -525,14 +530,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -653,16 +659,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -729,16 +735,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -921,19 +927,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -987,18 +995,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1056,14 +1066,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1111,14 +1122,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1136,14 +1148,44 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2013-2014,2016\n"
 "Language-Team: Catalan (http://app.transifex.com/divio/django-filer/language/"
 "ca/)\n"
-"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s fitxer"
 msgstr[1] "%(counter)s fitxers"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Roger Pons <rogerpons@gmail.com>, 2013-2014,2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2013-2014,2016\n"
-"Language-Team: Catalan (http://app.transifex.com/divio/django-filer/language/"
-"ca/)\n"
-"Language: ca\n"
+"Language-Team: Catalan (http://app.transifex.com/divio/django-filer/language/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avançat"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL canònica"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Cal seleccionar els elements en ordre per tal de realitzar accions sobre "
-"ells. No s'ha modificat cap element."
+msgstr "Cal seleccionar els elements en ordre per tal de realitzar accions sobre ells. No s'ha modificat cap element."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s seleccionat"
 msgstr[1] "Tots %(total_count)s seleccionats"
@@ -124,16 +124,15 @@
 msgstr "Ja existeixen carpetes amb els noms %s a la destinació seleccionada"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"S'han mogut %(count)d fitxers i/o carpetes a la carpeta '%(destination)s'"
+msgstr "S'han mogut %(count)d fitxers i/o carpetes a la carpeta '%(destination)s'"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Moure fitxers i/o carpetes"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -150,16 +149,15 @@
 msgstr "Canviar el nom a fitxers"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"S'han copiat %(count)d fitxeres i/o carpetes a la carpeta '%(destination)s'."
+msgstr "S'han copiat %(count)d fitxeres i/o carpetes a la carpeta '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copiar fitxers i/o carpetes"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,17 +181,15 @@
 msgstr "Sufix que serà afegit als noms de fitxer dels fitxers copiats"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"El sufix ha de ser una part de nom de fitxer vàlida, simple i en minúscules, "
-"com ara \"%(valid)s\"."
+msgstr "El sufix ha de ser una part de nom de fitxer vàlida, simple i en minúscules, com ara \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Format de renombrat amb valor de clau \"%(key)s\" desconegut."
 
 #: admin/forms.py:54
@@ -370,17 +366,15 @@
 msgid "Permissions disabled"
 msgstr "Permisos desactivats"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Desactiveu tots els permisos d'aquest fitxer. Aquest serà accessible de "
-"forma pública per a tothom."
+msgstr "Desactiveu tots els permisos d'aquest fitxer. Aquest serà accessible de forma pública per a tothom."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -448,14 +442,15 @@
 msgstr "permís de carpeta"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permisos de carpeta"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -466,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data agafada"
 
@@ -534,14 +531,15 @@
 msgstr "arrel"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Executar l'acció seleccionada"
 
@@ -549,16 +547,15 @@
 msgid "Go"
 msgstr "Anar"
 
 #: templates/admin/filer/actions.html:14
 #: templates/admin/filer/folder/directory_table_list.html:232
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 msgid "Click here to select the objects across all pages"
-msgstr ""
-"Cliqueu aquí per seleccionar els objectes a través de totes les pàgines"
+msgstr "Cliqueu aquí per seleccionar els objectes a través de totes les pàgines"
 
 #: templates/admin/filer/actions.html:14
 #, python-format
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Seleccionar tots els %(total_count)s fitixers i/o carpetes"
 
 #: templates/admin/filer/actions.html:16
@@ -602,34 +599,27 @@
 msgstr "Duplicats"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Esborrar els fitxers seleccionats provocarà l'esborrar d'objectes "
-"relacionats, però el teu compte no té permisos per esborrar els següents "
-"tipus d'objectes:"
+msgstr "Esborrar els fitxers seleccionats provocarà l'esborrar d'objectes relacionats, però el teu compte no té permisos per esborrar els següents tipus d'objectes:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Esborrer els fitxers i/o carpetes seleccionades provocarà l'esborrat dels "
-"següents objectes protegits relacionats:"
+msgstr "Esborrer els fitxers i/o carpetes seleccionades provocarà l'esborrat dels següents objectes protegits relacionats:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Segur que voleu esborrar els fitxers i/o carpetes seleccionades? Els "
-"següents objectes i els seus elements relacionats seran esborrats:"
+msgstr "Segur que voleu esborrar els fitxers i/o carpetes seleccionades? Els següents objectes i els seus elements relacionats seran esborrats:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "No, porta'm enrere."
 
@@ -670,16 +660,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icona de la carpeta"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr "Sense permisos per copiar tots els fitxers i/o carpetes seleccionats."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -696,17 +686,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "No hi ha fitxers i/o carpetes disponibles."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Els següents fitxers i/o carpetes seran copiats a una carpeta de destí "
-"(mantenint la seva estructura d'arbre):"
+msgstr "Els següents fitxers i/o carpetes seran copiats a una carpeta de destí (mantenint la seva estructura d'arbre):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Carpeta de destí:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -718,98 +706,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "No està permès copiar fitxers a la mateixa carpeta"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"El vostre compte no té permisos per redimensionar totes les imatges "
-"seleccionades."
+msgstr "El vostre compte no té permisos per redimensionar totes les imatges seleccionades."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "No hi ha imatges disponibles per redimensionar."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Les següents imatges seran redimensionades:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Trieu una opció de miniatura existent o especifiqueu paràmetres de "
-"redimensionat:"
+msgstr "Trieu una opció de miniatura existent o especifiqueu paràmetres de redimensionat:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Trieu els paràmetres de redimensionat:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Avís: les imatges seran redimensionades al mateix lloc i les originals es "
-"perdran. Considereu realitzar abans una còpia d'aquestes per mantenir els "
-"originals."
+msgstr "Avís: les imatges seran redimensionades al mateix lloc i les originals es perdran. Considereu realitzar abans una còpia d'aquestes per mantenir els originals."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"El vostre compte no té permisos per moure tots els fitxers i/o carpetes "
-"seleccionats."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "El vostre compte no té permisos per moure tots els fitxers i/o carpetes seleccionats."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "No hi ha fitxers i/o carpetes disponibles per moure."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Els següents fitxers i/o carpetes seran moguts a una carpeta de destí "
-"(mantenint la seva estructura d'arbre):"
+msgstr "Els següents fitxers i/o carpetes seran moguts a una carpeta de destí (mantenint la seva estructura d'arbre):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Moure"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "No està permès moure fitxers a la mateixa carpeta"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"El vostre compte no té permisos per canviar el nom de tots els fitxers "
-"seleccionats."
+msgstr "El vostre compte no té permisos per canviar el nom de tots els fitxers seleccionats."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "No hi ha fitxers per canviar el nom disponibles."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"En canviarà el nom dels següents fitxers (seguiran estant a les seves "
-"carpetes i mantindran el seu nom de fitxers original, només serà modificat "
-"el nom que es mostrarà):"
+msgstr "En canviarà el nom dels següents fitxers (seguiran estant a les seves carpetes i mantindran el seu nom de fitxers original, només serà modificat el nom que es mostrarà):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Canviar el nom"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -956,19 +928,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "activat"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Esborrar fitxer"
 
@@ -1022,18 +996,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Seleccionar tots/es %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Afegir nou"
@@ -1091,14 +1067,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipus"
 
@@ -1146,14 +1123,15 @@
 msgstr "Cercar"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Escollir Fitxer"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Jakub Dorňák <jakub.dornak@misli.cz>, 2020\n"
 "Language-Team: Czech (http://app.transifex.com/divio/django-filer/language/"
 "cs/)\n"
-"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "0 of %(cnt)s selected"
 msgstr "žádná položka z %(cnt)s není vybrána"
 
 msgid "Action"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Jakub Dorňák <jakub.dornak@misli.cz>, 2020
 # Mirek Simek <miroslav.simek@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Jakub Dorňák <jakub.dornak@misli.cz>, 2020\n"
-"Language-Team: Czech (http://app.transifex.com/divio/django-filer/language/"
-"cs/)\n"
-"Language: cs\n"
+"Language-Team: Czech (http://app.transifex.com/divio/django-filer/language/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Language: cs\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Pokročilé"
 
 #: admin/fileadmin.py:160
@@ -126,17 +127,15 @@
 msgstr "Složky pojmenované %s již v cílové složce existují"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Vybrané soubory a/nebo složky (%(count)d) byly přesunuty do složky "
-"'%(destination)s'."
+msgstr "Vybrané soubory a/nebo složky (%(count)d) byly přesunuty do složky '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Přesunout soubory a/nebo složky"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -153,17 +152,15 @@
 msgstr "Přejmenovat soubory"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Soubory a/nebo složky (%(count)d) byly zkopírovány do složky "
-"'%(destination)s'."
+msgstr "Soubory a/nebo složky (%(count)d) byly zkopírovány do složky '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopírovat soubory a/nebo složky"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -187,17 +184,15 @@
 msgstr "Koncovka, která bude přidána ke jménům kopírovaných souborů."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Koncovka by měla být jednoduchá součást názvu souboru malými písmeny, "
-"například \"%(valid)s\"."
+msgstr "Koncovka by měla být jednoduchá součást názvu souboru malými písmeny, například \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Neznámý formát klíče pro přejmenování \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -223,17 +218,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "zvětšit"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Musíte vybrat předdefinované volby náhledu nebo nastavit jednotlivé "
-"parametry."
+msgstr "Musíte vybrat předdefinované volby náhledu nebo nastavit jednotlivé parametry."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Parametry pro změny velikosti musí být vybrány."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -376,17 +369,15 @@
 msgid "Permissions disabled"
 msgstr "Oprávnění neaktivní"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Deaktivovat veškerá oprávnění pro tento soubor. Soubor bude komukoli veřejně "
-"dostupný."
+msgstr "Deaktivovat veškerá oprávnění pro tento soubor. Soubor bude komukoli veřejně dostupný."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -454,14 +445,15 @@
 msgstr "oprávnění složky"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "oprávnění složky"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -472,26 +464,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum pořízení"
 
@@ -540,14 +534,15 @@
 msgstr "kořenová složka"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Provést vybranou operaci"
 
@@ -607,34 +602,27 @@
 msgstr "Duplicity"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Smazání vybraných souborů a/nebo složek bude mít za následek smazání všech "
-"přidružených objektů, nicméně ke smazání následujících objektů nemáte "
-"oprávnění:"
+msgstr "Smazání vybraných souborů a/nebo složek bude mít za následek smazání všech přidružených objektů, nicméně ke smazání následujících objektů nemáte oprávnění:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Smazání vybraných souborů a/nebo složek bude mít za následek smazání "
-"následujících přidružených objektů:"
+msgstr "Smazání vybraných souborů a/nebo složek bude mít za následek smazání následujících přidružených objektů:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Opravdu chcete smazat vybrané soubory a složky? Všechny následující objekty "
-"budou smazány:"
+msgstr "Opravdu chcete smazat vybrané soubory a složky? Všechny následující objekty budou smazány:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ne, chci zpátky"
 
@@ -675,16 +663,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona složky"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr "Nemáte oprávnění kopírovat vybrané soubory a/nebo složky."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -701,17 +689,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Žádné soubory ani složky není možno kopírovat."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Následující soubory a/nebo složky budou zkopírovány do cílové slžoky (jejich "
-"stromová struktura bude zachována):"
+msgstr "Následující soubory a/nebo složky budou zkopírovány do cílové slžoky (jejich stromová struktura bude zachována):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cílová složka:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -735,51 +721,45 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Následujícím obrázkům bude změněna velikost:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Vyberte existující volby náhledu nebo zadejte parametry změny velikosti:"
+msgstr "Vyberte existující volby náhledu nebo zadejte parametry změny velikosti:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Vyberte parametry změny velikosti:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Varování: Bude změněna velikost obrázků a původní obrázky budou přepsány. "
-"Pokud chcete zachovat obrázky v původní velikosti, nejdříve vytvořte jejich "
-"kopie."
+msgstr "Varování: Bude změněna velikost obrázků a původní obrázky budou přepsány. Pokud chcete zachovat obrázky v původní velikosti, nejdříve vytvořte jejich kopie."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Změnit velikost"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr "Nemáte oprávnění k přesunu vybraných souborů nebo složek."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Žádné soubory k přesunutí."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Následující soubory a/nebo složky budou přesunyty do cílové složky (jejich "
-"stromová struktura bude zachována)"
+msgstr "Následující soubory a/nebo složky budou přesunyty do cílové složky (jejich stromová struktura bude zachována)"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Přesunout"
 
@@ -796,16 +776,15 @@
 msgid "There are no files available to rename."
 msgstr "Žádné soubory k přejmenování."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Následující soubory budou přejmenovány (změněno bude pouze zobrazované jméno)"
+msgstr "Následující soubory budou přejmenovány (změněno bude pouze zobrazované jméno)"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Přejmenovat"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -956,19 +935,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivní"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanonický odkaz '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Stáhnout '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Smazat soubor"
 
@@ -1022,18 +1003,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Vybrat všechny (%(total_count)s)"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Přidat"
@@ -1093,14 +1076,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Typ"
 
@@ -1148,14 +1132,15 @@
 msgstr "Vyhledat"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Vybrat soubor"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Luis Zárate <luisza@visualcon.net>, 2019\n"
 "Language-Team: Spanish (http://app.transifex.com/divio/django-filer/language/"
 "es/)\n"
-"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s archivo"
 msgstr[1] "%(counter)s archivos"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Cristian Acevedo <arucar17@gmail.com>, 2016
 # David <d.diazp@gmail.com>, 2015
 # Jason Gass Martinez <jason.tra@jason-pc.tk>, 2016
 # Luis Zárate <luisza@visualcon.net>, 2019
@@ -16,50 +16,49 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Luis Zárate <luisza@visualcon.net>, 2019\n"
-"Language-Team: Spanish (http://app.transifex.com/divio/django-filer/language/"
-"es/)\n"
-"Language: es\n"
+"Language-Team: Spanish (http://app.transifex.com/divio/django-filer/language/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
-"1 : 2;\n"
+"Language: es\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avanzado"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL canónica"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Los elementos deben estar seleccionados para efectuar acciones sobre ellos. "
-"Ningún elemento ha sido modificado."
+msgstr "Los elementos deben estar seleccionados para efectuar acciones sobre ellos. Ningún elemento ha sido modificado."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] " %(total_count)s seleccionado"
 msgstr[1] "Todos los %(total_count)s seleccionados"
@@ -133,17 +132,15 @@
 msgstr "Las carpetas con los nombres %s ya existen en el destino seleccionado"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Movidos con éxito %(count)d ficheros y/o directorios al directorio "
-"'%(destination)s'."
+msgstr "Movidos con éxito %(count)d ficheros y/o directorios al directorio '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Mover ficheros y/o directorios"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -160,17 +157,15 @@
 msgstr "Cambiar el nombre de los archivos"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Copiados con éxito %(count)d ficheros y/o directorios al directorio "
-"'%(destination)s'."
+msgstr "Copiados con éxito %(count)d ficheros y/o directorios al directorio '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copiar ficheros y/o directorios"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -187,31 +182,27 @@
 
 #: admin/folderadmin.py:1292
 msgid "Resize selected images"
 msgstr "Cambiar el tamaño de imágenes seleccionadas."
 
 #: admin/forms.py:24
 msgid "Suffix which will be appended to filenames of copied files."
-msgstr ""
-"Sufijo que se añadirá al nombre de los archivos de los archivos copiados."
+msgstr "Sufijo que se añadirá al nombre de los archivos de los archivos copiados."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"El sufijo debe ser una parte válida de un nombre de fichero, simple y en "
-"minúsculas, como \"%(valid)s\"."
+msgstr "El sufijo debe ser una parte válida de un nombre de fichero, simple y en minúsculas, como \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
-msgstr ""
-"Formato de cambio de nombre con valor de clave \"%(key)s\" desconocido."
+msgstr "Formato de cambio de nombre con valor de clave \"%(key)s\" desconocido."
 
 #: admin/forms.py:54
 #, python-format
 msgid "Invalid rename format: %(error)s."
 msgstr "Formato de cambio de nombre no válido: %(error)s."
 
 #: admin/forms.py:64 models/thumbnailoptionmodels.py:37
@@ -232,17 +223,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "ampliar"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Se debe elegir una opción de miniatura o unos parámetros para el cambio de "
-"tamaño."
+msgstr "Se debe elegir una opción de miniatura o unos parámetros para el cambio de tamaño."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Se deben elegir unos parámetros para el cambio de tamaño."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -385,17 +374,15 @@
 msgid "Permissions disabled"
 msgstr "Permisos desactivados"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Desactiva cualquier comprobación de permiso para este archivo. El archivo "
-"será accesible públicamente para todos."
+msgstr "Desactiva cualquier comprobación de permiso para este archivo. El archivo será accesible públicamente para todos."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -463,14 +450,15 @@
 msgstr "permiso de la carpeta"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permisos de la carpeta"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -481,26 +469,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "fecha"
 
@@ -549,14 +539,15 @@
 msgstr "raíz"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Ejecutar la acción seleccionada"
 
@@ -564,16 +555,15 @@
 msgid "Go"
 msgstr "Continuar"
 
 #: templates/admin/filer/actions.html:14
 #: templates/admin/filer/folder/directory_table_list.html:232
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 msgid "Click here to select the objects across all pages"
-msgstr ""
-"Haz clic aquí para seleccionar los objetos a través de todas las páginas"
+msgstr "Haz clic aquí para seleccionar los objetos a través de todas las páginas"
 
 #: templates/admin/filer/actions.html:14
 #, python-format
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Seleccionar los %(total_count)s archivos y/o carpetas"
 
 #: templates/admin/filer/actions.html:16
@@ -617,34 +607,27 @@
 msgstr "Duplicados"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Borrar los archivos y/o carpetas seleccionados borraría los objetos "
-"seleccionados, pero tu cuenta no tiene permiso para borrar los siguientes "
-"tipos de objetos:"
+msgstr "Borrar los archivos y/o carpetas seleccionados borraría los objetos seleccionados, pero tu cuenta no tiene permiso para borrar los siguientes tipos de objetos:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Borrar los archivos y/o carpetas requeriría borrar los siguientes objetos "
-"relacionados protegidos:"
+msgstr "Borrar los archivos y/o carpetas requeriría borrar los siguientes objetos relacionados protegidos:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"¿Estás seguro de que quieres borrar los archivos y/o carpetas seleccionados? "
-"Los siguientes objetos y sus elementos relacionados serán borrados:"
+msgstr "¿Estás seguro de que quieres borrar los archivos y/o carpetas seleccionados? Los siguientes objetos y sus elementos relacionados serán borrados:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "No, ir atrás"
 
@@ -685,19 +668,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icono de la Carpeta"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Tu cuenta no tiene permisos para copiar todos los archivos y/o carpetas "
-"seleccionados."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Tu cuenta no tiene permisos para copiar todos los archivos y/o carpetas seleccionados."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -713,17 +694,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "No hay archivos y/o carpetas disponibles para copiar."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Los siguientes archivos y/o carpetas serán copiados a una carpeta de destino "
-"(manteniendo su estructura en árbol):"
+msgstr "Los siguientes archivos y/o carpetas serán copiados a una carpeta de destino (manteniendo su estructura en árbol):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Carpeta de destino:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -735,96 +714,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "No está permitido copiar los archivos dentro de la misma carpeta"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Tu cuenta no tiene permisos para cambiar el tamaño de todas las imágenes "
-"seleccionadas."
+msgstr "Tu cuenta no tiene permisos para cambiar el tamaño de todas las imágenes seleccionadas."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "No hay imágenes disponibles a las que cambiarles el tamaño."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Se les cambiará el tamaño a las siguientes imágenes:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Elige una opción de miniatura existente o introduce parámetros para el "
-"cambio de tamaño:"
+msgstr "Elige una opción de miniatura existente o introduce parámetros para el cambio de tamaño:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Elegir parámetros para el cambio de tamaño:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Aviso: se cambiará el tamaño de las imágenes en el mismo sitio y los "
-"originales se perderán. Considera realizar una copia de aquellas para "
-"conservar los originales."
+msgstr "Aviso: se cambiará el tamaño de las imágenes en el mismo sitio y los originales se perderán. Considera realizar una copia de aquellas para conservar los originales."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Cambiar de tamaño"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Tu cuenta no tiene permisos para mover todos los archivos y/o carpetas "
-"seleccionados."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Tu cuenta no tiene permisos para mover todos los archivos y/o carpetas seleccionados."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "No hay archivos y/o carpetas disponibles para mover."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Los siguientes archivos y/o directorios serán movidos a una carpeta de "
-"destino (manteniendo su estructura de árbol):"
+msgstr "Los siguientes archivos y/o directorios serán movidos a una carpeta de destino (manteniendo su estructura de árbol):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Mover"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "No está permitido mover los archivos dentro de la misma carpeta"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Tu cuenta no tiene permisos para renombrar todos los objetos seleccionados."
+msgstr "Tu cuenta no tiene permisos para renombrar todos los objetos seleccionados."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "No hay archivos disponibles a los que cambiar el nombre."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Los siguientes archivos serán renombrados (se quedarán en sus carpetas y "
-"mantendrán su nombre original, solo los nombres mostrados serán cambiados):"
+msgstr "Los siguientes archivos serán renombrados (se quedarán en sus carpetas y mantendrán su nombre original, solo los nombres mostrados serán cambiados):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Cambiar el nombre"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -973,19 +938,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "activado"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Url canónica '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Descargar '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Eliminar archivo"
 
@@ -1039,18 +1006,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Seleccionar todo %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Añadir nuevo"
@@ -1109,14 +1078,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
@@ -1164,14 +1134,15 @@
 msgstr "Buscar"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Selecciona el archivo"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Johan Viirok, 2022\n"
 "Language-Team: Estonian (http://app.transifex.com/divio/django-filer/"
 "language/et/)\n"
-"Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s fail"
 msgstr[1] "%(counter)s faili"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/et/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Johan Viirok, 2022
 # Martin <martinpajuste@gmail.com>, 2016
 # Rivo Zängov <eraser@eraser.ee>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Johan Viirok, 2022\n"
-"Language-Team: Estonian (http://app.transifex.com/divio/django-filer/"
-"language/et/)\n"
-"Language: et\n"
+"Language-Team: Estonian (http://app.transifex.com/divio/django-filer/language/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -442,14 +444,15 @@
 msgstr "kausta õigus"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "kausta õigused"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -460,26 +463,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -528,14 +533,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -656,16 +662,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Kausta ikoon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -732,16 +738,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Muuda suurust"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -924,19 +930,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "sisse lülitatud"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Lae alla '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Eemalda fail"
 
@@ -990,18 +998,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Vali kõik %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Lisa uus"
@@ -1059,14 +1069,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tüüp"
 
@@ -1114,14 +1125,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Vali fail"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Ales Zabala Alava <shagi@gisa-elkartea.org>, 2013\n"
 "Language-Team: Basque (http://app.transifex.com/divio/django-filer/language/"
 "eu/)\n"
-"Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "bat haututa"
 msgstr[1] "%(total_count)s hautatuta"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Ales Zabala Alava <shagi@gisa-elkartea.org>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Ales Zabala Alava <shagi@gisa-elkartea.org>, 2013\n"
-"Language-Team: Basque (http://app.transifex.com/divio/django-filer/language/"
-"eu/)\n"
-"Language: eu\n"
+"Language-Team: Basque (http://app.transifex.com/divio/django-filer/language/eu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Aurreratua"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Elementuak hautatu behar dira beraiekin zeozer egiteko. Ez da elementurik "
-"aldatu."
+msgstr "Elementuak hautatu behar dira beraiekin zeozer egiteko. Ez da elementurik aldatu."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "bat haututa"
 msgstr[1] "%(total_count)s hautatuta"
@@ -124,16 +124,15 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fitxategi eta/edo karpeta '%(destination)s' karpetara mugituta."
+msgstr "%(count)d fitxategi eta/edo karpeta '%(destination)s' karpetara mugituta."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Fitxategi eta/edo karpetak mugitu"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -150,16 +149,15 @@
 msgstr "Fitxategiak berrizendatu"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fitxategi eta/edo karpeta %(destination)s karpetara kopiatuta."
+msgstr "%(count)d fitxategi eta/edo karpeta %(destination)s karpetara kopiatuta."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Fitxategi eta/edo karpetak kopiatu"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,17 +181,15 @@
 msgstr "Kopiatutako fitxategiei gehituko zaien atzizkia."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Atzizkia baliozko, sinple eta letra xehetan dagoen fitxategi izen zatia izan "
-"beharko luke, \"%(valid)s\" bezala."
+msgstr "Atzizkia baliozko, sinple eta letra xehetan dagoen fitxategi izen zatia izan beharko luke, \"%(valid)s\" bezala."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Berrizendatze formatuko gako balio ezezaguna \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -219,16 +215,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "handitu"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Argazkitxo aukerak edo tamaina aldatzeko parametroak zehaztu behar dira."
+msgstr "Argazkitxo aukerak edo tamaina aldatzeko parametroak zehaztu behar dira."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Tamaina aldatzeko parametroak zehaztu behar dira."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -447,14 +442,15 @@
 msgstr "karpeta baimena"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "karpeta baimenak"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -465,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "sortze data"
 
@@ -533,14 +531,15 @@
 msgstr "erroa"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Hautatutako ekintza abiarazi"
 
@@ -612,17 +611,15 @@
 "following protected related objects:"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Ziur hautatutako fitxategi eta/edo karpetak ezabatu nahi dituzula? Ondoko "
-"objektu eta erlazionatutako elementu guztiak ezabatuko lirateke:"
+msgstr "Ziur hautatutako fitxategi eta/edo karpetak ezabatu nahi dituzula? Ondoko objektu eta erlazionatutako elementu guztiak ezabatuko lirateke:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -663,16 +660,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Karpeta ikonoa"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -721,40 +718,35 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Ondoko irudien tamaina aldatuko da:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Argazkitxo aukera bat hautatu edo tamaina aldatzeko parametroak ezarri:"
+msgstr "Argazkitxo aukera bat hautatu edo tamaina aldatzeko parametroak ezarri:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Tamaina aldatzeko parametroak aukeratu:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Kontuz: Irudien tamaina aldatzean jatorrizkoak galduko dira. Lehenbizi "
-"jatorrizkoen kopia egin zenezake."
+msgstr "Kontuz: Irudien tamaina aldatzean jatorrizkoak galduko dira. Lehenbizi jatorrizkoen kopia egin zenezake."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Tamaina aldatu"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Zure kontuak ez du hautatutako fitxategi eta/edo karpeta guztiak mugitzeko "
-"baimenik."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Zure kontuak ez du hautatutako fitxategi eta/edo karpeta guztiak mugitzeko baimenik."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Ez dago mugitu daitekeen fitxategi edo/eta karpetarik."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
@@ -936,19 +928,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "gaituta"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1002,18 +996,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Berria gehitu"
@@ -1071,14 +1067,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1126,14 +1123,15 @@
 msgstr "Bilatu"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Persian (http://www.transifex.com/divio/django-filer/language/"
-"fa/)\n"
-"Language: fa\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Japanese (http://app.transifex.com/divio/django-filer/language/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -438,14 +440,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +459,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +529,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +658,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +734,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -918,19 +924,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +992,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1052,14 +1062,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1118,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,14 +1144,44 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Teemu Gratschev <teemu.gratschev@gmail.com>, 2022\n"
 "Language-Team: Finnish (http://app.transifex.com/divio/django-filer/language/"
 "fi/)\n"
-"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s tiedosto"
 msgstr[1] "%(counter)s tiedostoa"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Niklas Jerva <niklas.jerva@gmail.com>, 2016
 # Teemu Gratschev <teemu.gratschev@gmail.com>, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Teemu Gratschev <teemu.gratschev@gmail.com>, 2022\n"
-"Language-Team: Finnish (http://app.transifex.com/divio/django-filer/language/"
-"fi/)\n"
-"Language: fi\n"
+"Language-Team: Finnish (http://app.transifex.com/divio/django-filer/language/fi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Edistyneet asetukset"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "sääntöjenmukainen URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Toiminnon suorittamiseksi pitää valita kohteita. Yhtäänkohdetta ei ole "
-"valittu."
+msgstr "Toiminnon suorittamiseksi pitää valita kohteita. Yhtäänkohdetta ei ole valittu."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s valittu"
 msgstr[1] "Kaikki %(total_count)s valittu"
@@ -125,16 +125,15 @@
 msgstr "%s niminen kansio on jo valitussa kohteessa"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d tiedostoa ja/tai kansiota siirretty kansioon '%(destination)s'."
+msgstr "%(count)d tiedostoa ja/tai kansiota siirretty kansioon '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Siirrä tiedostot ja/tai kansiot"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -151,16 +150,15 @@
 msgstr "Nimeä tiedostot uudelleen"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d tiedostoa ja/tai kansiota kopioitu kansioon '%(destination)s'."
+msgstr "%(count)d tiedostoa ja/tai kansiota kopioitu kansioon '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopioi tiedostot ja/tai kansiot"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -184,17 +182,15 @@
 msgstr "Pääte, joka lisätään kopioitujen tiedostojen nimiin."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Päätteen tulee olla käypä, yksinkertainen ja pienellä kirjoitettu osa "
-"tiedostonimeä, esim. \"%(valid)s\"."
+msgstr "Päätteen tulee olla käypä, yksinkertainen ja pienellä kirjoitettu osa tiedostonimeä, esim. \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Tuntematon uudelleennimeämisarvo \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -371,17 +367,15 @@
 msgid "Permissions disabled"
 msgstr "Käyttöoikeudet pois käytöstä"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Poista käyttöoikeuksien tarkistus tältä tiedostolta. Tiedosto näkyy "
-"julkisena kaikille."
+msgstr "Poista käyttöoikeuksien tarkistus tältä tiedostolta. Tiedosto näkyy julkisena kaikille."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -449,14 +443,15 @@
 msgstr "kansion käyttöoikeus"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "kansion käyttöoikeudet"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -467,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "päivämäärä"
 
@@ -535,14 +532,15 @@
 msgstr "juuri"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Suorita valittu toiminto"
 
@@ -602,34 +600,27 @@
 msgstr "Kaksoiskappaleet"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Valittujen tiedostojen ja/tai kansioiden poistaminen vaatii liittyvien "
-"objektien poistamista, mutta käyttöoikeutesi eivät riitäseuraavien "
-"objektityyppien poistamiseen:"
+msgstr "Valittujen tiedostojen ja/tai kansioiden poistaminen vaatii liittyvien objektien poistamista, mutta käyttöoikeutesi eivät riitäseuraavien objektityyppien poistamiseen:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Valittujen tiedostojen ja/tai kansioiden poistaminen vaatisi seuraavien "
-"suojattujen liittyvien objektien poistamista:"
+msgstr "Valittujen tiedostojen ja/tai kansioiden poistaminen vaatisi seuraavien suojattujen liittyvien objektien poistamista:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Oletko varma, että haluat poistaa valitut tiedostot ja/tai kansiot? Kaikki "
-"seuraavat objektit ja niihin liittyvät kohteet poistetaan:"
+msgstr "Oletko varma, että haluat poistaa valitut tiedostot ja/tai kansiot? Kaikki seuraavat objektit ja niihin liittyvät kohteet poistetaan:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ei, vie minut takaisin"
 
@@ -670,19 +661,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Kansion kuvake"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai "
-"kansioidenkopioimiseen."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai kansioidenkopioimiseen."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -698,17 +687,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Kopioitavia tiedostoja ja/tai kansioita ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Seuraavat tiedostot ja/tai kansiot kopioidaan kohdekansioon (säilyttäen "
-"puurakenteen):"
+msgstr "Seuraavat tiedostot ja/tai kansiot kopioidaan kohdekansioon (säilyttäen puurakenteen):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Kohdekansio:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -720,16 +707,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Tiedostojen kopiointi samaan kansioon ei ole sallittu"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Käyttöoikeutesi eivät riitä kaikkien valittujen kuvien koon muuttamiseen."
+msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen kuvien koon muuttamiseen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Kuvia, joiden kokoa voisi muuttaa ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
@@ -743,71 +729,60 @@
 msgid "Choose resize parameters:"
 msgstr "Valitse kokoparametrit:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Varoitus: Kuvien kokoa muuttaessa alkuperäiset versiot menetetään. On hyvä "
-"idea tehdä kuvista ensin kopiot alkuperäisten säilyttämiseksi."
+msgstr "Varoitus: Kuvien kokoa muuttaessa alkuperäiset versiot menetetään. On hyvä idea tehdä kuvista ensin kopiot alkuperäisten säilyttämiseksi."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Muuta kokoa"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai "
-"kansioidensiirtämiseen."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai kansioidensiirtämiseen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Siirrettäviä tiedostoja ja/tai kansioita ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Seuraavat tiedostot ja/tai kansiot siirretään kohdekansioon (säilyttäen "
-"niiden puurakenne):"
+msgstr "Seuraavat tiedostot ja/tai kansiot siirretään kohdekansioon (säilyttäen niiden puurakenne):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Siirrä"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Tiedostojen siirto samaan kansioon ei ole sallittua"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen "
-"uudelleennimeämiseen."
+msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen uudelleennimeämiseen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Uudelleennimettäviä tiedostoja ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Seuraavat tiedostot uudelleennimetään (ne pysyvät kansioissaan ja "
-"alkuperäiset tiedostonimet säilytetään, vain näytettävä tiedostonimi "
-"muutetaan):"
+msgstr "Seuraavat tiedostot uudelleennimetään (ne pysyvät kansioissaan ja alkuperäiset tiedostonimet säilytetään, vain näytettävä tiedostonimi muutetaan):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Uudelleennimeä"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -954,19 +929,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "käytössä"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Canonical-osoite '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Lataa '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Poista tiedosto"
 
@@ -1020,18 +997,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Valitse kaikki %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Lisää uusi"
@@ -1089,14 +1068,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tyyppi"
 
@@ -1144,14 +1124,15 @@
 msgstr "Haku"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Valitse tiedosto"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Nicolas PASCAL <np.pascal@gmail.com>, 2019\n"
+"Last-Translator: Corentin Bettiol, 2023\n"
 "Language-Team: French (http://app.transifex.com/divio/django-filer/language/"
 "fr/)\n"
-"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s fichier"
 msgstr[1] "%(counter)s fichiers"
@@ -33,33 +33,47 @@
 
 msgid "0 of %(cnt)s selected"
 msgstr "0 sur %(cnt)s sélectionné"
 
 msgid "Action"
 msgstr "Action"
 
+msgid "Add children"
+msgstr "Ajouter un sous-dossier"
+
 msgid "Add new"
 msgstr "Ajouter un nouveau"
 
 msgid "Adds a new Folder"
 msgstr "Ajoute un nouveau dossier"
 
 msgid "Advanced"
 msgstr "Avancé"
 
+msgid "All Folders"
+msgstr "Tous les dossiers"
+
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
 msgstr ""
 "Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? "
 "Tous les objets suivants et leurs éléments liés seront supprimés :"
 
 msgid "Are you sure?"
 msgstr "Êtes-vous sûr(e) ?"
 
+msgid "Can't find folder to upload. Please refresh and try again"
+msgstr "Dossier d'hébergement introuvable, rafraîchissez la page et réessayez."
+
+msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgstr ""
+"Utilisation du dossier impossible : Permissions insuffisantes. Sélectionnez "
+"un autre dossier."
+
 msgid "Cannot delete files and/or folders"
 msgstr "Impossible de supprimer les fichiers et/ou dossiers."
 
 msgid "Canonical url '%(item_label)s'"
 msgstr "url canonique '%(item_label)s' "
 
 msgid "Change"
@@ -79,14 +93,17 @@
 
 msgid "Check it to limit the search to current folder"
 msgstr "Cochez pour limiter la recherche au dossier actuel"
 
 msgid "Choose File"
 msgstr "Sélectionner un fichier"
 
+msgid "Choose Folder"
+msgstr "Choisissez un dossier"
+
 msgid "Choose an existing thumbnail option or enter resize parameters:"
 msgstr ""
 "Choisissez une option de miniature existante ou entrez des paramètres de "
 "redimensionnement :"
 
 msgid "Choose resize parameters:"
 msgstr "Choisissez des paramètres de redimensionnement :"
@@ -161,39 +178,79 @@
 
 msgid "Disable permissions for selected files"
 msgstr "Désactiver les permissions pour les fichiers sélectionnés."
 
 msgid "Django site admin"
 msgstr "Django site admin"
 
+msgid "Download"
+msgstr "Télécharger"
+
 msgid "Download '%(item_label)s'"
 msgstr "Télécharger '%(item_label)s' "
 
 msgid "Drop files here or use the \"Upload Files\" button"
 msgstr ""
 "Déposez des fichiers ici ou utilisez le bouton « Téléverser des fichiers »"
 
 msgid "Drop your file to upload into:"
 msgstr "Déposez votre fichier à téléverser dans :"
 
 msgid "Duplicates"
 msgstr "Duplicatas"
 
+msgid "Edit"
+msgstr "Modifier"
+
 msgid "Empty Clipboard"
 msgstr "Vider le presse-papiers"
 
 msgid "Enable permissions for selected files"
 msgstr "Activer les permissions pour les fichiers sélectionnés."
 
+msgid "Everybody"
+msgstr "Tout le monde"
+
+msgid "Expand"
+msgstr "Agrandir"
+
+msgid "File \"{file_name}\": HTML upload denied by site security policy"
+msgstr ""
+"Fichier \"{file_name}\" : hébergement HTML refusé par la politique de "
+"sécurité du site"
+
+msgid ""
+"File \"{file_name}\": Rejected due to potential cross site scripting "
+"vulnerability"
+msgstr ""
+"Fichier \"{file_name}\" : Rejeté à cause d'une potentielle vulnérabilité de "
+"cross-site scripting"
+
+msgid "File \"{file_name}\": Upload denied by site security policy"
+msgstr ""
+"Fichier \"{file_name}\" : Hébergement refusé par la politique de sécurité du "
+"site"
+
+msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
+msgstr ""
+"Fichier \"{file_name}\" : hébergement de {file_type} refusé par la politique "
+"de sécurité du site"
+
+msgid "File is missing"
+msgstr "Le fichier est manquant"
+
 msgid "File-size"
 msgstr "Taille de fichier"
 
 msgid "Filer"
 msgstr "Filer"
 
+msgid "Files"
+msgstr "Fichiers"
+
 msgid "Folder"
 msgstr "Dossier"
 
 msgid "Folder Icon"
 msgstr "Icône du dossier"
 
 msgid "Folder with this name already exists."
@@ -222,14 +279,17 @@
 
 msgid "Go back to root folder"
 msgstr "Revenir au dossier racine"
 
 msgid "Go back to the parent folder"
 msgstr "Retourner au dossier parent"
 
+msgid "Group: {group}"
+msgstr "Groupe : {group}"
+
 msgid "History"
 msgstr "Historique"
 
 msgid "Home"
 msgstr "Accueil"
 
 msgid "Invalid rename format: %(error)s."
@@ -256,14 +316,17 @@
 
 msgid "Limit the search to current folder"
 msgstr "Limiter la recherche au dossier actuel"
 
 msgid "Location of the main subject of the scene. Format: \"x,y\"."
 msgstr "Emplacement du sujet principal de la scène. Format : « x,y »."
 
+msgid "Logical Path"
+msgstr "Chemin logique"
+
 msgid "Lookup"
 msgstr "Recherche"
 
 msgid "Media library"
 msgstr "Bibliotèque multimedia"
 
 msgid "Modified"
@@ -313,14 +376,17 @@
 
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] "Veuillez corriger l'erreur suivante."
 msgstr[1] "Veuillez corriger les erreurs suivantes."
 msgstr[2] "Veuillez corriger les erreurs suivantes."
 
+msgid "Read"
+msgstr "Lire"
+
 msgid "Remove file"
 msgstr "Supprimer le fichier"
 
 msgid "Remove folder"
 msgstr "Supprimer le dossier"
 
 msgid "Rename"
@@ -346,23 +412,32 @@
 
 msgid "Save"
 msgstr "Sauvegarder"
 
 msgid "Search"
 msgstr "Rechercher"
 
+msgid "Select all"
+msgstr "Tout sélectionner"
+
 msgid "Select all %(total_count)s"
 msgstr "Sélectionner les %(total_count)s"
 
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Sélectionner tous les %(total_count)s fichiers et/ou dossiers"
 
 msgid "Select this file"
 msgstr "Sélectionner ce fichier"
 
+msgid "Show table view"
+msgstr "Voir la vue en liste"
+
+msgid "Show thumbnail view"
+msgstr "Voir la vue avec des miniatures"
+
 msgid "Size"
 msgstr "Taille"
 
 msgid "Subject location"
 msgstr "Emplacement du sujet"
 
 msgid "Subject location is outside of the image. "
@@ -475,28 +550,40 @@
 
 msgid "Upload canceled!"
 msgstr "Téléversement annulé !"
 
 msgid "Upload success!"
 msgstr "Téléversement réussi !"
 
+msgid "User: {user}"
+msgstr "Utilisateur : {user}"
+
 msgid "View on site"
 msgstr "Voir sur le site"
 
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
 msgstr ""
 "Avertissement : Les images seront redimensionnées en place et les originales "
 "seront perdues. Faites-en éventuellement une copie préalable afin de les "
 "conserver."
 
+msgid "What"
+msgstr "Quoi"
+
+msgid "Who"
+msgstr "Qui"
+
 msgid "Yes, I&#39;m sure"
 msgstr "Oui, je suis sûr"
 
+msgid "You do not have permission to upload files."
+msgstr "Vous n'avez pas la permission d'héberger des fichiers."
+
 msgid "You have to select a folder first"
 msgstr "Vous devez d'abord sélectionner un dossier"
 
 msgid ""
 "Your account doesn't have permissions to copy all of the selected files and/"
 "or folders."
 msgstr ""
@@ -518,14 +605,20 @@
 
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
 msgstr ""
 "Votre compte na pas les permissions nécessaires pour redimensionner toutes "
 "les images sélectionnées."
 
+msgid "Your browser does not support audio."
+msgstr "Votre navigateur ne supporte pas l'audio."
+
+msgid "Your browser does not support video."
+msgstr "Votre navigateur ne supporte pas la vidéo."
+
 msgid "Your input: \"{subject_location}\". "
 msgstr "Votre entrée : « {subject_location} »."
 
 msgid "admin homepage"
 msgstr "page d'accueil de l'administrateur"
 
 msgid "all items"
@@ -638,14 +731,17 @@
 
 msgid "image"
 msgstr "image"
 
 msgid "images"
 msgstr "images"
 
+msgid "inherit"
+msgstr "hériter"
+
 msgid "modified at"
 msgstr "modifié le"
 
 msgid "must always publish author credit"
 msgstr "doit toujours publier l'attribution à l'auteur"
 
 msgid "must always publish copyright"
@@ -665,14 +761,17 @@
 
 msgid "original filename"
 msgstr "nom de fichier originel"
 
 msgid "owner"
 msgstr "propriétaire"
 
+msgid "parent"
+msgstr "parent"
+
 msgid "previous"
 msgstr "précédent"
 
 msgid "root"
 msgstr "racine"
 
 msgid "sha1"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Assma Buifruri <assma.buifruri@hotmail.com>, 2017
 # Bertrand Bordage <bordage.bertrand@gmail.com>, 2012-2013
 # Sylvain Chiron <chironsylvain@orange.fr>, 2016
+# Corentin Bettiol, 2023
 # Jason Gass Martinez <jason.tra@jason-pc.tk>, 2016
 # Marion Balensi <kitsunesama@laposte.net>, 2012
 # Nicolas PASCAL <np.pascal@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Nicolas PASCAL <np.pascal@gmail.com>, 2019\n"
-"Language-Team: French (http://app.transifex.com/divio/django-filer/language/"
-"fr/)\n"
-"Language: fr\n"
+"Last-Translator: Corentin Bettiol, 2023\n"
+"Language-Team: French (http://app.transifex.com/divio/django-filer/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: fr\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
-msgstr ""
+msgstr "Vous n'avez pas la permission d'héberger des fichiers."
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
-msgstr ""
+msgstr "Dossier d'hébergement introuvable, rafraîchissez la page et réessayez."
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
-msgstr ""
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
+msgstr "Utilisation du dossier impossible : Permissions insuffisantes. Sélectionnez un autre dossier."
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avancé"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL canonique"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Des éléments doivent être sélectionnés pour effectuer les actions. Aucun "
-"élément n'a été modifié."
+msgstr "Des éléments doivent être sélectionnés pour effectuer les actions. Aucun élément n'a été modifié."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s sélectionné"
 msgstr[1] "Tous les %(total_count)s sélectionnés"
@@ -131,17 +131,15 @@
 msgstr "Des dossiers nommés %s existent déjà dans la destination sélectionnée"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fichiers et/ou dossiers déplacés avec succès vers le dossier "
-"« %(destination)s »."
+msgstr "%(count)d fichiers et/ou dossiers déplacés avec succès vers le dossier « %(destination)s »."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Déplacer les fichiers et/ou dossiers"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -158,17 +156,15 @@
 msgstr "Renommer les fichiers"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fichiers et/dossiers copiés avec succès dans le dossier "
-"« %(destination)s »."
+msgstr "%(count)d fichiers et/dossiers copiés avec succès dans le dossier « %(destination)s »."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copier les fichiers et/ou dossiers"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -192,17 +188,15 @@
 msgstr "Suffixe qui sera ajouté au nom des fichiers copiés."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Le suffixe doit être une partie de nom de fichier valide, simple et en "
-"minuscules, comme « %(valid)s »."
+msgstr "Le suffixe doit être une partie de nom de fichier valide, simple et en minuscules, comme « %(valid)s »."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "La clé de formatage « %(key)s » est inconnue."
 
 #: admin/forms.py:54
@@ -228,17 +222,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "agrandir"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Une option de miniature ou des paramètres de dimensionnement doivent être "
-"choisis."
+msgstr "Une option de miniature ou des paramètres de dimensionnement doivent être choisis."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Des paramètres de dimensionnement doivent être choisis."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -259,19 +251,19 @@
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Votre entrée : « {subject_location} »."
 
 #: admin/permissionadmin.py:10 models/foldermodels.py:379
 msgid "Who"
-msgstr ""
+msgstr "Qui"
 
 #: admin/permissionadmin.py:11 models/foldermodels.py:400
 msgid "What"
-msgstr ""
+msgstr "Quoi"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Il existe déjà un dossier avec ce nom."
 
 #: apps.py:9 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
@@ -381,21 +373,19 @@
 msgid "Permissions disabled"
 msgstr "Permissions désactivées"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Désactiver la vérification des permissions pour ce fichier. Le fichier sera "
-"publiquement accessible à tout le monde."
+msgstr "Désactiver la vérification des permissions pour ce fichier. Le fichier sera publiquement accessible à tout le monde."
 
 #: models/foldermodels.py:93
 msgid "parent"
-msgstr ""
+msgstr "parent"
 
 #: models/foldermodels.py:120
 msgid "created at"
 msgstr "créé le"
 
 #: models/foldermodels.py:135
 msgid "Folder"
@@ -416,15 +406,15 @@
 
 #: models/foldermodels.py:261
 msgid "this item and all children"
 msgstr "cet élément et ses enfants"
 
 #: models/foldermodels.py:265
 msgid "inherit"
-msgstr ""
+msgstr "hériter"
 
 #: models/foldermodels.py:266
 msgid "allow"
 msgstr "autoriser"
 
 #: models/foldermodels.py:267
 msgid "deny"
@@ -459,46 +449,49 @@
 msgstr "permission du dossier"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permissions du dossier"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
-msgstr ""
+msgstr "Tous les dossiers"
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
-msgstr ""
+msgstr "Chemin logique"
 
 #: models/foldermodels.py:370
 #, python-brace-format
 msgid "User: {user}"
-msgstr ""
+msgstr "Utilisateur : {user}"
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
-msgstr ""
+msgstr "Groupe : {group}"
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
-msgstr ""
+msgstr "Tout le monde"
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
-msgstr ""
+msgstr "Modifier"
 
 #: models/foldermodels.py:388
 msgid "Read"
-msgstr ""
+msgstr "Lire"
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
-msgstr ""
+msgstr "Ajouter un sous-dossier"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "date de prise de vue"
 
 #: models/imagemodels.py:25
 msgid "author"
@@ -542,19 +535,20 @@
 #: templates/admin/filer/folder/directory_listing.html:37
 #: templates/admin/filer/folder/directory_listing.html:104
 msgid "root"
 msgstr "racine"
 
 #: settings.py:273
 msgid "Show table view"
-msgstr ""
+msgstr "Voir la vue en liste"
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
-msgstr ""
+msgstr "Voir la vue avec des miniatures"
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Exécuter l'action sélectionnée"
 
 #: templates/admin/filer/actions.html:5
 msgid "Go"
@@ -612,34 +606,27 @@
 msgstr "Duplicatas"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Supprimer les fichiers et/ou dossiers sélectionnés devrait provoquer la "
-"suppression des objets liés, mais votre compte n'a pas les permissions "
-"nécessaires pour supprimer les types d'objets suivants :"
+msgstr "Supprimer les fichiers et/ou dossiers sélectionnés devrait provoquer la suppression des objets liés, mais votre compte n'a pas les permissions nécessaires pour supprimer les types d'objets suivants :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Supprimer les fichiers et/ou dossiers provoquera la suppression des objets "
-"liés protégés suivants :"
+msgstr "Supprimer les fichiers et/ou dossiers provoquera la suppression des objets liés protégés suivants :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? "
-"Tous les objets suivants et leurs éléments liés seront supprimés :"
+msgstr "Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? Tous les objets suivants et leurs éléments liés seront supprimés :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Non, faites-moi revenir"
 
@@ -680,19 +667,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icône du dossier"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Votre compte n'a pas les permissions nécessaires pour copier tous les "
-"fichiers et/ou dossiers sélectionnés."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Votre compte n'a pas les permissions nécessaires pour copier tous les fichiers et/ou dossiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -708,17 +693,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Aucun fichier ou dossier n'est disponible à copier."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Les fichiers et/ou dossiers suivants seront copiés vers un dossier de "
-"destination (en conservant leur arborescence) :"
+msgstr "Les fichiers et/ou dossiers suivants seront copiés vers un dossier de destination (en conservant leur arborescence) :"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Dossier de destination :"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -730,98 +713,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Il est impossible de copier des fichiers dans le même dossier"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Votre compte na pas les permissions nécessaires pour redimensionner toutes "
-"les images sélectionnées."
+msgstr "Votre compte na pas les permissions nécessaires pour redimensionner toutes les images sélectionnées."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Il n'y a aucune image disponible à redimensionner."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Les images suivantes seront redimensionnées :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Choisissez une option de miniature existante ou entrez des paramètres de "
-"redimensionnement :"
+msgstr "Choisissez une option de miniature existante ou entrez des paramètres de redimensionnement :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Choisissez des paramètres de redimensionnement :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Avertissement : Les images seront redimensionnées en place et les originales "
-"seront perdues. Faites-en éventuellement une copie préalable afin de les "
-"conserver."
+msgstr "Avertissement : Les images seront redimensionnées en place et les originales seront perdues. Faites-en éventuellement une copie préalable afin de les conserver."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionner"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Votre compte n'a pas les permissions nécessaires pour déplacer tous les "
-"fichiers et/ou dossiers sélectionnés."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Votre compte n'a pas les permissions nécessaires pour déplacer tous les fichiers et/ou dossiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Il n'y a pas de fichiers et/ou dossiers disponibles à déplacer."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Les fichiers et/ou dossiers suivants seront déplacés vers un dossier de "
-"destination (en conservant leur arborescence) :"
+msgstr "Les fichiers et/ou dossiers suivants seront déplacés vers un dossier de destination (en conservant leur arborescence) :"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Déplacer"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Il est impossible de déplacer des fichiers dans le même dossier"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Votre compte n'a pas les permissions nécessaires pour renommer tous les "
-"fichiers sélectionnés."
+msgstr "Votre compte n'a pas les permissions nécessaires pour renommer tous les fichiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Il n'y a pas de fichiers disponibles à renommer."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Les fichiers suivants seront renommés (ils resteront dans leurs dossiers et "
-"conserveront leur nom de fichier d'origine ; seul le nom affiché sera "
-"changé) :"
+msgstr "Les fichiers suivants seront renommés (ils resteront dans leurs dossiers et conserveront leur nom de fichier d'origine ; seul le nom affiché sera changé) :"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Renommer"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -970,31 +937,32 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "activé"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "url canonique '%(item_label)s' "
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Télécharger '%(item_label)s' "
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Supprimer le fichier"
 
 #: templates/admin/filer/folder/directory_table_list.html:160
 #: templates/admin/filer/folder/directory_thumbnail_list.html:138
 msgid "Drop files here or use the \"Upload Files\" button"
-msgstr ""
-"Déposez des fichiers ici ou utilisez le bouton « Téléverser des fichiers »"
+msgstr "Déposez des fichiers ici ou utilisez le bouton « Téléverser des fichiers »"
 
 #: templates/admin/filer/folder/directory_table_list.html:175
 #: templates/admin/filer/folder/directory_thumbnail_list.html:153
 msgid "Drop your file to upload into:"
 msgstr "Déposez votre fichier à téléverser dans :"
 
 #: templates/admin/filer/folder/directory_table_list.html:185
@@ -1037,20 +1005,22 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Sélectionner les %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
-msgstr ""
+msgstr "Tout sélectionner"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
-msgstr ""
+msgstr "Fichiers"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Ajouter un nouveau"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
@@ -1066,19 +1036,19 @@
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr "Sauvegarder"
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
-msgstr ""
+msgstr "Votre navigateur ne supporte pas l'audio."
 
 #: templates/admin/filer/templatetags/file_icon.html:14
 msgid "Your browser does not support video."
-msgstr ""
+msgstr "Votre navigateur ne supporte pas la vidéo."
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:9
 msgid "Clipboard"
 msgstr "Presse-papiers"
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:21
 msgid "Paste all items here"
@@ -1098,25 +1068,26 @@
 
 #: templates/admin/filer/tools/clipboard/clipboard_item_rows.html:16
 msgid "upload failed"
 msgstr "transfert échoué"
 
 #: templates/admin/filer/tools/detail_info.html:11
 msgid "Download"
-msgstr ""
+msgstr "Télécharger"
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
-msgstr ""
+msgstr "Agrandir"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
-msgstr ""
+msgstr "Le fichier est manquant"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Type"
 
 #: templates/admin/filer/tools/detail_info.html:37
 msgid "File-size"
@@ -1162,38 +1133,39 @@
 msgstr "Recherche"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Sélectionner un fichier"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
-msgstr ""
+msgstr "Choisissez un dossier"
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
-msgstr ""
+msgstr "Fichier \"{file_name}\" : Hébergement refusé par la politique de sécurité du site"
 
 #: validation.py:22
 #, python-brace-format
 msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
-msgstr ""
+msgstr "Fichier \"{file_name}\" : hébergement de {file_type} refusé par la politique de sécurité du site"
 
 #: validation.py:33
 #, python-brace-format
 msgid "File \"{file_name}\": HTML upload denied by site security policy"
-msgstr ""
+msgstr "Fichier \"{file_name}\" : hébergement HTML refusé par la politique de sécurité du site"
 
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
-msgstr ""
+msgstr "Fichier \"{file_name}\" : Rejeté à cause d'une potentielle vulnérabilité de cross-site scripting"
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Galician (http://www.transifex.com/divio/django-filer/"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Pablo, 2015\n"
+"Language-Team: Galician (http://app.transifex.com/divio/django-filer/"
 "language/gl/)\n"
-"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s seleccionados"
 msgstr[1] "Os %(total_count)s seleccionados"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Pablo, 2015
 # Pablo, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Galician (http://www.transifex.com/divio/django-filer/"
-"language/gl/)\n"
-"Language: gl\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Pablo, 2015\n"
+"Language-Team: Galician (http://app.transifex.com/divio/django-filer/language/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avanzado"
 
 #: admin/fileadmin.py:160
@@ -441,18 +443,17 @@
 msgstr "permiso da carpeta"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permisos da carpeta"
 
 #: models/foldermodels.py:359
-#, fuzzy
 #| msgid "Folders"
 msgid "All Folders"
-msgstr "Carpetas"
+msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
 #: models/foldermodels.py:370
 #, python-brace-format
@@ -461,32 +462,30 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
-#, fuzzy
 #| msgid "everybody"
 msgid "Everybody"
-msgstr "todos"
+msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
-#, fuzzy
 #| msgid "can add children"
 msgid "Add children"
-msgstr "pode engadir fillos"
+msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data"
 
 #: models/imagemodels.py:25
 msgid "author"
@@ -533,18 +532,17 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#, fuzzy
 #| msgid "thumbnail option"
 msgid "Show thumbnail view"
-msgstr "opción da miniatura"
+msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Go"
@@ -663,16 +661,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -739,16 +737,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -931,19 +929,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -997,22 +997,22 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#, fuzzy
-#| msgid "files"
+#| msgid "Filer"
 msgid "Files"
-msgstr "arquivos"
+msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
@@ -1068,14 +1068,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1123,18 +1124,17 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#, fuzzy
-#| msgid "Folder"
+#| msgid "Choose File"
 msgid "Choose Folder"
-msgstr "Carpeta"
+msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
 
 #: validation.py:22
@@ -1150,14 +1150,44 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
 "Language-Team: Hebrew (http://app.transifex.com/divio/django-filer/language/"
 "he/)\n"
-"Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "אחד נבחר"
 msgstr[1] "כל ה-%(total_count)s  נבחרו"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/he/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Hebrew (http://app.transifex.com/divio/django-filer/language/"
-"he/)\n"
-"Language: he\n"
+"Language-Team: Hebrew (http://app.transifex.com/divio/django-filer/language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
-"1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
+"Language: he\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % 1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "מתקדם"
 
 #: admin/fileadmin.py:160
@@ -442,14 +443,15 @@
 msgstr "הרשאת תיקיה"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "הרשאות תיקיה"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -460,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "תאריך צילום"
 
@@ -528,14 +532,15 @@
 msgstr "שורש"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "הרץ את הפעולה הבחורה"
 
@@ -595,33 +600,27 @@
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק אובייקטים מקושרים, אך "
-"לחשבונך אין הרשאות למחוק אובייקטים מהסוגים הבאים:"
+msgstr "עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק אובייקטים מקושרים, אך לחשבונך אין הרשאות למחוק אובייקטים מהסוגים הבאים:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק את האובייקטים המוגנים "
-"הבאים:"
+msgstr "עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק את האובייקטים המוגנים הבאים:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"האם את/ה בטוח/ה שברצונך למחוק את הקבצים ו/או התיקיות הבחורים? כל הפריטים "
-"המקושרים יימחקו:"
+msgstr "האם את/ה בטוח/ה שברצונך למחוק את הקבצים ו/או התיקיות הבחורים? כל הפריטים המקושרים יימחקו:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -662,16 +661,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "צלמית תיקייה"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr "לחשבונך אין רשות להעתיק את כל הקבצים ו/או התיקיות הבחורים."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -688,16 +687,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "אין קבצים ו/או תיקיות זמינים להעתקה."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"הקבצים ו/או התיקיות הבאים יועתקו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
+msgstr "הקבצים ו/או התיקיות הבאים יועתקו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "תיקיית יעד:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -731,38 +729,35 @@
 msgid "Choose resize parameters:"
 msgstr "בחר פרמטרי שינוי גודל:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"הזהרה: התמונות ישונה גודלן במקום והמקוריות יאבדו. אולי ראשית עשה/י העתק שלהם "
-"כדי לשמור על המקויות."
+msgstr "הזהרה: התמונות ישונה גודלן במקום והמקוריות יאבדו. אולי ראשית עשה/י העתק שלהם כדי לשמור על המקויות."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "שנה גודל"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr "לחשבונך אין רשות להעביר את כל הקבצים ו/או התיקיות הבחורים."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "אין קבצים ו/או תיקיות זמינים להעברה."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"הקבצים ו/או התיקיות הבאים יועברו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
+msgstr "הקבצים ו/או התיקיות הבאים יועברו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "העבר"
 
@@ -779,17 +774,15 @@
 msgid "There are no files available to rename."
 msgstr "אין קבצים זמינים לשינוי שמם."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"הקבצים הבאים ישונו שמותיהם (הם יישארו בתיקיות הנוכחיות שלהם ושמם המקורי "
-"יישאר - רק שמות התצוגה שלהם ישונו):"
+msgstr "הקבצים הבאים ישונו שמותיהם (הם יישארו בתיקיות הנוכחיות שלהם ושמם המקורי יישאר - רק שמות התצוגה שלהם ישונו):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "שנה שם"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -940,19 +933,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "מאופשר"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1006,18 +1001,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "הוסף חדש"
@@ -1077,14 +1074,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1132,14 +1130,15 @@
 msgstr "חיפוש"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Aleks Acimovic, 2022\n"
 "Language-Team: Croatian (http://app.transifex.com/divio/django-filer/"
 "language/hr/)\n"
-"Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s odabrana"
 msgstr[1] "%(total_count)s odabrano"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Aleks Acimovic, 2022
 # Damir <damir.arbula@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Aleks Acimovic, 2022\n"
-"Language-Team: Croatian (http://app.transifex.com/divio/django-filer/"
-"language/hr/)\n"
-"Language: hr\n"
+"Language-Team: Croatian (http://app.transifex.com/divio/django-filer/language/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: hr\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Napredno"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Stavke moraju biti odabrane kako bi se obavila akcija. Nijedna stavka nije "
-"promijenjena."
+msgstr "Stavke moraju biti odabrane kako bi se obavila akcija. Nijedna stavka nije promijenjena."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s odabrana"
 msgstr[1] "%(total_count)s odabrano"
@@ -127,17 +126,15 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Uspješno premješteno %(count)d datoteka i/ili direktorija u direktorij "
-"'%(destination)s'."
+msgstr "Uspješno premješteno %(count)d datoteka i/ili direktorija u direktorij '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Premjesti datoteke i/ili direktorije"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -154,17 +151,15 @@
 msgstr "Preimenuj datoteke"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Uspješno kopirano %(count)d datoteka i/ili direktorija u direktorij "
-"'%(destination)s'."
+msgstr "Uspješno kopirano %(count)d datoteka i/ili direktorija u direktorij '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopiraj datoteke i/ili direktorije"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -188,16 +183,15 @@
 msgstr "Sufiks koji će biti dodan imenima kopiranih datoteka."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Sufiks treba biti jednostavan i upisan malim slovima poput \"%(valid)s\"."
+msgstr "Sufiks treba biti jednostavan i upisan malim slovima poput \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nepoznata vrijednost formata ključa za preimenovanje \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -223,16 +217,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "povećaj veličinu"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Opcija sličica ili parametri za promjenu veličine moraju biti izabrani."
+msgstr "Opcija sličica ili parametri za promjenu veličine moraju biti izabrani."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Parametri za promjenu veličine moraju biti izabrani."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -451,14 +444,15 @@
 msgstr "ovlast direktorija"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "ovlasti direktorija"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -469,26 +463,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum nastanka"
 
@@ -537,14 +533,15 @@
 msgstr "korijenski"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Pokreni odabranu akciju"
 
@@ -604,33 +601,27 @@
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Brisanje odabranih objekata bi rezultiralo brisanjem povezanih objekata, ali "
-"Vaš korisnički račun nema ovlasti za brisanje slijedećih tipova objekata:"
+msgstr "Brisanje odabranih objekata bi rezultiralo brisanjem povezanih objekata, ali Vaš korisnički račun nema ovlasti za brisanje slijedećih tipova objekata:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Brisanje odabranih datoteka i/ili direktorija bi zahtijevalo brisanje "
-"slijedećih zaštičenih povezanih objekata:"
+msgstr "Brisanje odabranih datoteka i/ili direktorija bi zahtijevalo brisanje slijedećih zaštičenih povezanih objekata:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Jeste li sigurni kako želite obrisati odabrane datoteke i/ili direktorije? "
-"Svi navedeni objekti i s njima povezane stavke biti će obrisani:"
+msgstr "Jeste li sigurni kako želite obrisati odabrane datoteke i/ili direktorije? Svi navedeni objekti i s njima povezane stavke biti će obrisani:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -671,19 +662,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona direktorija"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Vaš korisnički račun nema ovlasti za kopiranje odabranih datoteka i/ili "
-"direktorija."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Vaš korisnički račun nema ovlasti za kopiranje odabranih datoteka i/ili direktorija."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -699,17 +688,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nema dostupnih datoteka i/ili direktorija za kopiranje."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Slijedeće datoteke i/ili direktoriji biti će kopirani u odredišni direktorij "
-"(zadržavajući postojeću strukturu):"
+msgstr "Slijedeće datoteke i/ili direktoriji biti će kopirani u odredišni direktorij (zadržavajući postojeću strukturu):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Odredišni direktorij"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -721,95 +708,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Vaš korisnički račun nema ovlasti za promjenu veličina odabranih slika."
+msgstr "Vaš korisnički račun nema ovlasti za promjenu veličina odabranih slika."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Nema dostupnih slika kojima bi se promijenila veličina."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Slijedećim slikama biti će promijenjena veličina:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Izaberite postojeću opciju sličica ili unesite parametre za promjenu "
-"veličine:"
+msgstr "Izaberite postojeću opciju sličica ili unesite parametre za promjenu veličine:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Odaberite parametre za promjenu veličine:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Pažnja: Slikama će biti promijenjena veličina, a originali će biti prepisani "
-"sa slikama s novom veličinom. Preporuča se prvo kopirati originalne slike "
-"prije promjene veličine."
+msgstr "Pažnja: Slikama će biti promijenjena veličina, a originali će biti prepisani sa slikama s novom veličinom. Preporuča se prvo kopirati originalne slike prije promjene veličine."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Promjeni veličinu"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Vaš korisnički račun nema ovlasti za premještaj svih odabranih datoteka i/"
-"ili direktorija."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Vaš korisnički račun nema ovlasti za premještaj svih odabranih datoteka i/ili direktorija."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nema dostupnih datoteka i/ili direktorija za premještaj."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Slijedeće datoteke i/ili direktoriji biti će premješteni u odredišni "
-"direktorij (zadržavajući postojeću strukturu):"
+msgstr "Slijedeće datoteke i/ili direktoriji biti će premješteni u odredišni direktorij (zadržavajući postojeću strukturu):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Premjesti"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Vaš korisnički račun nema ovlasti za preimenovanje svih odabranih datoteka."
+msgstr "Vaš korisnički račun nema ovlasti za preimenovanje svih odabranih datoteka."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Nema dostupnih datoteka i/ili direktorija za preimenovanje."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Slijedeće datoteke če biti preimenovane (ostati će u svojim direktorijima i "
-"zadržati ime datoteke, samo će prikazano ime biti promijenjeno):"
+msgstr "Slijedeće datoteke če biti preimenovane (ostati će u svojim direktorijima i zadržati ime datoteke, samo će prikazano ime biti promijenjeno):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Preimenuj"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -958,19 +932,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "omogućeno"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1024,18 +1000,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Dodaj novi"
@@ -1094,14 +1072,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1149,14 +1128,15 @@
 msgstr "Pregled"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2016-2017\n"
 "Language-Team: Hungarian (http://app.transifex.com/divio/django-filer/"
 "language/hu/)\n"
-"Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s fájl"
 msgstr[1] "%(counter)s fájl"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Istvan Farkas <istvan.farkas@gmail.com>, 2016-2017
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2016-2017\n"
-"Language-Team: Hungarian (http://app.transifex.com/divio/django-filer/"
-"language/hu/)\n"
-"Language: hu\n"
+"Language-Team: Hungarian (http://app.transifex.com/divio/django-filer/language/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Haladó"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "egyedi URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Az akciók végrehajtásához egy vagy több elemet ki kell választani. Egyetlen "
-"elem sem változott."
+msgstr "Az akciók végrehajtásához egy vagy több elemet ki kell választani. Egyetlen elem sem változott."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s kiválasztva"
 msgstr[1] "Mind (%(total_count)s) kiválasztva"
@@ -124,17 +124,15 @@
 msgstr "A kiválasztott helyen már létezik %s nevű mappa"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fájl és/vagy mappa sikeresen átmozgatva ebbe a mappába: "
-"%(destination)s"
+msgstr "%(count)d fájl és/vagy mappa sikeresen átmozgatva ebbe a mappába: %(destination)s"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Fájlok és/vagy mappák mozgatása"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -151,17 +149,15 @@
 msgstr "Fájlok átnevezése"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d fájl és/vagy mappa sikeresen átmásolva ebbe a mappába: "
-"%(destination)s"
+msgstr "%(count)d fájl és/vagy mappa sikeresen átmásolva ebbe a mappába: %(destination)s"
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Fájlok és/vagy mappák másolása"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -185,17 +181,15 @@
 msgstr "Utótag, amely a másolt fájlok nevéhez lesz hozzáadva."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Az utótag lehetőleg egyszerű, kisbetűs fájlnév részlet legyen, például "
-"\"%(valid)s\"."
+msgstr "Az utótag lehetőleg egyszerű, kisbetűs fájlnév részlet legyen, például \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ismeretlen átnevezés formázási szó: \"%(key)s\" "
 
 #: admin/forms.py:54
@@ -221,16 +215,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "felméretezés"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Előnézeti kép beállítást vagy átméretezési paramétert kötelező kiválasztani."
+msgstr "Előnézeti kép beállítást vagy átméretezési paramétert kötelező kiválasztani."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Átméretezési paramétert kötelező kiválasztani."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -373,17 +366,15 @@
 msgid "Permissions disabled"
 msgstr "Jogosultságok kikapcsolva"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Jogosultságok ellenőrzésének kikapcsolása ennél a fájlnál. Ezt a fájlt bárki "
-"letöltheti."
+msgstr "Jogosultságok ellenőrzésének kikapcsolása ennél a fájlnál. Ezt a fájlt bárki letöltheti."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -451,14 +442,15 @@
 msgstr "mappa jogosultság"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "mappa jogosultságok"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -469,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "fotózás dátuma"
 
@@ -537,14 +531,15 @@
 msgstr "gyökér"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Kiválasztott akció végrehajtása"
 
@@ -604,34 +599,27 @@
 msgstr "Duplikátumok"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"A kiválasztott fájlok és mappák törlése csatlakozó elemek törlésével is "
-"járna, viszont a jelenlegi fiók nem rendelkezik a megfelelő jogosultságokkal "
-"a következő objektum típusok törléséhez:"
+msgstr "A kiválasztott fájlok és mappák törlése csatlakozó elemek törlésével is járna, viszont a jelenlegi fiók nem rendelkezik a megfelelő jogosultságokkal a következő objektum típusok törléséhez:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"A kiválasztott fájlok és mappák törlése azzal járna, hogy a következő "
-"kapcsolt elemek is törlődnek:"
+msgstr "A kiválasztott fájlok és mappák törlése azzal járna, hogy a következő kapcsolt elemek is törlődnek:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Biztosan törli a kiválasztott fájlokat és/vagy mappákat? A következő "
-"objektumok, és a hozzájuk kapcsolt elemek is törlődni fognak:"
+msgstr "Biztosan törli a kiválasztott fájlokat és/vagy mappákat? A következő objektumok, és a hozzájuk kapcsolt elemek is törlődni fognak:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Nem, mégsem"
 
@@ -672,18 +660,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappa Ikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa másolásához."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa másolásához."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -699,17 +686,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nincsenek másolható fájlok és/vagy könyvtárak"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"A következő fájlok és/vagy mappák lesznek a célkönyvtárba másolva (megtartva "
-"a szerkezetüket):"
+msgstr "A következő fájlok és/vagy mappák lesznek a célkönyvtárba másolva (megtartva a szerkezetüket):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cél mappa:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -733,52 +718,45 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "A következő képek lesznek átméretezve:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Válasszon ki egy meglévő előnézeti kép beállítást, vagy írja be az "
-"átméretezési paramétereket:"
+msgstr "Válasszon ki egy meglévő előnézeti kép beállítást, vagy írja be az átméretezési paramétereket:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Válasszon átméretezési paramétereket:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Figyelem: a képek helyben lesznek átméretezve, felülírva az eredetieket. Ha "
-"meg szeretné őrizni az eredeti képeket, előbb másolja át őket."
+msgstr "Figyelem: a képek helyben lesznek átméretezve, felülírva az eredetieket. Ha meg szeretné őrizni az eredeti képeket, előbb másolja át őket."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Átméretezés"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa mozgatásához."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa mozgatásához."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nincsenek mozgatható fájlok és/vagy mappák."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"A következő fájlok és/vagy mappák lesznek átmozgatva a cél mappába "
-"(megtartva a szerkezetüket):"
+msgstr "A következő fájlok és/vagy mappák lesznek átmozgatva a cél mappába (megtartva a szerkezetüket):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Mozgatás"
 
@@ -795,17 +773,15 @@
 msgid "There are no files available to rename."
 msgstr "Nincsenek átnevezhető fájlok."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"A következő fájlok lesznek átnevezve (a mappában maradnak, és az eredeti "
-"fájlnév megmarad, csak a megjelenített név változik):"
+msgstr "A következő fájlok lesznek átnevezve (a mappában maradnak, és az eredeti fájlnév megmarad, csak a megjelenített név változik):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Átnevezés"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -952,31 +928,32 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "engedélyezve"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "'%(item_label)s' letöltése"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Fájl eltávolítása"
 
 #: templates/admin/filer/folder/directory_table_list.html:160
 #: templates/admin/filer/folder/directory_thumbnail_list.html:138
 msgid "Drop files here or use the \"Upload Files\" button"
-msgstr ""
-"Egérrel dobjon ide fájlokat, vagy használja a \"Fájlok feltöltése\" gombot"
+msgstr "Egérrel dobjon ide fájlokat, vagy használja a \"Fájlok feltöltése\" gombot"
 
 #: templates/admin/filer/folder/directory_table_list.html:175
 #: templates/admin/filer/folder/directory_thumbnail_list.html:153
 msgid "Drop your file to upload into:"
 msgstr "Egérre dobja ide a fájl, hogy feltöltse ebbe a mappába:"
 
 #: templates/admin/filer/folder/directory_table_list.html:185
@@ -1019,18 +996,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Összes (%(total_count)s) kiválasztása"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Új"
@@ -1088,14 +1067,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Típus"
 
@@ -1143,14 +1123,15 @@
 msgstr "Keresés"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Fájl kiválasztása"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: yakky <i.spalletti@nephila.it>, 2013,2015-2018\n"
 "Language-Team: Italian (http://app.transifex.com/divio/django-filer/language/"
 "it/)\n"
-"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s file"
 msgstr[1] "%(counter)s file"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # yakky <i.spalletti@nephila.it>, 2012
 # yakky <i.spalletti@nephila.it>, 2013,2015-2018
 # yakky <i.spalletti@nephila.it>, 2012
 # yakky <i.spalletti@nephila.it>, 2012-2013,2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: yakky <i.spalletti@nephila.it>, 2013,2015-2018\n"
-"Language-Team: Italian (http://app.transifex.com/divio/django-filer/language/"
-"it/)\n"
-"Language: it\n"
+"Language-Team: Italian (http://app.transifex.com/divio/django-filer/language/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
-"1 : 2;\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avanzato"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL standard"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Gli elementi devono essere selezionati in modo da eseguire azioni su di "
-"essi. Nessun elemento è stato modificato."
+msgstr "Gli elementi devono essere selezionati in modo da eseguire azioni su di essi. Nessun elemento è stato modificato."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] " %(total_count)s elemento selezionato"
 msgstr[1] "Tutti e %(total_count)s selezionati"
@@ -129,17 +128,15 @@
 msgstr "Esistono altre cartelle chiamate %s nella destinazione selezionata"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d file e/o le cartelle spostati con successo nella cartella "
-"'%(destination)s'."
+msgstr "%(count)d file e/o le cartelle spostati con successo nella cartella '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Sposta i file e/o le cartelle"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -156,17 +153,15 @@
 msgstr "Rinomina file"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d file e/o cartelle copiati con successo nella cartella "
-"'%(destination)s '."
+msgstr "%(count)d file e/o cartelle copiati con successo nella cartella '%(destination)s '."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copia i file e/o le cartelle"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -190,17 +185,15 @@
 msgstr "Suffisso che sarà aggiunto al nome dei file copiati."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Il suffisso deve essere una sezione del nome del file valida, semplice e "
-"minuscola, come \"%(valid)s\"."
+msgstr "Il suffisso deve essere una sezione del nome del file valida, semplice e minuscola, come \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Valore del formato di rinomina non valido \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -226,17 +219,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "ingrandisci"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Devi selezionare l'opzione anteprima immagine o i parametri di "
-"ridimensionamento."
+msgstr "Devi selezionare l'opzione anteprima immagine o i parametri di ridimensionamento."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Seleziona le opzioni di ridimensionamento."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -379,17 +370,15 @@
 msgid "Permissions disabled"
 msgstr "Permessi disabilitati"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Disabilita ogni controllo dei permessi per questo file. Il file sarà "
-"accessibile da chiunque"
+msgstr "Disabilita ogni controllo dei permessi per questo file. Il file sarà accessibile da chiunque"
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -457,14 +446,15 @@
 msgstr "permessi cartella"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permessi cartella"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -475,26 +465,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data di creazione"
 
@@ -543,14 +535,15 @@
 msgstr "cartella principale"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Esegui l'azione selezionata"
 
@@ -610,34 +603,27 @@
 msgstr "Duplicati"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Cancellare i file selezionati e/o cartelle comporta l'eliminazione degli "
-"oggetti correlati, ma il tuo account non dispone dell'autorizzazione per "
-"eliminare i seguenti tipi di oggetti:"
+msgstr "Cancellare i file selezionati e/o cartelle comporta l'eliminazione degli oggetti correlati, ma il tuo account non dispone dell'autorizzazione per eliminare i seguenti tipi di oggetti:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Cancellare i file selezionati e/o cartelle richiede eliminazione dei "
-"seguenti oggetti protetti correlati:"
+msgstr "Cancellare i file selezionati e/o cartelle richiede eliminazione dei seguenti oggetti protetti correlati:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Sei sicuro di voler cancellare i file selezionati e/o le cartelle? Tutti gli "
-"oggetti seguenti e quelli correlati verranno cancellati:"
+msgstr "Sei sicuro di voler cancellare i file selezionati e/o le cartelle? Tutti gli oggetti seguenti e quelli correlati verranno cancellati:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "No, torna indietro"
 
@@ -678,19 +664,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icona della cartella"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Il tuo account non dispone delle autorizzazioni per copiare tutti i file e/o "
-"cartelle selezionati."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Il tuo account non dispone delle autorizzazioni per copiare tutti i file e/o cartelle selezionati."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -706,17 +690,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Non ci sono file e/o le cartelle disponibili per la copia."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"I seguenti file e/o cartelle verranno copiati in una cartella di "
-"destinazione (mantenendo la loro struttura ad albero):"
+msgstr "I seguenti file e/o cartelle verranno copiati in una cartella di destinazione (mantenendo la loro struttura ad albero):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cartella di destinazione:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -728,97 +710,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Non è autorizzato a copiare file nella stessa cartella"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Il tuo account non dispone delle autorizzazioni per ridimensionare tutte le "
-"immagini selezionate."
+msgstr "Il tuo account non dispone delle autorizzazioni per ridimensionare tutte le immagini selezionate."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Non ci sono immagini disponibili da ridimensionare."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Le seguenti immagini verranno ridimensionate:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Scegli un'opzione miniatura esistente o immetti i parametri di "
-"ridimensionamento:"
+msgstr "Scegli un'opzione miniatura esistente o immetti i parametri di ridimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Scegli i parametri di ridimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Attenzione: Le immagini verranno ridimensionate ora e le immagini originali "
-"andranno perse. Forse è meglio fare una copia per mantenere i file originali."
+msgstr "Attenzione: Le immagini verranno ridimensionate ora e le immagini originali andranno perse. Forse è meglio fare una copia per mantenere i file originali."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Ridimensiona"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Il tuo account non dispone delle autorizzazioni per spostare tutti i file e/"
-"o cartelle selezionati."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Il tuo account non dispone delle autorizzazioni per spostare tutti i file e/o cartelle selezionati."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Non ci sono file e/o cartelle a disponibili per lo spostamento."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"I seguenti file e/o cartelle verranno spostati in una cartella di "
-"destinazione (mantenendo la loro struttura ad albero):"
+msgstr "I seguenti file e/o cartelle verranno spostati in una cartella di destinazione (mantenendo la loro struttura ad albero):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Sposta"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Non è autorizzato a spostare file nella stessa cartella"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Il tuo account non dispone delle autorizzazioni per rinominare tutti i file "
-"selezionati."
+msgstr "Il tuo account non dispone delle autorizzazioni per rinominare tutti i file selezionati."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Non ci sono file disponibili da rinominare."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"I file seguenti saranno rinominati (rimarranno nelle rispettive cartelle e "
-"manterranno il nome del file originario, solo il nome visualizzato sarà "
-"modificato):"
+msgstr "I file seguenti saranno rinominati (rimarranno nelle rispettive cartelle e manterranno il nome del file originario, solo il nome visualizzato sarà modificato):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Rinomina"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -967,19 +934,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "abilitato"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "URL canonico '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Download '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Cancella file"
 
@@ -1033,18 +1002,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Seleziona tutti %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Aggiungi nuovo"
@@ -1103,14 +1074,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
@@ -1158,14 +1130,15 @@
 msgstr "Consultazione"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Seleziona file"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Japanese (http://www.transifex.com/divio/django-filer/"
-"language/ja/)\n"
-"Language: ja\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/divio/django-filer/language/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -438,14 +440,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +459,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +529,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +658,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +734,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -918,19 +924,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +992,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1052,14 +1062,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1118,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,14 +1144,44 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Japanese (Japan) (http://www.transifex.com/divio/django-filer/"
-"language/ja_JP/)\n"
-"Language: ja_JP\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Portuguese (http://app.transifex.com/divio/django-filer/language/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: pt\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -47,14 +49,16 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -438,14 +442,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +531,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +660,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +736,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -867,21 +875,25 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -918,19 +930,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +998,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1004,14 +1020,16 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1052,14 +1070,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1126,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,20 +1152,52 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
+#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Matas Dailyda <matas@dailyda.com>, 2015-2018\n"
 "Language-Team: Lithuanian (http://app.transifex.com/divio/django-filer/"
 "language/lt/)\n"
-"Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s byla"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Matas Dailyda <matas@dailyda.com>, 2015-2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Matas Dailyda <matas@dailyda.com>, 2015-2018\n"
-"Language-Team: Lithuanian (http://app.transifex.com/divio/django-filer/"
-"language/lt/)\n"
-"Language: lt\n"
+"Language-Team: Lithuanian (http://app.transifex.com/divio/django-filer/language/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
-"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
-"1 : n % 1 != 0 ? 2: 3);\n"
+"Language: lt\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Išplėstinės funkcijos"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "kanoninis URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Objektai turi būti pasirinkti, kad su jais būtų galima atlikti veiksmus. "
-"Jokie objektai nebuvo pakeisti."
+msgstr "Objektai turi būti pasirinkti, kad su jais būtų galima atlikti veiksmus. Jokie objektai nebuvo pakeisti."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "pasirinkta %(total_count)s"
 msgstr[1] "pasirinkta %(total_count)s"
@@ -121,25 +119,22 @@
 #: admin/folderadmin.py:811
 msgid "Delete selected files and/or folders"
 msgstr "Pašalinti pasirinktus failus ir / ar aplankus"
 
 #: admin/folderadmin.py:918
 #, python-format
 msgid "Folders with names %s already exist at the selected destination"
-msgstr ""
-"Aplankai su %s pavadinimais jau egzistuoja pasirinktoje paskirties vietoje."
+msgstr "Aplankai su %s pavadinimais jau egzistuoja pasirinktoje paskirties vietoje."
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Sėkmingai perkelti %(count)d failai ir / ar aplankai į aplanką "
-"'%(destination)s'."
+msgstr "Sėkmingai perkelti %(count)d failai ir / ar aplankai į aplanką '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Perkelti failus ir / ar aplankus"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -156,17 +151,15 @@
 msgstr "Pervardinti failus"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Sėkmingai nukopijuoti %(count)d failai ir / ar aplankai į aplanką "
-"'%(destination)s'."
+msgstr "Sėkmingai nukopijuoti %(count)d failai ir / ar aplankai į aplanką '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopijuoti failus ir / ar aplankus"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -190,17 +183,15 @@
 msgstr "Priesaga kuri bus pridėta prie nukopijuotų failų pavadinimų."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Priesaga turi būti paprasta ir taisyklinga bylos pavadinimo dalis pvz.  "
-"\"%(valid)s\"."
+msgstr "Priesaga turi būti paprasta ir taisyklinga bylos pavadinimo dalis pvz.  \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nežinomas pervardinimo formato reikšmės raktažodis \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -226,16 +217,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "išdidinti"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Miniatiūros nustatymas arba dydžio keitimo parametrai turi būti pasirinkti."
+msgstr "Miniatiūros nustatymas arba dydžio keitimo parametrai turi būti pasirinkti."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Turi būti pasirinkti dydžio keitimo parametrai."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -378,17 +368,15 @@
 msgid "Permissions disabled"
 msgstr "Leidimai išjungti"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Įšjungti bet kokius leidimų tikrinimus šiai bylai. Byla bus viešai "
-"pasiekiama bet kam."
+msgstr "Įšjungti bet kokius leidimų tikrinimus šiai bylai. Byla bus viešai pasiekiama bet kam."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -456,14 +444,15 @@
 msgstr "aplanko leidimas"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "aplanko leidimai"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -474,26 +463,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "paimta data"
 
@@ -542,14 +533,15 @@
 msgstr "pradinis"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Vykdyti pasirinktą veiksmą"
 
@@ -609,33 +601,27 @@
 msgstr "Dublikatai"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Pasirintų failų ir / ar aplankų šalinimas pašalintų susijusius objektus, "
-"tačiau jūsų vartotojas neturi leidimo šalinti šių objektų tipų:"
+msgstr "Pasirintų failų ir / ar aplankų šalinimas pašalintų susijusius objektus, tačiau jūsų vartotojas neturi leidimo šalinti šių objektų tipų:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Pasirinktų failų ir / ar aplankų šalinimas reikalautų pašalinti šiuos "
-"apsaugotus susijusius objektus:"
+msgstr "Pasirinktų failų ir / ar aplankų šalinimas reikalautų pašalinti šiuos apsaugotus susijusius objektus:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Ar tikrai norite pašalinti pasirinktus failus ir / ar aplankus? Visi susiję "
-"objektai bus pašalinti:"
+msgstr "Ar tikrai norite pašalinti pasirinktus failus ir / ar aplankus? Visi susiję objektai bus pašalinti:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ne, grįžti atgal"
 
@@ -676,19 +662,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Aplanko piktograma"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Jūsų vartotojas neturi leidimų kopijuoti visus pasirinktus failus ir / ar "
-"aplankus."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Jūsų vartotojas neturi leidimų kopijuoti visus pasirinktus failus ir / ar aplankus."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -704,17 +688,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nėra jokiu failų ir / ar aplankų kopijavimui."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Šie failai ir / ar aplankai bus nukopijuoti į paskirtą aplanką (išlaikant jų "
-"medžio struktūrą):"
+msgstr "Šie failai ir / ar aplankai bus nukopijuoti į paskirtą aplanką (išlaikant jų medžio struktūrą):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Paskyrimo aplankas:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -726,67 +708,57 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Neleidžiama kopijuoti bylų į tą patį aplanką"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Jūsų vartotojas neturi leidimų keisti dydžius visiems pasirinktiems "
-"paveikslėliams."
+msgstr "Jūsų vartotojas neturi leidimų keisti dydžius visiems pasirinktiems paveikslėliams."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Nėra jokiu paveikslėlių dydžio keitimui."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Šių paveikslėlių dydis bus pakeistas:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Pasirinkite esamą miniatiūros nustatymą, arba įveskite dydžio keitimo "
-"parametrus:"
+msgstr "Pasirinkite esamą miniatiūros nustatymą, arba įveskite dydžio keitimo parametrus:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Pasirinkite dydžio keitimo parametrus:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Įspėjimas: Paveikslėlių dydžiai bus pakeisti vietoje, ir originalas bus "
-"pašalintas. Patartina atsikopijuoti paveikslėlį, kad nedingtų originalas."
+msgstr "Įspėjimas: Paveikslėlių dydžiai bus pakeisti vietoje, ir originalas bus pašalintas. Patartina atsikopijuoti paveikslėlį, kad nedingtų originalas."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Pakeisti dydį"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Jūsų vartotojas neturi leidimų perkelti visus pasirinktus failus ir / ar "
-"aplankus."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Jūsų vartotojas neturi leidimų perkelti visus pasirinktus failus ir / ar aplankus."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nėra jokiu failų ir / ar aplankų perkelimui."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Šie failai ir / ar aplankai bus perkelti į paskirtą aplanką (išlaikant jų "
-"medžio struktūrą):"
+msgstr "Šie failai ir / ar aplankai bus perkelti į paskirtą aplanką (išlaikant jų medžio struktūrą):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Perkelti"
 
@@ -803,17 +775,15 @@
 msgid "There are no files available to rename."
 msgstr "Nėra jokių failų pervardinimui."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Šie failai bus pervardinti (jie liks savo aplankuose ir pasiliks savo "
-"originalius pavadinimus, pasikeis tik atvaizduojamas failo pavadinimas):"
+msgstr "Šie failai bus pervardinti (jie liks savo aplankuose ir pasiliks savo originalius pavadinimus, pasikeis tik atvaizduojamas failo pavadinimas):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Pervardinti"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -964,19 +934,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "įjungta"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanoninis url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Parsisiųsti '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Pašalinti bylą"
 
@@ -1030,18 +1002,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Pasirinkti visus %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Pridėti naują"
@@ -1101,14 +1075,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipas"
 
@@ -1156,14 +1131,15 @@
 msgstr "Informacijos ieškojimas"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Pasirinkti bylą"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Lithuanian (Lithuania) (http://www.transifex.com/divio/django-"
-"filer/language/lt_LT/)\n"
-"Language: lt_LT\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Chinese (http://app.transifex.com/divio/django-filer/language/zh/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"(n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Language: zh\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -48,16 +49,14 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -441,14 +440,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -459,26 +459,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -527,14 +529,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -655,16 +658,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -731,16 +734,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -870,25 +873,21 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -925,19 +924,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -991,18 +992,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1011,16 +1014,14 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1061,14 +1062,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1116,14 +1118,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1141,22 +1144,50 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
-#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
-#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
 "Language-Team: Norwegian Bokmål (http://app.transifex.com/divio/django-filer/"
 "language/nb/)\n"
-"Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s valgt"
 msgstr[1] "Alle %(total_count)s valgt"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
-"Language-Team: Norwegian Bokmål (http://app.transifex.com/divio/django-filer/"
-"language/nb/)\n"
-"Language: nb\n"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/divio/django-filer/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avansert"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Du må velge noen elementer for å utføre handlinger på dem. Ingen elementer "
-"er endret."
+msgstr "Du må velge noen elementer for å utføre handlinger på dem. Ingen elementer er endret."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s valgt"
 msgstr[1] "Alle %(total_count)s valgt"
@@ -124,16 +124,15 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Flyttet %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
+msgstr "Flyttet %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Flytt filer og/eller mapper"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -150,16 +149,15 @@
 msgstr "Endre navn på filer"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Kopierte %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
+msgstr "Kopierte %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopier filer og/eller mapper"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,17 +181,15 @@
 msgstr "Endelse som vil tilføyes filnavn på kopierte filer."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Endelse bør være en gyldig, enkel del av filnavnet med små bokstaver, som "
-"\"%(valid)s\"."
+msgstr "Endelse bør være en gyldig, enkel del av filnavnet med små bokstaver, som \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ugyldig nøkkel \"%(key)s\" for endring av navn."
 
 #: admin/forms.py:54
@@ -446,14 +442,15 @@
 msgstr "tillatelse for mappe"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "tillatelser for mappe"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -464,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "dato bildet ble tatt"
 
@@ -532,14 +531,15 @@
 msgstr "rot"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Utfør den valgte handlingen"
 
@@ -599,34 +599,27 @@
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Å slette de valgte filene og/eller mappene ville resultere i sletting av "
-"relaterte objekter, men din konto har ikke tillatelse til å slette objekter "
-"av følgende typer:"
+msgstr "Å slette de valgte filene og/eller mappene ville resultere i sletting av relaterte objekter, men din konto har ikke tillatelse til å slette objekter av følgende typer:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Å slette de valgte filene og/eller mappene ville kreve å slette følgende "
-"beskyttede relaterte objekter:"
+msgstr "Å slette de valgte filene og/eller mappene ville kreve å slette følgende beskyttede relaterte objekter:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Er du sikker på at du vil slette de valgte filene og/eller mappene? Alle de "
-"følgende objektene og deres relaterte elementer vil bli slettet:"
+msgstr "Er du sikker på at du vil slette de valgte filene og/eller mappene? Alle de følgende objektene og deres relaterte elementer vil bli slettet:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -667,19 +660,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappeikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Din konto har ikke tillatelse til å kopiere alle de valgte filene og/eller "
-"mappene."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Din konto har ikke tillatelse til å kopiere alle de valgte filene og/eller mappene."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -695,17 +686,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Det er ingen filer og/eller mapper å kopiere."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"De følgende filene og/eller mappene vil bli kopiert til en målmappe "
-"(mappestruktur vil beholdes):"
+msgstr "De følgende filene og/eller mappene vil bli kopiert til en målmappe (mappestruktur vil beholdes):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Målmappe:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -717,94 +706,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Din konto har ikke tillatelse til å endre størrelse på alle valgte bilder."
+msgstr "Din konto har ikke tillatelse til å endre størrelse på alle valgte bilder."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Det er ingen bilder å endre størrelse på."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "De følgende bildene vil få endret størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Velg et eksisterende miniatyrbildevalg eller skriv inn parametre for endring "
-"av størrelse:"
+msgstr "Velg et eksisterende miniatyrbildevalg eller skriv inn parametre for endring av størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Velg parametre for endring av størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Advarsel: Bilder vil få sin størrelse endret, og originalene vil gå tapt. "
-"Det kan være ønskelig å først gjøre en kopi for å beholde originalene."
+msgstr "Advarsel: Bilder vil få sin størrelse endret, og originalene vil gå tapt. Det kan være ønskelig å først gjøre en kopi for å beholde originalene."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Endre størrelse"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Din konto har ikke tillatelse til å flytte alle de valgte filene og/eller "
-"mappene."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Din konto har ikke tillatelse til å flytte alle de valgte filene og/eller mappene."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Det er ingen filer og/eller mapper å flytte."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"De følgende filene og/eller mappene vil bli flyttet til en målmappe "
-"(mappestruktur vil beholdes):"
+msgstr "De følgende filene og/eller mappene vil bli flyttet til en målmappe (mappestruktur vil beholdes):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Flytt"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Din konto har ikke tillatelse til å endre navn på alle de valgte filene."
+msgstr "Din konto har ikke tillatelse til å endre navn på alle de valgte filene."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Det er ingen filer å endre navn på."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"De følgende filene vil få endret navn (de vil forbli på samme sted og "
-"beholde originalt filnavn, bare visningsnavn vil endres):"
+msgstr "De følgende filene vil få endret navn (de vil forbli på samme sted og beholde originalt filnavn, bare visningsnavn vil endres):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Endre navn"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -951,19 +928,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivert"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1017,18 +996,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Legg til ny"
@@ -1086,14 +1067,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1141,14 +1123,15 @@
 msgstr "Slå opp"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Jeroen, 2018\n"
+"Last-Translator: Edwin Janssen, 2023\n"
 "Language-Team: Dutch (Netherlands) (http://app.transifex.com/divio/django-"
 "filer/language/nl_NL/)\n"
-"Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s bestand"
 msgstr[1] "%(counter)s bestanden"
 
@@ -29,34 +29,47 @@
 
 msgid "0 of %(cnt)s selected"
 msgstr "0 van %(cnt)s geselecteerd"
 
 msgid "Action"
 msgstr "Actie"
 
+msgid "Add children"
+msgstr "Toevoegen kinderen"
+
 msgid "Add new"
 msgstr "Toevoegen nieuwe"
 
 msgid "Adds a new Folder"
 msgstr "Voegt een nieuwe map toe"
 
 msgid "Advanced"
 msgstr "Geavanceerd"
 
+msgid "All Folders"
+msgstr "Alle Mappen"
+
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
 msgstr ""
 "Weet je zeker dat je de geselecteerde bestanden en/of folders wilt "
 "verwijderen? Alle volgende objecten en gerelateerde items zullen worden "
 "verwijderd: "
 
 msgid "Are you sure?"
 msgstr "Weet je het zeker?"
 
+msgid "Can't find folder to upload. Please refresh and try again"
+msgstr ""
+"Kan map niet vinden om te uploaden. Herlaad de pagina en probeer het opnieuw."
+
+msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgstr "Kan deze map niet gebruiken, rechten geweigerd. Kies een andere map."
+
 msgid "Cannot delete files and/or folders"
 msgstr "Bestanden en/of mappen kunnen niet worden verwijderd"
 
 msgid "Canonical url '%(item_label)s'"
 msgstr "Gebruikelijke url '%(item_label)s'"
 
 msgid "Change"
@@ -76,14 +89,17 @@
 
 msgid "Check it to limit the search to current folder"
 msgstr "Vink het aan om de zoekopdracht te beperken tot de huidige map"
 
 msgid "Choose File"
 msgstr "Kies bestand"
 
+msgid "Choose Folder"
+msgstr "Kies Map"
+
 msgid "Choose an existing thumbnail option or enter resize parameters:"
 msgstr "Kies een bestaande thumbnail optie of voer afmetingsopties in:"
 
 msgid "Choose resize parameters:"
 msgstr "Selecteer afmetingsopties:"
 
 msgid "Clear"
@@ -156,38 +172,78 @@
 
 msgid "Disable permissions for selected files"
 msgstr "Schakel toegangsrechten uit voor geselecteerde bestanden"
 
 msgid "Django site admin"
 msgstr "Django site beheer"
 
+msgid "Download"
+msgstr "Download"
+
 msgid "Download '%(item_label)s'"
 msgstr "Download '%(item_label)s'"
 
 msgid "Drop files here or use the \"Upload Files\" button"
 msgstr "Sleep hier bestanden naartoe of gebruik de \"Bestanden uploaden\"-knop"
 
 msgid "Drop your file to upload into:"
 msgstr "Sleep je bestand om te uploaden naar:"
 
 msgid "Duplicates"
 msgstr "Duplicaten"
 
+msgid "Edit"
+msgstr "Bewerken"
+
 msgid "Empty Clipboard"
 msgstr "Leeg klembord"
 
 msgid "Enable permissions for selected files"
 msgstr "Schakel toegangsrechten in voor geselecteerde bestanden"
 
+msgid "Everybody"
+msgstr "Iedereen"
+
+msgid "Expand"
+msgstr "Uitvouwen"
+
+msgid "File \"{file_name}\": HTML upload denied by site security policy"
+msgstr ""
+"Bestand \"{file_name}\": HTML upload geweigerd door het beveiligingsbeleid "
+"van de site"
+
+msgid ""
+"File \"{file_name}\": Rejected due to potential cross site scripting "
+"vulnerability"
+msgstr ""
+"Bestand \"{file_name}\": Afgewezen wegens mogelijke kwetsbaarheid voor cross-"
+"site scripting"
+
+msgid "File \"{file_name}\": Upload denied by site security policy"
+msgstr ""
+"Bestand \"{file_name}\": Upload geweigerd door het beveiligingsbeleid van de "
+"site"
+
+msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
+msgstr ""
+"Bestand \"{file_name}\": {file_type} upload geweigerd door het "
+"beveiligingsbeleid van de site"
+
+msgid "File is missing"
+msgstr "Bestand ontbreekt"
+
 msgid "File-size"
 msgstr "Bestandsgrootte"
 
 msgid "Filer"
 msgstr "Bestandsbeheer"
 
+msgid "Files"
+msgstr "Bestanden"
+
 msgid "Folder"
 msgstr "Map"
 
 msgid "Folder Icon"
 msgstr "Map icoon"
 
 msgid "Folder with this name already exists."
@@ -216,14 +272,17 @@
 
 msgid "Go back to root folder"
 msgstr "Ga terug naar de hoofdmap"
 
 msgid "Go back to the parent folder"
 msgstr "Ga terug naar de bovenliggende folder"
 
+msgid "Group: {group}"
+msgstr "Groep: {group}"
+
 msgid "History"
 msgstr "Geschiedenis"
 
 msgid "Home"
 msgstr "Home"
 
 msgid "Invalid rename format: %(error)s."
@@ -249,14 +308,17 @@
 
 msgid "Limit the search to current folder"
 msgstr "Zoekopdracht beperken tot huidige map"
 
 msgid "Location of the main subject of the scene. Format: \"x,y\"."
 msgstr "Locatie van het hoofdonderwerp van de scène. Formaat: \"x,y\"."
 
+msgid "Logical Path"
+msgstr "Logisch Pad"
+
 msgid "Lookup"
 msgstr "Opzoeken"
 
 msgid "Media library"
 msgstr "Mediabibliotheek"
 
 msgid "Modified"
@@ -283,15 +345,15 @@
 msgid "New Folder"
 msgstr "Nieuwe map"
 
 msgid "No action selected."
 msgstr "Geen actie geselecteerd."
 
 msgid "No, take me back"
-msgstr "Nee, neem me mee terug"
+msgstr "Nee, ga terug"
 
 msgid "Owner"
 msgstr "Eigenaar"
 
 msgid "Page %(number)s of %(num_pages)s."
 msgstr "Pagina %(number)s van %(num_pages)s."
 
@@ -305,14 +367,17 @@
 msgstr "Toegangsrechten uitgeschakeld"
 
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] "Herstel onderstaande fout."
 msgstr[1] "Herstel onderstaande fouten."
 
+msgid "Read"
+msgstr "Lezen"
+
 msgid "Remove file"
 msgstr "Verwijder bestand"
 
 msgid "Remove folder"
 msgstr "Verwijder map"
 
 msgid "Rename"
@@ -338,23 +403,32 @@
 
 msgid "Save"
 msgstr "Opslaan"
 
 msgid "Search"
 msgstr "Zoeken"
 
+msgid "Select all"
+msgstr "Alles selecteren"
+
 msgid "Select all %(total_count)s"
 msgstr "Selecteer alle %(total_count)s"
 
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Selecteer alle %(total_count)s bestanden en/of mappen"
 
 msgid "Select this file"
 msgstr "Selecteer dit bestand"
 
+msgid "Show table view"
+msgstr "Toon tabel weergave"
+
+msgid "Show thumbnail view"
+msgstr "Toon thumbnail weergave"
+
 msgid "Size"
 msgstr "Grootte"
 
 msgid "Subject location"
 msgstr "Locatie van onderwerp"
 
 msgid "Subject location is outside of the image. "
@@ -467,28 +541,40 @@
 
 msgid "Upload canceled!"
 msgstr "Upload geannuleerd!"
 
 msgid "Upload success!"
 msgstr "Upload succesvol!"
 
+msgid "User: {user}"
+msgstr "Gebruiker:{user}"
+
 msgid "View on site"
 msgstr "Bekijk op site"
 
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
 msgstr ""
 "Waarschuwing: bestaande afmetingen van afbeeldingen zullen worden aangepast. "
 "Oorspronkelijke bestanden zullen verloren gaan. Maak eventueel eerst een "
 "kopie om de oorspronkelijke bestanden te behouden."
 
+msgid "What"
+msgstr "Wat"
+
+msgid "Who"
+msgstr "Wie"
+
 msgid "Yes, I&#39;m sure"
 msgstr "Ja, ik weet het zeker"
 
+msgid "You do not have permission to upload files."
+msgstr "Je hebt geen rechten om bestanden te uploaden."
+
 msgid "You have to select a folder first"
 msgstr "Je moet eerst een map selecteren"
 
 msgid ""
 "Your account doesn't have permissions to copy all of the selected files and/"
 "or folders."
 msgstr ""
@@ -510,14 +596,20 @@
 
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
 msgstr ""
 "Je account heeft geen toegangsrechten om afmetingen van alle geselecteerde "
 "afbeeldingen aan te passen."
 
+msgid "Your browser does not support audio."
+msgstr "Je browser ondersteunt geen audio."
+
+msgid "Your browser does not support video."
+msgstr "Je browser ondersteunt geen video."
+
 msgid "Your input: \"{subject_location}\". "
 msgstr "Je invoer: \"{subject_location}\"."
 
 msgid "admin homepage"
 msgstr "admin homepage"
 
 msgid "all items"
@@ -544,15 +636,15 @@
 msgid "cancel"
 msgstr "annuleer"
 
 msgid "cancel search"
 msgstr "annuleer zoekopdracht"
 
 msgid "canonical URL"
-msgstr "Gebruikelijke URL"
+msgstr "canonieke URL"
 
 msgid "clipboard"
 msgstr "klembord"
 
 msgid "clipboard item"
 msgstr "klembord item"
 
@@ -630,14 +722,17 @@
 
 msgid "image"
 msgstr "afbeelding"
 
 msgid "images"
 msgstr "afbeeldingen"
 
+msgid "inherit"
+msgstr "overerven"
+
 msgid "modified at"
 msgstr "gewijzigd op"
 
 msgid "must always publish author credit"
 msgstr "naam auteur altijd publiceren"
 
 msgid "must always publish copyright"
@@ -657,14 +752,17 @@
 
 msgid "original filename"
 msgstr "oorspronkelijke bestandsnaam"
 
 msgid "owner"
 msgstr "eigenaar"
 
+msgid "parent"
+msgstr "ouder"
+
 msgid "previous"
 msgstr "vorige"
 
 msgid "root"
 msgstr "hoofdmap"
 
 msgid "sha1"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Alexander Schoemaker <alexander.schoemaker@gmail.com>, 2012
 # Alexander Schoemaker <alexander.schoemaker@gmail.com>, 2012
+# Edwin Janssen, 2023
 # Evelijn Saaltink <evelijnsaaltink@gmail.com>, 2017
 # Jeroen, 2018
 # Maikel Wever, 2013
 # Maikel Wever, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Jeroen, 2018\n"
-"Language-Team: Dutch (Netherlands) (http://app.transifex.com/divio/django-"
-"filer/language/nl_NL/)\n"
-"Language: nl_NL\n"
+"Last-Translator: Edwin Janssen, 2023\n"
+"Language-Team: Dutch (Netherlands) (http://app.transifex.com/divio/django-filer/language/nl_NL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
-msgstr ""
+msgstr "Je hebt geen rechten om bestanden te uploaden."
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
-msgstr ""
+msgstr "Kan map niet vinden om te uploaden. Herlaad de pagina en probeer het opnieuw."
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
-msgstr ""
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
+msgstr "Kan deze map niet gebruiken, rechten geweigerd. Kies een andere map."
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Geavanceerd"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
-msgstr "Gebruikelijke URL"
+msgstr "canonieke URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"De actie kan niet worden uitgevoerd omdat er zijn geen items geselecteerd."
+msgstr "De actie kan niet worden uitgevoerd omdat er zijn geen items geselecteerd."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s geselecteerd"
 msgstr[1] "Alle %(total_count)s geselecteerd"
@@ -128,17 +130,15 @@
 msgstr "Er bestaan al mappen met de namen %s op de geselecteerde bestemming"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d bestanden en of mappen zijn succesvol verplaatst naar map "
-"'%(destination)s'."
+msgstr "%(count)d bestanden en of mappen zijn succesvol verplaatst naar map '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Verplaats bestanden en/of mappen"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -155,17 +155,15 @@
 msgstr "Hernoem bestanden"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d bestanden en/of mappen zijn succesvol gekopieerd naar map "
-"'%(destination)s'."
+msgstr "%(count)d bestanden en/of mappen zijn succesvol gekopieerd naar map '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopieer bestanden en/of mappen"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -182,25 +180,22 @@
 
 #: admin/folderadmin.py:1292
 msgid "Resize selected images"
 msgstr "Afmetingen aanpassen van geselecteerde afbeeldingen"
 
 #: admin/forms.py:24
 msgid "Suffix which will be appended to filenames of copied files."
-msgstr ""
-"Achtervoegsel wordt toegevoegd aan bestandsnaam van gekopieerde bestanden"
+msgstr "Achtervoegsel wordt toegevoegd aan bestandsnaam van gekopieerde bestanden"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Achtervoegsel moet een geldige waarde zijn in kleine letters, bv. "
-"\"%(valid)s\"."
+msgstr "Achtervoegsel moet een geldige waarde zijn in kleine letters, bv. \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Type \"%(key)s\" voor het hernoemen van bestandsnamen is ongeldig."
 
 #: admin/forms.py:54
@@ -255,19 +250,19 @@
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Je invoer: \"{subject_location}\"."
 
 #: admin/permissionadmin.py:10 models/foldermodels.py:379
 msgid "Who"
-msgstr ""
+msgstr "Wie"
 
 #: admin/permissionadmin.py:11 models/foldermodels.py:400
 msgid "What"
-msgstr ""
+msgstr "Wat"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Er bestaat al een map met deze naam."
 
 #: apps.py:9 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
@@ -377,21 +372,19 @@
 msgid "Permissions disabled"
 msgstr "Toegangsrechten uitgeschakeld"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Schakel controle op toegangsrechten uit voor dit bestand. Het bestand zal "
-"publiek toegankelijk zijn voor iedereen"
+msgstr "Schakel controle op toegangsrechten uit voor dit bestand. Het bestand zal publiek toegankelijk zijn voor iedereen"
 
 #: models/foldermodels.py:93
 msgid "parent"
-msgstr ""
+msgstr "ouder"
 
 #: models/foldermodels.py:120
 msgid "created at"
 msgstr "aangemaakt op"
 
 #: models/foldermodels.py:135
 msgid "Folder"
@@ -412,15 +405,15 @@
 
 #: models/foldermodels.py:261
 msgid "this item and all children"
 msgstr "dit item en alle onderliggende items"
 
 #: models/foldermodels.py:265
 msgid "inherit"
-msgstr ""
+msgstr "overerven"
 
 #: models/foldermodels.py:266
 msgid "allow"
 msgstr "toestaan"
 
 #: models/foldermodels.py:267
 msgid "deny"
@@ -455,46 +448,49 @@
 msgstr "toegangsrecht folder"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "toegangsrechten folder"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
-msgstr ""
+msgstr "Alle Mappen"
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
-msgstr ""
+msgstr "Logisch Pad"
 
 #: models/foldermodels.py:370
 #, python-brace-format
 msgid "User: {user}"
-msgstr ""
+msgstr "Gebruiker:{user}"
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
-msgstr ""
+msgstr "Groep: {group}"
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
-msgstr ""
+msgstr "Iedereen"
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
-msgstr ""
+msgstr "Bewerken"
 
 #: models/foldermodels.py:388
 msgid "Read"
-msgstr ""
+msgstr "Lezen"
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
-msgstr ""
+msgstr "Toevoegen kinderen"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum"
 
 #: models/imagemodels.py:25
 msgid "author"
@@ -538,19 +534,20 @@
 #: templates/admin/filer/folder/directory_listing.html:37
 #: templates/admin/filer/folder/directory_listing.html:104
 msgid "root"
 msgstr "hoofdmap"
 
 #: settings.py:273
 msgid "Show table view"
-msgstr ""
+msgstr "Toon tabel weergave"
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
-msgstr ""
+msgstr "Toon thumbnail weergave"
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Geselecteerde actie uitvoeren"
 
 #: templates/admin/filer/actions.html:5
 msgid "Go"
@@ -608,41 +605,33 @@
 msgstr "Duplicaten"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Het verwijderen van de geselecteerde bestanden en/of mappen resulteert in "
-"het verwijderen van gerelateerde objecten. Je hebt echter geen "
-"toegangsrechten voor het verwijderen van de volgende objecttypes:"
+msgstr "Het verwijderen van de geselecteerde bestanden en/of mappen resulteert in het verwijderen van gerelateerde objecten. Je hebt echter geen toegangsrechten voor het verwijderen van de volgende objecttypes:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Het verwijderen van de geselecteerde bestanden en/of mappen leidt tot het "
-"verwijderen van de volgende beschermde gerelateerde objecten:"
+msgstr "Het verwijderen van de geselecteerde bestanden en/of mappen leidt tot het verwijderen van de volgende beschermde gerelateerde objecten:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Weet je zeker dat je de geselecteerde bestanden en/of folders wilt "
-"verwijderen? Alle volgende objecten en gerelateerde items zullen worden "
-"verwijderd: "
+msgstr "Weet je zeker dat je de geselecteerde bestanden en/of folders wilt verwijderen? Alle volgende objecten en gerelateerde items zullen worden verwijderd: "
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
-msgstr "Nee, neem me mee terug"
+msgstr "Nee, ga terug"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:47
 msgid "Yes, I&#39;m sure"
 msgstr "Ja, ik weet het zeker"
 
 #: templates/admin/filer/file/change_form.html:35
 #: templates/admin/filer/folder/change_form.html:21
@@ -677,19 +666,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Map icoon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Je account heeft geen toegangsrechten voor het kopiëren van de geselecteerde "
-"bestanden en/of mappen"
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Je account heeft geen toegangsrechten voor het kopiëren van de geselecteerde bestanden en/of mappen"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -705,17 +692,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Er zijn geen bestanden en/of mappen beschikbaar om te kopiëren."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"De volgende bestanden en/of mappen zullen worden gekopieerd naar een "
-"bestemmingsmap (structuur blijft behouden):"
+msgstr "De volgende bestanden en/of mappen zullen worden gekopieerd naar een bestemmingsmap (structuur blijft behouden):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Bestemmingsmap:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -727,22 +712,19 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Het is niet toegestaan om bestanden naar dezelfde map te kopiëren"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Je account heeft geen toegangsrechten om afmetingen van alle geselecteerde "
-"afbeeldingen aan te passen."
+msgstr "Je account heeft geen toegangsrechten om afmetingen van alle geselecteerde afbeeldingen aan te passen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
-msgstr ""
-"Er zijn geen afbeeldingen beschikbaar voor het aanpassen van afmetingen."
+msgstr "Er zijn geen afbeeldingen beschikbaar voor het aanpassen van afmetingen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "De afmetingen van de volgende afbeeldingen zullen worden aangepast:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
@@ -752,72 +734,60 @@
 msgid "Choose resize parameters:"
 msgstr "Selecteer afmetingsopties:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Waarschuwing: bestaande afmetingen van afbeeldingen zullen worden aangepast. "
-"Oorspronkelijke bestanden zullen verloren gaan. Maak eventueel eerst een "
-"kopie om de oorspronkelijke bestanden te behouden."
+msgstr "Waarschuwing: bestaande afmetingen van afbeeldingen zullen worden aangepast. Oorspronkelijke bestanden zullen verloren gaan. Maak eventueel eerst een kopie om de oorspronkelijke bestanden te behouden."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Afmetingen aanpassen"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Je account heeft geen toegangsrechten om alle geselecteerde bestanden en/of "
-"mappen te verplaatsen."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Je account heeft geen toegangsrechten om alle geselecteerde bestanden en/of mappen te verplaatsen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Er zijn geen bestanden en/of mappen beschikbaar om te verplaatsen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"De volgende bestanden en/of mappen zullen worden verplaatst naar een "
-"bestemmingsmap (huidige mapstructuur blijft behouden): "
+msgstr "De volgende bestanden en/of mappen zullen worden verplaatst naar een bestemmingsmap (huidige mapstructuur blijft behouden): "
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Verplaatsen"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Het is niet toegestaan om bestanden naar dezelfde map te verplaatsen"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Je account heeft onvoldoende toegangsrechten om alle geselecteerde bestanden "
-"te hernoemen."
+msgstr "Je account heeft onvoldoende toegangsrechten om alle geselecteerde bestanden te hernoemen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Er zijn geen bestanden beschikbaar om te hernoemen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"De volgende bestanden zullen worden hernoemd (de oorspronkelijke "
-"mapstructuur en bestandsnamen blijven behouden, alleen de weergave zal "
-"worden gewijzigd):"
+msgstr "De volgende bestanden zullen worden hernoemd (de oorspronkelijke mapstructuur en bestandsnamen blijven behouden, alleen de weergave zal worden gewijzigd):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Hernoemen"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -964,19 +934,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "ingeschakeld"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Gebruikelijke url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Download '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Verwijder bestand"
 
@@ -1030,20 +1002,22 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Selecteer alle %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
-msgstr ""
+msgstr "Alles selecteren"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
-msgstr ""
+msgstr "Bestanden"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Toevoegen nieuwe"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
@@ -1058,19 +1032,19 @@
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr "Opslaan"
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
-msgstr ""
+msgstr "Je browser ondersteunt geen audio."
 
 #: templates/admin/filer/templatetags/file_icon.html:14
 msgid "Your browser does not support video."
-msgstr ""
+msgstr "Je browser ondersteunt geen video."
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:9
 msgid "Clipboard"
 msgstr "Klembord"
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:21
 msgid "Paste all items here"
@@ -1090,25 +1064,26 @@
 
 #: templates/admin/filer/tools/clipboard/clipboard_item_rows.html:16
 msgid "upload failed"
 msgstr "upload mislukt"
 
 #: templates/admin/filer/tools/detail_info.html:11
 msgid "Download"
-msgstr ""
+msgstr "Download"
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
-msgstr ""
+msgstr "Uitvouwen"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
-msgstr ""
+msgstr "Bestand ontbreekt"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Type"
 
 #: templates/admin/filer/tools/detail_info.html:37
 msgid "File-size"
@@ -1154,38 +1129,39 @@
 msgstr "Opzoeken"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Kies bestand"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
-msgstr ""
+msgstr "Kies Map"
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
-msgstr ""
+msgstr "Bestand \"{file_name}\": Upload geweigerd door het beveiligingsbeleid van de site"
 
 #: validation.py:22
 #, python-brace-format
 msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
-msgstr ""
+msgstr "Bestand \"{file_name}\": {file_type} upload geweigerd door het beveiligingsbeleid van de site"
 
 #: validation.py:33
 #, python-brace-format
 msgid "File \"{file_name}\": HTML upload denied by site security policy"
-msgstr ""
+msgstr "Bestand \"{file_name}\": HTML upload geweigerd door het beveiligingsbeleid van de site"
 
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
-msgstr ""
+msgstr "Bestand \"{file_name}\": Afgewezen wegens mogelijke kwetsbaarheid voor cross-site scripting"
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
 "Language-Team: Norwegian Nynorsk (http://app.transifex.com/divio/django-"
 "filer/language/nn/)\n"
-"Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s vald"
 msgstr[1] "Alle %(total_count)s vald"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
-"Language-Team: Norwegian Nynorsk (http://app.transifex.com/divio/django-"
-"filer/language/nn/)\n"
-"Language: nn\n"
+"Language-Team: Norwegian Nynorsk (http://app.transifex.com/divio/django-filer/language/nn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avansert"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Element må vere vald for å utføre handlingar på dei. Ingen element vart "
-"endra."
+msgstr "Element må vere vald for å utføre handlingar på dei. Ingen element vart endra."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s vald"
 msgstr[1] "Alle %(total_count)s vald"
@@ -150,16 +150,15 @@
 msgstr "Endre namn på filer"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Kopierte %(count)d filer og/eller mapper til mappa \"%(destination)s\"."
+msgstr "Kopierte %(count)d filer og/eller mapper til mappa \"%(destination)s\"."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopier filer og/eller mapper"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,17 +182,15 @@
 msgstr "Ending som vert tilføyd filnamn på kopierte filer."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Ending bør vere ein gyldig, enkel del av filnamnet med små bokstavar, som "
-"\"%(valid)s\"."
+msgstr "Ending bør vere ein gyldig, enkel del av filnamnet med små bokstavar, som \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ugyldig nykel \"%(key)s\" for endring av namn."
 
 #: admin/forms.py:54
@@ -446,14 +443,15 @@
 msgstr "løyve for mappe"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "løyve for mappe"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -464,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "dato biletet vert tatt"
 
@@ -532,14 +532,15 @@
 msgstr "rot"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Utfør den valde handlinga"
 
@@ -599,34 +600,27 @@
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Å slette dei valde filene og/eller mappene ville resultere i sletting av "
-"relaterte objekt, men din konto har ikkje løyve til å slette objekt av "
-"følgjande typer:"
+msgstr "Å slette dei valde filene og/eller mappene ville resultere i sletting av relaterte objekt, men din konto har ikkje løyve til å slette objekt av følgjande typer:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Å slette dei valde filene og/eller mappene ville kreve å slette følgjande "
-"beskytta relaterte objekt:"
+msgstr "Å slette dei valde filene og/eller mappene ville kreve å slette følgjande beskytta relaterte objekt:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Er du sikker på at du vil slette dei valde filene og/eller mappene? Alle dei "
-"følgjande objekta og deira relaterte element vil verte sletta:"
+msgstr "Er du sikker på at du vil slette dei valde filene og/eller mappene? Alle dei følgjande objekta og deira relaterte element vil verte sletta:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -667,19 +661,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappeikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Din konto har ikkje løyve til å kopiere alle dei valde filene og/eller "
-"mappene."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Din konto har ikkje løyve til å kopiere alle dei valde filene og/eller mappene."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -695,17 +687,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Det er ingen filer og/eller mapper å kopiere."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Dei følgjande filene og/eller mappene vil verte kopiert til ein målmappe "
-"(mappestruktur vil behaldes):"
+msgstr "Dei følgjande filene og/eller mappene vil verte kopiert til ein målmappe (mappestruktur vil behaldes):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Målmappe:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -729,52 +719,45 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Dei følgjande bileta vil få endra storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Vel eit eksisterande miniatyrbileteval eller skriv inn parametrar for "
-"endring av storleik:"
+msgstr "Vel eit eksisterande miniatyrbileteval eller skriv inn parametrar for endring av storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Vel parametrar for endring av storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Åtvaring: Bileta vil få sin storleik endra, og originalane vil gå tapt. Det "
-"kan være ønskjeleg å først gjere ein kopi for å behalde originalane."
+msgstr "Åtvaring: Bileta vil få sin storleik endra, og originalane vil gå tapt. Det kan være ønskjeleg å først gjere ein kopi for å behalde originalane."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Endre storleik"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Din konto har ikke løyve til å flytte alle dei valde filene og/eller mappene."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Din konto har ikke løyve til å flytte alle dei valde filene og/eller mappene."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Det er ingen filer og/eller mapper å flytte."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Dei følgjande filene og/eller mappene vil verte flytta til ein målmappe "
-"(mappestruktur vil behaldes):"
+msgstr "Dei følgjande filene og/eller mappene vil verte flytta til ein målmappe (mappestruktur vil behaldes):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Flytt"
 
@@ -791,17 +774,15 @@
 msgid "There are no files available to rename."
 msgstr "Det er ingen filer å endre namn på."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Dei følgjande filene vil få endra namn (dei vil framleis vere på samme stad "
-"og behalde originalt filnamn, berre visningsnamn vil verte endra):"
+msgstr "Dei følgjande filene vil få endra namn (dei vil framleis vere på samme stad og behalde originalt filnamn, berre visningsnamn vil verte endra):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Endre namn"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -948,19 +929,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivert"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1014,18 +997,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Legg til ny"
@@ -1083,14 +1068,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1138,14 +1124,15 @@
 msgstr "Slå opp"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Grzegorz Biały <grzegorz@elcodo.pl>, 2017\n"
 "Language-Team: Polish (http://app.transifex.com/divio/django-filer/language/"
 "pl/)\n"
-"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s plik"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # crunchorn <crunchorn@prokonto.pl>, 2010
 # Grzegorz Biały <grzegorz@elcodo.pl>, 2017
 # Mateusz Marzantowicz <mmarzantowicz@osdf.com.pl>, 2013
 # Piotr Wojcik <pwwpww@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Grzegorz Biały <grzegorz@elcodo.pl>, 2017\n"
-"Language-Team: Polish (http://app.transifex.com/divio/django-filer/language/"
-"pl/)\n"
-"Language: pl\n"
+"Language-Team: Polish (http://app.transifex.com/divio/django-filer/language/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
-"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
-"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Language: pl\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Zaawansowane"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "kanoniczny URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Należy zaznaczyć elementy aby wykonań na nich jakąś akcję. Nie zaznaczono "
-"żadnych elementów."
+msgstr "Należy zaznaczyć elementy aby wykonań na nich jakąś akcję. Nie zaznaczono żadnych elementów."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "zaznaczono %(total_count)s"
 msgstr[1] "zaznaczono %(total_count)s"
@@ -131,16 +129,15 @@
 msgstr "Katalogi z nazwami %s już istnieją w podanej lokacji"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Pomyślnie przeniesiono %(count)d plików i/lub katalogów do '%(destination)s'."
+msgstr "Pomyślnie przeniesiono %(count)d plików i/lub katalogów do '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Przenieś pliki i/lub katalogi"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -157,16 +154,15 @@
 msgstr "Zmień nazwy plików"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Pomyślnie skopiowano %(count)d plików i/lub katalogów di '%(destination)s'."
+msgstr "Pomyślnie skopiowano %(count)d plików i/lub katalogów di '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Skopiuj pliki i/lub katalogi"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -190,17 +186,15 @@
 msgstr "Przyrostek, który zostanie dodany do nazw skopiowanych plików."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Przyrostek powinien być poprawną, prostą, składającą się z małych liter "
-"częścią nazwy pliku, np. \"%(valid)s\""
+msgstr "Przyrostek powinien być poprawną, prostą, składającą się z małych liter częścią nazwy pliku, np. \"%(valid)s\""
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nieznany format klucza \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -377,17 +371,15 @@
 msgid "Permissions disabled"
 msgstr "Uprawnienia wyłączone"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Wyłącz jakiekolwiek sprawdzanie uprawnień dla tego pliku. Plik będzie "
-"dostępny publicznie dla wszystkich."
+msgstr "Wyłącz jakiekolwiek sprawdzanie uprawnień dla tego pliku. Plik będzie dostępny publicznie dla wszystkich."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -455,14 +447,15 @@
 msgstr "uprawnienie katalogu"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "uprawnienia katalogu"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -473,26 +466,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data wykonania"
 
@@ -541,14 +536,15 @@
 msgstr "Katalog główny"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Wykonaj wybraną akcję"
 
@@ -608,34 +604,27 @@
 msgstr "Duplikaty"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Usunięcie zaznaczonych plików i/lub katalogów spowoduje usunięcie "
-"powiązanych obiektów, niestety Twoje konto nie posiada uprawnień do "
-"usunięcia następujących typów obiektów:"
+msgstr "Usunięcie zaznaczonych plików i/lub katalogów spowoduje usunięcie powiązanych obiektów, niestety Twoje konto nie posiada uprawnień do usunięcia następujących typów obiektów:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Usunięcie zaznaczonych plików i/lub katalogów wymaga usunięcia następujących "
-"chronionych obiektów powiązanych:"
+msgstr "Usunięcie zaznaczonych plików i/lub katalogów wymaga usunięcia następujących chronionych obiektów powiązanych:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Czy na pewno chcesz usunąć zaznaczone pliki i/lub katalogi? Następujące "
-"obiekty oraz powiązane z nimi elementy zostaną usunięte:"
+msgstr "Czy na pewno chcesz usunąć zaznaczone pliki i/lub katalogi? Następujące obiekty oraz powiązane z nimi elementy zostaną usunięte:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Nie, wróć"
 
@@ -676,19 +665,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona katalogu"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Twoje konto nie ma uprawnień do skopiowania wszystkich zaznaczonych plików i/"
-"lub katalogów."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Twoje konto nie ma uprawnień do skopiowania wszystkich zaznaczonych plików i/lub katalogów."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -704,17 +691,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Brak dostępnych plików i/lub katalogów do skopiowania."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Następujące pliki i/lub katalogi zostaną skopiowane do katalogu docelowego "
-"(z zachowaniem ich struktury):"
+msgstr "Następujące pliki i/lub katalogi zostaną skopiowane do katalogu docelowego (z zachowaniem ich struktury):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Katalog docelowy:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -726,96 +711,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Nie można kopiować plików to tego samego folderu"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Twoje konto nie ma uprawnień do zmiany rozmiaru wszystkich zaznaczonych "
-"obrazów."
+msgstr "Twoje konto nie ma uprawnień do zmiany rozmiaru wszystkich zaznaczonych obrazów."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Brak dostępnych obrazów do zmiany ich rozmiaru."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Następujące obrazy będą miały zmieniony rozmiar:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Wybierz istniejącą opcje miniatury albo wprowadź parametry zmiany rozmiaru:"
+msgstr "Wybierz istniejącą opcje miniatury albo wprowadź parametry zmiany rozmiaru:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Wybierz parametry zmiany rozmiaru:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Uwaga: Rozmiary obrazów zostanie zmienione w miejscu a oryginały zostaną "
-"utracone. W celu zachowania oryginałów, najpierw wykonaj ich kopię."
+msgstr "Uwaga: Rozmiary obrazów zostanie zmienione w miejscu a oryginały zostaną utracone. W celu zachowania oryginałów, najpierw wykonaj ich kopię."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Zmień rozmiar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Twoje konto nie ma uprawnień do przeniesienia wszystkich zaznaczonych plików "
-"i/lub katalogów."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Twoje konto nie ma uprawnień do przeniesienia wszystkich zaznaczonych plików i/lub katalogów."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Brak plików i/lub folderów do przeniesienia."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Następujące pliki i/lub katalogi zostaną przeniesione do katalogu docelowego "
-"(z zachowaniem ich struktury):"
+msgstr "Następujące pliki i/lub katalogi zostaną przeniesione do katalogu docelowego (z zachowaniem ich struktury):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Przenieś"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Nie można przenieść plików do tego samego folderu"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Twoje konto nie posiada uprawnień do zmiany nazwy wszystkich zaznaczonych "
-"plików."
+msgstr "Twoje konto nie posiada uprawnień do zmiany nazwy wszystkich zaznaczonych plików."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Brak dostępnych plików do zmiany nazwy."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Następujące pliki będą miały zmienioną nazwę (pliki pozostaną w swoich "
-"katalogach i zachowają oryginalne nazwy, zmieni się jedynie ich wyświetlana "
-"nazwa):"
+msgstr "Następujące pliki będą miały zmienioną nazwę (pliki pozostaną w swoich katalogach i zachowają oryginalne nazwy, zmieni się jedynie ich wyświetlana nazwa):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Zmień nazwę"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -966,19 +937,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "włączony"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanoniczny url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Pobierz '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Usuń plik"
 
@@ -1032,18 +1005,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Wybierz wszystkie %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Dodaj nowy"
@@ -1103,14 +1078,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Typ"
 
@@ -1158,14 +1134,15 @@
 msgstr "Wyszukaj"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Wybierz plik"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Portuguese (http://www.transifex.com/divio/django-filer/"
-"language/pt/)\n"
-"Language: pt\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/divio/django-filer/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_CN\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -47,15 +49,14 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
-msgstr[1] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -439,14 +440,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -457,26 +459,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -525,14 +529,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -653,16 +658,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -729,16 +734,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -868,23 +873,21 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -921,19 +924,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -987,18 +992,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1007,15 +1014,14 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1056,14 +1062,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1111,14 +1118,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1136,21 +1144,50 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
-#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Julio Lucchese <juliorieger@gmail.com>, 2018\n"
 "Language-Team: Portuguese (Brazil) (http://app.transifex.com/divio/django-"
 "filer/language/pt_BR/)\n"
-"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s arquivo"
 msgstr[1] "%(counter)s arquivos"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Claudio Rogerio Carvalho Filho <excriptbrasil@gmail.com>, 2017
 # Julio Lucchese <juliorieger@gmail.com>, 2018
 # Rodrigo <rprior@infranology.com.br>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Julio Lucchese <juliorieger@gmail.com>, 2018\n"
-"Language-Team: Portuguese (Brazil) (http://app.transifex.com/divio/django-"
-"filer/language/pt_BR/)\n"
-"Language: pt_BR\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/divio/django-filer/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: pt_BR\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Avançado"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL canônico"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"itens precisam ser selecionar para que a ação seja executada. Nenhuma "
-"alteração foi efetuada."
+msgstr "itens precisam ser selecionar para que a ação seja executada. Nenhuma alteração foi efetuada."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s selecionado"
 msgstr[1] "Todos %(total_count)s selecionados"
@@ -128,17 +127,15 @@
 msgstr "Pastas com os nomes %s s já existem no local selecionado"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d arquivo(s) e/ou pasta(s) foram movidos para a pasta "
-"'%(destination)s' com sucesso."
+msgstr "%(count)d arquivo(s) e/ou pasta(s) foram movidos para a pasta '%(destination)s' com sucesso."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Mover arquivo(s) e/ou pasta(s)"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -155,17 +152,15 @@
 msgstr "Renomear arquivos"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d arquivo(s) e/ou pasta(s) foram copiados para o pasta "
-"'%(destination)s' com sucesso."
+msgstr "%(count)d arquivo(s) e/ou pasta(s) foram copiados para o pasta '%(destination)s' com sucesso."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copiar arquivo(s) e/ou pasta(s)"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -189,24 +184,20 @@
 msgstr "Sufixo que será anexado aos nomes dos arquivos copiados"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"O sufixo precisa ser válido, simples e com letras minúsculas para o nome de "
-"um arquivo, como por exemplo: \"%(valid)s\"."
+msgstr "O sufixo precisa ser válido, simples e com letras minúsculas para o nome de um arquivo, como por exemplo: \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
-msgstr ""
-"A chave de valor \"%(key)s\" utilizada para renomear o arquivo é "
-"desconhecida."
+msgstr "A chave de valor \"%(key)s\" utilizada para renomear o arquivo é desconhecida."
 
 #: admin/forms.py:54
 #, python-format
 msgid "Invalid rename format: %(error)s."
 msgstr "Formato inválido para renomear: %(error)s."
 
 #: admin/forms.py:64 models/thumbnailoptionmodels.py:37
@@ -227,16 +218,15 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "aumentar"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr ""
-"Escolher entre as opções de miniaturas ou parâmetros de redimensionamento."
+msgstr "Escolher entre as opções de miniaturas ou parâmetros de redimensionamento."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Os parâmetros de redimensionamento precisam ser escolhidos"
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -379,17 +369,15 @@
 msgid "Permissions disabled"
 msgstr "Permissões desabilitadas"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Desative qualquer verificação de permissão para este arquivo. O arquivo "
-"estará acessível ao público para que qualquer possa acessar."
+msgstr "Desative qualquer verificação de permissão para este arquivo. O arquivo estará acessível ao público para que qualquer possa acessar."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -457,14 +445,15 @@
 msgstr "permissão de pasta"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "permissões de pasta"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -475,26 +464,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data de tomada"
 
@@ -543,14 +534,15 @@
 msgstr "raiz"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Executar a ação selecionada"
 
@@ -610,35 +602,27 @@
 msgstr "Duplicados"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Remover os arquivo(s) e/ou pasta(s) selecionados resultará na remoção de "
-"objetos relacionados, mas sua conta não tem permissão para remover os "
-"seguintes tipos de objetos:"
+msgstr "Remover os arquivo(s) e/ou pasta(s) selecionados resultará na remoção de objetos relacionados, mas sua conta não tem permissão para remover os seguintes tipos de objetos:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Remover os arquivo(s) e/ou pasta(s) selecionados, requer remover os seguites "
-"objetos protegidos relacionados:"
+msgstr "Remover os arquivo(s) e/ou pasta(s) selecionados, requer remover os seguites objetos protegidos relacionados:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Você tem certeza que deseja remover os arquivo(s) e/ou pasta(s) "
-"selecionados? Todos os seguintes objetos e itens relacionados serão "
-"removidos: "
+msgstr "Você tem certeza que deseja remover os arquivo(s) e/ou pasta(s) selecionados? Todos os seguintes objetos e itens relacionados serão removidos: "
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Não, me leve de volta"
 
@@ -679,19 +663,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ícone da Pasta"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Sua conta não possui permissão para copiar todos os arquivo(s) e/ou pasta(s) "
-"selecionados."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Sua conta não possui permissão para copiar todos os arquivo(s) e/ou pasta(s) selecionados."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -707,17 +689,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Não existem arquivo(s) e/ou pasta(s) disponíveis para copiar."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Os arquivo(s) e/ou pasta(s) serão copiados para a pasta de destino (mantendo "
-"a estrutura de diretórios):"
+msgstr "Os arquivo(s) e/ou pasta(s) serão copiados para a pasta de destino (mantendo a estrutura de diretórios):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Pasta de destino:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -729,96 +709,82 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Não é permitido copiar arquivos para a mesma pasta"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Sua conta não possui permissão para redimensionar todas as imagens "
-"selecionadas."
+msgstr "Sua conta não possui permissão para redimensionar todas as imagens selecionadas."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Não existem imagens disponíveis para redimensionar."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "As seguintes imagens serão redimensionadas:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Selecionar uma opção de miniatura ou digitar os parâmetros de "
-"redimensionamento:"
+msgstr "Selecionar uma opção de miniatura ou digitar os parâmetros de redimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Selecionar os parâmetros de redimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Cuidado: as imagens serão redimensionadas no mesmo local e os originais "
-"serão perdidos. Uma sugestão seria fazer uma cópia para guardar os originais."
+msgstr "Cuidado: as imagens serão redimensionadas no mesmo local e os originais serão perdidos. Uma sugestão seria fazer uma cópia para guardar os originais."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Sua conta não possui permissão para mover todos os arquivo(s) e/ou pasta(s) "
-"selecionados."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Sua conta não possui permissão para mover todos os arquivo(s) e/ou pasta(s) selecionados."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Não existem arquivo(s) e/ou pasta(s) disponíveis para mover."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Os arquivo(s) e/ou pasta(s) serão movidos para a pasta de destino (mantendo "
-"a estrutura de diretórios):"
+msgstr "Os arquivo(s) e/ou pasta(s) serão movidos para a pasta de destino (mantendo a estrutura de diretórios):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Mover"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Não é permitido mover arquivos na mesma pasta"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr ""
-"Sua conta não possui permissão para renomear todos os arquivos selecionados."
+msgstr "Sua conta não possui permissão para renomear todos os arquivos selecionados."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Não existem arquivos disponíveis para renomear."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Os seguintes arquivos serão renomeados (estes arquivos serão mantidos em "
-"suas pastas e os nomes originais serão mantidos, apenas o nome de "
-"apresentação será alterado):"
+msgstr "Os seguintes arquivos serão renomeados (estes arquivos serão mantidos em suas pastas e os nomes originais serão mantidos, apenas o nome de apresentação será alterado):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Renomear"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -967,19 +933,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "habilitado"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "URL Canônico '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Baixar '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Remover arquivo"
 
@@ -1033,18 +1001,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Selecione todos %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Adicionar novo"
@@ -1103,14 +1073,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
@@ -1158,14 +1129,15 @@
 msgstr "Pesquisar"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Alterar Arquivo"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Alexander Naydenko <an@zeppelinen.com>, 2020\n"
 "Language-Team: Russian (http://app.transifex.com/divio/django-filer/language/"
 "ru/)\n"
-"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s файл"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Alexander Naydenko <an@zeppelinen.com>, 2020
 # Oleg Fish <okfish@yandex.ru>, 2017
 # Pavel <neoascetic@gmail.com>, 2012
 # Pavel <neoascetic@gmail.com>, 2012
@@ -13,51 +13,49 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Alexander Naydenko <an@zeppelinen.com>, 2020\n"
-"Language-Team: Russian (http://app.transifex.com/divio/django-filer/language/"
-"ru/)\n"
-"Language: ru\n"
+"Language-Team: Russian (http://app.transifex.com/divio/django-filer/language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: ru\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Дополнительно"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "канонический URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Для выполнения действий нужно выбрать хотя бы один объект. Не произведено "
-"никаких изменений."
+msgstr "Для выполнения действий нужно выбрать хотя бы один объект. Не произведено никаких изменений."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s выбран"
 msgstr[1] "%(total_count)s выбрано"
@@ -189,17 +187,15 @@
 msgstr "Окончание, которое будет добавлено к именам скопированных файлов."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Окончание должно быть правильной, простой и в нижнем регистре частью имени "
-"файла, например \"%(valid)s\"."
+msgstr "Окончание должно быть правильной, простой и в нижнем регистре частью имени файла, например \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Неизвестный ключ форматирования \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -376,17 +372,15 @@
 msgid "Permissions disabled"
 msgstr "Разрешения отключены"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Отменить все проверки разрешений для этого файла. Файл будет доступен "
-"публично для каждого."
+msgstr "Отменить все проверки разрешений для этого файла. Файл будет доступен публично для каждого."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -454,14 +448,15 @@
 msgstr "разрешение папки"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "разрешения папки"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -472,26 +467,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "дата создания"
 
@@ -540,14 +537,15 @@
 msgstr "корень"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Выполнить выбранное действие"
 
@@ -607,33 +605,27 @@
 msgstr "Дубликаты"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Удаление выбранных файлов/папок приведет к удалению связанных объектов, но у "
-"вас нет прав удалять следующие объекты:"
+msgstr "Удаление выбранных файлов/папок приведет к удалению связанных объектов, но у вас нет прав удалять следующие объекты:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Удаление выбранных файлов/папок потребует удаления следующих защищенных "
-"связанных объектов:"
+msgstr "Удаление выбранных файлов/папок потребует удаления следующих защищенных связанных объектов:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Вы уверены, что хотите удалить выбранные файлы/папки? Следующие объекты "
-"вместе со связанными объектами будут удалены:"
+msgstr "Вы уверены, что хотите удалить выбранные файлы/папки? Следующие объекты вместе со связанными объектами будут удалены:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Нет, пустите меня обратно"
 
@@ -674,16 +666,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Иконка папки"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr "У вас нет прав на копирование выбранных файлов/папок"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -700,17 +692,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Нет файлов для копирования."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Эти файлы/папки будут скопированы в целевую папку (с сохранением "
-"иерархичности):"
+msgstr "Эти файлы/папки будут скопированы в целевую папку (с сохранением иерархичности):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Целевая папка:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -744,39 +734,35 @@
 msgid "Choose resize parameters:"
 msgstr "Выбрите параметры изменения размеров:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Внимание: изображения будут изменены в размерах с заменой оригиналов. "
-"Возможно, лучше будет сперва сделать копии."
+msgstr "Внимание: изображения будут изменены в размерах с заменой оригиналов. Возможно, лучше будет сперва сделать копии."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Изменить размеры"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr "Вы не имеете прав для перемещения выбранных файлов/папок."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Нет файлов/папок для перемещения."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Следующие файлы/папки будут перемещены в целевую папку (сохраняя "
-"иерархичность):"
+msgstr "Следующие файлы/папки будут перемещены в целевую папку (сохраняя иерархичность):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Переместить"
 
@@ -793,17 +779,15 @@
 msgid "There are no files available to rename."
 msgstr "Нет файлов для переименовывания."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Эти файлы будут переименованы (они остануться в их папках и сохранят имена "
-"оригинальных файлов, только отображаемое имя измениться):"
+msgstr "Эти файлы будут переименованы (они остануться в их папках и сохранят имена оригинальных файлов, только отображаемое имя измениться):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Переименовать"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -954,19 +938,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "включены"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Канонический URL '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Скачать '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Удалить файл"
 
@@ -1020,18 +1006,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Выбрать все %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Добавить новую"
@@ -1091,14 +1079,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Тип"
 
@@ -1146,14 +1135,15 @@
 msgstr "Выбрать"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Выбрать файл"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Slovak (http://www.transifex.com/divio/django-filer/language/"
-"sk/)\n"
-"Language: sk\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/divio/django-filer/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -47,16 +49,14 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -440,14 +440,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -458,26 +459,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -526,14 +529,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -654,16 +658,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -730,16 +734,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -869,25 +873,21 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -924,19 +924,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -990,18 +992,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1010,16 +1014,14 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1060,14 +1062,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1115,14 +1118,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1140,22 +1144,50 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
-#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
-#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013,2015-2016\n"
 "Language-Team: Turkish (http://app.transifex.com/divio/django-filer/language/"
 "tr/)\n"
-"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "0 of %(cnt)s selected"
 msgstr "%(cnt)s 0 adet  seçildi"
 
 msgid "Action"
 msgstr "İşlem"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013,2015-2016
 # Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013,2015-2016\n"
-"Language-Team: Turkish (http://app.transifex.com/divio/django-filer/language/"
-"tr/)\n"
-"Language: tr\n"
+"Language-Team: Turkish (http://app.transifex.com/divio/django-filer/language/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Gelişmiş"
 
 #: admin/fileadmin.py:160
@@ -123,16 +125,15 @@
 msgstr "%s isimli klasörler seçili hedefte var."
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d adet dosya/klasör başarıyla '%(destination)s' klasörüne taşındı"
+msgstr "%(count)d adet dosya/klasör başarıyla '%(destination)s' klasörüne taşındı"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Dosya veya klasörleri taşı"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,16 +150,15 @@
 msgstr "Dosyaları yeniden adlandır"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"%(count)d adet dosya veya klasör '%(destination)s' klasörüne kopyalandı"
+msgstr "%(count)d adet dosya veya klasör '%(destination)s' klasörüne kopyalandı"
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Dosya veya klasörleri kopyala"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -443,14 +443,15 @@
 msgstr "dizin yetki"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "dizin yetkileri"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -461,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -529,14 +532,15 @@
 msgstr "kök"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Seçili aksiyonu çalışıtır"
 
@@ -657,16 +661,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -733,16 +737,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -925,19 +929,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktif"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Dosyayı kaldır"
 
@@ -991,18 +997,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "%(total_count)s Tümünü seç"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Yeni ekle"
@@ -1060,14 +1068,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tip"
 
@@ -1115,14 +1124,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Dosya Seç"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/vi_VN/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/vi_VN/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Duong Vu Hong <duong.vuhong.uet@gmail.com>, 2021\n"
 "Language-Team: Vietnamese (Viet Nam) (http://app.transifex.com/divio/django-"
 "filer/language/vi_VN/)\n"
-"Language: vi_VN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: vi_VN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] "%(counter)s tệp"
 
 msgid "%(counter)s folder"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 # Duong Vu Hong <duong.vuhong.uet@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Duong Vu Hong <duong.vuhong.uet@gmail.com>, 2021\n"
-"Language-Team: Vietnamese (Viet Nam) (http://app.transifex.com/divio/django-"
-"filer/language/vi_VN/)\n"
-"Language: vi_VN\n"
+"Language-Team: Vietnamese (Viet Nam) (http://app.transifex.com/divio/django-filer/language/vi_VN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: vi_VN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr "Nâng Cao"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
 msgstr "URL hợp chuẩn"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
-"Những item được chọn để thực hiện hành động trên đó. Không có item nào bị "
-"thay đổi."
+msgstr "Những item được chọn để thực hiện hành động trên đó. Không có item nào bị thay đổi."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "Tất cả %(total_count)s được chọn"
 
@@ -123,16 +123,15 @@
 msgstr "Các thư mục với tên %s đã tồn tại ở vị trí đã chọn"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Đã di chuyển %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
+msgstr "Đã di chuyển %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Di chuyển tệp và/hoặc thư mục"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,17 +148,15 @@
 msgstr "Đổi tên tệp"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr ""
-"Đã thành công sao chép %(count)d tệp và/hoặc thư mục tới thư mục "
-"'%(destination)s'."
+msgstr "Đã thành công sao chép %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Sao chép tệp và/hoặc thư mục"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,17 +180,15 @@
 msgstr "Hậu tố sẽ được nối vào tên của tệp đã sao chép."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr ""
-"Hậu tố phải là một phần tên tệp hợp lệ, đơn giản và chữ thường, như "
-"\"%(valid)s\"."
+msgstr "Hậu tố phải là một phần tên tệp hợp lệ, đơn giản và chữ thường, như \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Không biết định dạng đổi tên của khóa giá trị \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -370,17 +365,15 @@
 msgid "Permissions disabled"
 msgstr "Quyền bị vô hiệu hóa"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr ""
-"Vô hiệu hóa bất kỳ quyền kiểm tra cho tệp này. Tệp sẽ truy cập được bởi bất "
-"kỳ ai."
+msgstr "Vô hiệu hóa bất kỳ quyền kiểm tra cho tệp này. Tệp sẽ truy cập được bởi bất kỳ ai."
 
 #: models/foldermodels.py:93
 msgid "parent"
 msgstr ""
 
 #: models/foldermodels.py:120
 msgid "created at"
@@ -448,14 +441,15 @@
 msgstr "quyền thư mục"
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr "những quyền thư mục"
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -466,26 +460,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "ngày nắm giữ"
 
@@ -534,14 +530,15 @@
 msgstr "gốc"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Chạy hành dộng đã chọn"
 
@@ -601,33 +598,27 @@
 msgstr "Lặp"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr ""
-"Xóa tệp và/hoặc thưc mục đã chọn sẽ dẫn đến xóa đối tượng liên quan, nhưng "
-"tài khoản của bạn không có quyền xóa những loại của các đối tượng:"
+msgstr "Xóa tệp và/hoặc thưc mục đã chọn sẽ dẫn đến xóa đối tượng liên quan, nhưng tài khoản của bạn không có quyền xóa những loại của các đối tượng:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr ""
-"Xóa tệp và/hoặc thư mục đã chọn sẽ yêu cầu xóa những đối tượng liên quan "
-"được bảo vệ sau:"
+msgstr "Xóa tệp và/hoặc thư mục đã chọn sẽ yêu cầu xóa những đối tượng liên quan được bảo vệ sau:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr ""
-"Bạn có chắc muốn xóa tệp và/hoặc thư mục đã chọn? Tất cả những đối tượng và "
-"những thứ liên quan đến chúng sẽ bị xóa:"
+msgstr "Bạn có chắc muốn xóa tệp và/hoặc thư mục đã chọn? Tất cả những đối tượng và những thứ liên quan đến chúng sẽ bị xóa:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Không, đưa tôi quay lại"
 
@@ -668,18 +659,17 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Biểu tượng thư mục"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
-msgstr ""
-"Tài khoản của bạn không có quyền để sao chép tất cả tệp và thư mục được chọn."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
+msgstr "Tài khoản của bạn không có quyền để sao chép tất cả tệp và thư mục được chọn."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -695,17 +685,15 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Không có tệp và/hoặc thư mục để sao chép."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Những tệp và thư mục sau sẽ được sao chép tới một thư mục đích (giữ cấu trúc "
-"cây thư mục):"
+msgstr "Những tệp và thư mục sau sẽ được sao chép tới một thư mục đích (giữ cấu trúc cây thư mục):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Thư mục đích:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
@@ -717,67 +705,57 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Không cho phép sao chép tệp tới cùng thư mục"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr ""
-"Tài khoản của bạn không có quyền để thay đổi kích thước của tất cả hình ảnh "
-"đã chọn."
+msgstr "Tài khoản của bạn không có quyền để thay đổi kích thước của tất cả hình ảnh đã chọn."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Không có hình ảnh để thay dổi kích thước"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Hình ảnh dưới đay sẽ bị thay đổi kích thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr ""
-"Chọn một tùy chọn của thumbnail đang tồn tại hoặc nhập tham số thay đổi kích "
-"thước:"
+msgstr "Chọn một tùy chọn của thumbnail đang tồn tại hoặc nhập tham số thay đổi kích thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Chọn tham số thay dổi kích thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr ""
-"Cảnh bảo: Hình ảnh sẽ bị thay đổi tại chỗ và ảnh gốc sẽ bị mất. Có thể tạo "
-"một sao chép của chúng để giữ lại hình ảnh gốc."
+msgstr "Cảnh bảo: Hình ảnh sẽ bị thay đổi tại chỗ và ảnh gốc sẽ bị mất. Có thể tạo một sao chép của chúng để giữ lại hình ảnh gốc."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Thay đổi kích thước"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
-msgstr ""
-"Tài khoản của bạn không có quyền để di chuyển tất cả các tệp và thư mục đã "
-"chọn."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
+msgstr "Tài khoản của bạn không có quyền để di chuyển tất cả các tệp và thư mục đã chọn."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Không có tệp và/hoặc thư mục để di chuyển."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr ""
-"Tệp và thư mục dưới đây sẽ được chuyển tới thư mục đích (giữ nguyên cấu trúc "
-"cây thư mục):"
+msgstr "Tệp và thư mục dưới đây sẽ được chuyển tới thư mục đích (giữ nguyên cấu trúc cây thư mục):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
 #: templates/admin/filer/folder/directory_listing.html:183
 msgid "Move"
 msgstr "Di chuyển"
 
@@ -794,17 +772,15 @@
 msgid "There are no files available to rename."
 msgstr "Không có tệp để đổi tên."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr ""
-"Tệp dưới đây sẽ bị đổi tên (chúng vẫn ở trong thư mục của chúng và giữ tên "
-"gốc, chỉ tên hiển thị sẽ bị thay đổi):"
+msgstr "Tệp dưới đây sẽ bị đổi tên (chúng vẫn ở trong thư mục của chúng và giữ tên gốc, chỉ tên hiển thị sẽ bị thay đổi):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Đổi tên"
 
 #: templates/admin/filer/folder/directory_listing.html:96
 msgid "Go back to the parent folder"
@@ -949,19 +925,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "đã kích hoạt"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Url hợp chuẩn '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Tải '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Xóa tệp"
 
@@ -1015,18 +993,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Chọn tất cả %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Thêm mới"
@@ -1083,14 +1063,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Kiểu"
 
@@ -1138,14 +1119,15 @@
 msgstr "Tìm kiếm"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Chọn tệp"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.0rc3/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,83 +1,87 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
+# Fariman Ghaedi <farimanghaedi@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Chinese (http://www.transifex.com/divio/django-filer/language/"
-"zh/)\n"
-"Language: zh\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Fariman Ghaedi <farimanghaedi@gmail.com>, 2019\n"
+"Language-Team: Persian (http://app.transifex.com/divio/django-filer/language/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: fa\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
-msgstr ""
+msgstr "پیشرفته"
 
 #: admin/fileadmin.py:160
 msgid "canonical URL"
-msgstr ""
+msgstr "آدرس کانونی"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr ""
+msgstr "برای اینکه بتوانید روی آیتم ها اقداماتی انجام دهید ابتدا باید آیتم ها را انتخاب کنید. هیچ آیتمی تغییر نکرد."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
 #, python-format
 msgid "0 of %(cnt)s selected"
 msgstr ""
 
 #: admin/folderadmin.py:600
 msgid "No action selected."
-msgstr ""
+msgstr "هیچ اقدامی انتخاب نشده است."
 
 #: admin/folderadmin.py:652
 #, python-format
 msgid "Successfully moved %(count)d files to clipboard."
 msgstr ""
 
 #: admin/folderadmin.py:657
 msgid "Move selected files to clipboard"
-msgstr ""
+msgstr "انتقال فایل های انتخاب شده به کلیپ برد"
 
 #: admin/folderadmin.py:697
 #, python-format
 msgid "Successfully disabled permissions for %(count)d files."
 msgstr ""
 
 #: admin/folderadmin.py:699
@@ -100,23 +104,23 @@
 
 #: admin/folderadmin.py:782
 msgid "Cannot delete files and/or folders"
 msgstr ""
 
 #: admin/folderadmin.py:784
 msgid "Are you sure?"
-msgstr ""
+msgstr "آیا مطمئن هستید؟"
 
 #: admin/folderadmin.py:790
 msgid "Delete files and/or folders"
-msgstr ""
+msgstr "پاک کردن فایل ها و/یا پوشه ها"
 
 #: admin/folderadmin.py:811
 msgid "Delete selected files and/or folders"
-msgstr ""
+msgstr "پاک کردن فایل ها و/یا پوشه های انتخاب شده"
 
 #: admin/folderadmin.py:918
 #, python-format
 msgid "Folders with names %s already exist at the selected destination"
 msgstr ""
 
 #: admin/folderadmin.py:922
@@ -438,14 +442,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +461,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +531,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +660,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +736,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -867,21 +875,23 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -918,19 +928,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +996,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1004,14 +1018,15 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1052,14 +1067,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1123,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,20 +1149,51 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-filer-3.0.0rc3/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.0.1/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Translators:
 # Aosp T, 2016-2017
 # node uuz <node1mei@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:02+0200\n"
+"POT-Creation-Date: 2023-06-28 19:25+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: node uuz <node1mei@gmail.com>, 2019\n"
 "Language-Team: Chinese Simplified (http://app.transifex.com/divio/django-filer/language/zh-Hans/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh-Hans\n"
@@ -1125,27 +1125,33 @@
 
 #: templates/admin/filer/widgets/admin_folder.html:16
 #| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
-msgid "File \"{}\": Upload denied by site security policy"
+#, python-brace-format
+msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
 
 #: validation.py:22
-msgid "File \"{}\": {} upload denied by site security policy"
+#, python-brace-format
+msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
 msgstr ""
 
-#: validation.py:30
-msgid "File \"{}\": HTML upload denied by site security policy"
+#: validation.py:33
+#, python-brace-format
+msgid "File \"{file_name}\": HTML upload denied by site security policy"
 msgstr ""
 
-#: validation.py:68
-msgid "File \"{}\": Rejected due to potential cross site scripting vulnerability"
+#: validation.py:71
+#, python-brace-format
+msgid ""
+"File \"{file_name}\": Rejected due to potential cross site scripting "
+"vulnerability"
 msgstr ""
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/divio/django-filer/"
-"language/zh_CN/)\n"
-"Language: zh_CN\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Slovak (http://app.transifex.com/divio/django-filer/language/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: sk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -47,14 +49,17 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -438,14 +443,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +532,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +661,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +737,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -867,21 +876,27 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -918,19 +933,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +1001,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1004,14 +1023,17 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1052,14 +1074,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1130,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,20 +1156,53 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
+#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
+#~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.0.1/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
+# 
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-06-28 19:25+0200\n"
-"PO-Revision-Date: 2018-04-09 06:58+0000\n"
-"Last-Translator: yakky <i.spalletti@nephila.it>\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/divio/django-filer/"
-"language/zh_TW/)\n"
-"Language: zh_TW\n"
+"PO-Revision-Date: 2012-07-13 15:50+0000\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/divio/django-filer/language/lt_LT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: lt_LT\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
+#| msgid ""
+#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgid ""
+"Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
 #: admin/fileadmin.py:45
 msgid "Advanced"
 msgstr ""
 
 #: admin/fileadmin.py:160
@@ -47,14 +49,17 @@
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -438,14 +443,15 @@
 msgstr ""
 
 #: models/foldermodels.py:333
 msgid "folder permissions"
 msgstr ""
 
 #: models/foldermodels.py:359
+#| msgid "Folders"
 msgid "All Folders"
 msgstr ""
 
 #: models/foldermodels.py:361
 msgid "Logical Path"
 msgstr ""
 
@@ -456,26 +462,28 @@
 
 #: models/foldermodels.py:372
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
 #: models/foldermodels.py:374
+#| msgid "everybody"
 msgid "Everybody"
 msgstr ""
 
 #: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
 #: models/foldermodels.py:388
 msgid "Read"
 msgstr ""
 
 #: models/foldermodels.py:389
+#| msgid "can add children"
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -524,14 +532,15 @@
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
+#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -652,16 +661,16 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to copy all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -728,16 +737,16 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files and/"
-"or folders."
+"Your account doesn't have permissions to move all of the selected files "
+"and/or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
@@ -867,21 +876,27 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -918,19 +933,21 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
+#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -984,18 +1001,20 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
+#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
+#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1004,14 +1023,17 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1052,14 +1074,15 @@
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
 #: templatetags/filer_admin_tags.py:101
+#| msgid "file missing"
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1107,14 +1130,15 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
+#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1132,20 +1156,53 @@
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
 msgstr ""
 
+#~ msgid "Open file"
+#~ msgstr "Open file"
+
+#~ msgid "Full size preview"
+#~ msgstr "Full size preview"
+
+#~ msgid "Add Description"
+#~ msgstr "Add Description"
+
+#~ msgid "Author"
+#~ msgstr "Author"
+
+#~ msgid "Add Alt-Text"
+#~ msgstr "Add Alt-Text"
+
+#~ msgid "Add caption"
+#~ msgstr "Add caption"
+
+#~ msgid "Add Tags"
+#~ msgstr "Add Tags"
+
+#~ msgid "Change File"
+#~ msgstr "Change File"
+
+#~ msgid "none selected"
+#~ msgstr "none selected"
+
+#~ msgid "Add Folder"
+#~ msgstr "Add Folder"
+
 #~ msgid "Subject Location"
 #~ msgstr "Subject location"
 
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
+#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
+#~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.0rc3/filer/management/commands/filer_check.py` & `django-filer-3.0.1/filer/management/commands/filer_check.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/management/commands/generate_thumbnails.py` & `django-filer-3.0.1/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/management/commands/import_files.py` & `django-filer-3.0.1/filer/management/commands/import_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,20 @@
         self.image_created = 0
         self.folder_created = 0
 
     def import_file(self, file_obj, folder):
         """
         Create a File or an Image into the given folder
         """
+        from ...settings import IMAGE_EXTENSIONS
         try:
             iext = os.path.splitext(file_obj.name)[1].lower()
         except:  # noqa
             iext = ''
-        if iext in ['.jpg', '.jpeg', '.png', '.gif', '.webp']:
+        if iext in IMAGE_EXTENSIONS:
             obj, created = Image.objects.get_or_create(
                 original_filename=file_obj.name,
                 file=file_obj,
                 folder=folder,
                 is_public=FILER_IS_PUBLIC_DEFAULT)
             if created:
                 self.image_created += 1
```

### Comparing `django-filer-3.0.0rc3/filer/migrations/0001_initial.py` & `django-filer-3.0.1/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.0.1/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.0.1/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.0.1/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.0.1/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.0.1/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.0.1/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.0.1/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0012_file_mime_type.py` & `django-filer-3.0.1/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.0.1/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.0.1/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.0.1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py` & `django-filer-3.0.1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/abstract.py` & `django-filer-3.0.1/filer/models/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
         verbose_name_plural = _("images")
         abstract = True
         default_manager_name = 'objects'
 
     @classmethod
     def matches_file_type(cls, iname, ifile, mime_type):
         # source: https://www.freeformatter.com/mime-types-list.html
-        image_subtypes = ['gif', 'jpeg', 'png', 'x-png', 'svg+xml', 'webp']
+        from ..settings import IMAGE_MIME_TYPES
         maintype, subtype = mime_type.split('/')
-        return maintype == 'image' and subtype in image_subtypes
+        return maintype == 'image' and subtype in IMAGE_MIME_TYPES
 
     def file_data_changed(self, post_init=False):
         attrs_updated = super().file_data_changed(post_init=post_init)
         if attrs_updated:
             try:
                 try:
                     imgfile = self.file.file
```

### Comparing `django-filer-3.0.0rc3/filer/models/clipboardmodels.py` & `django-filer-3.0.1/filer/models/clipboardmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/filemodels.py` & `django-filer-3.0.1/filer/models/filemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/foldermodels.py` & `django-filer-3.0.1/filer/models/foldermodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.contrib.auth import models as auth_models
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.db.models import Q
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.html import format_html, format_html_join
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from .. import settings as filer_settings
 from . import mixins
 
 
 class FolderPermissionManager(models.Manager):
     """
```

### Comparing `django-filer-3.0.0rc3/filer/models/imagemodels.py` & `django-filer-3.0.1/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/mixins.py` & `django-filer-3.0.1/filer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/thumbnailoptionmodels.py` & `django-filer-3.0.1/filer/models/thumbnailoptionmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/tools.py` & `django-filer-3.0.1/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/models/virtualitems.py` & `django-filer-3.0.1/filer/models/virtualitems.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/server/backends/base.py` & `django-filer-3.0.1/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/server/backends/default.py` & `django-filer-3.0.1/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/server/backends/nginx.py` & `django-filer-3.0.1/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/server/backends/xsendfile.py` & `django-filer-3.0.1/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/server/views.py` & `django-filer-3.0.1/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/settings.py` & `django-filer-3.0.1/filer/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,16 @@
         'icon': 'th-large',
         'tooltip_text': _('Show thumbnail view'),
         'template': 'admin/filer/folder/directory_thumbnail_list.html',
     },
 }
 
 DEFERRED_THUMBNAIL_SIZES = (40, 80, 160)
+IMAGE_EXTENSIONS = ['.jpg', '.jpeg', '.png', '.gif', '.webp']
+IMAGE_MIME_TYPES = ['gif', 'jpeg', 'png', 'x-png', 'svg+xml', 'webp']
 
 FILE_VALIDATORS = {
     "text/html": ["filer.validation.deny_html"],
     "image/svg+xml": ["filer.validation.validate_svg"],
 }
 
 remove_mime_types = getattr(settings, "FILER_REMOVE_FILE_VALIDATORS", [])
```

### Comparing `django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.cms.icons.css` & `django-filer-3.0.1/filer/static/filer/css/admin_filer.cms.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.css` & `django-filer-3.0.1/filer/static/filer/css/admin_filer.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/css/admin_filer.fa.icons.css` & `django-filer-3.0.1/filer/static/filer/css/admin_filer.fa.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/css/maps/admin_filer.css.map` & `django-filer-3.0.1/filer/static/filer/css/maps/admin_filer.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.0.1/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.eot` & `django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.svg` & `django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.ttf` & `django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.woff` & `django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/django-filer-iconfont.woff2` & `django-filer-3.0.1/filer/static/filer/fonts/django-filer-iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.0.1/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/src/arrow-down.svg` & `django-filer-3.0.1/filer/static/filer/fonts/src/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/src/link.svg` & `django-filer-3.0.1/filer/static/filer/fonts/src/link.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/src/move-to-folder.svg` & `django-filer-3.0.1/filer/static/filer/fonts/src/move-to-folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/src/th-list.svg` & `django-filer-3.0.1/filer/static/filer/fonts/src/th-list.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/fonts/src/upload.svg` & `django-filer-3.0.1/filer/static/filer/fonts/src/upload.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.0.1/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-audio.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-empty.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-font.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-missing.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-picture.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-video.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/file-zip.svg` & `django-filer-3.0.1/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.0.1/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/folder-root.svg` & `django-filer-3.0.1/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.0.1/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/icons/folder.svg` & `django-filer-3.0.1/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.0.1/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.0.1/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/img/loading_animation.gif` & `django-filer-3.0.1/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/img/upload_button.png` & `django-filer-3.0.1/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.0.1/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.0.1/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.0.1/filer/static/filer/js/addons/dropzone.init.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/filer_popup_response.js` & `django-filer-3.0.1/filer/static/filer/js/addons/filer_popup_response.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.0.1/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.0.1/filer/static/filer/js/addons/popup_handling.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.0.1/filer/static/filer/js/addons/table-dropzone.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/toggler.js` & `django-filer-3.0.1/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.0.1/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.0.1/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/addons/widget.js` & `django-filer-3.0.1/filer/static/filer/js/addons/widget.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/base.js` & `django-filer-3.0.1/filer/static/filer/js/base.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/class.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery-ui.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.0.1/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/storage.py` & `django-filer-3.0.1/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/actions.html` & `django-filer-3.0.1/filer/templates/admin/filer/actions.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/base_site.html` & `django-filer-3.0.1/filer/templates/admin/filer/base_site.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.0.1/filer/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/change_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.0.1/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.0.1/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.0.1/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.0.1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.0.1/filer/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/tools/search_form.html` & `django-filer-3.0.1/filer/templates/admin/filer/tools/search_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.0.1/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.0.1/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templatetags/filer_admin_tags.py` & `django-filer-3.0.1/filer/templatetags/filer_admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templatetags/filer_image_tags.py` & `django-filer-3.0.1/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/templatetags/filer_tags.py` & `django-filer-3.0.1/filer/templatetags/filer_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/thumbnail_processors.py` & `django-filer-3.0.1/filer/thumbnail_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,21 @@
     if zoom:
         if not crop:
             target_x = round(source_x * scale)
             target_y = round(source_y * scale)
         scale *= (100 + int(zoom)) / 100.0
 
     if scale < 1.0 or (scale > 1.0 and upscale):
-        im = im.resize((int(source_x * scale), int(source_y * scale)),
-                       resample=Image.ANTIALIAS)
+        try:
+            im = im.resize((int(source_x * scale), int(source_y * scale)),
+                           resample=Image.LANCZOS)
+        except AttributeError:  # pragma: no cover
+            im = im.resize((int(source_x * scale), int(source_y * scale)),
+                           resample=Image.ANTIALIAS)
+
     # --endsnip-- begin real code
 
     # ===============================
     # subject location aware cropping
     # ===============================
     # res_x, res_y: the resolution of the possibly already resized image
     res_x, res_y = (float(v) for v in im.size)
```

### Comparing `django-filer-3.0.0rc3/filer/utils/compatibility.py` & `django-filer-3.0.1/filer/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.0.1/filer/utils/filer_easy_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/files.py` & `django-filer-3.0.1/filer/utils/files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/generate_filename.py` & `django-filer-3.0.1/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/loader.py` & `django-filer-3.0.1/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/pil_exif.py` & `django-filer-3.0.1/filer/utils/pil_exif.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/recursive_dictionary.py` & `django-filer-3.0.1/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/utils/zip.py` & `django-filer-3.0.1/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/filer/validation.py` & `django-filer-3.0.1/filer/validation.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/setup.cfg` & `django-filer-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc3/setup.py` & `django-filer-3.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 REQUIREMENTS = [
     'django>=2.2,<5',
     'django-polymorphic',
     'easy-thumbnails[svg]',
 ]
 
 
+EXTRA_REQUIREMENTS = {
+    "heif": [
+        "pillow-heif",
+    ],
+}
+
+
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
@@ -57,11 +64,12 @@
     description='A file management application for django that makes handling '
                 'of files and images a breeze.',
     long_description=open('README.rst').read(),
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
+    extras_require=EXTRA_REQUIREMENTS,
     python_requires='>=3.8',
     classifiers=CLASSIFIERS,
     test_suite='tests.settings.run',
 )
```

