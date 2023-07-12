# Comparing `tmp/invenio-i18n-2.0.0.tar.gz` & `tmp/invenio-i18n-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-i18n-2.0.0.tar", last modified: Mon Feb 27 16:57:48 2023, max compression
+gzip compressed data, was "invenio-i18n-2.1.0.tar", last modified: Wed Jul 12 08:42:19 2023, max compression
```

## Comparing `invenio-i18n-2.0.0.tar` & `invenio-i18n-2.1.0.tar`

### file list

```diff
@@ -1,221 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3688 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10056 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/
--rw-r--r--   0 runner    (1001) docker     (122)     9559 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/app.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/assets/semantic-ui/js/invenio_i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/assets/semantic-ui/js/invenio_i18n/app.js
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/babel.py
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6402 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/templates/invenio_i18n/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/templates/invenio_i18n/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/templates/invenio_i18n/macros/language_selector.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/templates/semantic-ui/invenio_i18n/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/language_selector.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.571778 invenio-i18n-2.0.0/invenio_i18n/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.583778 invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/invenio_i18n/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.579778 invenio-i18n-2.0.0/invenio_i18n.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3688 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      333 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-02-27 16:57:48.000000 invenio-i18n-2.0.0/invenio_i18n.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/test_babel.py
--rw-r--r--   0 runner    (1001) docker     (122)     7428 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/test_invenio_i18n.py
--rw-r--r--   0 runner    (1001) docker     (122)     4661 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/test_invenio_i18n_selectors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/tests/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/tests/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/tests/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.575778 invenio-i18n-2.0.0/tests/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 16:57:48.587778 invenio-i18n-2.0.0/tests/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-02-27 16:57:45.000000 invenio-i18n-2.0.0/tests/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/i18n-pull-base.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/i18n-push-base.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3803 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10214 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/invenio_i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/app.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/invenio_i18n/assets/semantic-ui/js/invenio_i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/assets/semantic-ui/js/invenio_i18n/app.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/babel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6884 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/templates/invenio_i18n/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/templates/invenio_i18n/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/templates/invenio_i18n/macros/language_selector.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/templates/semantic-ui/invenio_i18n/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/language_selector.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.752637 invenio-i18n-2.1.0/invenio_i18n/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.764637 invenio-i18n-2.1.0/invenio_i18n/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/invenio_i18n/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.760637 invenio-i18n-2.1.0/invenio_i18n.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3803 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-12 08:42:19.000000 invenio-i18n-2.1.0/invenio_i18n.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      339 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-12 08:42:19.772637 invenio-i18n-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/test_babel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/test_invenio_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/test_invenio_i18n_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/tests/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/tests/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/tests/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.756637 invenio-i18n-2.1.0/tests/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:42:19.768637 invenio-i18n-2.1.0/tests/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-12 08:42:06.000000 invenio-i18n-2.1.0/tests/translations/en/LC_MESSAGES/messages.po
```

### Comparing `invenio-i18n-2.0.0/.editorconfig` & `invenio-i18n-2.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/.github/workflows/i18n-push.yml` & `invenio-i18n-2.1.0/.github/workflows/i18n-push-base.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,80 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-i18n is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 name: i18n:push translations
-on: workflow_dispatch # manually trigger
+on:
+  workflow_call:
+    inputs:
+      extract-backend:
+        required: true
+        type: boolean
+        default: true
+      frontend-package-path:
+        required: false
+        type: string
+    secrets:
+      TRANSIFEX_TOKEN:
+        required: true
 
 jobs:
   i18n-extract:
     runs-on: ubuntu-20.04
     env:
       PYTHON-VERSION: 3.9
+      NODE-VERSION: 14.x
     steps:
       - name: Checkout
         uses: actions/checkout@v2
 
       # setup python
       - name: Set up Python ${{ env.PYTHON-VERSION }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ env.PYTHON-VERSION }}
 
       # install dependencies
       - name: Install dependencies
         run: |
-          pip install -e ".[all]"  
+          pip install -e ".[all]"
 
