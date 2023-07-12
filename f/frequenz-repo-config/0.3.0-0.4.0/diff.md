# Comparing `tmp/frequenz-repo-config-0.3.0.tar.gz` & `tmp/frequenz-repo-config-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-repo-config-0.3.0.tar", last modified: Sat Jul  1 07:04:01 2023, max compression
+gzip compressed data, was "frequenz-repo-config-0.4.0.tar", last modified: Wed Jul 12 15:48:46 2023, max compression
```

## Comparing `frequenz-repo-config-0.3.0.tar` & `frequenz-repo-config-0.4.0.tar`

### file list

```diff
@@ -1,127 +1,371 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.cookiecutter-replay.json
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.darglint
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/feature.yml
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/RELEASE_NOTES.template.md
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/keylabeler.yml
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     8141 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/dco-merge-queue.yml
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     4344 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)    15982 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/local_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/feature.yml
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/RELEASE_NOTES.template.md
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/keylabeler.yml
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     8243 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/dco-merge-queue.yml
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     5645 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/{{cookiecutter.name}}.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4637 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)     8118 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/src/frequenz/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/src/frequenz/repo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/
--rw-r--r--   0 runner    (1001) docker     (122)    10857 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/mkdocs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/
--rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8792 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3726 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     6943 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/grpc_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/integration/test_cookiecutter_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/nox/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/nox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/nox/test_default.py
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/test_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.cookiecutter-replay.json
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.darglint
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/hooks/pre_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7246 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/local_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/variable-reference.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     9052 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     5645 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3769 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name | as_identifier}}/
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name | as_identifier}}/{{cookiecutter.name | as_identifier}}.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name | as_identifier}}/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name | as_identifier}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name | as_identifier}}/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.239348 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name | as_identifier}}.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8605 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/src/frequenz/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/src/frequenz/repo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/src/frequenz/repo/config/
+-rw-r--r--   0 runner    (1001) docker     (122)    10857 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/mkdocs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8792 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3726 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6943 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/src/frequenz/repo/config/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/setuptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/src/frequenz/repo/config/setuptools/grpc_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21042 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-12 15:48:46.000000 frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     8888 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/integration/test_cookiecutter_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/tests/nox/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/nox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/nox/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/test_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.243348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/cookiecutter-stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/cookiecutter-stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.cookiecutter-replay.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4321 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/actor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/actor/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/actor/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/actor/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.247348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/cookiecutter-stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/cookiecutter-stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.cookiecutter-replay.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8854 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/proto/frequenz/api/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/proto/frequenz/api/test/test.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/frequenz/api/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/frequenz/api/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/py/frequenz/api/test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3331 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/pytests/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/api/frequenz-api-test/pytests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.251348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/cookiecutter-stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/cookiecutter-stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4290 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.cookiecutter-replay.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.231348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/frequenz/app/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/frequenz/app/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/frequenz/app/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/src/frequenz/app/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/app/frequenz-app-test/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/cookiecutter-stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/cookiecutter-stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.255348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/
+-rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.cookiecutter-replay.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4317 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/src/frequenz/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/src/frequenz/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/src/frequenz/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/lib/frequenz-test-python/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/cookiecutter-stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/cookiecutter-stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4295 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.cookiecutter-replay.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.259348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.235348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/frequenz/model/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/frequenz/model/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/frequenz/model/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/src/frequenz/model/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:48:46.263348 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-12 15:48:35.000000 frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/tests/test_test.py
```

### Comparing `frequenz-repo-config-0.3.0/.cookiecutter-replay.json` & `frequenz-repo-config-0.4.0/.cookiecutter-replay.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998015873015873%*

 * *Differences: {"'cookiecutter'": "{'_extensions': {insert: [(1, 'local_extensions.as_identifier')]}}"}*

```diff
@@ -1,11 +1,12 @@
 {
     "cookiecutter": {
         "_extensions": [
             "jinja2_time.TimeExtension",
+            "local_extensions.as_identifier",
             "local_extensions.default_codeowners",
             "local_extensions.github_repo_name",
             "local_extensions.keywords",
             "local_extensions.pypi_package_name",
             "local_extensions.python_package",
             "local_extensions.src_path",
             "local_extensions.title"
```

### Comparing `frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/bug.yml` & `frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/config.yml` & `frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/feature.yml` & `frequenz-repo-config-0.4.0/.github/ISSUE_TEMPLATE/feature.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.github/dependabot.yml` & `frequenz-repo-config-0.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.github/keylabeler.yml` & `frequenz-repo-config-0.4.0/.github/keylabeler.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.github/workflows/ci.yaml` & `frequenz-repo-config-0.4.0/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
       - name: Install required Python packages
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e .[dev-noxfile]
 
       - name: Run nox
-        # To speed things up a bit we use the speciall ci_checks_max session
+        # To speed things up a bit we use the special ci_checks_max session
         # that uses the same venv to run multiple linting sessions
         run: nox -e ci_checks_max pytest_min
         timeout-minutes: 60
 
   build:
     name: Build distribution packages
     runs-on: ubuntu-20.04
