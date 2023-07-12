# Comparing `tmp/invenio-users-resources-2.1.0.tar.gz` & `tmp/invenio-users-resources-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-users-resources-2.1.0.tar", last modified: Fri Jul  7 15:20:38 2023, max compression
+gzip compressed data, was "dist/invenio-users-resources-2.1.1.tar", last modified: Wed Jul 12 07:09:48 2023, max compression
```

## Comparing `invenio-users-resources-2.1.0.tar` & `invenio-users-resources-2.1.1.tar`

### file list

```diff
@@ -1,326 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/administration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/administration/views/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/administration/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/administration/views/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/entity_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/notifications/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/notifications/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/dumpers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/users/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/resources/users/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/groups/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/services/users/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/avatar.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/invenio_users_resources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/invenio_users_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/resources/test_resources_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/resources/test_resources_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:20:38.000000 invenio-users-resources-2.1.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/services/test_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/services/test_service_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/test_invenio_users_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 15:20:29.000000 invenio-users-resources-2.1.0/tests/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/administration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/administration/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/administration/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/administration/views/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/entity_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/notifications/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/notifications/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/dumpers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/resources/users/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/groups/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/services/users/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/avatar.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 07:09:47.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/invenio_users_resources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/invenio_users_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/resources/test_resources_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/resources/test_resources_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:09:48.000000 invenio-users-resources-2.1.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/services/test_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/services/test_service_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/test_invenio_users_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-12 07:09:41.000000 invenio-users-resources-2.1.1/tests/test_notifications.py
```

### Comparing `invenio-users-resources-2.1.0/.editorconfig` & `invenio-users-resources-2.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/.github/workflows/pypi-publish.yml` & `invenio-users-resources-2.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/.github/workflows/tests.yml` & `invenio-users-resources-2.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/.tx/config` & `invenio-users-resources-2.1.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/CHANGES.rst` & `invenio-users-resources-2.1.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     Invenio-Users-Resources is free software; you can redistribute it
     and/or modify it under the terms of the MIT License; see LICENSE file for
     more details.
 
 Changes
 =======
 
+Version 2.1.1 (2023-07-12)
+
+- users: make username optional on expansion
+
 Version 2.1.0 (2023-07-07)
 
 - administration: add users administration panel
 
 Version 2.0.1 (2023-07-05)
 
 - fix post_commit hooks
```

### Comparing `invenio-users-resources-2.1.0/CONTRIBUTING.rst` & `invenio-users-resources-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/LICENSE` & `invenio-users-resources-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/MANIFEST.in` & `invenio-users-resources-2.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/PKG-INFO` & `invenio-users-resources-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 2.1.1 (2023-07-12)
+        
+        - users: make username optional on expansion
+        
         Version 2.1.0 (2023-07-07)
         
         - administration: add users administration panel
         
         Version 2.0.1 (2023-07-05)
         
         - fix post_commit hooks
```

### Comparing `invenio-users-resources-2.1.0/README.rst` & `invenio-users-resources-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/docs/Makefile` & `invenio-users-resources-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/docs/conf.py` & `invenio-users-resources-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/docs/index.rst` & `invenio-users-resources-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/docs/make.bat` & `invenio-users-resources-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/administration/views/users.py` & `invenio-users-resources-2.1.1/invenio_users_resources/administration/views/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     search_config_name = "USERS_RESOURCES_SEARCH"
     search_sort_config_name = "USERS_RESOURCES_SORT_OPTIONS"
 
     @staticmethod
     def disabled():
         """Disable the view on demand."""
-        return current_app.config["USERS_RESOURCES_ADMINISTRATION_DISABLED"]
+        return not current_app.config["USERS_RESOURCES_ADMINISTRATION_ENABLED"]
 
 
 class UsersDetailView(AdminResourceDetailView):
     """Configuration for users sets detail view."""
 
     url = "/users/<pid_value>"
     api_endpoint = "/users/"
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/config.py` & `invenio-users-resources-2.1.1/invenio_users_resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/entity_resolvers.py` & `invenio-users-resources-2.1.1/invenio_users_resources/entity_resolvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from invenio_records_resources.references.entity_resolvers import (
     EntityProxy,
     EntityResolver,
 )
 from sqlalchemy.exc import NoResultFound
 
 from .proxies import current_users_service
-from .services.schemas import SystemUserSchema, UserGhostSchema
+from .services.schemas import SystemUserSchema, UserGhostSchema, UserSchema
 from .services.users.config import UsersServiceConfig
 
 
 class UserProxy(EntityProxy):
     """Resolver proxy for a User entity."""
 
     def _resolve(self):
@@ -59,25 +59,27 @@
     def pick_resolved_fields(self, identity, resolved_dict):
         """Select which fields to return when resolving the reference."""
         profile = resolved_dict.get("profile", {})
         fake_user_obj = SimpleNamespace(id=resolved_dict["id"])
         avatar = current_users_service.links_item_tpl.expand(identity, fake_user_obj)[
             "avatar"
         ]