-      # install transifex client
-      - name: transifex-client
-        run: |
-          pip install transifex-client
-
-      # store token
-      - name: store token
-        run: |
-          touch ~/.transifexrc
-          echo [https://www.transifex.com] >> ~/.transifexrc
-          echo api_hostname=https://api.transifex.com >> ~/.transifexrc
-          echo hostname=https://www.transifex.com >> ~/.transifexrc
-          echo password=${{ secrets.TRANSIFEX_TOKEN }} >> ~/.transifexrc
-          echo username=api  >> ~/.transifexrc
-
-      # extract
-      - name: extract_messages
+      # extract backend messages
+      - name: Extract backend messages
+        if: ${{ inputs.extract-backend }}
         run: |
           python setup.py extract_messages
 
-      # push source
-      - name: push_messages
+      # setup node
+      - name: Setup node
+        if: ${{ inputs.frontend-package-path != '' }}
+        uses: actions/setup-node@v3
+        with:
+          node-version: ${{ env.NODE-VERSION }}
+
+      # extract frontend messages
+      - name: Extract frontend messages
+        if: ${{ inputs.frontend-package-path != '' }}
+        working-directory: ./${{ inputs.frontend-package-path }}
+        # installing from package-lock.json
         run: |
-          tx push -s
+          npm ci
+          npm run extract_messages
 
-      # remove transifex credential file
-      - name: remove transifexrc file
-        uses: JesseTG/rm@v1.0.2
+      # Push only source file to transifex
+      - name: Push source file using transifex client
+        uses: transifex/cli-action@v1
         with:
-          path: ~/.transifexrc
+          token: ${{ secrets.TRANSIFEX_TOKEN }}
+          args: push -s
 
       - name: Create Pull Request
         uses: peter-evans/create-pull-request@v3
         with:
           commit-message: i18n:push translations
           title: i18n:push translations
           body: i18n:push translations
-          branch: 101-translations-push  # name of branch which PR is created from
-          delete-branch: true  # delete branch once merged,closed
+          branch: 101-translations-push # name of branch which PR is created from
+          delete-branch: true # delete branch once merged,closed
```

### Comparing `invenio-i18n-2.0.0/.github/workflows/pypi-release.yml` & `invenio-i18n-2.1.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/.github/workflows/tests.yml` & `invenio-i18n-2.1.0/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2020 CERN.
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 name: CI
 
 on:
@@ -56,10 +56,13 @@
 
       - name: Install dependencies
         run: |
           pip install -r .${{matrix.requirements-level}}-${{ matrix.python-version }}-requirements.txt
           pip install -e .[$EXTRAS]
           pip freeze
 
+      - name: Run translations test
+        run: ./run-i18n-tests.sh
+
       - name: Run tests
         run: |
           ./run-tests.sh
```

### Comparing `invenio-i18n-2.0.0/CHANGES.rst` & `invenio-i18n-2.1.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.0 (released 2023-07-12)
+
+- add method to check if locale is available
+
 Version 2.0.0 (released 2023-02-27)
 
 - Remove deprecated flask-babelex
 - Expose LazyString, gettext from flask_babel to invenio
 - Fix get_locale in cli (without request context)
 - Replace set_locale with flask_babel.set_locale
 - Use Multidomain translation in flask_babel context
```

### Comparing `invenio-i18n-2.0.0/CONTRIBUTING.rst` & `invenio-i18n-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/LICENSE` & `invenio-i18n-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/MANIFEST.in` & `invenio-i18n-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/PKG-INFO` & `invenio-i18n-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-i18n
-Version: 2.0.0
+Version: 2.1.0
 Summary: Invenio internationalization (I18N) module.
 Home-page: https://github.com/inveniosoftware/invenio-i18n
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.0 (released 2023-07-12)
+        
+        - add method to check if locale is available
+        
         Version 2.0.0 (released 2023-02-27)
         
         - Remove deprecated flask-babelex
         - Expose LazyString, gettext from flask_babel to invenio
         - Fix get_locale in cli (without request context)
         - Replace set_locale with flask_babel.set_locale
         - Use Multidomain translation in flask_babel context
```

### Comparing `invenio-i18n-2.0.0/README.rst` & `invenio-i18n-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/babel.ini` & `invenio-i18n-2.1.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/docs/Makefile` & `invenio-i18n-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/docs/api.rst` & `invenio-i18n-2.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/docs/conf.py` & `invenio-i18n-2.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,11 +310,15 @@
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/": None}
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/", None),
+    # TODO: Configure external documentation references, eg:
+    # 'Flask-Admin': ('https://flask-admin.readthedocs.io/en/latest/', None),
+}
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-i18n-2.0.0/docs/index.rst` & `invenio-i18n-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/docs/make.bat` & `invenio-i18n-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/__init__.py` & `invenio-i18n-2.1.0/invenio_i18n/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,24 +299,32 @@
     # Werkzeug >=2.1
     import hmac
 
     from werkzeug import security
 
     security.safe_str_cmp = hmac.compare_digest
 