```

### Comparing `frequenz-repo-config-0.3.0/.github/workflows/labeler.yml` & `frequenz-repo-config-0.4.0/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/.gitignore` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/CONTRIBUTING.md` & `frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contributing to Frequenz Repository Configuration
+# Contributing to Frequenz Test Actor
 
 ## Build
 
 You can use `build` to simply build the source and binary distribution:
 
 ```sh
 python -m pip install build
@@ -135,17 +135,17 @@
    git tag -s --cleanup=whitespace -F RELEASE_NOTES.md v0.0.1
    ```
 
 4. Push the new tag.
 
 5. A GitHub action will test the tag and if all goes well it will create
    a [GitHub
-   Release](https://github.com/frequenz-floss/frequenz-repo-config-python/releases),
+   Release](https://github.com/frequenz-floss/frequenz-actor-test/releases),
    and upload a new package to
-   [PyPI](https://pypi.org/project/frequenz-repo-config/)
+   [PyPI](https://pypi.org/project/frequenz-actor-test/)
    automatically.
 
 6. Once this is done, reset the `RELEASE_NOTES.md` with the template:
 
    ```sh
    cp .github/RELEASE_NOTES.template.md RELEASE_NOTES.md
    ```
```

### Comparing `frequenz-repo-config-0.3.0/LICENSE` & `frequenz-repo-config-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/PKG-INFO` & `frequenz-repo-config-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-repo-config
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frequenz repository setup tools and common configuration
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-repo-config-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-repo-config-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-repo-config-python
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-repo-config-python/discussions/categories/support
```

### Comparing `frequenz-repo-config-0.3.0/README.md` & `frequenz-repo-config-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/hooks/post_gen_project.py` & `frequenz-repo-config-0.4.0/cookiecutter/hooks/post_gen_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This module contains post-generation hooks to adjust the generated project to the
 different types of projects and do some final checks and configuration.
 """
 
 import configparser as _configparser
 import dataclasses as _dataclasses
 import json as _json
+import os
 import pathlib as _pathlib
 import shutil as _shutil
 import subprocess as _subprocess
 from collections import namedtuple
 from typing import Any
 
 
@@ -26,15 +27,15 @@
     Returns:
         The named tuple with the same keys and values as the dictionary.
     """
     filtered = {k: v for k, v in dictionary.items() if not k.startswith("_")}
     return namedtuple("Cookiecutter", filtered.keys())(*filtered.values())
 
 
-cookiecutter = to_named_tuple(_json.loads("""{{cookiecutter | tojson}}"""))
+cookiecutter = to_named_tuple(_json.loads(r"""{{cookiecutter | tojson}}"""))
 
 
 def main() -> None:
     """Run some post-generation steps.
 
     This function is called after the project has been generated and it performs
     some fixes for different types of projects and some sanity checks.
@@ -137,18 +138,45 @@
 
     if dst.exists():
         print(f"Replay file {dst} already exists. Skipping...")
         return
 
     if not src.exists():
         print(f"WARNING: No replay file found in {src}. Skipping...")
+        return
 
     try:
-        _shutil.copyfile(src, dst)
-    except (OSError, IOError) as error:
+        with src.open("r", encoding="utf8") as input_file:
+            replay_data = _json.load(input_file)
+
+        # Remove the _output_dir key from the replay data because it is an absolute path
+        # that depends on the current environment and we don't want to add it as part of
+        # the generated project.
+        replay_data["cookiecutter"].pop("_output_dir", None)
+
+        if template := replay_data["cookiecutter"].get("_template"):
+            if not template.startswith(("gh:", "git@", "https://")):
+                print(
+                    f"WARNING: The replay file's `_template` ({template}) doesn't seem "
+                    "to be a remote repository, it won't be saved to avoid storing a "
+                    "local template in the new repository. If this is incorrect, "
+                    f"please add it back manually to {dst}."
+                )
+                replay_data["cookiecutter"].pop("_template", None)
+
+        with dst.open("w", encoding="utf8") as output_file:
+            _json.dump(replay_data, output_file, indent=2)
+    except KeyError as error:
+        print(
+            f"WARNING: Error parsing the replay file {src} -> {dst} ({error}). "
+            "Skipping..."
+        )
+    # We want to catch a broad range of exceptions here because we don't want to fail
+    # the whole generation process just because the replay file is broken.
+    except Exception as error:  # pylint: disable=broad-except
         print(
             f"WARNING: Error copying the replay file {src} -> {dst} ({error}). "
             "Skipping..."
         )
 
 
 def initialize_git_submodules() -> bool:
@@ -158,14 +186,19 @@
     the git submodules using `git submodule update --init --recursive`.
 
     If an empty `.gitmodules` file exists, it will be deleted.
 
     Returns:
         Whether any git submodules were initialized.
     """
+    if is_golden_testing():
+        # We don't use external tools when running tests because they are too flaky, as
+        # different versions emit different outputs
+        return False
+
     gitmodules_path = _pathlib.Path(".gitmodules")
 
     if not gitmodules_path.exists():
         return False
 
     if not gitmodules_path.is_file():
         warn("`.gitmodules` exists but is not a file! Ignoring...")
