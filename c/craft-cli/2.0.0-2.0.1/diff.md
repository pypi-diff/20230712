# Comparing `tmp/craft-cli-2.0.0.tar.gz` & `tmp/craft-cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-cli-2.0.0.tar", last modified: Fri Jun 16 18:37:43 2023, max compression
+gzip compressed data, was "craft-cli-2.0.1.tar", last modified: Wed Jul 12 11:38:15 2023, max compression
```

## Comparing `craft-cli-2.0.0.tar` & `craft-cli-2.0.1.tar`

### file list

```diff
@@ -1,89 +1,81 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      193 2022-08-15 14:30:03.000000 craft-cli-2.0.0/.bumpversion.cfg
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.editorconfig
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.471392 craft-cli-2.0.0/.github/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      172 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/release-drafter.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3504 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/renovate.json5
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/.github/workflows/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/cla-check.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      822 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/docs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      347 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2441 2023-06-15 22:43:44.000000 craft-cli-2.0.0/.github/workflows/tests.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.gitignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    17440 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.pylintrc
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      485 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.readthedocs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.yamllint.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3819 2023-06-16 18:31:51.000000 craft-cli-2.0.0/HACKING.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2362 2022-08-15 14:30:03.000000 craft-cli-2.0.0/HOWTO_RELEASE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-06-15 13:31:45.000000 craft-cli-2.0.0/LICENSE
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       34 2022-08-15 14:30:03.000000 craft-cli-2.0.0/MANIFEST.in
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-06-16 18:37:43.479392 craft-cli-2.0.0/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      755 2023-06-16 18:31:51.000000 craft-cli-2.0.0/README.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/craft_cli/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1661 2023-06-15 14:02:00.000000 craft-cli-2.0.0/craft_cli/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      160 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli/_version.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    18909 2023-06-15 18:06:58.000000 craft-cli-2.0.0/craft_cli/dispatcher.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3076 2023-06-07 17:48:53.000000 craft-cli-2.0.0/craft_cli/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    14578 2023-06-07 18:36:51.000000 craft-cli-2.0.0/craft_cli/helptexts.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    26272 2023-06-15 17:13:52.000000 craft-cli-2.0.0/craft_cli/messages.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    14777 2023-06-15 14:02:00.000000 craft-cli-2.0.0/craft_cli/printer.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/craft_cli/py.typed
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8155 2023-06-15 17:18:02.000000 craft-cli-2.0.0/craft_cli/pytest_plugin.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/craft_cli.egg-info/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1693 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       45 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      554 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       19 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       42 2022-08-15 14:30:03.000000 craft-cli-2.0.0/docs/.gitignore
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/_static/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/docs/_static/.gitempty
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/_static/css/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/_static/css/custom.css
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2668 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/conf.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16076 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/explanations.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8484 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/howtos.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      771 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       90 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/reference.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6550 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/tutorials.rst
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)    14270 2023-06-15 14:01:56.000000 craft-cli-2.0.0/examples.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8687 2023-06-16 18:31:51.000000 craft-cli-2.0.0/pyproject.toml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2023-06-16 18:37:43.479392 craft-cli-2.0.0/setup.cfg
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2813 2023-06-15 17:20:37.000000 craft-cli-2.0.0/tests/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1285 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/factory.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/tests/integration/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/integration/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       33 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/integration/test_stub.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/py.typed
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7507 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/test_pytest_plugin.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/tests/unit/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/unit/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    23381 2023-06-15 14:01:56.000000 craft-cli-2.0.0/tests/unit/test_dispatcher.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2046 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    44447 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_help.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    37699 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_emitter.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    14173 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_messages_helpers.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    45581 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_integration.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10797 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_stream_cm.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    39741 2023-06-14 18:56:33.000000 craft-cli-2.0.0/tests/unit/test_printer.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5350 2023-06-15 22:43:44.000000 craft-cli-2.0.0/tox.ini
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.471392 craft-cli-2.0.0/venv/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/venv/bin/
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      631 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      751 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html4.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)     1119 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html5.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      828 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2latex.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      636 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2man.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      801 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2odt.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)     1763 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      638 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      674 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2s5.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      908 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2xetex.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      639 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2xml.py
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)      707 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rstpep2html.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.254357 craft-cli-2.0.1/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      193 2022-08-15 14:30:03.000000 craft-cli-2.0.1/.bumpversion.cfg
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.226357 craft-cli-2.0.1/.github/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.226357 craft-cli-2.0.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-07-06 12:16:42.000000 craft-cli-2.0.1/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-07-06 12:16:42.000000 craft-cli-2.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-07-06 12:16:42.000000 craft-cli-2.0.1/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      172 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3504 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.230357 craft-cli-2.0.1/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      822 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      594 2023-07-06 12:16:42.000000 craft-cli-2.0.1/.github/workflows/issues.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      347 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2441 2023-06-15 22:43:44.000000 craft-cli-2.0.1/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17440 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.pylintrc
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      485 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-06-15 14:02:00.000000 craft-cli-2.0.1/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3819 2023-06-16 18:31:51.000000 craft-cli-2.0.1/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2362 2022-08-15 14:30:03.000000 craft-cli-2.0.1/HOWTO_RELEASE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-06-15 13:31:45.000000 craft-cli-2.0.1/LICENSE
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       34 2022-08-15 14:30:03.000000 craft-cli-2.0.1/MANIFEST.in
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-07-12 11:38:15.254357 craft-cli-2.0.1/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      755 2023-06-16 18:31:51.000000 craft-cli-2.0.1/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.234357 craft-cli-2.0.1/craft_cli/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1622 2023-07-06 12:16:42.000000 craft-cli-2.0.1/craft_cli/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      160 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    19092 2023-07-06 12:16:42.000000 craft-cli-2.0.1/craft_cli/dispatcher.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3161 2023-07-06 12:16:42.000000 craft-cli-2.0.1/craft_cli/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14578 2023-06-07 18:36:51.000000 craft-cli-2.0.1/craft_cli/helptexts.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    26277 2023-07-06 12:16:42.000000 craft-cli-2.0.1/craft_cli/messages.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14908 2023-07-12 11:35:17.000000 craft-cli-2.0.1/craft_cli/printer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/craft_cli/py.typed
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8155 2023-06-15 17:18:02.000000 craft-cli-2.0.1/craft_cli/pytest_plugin.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.238357 craft-cli-2.0.1/craft_cli.egg-info/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1587 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       45 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      554 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-07-12 11:38:15.000000 craft-cli-2.0.1/craft_cli.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.242357 craft-cli-2.0.1/docs/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       42 2022-08-15 14:30:03.000000 craft-cli-2.0.1/docs/.gitignore
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.242357 craft-cli-2.0.1/docs/_static/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/docs/_static/.gitempty
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.246357 craft-cli-2.0.1/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2681 2023-07-06 12:16:42.000000 craft-cli-2.0.1/docs/conf.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16076 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/explanations.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8484 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/howtos.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      771 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       90 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/reference.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6550 2023-06-15 14:02:00.000000 craft-cli-2.0.1/docs/tutorials.rst
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)    14270 2023-06-15 14:01:56.000000 craft-cli-2.0.1/examples.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8687 2023-06-16 18:31:51.000000 craft-cli-2.0.1/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2023-07-12 11:38:15.254357 craft-cli-2.0.1/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.246357 craft-cli-2.0.1/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2813 2023-06-15 17:20:37.000000 craft-cli-2.0.1/tests/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1285 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.250357 craft-cli-2.0.1/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2710 2023-07-12 11:35:17.000000 craft-cli-2.0.1/tests/integration/test_logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       33 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/integration/test_stub.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/py.typed
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7507 2023-06-07 17:48:53.000000 craft-cli-2.0.1/tests/test_pytest_plugin.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-07-12 11:38:15.250357 craft-cli-2.0.1/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.1/tests/unit/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    23381 2023-07-12 11:35:09.000000 craft-cli-2.0.1/tests/unit/test_dispatcher.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2046 2023-06-07 17:48:53.000000 craft-cli-2.0.1/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    44447 2023-06-07 17:48:53.000000 craft-cli-2.0.1/tests/unit/test_help.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    37699 2023-06-15 17:13:52.000000 craft-cli-2.0.1/tests/unit/test_messages_emitter.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14173 2023-06-07 17:48:53.000000 craft-cli-2.0.1/tests/unit/test_messages_helpers.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    45581 2023-06-15 17:13:52.000000 craft-cli-2.0.1/tests/unit/test_messages_integration.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10797 2023-06-15 17:13:52.000000 craft-cli-2.0.1/tests/unit/test_messages_stream_cm.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    40399 2023-07-12 11:35:17.000000 craft-cli-2.0.1/tests/unit/test_printer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5350 2023-06-15 22:43:44.000000 craft-cli-2.0.1/tox.ini
```

### Comparing `craft-cli-2.0.0/.editorconfig` & `craft-cli-2.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.github/renovate.json5` & `craft-cli-2.0.1/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.github/workflows/docs.yaml` & `craft-cli-2.0.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.github/workflows/tests.yaml` & `craft-cli-2.0.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.gitignore` & `craft-cli-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.pre-commit-config.yaml` & `craft-cli-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/.pylintrc` & `craft-cli-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/HACKING.rst` & `craft-cli-2.0.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/HOWTO_RELEASE.md` & `craft-cli-2.0.1/HOWTO_RELEASE.md`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/LICENSE` & `craft-cli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/PKG-INFO` & `craft-cli-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Command Line Interface
 Author-email: Canonical Ltd <snapcraft@lists.snapcraft.io>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `craft-cli-2.0.0/README.rst` & `craft-cli-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/craft_cli/__init__.py` & `craft-cli-2.0.1/craft_cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-"""Interact with Canonical services such as Charmhub and the Snap Store."""
