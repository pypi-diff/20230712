# Comparing `tmp/invenio-webhooks-1.0.0a4.tar.gz` & `tmp/invenio-webhooks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-webhooks-1.0.0a4.tar", last modified: Mon Oct  3 14:28:04 2016, max compression
+gzip compressed data, was "dist/invenio-webhooks-1.0.1.tar", last modified: Wed Jul 12 08:37:01 2023, max compression
```

## Comparing `invenio-webhooks-1.0.0a4.tar` & `invenio-webhooks-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,94 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/.tx/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1801 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.tx/config
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/docs/
--rw-rw-r--   0 travis    (1000) travis    (1000)     7449 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/Makefile
--rw-rw-r--   0 travis    (1000) travis    (1000)     1412 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/api.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/authors.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/changes.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    10729 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/conf.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1013 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/contributing.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1573 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/index.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/installation.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      867 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/license.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     7001 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/make.bat
--rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     1026 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/usage.rst
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/examples/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1409 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/examples/app.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      829 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      803 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      803 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      804 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      912 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      910 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/LC_MESSAGES/messages.po
--rw-rw-r--   0 travis    (1000) travis    (1000)      740 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/messages.pot
--rw-rw-r--   0 travis    (1000) travis    (1000)     1311 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1192 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/config.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2882 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/ext.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7631 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1170 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/proxies.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1941 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/signatures.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1193 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/version.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3397 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/views.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4818 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     1524 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      369 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-10-03 14:27:32.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)      692 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/tests/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4748 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/conftest.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6196 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_api.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1975 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_invenio_webhooks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5788 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_receivers.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      124 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.dockerignore
--rw-rw-r--   0 travis    (1000) travis    (1000)     1588 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.editorconfig
--rw-rw-r--   0 travis    (1000) travis    (1000)       60 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.lgtm
--rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-devel-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-lowest-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-release-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     1335 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/AUTHORS.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1142 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/CHANGES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     3482 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)       26 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/INSTALL.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    18092 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/LICENSE
--rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/MAINTAINERS
--rw-rw-r--   0 travis    (1000) travis    (1000)     1703 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     1997 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      771 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/RELEASE-NOTES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1289 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/babel.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1061 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/pytest.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1245 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/requirements-devel.txt
--rwxrwxr-x   0 travis    (1000) travis    (1000)     1222 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/run-tests.sh
--rw-rw-r--   0 travis    (1000) travis    (1000)      674 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)     3937 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4818 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.lgtm
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4989 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10777 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/alembic/469925575192_create_webhooks_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/alembic/a095bd179f5c_create_webhooks_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9374 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/invenio_webhooks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4989 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/invenio_webhooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      787 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:37:01.000000 invenio-webhooks-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     5164 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9722 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/tests/test_invenio_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-07-12 08:36:53.000000 invenio-webhooks-1.0.1/tests/test_receivers.py
```

### Comparing `invenio-webhooks-1.0.0a4/.tx/config` & `invenio-webhooks-1.0.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/Makefile` & `invenio-webhooks-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/api.rst` & `invenio-webhooks-1.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/authors.rst` & `invenio-webhooks-1.0.1/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/changes.rst` & `invenio-webhooks-1.0.1/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/conf.py` & `invenio-webhooks-1.0.1/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,317 +18,322 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
+"""Sphinx configuration."""
+
 from __future__ import print_function
 
 import os
 
 import sphinx.environment
 
+from invenio_webhooks import __version__
+
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Do not warn on external images.
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Invenio-Webhooks'
-copyright = u'2015, CERN'
-author = u'CERN'
+project = "Invenio-Webhooks"
+copyright = "2015, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
-# Get the version string. Cannot be done with import!
-g = {}
-with open(os.path.join('..', 'invenio_webhooks', 'version.py'), 'rt') as fp:
-    exec(fp.read(), g)
-    version = g['__version__']
-
 # The full version, including alpha/beta/rc tags.