-from flask_babel import Babel, LazyString, get_locale, gettext, lazy_gettext
+from flask_babel import (
+    Babel,
+    LazyString,
+    force_locale,
+    get_locale,
+    gettext,
+    lazy_gettext,
+)
 
 from .ext import InvenioI18N
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 _ = gettext
 
 __all__ = (
     "__version__",
+    "force_locale",
     "InvenioI18N",
     "lazy_gettext",
     "gettext",
     "Babel",
     "_",
     "get_locale",
     "LazyString",
```

#### html2text {}

```diff
@@ -112,11 +112,12 @@
 push -s $ tx pull -a """ # Monkey patch Werkzeug 2.1 # Flask-Login uses the
 safe_str_cmp method which has been removed in Werkzeug # 2.1. Flask-Login
 v0.6.0 (yet to be released at the time of writing) fixes the # issue. Once we
 depend on Flask-Login v0.6.0 as the minimal version in # Flask-Security-
 Invenio/Invenio-Accounts we can remove this patch again. try: # Werkzeug <2.1
 from werkzeug import security security.safe_str_cmp except AttributeError: #
 Werkzeug >=2.1 import hmac from werkzeug import security security.safe_str_cmp
-= hmac.compare_digest from flask_babel import Babel, LazyString, get_locale,
-gettext, lazy_gettext from .ext import InvenioI18N __version__ = "2.0.0" _ =
-gettext __all__ = ( "__version__", "InvenioI18N", "lazy_gettext", "gettext",
-"Babel", "_", "get_locale", "LazyString", )
+= hmac.compare_digest from flask_babel import ( Babel, LazyString,
+force_locale, get_locale, gettext, lazy_gettext, ) from .ext import InvenioI18N
+__version__ = "2.1.0" _ = gettext __all__ = ( "__version__", "force_locale",
+"InvenioI18N", "lazy_gettext", "gettext", "Babel", "_", "get_locale",
+"LazyString", )
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/app.js` & `invenio-i18n-2.1.0/invenio_i18n/assets/bootstrap3/js/invenio_i18n/app.js`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/babel.py` & `invenio-i18n-2.1.0/invenio_i18n/babel.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/config.py` & `invenio-i18n-2.1.0/invenio_i18n/config.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/ext.py` & `invenio-i18n-2.1.0/invenio_i18n/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio internationalization module."""
 
 import json
 import os.path
 
-from babel import Locale
+from babel import Locale, UnknownLocaleError
 from flask import current_app
 from flask_babel import Babel, LazyString
 from flask_babel import get_locale as get_current_locale
 from flask_babel import get_timezone as get_current_timezone
 from werkzeug.local import LocalProxy
 
 from . import config
@@ -170,14 +170,26 @@
             langs = [self.babel.default_locale]
             for lang, dummy_title in current_app.config.get("I18N_LANGUAGES", []):
                 langs.append(Locale.parse(lang))
             self._locales_cache = langs
 
         return self._locales_cache
 
+    def is_locale_available(self, locale):
+        """Check if provided locale is available.
+
+        First parse a locale and then check if it is configured as available.
+        Could be that locale data is available (Locale will not raise) but it
+        is not configured as available in the app.
+        """
+        try:
+            return Locale.parse(locale) in self.get_locales()
+        except (UnknownLocaleError, TypeError):
+            return False
+
     @property
     def locale(self):
         """Get current locale."""
         return get_current_locale()
 
     @property
     def language(self):
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/jinja2.py` & `invenio-i18n-2.1.0/invenio_i18n/jinja2.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/selectors.py` & `invenio-i18n-2.1.0/invenio_i18n/selectors.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/templates/invenio_i18n/macros/language_selector.html` & `invenio-i18n-2.1.0/invenio_i18n/templates/invenio_i18n/macros/language_selector.html`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/language_selector.html` & `invenio-i18n-2.1.0/invenio_i18n/templates/semantic-ui/invenio_i18n/macros/language_selector.html`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/af/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d401 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 fc01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d69 3138 6e20 312e   invenio-i18n 1.
 00000050: 332e 320a 5265 706f 7274 2d4d 7367 6964  3.2.Report-Msgid
 00000060: 2d42 7567 732d 546f 3a20 696e 666f 4069  -Bugs-To: info@i
 00000070: 6e76 656e 696f 736f 6674 7761 7265 2e6f  nveniosoftware.o
 00000080: 7267 0a50 4f54 2d43 7265 6174 696f 6e2d  rg.POT-Creation-
 00000090: 4461 7465 3a20 3230 3232 2d31 302d 3132  Date: 2022-10-12
 000000a0: 2030 393a 3032 2b30 3030 300a 504f 2d52   09:02+0000.PO-R
 000000b0: 6576 6973 696f 6e2d 4461 7465 3a20 3230  evision-Date: 20
 000000c0: 3136 2d30 382d 3235 2030 393a 3136 2b30  16-08-25 09:16+0
 000000d0: 3030 300a 4c61 7374 2d54 7261 6e73 6c61  000.Last-Transla
 000000e0: 746f 723a 2046 554c 4c20 4e41 4d45 203c  tor: FULL NAME <
 000000f0: 454d 4149 4c40 4144 4452 4553 533e 0a4c  EMAIL@ADDRESS>.L
-00000100: 616e 6775 6167 653a 2061 660a 4c61 6e67  anguage: af.Lang
-00000110: 7561 6765 2d54 6561 6d3a 2041 6672 696b  uage-Team: Afrik
-00000120: 6161 6e73 2028 6874 7470 733a 2f2f 7777  aans (https://ww
-00000130: 772e 7472 616e 7369 6665 782e 636f 6d2f  w.transifex.com/
-00000140: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
-00000150: 7465 616d 732f 3233 3533 372f 6166 2f29  teams/23537/af/)
-00000160: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
-00000170: 706c 7572 616c 733d 323b 2070 6c75 7261  plurals=2; plura
-00000180: 6c3d 286e 2021 3d20 3129 3b0a 4d49 4d45  l=(n != 1);.MIME
-00000190: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
-000001a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-000001b0: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
-000001c0: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
-000001d0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
-000001e0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
-000001f0: 4279 3a20 4261 6265 6c20 322e 3131 2e30  By: Babel 2.11.0
-00000200: 0a00                                     ..
+00000100: 616e 6775 6167 653a 2072 6f0a 4c61 6e67  anguage: ro.Lang
+00000110: 7561 6765 2d54 6561 6d3a 2052 6f6d 616e  uage-Team: Roman
+00000120: 6961 6e20 2868 7474 7073 3a2f 2f77 7777  ian (https://www
+00000130: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
+00000140: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
+00000150: 6561 6d73 2f32 3335 3337 2f72 6f2f 290a  eams/23537/ro/).
+00000160: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
+00000170: 6c75 7261 6c73 3d33 3b20 706c 7572 616c  lurals=3; plural
+00000180: 3d28 6e3d 3d31 3f30 3a28 2828 6e25 3130  =(n==1?0:(((n%10
+00000190: 303e 3139 297c 7c28 286e 2531 3030 3d3d  0>19)||((n%100==
+000001a0: 3029 2626 286e 213d 3029 2929 3f32 3a31  0)&&(n!=0)))?2:1
+000001b0: 2929 3b0a 4d49 4d45 2d56 6572 7369 6f6e  ));.MIME-Version
+000001c0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
+000001d0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+000001e0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
+000001f0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
+00000200: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
+00000210: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
+00000220: 6c20 322e 3132 2e31 0a00                 l 2.12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/af/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "اللغة:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 3% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 00000180: 6c3d 286e 2021 3d20 3129 3b0a 4d49 4d45  l=(n != 1);.MIME
 00000190: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
 000001a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 000001b0: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
 000001c0: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
 000001d0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
 000001e0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
-000001f0: 4279 3a20 4261 6265 6c20 322e 3131 2e30  By: Babel 2.11.0
+000001f0: 4279 3a20 4261 6265 6c20 322e 3132 2e31  By: Babel 2.12.1
 00000200: 0a00                                     ..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: ca\n"
 "Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Llengua:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Jazyk:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/da/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/da/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: da\n"
 "Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/"
 "da/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Sprog:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/da/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/de/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/de/LC_MESSAGES/messages.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: de\n"
 "Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Sprache:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/de/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/el/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/en/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/es/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/es/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Idioma:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/es/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/et/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-i18n 1.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:02+0000\n"
-"PO-Revision-Date: 2016-08-25 09:16+0000\n"
-"Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2021\n"
-"Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/et/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
-
-msgid "Language:"
-msgstr "Keel:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/et/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 00000190: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
 000001a0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
 000001b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 000001c0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
 000001d0: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
 000001e0: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
 000001f0: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
-00000200: 793a 2042 6162 656c 2032 2e31 312e 300a  y: Babel 2.11.0.
+00000200: 793a 2042 6162 656c 2032 2e31 322e 310a  y: Babel 2.12.1.
 00000210: 00                                       .
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Langue:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/et/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,18 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-i18n 1.3.2\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:02+0000\n"
+"PO-Revision-Date: 2016-08-25 09:16+0000\n"
+"Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2021\n"
+"Language: et\n"
+"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"teams/23537/et/)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.12.1\n"
+
+msgid "Language:"
+msgstr "Keel:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 000001d0: 323b 0a4d 494d 452d 5665 7273 696f 6e3a  2;.MIME-Version:
 000001e0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
 000001f0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
 00000200: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
 00000210: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
 00000220: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
 00000230: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000240: 2032 2e31 312e 300a 00                    2.11.0..