@@ -256,16 +289,22 @@
     `git init`.
 
     If the project is already a git repository, it will be left untouched.
 
     Returns:
         Whether the project was initialized as a git repository.
     """
+    if is_golden_testing():
+        # We don't use external tools when running tests because they are too flaky, as
+        # different versions emit different outputs
+        return False
+
     if _pathlib.Path(".git").exists():
         return False
+
     print()
     note("Initializing git repository...")
     try_run(
         ["git", "init"],
         verbose=True,
         warn_on_error=True,
         warn_on_bad_status="Failed to initialize the git repository!",
@@ -278,14 +317,19 @@
     """Commit all changes in the git repository.
 
     If there are no changes to commit, this function does nothing.
 
     Args:
         first_commit: Whether this is the first commit in the git repository.
     """
+    if is_golden_testing():
+        # We don't use external tools when running tests because they are too flaky, as
+        # different versions emit different outputs
+        return
+
     if not try_run(["git", "status", "--porcelain"]):
         return
 
     print()
     try_run(
         ["git", "add", "."],
         verbose=True,
@@ -336,29 +380,35 @@
     with path.open("r", encoding="utf8") as file_handle:
         contents = file_handle.read(1024).strip()
         return not contents
 
 
 def print_generated_tree() -> None:
     """Print the generated files tree."""
+    if is_golden_testing():
+        # We don't use external tools when running tests because they are too flaky, as
+        # different versions emit different outputs
+        return
+
     result = try_run(["tree"])
     if result is not None and result.returncode == 0:
         print()
 
 
 def print_todos() -> None:
     """Print all TODOs in the generated project."""
     todo_str = "TODO(cookiecutter):"
     repo = cookiecutter.github_repo_name
-    cmd = ["grep", "-r", "--color", rf"\<{todo_str}.*", "."]
+    cmd = rf"grep -r --color '\<{todo_str}.*' . | sort"
     try_run(
         cmd,
         warn_on_error=True,
-        warn_on_bad_status=f"No `{todo_str}` found using `{' '.join(cmd)}`",
+        warn_on_bad_status=f"No `{todo_str}` found using `{cmd}`",
         note_on_failure=f"Please search for `{todo_str}` in `{repo}/` manually.",
+        shell=True,
     )
     print()
     note(
         "Make sure to (create and) configure your GitHub repository too: "
         "https://github.com/frequenz-floss/frequenz-repo-config-python/"
         "wiki/Configuring-a-new-GitHub-repository"
     )
@@ -420,61 +470,66 @@
     Operations performed by this function:
 
     * Avoid having a subfolder for the type
 
       - `lib`: `src/frequenz/{name}`
       - `rest`: `src/frequenz/{type}/{name}`
     """
+    name = cookiecutter.name.lower().replace("-", "_")
     recursive_overwrite_move(
-        _pathlib.Path(f"src/frequenz/{cookiecutter.type}/{cookiecutter.name}"),
-        _pathlib.Path(f"src/frequenz/{cookiecutter.name}"),
+        _pathlib.Path(f"src/frequenz/{cookiecutter.type}/{name}"),
+        _pathlib.Path(f"src/frequenz/{name}"),
     )
     _pathlib.Path(f"src/frequenz/{cookiecutter.type}").rmdir()
 
 
 def finish_model_setup() -> None:
     """Finish the setup for a model.
 
     This function is called after the project has been generated and can be used
     to perform any additional setup steps that are required for a model.
     """
 
 
 def try_run(
-    cmd: list[str],
+    cmd: list[str] | str,
     /,
     *,
     warn_on_error: bool = False,
     warn_on_bad_status: str | None = None,
     note_on_failure: str | None = None,
     verbose: bool = False,
+    shell: bool = False,
 ) -> _subprocess.CompletedProcess[Any] | None:
     """Try to run a command.
 
     Args:
         cmd: The command to run.
         warn_on_error: Whether to warn on errors (like command not found) of fail
             silently.
         warn_on_bad_status: If not `None`, warn if the command fails with a non-zero
             status code and use this string as the warning message (the status code
             will be appended to the message).
         note_on_failure: If not `None`, print this note if the command fails (either
             because of an error or a non-zero status code).
         verbose: Whether to print the command before running it.
+        shell: Whether to run the command in a shell. If `True`, `cmd` must be a
+            string, otherwise it must be a list of strings.
 
     Returns:
         The result of the command or `None` if the command could not be run because
         of an error.
     """
+    assert isinstance(cmd, str) and shell or isinstance(cmd, list) and not shell
     result = None
     failed = False
     if verbose:
         print(f"Executing: {' '.join(cmd)}")
     try:
-        result = _subprocess.run(cmd, check=False)
+        result = _subprocess.run(cmd, check=False, shell=shell)
     except (OSError, _subprocess.CalledProcessError) as exc:
         if warn_on_error:
             warn(f"Failed to run the search command `{' '.join(cmd)}`: {exc}")
         failed = True
     else:
         if result.returncode != 0:
             if warn_on_bad_status is not None:
@@ -482,14 +537,23 @@
             failed = True
     if failed and note_on_failure is not None:
         note(note_on_failure)
 
     return result
 
 