+"""A Command Line Client builder."""
 
 try:
     from ._version import __version__
 except ImportError:  # pragma: no cover
     from importlib.metadata import version, PackageNotFoundError
 
     try:
```

### Comparing `craft-cli-2.0.0/craft_cli/dispatcher.py` & `craft-cli-2.0.1/craft_cli/dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,53 +13,55 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Argument processing and command dispatching functionality."""
 
 import argparse
 import difflib
-from typing import Any, Dict, List, Literal, NamedTuple, Optional, Tuple, Type
+from typing import Any, Dict, List, Literal, NamedTuple, Optional, Sequence, Tuple, Type
 
 from craft_cli import EmitterMode, emit
 from craft_cli.errors import ArgumentParsingError, ProvideHelpException
 from craft_cli.helptexts import HelpBuilder, OutputFormat
 
 
 class CommandGroup(NamedTuple):
     """Definition of a command group.
 
     A list of these is what is passed to the ``Dispatcher`` to run commands as part
     of the application.
-
-    :param name: identifier of the command group (to be used in help texts).
-    :param commands: a list of the commands in this group.
     """
 
     name: str
-    commands: List[Type["BaseCommand"]]
+    """The identifier of the command group (to be used in help texts)."""
 
+    commands: Sequence[Type["BaseCommand"]]
+    """A list of the commands belonging in this group."""
 
-class GlobalArgument(NamedTuple):
-    """Definition of a global argument to be handled by the Dispatcher.
 