-        return {
+        serialized_user = {
             "id": resolved_dict["id"],
-            "username": resolved_dict["username"],
+            "username": resolved_dict.get("username", ""),
             "email": resolved_dict.get("email", ""),
             "profile": {
                 "full_name": profile.get("full_name", ""),
                 "affiliations": profile.get("affiliations", ""),
             },
             "links": {"avatar": avatar},
         }
 
+        return serialized_user
+
 
 class UserResolver(EntityResolver):
     """Resolver for users."""
 
     type_id = "user"
 
     def __init__(self):
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/ext.py` & `invenio-users-resources-2.1.1/invenio_users_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/forms.py` & `invenio-users-resources-2.1.1/invenio_users_resources/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/models.py` & `invenio-users-resources-2.1.1/invenio_users_resources/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/notifications/filters.py` & `invenio-users-resources-2.1.1/invenio_users_resources/notifications/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/notifications/generators.py` & `invenio-users-resources-2.1.1/invenio_users_resources/notifications/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/proxies.py` & `invenio-users-resources-2.1.1/invenio_users_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/api.py` & `invenio-users-resources-2.1.1/invenio_users_resources/records/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     # NOTE: the "uuid" isn't a UUID but contains the same value as the "id"
     #       field, which is currently a str for Role objects (role.name)!
     dumper = SearchDumper(extensions=[], model_fields={"id": ("uuid", str)})
 
     metadata = None
     """Disabled metadata field from the base class."""
 
-    index = IndexField("groups-group-v1.0.0", search_alias="groups")
+    index = IndexField("groups-group-v2.0.0", search_alias="groups")
     """The search engine index to use."""
 
     # TODO
     id = ModelField("id")
     """The data-layer id."""
 
     name = DictField("name")
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/dumpers/email.py` & `invenio-users-resources-2.1.1/invenio_users_resources/records/dumpers/email.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/hooks.py` & `invenio-users-resources-2.1.1/invenio_users_resources/records/hooks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json` & `invenio-users-resources-2.1.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/records/models.py` & `invenio-users-resources-2.1.1/invenio_users_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/config.py` & `invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/resources/groups/resource.py` & `invenio-users-resources-2.1.1/invenio_users_resources/resources/groups/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/resources/users/config.py` & `invenio-users-resources-2.1.1/invenio_users_resources/resources/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/resources/users/resource.py` & `invenio-users-resources-2.1.1/invenio_users_resources/resources/users/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/common.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/common.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/generators.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/groups/config.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/groups/results.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/groups/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/groups/service.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/groups/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/groups/tasks.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/groups/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/params.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/params.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/permissions.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/results.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/schemas.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,18 +63,21 @@
     username = fields.String()
     profile = fields.Dict()
     preferences = fields.Nested(UserPreferencesSchema)
 
     def is_self(self, obj):
         """Determine if identity is the current identity."""
         current_identity = self.context["identity"]
+
+        _id = obj.get("id") or obj.id
+
         return (
-            obj.id is not None
+            _id is not None
             and current_identity.id is not None
-            and str(obj.id) == str(current_identity.id)
+            and str(_id) == str(current_identity.id)
         )
 
 
 class GroupSchema(BaseRecordSchema):
     """Schema for user groups."""
 
     name = fields.String()
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/users/config.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/users/results.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/users/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/users/service.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/users/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/services/users/tasks.py` & `invenio-users-resources-2.1.1/invenio_users_resources/services/users/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html` & `invenio-users-resources-2.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/messages.pot` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-users-resources-2.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources/views.py` & `invenio-users-resources-2.1.1/invenio_users_resources/views.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources.egg-info/PKG-INFO` & `invenio-users-resources-2.1.1/invenio_users_resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 2.1.1 (2023-07-12)
+        
+        - users: make username optional on expansion
+        
         Version 2.1.0 (2023-07-07)
         
         - administration: add users administration panel
         
         Version 2.0.1 (2023-07-05)
         
         - fix post_commit hooks
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources.egg-info/SOURCES.txt` & `invenio-users-resources-2.1.1/invenio_users_resources.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,23 @@
 invenio_users_resources/records/hooks.py
 invenio_users_resources/records/models.py
 invenio_users_resources/records/dumpers/__init__.py
 invenio_users_resources/records/dumpers/email.py
 invenio_users_resources/records/mappings/__init__.py
 invenio_users_resources/records/mappings/os-v1/__init__.py
 invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
+invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json
 invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
 invenio_users_resources/records/mappings/os-v2/__init__.py
 invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
+invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json
 invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
 invenio_users_resources/records/mappings/v7/__init__.py
 invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
+invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json
 invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
 invenio_users_resources/resources/__init__.py
 invenio_users_resources/resources/groups/__init__.py
 invenio_users_resources/resources/groups/config.py
 invenio_users_resources/resources/groups/resource.py
 invenio_users_resources/resources/users/__init__.py
 invenio_users_resources/resources/users/config.py
```

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources.egg-info/entry_points.txt` & `invenio-users-resources-2.1.1/invenio_users_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/invenio_users_resources.egg-info/requires.txt` & `invenio-users-resources-2.1.1/invenio_users_resources.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/run-tests.sh` & `invenio-users-resources-2.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/setup.cfg` & `invenio-users-resources-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/conftest.py` & `invenio-users-resources-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/resources/test_resources_groups.py` & `invenio-users-resources-2.1.1/tests/resources/test_resources_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/resources/test_resources_users.py` & `invenio-users-resources-2.1.1/tests/resources/test_resources_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/services/test_service_groups.py` & `invenio-users-resources-2.1.1/tests/services/test_service_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/services/test_service_users.py` & `invenio-users-resources-2.1.1/tests/services/test_service_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/test_invenio_users_resources.py` & `invenio-users-resources-2.1.1/tests/test_invenio_users_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.1.0/tests/test_notifications.py` & `invenio-users-resources-2.1.1/tests/test_notifications.py`

 * *Files identical despite different names*