+00000240: 2032 2e31 322e 310a 00                    2.12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: hu\n"
 "Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Nyelv:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/it/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/it/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Lingua:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/it/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 00000210: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 00000220: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
 00000230: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
 00000240: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
 00000250: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
 00000260: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
 00000270: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000280: 3131 2e30 0a00                           11.0..
+00000280: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/messages.pot` & `invenio-i18n-2.1.0/invenio_i18n/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/no/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/no/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 3% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 00000180: 6c3d 286e 2021 3d20 3129 3b0a 4d49 4d45  l=(n != 1);.MIME
 00000190: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
 000001a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 000001b0: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
 000001c0: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
 000001d0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
 000001e0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
-000001f0: 4279 3a20 4261 6265 6c20 322e 3131 2e30  By: Babel 2.11.0
+000001f0: 4279 3a20 4261 6265 6c20 322e 3132 2e31  By: Babel 2.12.1
 00000200: 0a00                                     ..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/no/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 00000210: 203f 2032 203a 2033 293b 0a4d 494d 452d   ? 2 : 3);.MIME-
 00000220: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
 00000230: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000240: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
 00000250: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
 00000260: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
 00000270: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
-00000280: 793a 2042 6162 656c 2032 2e31 312e 300a  y: Babel 2.11.0.
+00000280: 793a 2042 6162 656c 2032 2e31 322e 310a  y: Babel 2.12.1.
 00000290: 00                                       .
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 000001c0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001d0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
 000001e0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
 000001f0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
 00000200: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
 00000210: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
 00000220: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000230: 3131 2e30 0a00                           11.0..