+def is_golden_testing() -> bool:
+    """Return `True` if we are running as part of a golden testing.
+
+    Returns:
+        Whether we are running as part of a golden testing.
+    """
+    return os.environ.get("GOLDEN_TEST", None) is not None
+
+
 def recursive_overwrite_move(src: _pathlib.Path, dst: _pathlib.Path) -> None:
     """Recursively move a directory overwriting the target files if they exist.
 
     Useful when overwriting an existing project to update it.
 
     Args:
         src: The source directory.
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/bug.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/config.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/feature.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/feature.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/dependabot.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/keylabeler.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/keylabeler.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/labeler.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/labeler.yml`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,26 @@
 # For more details on the configuration please see:
 # https://github.com/marketplace/actions/labeler
 
 # TODO(cookiecutter): Add different parts of the source
 # For example:
 #
 # "part:module":
-#   - "src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/module/**"
+#   - "src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name | as_identifier}}/module/**"
 #
 # "part:other":
-#   - "src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/other/**"
+#   - "src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name | as_identifier}}/other/**"
+#
+# # For excluding some files (in this example, label "part:complicated"
+# # everything inside src/ with a .py suffix, except for src/__init__.py)
+# "part:complicated":
+#   - any:
+#       - "src/**/*.py"
+#   - all:
+#       - "!src/__init__.py"
 #
 # Please have in mind that that the part:xxx labels need to
 # be created in the GitHub repository.
 
 "part:docs":
   - "**/*.md"
   - "docs/**"
@@ -34,10 +42,11 @@
 "part:tooling":
   - "**/*.ini"
   - "**/*.toml"
   - "**/*.yaml"
   - "**/*.yml"
   - ".git*"
   - ".git*/**"
+  - "docs/*.py"
   - CODEOWNERS
   - MANIFEST.in
   - noxfile.py
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/ci.yaml` & `frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -28,48 +28,48 @@
     strategy:
       fail-fast: false
       matrix:
         os:
           - ubuntu-20.04
         python:
           - "3.11"
-    runs-on: {{'${{ matrix.os }}'}}
+    runs-on: ${{ matrix.os }}
 
     steps:
       - name: Fetch sources
         uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: {{'${{ matrix.python }}'}}
+          python-version: ${{ matrix.python }}
           cache: 'pip'
 
       - name: Install required Python packages
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e .[dev-noxfile]
 
       - name: Run nox
-        # To speed things up a bit we use the speciall ci_checks_max session
+        # To speed things up a bit we use the special ci_checks_max session
         # that uses the same venv to run multiple linting sessions
         run: nox -e ci_checks_max pytest_min
         timeout-minutes: 10
 
   build:
     name: Build distribution packages
     runs-on: ubuntu-20.04
     steps:
       - name: Fetch sources
         uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: {{'${{ env.DEFAULT_PYTHON_VERSION }}'}}
+          python-version: ${{ env.DEFAULT_PYTHON_VERSION }}
           cache: 'pip'
 
       - name: Install required Python packages
         run: |
           python -m pip install -U pip
           python -m pip install -U build
 
@@ -93,25 +93,25 @@
 
       - name: Setup Git user and e-mail
         uses: frequenz-floss/setup-git-user@v2
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: {{'${{ env.DEFAULT_PYTHON_VERSION }}'}}
+          python-version: ${{ env.DEFAULT_PYTHON_VERSION }}
           cache: 'pip'
 
       - name: Install build dependencies
         run: |
           python -m pip install -U pip
           python -m pip install .[dev-mkdocs]
 
       - name: Generate the documentation
         env:
-          MIKE_VERSION: gh-{{'${{ github.job }}'}}
+          MIKE_VERSION: gh-${{ github.job }}
         run: |
           mike deploy $MIKE_VERSION
           mike set-default $MIKE_VERSION
 
       - name: Upload site
         uses: actions/upload-artifact@v3
         with:
@@ -126,17 +126,17 @@
     runs-on: ubuntu-20.04
     permissions:
       contents: write
     steps:
       - name: Calculate and check version
         id: mike-metadata
         env:
-          REF: {{'${{ github.ref }}'}}
-          REF_NAME: {{'${{ github.ref_name }}'}}
-          DEFAULT_BRANCH: {{'${{ github.event.repository.default_branch }}'}}
+          REF: ${{ github.ref }}
+          REF_NAME: ${{ github.ref_name }}
+          DEFAULT_BRANCH: ${{ github.event.repository.default_branch }}
         run: |
           aliases=
           version=
           if test "$REF_NAME" = "$DEFAULT_BRANCH"
           then
             version=next
           # A tag that starts with vX.Y or X.Y
@@ -172,15 +172,15 @@
         if: steps.mike-metadata.outputs.version
         uses: frequenz-floss/setup-git-user@v2
 
       - name: Set up Python
         if: steps.mike-metadata.outputs.version
         uses: actions/setup-python@v4
         with:
-          python-version: {{'${{ env.DEFAULT_PYTHON_VERSION }}'}}
+          python-version: ${{ env.DEFAULT_PYTHON_VERSION }}
           cache: 'pip'
 
       - name: Install build dependencies
         if: steps.mike-metadata.outputs.version
         run: |
           python -m pip install -U pip
           python -m pip install .[dev-mkdocs]
@@ -188,16 +188,16 @@
       - name: Fetch the gh-pages branch
         if: steps.mike-metadata.outputs.version
         run: git fetch origin gh-pages --depth=1
 
       - name: Publish site
         if: steps.mike-metadata.outputs.version
         env:
-          VERSION: {{'${{ steps.mike-metadata.outputs.version }}'}}
-          ALIASES: {{'${{ steps.mike-metadata.outputs.aliases }}'}}
+          VERSION: ${{ steps.mike-metadata.outputs.version }}
+          ALIASES: ${{ steps.mike-metadata.outputs.aliases }}
         run: |
           mike deploy --push --update-aliases "$VERSION" $ALIASES
 
   create-github-release:
     name: Create GitHub release
     needs: ["publish-docs"]
     # Create a release only on tags creation
@@ -221,34 +221,34 @@
           gh api \
               -X GET \
               -f ref=$REF \
               -H "Accept: application/vnd.github.raw" \
               "/repos/$REPOSITORY/contents/RELEASE_NOTES.md" \
             > RELEASE_NOTES.md
         env:
-          REF: {{'${{ github.ref }}'}}
-          REPOSITORY: {{'${{ github.repository }}'}}
-          GH_TOKEN: {{'${{ secrets.GITHUB_TOKEN }}'}}
+          REF: ${{ github.ref }}
+          REPOSITORY: ${{ github.repository }}
+          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Create GitHub release
         run: |
           set -ux
           extra_opts=
           if echo "$REF_NAME" | grep -- -; then extra_opts=" --prerelease"; fi
           gh release create \
             -R "$REPOSITORY" \
             --notes-file RELEASE_NOTES.md \
             --generate-notes \
             $extra_opts \
             $REF_NAME \
             dist/*
         env:
-          REF_NAME: {{'${{ github.ref_name }}'}}
-          REPOSITORY: {{'${{ github.repository }}'}}
-          GH_TOKEN: {{'${{ secrets.GITHUB_TOKEN }}'}}
+          REF_NAME: ${{ github.ref_name }}
+          REPOSITORY: ${{ github.repository }}
+          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   publish-to-pypi:
     name: Publish packages to PyPI
     needs: ["create-github-release"]
     runs-on: ubuntu-20.04
     permissions:
       # For trusted publishing. See:
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/labeler.yml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore` & `frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/.gitignore`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/CONTRIBUTING.md` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/mkdocstrings.css` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/style.css` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/logo.png` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/mkdocs.yml` & `frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/model/frequenz-model-test/mkdocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # MkDocs configuration
 # For details see: https://www.mkdocs.org/user-guide/configuration/
 
 # Project information
-site_name: "{{cookiecutter.title}}"
-site_description: "{{cookiecutter.description}}"
-site_author: "{{cookiecutter.author_name}}"
-copyright: "Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}"
-repo_name: "{{cookiecutter.github_repo_name}}"
-repo_url: "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}"
+site_name: "Frequenz Test AI Model"
+site_description: "Test description"
+site_author: "Frequenz Energy-as-a-Service GmbH"
+copyright: "Copyright © 2023 Frequenz Energy-as-a-Service GmbH"
+repo_name: "frequenz-model-test"
+repo_url: "https://github.com/frequenz-floss/frequenz-model-test"
 # TODO(cookiecutter): "main" is the GitHub repo default branch, you might want to update it
 # if the project uses a different default branch.
 edit_uri: "edit/main/docs/"
 strict: true  # Treat warnings as errors
 
 # Build directories
 theme:
@@ -21,14 +21,16 @@
   favicon: logo.png
   language: en
   icon:
     edit: material/file-edit-outline
     repo: fontawesome/brands/github
   custom_dir: docs/overrides
   features:
+    - content.code.annotate
+    - content.code.copy
     - navigation.instant
     - navigation.tabs
     - navigation.top
     - navigation.tracking
     - toc.follow
   palette:
   - media: "(prefers-color-scheme: light)"
@@ -45,15 +47,15 @@
     toggle:
       icon: material/weather-night
       name: Switch to light mode
 
 extra:
   social:  # TODO(cookiecutter): You probably want to update the links
   - icon: fontawesome/brands/github
-    link: https://github.com/{{cookiecutter.github_org}}
+    link: https://github.com/frequenz-floss
   - icon: fontawesome/brands/linkedin
     link: https://www.linkedin.com/company/frequenz-com
   version:
     provider: mike
     default: latest
 
 extra_css:
@@ -61,24 +63,28 @@
   - css/mkdocstrings.css
 
 # Formatting options
 markdown_extensions:
   - admonition
   - attr_list
   - pymdownx.details
-  - pymdownx.superfences
-  - pymdownx.tasklist
-  - pymdownx.tabbed
+  - pymdownx.highlight:
+      anchor_linenums: true
+      line_spans: __span
+      pygments_lang_class: true
+  - pymdownx.keys
   - pymdownx.snippets:
       check_paths: true
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: "!!python/name:pymdownx.superfences.fence_code_format"
+  - pymdownx.tabbed
+  - pymdownx.tasklist
   - toc:
       permalink: "¤"
 
 plugins:
   - gen-files:
       scripts:
         - docs/mkdocstrings_autoapi.py
@@ -88,26 +94,29 @@
       canonical_version: latest
   - mkdocstrings:
       custom_templates: templates
       default_handler: python
       handlers:
         python:
           options:
-            paths: ["{{cookiecutter | src_path}}"]
+            paths: ["src"]
             docstring_section_style: spacy
             merge_init_into_class: false
             show_category_heading: true
             show_root_heading: true
             show_root_members_full_path: true
             show_source: true
           import:
             # TODO(cookiecutter): You might want to add other external references here
             # See https://mkdocstrings.github.io/python/usage/#import for details
             - https://docs.python.org/3/objects.inv
+            - https://frequenz-floss.github.io/frequenz-channels-python/v0.14/objects.inv
+            - https://frequenz-floss.github.io/frequenz-sdk-python/v0.22/objects.inv
+            - https://typing-extensions.readthedocs.io/en/stable/objects.inv
   - search
   - section-index
 
 # Preview controls
 watch:
-  - "{{cookiecutter | src_path}}"
+  - "src"
   - README.md
   - CONTRIBUTING.md
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# License: MIT
+# License: {{cookiecutter.license}}
 # Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
 [build-system]
 requires = [
   "setuptools == 67.7.2",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[{{cookiecutter.type}}] == 0.2.0",
+  "frequenz-repo-config[{{cookiecutter.type}}] == 0.4.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "{{cookiecutter.pypi_package_name}}"
 description = "{{cookiecutter.description}}"
 readme = "README.md"
@@ -30,15 +30,18 @@
   {%- endif %}
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 {%- if cookiecutter.type in ("app", "actor", "model") %}
 dependencies = [ # TODO(cookiecutter): Remove and add more if appropriate
   "typing-extensions == 4.5.0",
-  "frequenz-sdk == 0.20.0",
+  # Make sure to update the mkdocs.yml file when
+  # changing the version
+  # (plugins.mkdocstrings.handlers.python.import)
+  "frequenz-sdk == 0.22.0",
 ]
 {%- elif cookiecutter.type == "api" %}
 dependencies = [ # TODO(cookiecutter): Remove and add more if appropriate
   "frequenz-api-common >= 0.2.0, < 0.3.0",
   "googleapis-common-protos >= 1.56.2, < 2",
   "grpcio >= 1.51.1, < 2",
 ]
@@ -63,23 +66,24 @@
 dev-mkdocs = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.0",
   "mkdocs-material == 9.1.16",
   "mkdocs-section-index == 0.3.5",
   "mkdocstrings[python] == 0.22.0",
+  "frequenz-repo-config[{{cookiecutter.type}}] == 0.4.0",
 ]
 dev-mypy = [
   "mypy == 1.2.0",
   # For checking the noxfile, docs/ script, and tests
   "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-noxfile = [
   "nox == 2023.4.22",
-  "frequenz-repo-config[{{cookiecutter.type}}] == 0.2.0",
+  "frequenz-repo-config[{{cookiecutter.type}}] == 0.4.0",
 ]
 dev-pylint = [
   "pylint == 2.17.3",
   # For checking the noxfile, docs/ script, and tests
   "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 {%- if cookiecutter.type == "api" %}
@@ -89,15 +93,15 @@
   "pytest == 7.3.1",
   "pytest-mock == 3.10.0",
   "pytest-asyncio == 0.21.0",
   "async-solipsism == 0.5",
 ]
 {%- endif %}
 dev = [
-  "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-docstrings,dev-formatting,dev-gen-docs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
+  "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/releases"
 Issues = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/issues"
 Repository = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}"
 Support = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/discussions/categories/support"
@@ -109,28 +113,31 @@
 include = '\.pyi?$'
 {%- endif %}
 
 [tool.isort]
 profile = "black"
 line_length = 88
 {#- We don't include "py" here for API because we don't want to check generated files #}
-src_paths = ["src", "examples", "tests"]
+src_paths = ["benchmarks", "examples", "src", "tests"]
 
 [tool.pylint.similarities]
 ignore-comments = ['yes']
 ignore-docstrings = ['yes']
 ignore-imports = ['no']
 min-similarity-lines = 40
 
 [tool.pylint.messages_control]
 disable = [
   "too-few-public-methods",
   # disabled because it conflicts with isort
   "wrong-import-order",
   "ungrouped-imports",
+  # pylint's unsubscriptable check is buggy and is not needed because
+  # it is a type-check, for which we already have mypy.
+  "unsubscriptable-object",
 ]
 
 [tool.pytest.ini_options]
 {%- if cookiecutter.type != "api" %}
 testpaths = ["tests"]
 asyncio_mode = "auto"
 required_plugins = ["pytest-asyncio", "pytest-mock"]
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py` & `frequenz-repo-config-0.4.0/tests_golden/integration/test_cookiecutter_generation/actor/frequenz-actor-test/src/frequenz/actor/test/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # License: MIT
-# Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
+# Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
-"""{{cookiecutter.description}}.
+"""Test description.
 
 TODO(cookiecutter): Add a more descriptive module description.
 """