-    :param name: identifier of the argument (the reference in the dictionary returned
-        by ``Dispatcher.pre_parse_args`` method)
-    :param type: the argument type: ``flag`` for arguments that are set to ``True`` if
-        specified (``False`` by default), or ``option`` if a value is needed after it.
-    :param short_option: the short form of the argument (a dash with a letter, e.g. ``-s``); it can
-        be None if the option does not have a short form.
-    :param long_option: the long form of the argument (two dashes and a name, e.g. ``--secure``).
-    :param help_message: the one-line text that describes the argument, for building the help texts.
-    """
+class GlobalArgument(NamedTuple):
+    """Definition of a global argument to be handled by the Dispatcher."""
 
     name: str
+    """Identifier of the argument (the reference in the dictionary returned) by the
+      ``Dispatcher.pre_parse_args()`` method)"""
+
     type: Literal["flag", "option"]
+    """The argument type: ``flag`` for arguments that are set to ``True`` if specified
+      (``False`` by default), or ``option`` if a value is needed after it."""
+
     short_option: Optional[str]
+    """The short form of the argument (a dash with a letter, e.g. ``-s``); it can be None
+      if the option does not have a short form."""
+
     long_option: str
+    """The long form of the argument (two dashes and a name, e.g. ``--secure``)."""
+
     help_message: str
+    """the one-line text that describes the argument, for building the help texts."""
 
 
 _DEFAULT_GLOBAL_ARGS = [
     GlobalArgument(
         "help",
         "flag",
         "-h",
@@ -89,42 +91,41 @@
     ),
 ]
 
 
 class BaseCommand:
     """Base class to build application commands.
 