+00000230: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 fc01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d301 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d69 3138 6e20 312e   invenio-i18n 1.
 00000050: 332e 320a 5265 706f 7274 2d4d 7367 6964  3.2.Report-Msgid
 00000060: 2d42 7567 732d 546f 3a20 696e 666f 4069  -Bugs-To: info@i
 00000070: 6e76 656e 696f 736f 6674 7761 7265 2e6f  nveniosoftware.o
 00000080: 7267 0a50 4f54 2d43 7265 6174 696f 6e2d  rg.POT-Creation-
 00000090: 4461 7465 3a20 3230 3232 2d31 302d 3132  Date: 2022-10-12
 000000a0: 2030 393a 3032 2b30 3030 300a 504f 2d52   09:02+0000.PO-R
 000000b0: 6576 6973 696f 6e2d 4461 7465 3a20 3230  evision-Date: 20
 000000c0: 3136 2d30 382d 3235 2030 393a 3136 2b30  16-08-25 09:16+0
 000000d0: 3030 300a 4c61 7374 2d54 7261 6e73 6c61  000.Last-Transla
 000000e0: 746f 723a 2046 554c 4c20 4e41 4d45 203c  tor: FULL NAME <
 000000f0: 454d 4149 4c40 4144 4452 4553 533e 0a4c  EMAIL@ADDRESS>.L
-00000100: 616e 6775 6167 653a 2072 6f0a 4c61 6e67  anguage: ro.Lang
-00000110: 7561 6765 2d54 6561 6d3a 2052 6f6d 616e  uage-Team: Roman
+00000100: 616e 6775 6167 653a 2067 6c0a 4c61 6e67  anguage: gl.Lang
+00000110: 7561 6765 2d54 6561 6d3a 2047 616c 6963  uage-Team: Galic
 00000120: 6961 6e20 2868 7474 7073 3a2f 2f77 7777  ian (https://www
 00000130: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
 00000140: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
-00000150: 6561 6d73 2f32 3335 3337 2f72 6f2f 290a  eams/23537/ro/).
+00000150: 6561 6d73 2f32 3335 3337 2f67 6c2f 290a  eams/23537/gl/).
 00000160: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
-00000170: 6c75 7261 6c73 3d33 3b20 706c 7572 616c  lurals=3; plural
-00000180: 3d28 6e3d 3d31 3f30 3a28 2828 6e25 3130  =(n==1?0:(((n%10
-00000190: 303e 3139 297c 7c28 286e 2531 3030 3d3d  0>19)||((n%100==
-000001a0: 3029 2626 286e 213d 3029 2929 3f32 3a31  0)&&(n!=0)))?2:1
-000001b0: 2929 3b0a 4d49 4d45 2d56 6572 7369 6f6e  ));.MIME-Version
-000001c0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
-000001d0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
-000001e0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
-000001f0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
-00000200: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
-00000210: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
-00000220: 6c20 322e 3131 2e30 0a00                 l 2.11.0..
+00000170: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
+00000180: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
+00000190: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
+000001a0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001b0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
+000001c0: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
+000001d0: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
+000001e0: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
+000001f0: 793a 2042 6162 656c 2032 2e31 322e 310a  y: Babel 2.12.1.
+00000200: 00                                       .
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 00000210: 3329 3b0a 4d49 4d45 2d56 6572 7369 6f6e  3);.MIME-Version
 00000220: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
 00000230: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
 00000240: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
 00000250: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
 00000260: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
 00000270: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
-00000280: 6c20 322e 3131 2e30 0a00                 l 2.11.0..
+00000280: 6c20 322e 3132 2e31 0a00                 l 2.12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,18 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-i18n 1.3.2\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:02+0000\n"
+"PO-Revision-Date: 2016-08-25 09:16+0000\n"
+"Last-Translator: Kalven Richie, 2022\n"
+"Language: zh_CN\n"
+"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"teams/23537/zh_CN/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.12.1\n"
+
+msgid "Language:"
+msgstr "语言："
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Jazyk:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: sv\n"
 "Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Language:"
 msgstr "Språk:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-i18n 1.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:02+0000\n"
-"PO-Revision-Date: 2016-08-25 09:16+0000\n"
-"Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
-"com>, 2021\n"
-"Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
-"teams/23537/tr/)\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
-
-msgid "Language:"
-msgstr "Dil:"
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 15% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 00000260: 203f 2032 3a20 3329 3b0a 4d49 4d45 2d56   ? 2: 3);.MIME-V
 00000270: 6572 7369 6f6e 3a20 312e 300a 436f 6e74  ersion: 1.0.Cont
 00000280: 656e 742d 5479 7065 3a20 7465 7874 2f70  ent-Type: text/p
 00000290: 6c61 696e 3b20 6368 6172 7365 743d 7574  lain; charset=ut
 000002a0: 662d 380a 436f 6e74 656e 742d 5472 616e  f-8.Content-Tran
 000002b0: 7366 6572 2d45 6e63 6f64 696e 673a 2038  sfer-Encoding: 8
 000002c0: 6269 740a 4765 6e65 7261 7465 642d 4279  bit.Generated-By