-{%- if cookiecutter.type != "api" %}
 
 
 # TODO(cookiecutter): Remove this function
 def delete_me(*, blow_up: bool = False) -> bool:
     """Do stuff for demonstration purposes.
 
     Args:
@@ -20,8 +19,7 @@
 
     Raises:
         RuntimeError: if blow_up is True.
     """
     if blow_up:
         raise RuntimeError("This function should be removed!")
     return True
-{%- endif %}
```

### Comparing `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py` & `frequenz-repo-config-0.4.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name | as_identifier}}.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# License: MIT
+# License: {{cookiecutter.license}}
 # Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
-"""Tests for the {{cookiecutter.name}} package."""
+"""Tests for the {{cookiecutter.python_package}} package."""
 
 {%- if cookiecutter.type == "api" %}
 
 
 def test_package_import() -> None:
     """Test that the package can be imported."""
     # pylint: disable=import-outside-toplevel
-    from frequenz.api import {{cookiecutter.name}}
+    from frequenz.api import {{cookiecutter.name | as_identifier}}
 
-    assert {{cookiecutter.name}} is not None
+    assert {{cookiecutter.name | as_identifier}} is not None
 
 
 def test_module_import_components() -> None:
     """Test that the modules can be imported."""
     # pylint: disable=import-outside-toplevel