-release = version
+release = __version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
-    'description': 'Invenio module for processing webhook events.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'invenio-webhooks',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'invenio-webhooks@GitHub': 'https://github.com/inveniosoftware/invenio-webhooks',
-        'invenio-webhooks@PyPI': 'https://pypi.python.org/pypi/invenio-webhooks/',
-    }
+    "description": "Invenio module for processing webhook events.",
+    "github_user": "inveniosoftware",
+    "github_repo": "invenio-webhooks",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "invenio-webhooks@GitHub": "https://github.com/inveniosoftware/invenio-webhooks",
+        "invenio-webhooks@PyPI": "https://pypi.python.org/pypi/invenio-webhooks/",
+    },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "relations.html",
+        "searchbox.html",
+        "donate.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'invenio-webhooks_namedoc'
+htmlhelp_basename = "invenio-webhooks_namedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'invenio-webhooks.tex', u'invenio-webhooks Documentation',
-   u'CERN', 'manual'),
+    (
+        master_doc,
+        "invenio-webhooks.tex",
+        "invenio-webhooks Documentation",
+        "CERN",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'invenio-webhooks', u'invenio-webhooks Documentation',
-     [author], 1)
+    (master_doc, "invenio-webhooks", "invenio-webhooks Documentation", [author], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'invenio-webhooks', u'Invenio-Webhooks Documentation',
-   author, 'invenio-webhooks', 'Invenio module for processing webhook events.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "invenio-webhooks",
+        "Invenio-Webhooks Documentation",
+        author,
+        "invenio-webhooks",
+        "Invenio module for processing webhook events.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {"https://docs.python.org/": None}
 
 # Autodoc configuraton.
-autoclass_content = 'both'
+autoclass_content = "both"
```

### Comparing `invenio-webhooks-1.0.0a4/docs/contributing.rst` & `invenio-webhooks-1.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/index.rst` & `invenio-webhooks-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/installation.rst` & `invenio-webhooks-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/license.rst` & `invenio-webhooks-1.0.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/make.bat` & `invenio-webhooks-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/docs/usage.rst` & `invenio-webhooks-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/examples/app.py` & `invenio-webhooks-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015 CERN.
+# Copyright (C) 2015-2022 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,32 +18,12 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
+"""Invenio module for processing webhook events."""
 
-"""Minimal Flask application example for development.
+from setuptools import setup
 
-Run example development server:
-
-.. code-block:: console
-
-   $ cd examples
-   $ python app.py
-"""
-
-from __future__ import absolute_import, print_function
-
-from flask import Flask
-from flask_babelex import Babel
-
-from invenio_webhooks import InvenioWebhooks
-
-# Create Flask application
-app = Flask(__name__)
-Babel(app)
-InvenioWebhooks(app)
-
-if __name__ == "__main__":
-    app.run()
+setup()
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/messages.pot` & `invenio-webhooks-1.0.1/invenio_webhooks/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/__init__.py` & `invenio-webhooks-1.0.1/invenio_webhooks/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module for processing webhook events."""
 
-from __future__ import absolute_import, print_function
-
 from .ext import InvenioWebhooks
 from .models import Receiver
 from .proxies import current_webhooks
-from .version import __version__
+
+__version__ = "1.0.1"
 
 __all__ = (
-    '__version__',
-    'current_webhooks',
-    'InvenioWebhooks',
-    'Receiver',
+    "__version__",
+    "current_webhooks",
+    "InvenioWebhooks",
+    "Receiver",
 )
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/config.py` & `invenio-webhooks-1.0.1/invenio_webhooks/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 .. code-block:: python
 
     WEBHOOKS_DEBUG_RECEIVER_URLS = {
         'github': 'https://hook.user.ultrahook.com/?access_token=%%(token)s'
     }
 """
 
-WEBHOOKS_SECRET_KEY = 'secret_key'
+WEBHOOKS_SECRET_KEY = "secret_key"
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/ext.py` & `invenio-webhooks-1.0.1/invenio_webhooks/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module for processing webhook events."""
 
-from __future__ import absolute_import, print_function
-
 import pkg_resources
 
 from . import config
 
 
 class _WebhooksState(object):
     """Webhooks state storing registered receivers."""
@@ -61,23 +59,23 @@
     """Invenio-Webhooks extension."""
 
     def __init__(self, app=None, **kwargs):
         """Extension initialization."""
         if app:
             self.init_app(app, **kwargs)
 
-    def init_app(self, app, entry_point_group='invenio_webhooks.receivers'):
+    def init_app(self, app, entry_point_group="invenio_webhooks.receivers"):
         """Flask application initialization."""
         self.init_config(app)
         state = _WebhooksState(app, entry_point_group=entry_point_group)
-        self._state = app.extensions['invenio-webhooks'] = state
+        self._state = app.extensions["invenio-webhooks"] = state
 
     def init_config(self, app):
         """Initialize configuration."""
         app.config.setdefault(
-            'WEBHOOKS_BASE_TEMPLATE',
-            app.config.get('BASE_TEMPLATE',
-                           'invenio_webhooks/base.html'))
+            "WEBHOOKS_BASE_TEMPLATE",
+            app.config.get("BASE_TEMPLATE", "invenio_webhooks/base.html"),
+        )
 
         for k in dir(config):
-            if k.startswith('WEBHOOKS_'):
+            if k.startswith("WEBHOOKS_"):
                 app.config.setdefault(k, getattr(config, k))
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/models.py` & `invenio-webhooks-1.0.1/invenio_webhooks/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,76 +20,71 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Models for webhook receivers."""
 
-from __future__ import absolute_import
-
 import re
 import uuid
 
-from celery import shared_task
+from celery import shared_task, states
+from celery.result import AsyncResult
 from flask import current_app, request, url_for
 from invenio_accounts.models import User
 from invenio_db import db
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.orm import validates
-from sqlalchemy_utils.models import Timestamp
-from sqlalchemy_utils.types import JSONType, UUIDType
+from sqlalchemy.orm.attributes import flag_modified
+from sqlalchemy_utils import JSONType, Timestamp, UUIDType
 
 from . import signatures
+from ._compat import delete_cached_json_for
+from .errors import InvalidPayload, InvalidSignature, ReceiverDoesNotExist
 from .proxies import current_webhooks
 
 
 #
-# Errors
-#
-class WebhookError(Exception):
-    """General webhook error."""
-
-
-class ReceiverDoesNotExist(WebhookError):
-    """Raised when receiver does not exist."""
-
-
-class InvalidPayload(WebhookError):
-    """Raised when the payload is invalid."""
-
-
-class InvalidSignature(WebhookError):
-    """Raised when the signature does not match."""
-
-
-#
 # Models
 #
 class Receiver(object):
     """Base class for a webhook receiver.
 
     A receiver is responsible for receiving and extracting a payload from a
     request. You must implement ``run`` method that accepts the event
     instance.
     """
 
-    signature = ''
+    signature = ""
     """Default signature."""
 
     def __init__(self, receiver_id):
         """Initialize a receiver identifier."""
         self.receiver_id = receiver_id
 
     def __call__(self, event):
         """Proxy to ``self.run`` method."""
         return self.run(event)
 
     def run(self, event):
         """Implement method accepting the ``Event`` instance."""
-        raise NotImplemented()
+        raise NotImplementedError()
+
+    def status(self, event):
+        """Return a tuple with current processing status code and message.
+
+        Return ``None`` if the backend does not support states.
+        """
+        pass
+
+    def delete(self, event):
+        """Mark event as deleted."""
+        assert self.receiver_id == event.receiver_id
+        event.response = {"status": 410, "message": "Gone."}
+        event.response_code = 410
 
     def get_hook_url(self, access_token):
         """Get URL for webhook.
 
         In debug and testing mode the hook URL can be overwritten using
         ``WEBHOOKS_DEBUG_RECEIVER_URLS`` configuration variable to allow
         testing webhooks via services such as e.g. Ultrahook.
@@ -97,94 +92,131 @@
         .. code-block:: python
 
             WEBHOOKS_DEBUG_RECEIVER_URLS = dict(
                 github='http://github.userid.ultrahook.com',
             )
         """
         # Allow overwriting hook URL in debug mode.
-        if (current_app.debug or current_app.testing) and \
-           current_app.config.get('WEBHOOKS_DEBUG_RECEIVER_URLS', None):
-            url_pattern = current_app.config[
-                'WEBHOOKS_DEBUG_RECEIVER_URLS'].get(self.receiver_id, None)
+        if (current_app.debug or current_app.testing) and current_app.config.get(
+            "WEBHOOKS_DEBUG_RECEIVER_URLS", None
+        ):
+            url_pattern = current_app.config["WEBHOOKS_DEBUG_RECEIVER_URLS"].get(
+                self.receiver_id, None
+            )
             if url_pattern:
                 return url_pattern % dict(token=access_token)
         return url_for(
-            'invenio_webhooks.event_list',
+            "invenio_webhooks.event_list",
             receiver_id=self.receiver_id,
             access_token=access_token,
-            _external=True
+            _external=True,
         )
 
     #
     # Instance methods (override if needed)
     #
     def check_signature(self):
         """Check signature of signed request."""
         if not self.signature:
             return True
         signature_value = request.headers.get(self.signature, None)
         if signature_value:
-            validator = 'check_' + re.sub(r'[-]', '_', self.signature).lower()
+            validator = "check_" + re.sub(r"[-]", "_", self.signature).lower()
             check_signature = getattr(signatures, validator)
             if check_signature(signature_value, request.data):
                 return True
         return False
 
     def extract_payload(self):
         """Extract payload from request."""
         if not self.check_signature():
-            raise InvalidSignature('Invalid Signature')
-        if request.content_type == 'application/json':
-            return request.get_json()
-        elif request.content_type == 'application/x-www-form-urlencoded':
+            raise InvalidSignature("Invalid Signature")
+        if request.is_json:
+            # Request.get_json() could be first called with silent=True.
+            delete_cached_json_for(request)
+            return request.get_json(silent=False, cache=False)
+        elif request.content_type == "application/x-www-form-urlencoded":
             return dict(request.form)
         raise InvalidPayload(request.content_type)
 
 
-@shared_task(ignore_results=True)
-def process_event(event_id):
+@shared_task(bind=True, ignore_results=True)
+def process_event(self, event_id):
     """Process event in Celery."""
     with db.session.begin_nested():
         event = Event.query.get(event_id)
-        event.receiver.run(event)  # call run directly to avoild circular calls
+        event._celery_task = self  # internal binding to a Celery task
+        event.receiver.run(event)  # call run directly to avoid circular calls
+        flag_modified(event, "response")
+        flag_modified(event, "response_headers")
         db.session.add(event)
     db.session.commit()
 
 
 class CeleryReceiver(Receiver):
     """Asynchronous receiver.
 
     Receiver which will fire a celery task to handle payload instead of running
     it synchronously during the request.
     """
 
+    CELERY_STATES_TO_HTTP = {
+        states.PENDING: 202,
+        states.STARTED: 202,
+        states.RETRY: 202,
+        states.FAILURE: 500,
+        states.SUCCESS: 201,
+    }
+    """Mapping of Celery result states to HTTP codes."""
+
+    CELERY_RESULT_INFO_FOR = {
+        states.PENDING,
+        states.STARTED,
+    }
+    """Celery states in which the task's status is reported."""
+
     def __call__(self, event):
         """Fire a celery task."""
-        process_event.apply_async(args=[event.id])
+        process_event.apply_async(task_id=str(event.id), args=[str(event.id)])
+
+    def status(self, event):
+        """Return a tuple with current processing status code and message."""
+        result = AsyncResult(str(event.id))
+        return (
+            self.CELERY_STATES_TO_HTTP.get(result.state),
+            result.info.get("message")
+            if result.state in self.CELERY_RESULT_INFO_FOR and result.info
+            else event.response.get("message"),
+        )
+
+    def delete(self, event):
+        """Abort running task if it exists."""
+        super(CeleryReceiver, self).delete(event)
+        AsyncResult(event.id).revoke(terminate=True)
 
 
 def _json_column(**kwargs):
     """Return JSON column."""
     return db.Column(
         JSONType().with_variant(
             postgresql.JSON(none_as_null=True),
-            'postgresql',
+            "postgresql",
         ),
         nullable=True,
         **kwargs
     )
 
 
 class Event(db.Model, Timestamp):
     """Incoming webhook event data.
 
     Represents webhook event data which consists of a payload and a user id.
     """
 
-    __tablename__ = 'webhooks_events'
+    __tablename__ = "webhooks_events"
 
     id = db.Column(
         UUIDType,
         primary_key=True,
         default=uuid.uuid4,
     )
     """Event identifier."""
@@ -201,25 +233,23 @@
 
     payload = _json_column()
     """Store payload in JSON format."""
 
     payload_headers = _json_column()
     """Store payload headers in JSON format."""
 
-    response = _json_column(
-        default=lambda: {'status': 202, 'message': 'Accepted.'}
-    )
+    response = _json_column(default=lambda: {"status": 202, "message": "Accepted."})
     """Store response in JSON format."""
 
     response_headers = _json_column()
     """Store response headers in JSON format."""
 
     response_code = db.Column(db.Integer, default=202)
 
-    @validates('receiver_id')
+    @validates("receiver_id")
     def validate_receiver(self, key, value):
         """Validate receiver identifier."""
         if value not in current_webhooks.receivers:
             raise ReceiverDoesNotExist(self.receiver_id)
         return value
 
     @classmethod
@@ -243,13 +273,21 @@
         assert isinstance(value, Receiver)
         self.receiver_id = value.receiver_id
 
     def process(self):
         """Process current event."""
         try:
             self.receiver(self)
-        # TODO RESTException
         except Exception as e:
-            current_app.logger.exception('Could not process event.')
-            self.response_code = 500
-            self.response = dict(status=500, message=str(e))
+            current_app.logger.exception("Could not process event.")
+            raise
         return self
+
+    @property
+    def status(self):
+        """Return a tuple with current processing status code and message."""
+        status = self.receiver.status(self)
+        return status if status else (self.response_code, self.response.get("message"))
+
+    def delete(self):
+        """Make receiver delete this event."""
+        self.receiver.delete(self)
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/proxies.py` & `invenio-webhooks-1.0.1/invenio_webhooks/proxies.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,10 +23,8 @@
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Helper proxy to the state object."""
 
 from flask import current_app
 from werkzeug.local import LocalProxy
 
-current_webhooks = LocalProxy(
-    lambda: current_app.extensions['invenio-webhooks']
-)
+current_webhooks = LocalProxy(lambda: current_app.extensions["invenio-webhooks"])
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/signatures.py` & `invenio-webhooks-1.0.1/invenio_webhooks/signatures.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 
 
 def get_hmac(message):
     """Calculate HMAC value of message using ``WEBHOOKS_SECRET_KEY``.
 
     :param message: String to calculate HMAC for.
     """
-    key = current_app.config['WEBHOOKS_SECRET_KEY']
+    key = current_app.config["WEBHOOKS_SECRET_KEY"]
     hmac_value = hmac.new(
-        key.encode('utf-8') if hasattr(key, 'encode') else key,
-        message.encode('utf-8') if hasattr(message, 'encode') else message,
-        sha1
+        key.encode("utf-8") if hasattr(key, "encode") else key,
+        message.encode("utf-8") if hasattr(message, "encode") else message,
+        sha1,
     ).hexdigest()
     return hmac_value
 
 
 def check_x_hub_signature(signature, message):
     """Check X-Hub-Signature used by GitHub to sign requests.
 
     :param signature: HMAC signature extracted from request.
     :param message: Request message.
     """
     hmac_value = get_hmac(message)
-    if hmac_value == signature or \
-       (signature.find('=') > -1 and
-            hmac_value == signature[signature.find('=') + 1:]):
+    if hmac_value == signature or (
+        signature.find("=") > -1 and hmac_value == signature[signature.find("=") + 1 :]
+    ):
         return True
     return False
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks/version.py` & `invenio-webhooks-1.0.1/invenio_webhooks/alembic/469925575192_create_webhooks_branch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015, 2016 CERN.
+# Copyright (C) 2016 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,16 +17,27 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-"""Version information for Invenio-Webhooks.
+"""Create webhooks branch."""
 
-This file is imported by ``invenio_webhooks.__init__``,
-and parsed by ``setup.py``.
-"""
+import sqlalchemy as sa
+from alembic import op
 
-from __future__ import absolute_import, print_function
+# revision identifiers, used by Alembic.
+revision = "469925575192"
+down_revision = "12a88921ada2"
+branch_labels = ("invenio_webhooks",)
+depends_on = "dbdbc1b19cf2"
 
-__version__ = "1.0.0a4"
+
+def upgrade():
+    """Upgrade database."""
+    pass
+
+
+def downgrade():
+    """Downgrade database."""
+    pass
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/PKG-INFO` & `invenio-webhooks-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: invenio-webhooks
-Version: 1.0.0a4
-Summary: Invenio module for processing webhook events.
+Version: 1.0.1
+Summary: "Invenio webhooks module to create REST APIs."
 Home-page: https://github.com/inveniosoftware/invenio-webhooks
 Author: CERN
 Author-email: info@inveniosoftware.org
-License: GPLv2
+License: MIT
 Description: ..
             This file is part of Invenio.
             Copyright (C) 2015 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
@@ -29,16 +29,16 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         ==================
          Invenio-Webhooks
         ==================
         
-        .. image:: https://img.shields.io/travis/inveniosoftware/invenio-webhooks.svg
-                :target: https://travis-ci.org/inveniosoftware/invenio-webhooks
+        .. image:: https://github.com/inveniosoftware/invenio-webhooks/workflows/CI/badge.svg
+                :target: https://github.com/inveniosoftware/invenio-webhooks/actions?query=workflow%3ACI
         
         .. image:: https://img.shields.io/coveralls/inveniosoftware/invenio-webhooks.svg
                 :target: https://coveralls.io/r/inveniosoftware/invenio-webhooks
         
         .. image:: https://img.shields.io/github/tag/inveniosoftware/invenio-webhooks.svg
                 :target: https://github.com/inveniosoftware/invenio-webhooks/releases
         
@@ -49,18 +49,17 @@
                 :target: https://github.com/inveniosoftware/invenio-webhooks/blob/master/LICENSE
         
         
         Invenio module for processing webhook events.
         
         *This is an experimental developer preview release.*
         
-        * Free software: GPLv2 license
+        * Free software: MIT license
         * Documentation: https://invenio-webhooks.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
             Copyright (C) 2015, 2016 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
@@ -79,30 +78,39 @@
             In applying this license, CERN does not
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         Changes
         =======
         
+        Version 1.0.1 (release 2023-07-12)
+        
+        - add event error handling
+        
+        Version 1.0.0 (release 2023-07-03)
+        
+        - v1.0.0 release
+        
         Version 1.0.0a4 (release 2016-10-03)
         
         - Port to new structure for Invenio 3.
         
         Version 0.1.0 (release 2015-08-05)
         
         - Initial public release.
         
 Keywords: invenio webhooks
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 1 - Planning
+Requires-Python: >=3.7
+Provides-Extra: tests
```

### Comparing `invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/SOURCES.txt` & `invenio-webhooks-1.0.1/invenio_webhooks.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 .dockerignore
 .editorconfig
+.git-blame-ignore-revs
 .lgtm
-.travis-devel-requirements.txt
-.travis-lowest-requirements.txt
-.travis-release-requirements.txt
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MAINTAINERS
 MANIFEST.in
 README.rst
 RELEASE-NOTES.rst
 babel.ini
-pytest.ini
+constraints-pypi.txt
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/pypi-publish.yml
+.github/workflows/tests.yml
 .tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
@@ -30,32 +30,41 @@
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
 examples/app.py
 invenio_webhooks/__init__.py
+invenio_webhooks/_compat.py
 invenio_webhooks/config.py
+invenio_webhooks/errors.py
 invenio_webhooks/ext.py
 invenio_webhooks/models.py
 invenio_webhooks/proxies.py
 invenio_webhooks/signatures.py
-invenio_webhooks/version.py
 invenio_webhooks/views.py
 invenio_webhooks.egg-info/PKG-INFO
 invenio_webhooks.egg-info/SOURCES.txt
 invenio_webhooks.egg-info/dependency_links.txt
 invenio_webhooks.egg-info/entry_points.txt
 invenio_webhooks.egg-info/not-zip-safe
 invenio_webhooks.egg-info/requires.txt
 invenio_webhooks.egg-info/top_level.txt
+invenio_webhooks/alembic/469925575192_create_webhooks_branch.py
+invenio_webhooks/alembic/a095bd179f5c_create_webhooks_tables.py
 invenio_webhooks/translations/messages.pot
+invenio_webhooks/translations/cs/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/cs/LC_MESSAGES/messages.po
+invenio_webhooks/translations/da/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/da/LC_MESSAGES/messages.po
+invenio_webhooks/translations/de/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/de/LC_MESSAGES/messages.po
+invenio_webhooks/translations/es/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/es/LC_MESSAGES/messages.po
+invenio_webhooks/translations/fr/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
+invenio_webhooks/translations/it/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/it/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/test_api.py
 tests/test_invenio_webhooks.py
 tests/test_receivers.py
```

### Comparing `invenio-webhooks-1.0.0a4/tests/conftest.py` & `invenio-webhooks-1.0.1/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,133 +21,144 @@
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 """Pytest configuration."""
 
-from __future__ import absolute_import, print_function
-
 import os
 
 import pytest
 from flask import Flask
-from flask_babelex import Babel
 from flask_breadcrumbs import Breadcrumbs
-from flask_celeryext import FlaskCeleryExt
 from flask_mail import Mail
 from flask_menu import Menu
+from flask_security.utils import hash_password
 from invenio_accounts import InvenioAccounts
 from invenio_accounts.views import blueprint as accounts_blueprint
+from invenio_celery import InvenioCelery
 from invenio_db import InvenioDB, db
-from invenio_oauth2server import InvenioOAuth2Server
+from invenio_i18n import InvenioI18N
+from invenio_oauth2server import InvenioOAuth2Server, InvenioOAuth2ServerREST
 from invenio_oauth2server.models import Token
 from invenio_oauth2server.views import server_blueprint, settings_blueprint
+from sqlalchemy_utils.functions import create_database, database_exists, drop_database
 
 from invenio_webhooks import InvenioWebhooks
 from invenio_webhooks.models import Receiver
 from invenio_webhooks.views import blueprint
 
 
 @pytest.fixture
 def app(request):
     """Flask application fixture."""
-    app = Flask('testapp')
+    app = Flask("testapp")
     app.config.update(
-        TESTING=True,
+        ACCOUNTS_JWT_ENABLE=False,
+        APP_THEME=[],
+        THEME_ICONS=[],
+        CELERY_BROKER_TRANSPORT="redis",
         CELERY_ALWAYS_EAGER=True,
         CELERY_CACHE_BACKEND="memory",
         CELERY_EAGER_PROPAGATES_EXCEPTIONS=True,
         CELERY_RESULT_BACKEND="cache",
+        CELERY_TASK_TRACK_STARTED=True,
         LOGIN_DISABLED=False,
-        SECRET_KEY='test_key',
-        SQLALCHEMY_TRACK_MODIFICATIONS=True,
-        SQLALCHEMY_DATABASE_URI=os.getenv('SQLALCHEMY_DATABASE_URI',
-                                          'sqlite:///test.db'),
-        WTF_CSRF_ENABLED=False,
+        OAUTH2_CACHE_TYPE="simple",
         OAUTHLIB_INSECURE_TRANSPORT=True,
-        OAUTH2_CACHE_TYPE='simple',
-        SECURITY_PASSWORD_HASH='plaintext',
-        SECURITY_PASSWORD_SCHEMES=['plaintext'],
+        SECRET_KEY="test_key",
         SECURITY_DEPRECATED_PASSWORD_SCHEMES=[],
+        SECURITY_PASSWORD_HASH="plaintext",
+        SECURITY_PASSWORD_SCHEMES=["plaintext"],
+        SECURITY_PASSWORD_SINGLE_HASH=False,
+        SQLALCHEMY_TRACK_MODIFICATIONS=True,
+        SQLALCHEMY_DATABASE_URI=os.getenv(
+            "SQLALCHEMY_DATABASE_URI", "sqlite:///test.db"
+        ),
+        TESTING=True,
+        WTF_CSRF_ENABLED=False,
     )
-    celeryext = FlaskCeleryExt(app)
-    celeryext.celery.flask_app = app  # Make sure both apps are the same!
-    Babel(app)
+    InvenioI18N(app)
     Mail(app)
     Menu(app)
     Breadcrumbs(app)
+    InvenioCelery(app)
     InvenioDB(app)
     InvenioAccounts(app)
     app.register_blueprint(accounts_blueprint)
     InvenioOAuth2Server(app)
+    InvenioOAuth2ServerREST(app)
     app.register_blueprint(server_blueprint)
     app.register_blueprint(settings_blueprint)
     InvenioWebhooks(app)
     app.register_blueprint(blueprint)
 
     with app.app_context():
+        if not database_exists(str(db.engine.url)):
+            create_database(str(db.engine.url))
         db.create_all()
 
     def teardown():
         with app.app_context():
-            db.drop_all()
+            drop_database(str(db.engine.url))
 
     request.addfinalizer(teardown)
     return app
 
 
 @pytest.fixture
 def tester_id(app):
     """Fixture that contains the test data for models tests."""
     with app.app_context():
-        datastore = app.extensions['security'].datastore
+        datastore = app.extensions["security"].datastore
         tester = datastore.create_user(
-            email='info@inveniosoftware.org', password='tester',
+            email="info@inveniosoftware.org",
+            password=hash_password("tester"),
+            active=True,
         )
-        db.session.commit()
+        datastore.commit()
         tester_id = tester.id
     return tester_id
 
 
 @pytest.fixture
 def access_token(app, tester_id):
     """Fixture that create an access token."""
     with app.app_context():
         token = Token.create_personal(
-            'test-personal-{0}'.format(tester_id),
+            "test-personal-{0}".format(tester_id),
             tester_id,
-            scopes=['webhooks:event'],
+            scopes=["webhooks:event"],
             is_internal=True,
         ).access_token
         db.session.commit()
         return token
 
 
 @pytest.fixture
 def access_token_no_scope(app, tester_id):
     """Fixture that create an access token without scope."""
     with app.app_context():
         token = Token.create_personal(
-            'test-personal-{0}'.format(tester_id),
+            "test-personal-{0}".format(tester_id),
             tester_id,
-            scopes=[''],
+            scopes=[""],
             is_internal=True,
         ).access_token
         db.session.commit()
         return token
 
 
 @pytest.fixture
 def receiver(app):
     """Register test receiver."""
-    class TestReceiver(Receiver):
 
+    class TestReceiver(Receiver):
         def __init__(self, *args, **kwargs):
             super(TestReceiver, self).__init__(*args, **kwargs)
             self.calls = []
 
         def run(self, event):
             self.calls.append(event)
 
-    app.extensions['invenio-webhooks'].register('test-receiver', TestReceiver)
+    app.extensions["invenio-webhooks"].register("test-receiver", TestReceiver)
     return TestReceiver
```

### Comparing `invenio-webhooks-1.0.0a4/tests/test_invenio_webhooks.py` & `invenio-webhooks-1.0.1/tests/test_invenio_webhooks.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,45 +21,64 @@
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 """Module tests."""
 
-from __future__ import absolute_import, print_function
-
+import pytest
 from flask import Flask, url_for
+from invenio_db import db
 
 from invenio_webhooks import InvenioWebhooks
 
 
 def test_version():
     """Test version import."""
     from invenio_webhooks import __version__
+
     assert __version__
 
 
 def test_init():
     """Test extension initialization."""
-    app = Flask('testapp')
+    app = Flask("testapp")
     ext = InvenioWebhooks(app)
-    assert 'invenio-webhooks' in app.extensions
+    assert "invenio-webhooks" in app.extensions
 
-    app = Flask('testapp')
+    app = Flask("testapp")
     ext = InvenioWebhooks()
-    assert 'invenio-webhooks' not in app.extensions
+    assert "invenio-webhooks" not in app.extensions
     ext.init_app(app)
-    assert 'invenio-webhooks' in app.extensions
+    assert "invenio-webhooks" in app.extensions
+
+
+def test_alembic(app):
+    """Test alembic recipes."""
+    ext = app.extensions["invenio-db"]
+
+    with app.app_context():
+        if db.engine.name == "sqlite":
+            raise pytest.skip("Upgrades are not supported on SQLite.")
+
+        assert not ext.alembic.compare_metadata()
+        db.drop_all()
+        ext.alembic.upgrade()
+
+        assert not ext.alembic.compare_metadata()
+        ext.alembic.downgrade(target="96e796392533")
+        ext.alembic.upgrade()
+
+        assert not ext.alembic.compare_metadata()
 
 
-def test_view(app):
+def test_view(app, receiver):
     """Test view."""
     with app.test_request_context():
-        view_url = url_for('invenio_webhooks.event_list',
-                           receiver_id='test_receiver')
+        view_url = url_for("invenio_webhooks.event_list", receiver_id="test_receiver")
 
     with app.test_client() as client:
         res = client.get(view_url)
         assert res.status_code == 405
 
         res = client.post(view_url)
         assert res.status_code == 401
```

### Comparing `invenio-webhooks-1.0.0a4/tests/test_receivers.py` & `invenio-webhooks-1.0.1/tests/test_receivers.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,146 +13,211 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Invenio; if not, write to the Free Software Foundation, Inc.,
 # 59 Temple Place, Suite 330, Boston, MA 02111-1307, USA.
 
-from __future__ import absolute_import
-
 import json
 
 import pytest
 from flask import url_for
 from invenio_db import db
 
-from invenio_webhooks.models import CeleryReceiver, Event, InvalidPayload, \
-    InvalidSignature, ReceiverDoesNotExist
+from invenio_webhooks.models import (
+    CeleryReceiver,
+    Event,
+    InvalidPayload,
+    InvalidSignature,
+    Receiver,
+    ReceiverDoesNotExist,
+)
 from invenio_webhooks.proxies import current_webhooks
 from invenio_webhooks.signatures import get_hmac
 
 
+def test_run_must_be_implemeted():
+    """Test that run raises NotImplementedError if not overriden."""
+    with pytest.raises(NotImplementedError):
+        Receiver("not-implemented").run(None)
+
+
 def test_receiver_registration(app, receiver):
     with app.app_context():
-        current_webhooks.register('test-invalid', receiver)
+        current_webhooks.register("test-invalid", receiver)
 
-        assert 'test-receiver' in current_webhooks.receivers
-        assert 'test-receiver' == current_webhooks.receivers[
-            'test-receiver'].receiver_id
+        assert "test-receiver" in current_webhooks.receivers
+        assert (
+            "test-receiver" == current_webhooks.receivers["test-receiver"].receiver_id
+        )
 
         # Double registration
         with pytest.raises(AssertionError):
-            current_webhooks.register('test-receiver', receiver)
+            current_webhooks.register("test-receiver", receiver)
 
-        current_webhooks.unregister('test-receiver')
-        assert 'test-receiver' not in current_webhooks.receivers
+        current_webhooks.unregister("test-receiver")
+        assert "test-receiver" not in current_webhooks.receivers
 
-        current_webhooks.register('test-receiver', receiver)
+        current_webhooks.register("test-receiver", receiver)
 
     # JSON payload parsing
-    payload = json.dumps(dict(somekey='somevalue'))
-    headers = [('Content-Type', 'application/json')]
+    payload = json.dumps(dict(somekey="somevalue"))
+    headers = [("Content-Type", "application/json")]
     with app.test_request_context(headers=headers, data=payload):
-        event = Event.create(receiver_id='test-receiver')
+        event = Event.create(receiver_id="test-receiver")
         event.process()
         assert 1 == len(event.receiver.calls)
         assert json.loads(payload) == event.receiver.calls[0].payload
         assert event.receiver.calls[0].user_id is None
 
     # Form encoded values payload parsing
-    payload = dict(somekey='somevalue')
-    with app.test_request_context(method='POST', data=payload):
-        event = Event.create(receiver_id='test-receiver')
+    payload = dict(somekey="somevalue")
+    with app.test_request_context(method="POST", data=payload):
+        event = Event.create(receiver_id="test-receiver")
         event.process()
         assert 2 == len(event.receiver.calls)
-        assert dict(somekey=['somevalue']) == event.receiver.calls[1].payload
+        assert dict(somekey="somevalue") == event.receiver.calls[1].payload
 
     # Test invalid post data
-    with app.test_request_context(method='POST', data="invaliddata"):
+    with app.test_request_context(method="POST", data="invaliddata"):
         with pytest.raises(InvalidPayload):
-            event = Event.create(receiver_id='test-receiver')
+            event = Event.create(receiver_id="test-receiver")
 
     calls = []
 
     # Test Celery Receiver
     class TestCeleryReceiver(CeleryReceiver):
-
         def run(self, event):
             calls.append(event.payload)
 
-    app.extensions['invenio-webhooks'].register('celery-receiver',
-                                                TestCeleryReceiver)
+    app.extensions["invenio-webhooks"].register("celery-receiver", TestCeleryReceiver)
 
     # Form encoded values payload parsing
-    payload = dict(somekey='somevalue')
-    with app.test_request_context(method='POST', data=payload):
-        event = Event.create(receiver_id='celery-receiver')
+    payload = dict(somekey="somevalue")
+    with app.test_request_context(method="POST", data=payload):
+        event = Event.create(receiver_id="celery-receiver")
         db.session.add(event)
         db.session.commit()
         event.process()
         assert 1 == len(calls)
-        assert dict(somekey=['somevalue']) == calls[0]
+        assert dict(somekey="somevalue") == calls[0]
 
 
 def test_unknown_receiver(app):
     """Raise when receiver does not exist."""
     with app.app_context():
         with pytest.raises(ReceiverDoesNotExist):
-            Event.create(receiver_id='unknown')
+            Event.create(receiver_id="unknown")
 
 
 def test_hookurl(app, receiver):
     with app.test_request_context():
-        assert current_webhooks.receivers['test-receiver'].get_hook_url(
-            'token'
+        assert current_webhooks.receivers["test-receiver"].get_hook_url(
+            "token"
         ) == url_for(
-            'invenio_webhooks.event_list',
-            receiver_id='test-receiver',
-            access_token='token',
-            _external=True
+            "invenio_webhooks.event_list",
+            receiver_id="test-receiver",
+            access_token="token",
+            _external=True,
         )
 
-    app.config['WEBHOOKS_DEBUG_RECEIVER_URLS'] = {
-        'test-receiver': 'http://test.local/?access_token=%(token)s'
+    app.config["WEBHOOKS_DEBUG_RECEIVER_URLS"] = {
+        "test-receiver": "http://test.local/?access_token=%(token)s"
     }
 
     with app.test_request_context():
-        assert 'http://test.local/?access_token=token' == \
-            current_webhooks.receivers['test-receiver'].get_hook_url(
-                'token'
-            )
+        assert "http://test.local/?access_token=token" == current_webhooks.receivers[
+            "test-receiver"
+        ].get_hook_url("token")
 
 
 def test_signature_checking(app, receiver):
     """Check signatures for payload."""
+
     class TestReceiverSign(receiver):
-        signature = 'X-Hub-Signature'
+        signature = "X-Hub-Signature"
 
     with app.app_context():
-        current_webhooks.register('test-receiver-sign', TestReceiverSign)
+        current_webhooks.register("test-receiver-sign", TestReceiverSign)
 
     # check correct signature
-    payload = json.dumps(dict(somekey='somevalue'))
+    payload = json.dumps(dict(somekey="somevalue"))
     with app.app_context():
-        headers = [('Content-Type', 'application/json'),
-                   ('X-Hub-Signature', get_hmac(payload))]
+        headers = [
+            ("Content-Type", "application/json"),
+            ("X-Hub-Signature", get_hmac(payload)),
+        ]
     with app.test_request_context(headers=headers, data=payload):
-        event = Event.create(receiver_id='test-receiver-sign')
+        event = Event.create(receiver_id="test-receiver-sign")
         event.process()
         assert json.loads(payload) == event.receiver.calls[0].payload
 
     # check signature with prefix
     with app.app_context():
-        headers = [('Content-Type', 'application/json'),
-                   ('X-Hub-Signature', 'sha1=' + get_hmac(payload))]
+        headers = [
+            ("Content-Type", "application/json"),
+            ("X-Hub-Signature", "sha1=" + get_hmac(payload)),
+        ]
     with app.test_request_context(headers=headers, data=payload):
-        event = Event.create(receiver_id='test-receiver-sign')
+        event = Event.create(receiver_id="test-receiver-sign")
         event.process()
         assert json.loads(payload) == event.receiver.calls[1].payload
 
     # check incorrect signature
     with app.app_context():
-        headers = [('Content-Type', 'application/json'),
-                   ('X-Hub-Signature', get_hmac("somevalue"))]
+        headers = [
+            ("Content-Type", "application/json"),
+            ("X-Hub-Signature", get_hmac("somevalue")),
+        ]
     with app.test_request_context(headers=headers, data=payload):
         with pytest.raises(InvalidSignature):
-            Event.create(receiver_id='test-receiver-sign')
+            Event.create(receiver_id="test-receiver-sign")
+
+
+def test_event_deletion(app, receiver):
+    """Test event deletion."""
+    with app.test_request_context(method="POST", data={"foo": "bar"}):
+        event = Event.create(receiver_id="test-receiver")
+        event.delete()
+        assert event.response == {"status": 410, "message": "Gone."}
+        assert event.response_code == 410
+
+
+def test_event_status(app):
+    """Test event status reporting."""
+    data = json.dumps({"x": 40, "y": 2})
+
+    class TestCeleryReceiver(CeleryReceiver):
+        def run(self, event):
+            """Change task state."""
+            from celery import current_task, states
+
+            event.response["message"] = event.payload["x"] + event.payload["y"]
+            current_task.update_state(
+                task_id=str(event.id), state=states.PENDING, meta={"message": 0}
+            )
+            assert event.status == (202, 0)
+            current_task.update_state(
+                task_id=str(event.id), state=states.PENDING, meta={"message": 1}
+            )
+            assert event.status == (202, 1)
+            current_task.update_state(
+                task_id=str(event.id), state=states.SUCCESS, meta={"message": 2}
+            )
+
+    app.extensions["invenio-webhooks"].register(
+        "test-celery-receiver", TestCeleryReceiver
+    )
+
+    headers = [("Content-Type", "application/json")]
+    with app.test_request_context(method="POST", headers=headers, data=data):
+        event = Event.create(receiver_id="test-celery-receiver")
+        db.session.add(event)
+        db.session.commit()
+        event_id = event.id
+        assert event.status == (202, "Accepted.")
+        event.process()
+
+    with app.app_context():
+        event = Event.query.get(event_id)
+        assert event.status == (201, 42)
+        assert event.response["message"] == 42
```

### Comparing `invenio-webhooks-1.0.0a4/.editorconfig` & `invenio-webhooks-1.0.1/.editorconfig`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,14 @@
 [*.rst]
 indent_size = 4
 
 # CSS, HTML, JS, JSON, YML
 [*.{css,html,js,json,yml}]
 indent_size = 2
 
-# Matches the exact files either package.json or .travis.yml
-[{package.json,.travis.yml}]
+# Matches the exact files either package.json or .github/workflows/*.yml
+[{package.json, .github/workflows/*.yml}]
 indent_size = 2
 
 # Dockerfile
 [Dockerfile]
 indent_size = 4
```

### Comparing `invenio-webhooks-1.0.0a4/AUTHORS.rst` & `invenio-webhooks-1.0.1/AUTHORS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 
 - Alizee Pace <alizee.pace@gmail.com>
 - Grzegorz Szpura <grzegorz.szpura@cern.ch>
 - Jiri Kuncar <jiri.kuncar@cern.ch>
 - Konstantinos Kostis <konstantinos.kostis@cern.ch>
 - Lars Holm Nielsen <lars.holm.nielsen@cern.ch>
 - Leonardo Rossi <leonardo.r@cern.ch>
+- Orestis Melkonian <melkon.or@gmail.com>
 - Tibor Simko <tibor.simko@cern.ch>
```

### Comparing `invenio-webhooks-1.0.0a4/CHANGES.rst` & `invenio-webhooks-1.0.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     In applying this license, CERN does not
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 Changes
 =======
 
+Version 1.0.1 (release 2023-07-12)
+
+- add event error handling
+
+Version 1.0.0 (release 2023-07-03)
+
+- v1.0.0 release
+
 Version 1.0.0a4 (release 2016-10-03)
 
 - Port to new structure for Invenio 3.
 
 Version 0.1.0 (release 2015-08-05)
 
 - Initial public release.
```

### Comparing `invenio-webhooks-1.0.0a4/CONTRIBUTING.rst` & `invenio-webhooks-1.0.1/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -110,9 +110,9 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests and must not decrease test coverage.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring.
 3. The pull request should work for Python 2.7, 3.3, 3.4 and 3.5. Check
-   https://travis-ci.org/inveniosoftware/invenio-webhooks/pull_requests
+   https://github.com/inveniosoftware/invenio-webhooks/actions?query=event%3Apull_request
    and make sure that the tests pass for all supported Python versions.
```

### Comparing `invenio-webhooks-1.0.0a4/LICENSE` & `invenio-webhooks-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/MANIFEST.in` & `invenio-webhooks-1.0.1/MANIFEST.in`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015 CERN.
+# Copyright (C) 2015, 2016 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,38 +18,30 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-
-# TODO: Generate this manifest file by running the following commands:
-#
-#  git init
-#  git add -A
-#  pip install -e .[all]
-#  check-manifest -u
-
-# Check manifest will not automatically add these two files:
-include .dockerignore
-include .editorconfig
-include .tx/config
-recursive-include invenio_webhooks *.po *.pot *.mo
-
-# added by check_manifest.py
 include *.rst
 include *.sh
 include *.txt
+include .dockerignore
+include .editorconfig
+include .git-blame-ignore-revs
 include .lgtm
+include .tx/config
 include LICENSE
 include MAINTAINERS
 include babel.ini
 include docs/requirements.txt
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs Makefile
 recursive-include examples *.py
 recursive-include invenio_webhooks *.html
+recursive-include invenio_webhooks *.po *.pot *.mo
+recursive-include invenio_webhooks *.py
 recursive-include tests *.py
+recursive-include .github/workflows *.yml
```

### Comparing `invenio-webhooks-1.0.0a4/README.rst` & `invenio-webhooks-1.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 ==================
  Invenio-Webhooks
 ==================
 
-.. image:: https://img.shields.io/travis/inveniosoftware/invenio-webhooks.svg
-        :target: https://travis-ci.org/inveniosoftware/invenio-webhooks
+.. image:: https://github.com/inveniosoftware/invenio-webhooks/workflows/CI/badge.svg
+        :target: https://github.com/inveniosoftware/invenio-webhooks/actions?query=workflow%3ACI
 
 .. image:: https://img.shields.io/coveralls/inveniosoftware/invenio-webhooks.svg
         :target: https://coveralls.io/r/inveniosoftware/invenio-webhooks
 
 .. image:: https://img.shields.io/github/tag/inveniosoftware/invenio-webhooks.svg
         :target: https://github.com/inveniosoftware/invenio-webhooks/releases
 
@@ -41,9 +41,9 @@
         :target: https://github.com/inveniosoftware/invenio-webhooks/blob/master/LICENSE
 
 
 Invenio module for processing webhook events.
 
 *This is an experimental developer preview release.*
 
-* Free software: GPLv2 license
+* Free software: MIT license
 * Documentation: https://invenio-webhooks.readthedocs.io/
```

### Comparing `invenio-webhooks-1.0.0a4/RELEASE-NOTES.rst` & `invenio-webhooks-1.0.1/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/babel.ini` & `invenio-webhooks-1.0.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/pytest.ini` & `invenio-webhooks-1.0.1/invenio_webhooks/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015 CERN.
+# Copyright (C) 2016 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,9 +18,24 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-[pytest]
-addopts = --pep8 --ignore=docs --cov=invenio_webhooks --cov-report=term-missing
+"""Webhook errors."""
+
+
+class WebhooksError(Exception):
+    """General webhook error."""
+
+
+class ReceiverDoesNotExist(WebhooksError):
+    """Raised when receiver does not exist."""
+
+
+class InvalidPayload(WebhooksError):
+    """Raised when the payload is invalid."""
+
+
+class InvalidSignature(WebhooksError):
+    """Raised when the signature does not match."""
```

### Comparing `invenio-webhooks-1.0.0a4/requirements-devel.txt` & `invenio-webhooks-1.0.1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a4/PKG-INFO` & `invenio-webhooks-1.0.1/invenio_webhooks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: invenio-webhooks
-Version: 1.0.0a4
-Summary: Invenio module for processing webhook events.
+Version: 1.0.1
+Summary: "Invenio webhooks module to create REST APIs."
 Home-page: https://github.com/inveniosoftware/invenio-webhooks
 Author: CERN
 Author-email: info@inveniosoftware.org
-License: GPLv2
+License: MIT
 Description: ..
             This file is part of Invenio.
             Copyright (C) 2015 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
@@ -29,16 +29,16 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         ==================
          Invenio-Webhooks
         ==================
         
-        .. image:: https://img.shields.io/travis/inveniosoftware/invenio-webhooks.svg
-                :target: https://travis-ci.org/inveniosoftware/invenio-webhooks
+        .. image:: https://github.com/inveniosoftware/invenio-webhooks/workflows/CI/badge.svg
+                :target: https://github.com/inveniosoftware/invenio-webhooks/actions?query=workflow%3ACI
         
         .. image:: https://img.shields.io/coveralls/inveniosoftware/invenio-webhooks.svg
                 :target: https://coveralls.io/r/inveniosoftware/invenio-webhooks
         
         .. image:: https://img.shields.io/github/tag/inveniosoftware/invenio-webhooks.svg
                 :target: https://github.com/inveniosoftware/invenio-webhooks/releases
         
@@ -49,18 +49,17 @@
                 :target: https://github.com/inveniosoftware/invenio-webhooks/blob/master/LICENSE
         
         
         Invenio module for processing webhook events.
         
         *This is an experimental developer preview release.*
         
-        * Free software: GPLv2 license
+        * Free software: MIT license
         * Documentation: https://invenio-webhooks.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
             Copyright (C) 2015, 2016 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
@@ -79,30 +78,39 @@
             In applying this license, CERN does not
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         Changes
         =======
         
+        Version 1.0.1 (release 2023-07-12)
+        
+        - add event error handling
+        
+        Version 1.0.0 (release 2023-07-03)
+        
+        - v1.0.0 release
+        
         Version 1.0.0a4 (release 2016-10-03)
         
         - Port to new structure for Invenio 3.
         
         Version 0.1.0 (release 2015-08-05)
         
         - Initial public release.
         
 Keywords: invenio webhooks
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 1 - Planning
+Requires-Python: >=3.7
+Provides-Extra: tests
```