-000002d0: 3a20 4261 6265 6c20 322e 3131 2e30 0a00  : Babel 2.11.0..
+000002d0: 3a20 4261 6265 6c20 322e 3132 2e31 0a00  : Babel 2.12.1..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-i18n-2.1.0/invenio_i18n/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-i18n 1.3.2*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 da01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d401 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d69 3138 6e20 312e   invenio-i18n 1.
 00000050: 332e 320a 5265 706f 7274 2d4d 7367 6964  3.2.Report-Msgid
 00000060: 2d42 7567 732d 546f 3a20 696e 666f 4069  -Bugs-To: info@i
 00000070: 6e76 656e 696f 736f 6674 7761 7265 2e6f  nveniosoftware.o
 00000080: 7267 0a50 4f54 2d43 7265 6174 696f 6e2d  rg.POT-Creation-
 00000090: 4461 7465 3a20 3230 3232 2d31 302d 3132  Date: 2022-10-12
 000000a0: 2030 393a 3032 2b30 3030 300a 504f 2d52   09:02+0000.PO-R
 000000b0: 6576 6973 696f 6e2d 4461 7465 3a20 3230  evision-Date: 20
 000000c0: 3136 2d30 382d 3235 2030 393a 3136 2b30  16-08-25 09:16+0
 000000d0: 3030 300a 4c61 7374 2d54 7261 6e73 6c61  000.Last-Transla
 000000e0: 746f 723a 2046 554c 4c20 4e41 4d45 203c  tor: FULL NAME <
 000000f0: 454d 4149 4c40 4144 4452 4553 533e 0a4c  EMAIL@ADDRESS>.L
-00000100: 616e 6775 6167 653a 207a 685f 5457 0a4c  anguage: zh_TW.L
-00000110: 616e 6775 6167 652d 5465 616d 3a20 4368  anguage-Team: Ch
-00000120: 696e 6573 6520 2854 6169 7761 6e29 2028  inese (Taiwan) (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 7a68 5f54 572f 290a 506c  23537/zh_TW/).Pl
-00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
-00000180: 7261 6c73 3d31 3b20 706c 7572 616c 3d30  rals=1; plural=0
-00000190: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
-000001a0: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
-000001b0: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
-000001c0: 6172 7365 743d 7574 662d 380a 436f 6e74  arset=utf-8.Cont
-000001d0: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
-000001e0: 6f64 696e 673a 2038 6269 740a 4765 6e65  oding: 8bit.Gene
-000001f0: 7261 7465 642d 4279 3a20 4261 6265 6c20  rated-By: Babel 
-00000200: 322e 3131 2e30 0a00                      2.11.0..
+00000100: 616e 6775 6167 653a 2061 660a 4c61 6e67  anguage: af.Lang
+00000110: 7561 6765 2d54 6561 6d3a 2041 6672 696b  uage-Team: Afrik
+00000120: 6161 6e73 2028 6874 7470 733a 2f2f 7777  aans (https://ww
+00000130: 772e 7472 616e 7369 6665 782e 636f 6d2f  w.transifex.com/
+00000140: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
+00000150: 7465 616d 732f 3233 3533 372f 6166 2f29  teams/23537/af/)
+00000160: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
+00000170: 706c 7572 616c 733d 323b 2070 6c75 7261  plurals=2; plura
+00000180: 6c3d 286e 2021 3d20 3129 3b0a 4d49 4d45  l=(n != 1);.MIME
+00000190: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
+000001a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000001b0: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
+000001c0: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
+000001d0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
+000001e0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
+000001f0: 4279 3a20 4261 6265 6c20 322e 3132 2e31  By: Babel 2.12.1
+00000200: 0a00                                     ..
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/invenio_i18n/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/views.py` & `invenio-i18n-2.1.0/invenio_i18n/views.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n/webpack.py` & `invenio-i18n-2.1.0/invenio_i18n/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/invenio_i18n.egg-info/PKG-INFO` & `invenio-i18n-2.1.0/invenio_i18n.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-i18n
-Version: 2.0.0
+Version: 2.1.0
 Summary: Invenio internationalization (I18N) module.
 Home-page: https://github.com/inveniosoftware/invenio-i18n
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.0 (released 2023-07-12)
+        
+        - add method to check if locale is available
+        
         Version 2.0.0 (released 2023-02-27)
         
         - Remove deprecated flask-babelex
         - Expose LazyString, gettext from flask_babel to invenio
         - Fix get_locale in cli (without request context)
         - Replace set_locale with flask_babel.set_locale
         - Use Multidomain translation in flask_babel context
```

### Comparing `invenio-i18n-2.0.0/invenio_i18n.egg-info/SOURCES.txt` & `invenio-i18n-2.1.0/invenio_i18n.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
 babel.ini
 pyproject.toml
 requirements-devel.txt
+run-i18n-tests.sh
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/i18n-pull-base.yml
 .github/workflows/i18n-pull.yml
+.github/workflows/i18n-push-base.yml
 .github/workflows/i18n-push.yml
 .github/workflows/pypi-release.yml
 .github/workflows/tests.yml
 .tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
@@ -33,14 +36,15 @@
 docs/requirements.txt
 docs/usage.rst
 invenio_i18n/__init__.py
 invenio_i18n/babel.py
 invenio_i18n/config.py
 invenio_i18n/ext.py
 invenio_i18n/jinja2.py