-    from frequenz.api.{{cookiecutter.name}} import {{cookiecutter.name}}_pb2
+    from frequenz.api.{{cookiecutter.name | as_identifier}} import {{cookiecutter.name | as_identifier}}_pb2
 
-    assert {{cookiecutter.name}}_pb2 is not None
+    assert {{cookiecutter.name | as_identifier}}_pb2 is not None
 
     # pylint: disable=import-outside-toplevel
-    from frequenz.api.{{cookiecutter.name}} import {{cookiecutter.name}}_pb2_grpc
+    from frequenz.api.{{cookiecutter.name | as_identifier}} import {{cookiecutter.name | as_identifier}}_pb2_grpc
 
-    assert {{cookiecutter.name}}_pb2_grpc is not None
+    assert {{cookiecutter.name | as_identifier}}_pb2_grpc is not None
 {%- else %}
 import pytest
 
 from {{cookiecutter.python_package}} import delete_me
 
 
-def test_{{cookiecutter.name}}_succeeds() -> None:  # TODO(cookiecutter): Remove
+def test_{{cookiecutter.name | as_identifier}}_succeeds() -> None:  # TODO(cookiecutter): Remove
     """Test that the delete_me function succeeds."""
     assert delete_me() is True
 
 
-def test_{{cookiecutter.name}}_fails() -> None:  # TODO(cookiecutter): Remove
+def test_{{cookiecutter.name | as_identifier}}_fails() -> None:  # TODO(cookiecutter): Remove
     """Test that the delete_me function fails."""
     with pytest.raises(RuntimeError, match="This function should be removed!"):
         delete_me(blow_up=True)
 {%- endif %}
