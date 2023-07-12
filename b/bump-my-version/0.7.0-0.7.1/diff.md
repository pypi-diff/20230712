# Comparing `tmp/bump-my-version-0.7.0.tar.gz` & `tmp/bump-my-version-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.7.0.tar", last modified: Mon Jul 10 14:55:38 2023, max compression
+gzip compressed data, was "bump-my-version-0.7.1.tar", last modified: Wed Jul 12 12:36:23 2023, max compression
```

## Comparing `bump-my-version-0.7.0.tar` & `bump-my-version-0.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.485710 bump-my-version-0.7.0/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.485710 bump-my-version-0.7.0/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/yaml_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected_full.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/pep440.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_show.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.363640 bump-my-version-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-12 12:36:23.363640 bump-my-version-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.355639 bump-my-version-0.7.1/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 12:36:23.000000 bump-my-version-0.7.1/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.355639 bump-my-version-0.7.1/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/bumpversion/yaml_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 12:36:23.363640 bump-my-version-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.359640 bump-my-version-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.359640 bump-my-version-0.7.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected_full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.359640 bump-my-version-0.7.1/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.359640 bump-my-version-0.7.1/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:36:23.363640 bump-my-version-0.7.1/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/fixtures/pep440.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-12 12:36:01.000000 bump-my-version-0.7.1/tests/test_yaml.py
```

### Comparing `bump-my-version-0.7.0/CHANGELOG.md` & `bump-my-version-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## 0.7.1 (2023-07-12)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.7.0...0.7.1)
+
+### Fixes
+
+- Fix search and replace options for replace. [781e8d8](https://github.com/callowayproject/bump-my-version/commit/781e8d8094ba9f16d915a551b3bc51bd6aa54cfa)
+    
+  - The `--search` and `--replace` options now completely override any other search and replace logic.
+
+  Fixes #34
+### Other
+
+- [pre-commit.ci] pre-commit autoupdate. [531738d](https://github.com/callowayproject/bump-my-version/commit/531738d62d3a2583c7831d17151cb8ae7b14677c)
+    
+  **updates:** - [github.com/astral-sh/ruff-pre-commit: v0.0.276 → v0.0.277](https://github.com/astral-sh/ruff-pre-commit/compare/v0.0.276...v0.0.277)
+
+- [pre-commit.ci] pre-commit autoupdate. [61e6747](https://github.com/callowayproject/bump-my-version/commit/61e6747529b347530c7ef3e7a6fe13c19cbe61d9)
+    
+  **updates:** - https://github.com/charliermarsh/ruff-pre-commit → https://github.com/astral-sh/ruff-pre-commit
+
+
 ## 0.7.0 (2023-07-10)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.6.0...0.7.0)
 
 ### Fixes
 
 - Fixed test coverage. [3fe96f0](https://github.com/callowayproject/bump-my-version/commit/3fe96f0e244ab5be4f96ec8ecbe1ca63f1f06e6b)
```

### Comparing `bump-my-version-0.7.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/CONTRIBUTING.md` & `bump-my-version-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/LICENSE` & `bump-my-version-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/PKG-INFO` & `bump-my-version-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.7.0
+Version: 0.7.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.7.0/README.md` & `bump-my-version-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.7.1/bump_my_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.7.0
+Version: 0.7.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.7.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.7.1/bump_my_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/aliases.py` & `bump-my-version-0.7.1/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/autocast.py` & `bump-my-version-0.7.1/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/bump.py` & `bump-my-version-0.7.1/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/cli.py` & `bump-my-version-0.7.1/bumpversion/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,16 +404,14 @@
 
     overrides = get_overrides(
         allow_dirty=allow_dirty,
         current_version=current_version,
         new_version=new_version,
         parse=parse,
         serialize=serialize or None,
-        search=search,
-        replace=replace,
         commit=False,
         tag=False,
         sign_tags=False,
         tag_name=None,
         tag_message=None,
         message=None,
         commit_args=None,
@@ -437,10 +435,10 @@
     if new_version:
         next_version = config.version_config.parse(new_version)
     else:
         next_version = None
 
     ctx = get_context(config, version, next_version)
 
-    configured_files = resolve_file_config(config.files, config.version_config)
+    configured_files = resolve_file_config(config.files, config.version_config, search, replace)
 
     modify_files(configured_files, version, next_version, ctx, dry_run)
```

### Comparing `bump-my-version-0.7.0/bumpversion/config.py` & `bump-my-version-0.7.1/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/exceptions.py` & `bump-my-version-0.7.1/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/files.py` & `bump-my-version-0.7.1/bumpversion/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """Methods for changing files."""
 import glob
 import logging
 from difflib import context_diff
-from typing import List, MutableMapping
+from typing import List, MutableMapping, Optional
 
 from bumpversion.config import FileConfig
 from bumpversion.exceptions import VersionNotFoundError
 from bumpversion.version_part import Version, VersionConfig
 
 logger = logging.getLogger(__name__)
 
 
 class ConfiguredFile:
     """A file to modify in a configured way."""
 
-    def __init__(self, file_cfg: FileConfig, version_config: VersionConfig) -> None:
+    def __init__(
+        self,
+        file_cfg: FileConfig,
+        version_config: VersionConfig,
+        search: Optional[str] = None,
+        replace: Optional[str] = None,
+    ) -> None:
         self.path = file_cfg.filename
         self.parse = file_cfg.parse or version_config.parse_regex.pattern
         self.serialize = file_cfg.serialize or version_config.serialize_formats
-        self.search = file_cfg.search or version_config.search
-        self.replace = file_cfg.replace or version_config.replace
+        self.search = search or file_cfg.search or version_config.search
+        self.replace = replace or file_cfg.replace or version_config.replace
         self.version_config = VersionConfig(
             self.parse, self.serialize, self.search, self.replace, version_config.part_configs
         )
 
     def contains_version(self, version: Version, context: MutableMapping) -> bool:
         """
         Check whether the version is present in the file.
@@ -94,15 +100,16 @@
     ) -> None:
         """Replace the current version with the new version."""
         with open(self.path, "rt", encoding="utf-8") as f:
             file_content_before = f.read()
             file_new_lines = f.newlines[0] if isinstance(f.newlines, tuple) else f.newlines
 
         context["current_version"] = self.version_config.serialize(current_version, context)
-        context["new_version"] = self.version_config.serialize(new_version, context)
+        if new_version:
+            context["new_version"] = self.version_config.serialize(new_version, context)
 
         search_for = self.version_config.search.format(**context)
         replace_with = self.version_config.replace.format(**context)
 
         file_content_after = file_content_before.replace(search_for, replace_with)
 
         if file_content_before == file_content_after and current_version.original:
@@ -123,42 +130,46 @@
                         )
                     )
                 )
             )
         else:
             logger.info("%s file %s", "Would not change" if dry_run else "Not changing", self.path)
 
-        if not dry_run:
+        if not dry_run:  # pragma: no-coverage
             with open(self.path, "wt", encoding="utf-8", newline=file_new_lines) as f:
                 f.write(file_content_after)
 
-    def __str__(self) -> str:
+    def __str__(self) -> str:  # pragma: no-coverage
         return self.path
 
-    def __repr__(self) -> str:
+    def __repr__(self) -> str:  # pragma: no-coverage
         return f"<bumpversion.ConfiguredFile:{self.path}>"
 
 
-def resolve_file_config(files: List[FileConfig], version_config: VersionConfig) -> List[ConfiguredFile]:
+def resolve_file_config(
+    files: List[FileConfig], version_config: VersionConfig, search: Optional[str] = None, replace: Optional[str] = None
+) -> List[ConfiguredFile]:
     """
     Resolve the files, searching and replacing values according to the FileConfig.
 
     Args:
         files: A list of file configurations
         version_config: How the version should be changed
+        search: The search pattern to use instead of any configured search pattern
+        replace: The replace pattern to use instead of any configured replace pattern
 
     Returns:
         A list of ConfiguredFiles
     """
     configured_files = []
     for file_cfg in files:
         if file_cfg.glob:
             configured_files.extend(get_glob_files(file_cfg, version_config))
         else:
-            configured_files.append(ConfiguredFile(file_cfg, version_config))
+            configured_files.append(ConfiguredFile(file_cfg, version_config, search, replace))
 
     return configured_files
 
 
 def modify_files(
     files: List[ConfiguredFile],
     current_version: Version,
@@ -177,30 +188,34 @@
         dry_run: True if this should be a report-only job
     """
     _check_files_contain_version(files, current_version, context)
     for f in files:
         f.replace_version(current_version, new_version, context, dry_run)
 
 
-def get_glob_files(file_cfg: FileConfig, version_config: VersionConfig) -> List[ConfiguredFile]:
+def get_glob_files(
+    file_cfg: FileConfig, version_config: VersionConfig, search: Optional[str] = None, replace: Optional[str] = None
+) -> List[ConfiguredFile]:
     """
     Return a list of files that match the glob pattern.
 
     Args:
         file_cfg: The file configuration containing the glob pattern
         version_config: The version configuration
+        search: The search pattern to use instead of any configured search pattern
+        replace: The replace pattern to use instead of any configured replace pattern
 
     Returns:
         A list of resolved files according to the pattern.
     """
     files = []
     for filename_glob in glob.glob(file_cfg.glob, recursive=True):
         new_file_cfg = file_cfg.copy()
         new_file_cfg.filename = filename_glob
-        files.append(ConfiguredFile(new_file_cfg, version_config))
+        files.append(ConfiguredFile(new_file_cfg, version_config, search, replace))
     return files
 
 
 def _check_files_contain_version(
     files: List[ConfiguredFile], current_version: Version, context: MutableMapping
 ) -> None:
     """Make sure files exist and contain version string."""
```

### Comparing `bump-my-version-0.7.0/bumpversion/functions.py` & `bump-my-version-0.7.1/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/logging.py` & `bump-my-version-0.7.1/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/scm.py` & `bump-my-version-0.7.1/bumpversion/scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/show.py` & `bump-my-version-0.7.1/bumpversion/show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/utils.py` & `bump-my-version-0.7.1/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/version_part.py` & `bump-my-version-0.7.1/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/bumpversion/yaml_dump.py` & `bump-my-version-0.7.1/bumpversion/yaml_dump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/pyproject.toml` & `bump-my-version-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.7.0"
+current_version = "0.7.1"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.7.0/tests/conftest.py` & `bump-my-version-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.txt` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.yaml` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected.yaml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected_full.json` & `bump-my-version-0.7.1/tests/fixtures/basic_cfg_expected_full.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/fixtures/pep440.toml` & `bump-my-version-0.7.1/tests/fixtures/pep440.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_autocast.py` & `bump-my-version-0.7.1/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_bump.py` & `bump-my-version-0.7.1/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_cli.py` & `bump-my-version-0.7.1/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for `bumpversion` package."""
 import shutil
 import subprocess
+import traceback
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner, Result
 from pytest import param
 
 from bumpversion import __version__, cli
@@ -425,7 +426,66 @@
 
     assert result.exit_code == 0
 
     call_args = mocked_modify_files.call_args[0]
     configured_files = call_args[0]
     assert len(configured_files) == 1
     assert configured_files[0].path == "VERSION"
+
+
+TEST_REPLACE_CONFIG = {
+    "tool": {
+        "bumpversion": {
+            "allow_dirty": True,
+            "commit": False,
+            "current_version": "2.17.7",
+            "files": [],
+            "message": "Bump version: {current_version} → {new_version}",
+            "parse": "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)",
+            "parts": {
+                "major": {},
+                "minor": {},
+                "patch": {},
+            },
+            "replace": "{new_version}",
+            "search": "{current_version}",
+            "serialize": ["{major}.{minor}.{patch}"],
+            "sign_tags": False,
+            "tag": False,
+            "tag_message": "Bump version: {current_version} → {new_version}",
+            "tag_name": "v{new_version}",
+        }
+    }
+}
+
+
+def test_replace_search_with_plain_string(tmp_path, fixtures_path):
+    """Replace should not worry if the search or replace values have version info."""
+    from tomlkit import dumps
+
+    # Arrange
+    config_path = tmp_path / "pyproject.toml"
+    config_path.write_text(dumps(TEST_REPLACE_CONFIG))
+    doc_path = tmp_path / "docs.yaml"
+    doc_path.write_text("url: https://github.com/sampleuser/workflows/main/.github/update_mailmap.py")
+
+    runner: CliRunner = CliRunner()
+    with inside_dir(tmp_path):
+        result: Result = runner.invoke(
+            cli.cli,
+            [
+                "replace",
+                "--no-configured-files",
+                "--search",
+                "/workflows/main/",
+                "--replace",
+                "/workflows/v{current_version}/",
+                "./docs.yaml",
+            ],
+        )
+
+    if result.exit_code != 0:
+        print("Here is the output:")
+        print(result.output)
+        print(traceback.print_exception(result.exc_info[1]))
+
+    assert result.exit_code == 0
```

### Comparing `bump-my-version-0.7.0/tests/test_config.py` & `bump-my-version-0.7.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_files.py` & `bump-my-version-0.7.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_functions.py` & `bump-my-version-0.7.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_scm.py` & `bump-my-version-0.7.1/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_show.py` & `bump-my-version-0.7.1/tests/test_show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_version_part.py` & `bump-my-version-0.7.1/tests/test_version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.7.0/tests/test_yaml.py` & `bump-my-version-0.7.1/tests/test_yaml.py`

 * *Files identical despite different names*