+invenio_i18n/proxies.py
 invenio_i18n/selectors.py
 invenio_i18n/views.py
 invenio_i18n/webpack.py
 invenio_i18n.egg-info/PKG-INFO
 invenio_i18n.egg-info/SOURCES.txt
 invenio_i18n.egg-info/dependency_links.txt
 invenio_i18n.egg-info/entry_points.txt
```

### Comparing `invenio-i18n-2.0.0/run-tests.sh` & `invenio-i18n-2.1.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/setup.cfg` & `invenio-i18n-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/tests/test_babel.py` & `invenio-i18n-2.1.0/tests/test_babel.py`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/tests/test_invenio_i18n.py` & `invenio-i18n-2.1.0/tests/test_invenio_i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Basic tests."""
 
 from datetime import datetime
 from os.path import dirname, join
 
+from babel import Locale
 from flask import render_template_string
 from flask_babel import (
-    _get_current_context,
     force_locale,
     format_datetime,
     format_number,
     get_locale,
     gettext,
     lazy_gettext,
 )
@@ -89,31 +89,32 @@
 
 def test_timezone_selector(app):
     """Test format_datetime."""
     app.config["I18N_LANGUAGES"] = [("da", "Danish")]
     InvenioI18N(app)
     with app.test_request_context():
         assert (
-            format_datetime(datetime(1987, 3, 5, 17, 12)) == "Mar 5, 1987, 5:12:00 PM"
+            format_datetime(datetime(1987, 3, 5, 17, 12))
+            == "Mar 5, 1987, 5:12:00\u202fPM"
         )
         # Adds the new date format due to a library update 2
         assert format_datetime(datetime(1987, 3, 5, 17, 12), "full") in [
-            "Thursday, March 5, 1987 at 5:12:00 PM GMT+00:00",
-            "Thursday, March 5, 1987 at 5:12:00 PM Coordinated Universal Time",
+            "Thursday, March 5, 1987, 5:12:00\u202fPM GMT+00:00",
+            "Thursday, March 5, 1987, 5:12:00\u202fPM Coordinated Universal Time",
         ]
         assert (
-            format_datetime(datetime(1987, 3, 5, 17, 12), "short") == "3/5/87, 5:12 PM"
+            format_datetime(datetime(1987, 3, 5, 17, 12), "short")
+            == "3/5/87, 5:12\u202fPM"
         )
         assert (
             format_datetime(datetime(1987, 3, 5, 17, 12), "dd mm yyy") == "05 12 1987"
         )
         assert (
             format_datetime(datetime(1987, 3, 5, 17, 12), "dd mm yyyy") == "05 12 1987"
         )
-    _get_current_context().babel_locale = None
 
     with app.test_request_context(headers=[("Accept-Language", "da")]):
         assert str(get_locale()) == "da"
         assert (
             format_datetime(datetime(1987, 3, 5, 17, 12), "short") == "05.03.1987 17.12"
         )
 
@@ -126,15 +127,14 @@
     )
 
     with app.test_request_context(headers=[("Accept-Language", "da")]):
         InvenioI18N(app)
         assert str(get_locale()) == "da"
         assert format_number(10.1) == "10,1"
         assert gettext("Translate") == "Oversætte"
-    _get_current_context().babel_locale = None
 
     with app.test_request_context(headers=[("Accept-Language", "en")]):
         InvenioI18N(app)
         assert str(get_locale()) == "en"
         assert format_number(10.1) == "10.1"
         assert gettext("Translate") == "From test catalog"
 
@@ -144,31 +144,50 @@
     app.config["I18N_LANGUAGES"] = [("da", "Danish")]
     i18n = InvenioI18N(app)
 
     with app.app_context():
         assert [str(lang) for lang in i18n.get_locales()] == ["en", "da"]
 
 
+def test_is_locale_available(app):
+    """Test checking if provided locale is available."""
+    app.config["I18N_LANGUAGES"] = [("da", "Danish")]
+    i18n = InvenioI18N(app)
+
+    # default locale
+    assert i18n.is_locale_available("en")
+    # additional locale
+    assert i18n.is_locale_available("da")
+    # valid locale but it is not configured
+    assert Locale.parse("es")
+    assert not i18n.is_locale_available("es")
+    # locale for which no translations are available
+    assert not i18n.is_locale_available("de_AT")
+    # false value passed
+    for v in ["no_loc-ale", {"de"}, ["de"], 42, None, {}]:
+        assert not i18n.is_locale_available(v)
+
+
 def test_current_i18n(app):
     """Test getting locales."""
     app.config["I18N_LANGUAGES"] = [("da", "Danish"), ("ar", "Arabic")]
     InvenioI18N(app)
 
     with app.test_request_context(headers=[("Accept-Language", "da")]):
         assert current_i18n.language == "da"
         assert str(current_i18n.locale) == "da"
         assert str(current_i18n.timezone) == "UTC"
         assert current_i18n.locale.text_direction == "ltr"
-    _get_current_context().babel_locale = None
+
     with app.test_request_context(headers=[("Accept-Language", "en")]):
         assert current_i18n.language == "en"
         assert str(current_i18n.locale) == "en"
         assert str(current_i18n.timezone) == "UTC"
         assert current_i18n.locale.text_direction == "ltr"
-    _get_current_context().babel_locale = None
+
     with app.test_request_context(headers=[("Accept-Language", "ar")]):
         assert current_i18n.language == "ar"
         assert str(current_i18n.locale) == "ar"
         assert str(current_i18n.timezone) == "UTC"
         assert current_i18n.locale.text_direction == "rtl"
 
 
@@ -182,15 +201,15 @@
 
     dt = datetime(1987, 3, 5, 17, 12)
     dt_tz = datetime(1987, 3, 5, 17, 12, tzinfo=timezone("CET"))
 
     with app.test_request_context():
         assert (
             render_template_string("{{dt|datetimeformat}}", dt=dt)
-            == "Mar 5, 1987, 5:12:00 PM"
+            == "Mar 5, 1987, 5:12:00\u202fPM"
         )
         assert render_template_string("{{dt|toutc}}", dt=dt_tz) == "1987-03-05 16:12:00"
         assert (
             render_template_string("{{dt|tousertimezone}}", dt=dt_tz)
             == "1987-03-05 16:12:00+00:00"
         )
         assert render_template_string('{{_("Translate")}}') == "Translate"
```