```

### Comparing `frequenz-repo-config-0.3.0/docs/css/mkdocstrings.css` & `frequenz-repo-config-0.4.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/docs/css/style.css` & `frequenz-repo-config-0.4.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/docs/index.md` & `frequenz-repo-config-0.4.0/docs/index.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,29 +27,46 @@
 $ cd cookiecutter
 $ . bin/activate
 [cookiecutter] $ pip install cookiecutter
 Collecting cookiecutter
 ...
 ```
 
-Then simply run [Cookiecutter] where you want to create the new project. A new
-directory will be created with the generated project name. For example:
+Then simply run [Cookiecutter] where you want to create the new project:
 
 ```sh
-cd ~/devel
-cookiecutter gh:frequenz-floss/frequenz-repo-config-python --directory=cookiecutter
+cookiecutter gh:frequenz-floss/frequenz-repo-config-python \
+    --directory=cookiecutter
 ```
 
 This command will prompt you for the project type, name, and other
-configuration options, and it will generate the entire project for you.
+configuration options, and it will generate the entire project for you in a new
+subdirectory.
+
+!!! warning
+
+    This command needs to be typed literally!
+
+    `frequenz-floss/frequenz-repo-config-python` is the GitHub repository with
+    the cookiecutter template that will be downloaded, and
+    `--directory=cookiecutter` is needed because the cookiecutter template
+    doesn't live at the top-level of that repository, but in a subdirectory
+    called `cookiecutter`.
+
+    All information about your project will be prompted interactively by that
+    command.
 
 After completing the project and fixing the `TODO`s, you can either amend the
 previous commit using `git commit --amend` or create a new commit for the
 changes using `git commit`.
 
+### Template variables reference
+
+--8<-- "cookiecutter/variable-reference.md"
+
 ### Create the local development environment
 
 To start development, you need to make sure your environment is correctly set
 up. One way to do this is by using a virtual environment and installing all the
 dependencies there:
 
 ```sh
```

### Comparing `frequenz-repo-config-0.3.0/docs/logo.png` & `frequenz-repo-config-0.4.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/mkdocs.yml` & `frequenz-repo-config-0.4.0/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,16 @@
   favicon: logo.png
   language: en
   icon:
     edit: material/file-edit-outline
     repo: fontawesome/brands/github
   custom_dir: docs/overrides
   features:
+    - content.code.annotate
+    - content.code.copy
     - navigation.instant
     - navigation.tabs
     - navigation.top
     - navigation.tracking
     - toc.follow
   palette:
   - media: "(prefers-color-scheme: light)"