-    Subclass this to create a new command; the subclass must define the following attributes:
-
-    - name: the identifier in the command line
-
-    - help_msg: a one line help for user documentation
+    Subclass this to create a new command; the subclass must define the ``name``,
+    ``help_msg``, and ``overview`` attributes. Additionally, it may override the
+    ``common`` and ``hidden`` attributes to change from their default values.
 
-    - overview: a longer multi-line text with the whole command description
-
-    Also it may override the following one to change its default:
-
-    - common: if it's a common/starter command, which are prioritized in the help (default to
-      False)
-
-    - hidden: do not show in help texts, useful for aliases or deprecated commands (default
-      to False)
-
-    It also must/can override some methods for the proper command behaviour (see each
+    The subclass may also override some methods for the proper command behaviour (see each
     method's docstring).
 
-    The subclass must be declared in the corresponding section of command groups indicated
-    to the Dispatcher.
+    Finally, the subclass must be declared in the corresponding section of command groups
+    indicated to the Dispatcher.
     """
 
     name: str
+    """The identifier in the command line, like "build" or "pack"."""
+
     help_msg: str
+    """A one-line help message for user documentation."""
+
     overview: str
-    common = False
-    hidden = False
+    """Longer, multi-line text with the whole command description."""
+
+    common: bool = False
+    """Whether this is a common/starter command, which are prioritized in the help
+      (defaults to False)."""
+
+    hidden: bool = False
+    """Do not show in help texts, useful for aliases or deprecated commands (defaults
+      to False)."""
 
     def __init__(self, config: Optional[Dict[str, Any]]):
         self.config = config
 
         # validate attributes
         mandatory = ("name", "help_msg", "overview")
         for attr_name in mandatory:
@@ -136,24 +137,25 @@
     def fill_parser(self, parser: "_CustomArgumentParser") -> None:
         """Specify command's specific parameters.
 
         Each command parameters are independent of other commands, but note there are some
         global ones (see `main.Dispatcher._build_argument_parser`).
 
         If this method is not overridden, the command will not have any parameters.
+
+        :param parser: The object to fill with this command's parameters.
         """
 
     def run(self, parsed_args: argparse.Namespace) -> Optional[int]:
         """Execute command's actual functionality.
 
         It must be overridden by the command implementation.
 
-        This will receive parsed arguments that were defined in :meth:.fill_parser.
-
-        It should return None or the desired process' return code.
+        :param parsed_args: The parsed arguments that were defined in :meth:`fill_parser`.
+        :return: This method should return ``None`` or the desired process' return code.
         """
         raise NotImplementedError()
 
 
 class _CustomArgumentParser(argparse.ArgumentParser):
     """ArgumentParser with custom error manager.."""
```

### Comparing `craft-cli-2.0.0/craft_cli/errors.py` & `craft-cli-2.0.1/craft_cli/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,37 +20,41 @@
     "CraftError",
 ]
 
 from typing import Optional
 
 
 class CraftError(Exception):
-    """Signal a program error with a lot of information to report.
+    """Signal a program error with a lot of information to report."""
 
-    :ivar message: the main message to the user, to be shown as first line (and
-      probably only that, according to the different modes); note that in some
-      cases the log location will be attached to this message.
+    message: str
+    """The main message to the user, to be shown as first line (and probably only that,
+      according to the different modes); note that in some cases the log location will be
+      attached to this message."""
 
-    :ivar details: the full error details received from a third party which
-      originated the error situation
+    details: Optional[str]
+    """The full error details received from a third party which originated the error
+      situation."""
 
-    :ivar resolution: an extra line indicating to the user how the error may be
-      fixed or avoided (to be shown together with 'message')
+    resolution: Optional[str]
+    """An extra line indicating to the user how the error may be fixed or avoided (to be
+      shown together with ``message``)."""
 
-    :ivar docs_url: an URL to point the user to documentation (to be shown
-      together with 'message')
+    docs_url: Optional[str]
+    """An URL to point the user to documentation (to be shown together with ``message``)."""
 
-    :ivar logpath_report: if the location of the log filepath should be presented
-      in the screen as the final message
+    logpath_report: bool
+    """Whether the location of the log filepath should be presented in the screen as the
+     final message."""
 
-    :ivar reportable: if an error report should be sent to some error-handling
-      backend (like Sentry)
+    reportable: bool
+    """If an error report should be sent to some error-handling backend (like Sentry)."""
 
-    :ivar retcode: the code to return when the application finishes
-    """
+    retcode: int
+    """The code to return when the application finishes."""
 
     def __init__(
         self,
         message: str,
         *,
         details: Optional[str] = None,
         resolution: Optional[str] = None,
```

### Comparing `craft-cli-2.0.0/craft_cli/helptexts.py` & `craft-cli-2.0.1/craft_cli/helptexts.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/craft_cli/messages.py` & `craft-cli-2.0.1/craft_cli/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     _WINDOWS_MODE = True
 except ImportError:
     _WINDOWS_MODE = False
 
 from craft_cli import errors
 from craft_cli.printer import Printer
 
-# the different modes the Emitter can be set
 EmitterMode = enum.Enum("EmitterMode", "QUIET BRIEF VERBOSE DEBUG TRACE")
+"""The different modes the Emitter can be set."""
 
 # the limit to how many log files to have
 _MAX_LOG_FILES = 5
 
 # the size of bytes chunk that the pipe reader will read at once
 _PIPE_READER_CHUNK_SIZE = 4096
```

### Comparing `craft-cli-2.0.0/craft_cli/printer.py` & `craft-cli-2.0.1/craft_cli/printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,17 @@
         self.prv_msg = msg
 
     def _log(self, message: _MessageInfo) -> None:
         """Write the line message to the log file."""
         # prepare the text with (maybe) the timestamp
         timestamp_str = message.created_at.isoformat(sep=" ", timespec="milliseconds")
         self.log.write(f"{timestamp_str} {message.text}\n")
+        # Flush the file: protect a bit in case of crashes, and multiprocess-based
+        # parallelism.
+        self.log.flush()
 
     def spin(self, message: _MessageInfo, spintext: str) -> None:
         """Write a line message including a spin text, only to a terminal."""
         if _stream_is_terminal(message.stream):
             self._write_line_terminal(message, spintext=spintext)
 
     def show(
```

### Comparing `craft-cli-2.0.0/craft_cli/pytest_plugin.py` & `craft-cli-2.0.1/craft_cli/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/craft_cli.egg-info/PKG-INFO` & `craft-cli-2.0.1/craft_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Command Line Interface
 Author-email: Canonical Ltd <snapcraft@lists.snapcraft.io>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `craft-cli-2.0.0/craft_cli.egg-info/requires.txt` & `craft-cli-2.0.1/craft_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/docs/conf.py` & `craft-cli-2.0.1/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx-pydantic",
     "sphinx_toolbox",
-    "sphinx_toolbox.more_autodoc",
-    "sphinx.ext.autodoc",  # Must be loaded after more_autodoc
+    "sphinx.ext.autodoc",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 show_authors = False
 
@@ -66,14 +65,17 @@
 typehints_document_rtype = True
 
 # Github config
 github_username = "canonical"
 github_repository = "craft-cli"
 # endregion
 
+# Document class properties before public methods
+autodoc_member_order = "bysource"
+
 
 # region Setup reference generation
 def run_apidoc(_):
     from sphinx.ext.apidoc import main
     import os
     import sys
```

### Comparing `craft-cli-2.0.0/docs/explanations.rst` & `craft-cli-2.0.1/docs/explanations.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/docs/howtos.rst` & `craft-cli-2.0.1/docs/howtos.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/docs/index.rst` & `craft-cli-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/docs/tutorials.rst` & `craft-cli-2.0.1/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/examples.py` & `craft-cli-2.0.1/examples.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/pyproject.toml` & `craft-cli-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/conftest.py` & `craft-cli-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/factory.py` & `craft-cli-2.0.1/tests/factory.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/test_pytest_plugin.py` & `craft-cli-2.0.1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_dispatcher.py` & `craft-cli-2.0.1/tests/unit/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_errors.py` & `craft-cli-2.0.1/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_help.py` & `craft-cli-2.0.1/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_messages_emitter.py` & `craft-cli-2.0.1/tests/unit/test_messages_emitter.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_messages_helpers.py` & `craft-cli-2.0.1/tests/unit/test_messages_helpers.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_messages_integration.py` & `craft-cli-2.0.1/tests/unit/test_messages_integration.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_messages_stream_cm.py` & `craft-cli-2.0.1/tests/unit/test_messages_stream_cm.py`

 * *Files identical despite different names*

### Comparing `craft-cli-2.0.0/tests/unit/test_printer.py` & `craft-cli-2.0.1/tests/unit/test_printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Tests that check the whole Printer machinery."""
 
 import re
 import shutil
 import sys
+import textwrap
 import threading
 import time
 from datetime import datetime
 
 import pytest
 
 from craft_cli import printer as printermod
@@ -636,14 +637,37 @@
     msg = _MessageInfo(sys.stdout, "test text", use_timestamp=True, created_at=fake_now)
     printer._log(msg)
     printer.stop()
 
     assert log_filepath.read_text() == "2009-09-01 12:13:15.123 test text\n"
 
 
+def test_logfile_flush(log_filepath, mocker):
+    """Printer flushes the log file after every write."""
+    printer = Printer(log_filepath)
+
+    fake_now = datetime(2009, 9, 1, 12, 13, 15, 123456)
+    msg = _MessageInfo(None, "test text", created_at=fake_now)
+
+    flush = mocker.spy(printer.log, "flush")
+    assert flush.call_count == 0
+    printer._log(msg)
+    assert flush.call_count == 1
+    printer._log(msg)
+    assert flush.call_count == 2
+
+    printer.stop()
+    assert log_filepath.read_text() == textwrap.dedent(
+        """\
+        2009-09-01 12:13:15.123 test text
+        2009-09-01 12:13:15.123 test text
+        """
+    )
+
+
 # -- tests for message showing external API
 
 
 def test_show_defaults_no_stream(recording_printer):
     """Write a message with all defaults (without a stream)."""
     before = datetime.now()
     recording_printer.show(None, "test text")
```

### Comparing `craft-cli-2.0.0/tox.ini` & `craft-cli-2.0.1/tox.ini`

 * *Files identical despite different names*