### Comparing `invenio-i18n-2.0.0/tests/test_invenio_i18n_selectors.py` & `invenio-i18n-2.1.0/tests/test_invenio_i18n_selectors.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Selector tests."""
 
 from os.path import dirname, join
 
-from flask import g, session
+from flask import session
 from flask_babel import gettext
 from flask_login import LoginManager, login_user
 
 from invenio_i18n import InvenioI18N
 from invenio_i18n.selectors import get_locale
 
 
@@ -38,22 +38,25 @@
     app.config["I18N_LANGUAGES"] = [
         ("da", "Danish"),
         ("en", "English"),
         ("es", "Spanish"),
     ]
     InvenioI18N(app)
 
-    with app.test_request_context("/?ln=da"):
-        assert "da" == get_locale()
-
     with app.test_request_context("/?ln=en"):
         assert "en" == get_locale()
+        assert gettext("Language:") == "Language:"
+
+    with app.test_request_context("/?ln=da"):
+        assert "da" == get_locale()
+        assert gettext("Language:") == "Sprog:"
 
     with app.test_request_context("/?ln=es"):
         assert "es" == get_locale()
+        assert gettext("Language:") == "Idioma:"
 
 
 def test_get_locale_session(app):
     """Test getting locales from the current session."""
     app.config["I18N_LANGUAGES"] = [
         ("da", "Danish"),
         ("en", "English"),
@@ -89,25 +92,19 @@
     login_manager.login_view = "login"
     InvenioI18N(app)
     with app.test_request_context():
         login_user(FakeUser("da"))
         assert "da" == get_locale()
         assert gettext("Language:") == "Sprog:"
 
-    # the context will not the reseted with a `with` statement, therefore the
-    # babel_locale within that context remains, which leads to the problem
-    g._flask_babel.babel_locale = None
-
     with app.test_request_context():
         login_user(FakeUser("en"))
         assert "en" == get_locale()
         assert gettext("Language:") == "Language:"
 
-    g._flask_babel.babel_locale = None
-
     with app.test_request_context():
         login_user(FakeUser("es"))
         assert "es" == get_locale()
         assert gettext("Language:") == "Idioma:"
 
 
 def test_get_locale_headers(app):
@@ -122,22 +119,18 @@
     )
     InvenioI18N(app)
 
     with app.test_request_context(headers=[("Accept-Language", "da")]):
         assert "da" == get_locale()
         assert gettext("Translate") == "Oversætte"
 
-    g._flask_babel.babel_locale = None
-
     with app.test_request_context(headers=[("Accept-Language", "en")]):
         assert "en" == get_locale()
         assert gettext("Language:") == "Language:"
 
-    g._flask_babel.babel_locale = None
-
     with app.test_request_context(headers=[("Accept-Language", "es")]):
         assert "es" == get_locale()
         assert gettext("Language:") == "Idioma:"
 
 
 def test_get_locale_default(app):
     """Test getting locale by default."""
```

### Comparing `invenio-i18n-2.0.0/tests/test_views.py` & `invenio-i18n-2.1.0/tests/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Basic tests."""
 
 from flask import session, url_for
-from flask_babel import _get_current_context, get_locale
+from flask_babel import get_locale
 
 from invenio_i18n import InvenioI18N
 from invenio_i18n.views import create_blueprint_from_app
 
 
 def test_lang_view(app):
     """Test extension initalization."""
@@ -48,16 +49,15 @@
 
         # Set language to english
         res = client.get(en_lang_url)
         assert res.status_code == 302
         assert res.location == "/"
         assert session[app.config["I18N_SESSION_KEY"]] == "en"
 
-        _get_current_context().babel_locale = None
-
+    with app.test_client() as client:
         res = client.get("/")
         assert res.get_data(as_text=True) == "en"
 
         # Try to set invalid language.
         res = client.get(es_lang_url)
         assert res.status_code == 404
```

### Comparing `invenio-i18n-2.0.0/tests/translations/da/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/tests/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-i18n-2.0.0/tests/translations/en/LC_MESSAGES/messages.po` & `invenio-i18n-2.1.0/tests/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