@@ -58,24 +60,28 @@
   - css/mkdocstrings.css
 
 # Formatting options
 markdown_extensions:
   - admonition
   - attr_list
   - pymdownx.details
-  - pymdownx.superfences
-  - pymdownx.tasklist
-  - pymdownx.tabbed
+  - pymdownx.highlight:
+      anchor_linenums: true
+      line_spans: __span
+      pygments_lang_class: true
+  - pymdownx.keys
   - pymdownx.snippets:
       check_paths: true
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: "!!python/name:pymdownx.superfences.fence_code_format"
+  - pymdownx.tabbed
+  - pymdownx.tasklist
   - toc:
       permalink: "¤"
 
 plugins:
   - gen-files:
       scripts:
         - docs/mkdocstrings_autoapi.py
@@ -99,15 +105,17 @@
           import:
             - https://cookiecutter.readthedocs.io/en/stable/objects.inv
             - https://docs.python.org/3/objects.inv
             - https://mkdocstrings.github.io/objects.inv
             - https://nox.thea.codes/en/stable/objects.inv
             - https://setuptools.pypa.io/en/latest/objects.inv
             - https://oprypin.github.io/mkdocs-gen-files/objects.inv
+            - https://typing-extensions.readthedocs.io/en/stable/objects.inv
   - search
   - section-index
 
 # Preview controls
 watch:
+  - "cookiecutter/variable-reference.md"
   - "src"
   - README.md
   - CONTRIBUTING.md
```

### Comparing `frequenz-repo-config-0.3.0/pyproject.toml` & `frequenz-repo-config-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
   "frequenz-repo-config[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
   "pytest == 7.3.1",
   "cookiecutter == 2.1.1", # For checking the cookiecutter scripts
 ]
 dev = [
-  "frequenz-repo-config[dev-mkdocs,dev-docstrings,dev-formatting,dev-gen-docs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
+  "frequenz-repo-config[dev-mkdocs,dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-repo-config-python/releases"
 Issues = "https://github.com/frequenz-floss/frequenz-repo-config-python/issues"
 Repository = "https://github.com/frequenz-floss/frequenz-repo-config-python"
 Support = "https://github.com/frequenz-floss/frequenz-repo-config-python/discussions/categories/support"
@@ -100,34 +100,38 @@
 line-length = 88
 target-version = ['py311']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
 line_length = 88
-src_paths = ["src", "examples", "tests"]
+src_paths = ["benchmarks", "examples", "src", "tests"]
 
 [tool.pylint.similarities]
 ignore-comments = ['yes']
 ignore-docstrings = ['yes']
 ignore-imports = ['no']
 min-similarity-lines = 40
 
 [tool.pylint.messages_control]
 disable = [
   "too-few-public-methods",
   # disabled because it conflicts with isort
   "wrong-import-order",
   "ungrouped-imports",
+  # pylint's unsubscriptable check is buggy and is not needed because
+  # it is a type-check, for which we already have mypy.
+  "unsubscriptable-object",
 ]
 
 [[tool.mypy.overrides]]
 module = ["cookiecutter", "cookiecutter.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 markers = [
   "integration: integration tests (deselect with '-m \"not integration\"')",
 ]
+
 [tool.setuptools_scm]
 version_scheme = "post-release"
```

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/__init__.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 Then you need to add this package as a build dependency and a few extra
 dependencies to your project, for example:
 
 ```toml
 requires = [
   "setuptools >= 67.3.2, < 68",
   "setuptools_scm[toml] >= 7.1.0, < 8",
-  "frequenz-repo-config[api] >= 0.1.0, < 0.2.0",
+  "frequenz-repo-config[api] >= 0.3.0, < 0.4.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
   "frequenz-api-common >= 0.2.0, < 0.3.0",
   "googleapis-common-protos >= 1.56.2, < 2",
```

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/mkdocs.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/mkdocs.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/__init__.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/config.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/config.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/default.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/default.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/session.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/session.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/util.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/nox/util.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/protobuf.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/protobuf.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/grpc_tools.py` & `frequenz-repo-config-0.4.0/src/frequenz/repo/config/setuptools/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/PKG-INFO` & `frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-repo-config
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frequenz repository setup tools and common configuration
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-repo-config-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-repo-config-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-repo-config-python
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-repo-config-python/discussions/categories/support
```

### Comparing `frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/requires.txt` & `frequenz-repo-config-0.4.0/src/frequenz_repo_config.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 grpcio-tools<2,>=1.47.0
 mypy-protobuf<4,>=3.0.0
 setuptools<68,>=67.6.0
 
 [app]
 
 [dev]
-frequenz-repo-config[dev-docstrings,dev-formatting,dev-gen-docs,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
+frequenz-repo-config[dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-docstrings]
 pydocstyle==6.3.0
 darglint==1.8.1
 tomli==2.0.1
 
 [dev-formatting]
```

### Comparing `frequenz-repo-config-0.3.0/tests/nox/test_default.py` & `frequenz-repo-config-0.4.0/tests/nox/test_default.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.3.0/tests/test_pyproject.py` & `frequenz-repo-config-0.4.0/tests/test_pyproject.py`

 * *Files identical despite different names*

