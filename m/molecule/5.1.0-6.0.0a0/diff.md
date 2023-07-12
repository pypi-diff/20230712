# Comparing `tmp/molecule-5.1.0.tar.gz` & `tmp/molecule-6.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-5.1.0.tar", last modified: Fri Jun 23 15:19:47 2023, max compression
+gzip compressed data, was "molecule-6.0.0a0.tar", last modified: Wed Jul 12 12:47:21 2023, max compression
```

## Comparing `molecule-5.1.0.tar` & `molecule-6.0.0a0.tar`

### file list

```diff
@@ -1,431 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.070133 molecule-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 15:19:28.000000 molecule-5.1.0/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 15:19:28.000000 molecule-5.1.0/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.006132 molecule-5.1.0/.config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.006132 molecule-5.1.0/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-23 15:19:28.000000 molecule-5.1.0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 15:19:28.000000 molecule-5.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-23 15:19:28.000000 molecule-5.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.010132 molecule-5.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.010132 molecule-5.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.014132 molecule-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/workflows/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-23 15:19:28.000000 molecule-5.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 15:19:28.000000 molecule-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 15:19:28.000000 molecule-5.1.0/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-23 15:19:28.000000 molecule-5.1.0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-23 15:19:28.000000 molecule-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:19:28.000000 molecule-5.1.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.014132 molecule-5.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-23 15:19:28.000000 molecule-5.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-23 15:19:28.000000 molecule-5.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 15:19:28.000000 molecule-5.1.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 15:19:28.000000 molecule-5.1.0/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 15:19:28.000000 molecule-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 15:19:28.000000 molecule-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-23 15:19:47.070133 molecule-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-23 15:19:28.000000 molecule-5.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-23 15:19:28.000000 molecule-5.1.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 15:19:28.000000 molecule-5.1.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 15:19:28.000000 molecule-5.1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.018132 molecule-5.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.954131 molecule-5.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.022132 molecule-5.1.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/google04e29a42ae6e6cbc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.022132 molecule-5.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 15:19:28.000000 molecule-5.1.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 15:19:28.000000 molecule-5.1.0/linkcheckerrc
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-23 15:19:28.000000 molecule-5.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 15:19:28.000000 molecule-5.1.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.022132 molecule-5.1.0/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 15:19:28.000000 molecule-5.1.0/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-23 15:19:28.000000 molecule-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 15:19:28.000000 molecule-5.1.0/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:19:47.070133 molecule-5.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.022132 molecule-5.1.0/snap/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-23 15:19:28.000000 molecule-5.1.0/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.954131 molecule-5.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.030132 molecule-5.1.0/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.042132 molecule-5.1.0/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/init/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.954131 molecule-5.1.0/src/molecule/cookiecutter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/molecule/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.954131 molecule-5.1.0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.958131 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/data/driver.json
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.046132 molecule-5.1.0/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/functional/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.962131 molecule-5.1.0/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.050132 molecule-5.1.0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.966131 molecule-5.1.0/src/molecule/test/resources/schema_instance_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/resources/schema_instance_files/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/resources/schema_instance_files/valid/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.966131 molecule-5.1.0/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.966131 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.966131 molecule-5.1.0/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.970131 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.974131 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.054133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.974131 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/links/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.978131 molecule-5.1.0/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.982131 molecule-5.1.0/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.982131 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.982131 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.982131 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:46.982131 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.058133 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.062133 molecule-5.1.0/src/molecule/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/init/test_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/cookiecutter/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.066133 molecule-5.1.0/src/molecule/test/unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25691 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.070133 molecule-5.1.0/src/molecule/test/unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/verifier/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/test/unit/verifier/test_testinfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.070133 molecule-5.1.0/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-23 15:19:28.000000 molecule-5.1.0/src/molecule/verifier/testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.034132 molecule-5.1.0/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 15:19:46.000000 molecule-5.1.0/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:19:47.070133 molecule-5.1.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-06-23 15:19:28.000000 molecule-5.1.0/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 15:19:28.000000 molecule-5.1.0/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-06-23 15:19:28.000000 molecule-5.1.0/tools/smoketest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-06-23 15:19:28.000000 molecule-5.1.0/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-06-23 15:19:28.000000 molecule-5.1.0/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-23 15:19:28.000000 molecule-5.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.450082 molecule-6.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-12 12:47:04.000000 molecule-6.0.0a0/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-12 12:47:04.000000 molecule-6.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 12:47:04.000000 molecule-6.0.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-12 12:47:21.450082 molecule-6.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-12 12:47:04.000000 molecule-6.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-12 12:47:04.000000 molecule-6.0.0a0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-12 12:47:04.000000 molecule-6.0.0a0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/google04e29a42ae6e6cbc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/next.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/podman.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:04.000000 molecule-6.0.0a0/linkcheckerrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-12 12:47:04.000000 molecule-6.0.0a0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/podman/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-12 12:47:04.000000 molecule-6.0.0a0/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-12 12:47:04.000000 molecule-6.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:47:04.000000 molecule-6.0.0a0/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:47:21.450082 molecule-6.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 12:47:04.000000 molecule-6.0.0a0/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.426082 molecule-6.0.0a0/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/init-scenario.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/data/templates/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/create.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/destroy.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/test/a_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/test_ansible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/b_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.426082 molecule-6.0.0a0/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.450082 molecule-6.0.0a0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tox.ini
```

### Comparing `molecule-5.1.0/.config/molecule.spec` & `molecule-6.0.0a0/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.config/requirements-lock.txt` & `molecule-6.0.0a0/.config/requirements-lock.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --no-annotate --output-file=.config/requirements-lock.txt --resolver=backtracking --strip-extras --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
 ansible-compat==4.1.2
-ansible-core==2.14.4
-arrow==1.2.3
+ansible-core==2.15.1
 attrs==23.1.0
-binaryornot==0.4.4
-certifi==2022.12.7
 cffi==1.15.1
-chardet==5.1.0
-charset-normalizer==3.1.0
-click==8.1.3
+click==8.1.4
 click-help-colors==0.9.1
-cookiecutter==2.1.1
-cryptography==41.0.0
+cryptography==41.0.1
 enrich==1.2.7
-idna==3.4
+importlib-resources==5.0.7
 jinja2==3.1.2
-jinja2-time==0.2.0
-jsonschema==4.17.3
-markdown-it-py==2.2.0
-markupsafe==2.1.2
+jsonschema==4.18.0
+jsonschema-specifications==2023.6.1
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 mdurl==0.1.2
 packaging==23.1
-pluggy==1.0.0
+pluggy==1.2.0
 pycparser==2.21
 pygments==2.15.1
-pyrsistent==0.19.3
-python-dateutil==2.8.2
-python-slugify==8.0.1
 pyyaml==6.0
-requests==2.31.0
-resolvelib==0.8.1
-rich==13.3.4
-six==1.16.0
+referencing==0.29.1
+resolvelib==1.0.1
+rich==13.4.2
+rpds-py==0.8.10
 subprocess-tee==0.4.1
-text-unidecode==1.3
-urllib3==1.26.15
+typing-extensions==4.7.1
```

### Comparing `molecule-5.1.0/.config/requirements.txt` & `molecule-6.0.0a0/.config/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,109 +2,103 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=.config/requirements.txt --resolver=backtracking --strip-extras pyproject.toml
 #
 ansi2html==1.8.0
 ansible-compat==4.1.2
-ansible-core==2.14.4
-ansible-lint==6.14.6
-arrow==1.2.3
+ansible-core==2.15.1
+ansible-lint==6.17.2
 attrs==23.1.0
-beautifulsoup4==4.12.1
-binaryornot==0.4.4
+beautifulsoup4==4.12.2
 black==23.3.0
 bracex==2.3.post1
-cairocffi==1.5.0
+cairocffi==1.5.1
 cairosvg==2.7.0
-certifi==2022.12.7
+certifi==2023.5.7
 cffi==1.15.1
-chardet==5.1.0
 charset-normalizer==3.1.0
-check-jsonschema==0.22.0
+check-jsonschema==0.23.2
 click==8.1.3
 click-help-colors==0.9.1
 colorama==0.4.6
-cookiecutter==2.1.1
-coverage==7.2.3
-cryptography==40.0.2
+coverage==7.2.7
+cryptography==41.0.1
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 dnspython==2.3.0
 enrich==1.2.7
-exceptiongroup==1.1.1
-execnet==1.9.0
-filelock==3.12.0
+exceptiongroup==1.1.2
+execnet==2.0.0
+filelock==3.12.2
 ghp-import==2.1.0
-griffe==0.26.0
+griffe==0.29.0
 htmlmin2==0.1.13
 idna==3.4
-importlib-metadata==6.1.0
+importlib-metadata==6.6.0
+importlib-resources==5.0.7
 iniconfig==2.0.0
 jinja2==3.1.2
-jinja2-time==0.2.0
 jsmin==3.0.1
-jsonschema==4.17.3
+jsonschema==4.18.0
+jsonschema-specifications==2023.6.1
 linkchecker==10.2.1
 markdown==3.3.7
-markdown-exec==1.4.0
+markdown-exec==1.6.0
 markdown-include==0.8.1
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
 markupsafe==2.1.2
 mdurl==0.1.2
 mergedeep==1.3.4
-mkdocs==1.4.2
-mkdocs-ansible==0.1.4
+mkdocs==1.4.3
+mkdocs-ansible==0.1.6
 mkdocs-autorefs==0.4.1
-mkdocs-gen-files==0.4.0
-mkdocs-htmlproofer-plugin==0.11.0
-mkdocs-material==9.1.5
+mkdocs-gen-files==0.5.0
+mkdocs-htmlproofer-plugin==0.13.1
+mkdocs-material==9.1.15
 mkdocs-material-extensions==1.1.1
 mkdocs-minify-plugin==0.6.4
-mkdocs-monorepo-plugin==1.0.4
-mkdocstrings==0.21.2
-mkdocstrings-python==0.9.0
+mkdocs-monorepo-plugin==1.0.5
+mkdocstrings==0.22.0
+mkdocstrings-python==1.1.0
 mypy-extensions==1.0.0
-packaging==23.0
+packaging==23.1
 pathspec==0.11.1
 pexpect==4.8.0
 pillow==9.5.0
-pipdeptree==2.7.0
-platformdirs==3.2.0
-pluggy==1.0.0
+pipdeptree==2.7.1
+platformdirs==3.8.1
+pluggy==1.2.0
 ptyprocess==0.7.0
 pycparser==2.21
-pygments==2.14.0
-pymdown-extensions==9.10
-pyrsistent==0.19.3
-pytest==7.3.1
-pytest-mock==3.10.0
+pygments==2.15.1
+pymdown-extensions==10.0.1
+pytest==7.4.0
+pytest-mock==3.11.1
 pytest-plus==0.4.0
-pytest-testinfra==7.0.0
-pytest-xdist==3.2.1
+pytest-xdist==3.3.1
 python-dateutil==2.8.2
 python-slugify==8.0.1
 pyyaml==6.0
 pyyaml-env-tag==0.1
-regex==2023.3.23
-requests==2.28.2
-resolvelib==0.8.1
-rich==13.3.4
-ruamel-yaml==0.17.21
+referencing==0.29.1
+regex==2023.5.5
+requests==2.31.0
+resolvelib==1.0.1
+rich==13.4.2
+rpds-py==0.8.10
+ruamel-yaml==0.17.31
 ruamel-yaml-clib==0.2.7
 six==1.16.0
-soupsieve==2.4
+soupsieve==2.4.1
 subprocess-tee==0.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
-typing-extensions==4.5.0
-urllib3==1.26.15
+typing-extensions==4.6.2
+urllib3==2.0.2
 watchdog==3.0.0
 wcmatch==8.4.1
 webencodings==0.5.1
-yamllint==1.30.0
+yamllint==1.32.0
 zipp==3.15.0
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `molecule-5.1.0/.gitattributes` & `molecule-6.0.0a0/.gitattributes`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `molecule-6.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/ISSUE_TEMPLATE/config.yml` & `molecule-6.0.0a0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/dependabot.yml` & `molecule-6.0.0a0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/workflows/redirects.yml` & `molecule-6.0.0a0/.github/workflows/redirects.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/workflows/release.yml` & `molecule-6.0.0a0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.github/workflows/tox.yml` & `molecule-6.0.0a0/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # limit potential endless looks like we had with build-containers
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
     env:
-      PYTEST_REQPASS: 455
+      PYTEST_REQPASS: 424
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Set pre-commit cache
```

### Comparing `molecule-5.1.0/.packit.yaml` & `molecule-6.0.0a0/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.pre-commit-config.yaml` & `molecule-6.0.0a0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     # keep it before yamllint
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         # Temporary excludes so we can gradually normalize the formatting
         exclude: >
           (?x)^(
-            src/molecule/cookiecutter/.*|
             src/molecule/test/resources/templates/.*|
           )$
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
@@ -50,52 +49,54 @@
         entry: yamllint --strict
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.275"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: []
         entry: mypy src/
         pass_filenames: false
         additional_dependencies:
           - ansible-compat>=4.1.2
-          - click>=8.0.1
+          - click>=8.0.1,<8.1.4 # https://github.com/pallets/click/issues/2558
           - enrich>=1.2.7
           - importlib-metadata>=4.6.1
           - jinja2
           - packaging
+          - pytest
+          - pytest-mock
           - rich
           - ruamel.yaml>=0.17.10
           - types-PyYAML
           - types-dataclasses
           - types-filelock
+          - types-jsonschema
           - types-setuptools
   - repo: https://github.com/pycqa/pylint
     rev: v3.0.0a6
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
           - ansible-compat>=4.1.2
           - click
           - click-help-colors
-          - cookiecutter
           - enrich>=1.2.7
           - filelock
           - jsonschema
           - pexpect
-          - testinfra
+          - pytest-mock
   - repo: https://github.com/jazzband/pip-tools
-    rev: 6.13.0
+    rev: 6.14.0
     hooks:
       - id: pip-compile
         entry: pip-compile -q --resolver=backtracking --strip-extras --no-annotate --output-file=.config/requirements.txt pyproject.toml --extra docs --extra test
         files: ^(pyproject\.toml|\.config\/.*)$
       - id: pip-compile
         name: pip-compile-upgrade
         alias: up
```

### Comparing `molecule-5.1.0/.vscode/settings.json` & `molecule-6.0.0a0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/.yamllint` & `molecule-6.0.0a0/.yamllint`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 ---
 # Based on ansible-lint config
 extends: default
-ignore: |
-  src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}
-  src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}
-  src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}
 rules:
   braces:
     max-spaces-inside: 1
     level: error
   brackets:
     max-spaces-inside: 1
     level: error
```

### Comparing `molecule-5.1.0/DCO_1_1.md` & `molecule-6.0.0a0/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/LICENSE` & `molecule-6.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/PKG-INFO` & `molecule-6.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.1.0
+Version: 6.0.0a0
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-5.1.0/README.md` & `molecule-6.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/bindep.txt` & `molecule-6.0.0a0/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/conftest.py` & `molecule-6.0.0a0/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/_static/images/favicon.ico` & `molecule-6.0.0a0/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/_static/images/logo.png` & `molecule-6.0.0a0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/_static/images/logo_big.png` & `molecule-6.0.0a0/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/ci.md` & `molecule-6.0.0a0/docs/ci.md`

 * *Files 1% similar despite different names*

```diff
@@ -397,21 +397,17 @@
 platform in `molecule.yml` configuration file. This way, their names
 won't create any conflict.
 
 ```yaml
 ---
 dependency:
   name: galaxy
-driver:
-  name: docker
 platforms:
   - name: instance1-$TOX_ENVNAME
     image: mariadb
   - name: instance2-$TOX_ENVNAME
     image: retr0h/centos7-systemd-ansible:latest
     privileged: True
     command: /usr/sbin/init
 provisioner:
   name: ansible
-verifier:
-  name: testinfra
 ```
```

### Comparing `molecule-5.1.0/docs/configuration.md` & `molecule-6.0.0a0/docs/configuration.md`

 * *Files 0% similar despite different names*

```diff
@@ -290,11 +290,7 @@
 ## Verifier
 
 Molecule handles role testing by invoking configurable verifiers.
 
 ### Ansible
 
 ::: molecule.verifier.ansible.Ansible
-
-### Testinfra
-
-::: molecule.verifier.testinfra.Testinfra
```

### Comparing `molecule-5.1.0/docs/contributing.md` & `molecule-6.0.0a0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/examples.md` & `molecule-6.0.0a0/docs/examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 1.  `platforms[*].image`: Docker image name:tag to use as base image.
 
 2.  `platforms[*].pre_build_image`: Whether to customize base image or
     use as-is[^1].
 
     > - When `true`, use the specified `platform[].image` as-is.
-    >
     > - When `false`, exec `docker build` to customize base image
     >   using either:
     >
     >   > - Dockerfile specified by `platforms[*].dockerfile` or
     >   > - Dockerfile rendered from `Dockerfile.j2` template (in
     >   >   scenario dir)
 
@@ -356,23 +355,14 @@
 │   │   └── molecule.yml
 │   └── ubuntu-upstart
 │       └── molecule.yml
 ```
 
 Tests and playbooks can be shared across scenarios.
 
-In this example the `tests` directory lives in a shared
-location and `molecule.yml` points to the shared tests.
-
-```yaml
-verifier:
-  name: testinfra
-  directory: ../resources/tests/
-```
-
 In this second example the actions `create`,
 `destroy`, `converge` and `prepare`
 are loaded from a shared directory.
 
 ```yaml
 provisioner:
   name: ansible
```

### Comparing `molecule-5.1.0/docs/faq.md` & `molecule-6.0.0a0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/getting-started.md` & `molecule-6.0.0a0/docs/getting-started.md`

 * *Files 21% similar despite different names*

```diff
@@ -7,37 +7,14 @@
 !!! note
 
     In order to complete this guide by hand, you will need to additionally
     install [Docker](https://docs.docker.com/). Molecule requires an
     external Python dependency for the Docker driver which is provided when
     installing Molecule using `pip install 'molecule-plugins[docker]'`.
 
-## Creating a new role
-
-Molecule uses [ansible-galaxy](https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html) under the hood to generate conventional role layouts. If
-you've ever worked with Ansible roles before, you'll be right at home.
-If not, please review the
-[role directory structure](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html#role-directory-structure)
-guide to see what each folder is responsible for.
-
-To generate a new role with Molecule, simply run:
-
-```shell
-$ molecule init role acme.my_new_role --driver-name docker
-```
-
-You should then see a `my_new_role` folder in your current directory.
-
-!!! note
-
-    For future reference, if you want to initialize Molecule within an
-    existing role, you would use the
-    `molecule init scenario -r my_role_name` command from within the role's
-    directory (e.g. `my_role_name/`).
-
 ## Molecule Scenarios
 
 You will notice one new folder which is the `molecule` folder.
 
 In this folder there is a single `root_scenario` called `default`.
 
 Scenarios are the starting point for a lot of powerful functionality
@@ -63,16 +40,15 @@
   employ when testing your role.
 - `converge.yml` is the playbook file that contains the call for your
   role. Molecule will invoke this playbook with `ansible-playbook` and
   run it against an instance created by the driver.
 - `verify.yml` is the Ansible file used for testing as Ansible is the
   default [verifier](configuration.md#verifier). This allows you to
   write specific tests against the state of the container after your
-  role has finished executing. Other verifier tools are available
-  Note that [testinfra](https://testinfra.readthedocs.io/en/latest/) was the default verifier prior to molecule version 3.
+  role has finished executing.
 
 !!! note
 
     If the `verify.yml` playbook does not explicitly `include_role` your
     role, the `library` and `module_utils` provided by your role are not
     available in the playbook by default. If you need those for testing but
     would like to avoid re-running your role, consider adding an empty task
```

### Comparing `molecule-5.1.0/docs/images/favicon.ico` & `molecule-6.0.0a0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/images/logo.png` & `molecule-6.0.0a0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/images/logo.svg` & `molecule-6.0.0a0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/index.md` & `molecule-6.0.0a0/docs/index.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/installation.md` & `molecule-6.0.0a0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/docs/usage.md` & `molecule-6.0.0a0/docs/usage.md`

 * *Files 18% similar despite different names*

```diff
@@ -41,20 +41,14 @@
     command.  Use this option with care, as there is no sanitation or
     validation of input.  Options passed on the CLI override options
     provided in provisioner's `options` section of `molecule.yml`.
 ```
 
 ## molecule init
 
-### molecule init role
-
-Initialize a new role using ansible-galaxy and include default
-molecule directory. Please refer to the `init scenario`
-command in order to generate a custom `molecule` scenario.
-
 ### molecule init scenario
 
 ## molecule list
 
 List command shows information about current scenarios.
 
 ```
```

### Comparing `molecule-5.1.0/mkdocs.yml` & `molecule-6.0.0a0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,19 @@
 
 nav:
   - Home: index.md
   - installation.md
   - Using:
       - getting-started.md
       - usage.md
+      - next.md
       - configuration.md
       - ci.md
+  - Examples:
+      - podman.md
   - examples.md
   - faq.md
   - contributing.md
 
 plugins:
   - autorefs
   - search
@@ -83,14 +86,16 @@
           import:
             - url: https://docs.ansible.com/ansible/latest/objects.inv
               domains: [py, std, "std:doc", "std:label"]
             - url: https://pip.pypa.io/en/latest/objects.inv
               domains: [py, std]
 
 markdown_extensions:
+  - markdown_include.include:
+      base_path: docs
   - admonition
   - def_list
   - footnotes
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite
   - pymdownx.snippets:
```

### Comparing `molecule-5.1.0/playbooks/snap-pre-run.yaml` & `molecule-6.0.0a0/playbooks/snap-pre-run.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/pyproject.toml` & `molecule-6.0.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,18 @@
 documentation = "https://molecule.readthedocs.io/"
 repository = "https://github.com/ansible-community/molecule"
 changelog = "https://github.com/ansible-community/molecule/releases"
 
 [project.scripts]
 molecule = "molecule.__main__:main"
 
-[project.entry-points."molecule.driver"]
-delegated = "molecule.driver.delegated:Delegated"
+[project.entry-points."molecule.driver.next"]
+default = "molecule.driver.delegated:Delegated"
 
-[project.entry-points."molecule.verifier"]
-testinfra = "molecule.verifier.testinfra:Testinfra"
+[project.entry-points."molecule.verifier.next"]
 ansible = "molecule.verifier.ansible:Ansible"
 
 [tool.coverage.run]
 source = ["src"]
 # branch = true
 parallel = true
 concurrency = ["multiprocessing", "thread"]
@@ -71,14 +70,41 @@
 [tool.black]
 skip-string-normalization = false
 
 [tool.isort]
 profile = "black"
 known_first_party = "molecule"
 
+[tool.mypy]
+python_version = 3.9
+# strict = true
+color_output = true
+error_summary = true
+# disallow_untyped_calls = true
+# disallow_untyped_defs = true
+# disallow_any_generics = true
+# disallow_any_unimported = True
+# warn_redundant_casts = True
+# warn_return_any = True
+# warn_unused_configs = True
+# site-packages is here to help vscode mypy integration getting confused
+exclude = "(build|dist|test/local-content|site-packages|~/.pyenv|examples/playbooks/collections|plugins/modules)"
+# https://github.com/python/mypy/issues/12664
+no_incremental = true
+
+[[tool.mypy.overrides]]
+module = [
+  "click_help_colors", # https://github.com/click-contrib/click-help-colors/issues/20
+  "pexpect", # https://github.com/pexpect/pexpect/issues/759
+  "pluggy", # https://github.com/pytest-dev/pluggy/pull/414
+  "pytest_mock",
+]
+ignore_missing_imports = true
+ignore_errors = true
+
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
   # TODO(ssbarnea): remove temporary skips adding during initial adoption:
   "abstract-method",
   "arguments-differ",
   "broad-except",
   "consider-merging-isinstance",
@@ -125,15 +151,14 @@
 ]
 norecursedirs = [
   ".eggs",
   ".tox",
   "build",
   "dist",
   "doc",
-  "src/molecule/cookiecutter/scenario",
   "src/molecule/test/resources",
   "src/molecule/test/scenarios",
 ]
 addopts = "--doctest-modules --durations 10 --color=yes"
 doctest_optionflags = ["ALLOW_UNICODE", "ELLIPSIS"]
 junit_suite_name = "molecule_test_suite"
 testpaths = "src/molecule/test/"
```

### Comparing `molecule-5.1.0/snap/snapcraft.yaml` & `molecule-6.0.0a0/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/__init__.py` & `molecule-6.0.0a0/src/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/__main__.py` & `molecule-6.0.0a0/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/api.py` & `molecule-6.0.0a0/src/molecule/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     """A warning noting an unsupported runtime environment."""
 
 
 @cache
 def drivers(config=None) -> UserListMap:
     """Return list of active drivers."""
     plugins = UserListMap()
-    pm = pluggy.PluginManager("molecule.driver")
+    pm = pluggy.PluginManager("molecule.driver.next")
     try:
-        pm.load_setuptools_entrypoints("molecule.driver")
+        pm.load_setuptools_entrypoints("molecule.driver.next")
     except (Exception, SystemExit):
         # These are not fatal because a broken driver should not make the entire
         # tool unusable.
         LOG.error("Failed to load driver entry point %s", traceback.format_exc())
     for p in pm.get_plugins():
         try:
             plugins.append(p(config))
@@ -64,17 +64,17 @@
     return plugins
 
 
 @cache
 def verifiers(config=None) -> UserListMap:
     """Return list of active verifiers."""
     plugins = UserListMap()
-    pm = pluggy.PluginManager("molecule.verifier")
+    pm = pluggy.PluginManager("molecule.verifier.next")
     try:
-        pm.load_setuptools_entrypoints("molecule.verifier")
+        pm.load_setuptools_entrypoints("molecule.verifier.next")
     except Exception:
         # These are not fatal because a broken verifier should not make the entire
         # tool unusable.
         LOG.error("Failed to load verifier entry point %s", traceback.format_exc())
     for p in pm.get_plugins():
         try:
             plugins.append(p(config))
```

### Comparing `molecule-5.1.0/src/molecule/command/__init__.py` & `molecule-6.0.0a0/src/molecule/command/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/base.py` & `molecule-6.0.0a0/src/molecule/command/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/check.py` & `molecule-6.0.0a0/src/molecule/command/check.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/cleanup.py` & `molecule-6.0.0a0/src/molecule/command/cleanup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 @click.pass_context
 @click.option(
     "--scenario-name",
     "-s",
     default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
     help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
 )
-def cleanup(ctx, scenario_name):  # pragma: no cover
+def cleanup(ctx, scenario_name="default"):  # pragma: no cover
     """Use the provisioner to cleanup any changes made to external systems during \
     the stages of testing.
     """
     args = ctx.obj.get("args")
     subcommand = base._get_subcommand(__name__)
     command_args = {"subcommand": subcommand}
```

### Comparing `molecule-5.1.0/src/molecule/command/converge.py` & `molecule-6.0.0a0/src/molecule/command/verify.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,47 +13,45 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
-"""Converge Command Module."""
+"""Verify Command Module."""
 
 import logging
 
 import click
 
 from molecule.command import base
 
 LOG = logging.getLogger(__name__)
 
 
-class Converge(base.Base):
-    """Converge Command Class."""
+class Verify(base.Base):
+    """Verify Command Class."""
 
     def execute(self, action_args=None):
-        """Execute the actions necessary to perform a `molecule converge` and \
+        """Execute the actions necessary to perform a `molecule verify` and \
         returns None.
 
         :return: None
         """
-        self._config.provisioner.converge()
-        self._config.state.change_state("converged", True)
+        self._config.verifier.execute(action_args)
 
 
 @base.click_command_ex()
 @click.pass_context
 @click.option(
     "--scenario-name",
     "-s",
     default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
     help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
 )
-@click.argument("ansible_args", nargs=-1, type=click.UNPROCESSED)
-def converge(ctx, scenario_name, ansible_args):  # pragma: no cover
-    """Use the provisioner to configure instances (dependency, create, prepare converge)."""
+def verify(ctx, scenario_name="default"):  # pragma: no cover
+    """Run automated tests against instances."""
     args = ctx.obj.get("args")
     subcommand = base._get_subcommand(__name__)
     command_args = {"subcommand": subcommand}
 
-    base.execute_cmdline_scenarios(scenario_name, args, command_args, ansible_args)
+    base.execute_cmdline_scenarios(scenario_name, args, command_args)
```

### Comparing `molecule-5.1.0/src/molecule/command/create.py` & `molecule-6.0.0a0/src/molecule/command/create.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,24 +37,14 @@
         """Execute the actions necessary to perform a `molecule create` and \
         returns None.
 
         :return: None
         """
         self._config.state.change_state("driver", self._config.driver.name)
 
-        if self._config.driver.delegated and not self._config.driver.managed:
-            msg = "Skipping, instances are delegated."
-            LOG.warning(msg)
-            return
-
-        if self._config.state.created:
-            msg = "Skipping, instances already created."
-            LOG.warning(msg)
-            return
-
         self._config.provisioner.create()
 
         self._config.state.change_state("created", True)
 
 
 @base.click_command_ex()
 @click.pass_context
```

### Comparing `molecule-5.1.0/src/molecule/command/dependency.py` & `molecule-6.0.0a0/src/molecule/command/dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/destroy.py` & `molecule-6.0.0a0/src/molecule/command/destroy.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,19 +43,14 @@
         :return: None
         """
         if self._config.command_args.get("destroy") == "never":
             msg = "Skipping, '--destroy=never' requested."
             LOG.warning(msg)
             return
 
-        if self._config.driver.delegated and not self._config.driver.managed:
-            msg = "Skipping, instances are delegated."
-            LOG.warning(msg)
-            return
-
         self._config.provisioner.destroy()
         self._config.state.reset()
 
 
 @base.click_command_ex()
 @click.pass_context
 @click.option(
```

### Comparing `molecule-5.1.0/src/molecule/command/drivers.py` & `molecule-6.0.0a0/src/molecule/command/drivers.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/idempotence.py` & `molecule-6.0.0a0/src/molecule/command/idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/init/init.py` & `molecule-6.0.0a0/src/molecule/command/init/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base class used by init command."""
 
 import logging
 
 from molecule.command import base
-from molecule.command.init import role, scenario
+from molecule.command.init import scenario
 
 LOG = logging.getLogger(__name__)
 
 
 @base.click_group_ex()  # type: ignore
 def init():  # pragma: no cover
     """Initialize a new role or scenario."""
 
 
-init.add_command(role.role)
 init.add_command(scenario.scenario)
```

### Comparing `molecule-5.1.0/src/molecule/command/init/scenario.py` & `molecule-6.0.0a0/src/molecule/command/init/scenario.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base class used by init scenario command."""
 
+import json
 import logging
 import os
 
 import click
 
 from molecule import api, config, util
 from molecule.command import base as command_base
 from molecule.command.init import base
-from molecule.config import DEFAULT_DRIVER
+from molecule.config import DEFAULT_DRIVER, MOLECULE_EMBEDDED_DATA_DIR
 
 LOG = logging.getLogger(__name__)
 
 
 class Scenario(base.Base):
     """
     Scenario Class.
@@ -49,74 +50,58 @@
 
         Initialize an existing role with Molecule:
 
     .. program:: cd foo; molecule init scenario bar --role-name foo
 
     .. option:: cd foo; molecule init scenario bar --role-name foo
 
-        Initialize a new scenario using a local *cookiecutter* template for the
-        driver configuration.
+        Initialize a new scenario using a embedded template.
     """
 
     def __init__(self, command_args: dict[str, str]) -> None:
         """Construct Scenario."""
         self._command_args = command_args
 
     def execute(self, action_args=None):
         """Execute the actions necessary to perform a `molecule init scenario` and \
         returns None.
 
         :return: None
         """
         scenario_name = self._command_args["scenario_name"]
-        role_name = os.getcwd().split(os.sep)[-1]
-        role_directory = util.abs_path(os.path.join(os.getcwd(), os.pardir))
 
         msg = f"Initializing new scenario {scenario_name}..."
         LOG.info(msg)
-        molecule_directory = config.molecule_directory(
-            os.path.join(role_directory, role_name),
-        )
+        molecule_directory = config.molecule_directory(os.getcwd())
         scenario_directory = os.path.join(molecule_directory, scenario_name)
 
         if os.path.isdir(scenario_directory):
             msg = (
                 f"The directory molecule/{scenario_name} exists. "
                 "Cannot create new scenario."
             )
             util.sysexit_with_message(msg)
 
-        driver_template = api.drivers()[
-            self._command_args["driver_name"]
-        ].template_dir()
-        if "driver_template" in self._command_args:
-            self._validate_template_dir(self._command_args["driver_template"])
-            cli_driver_template = f"{self._command_args['driver_template']}/{self._command_args['driver_name']}"
-            if os.path.isdir(cli_driver_template):
-                driver_template = cli_driver_template
-            else:
-                LOG.warning(
-                    "Driver not found in custom template directory(%s), "
-                    "using the default template instead",
-                    cli_driver_template,
-                )
-        scenario_base_directory = os.path.join(role_directory, role_name)
-        templates = [
-            driver_template,
-            api.verifiers()[self._command_args["verifier_name"]].template_dir(),
+        extra_vars = json.dumps(self._command_args)
+        cmd = [
+            "ansible-playbook",
+            "-i",
+            "localhost,",
+            "--connection=local",
+            "--extra-vars",
+            extra_vars,
+            f"{MOLECULE_EMBEDDED_DATA_DIR}/init-scenario.yml",
         ]
-        self._process_templates("molecule", self._command_args, role_directory)
-        for template in templates:
-            self._process_templates(
-                template,
-                self._command_args,
-                scenario_base_directory,
-            )
+        env = os.environ.copy()
+        # As ansible fails to find a terminal when run by molecule, we force
+        # it to use colors.
+        env["ANSIBLE_FORCE_COLOR"] = "1"
+        env["ANSIBLE_PYTHON_INTERPRETER"] = "auto_silent"
+        util.run_command(cmd, env=env, check=True)
 
-        role_directory = os.path.join(role_directory, role_name)
         msg = f"Initialized scenario in {scenario_directory} successfully."
         LOG.info(msg)
 
 
 def _role_exists(ctx, param, value: str):  # pragma: no cover
     # if role name was not mentioned we assume that current directory is the
     # one hosting the role and determining the role name.
@@ -126,28 +111,14 @@
     role_directory = os.path.join(os.pardir, value)
     if not os.path.exists(role_directory):
         msg = f"The role '{value}' not found. Please choose the proper role name."
         util.sysexit_with_message(msg)
     return value
 
 
-def _default_scenario_exists(ctx, param, value: str):  # pragma: no cover
-    if value == command_base.MOLECULE_DEFAULT_SCENARIO_NAME:
-        return value
-
-    default_scenario_directory = os.path.join(
-        "molecule",
-        command_base.MOLECULE_DEFAULT_SCENARIO_NAME,
-    )
-    if not os.path.exists(default_scenario_directory):
-        msg = f"The default scenario not found.  Please create a scenario named '{command_base.MOLECULE_DEFAULT_SCENARIO_NAME}' first."
-        util.sysexit_with_message(msg)
-    return value
-
-
 @command_base.click_command_ex()
 @click.pass_context
 @click.option(
     "--dependency-name",
     type=click.Choice(["galaxy"]),
     default="galaxy",
     help="Name of dependency to initialize. (galaxy)",
@@ -161,51 +132,33 @@
 )
 @click.option(
     "--provisioner-name",
     type=click.Choice(["ansible"]),
     default="ansible",
     help="Name of provisioner to initialize. (ansible)",
 )
-@click.option(
-    "--role-name",
-    "-r",
-    required=False,
-    callback=_role_exists,
-    help="Name of the role to create.",
-)
 @click.argument(
     "scenario-name",
     default=command_base.MOLECULE_DEFAULT_SCENARIO_NAME,
     required=False,
-    callback=_default_scenario_exists,
-)
-@click.option(
-    "--verifier-name",
-    type=click.Choice([str(s) for s in api.verifiers()]),
-    default="ansible",
-    help="Name of verifier to initialize. (ansible)",
 )
 def scenario(
     ctx,
     dependency_name,
     driver_name,
     provisioner_name,
-    role_name,
     scenario_name,
-    verifier_name,
 ):  # pragma: no cover
     """Initialize a new scenario for use with Molecule.
 
     If name is not specified the 'default' value will be used.
     """
     command_args = {
         "dependency_name": dependency_name,
         "driver_name": driver_name,
         "provisioner_name": provisioner_name,
-        "role_name": role_name,
         "scenario_name": scenario_name,
         "subcommand": __name__,
-        "verifier_name": verifier_name,
     }
 
     s = Scenario(command_args)
     s.execute()
```

### Comparing `molecule-5.1.0/src/molecule/command/list.py` & `molecule-6.0.0a0/src/molecule/command/list.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/login.py` & `molecule-6.0.0a0/src/molecule/command/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,20 @@
 
     def _get_login(self, hostname):  # pragma: no cover
         # ruff: noqa: S605,S607
         lines, columns = os.popen("stty size", "r").read().split()
         login_options = self._config.driver.login_options(hostname)
         login_options["columns"] = columns
         login_options["lines"] = lines
+        if not self._config.driver.login_cmd_template:
+            LOG.warning(
+                "Login command is not supported for [dim]%s[/] host because 'login_cmd_template' was not defined in driver options.",
+                login_options["instance"],
+            )
+            return
         login_cmd = self._config.driver.login_cmd_template.format(**login_options)
 
         cmd = shlex.split(f"/usr/bin/env {login_cmd}")
         # ruff: noqa: S603
         subprocess.run(cmd, check=False)
```

### Comparing `molecule-5.1.0/src/molecule/command/matrix.py` & `molecule-6.0.0a0/src/molecule/command/matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/prepare.py` & `molecule-6.0.0a0/src/molecule/command/prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/reset.py` & `molecule-6.0.0a0/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/side_effect.py` & `molecule-6.0.0a0/src/molecule/command/side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/syntax.py` & `molecule-6.0.0a0/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/test.py` & `molecule-6.0.0a0/src/molecule/command/test.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/command/verify.py` & `molecule-6.0.0a0/src/molecule/provisioner/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,45 +13,48 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
-"""Verify Command Module."""
+"""Provisioner Base Module."""
 
-import logging
+import abc
 
-import click
 
-from molecule.command import base
+class Base:
+    """Provisioner Base Class."""
 
-LOG = logging.getLogger(__name__)
+    __metaclass__ = abc.ABCMeta
 
+    def __init__(self, config) -> None:
+        """Initialize code for all :ref:`Provisioner` classes.
 
-class Verify(base.Base):
-    """Verify Command Class."""
+        :param config: An instance of a Molecule config.
+        :returns: None
+        """
+        self._config = config
 
-    def execute(self, action_args=None):
-        """Execute the actions necessary to perform a `molecule verify` and \
-        returns None.
+    @property
+    @abc.abstractmethod
+    def default_options(self):  # pragma: no cover
+        """Get default CLI arguments provided to ``cmd`` as a dict.
 
-        :return: None
+        :return: dict
         """
-        self._config.verifier.execute(action_args)
 
+    @property
+    @abc.abstractmethod
+    def default_env(self):  # pragma: no cover
+        """Get default env variables provided to ``cmd`` as a dict.
+
+        :return: dict
+        """
 
-@base.click_command_ex()
-@click.pass_context
-@click.option(
-    "--scenario-name",
-    "-s",
-    default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
-    help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
-)
-def verify(ctx, scenario_name):  # pragma: no cover
-    """Run automated tests against instances."""
-    args = ctx.obj.get("args")
-    subcommand = base._get_subcommand(__name__)
-    command_args = {"subcommand": subcommand}
+    @property
+    @abc.abstractmethod
+    def name(self):  # pragma: no cover
+        """Name of the provisioner and returns a string.
 
-    base.execute_cmdline_scenarios(scenario_name, args, command_args)
+        :returns: str
+        """
```

### Comparing `molecule-5.1.0/src/molecule/config.py` & `molecule-6.0.0a0/src/molecule/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,29 @@
 from uuid import uuid4
 
 from ansible_compat.ports import cache, cached_property
 from packaging.version import Version
 
 from molecule import api, interpolation, platforms, scenario, state, util
 from molecule.app import app
+from molecule.data import __file__ as data_module
 from molecule.dependency import ansible_galaxy, shell
 from molecule.model import schema_v3
 from molecule.provisioner import ansible
 from molecule.util import boolean
 
 LOG = logging.getLogger(__name__)
 MOLECULE_DEBUG = boolean(os.environ.get("MOLECULE_DEBUG", "False"))
 MOLECULE_VERBOSITY = int(os.environ.get("MOLECULE_VERBOSITY", 0))
 MOLECULE_DIRECTORY = "molecule"
 MOLECULE_FILE = "molecule.yml"
 MOLECULE_KEEP_STRING = "MOLECULE_"
-DEFAULT_DRIVER = "delegated"
+DEFAULT_DRIVER = "default"
+
+MOLECULE_EMBEDDED_DATA_DIR = os.path.dirname(data_module)
 
 
 @cache
 def ansible_version() -> Version:
     """Retrieve Ansible version."""
     warnings.warn(
         "molecule.config.ansible_version is deprecated, will be removed in the future.",
@@ -327,24 +330,24 @@
            merge.
 
         :return: dict
         """
         defaults = self._get_defaults()
         base_configs = filter(os.path.exists, self.args.get("base_config", []))
         for base_config in base_configs:
-            with util.open_file(base_config) as stream:
+            with open(base_config) as stream:
                 s = stream.read()
                 interpolated_config = self._interpolate(s, env, keep_string)
                 defaults = util.merge_dicts(
                     defaults,
                     util.safe_load(interpolated_config),
                 )
 
         if self.molecule_file:
-            with util.open_file(self.molecule_file) as stream:
+            with open(self.molecule_file) as stream:
                 s = stream.read()
                 interpolated_config = self._interpolate(s, env, keep_string)
                 defaults = util.merge_dicts(
                     defaults,
                     util.safe_load(interpolated_config),
                 )
 
@@ -376,15 +379,15 @@
                 "name": "galaxy",
                 "command": None,
                 "enabled": True,
                 "options": {},
                 "env": {},
             },
             "driver": {
-                "name": "delegated",
+                "name": "default",
                 "provider": {"name": None},
                 "options": {"managed": True},
                 "ssh_connection_options": [],
                 "safe_files": [],
             },
             "platforms": [],
             "prerun": True,
```

### Comparing `molecule-5.1.0/src/molecule/console.py` & `molecule-6.0.0a0/src/molecule/console.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-6.0.0a0/molecule/default/create.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ---
-{% raw -%}
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
-
     # TODO: Developer must implement and populate 'server' variable
 
     - name: Create instance config
-      when: server.changed | default(false) | bool  # noqa no-handler
+      when: server.changed | default(false) | bool # noqa no-handler
       block:
-        - name: Populate instance config dict  # noqa jinja
+        - name: Populate instance config dict # noqa jinja
           ansible.builtin.set_fact:
-            instance_conf_dict: {
-              'instance': "{{ }}",
-              'address': "{{ }}",
-              'user': "{{ }}",
-              'port': "{{ }}",
-              'identity_file': "{{ }}", }
+            instance_conf_dict:
+              {
+                "instance": "{{ }}",
+                "address": "{{ }}",
+                "user": "{{ }}",
+                "port": "{{ }}",
+                "identity_file": "{{ }}",
+              }
           with_items: "{{ server.results }}"
           register: instance_config_dict
 
         - name: Convert instance config dict to a list
           ansible.builtin.set_fact:
             instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
@@ -31,8 +31,7 @@
           ansible.builtin.copy:
             content: |
               # Molecule managed
 
               {{ instance_conf | to_json | from_json | to_yaml }}
             dest: "{{ molecule_instance_config }}"
             mode: 0600
-{%- endraw %}
```

### Comparing `molecule-5.1.0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-6.0.0a0/molecule/default/destroy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ---
-{% raw -%}
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
     # Developer must implement.
@@ -18,9 +17,8 @@
       ansible.builtin.copy:
         content: |
           # Molecule managed
 
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
         mode: 0600
-      when: server.changed | default(false) | bool  # noqa no-handler
-{%- endraw %}
+      when: server.changed | default(false) | bool # noqa no-handler
```

### Comparing `molecule-5.1.0/src/molecule/data/driver.json` & `molecule-6.0.0a0/src/molecule/data/driver.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999819155092593%*

 * *Differences: {"'$defs'": "{'MoleculeDriverModel': {'properties': {'name': {'enum': {insert: [(1, "*

 * *            "'default')]}}}}}"}*

```diff
@@ -1,14 +1,15 @@
 {
     "$defs": {
         "MoleculeDriverModel": {
             "properties": {
                 "name": {
                     "enum": [
-                        "delegated"
+                        "delegated",
+                        "default"
                     ],
                     "title": "Name",
                     "type": "string"
                 },
                 "options": {
                     "$ref": "#/$defs/MoleculeDriverOptionsModel"
                 },
```

### Comparing `molecule-5.1.0/src/molecule/data/molecule.json` & `molecule-6.0.0a0/src/molecule/data/molecule.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722220082045803%*

 * *Differences: {"'$defs'": "{'MoleculeDriverModel': {'properties': {'name': {'anyOf': {0: {'enum': {insert: [(3, "*

 * *            "'default')]}}}}}}}",*

 * * "'required'": '{delete: [0]}'}*

```diff
@@ -95,14 +95,15 @@
                 "name": {
                     "anyOf": [
                         {
                             "enum": [
                                 "azure",
                                 "ec2",
                                 "delegated",
+                                "default",
                                 "docker",
                                 "containers",
                                 "openstack",
                                 "podman",
                                 "vagrant",
                                 "digitalocean",
                                 "gce",
@@ -619,13 +620,12 @@
             "$ref": "#/$defs/MoleculeScenarioModel"
         },
         "verifier": {
             "$ref": "#/$defs/VerifierModel"
         }
     },
     "required": [
-        "driver",
         "platforms"
     ],
     "title": "Molecule Scenario Schema",
     "type": "object"
 }
```

### Comparing `molecule-5.1.0/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,14 @@
         super().__init__(config)
         self._sh_command = None
 
         self.command = "ansible-galaxy"
 
     @property
     @abc.abstractmethod
-    def install_path(self):  # cover
-        pass
-
-    @property
-    @abc.abstractmethod
     def requirements_file(self):  # cover
         pass
 
     @property
     def default_options(self):
         d = {
             "force": True,
@@ -101,18 +96,20 @@
         None.
 
         :return: None
         """
         options = self.options
         verbose_flag = util.verbose_flag(options)
 
-        self._sh_command = util.BakedCommand(
-            cmd=[self.command, *self.COMMANDS, *util.dict2args(options), *verbose_flag],
-            env=self.env,
-        )
+        self._sh_command = [
+            self.command,
+            *self.COMMANDS,
+            *util.dict2args(options),
+            *verbose_flag,
+        ]
 
     def execute(self, action_args=None):
         if not self.enabled:
             msg = "Skipping, dependency is disabled."
             LOG.warning(msg)
             return
         super().execute()
@@ -129,12 +126,10 @@
         self.execute_with_retries()
 
     def _setup(self):
         """Prepare the system for using ``ansible-galaxy`` and returns None.
 
         :return: None
         """
-        if not os.path.isdir(self.install_path):
-            os.makedirs(self.install_path, exist_ok=True)
 
     def _has_requirements_file(self):
         return os.path.isfile(self.requirements_file)
```

### Comparing `molecule-5.1.0/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,44 +7,32 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class Collections(AnsibleGalaxyBase):
     """Collection-specific Ansible Galaxy dependency handling."""
 
-    FILTER_OPTS = ("role-file", "roles-path")  # type: ignore
+    FILTER_OPTS = ("role-file",)  # type: ignore
     COMMANDS = ("collection", "install")
 
     @property
     def default_options(self):
         general = super().default_options
         specific = util.merge_dicts(
             general,
             {
                 "requirements-file": os.path.join(
                     self._config.scenario.directory,
                     "collections.yml",
                 ),
-                "collections-path": os.path.join(
-                    self._config.scenario.ephemeral_directory,
-                    "collections",
-                ),
             },
         )
 
         return specific
 
     @property
     def default_env(self):
-        general = super().default_env
-        return util.merge_dicts(
-            general,
-            {self._config.ansible_collections_path: self.install_path},
-        )
-
-    @property
-    def install_path(self):
-        return self.options["collections-path"]
+        return super().default_env
 
     @property
     def requirements_file(self):
         return self.options["requirements-file"]
```

### Comparing `molecule-5.1.0/src/molecule/dependency/base.py` & `molecule-6.0.0a0/src/molecule/dependency/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base Dependency Module."""
+from __future__ import annotations
 
 import abc
 import logging
 import os
 import time
 from subprocess import CalledProcessError
 
@@ -42,14 +43,15 @@
     def __init__(self, config) -> None:
         """Initialize code for all :ref:`Dependency` classes.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
+        self._sh_command: list[str] | None = None
 
     def execute_with_retries(self):
         """Run dependency downloads with retry and timed back-off."""
         exception = None
 
         try:
             util.run_command(self._sh_command, debug=self._config.debug, check=True)
```

### Comparing `molecule-5.1.0/src/molecule/dependency/shell.py` & `molecule-6.0.0a0/src/molecule/dependency/shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Shell Dependency Module."""
 
 import logging
 
 from molecule.dependency import base
-from molecule.util import BakedCommand
 
 LOG = logging.getLogger(__name__)
 
 
 class Shell(base.Base):
     """``Shell`` is an alternate dependency manager.
 
@@ -80,23 +79,22 @@
 
     @property
     def default_options(self):
         return {}
 
     def bake(self) -> None:
         """Bake a ``shell`` command so it's ready to execute."""
-        self._sh_command = BakedCommand(cmd=self.command, env=self.env)  # type: ignore
+        self._sh_command = self.command
 
     def execute(self, action_args=None):
         if not self.enabled:
             msg = "Skipping, dependency is disabled."
             LOG.warning(msg)
             return
         super().execute()
 
         if self._sh_command is None:
             self.bake()
-
         self.execute_with_retries()
 
     def _has_command_configured(self):
         return "command" in self._config.config["dependency"]
```

### Comparing `molecule-5.1.0/src/molecule/driver/base.py` & `molecule-6.0.0a0/src/molecule/driver/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 """Base Driver Module."""
 
 import inspect
 import os
 from abc import ABCMeta, abstractmethod
 from importlib.metadata import version
 
-import molecule
 from molecule.status import Status
 
 
 class Driver:
     """Driver Class."""
 
     __metaclass__ = ABCMeta
@@ -56,25 +55,14 @@
     def name(self, value):  # pragma: no cover
         """Driver name setter and returns None.
 
         :returns: None
         """
 
     @property
-    def testinfra_options(self):
-        """Testinfra specific options and returns a dict.
-
-        :returns: dict
-        """
-        return {
-            "connection": "ansible",
-            "ansible-inventory": self._config.provisioner.inventory_directory,
-        }
-
-    @property
     @abstractmethod
     def login_cmd_template(self):  # pragma: no cover
         """Get the login command template to be populated by ``login_options`` as \
         a string.
 
         :returns: str
         """
@@ -109,15 +97,15 @@
         dict.
 
         :param instance_name: A string containing the instance to login to.
         :returns: dict
         """
 
     @abstractmethod
-    def sanity_checks(self):
+    def sanity_checks(self) -> None:
         """Confirm that driver is usable.
 
         Sanity checks to ensure the driver can do work successfully. For
         example, when using the Docker driver, we want to know that the Docker
         daemon is running and we have the correct Docker Python dependency.
         Each driver implementation can decide what is the most stable sanity
         check for itself.
@@ -144,19 +132,19 @@
 
     @property
     def safe_files(self):
         return self.default_safe_files + self._config.config["driver"]["safe_files"]
 
     @property
     def delegated(self):
-        """Is the driver delegated and returns a bool.
+        """Is the dedriver delegated and returns a bool.
 
         :returns: bool
         """
-        return self.name == "delegated"
+        return self.name == "default"
 
     @property
     def managed(self):
         """Is the driver is managed and returns a bool.
 
         :returns: bool
         """
@@ -236,29 +224,14 @@
         """Return detailed string representation of object."""
         return self.name
 
     def __rich__(self):
         """Return rich representation of object."""
         return self.__str__()
 
-    def template_dir(self):
-        p = os.path.join(self._path, "cookiecutter")
-
-        if not os.path.isdir(p):
-            p = os.path.abspath(
-                os.path.join(
-                    os.path.dirname(molecule.__file__),
-                    "cookiecutter",
-                    "scenario",
-                    "driver",
-                    self.name,
-                ),
-            )
-        return p
-
     def get_playbook(self, step):
         """Return embedded playbook location or None.
 
         The default location is relative to the file implementing the driver
         class, allowing driver writers to define playbooks without having
         to override this method.
         """
```

### Comparing `molecule-5.1.0/src/molecule/driver/delegated.py` & `molecule-6.0.0a0/src/molecule/driver/delegated.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 from molecule.api import Driver
 from molecule.data import __file__ as data_module
 
 LOG = logging.getLogger(__name__)
 
 
 class Delegated(Driver):
-    r"""The class responsible for managing delegated instances.
+    r"""The class responsible for managing default instances.
 
     Delegated is `not` the default driver used in Molecule.
 
     Under this driver, it is the developers responsibility to implement the
     create and destroy playbooks.  ``Managed`` is the default behaviour of all
     drivers.
 
     ``` yaml
         driver:
-          name: delegated
+          name: de
     ```
 
     However, the developer must adhere to the instance-config API. The
     developer's create playbook must provide the following instance-config
     data, and the developer's destroy playbook must reset the instance-config.
 
     ``` yaml
@@ -77,15 +77,15 @@
 
     Molecule can also skip the provisioning/deprovisioning steps.  It is the
     developers responsibility to manage the instances, and properly configure
     Molecule to connect to said instances.
 
     ``` yaml
         driver:
-          name: delegated
+          name: default
           options:
             managed: False
             login_cmd_template: 'docker exec -ti {instance} bash'
             ansible_connection_options:
               ansible_connection: docker
         platforms:
           - name: instance-docker
@@ -103,49 +103,49 @@
 
     !!! note
 
         It is the developer's responsibility to configure the ssh config file.
 
     ``` yaml
         driver:
-          name: delegated
+          name: default
           options:
             managed: False
             login_cmd_template: 'ssh {instance} -F /tmp/ssh-config'
             ansible_connection_options:
               ansible_connection: ssh
               ansible_ssh_common_args: '-F /path/to/ssh-config'
         platforms:
           - name: instance
     ```
 
     Provide the files Molecule will preserve post ``destroy`` action.
 
     ``` yaml
         driver:
-          name: delegated
+          name: default
           safe_files:
             - foo
     ```
     And in order to use localhost as molecule's target:
 
     ``` yaml
         driver:
-          name: delegated
+          name: default
           options:
             managed: False
             ansible_connection_options:
               ansible_connection: local
     ```
     """
 
     def __init__(self, config=None) -> None:
         """Construct Delegated."""
         super().__init__(config)
-        self._name = "delegated"
+        self._name = "default"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
@@ -210,29 +210,27 @@
         if self.managed:
             try:
                 d = self._get_instance_config(instance_name)
                 conn_dict = {}
                 # Check if optional mappable params are in the instance config
                 for i in instance_params:
                     if d.get(i[0], i[1]):
-                        conn_dict["ansible_" + i[0]] = d.get(i[0])
+                        conn_dict["ansible_" + i[0]] = d.get(i[0], i[1])
 
                 conn_dict["ansible_user"] = d.get("user")
                 conn_dict["ansible_host"] = d.get("address")
                 conn_dict["ansible_port"] = d.get("port")
 
                 if d.get("identity_file", None):
                     conn_dict["ansible_private_key_file"] = d.get("identity_file")
                     conn_dict["ansible_ssh_common_args"] = " ".join(
                         self.ssh_connection_options,
                     )
                 if d.get("password", None):
                     conn_dict["ansible_password"] = d.get("password")
-                    # Based on testinfra documentation, ansible password must be passed via ansible_ssh_pass
-                    # issue to fix this can be found https://github.com/pytest-dev/pytest-testinfra/issues/580
                     conn_dict["ansible_ssh_pass"] = d.get("password")
 
                 return conn_dict
 
             except StopIteration:
                 return {}
             except OSError:
```

### Comparing `molecule-5.1.0/src/molecule/interpolation.py` & `molecule-6.0.0a0/src/molecule/interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,30 +28,14 @@
         self.string = string
         self.place = place
 
 
 class Interpolator:
     """Configuration options may contain environment variables.
 
-    For example, suppose the shell contains ``VERIFIER_NAME=testinfra`` and
-    the following molecule.yml is supplied.
-
-    ```yaml
-        verifier:
-          - name: ${VERIFIER_NAME}
-    ```
-
-    Molecule will substitute ``$VERIFIER_NAME`` with the value of the
-    ``VERIFIER_NAME`` environment variable.
-
-    !!! warning
-
-        If an environment variable is not set, Molecule substitutes with an
-        empty string.
-
     Both ``$VARIABLE`` and ``${VARIABLE}`` syntax are supported. Extended
     shell-style features, such as ``${VARIABLE-default}`` and
     ``${VARIABLE:-default}`` are also supported. Even the default as another
     environment variable is supported like ``${VARIABLE-$DEFAULT}`` or
     ``${VARIABLE:-$DEFAULT}``. An empty string is returned when
     both variables are undefined.
```

### Comparing `molecule-5.1.0/src/molecule/logger.py` & `molecule-6.0.0a0/src/molecule/logger.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/model/schema_v3.py` & `molecule-6.0.0a0/src/molecule/model/schema_v3.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/platforms.py` & `molecule-6.0.0a0/src/molecule/platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/provisioner/ansible.py` & `molecule-6.0.0a0/src/molecule/provisioner/ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         of the `privilege_escalation`.
 
     ``` yaml
         provisioner:
           name: ansible
           config_options:
             defaults:
-              roles_path: /path/to/roles_path
               library: /path/to/library
               filter_plugins: /path/to/filter_plugins
             privilege_escalation: {}
     ```
 
     Roles which require host/groups to have certain variables set.  Molecule
     uses the same `variables defined in a playbook`_ syntax as `Ansible`_.
@@ -460,20 +459,14 @@
         # Finds if the current project is part of an ansible_collections hierarchy
         collection_indicator = "ansible_collections"
         # isolating test environment by injects ephemeral scenario directory on
         # top of the collection_path_list. This prevents dependency commands
         # from installing dependencies to user list of collections.
         collections_path_list = [
             util.abs_path(
-                os.path.join(
-                    self._config.scenario.config.runtime.cache_dir,
-                    "collections",
-                ),
-            ),
-            util.abs_path(
                 os.path.join(self._config.scenario.ephemeral_directory, "collections"),
             ),
         ]
         if collection_indicator in self._config.project_directory:
             collection_path, right = self._config.project_directory.rsplit(
                 collection_indicator,
                 1,
@@ -497,17 +490,14 @@
                         os.environ["ANSIBLE_COLLECTIONS_PATH"].split(":"),
                     ),
                 ),
             )
 
         roles_path_list = [
             util.abs_path(
-                os.path.join(self._config.scenario.config.runtime.cache_dir, "roles"),
-            ),
-            util.abs_path(
                 os.path.join(self._config.scenario.ephemeral_directory, "roles"),
             ),
             util.abs_path(os.path.join(self._config.project_directory, os.path.pardir)),
             util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
             "/usr/share/ansible/roles",
             "/etc/ansible/roles",
         ]
@@ -589,37 +579,29 @@
     @property
     def env(self):
         default_env = self.default_env
         env = self._config.config["provisioner"]["env"].copy()
         # ensure that all keys and values are strings
         env = {str(k): str(v) for k, v in env.items()}
 
-        roles_path = default_env["ANSIBLE_ROLES_PATH"]
         library_path = default_env["ANSIBLE_LIBRARY"]
         filter_plugins_path = default_env["ANSIBLE_FILTER_PLUGINS"]
 
         try:
-            path = self._absolute_path_for(env, "ANSIBLE_ROLES_PATH")
-            roles_path = f"{roles_path}:{path}"
-        except KeyError:
-            pass
-
-        try:
             path = self._absolute_path_for(env, "ANSIBLE_LIBRARY")
             library_path = f"{library_path}:{path}"
         except KeyError:
             pass
 
         try:
             path = self._absolute_path_for(env, "ANSIBLE_FILTER_PLUGINS")
             filter_plugins_path = f"{filter_plugins_path}:{path}"
         except KeyError:
             pass
 
-        env["ANSIBLE_ROLES_PATH"] = roles_path
         env["ANSIBLE_LIBRARY"] = library_path
         env["ANSIBLE_FILTER_PLUGINS"] = filter_plugins_path
 
         return util.merge_dicts(default_env, env)
 
     @property
     def hosts(self):
```

### Comparing `molecule-5.1.0/src/molecule/provisioner/ansible_playbook.py` & `molecule-6.0.0a0/src/molecule/provisioner/ansible_playbook.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Ansible-Playbook Provisioner Module."""
 
 import logging
+import shlex
 import warnings
 
 from molecule import util
 from molecule.api import MoleculeRuntimeWarning
 
 LOG = logging.getLogger(__name__)
 
@@ -82,25 +83,21 @@
         if self._config.action not in ["create", "destroy"]:
             ansible_args = list(self._config.provisioner.ansible_args) + list(
                 self._config.ansible_args,
             )
         else:
             ansible_args = []
 
-        self._ansible_command = util.BakedCommand(
-            cmd=[
-                "ansible-playbook",
-                *util.dict2args(options),
-                *util.bool2args(verbose_flag),
-                *ansible_args,
-                self._playbook,  # must always go last
-            ],
-            cwd=self._config.scenario.directory,
-            env=self._env,
-        )
+        self._ansible_command = [
+            "ansible-playbook",
+            *util.dict2args(options),
+            *util.bool2args(verbose_flag),
+            *ansible_args,
+            self._playbook,  # must always go last
+        ]
 
     def execute(self, action_args=None):
         """Execute ``ansible-playbook`` and returns a string.
 
         :return: str
         """
         if self._ansible_command is None:
@@ -109,19 +106,25 @@
         if not self._playbook:
             LOG.warning("Skipping, %s action has no playbook.", self._config.action)
             return None
 
         with warnings.catch_warnings(record=True) as warns:
             warnings.filterwarnings("default", category=MoleculeRuntimeWarning)
             self._config.driver.sanity_checks()
-            result = util.run_command(self._ansible_command, debug=self._config.debug)
+            result = util.run_command(
+                cmd=self._ansible_command,
+                env=self._env,
+                debug=self._config.debug,
+            )
 
         if result.returncode != 0:
+            from rich.markup import escape
+
             util.sysexit_with_message(
-                f"Ansible return code was {result.returncode}, command was: {result.args}",
+                f"Ansible return code was {result.returncode}, command was: [dim]{escape(shlex.join(result.args))}[/dim]",
                 result.returncode,
                 warns=warns,
             )
 
         return result.stdout
 
     def add_cli_arg(self, name, value):
```

### Comparing `molecule-5.1.0/src/molecule/provisioner/ansible_playbooks.py` & `molecule-6.0.0a0/src/molecule/provisioner/ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/provisioner/base.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,48 +13,34 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
-"""Provisioner Base Module."""
 
-import abc
+from molecule.model import schema_v3
+from molecule.util import run_command
 
 
-class Base:
-    """Provisioner Base Class."""
+def test_base_config(_config):
+    assert not schema_v3.validate(_config)
 
-    __metaclass__ = abc.ABCMeta
 
-    def __init__(self, config) -> None:
-        """Initialize code for all :ref:`Provisioner` classes.
-
-        :param config: An instance of a Molecule config.
-        :returns: None
-        """
-        self._config = config
-
-    @property
-    @abc.abstractmethod
-    def default_options(self):  # pragma: no cover
-        """Get default CLI arguments provided to ``cmd`` as a dict.
-
-        :return: dict
-        """
-
-    @property
-    @abc.abstractmethod
-    def default_env(self):  # pragma: no cover
-        """Get default env variables provided to ``cmd`` as a dict.
-
-        :return: dict
-        """
-
-    @property
-    @abc.abstractmethod
-    def name(self):  # pragma: no cover
-        """Name of the provisioner and returns a string.
-
-        :returns: str
-        """
+def test_molecule_schema():
+    cmd = [
+        "check-jsonschema",
+        "-v",
+        "--schemafile",
+        "src/molecule/data/molecule.json",
+        "src/molecule/test/resources/schema_instance_files/valid/molecule.yml",
+    ]
+    assert run_command(cmd).returncode == 0
+
+    cmd = [
+        "check-jsonschema",
+        "-v",
+        "--schemafile",
+        "src/molecule/data/driver.json",
+        "src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml",
+    ]
+    assert run_command(cmd).returncode != 0
```

### Comparing `molecule-5.1.0/src/molecule/scenario.py` & `molecule-6.0.0a0/src/molecule/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/scenarios.py` & `molecule-6.0.0a0/src/molecule/scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/shell.py` & `molecule-6.0.0a0/src/molecule/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/state.py` & `molecule-6.0.0a0/src/molecule/state.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/status.py` & `molecule-6.0.0a0/src/molecule/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 class Status(NamedTuple):
     """Scenario status information."""
 
     instance_name: str
     driver_name: str
     provisioner_name: str
     scenario_name: str
-    created: bool
-    converged: bool
+    created: str
+    converged: str
```

### Comparing `molecule-5.1.0/src/molecule/test/conftest.py` & `molecule-6.0.0a0/src/molecule/test/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/functional/conftest.py` & `molecule-6.0.0a0/src/molecule/test/b_functional/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             assert run_command(cmd).returncode == 0
 
 
 @pytest.fixture()
 def skip_test(request, driver_name):
     msg_tmpl = "Skipped '{}' not supported"
     support_checks_map = {
-        "delegated": lambda: True,
+        "default": lambda: True,
     }
     try:
         check_func = support_checks_map[driver_name]
         if not check_func():
             pytest.skip(msg_tmpl.format(driver_name))
     except KeyError:
         pass
@@ -101,45 +101,25 @@
     cmd = ["molecule", "converge", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
     cmd = ["molecule", "idempotence", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-def init_role(temp_dir, driver_name):
-    role_directory = os.path.join(temp_dir.strpath, "myrole")
-
-    cmd = ["molecule", "init", "role", "myorg.myrole", "--driver-name", driver_name]
-    assert run_command(cmd).returncode == 0
-    metadata_lint_update(role_directory)
-
-    with change_dir_to(role_directory):
-        cmd = ["molecule", "test", "--all"]
-        assert run_command(cmd).returncode == 0
-
-
 def init_scenario(temp_dir, driver_name):
-    # Create role
-    role_directory = os.path.join(temp_dir.strpath, "test_init")
-    cmd = ["molecule", "init", "role", "myorg.test_init", "--driver-name", driver_name]
-    assert run_command(cmd).returncode == 0
-    metadata_lint_update(role_directory)
-
-    with change_dir_to(role_directory):
+    with change_dir_to(temp_dir.strpath):
         # Create scenario
         molecule_dir = molecule_directory()
         scenario_directory = os.path.join(molecule_dir, "test-scenario")
 
         cmd = [
             "molecule",
             "init",
             "scenario",
             "test-scenario",
-            "--role-name",
-            "test_init",
             "--driver-name",
             driver_name,
         ]
         assert run_command(cmd).returncode == 0
 
         assert os.path.isdir(scenario_directory)
 
@@ -205,15 +185,15 @@
         child.expect(regexp)
         # If the test returns and doesn't hang it succeeded.
         child.sendline("exit")
 
 
 def run_test(driver_name, scenario_name="default", parallel=False):
     cmd = ["molecule", "test", "--scenario-name", scenario_name]
-    if driver_name != "delegated":
+    if driver_name != "default":
         if scenario_name is None:
             cmd.append("--all")
         if parallel:
             cmd.append("--parallel")
 
     assert run_command(cmd).returncode == 0
```

### Comparing `molecule-5.1.0/src/molecule/test/functional/test_command.py` & `molecule-6.0.0a0/src/molecule/test/b_functional/test_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 
 import os
 from typing import Optional
 
 import pytest
 from pytest import FixtureRequest
 
-from molecule.test.functional.conftest import (
+from molecule.test.b_functional.conftest import (
     idempotence,
-    init_role,
     init_scenario,
     list_with_format_plain,
     run_test,
     verify,
 )
 from molecule.util import run_command
 
@@ -65,77 +64,76 @@
         return None
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_check(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "check", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_cleanup(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "cleanup", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_converge(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "converge", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_create(scenario_to_test, with_scenario, scenario_name, tmp_path):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd, env=os.environ).returncode == 0
 
 
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
         pytest.param(
             "dependency",
-            "delegated",
+            "default",
             "shell",
-            id="shell",
         ),
         pytest.param(
             "dependency",
-            "delegated",
+            "default",
             "ansible-galaxy",
             id="galaxy",
         ),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
@@ -148,79 +146,62 @@
     assert run_command(cmd, echo=True).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
-    [("driver/delegated", "delegated", "default")],
+    [("driver/delegated", "default", "default")],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_destroy(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "destroy", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_idempotence(scenario_to_test, with_scenario, scenario_name):
     idempotence(scenario_name)
 
 
 @pytest.mark.serial()
-@pytest.mark.parametrize("driver_name", [("delegated")], indirect=["driver_name"])
-def test_command_init_role(temp_dir, driver_name):
-    init_role(temp_dir, driver_name)
-
-
-@pytest.mark.serial()
-@pytest.mark.parametrize("driver_name", [("delegated")], indirect=["driver_name"])
-def test_command_init_scenario(temp_dir, driver_name):
-    init_scenario(temp_dir, driver_name)
+def test_command_init_scenario(temp_dir):
+    init_scenario(temp_dir, "default")
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "expected"),
     [
         (
             "driver/delegated",
-            "delegated",
-            "instance        delegated       ansible default",
+            "default",
+            "instance        default ansible default",
         ),
     ],
     indirect=["scenario_to_test", "driver_name"],
 )
 def test_command_list_with_format_plain(scenario_to_test, with_scenario, expected):
     list_with_format_plain(expected)
 
 
-# @pytest.mark.parametrize(
-#     "scenario_to_test, driver_name, login_args, scenario_name",
-#             "driver/delegated",
-#             "delegated",
-#             "default",
-#         ),
-#     ],
-# def test_command_login(scenario_to_test, with_scenario, login_args, scenario_name):
-
-
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_prepare(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
@@ -229,42 +210,42 @@
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_side_effect(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "side-effect", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_syntax(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "syntax", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test(scenario_to_test, with_scenario, scenario_name, driver_name):
     run_test(driver_name, scenario_name)
 
 
@@ -280,28 +261,28 @@
         "--debug",
         "test",
         "--scenario-name",
         scenario_name,
         "--platform-name",
         platform_name,
     ]
-    if driver_name != "delegated":
+    if driver_name != "default":
         if scenario_name is None:
             cmd.append("--all")
         if parallel:
             cmd.append("--parallel")
 
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name", "platform_name"),
     [
-        ("driver/delegated", "delegated", "default", "instance"),
+        ("driver/delegated", "default", "default", "instance"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name", "platform_name"],
 )
 def test_command_test_with_platform_name(
     scenario_to_test,
     with_scenario,
     scenario_name,
@@ -313,15 +294,15 @@
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
         (
             "driver/delegated_invalid_role_name_with_role_name_check_equals_to_1",
-            "delegated",
+            "default",
             "default",
         ),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test_with_role_name_check_equals_to_1(
     scenario_to_test,
@@ -333,23 +314,32 @@
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "delegated", "default"),
+        ("driver/delegated", "default", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_verify(scenario_to_test, with_scenario, scenario_name):
     verify(scenario_name)
 
 
-def test_sample_collection():
+def test_sample_collection() -> None:
     assert (
         run_command(
             ["molecule", "test"],
             cwd="src/molecule/test/resources/sample-collection",
         ).returncode
         == 0
     )
+
+
+def test_podman() -> None:
+    assert (
+        run_command(
+            ["molecule", "test", "--scenario-name", "podman"],
+        ).returncode
+        == 0
+    )
```

### Comparing `molecule-5.1.0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml` & `molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   options:
     ignore-certs: true
     ignore-errors: true
   env:
     FOO: bar
 
 driver:
-  name: delegated
+  name: default
   options:
     managed: false
     login_cmd_template: ...
     ansible_connection_options:
       ansible_connection: ssh
 
 log: true
@@ -64,8 +64,8 @@
     - prepare
     - converge
     - check
     - verify
     - destroy
 
 verifier:
-  name: testinfra
+  name: ansible
```

### Comparing `molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 dependency:
   name: galaxy
 driver:
-  name: delegated
+  name: default
 platforms:
   - name: instance
     image: ${TEST_BASE_IMAGE}
     groups:
       - example
     children:
       - example_1
```

### Comparing `molecule-5.1.0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 """Testinfra tests."""
 
-import os
-
-import testinfra.utils.ansible_runner
-
-testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"],
-).get_hosts("all")
-
 
 def test_hostname(host):
     """Validate hostname."""
     assert host.check_output("hostname -s") == "instance"
 
 
 def test_etc_molecule_directory(host):
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/conftest.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,21 @@
     return mocker.patch("molecule.provisioner.ansible.Ansible.create")
 
 
 @pytest.fixture()
 def command_driver_delegated_section_data():
     x = {
         "driver": {
-            "name": "delegated",
+            "name": "default",
             "options": {
                 "managed": False,
             },
         },
     }
     # if "DOCKER_HOST" in os.environ:
     #     x["driver"]["options"]["ansible_docker_extra_args"] = "-H={}".format(
     return x
 
 
 @pytest.fixture()
 def command_driver_delegated_managed_section_data():
-    return {"driver": {"name": "delegated", "managed": True}}
+    return {"driver": {"name": "default", "managed": True}}
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/init/test_role.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/init/test_scenario.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,52 +18,49 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
 
-from molecule.command.init import role
+from molecule.command.init import scenario
 
 
 @pytest.fixture()
 def _command_args():
     return {
-        "dependency_name": "galaxy",
-        "driver_name": "delegated",
-        "provisioner_name": "ansible",
-        "role_name": "acme.test_role",
-        "scenario_name": "default",
+        "driver_name": "default",
+        "role_name": "test-role",
+        "scenario_name": "test-scenario",
         "subcommand": __name__,
         "verifier_name": "ansible",
     }
 
 
 @pytest.fixture()
 def _instance(_command_args):
-    return role.Role(_command_args)
+    return scenario.Scenario(_command_args)
 
 
 def test_execute(temp_dir, _instance, patched_logger_info):
     _instance.execute()
 
-    msg = "Initializing new role test_role..."
+    msg = "Initializing new scenario test-scenario..."
     patched_logger_info.assert_any_call(msg)
 
-    assert os.path.isdir("./test_role")
-    assert os.path.isdir("./test_role/molecule/default")
+    assert os.path.isdir("./molecule/test-scenario")
 
-    role_directory = os.path.join(temp_dir.strpath, "test_role")
-    msg = f"Initialized role in {role_directory} successfully."
+    scenario_directory = os.path.join(temp_dir.strpath, "molecule", "test-scenario")
+    msg = f"Initialized scenario in {scenario_directory} successfully."
     patched_logger_info.assert_any_call(msg)
 
 
-def test_execute_role_exists(temp_dir, _instance, patched_logger_critical):
+def test_execute_scenario_exists(temp_dir, _instance, caplog):
     _instance.execute()
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
-    msg = "The directory test_role exists. Cannot create new role."
-    patched_logger_critical.assert_called_once_with(msg)
+    msg = "The directory molecule/test-scenario exists. Cannot create new scenario."
+    assert msg in caplog.text
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/init/test_scenario.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_scenario_section.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,74 +14,45 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import os
-
 import pytest
 
-from molecule.command.init import scenario
+from molecule.model import schema_v3
 
 
 @pytest.fixture()
-def _command_args():
+def _model_scenario_section_data():
     return {
-        "driver_name": "delegated",
-        "role_name": "test-role",
-        "scenario_name": "test-scenario",
-        "subcommand": __name__,
-        "verifier_name": "ansible",
+        "scenario": {
+            "name": "foo",
+            "check_sequence": ["check"],
+            "converge_sequence": ["converge"],
+            "create_sequence": ["create"],
+            "destroy_sequence": ["destroy"],
+            "test_sequence": ["test"],
+        },
     }
 
 
-@pytest.fixture()
-def _instance(_command_args):
-    return scenario.Scenario(_command_args)
+@pytest.mark.parametrize("_config", ["_model_scenario_section_data"], indirect=True)
+def test_scenario(_config):
+    assert not schema_v3.validate(_config)
 
 
 @pytest.fixture()
-def invalid_template_dir(resources_folder_path):
-    invalid_role_template_path = os.path.join(
-        resources_folder_path,
-        "invalid_scenario_template",
-    )
-    return invalid_role_template_path
-
-
-def test_execute(temp_dir, _instance, patched_logger_info):
-    _instance.execute()
-
-    msg = "Initializing new scenario test-scenario..."
-    patched_logger_info.assert_any_call(msg)
-
-    assert os.path.isdir("./molecule/test-scenario")
-
-    scenario_directory = os.path.join(temp_dir.strpath, "molecule", "test-scenario")
-    msg = f"Initialized scenario in {scenario_directory} successfully."
-    patched_logger_info.assert_any_call(msg)
-
-
-def test_execute_scenario_exists(temp_dir, _instance, patched_logger_critical):
-    _instance.execute()
-
-    with pytest.raises(SystemExit) as e:
-        _instance.execute()
-
-    assert e.value.code == 1
-
-    msg = "The directory molecule/test-scenario exists. Cannot create new scenario."
-    patched_logger_critical.assert_called_once_with(msg)
+def _model_scenario_errors_section_data():
+    return {"scenario": {"name": 0}}
 
 
-def test_execute_with_invalid_driver(
-    temp_dir,
-    _instance,
-    _command_args,
-    patched_logger_critical,
-):
-    _command_args["driver_name"] = "ec3"
+@pytest.mark.parametrize(
+    "_config",
+    ["_model_scenario_errors_section_data"],
+    indirect=True,
+)
+def test_scenario_has_errors(_config):
+    x = ["0 is not of type 'string'"]
 
-    with pytest.raises(KeyError):
-        _instance.execute()
+    assert x == schema_v3.validate(_config)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_base.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import config, util
 from molecule.command import base
 
 
 class ExtendedBase(base.Base):
     """ExtendedBase Class."""
@@ -33,26 +34,26 @@
         pass
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _base_class(patched_config_validate, config_instance):
+def _base_class(patched_config_validate, config_instance: config.Config):
     return ExtendedBase
 
 
 @pytest.fixture()
-def _instance(_base_class, config_instance):
+def _instance(_base_class, config_instance: config.Config):
     return _base_class(config_instance)
 
 
 @pytest.fixture()
 def _patched_base_setup(mocker):
-    return mocker.patch("molecule.test.unit.command.test_base.ExtendedBase._setup")
+    return mocker.patch("molecule.test.a_unit.command.test_base.ExtendedBase._setup")
 
 
 @pytest.fixture()
 def _patched_write_config(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.write_config")
 
 
@@ -91,94 +92,94 @@
 
 
 def test_init_calls_setup(_patched_base_setup, _instance):
     _patched_base_setup.assert_called_once_with()
 
 
 def test_setup(
-    mocker,
+    mocker: MockerFixture,
     patched_add_or_update_vars,
     _patched_write_config,
     _patched_manage_inventory,
     _instance,
 ):
     assert os.path.isdir(os.path.dirname(_instance._config.provisioner.inventory_file))
     assert os.path.isfile(_instance._config.config_file)
 
     _patched_manage_inventory.assert_called_once_with()
     _patched_write_config.assert_called_once_with()
 
 
 def test_execute_cmdline_scenarios(
-    config_instance,
+    config_instance: config.Config,
     _patched_print_matrix,
     _patched_execute_scenario,
 ):
     # Ensure execute_cmdline_scenarios runs normally:
     # - scenarios.print_matrix is called, which also indicates Scenarios
     #   was instantiated correctly
     # - execute_scenario is called once, indicating the function correctly
     #   loops over Scenarios.
     scenario_name = None
-    args = {}
+    args: dict[str, str] = {}
     command_args = {"destroy": "always", "subcommand": "test"}
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_print_matrix.called_once_with()
     assert _patched_execute_scenario.call_count == 1
 
 
 def test_execute_cmdline_scenarios_prune(
-    config_instance,
+    config_instance: config.Config,
     _patched_prune,
     _patched_execute_subcommand,
 ):
     # Subcommands should be executed and prune *should* run when
     # destroy is 'always'
     scenario_name = "default"
-    args = {}
+    args: dict[str, str] = {}
     command_args = {"destroy": "always", "subcommand": "test"}
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_execute_subcommand.called
     assert _patched_prune.called
 
 
 def test_execute_cmdline_scenarios_no_prune(
-    config_instance,
+    config_instance: config.Config,
     _patched_prune,
     _patched_execute_subcommand,
 ):
     # Subcommands should be executed but prune *should not* run when
     # destroy is 'never'
     scenario_name = "default"
-    args = {}
+    args: dict[str, str] = {}
     command_args = {"destroy": "never", "subcommand": "test"}
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_execute_subcommand.called
     assert not _patched_prune.called
 
 
 def test_execute_cmdline_scenarios_exit_destroy(
-    config_instance,
+    config_instance: config.Config,
     _patched_execute_scenario,
     _patched_prune,
     _patched_execute_subcommand,
     _patched_sysexit,
 ):
     # Ensure execute_cmdline_scenarios handles errors correctly when 'destroy'
     # is 'always':
     # - cleanup and destroy subcommands are run when execute_scenario
     #   raises SystemExit
     # - scenario is pruned
     scenario_name = "default"
-    args = {}
+    args: dict[str, str] = {}
     command_args = {"destroy": "always", "subcommand": "test"}
     _patched_execute_scenario.side_effect = SystemExit()
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_execute_subcommand.call_count == 2
     # pull out the second positional call argument for each call,
@@ -186,152 +187,115 @@
     assert _patched_execute_subcommand.call_args_list[0][0][1] == "cleanup"
     assert _patched_execute_subcommand.call_args_list[1][0][1] == "destroy"
     assert _patched_prune.called
     assert _patched_sysexit.called
 
 
 def test_execute_cmdline_scenarios_exit_nodestroy(
-    config_instance,
+    config_instance: config.Config,
     _patched_execute_scenario,
     _patched_prune,
     _patched_sysexit,
 ):
     # Ensure execute_cmdline_scenarios handles errors correctly when 'destroy'
     # is 'always':
     # - destroy subcommand is not run when execute_scenario raises SystemExit
     # - scenario is not pruned
     # - caught SystemExit is reraised
     scenario_name = "default"
-    args = {}
+    args: dict[str, str] = {}
     command_args = {"destroy": "never", "subcommand": "test"}
 
     _patched_execute_scenario.side_effect = SystemExit()
 
     # Catch the expected SystemExit reraise
     with pytest.raises(SystemExit):
         base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_execute_scenario.called
     assert not _patched_prune.called
     assert not _patched_sysexit.called
 
 
-def test_runtime_paths(config_instance, _patched_sysexit):
-    # the ansible_collections_path and ansible_roles_path from the runtime
-    # should be added to the provisioner's paths
-    scenario_name = None
-    args = {}
-    command_args = {"destroy": "never", "subcommand": "verify"}
-
-    base.result_callback()
-    base.execute_cmdline_scenarios(scenario_name, args, command_args)
-
-    home = os.path.expanduser("~")
-    cache_dir = config_instance.runtime.cache_dir
-    runtime_roles_path = config_instance.runtime.environ.get("ANSIBLE_ROLES_PATH")
-    provisioner_roles_path = config_instance.provisioner.env.get("ANSIBLE_ROLES_PATH")
-    runtime_collections_path = config_instance.runtime.environ.get(
-        config_instance.ansible_collections_path,
-    )
-    provisioner_collections_path = config_instance.provisioner.env.get(
-        config_instance.ansible_collections_path,
-    )
-
-    assert runtime_roles_path.startswith(
-        f"{cache_dir}/roles:"
-        f"{home}/.ansible/roles:"
-        f"/usr/share/ansible/roles:"
-        f"/etc/ansible/roles",
-    )
-
-    assert runtime_collections_path.startswith(
-        f"{cache_dir}/collections:{home}/.ansible/collections",
-    )
-
-    assert provisioner_roles_path.startswith(f"{cache_dir}/roles")
-
-    assert provisioner_collections_path.startswith(f"{cache_dir}/collections")
-
-
-def test_execute_subcommand(config_instance):
+def test_execute_subcommand(config_instance: config.Config):
     # scenario's config.action is mutated in-place for every sequence action,
     # so make sure that is currently set to the executed action
     assert config_instance.action != "list"
     assert base.execute_subcommand(config_instance, "list")
     assert config_instance.action == "list"
 
 
-def test_execute_scenario(mocker, _patched_execute_subcommand):
+def test_execute_scenario(mocker: MockerFixture, _patched_execute_subcommand):
     # call a spoofed scenario with a sequence that does not include destroy:
     # - execute_subcommand should be called once for each sequence item
     # - prune should not be called, since the sequence has no destroy step
     scenario = mocker.Mock()
     scenario.sequence = ("a", "b", "c")
 
     base.execute_scenario(scenario)
 
     assert _patched_execute_subcommand.call_count == len(scenario.sequence)
     assert not scenario.prune.called
 
 
-def test_execute_scenario_destroy(mocker, _patched_execute_subcommand):
+def test_execute_scenario_destroy(mocker: MockerFixture, _patched_execute_subcommand):
     # call a spoofed scenario with a sequence that includes destroy:
     # - execute_subcommand should be called once for each sequence item
     # - prune should be called, since the sequence has a destroy step
     scenario = mocker.Mock()
     scenario.sequence = ("a", "b", "destroy", "c")
 
     base.execute_scenario(scenario)
 
     assert _patched_execute_subcommand.call_count == len(scenario.sequence)
     assert scenario.prune.called
 
 
-def test_get_configs(config_instance):
+def test_get_configs(config_instance: config.Config):
     molecule_file = config_instance.molecule_file
     data = config_instance.config
     util.write_file(molecule_file, util.safe_dump(data))
 
     result = base.get_configs({}, {})
     assert len(result) == 1
     assert isinstance(result, list)
     assert isinstance(result[0], config.Config)
 
 
-def test_verify_configs(config_instance):
+def test_verify_configs(config_instance: config.Config):
     configs = [config_instance]
 
     assert base._verify_configs(configs) is None
 
 
-def test_verify_configs_raises_with_no_configs(patched_logger_critical):
+def test_verify_configs_raises_with_no_configs(caplog):
     with pytest.raises(SystemExit) as e:
         base._verify_configs([])
 
     assert e.value.code == 1
 
     msg = "'molecule/*/molecule.yml' glob failed.  Exiting."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_verify_configs_raises_with_duplicate_configs(
-    patched_logger_critical,
-    config_instance,
+    caplog: pytest.LogCaptureFixture,
+    config_instance: config.Config,
 ):
     with pytest.raises(SystemExit) as e:
         configs = [config_instance, config_instance]
         base._verify_configs(configs)
 
     assert e.value.code == 1
 
     msg = "Duplicate scenario name 'default' found.  Exiting."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
-def test_get_subcommand():
+def test_get_subcommand() -> None:
     assert base._get_subcommand(__name__) == "test_base"
 
 
 @pytest.mark.parametrize(
     "shell",
     [
         "bash",
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_check.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_verify.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,34 +14,28 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
+from pytest_mock import MockerFixture
 
-from molecule.command import check
-
-
-@pytest.fixture()
-def _patched_ansible_check(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.check")
+from molecule import config
+from molecule.command import verify
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 def test_execute(
-    mocker,
-    patched_logger_info,
-    _patched_ansible_check,
+    mocker: MockerFixture,
+    caplog,
+    patched_default_verifier,
     patched_config_validate,
-    config_instance,
+    config_instance: config.Config,
 ):
-    c = check.Check(config_instance)
-    c.execute()
+    v = verify.Verify(config_instance)
+    v.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "check" in args
+    assert "default" in caplog.text
+    assert "verify" in caplog.text
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_cleanup.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_cleanup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
+from pytest_mock import MockerFixture
 
-from molecule import util
+from molecule import config, util
 from molecule.command import cleanup
 
 
 @pytest.fixture()
 def _command_provisioner_section_with_cleanup_data():
     return {"provisioner": {"name": "ansible", "playbooks": {"cleanup": "cleanup.yml"}}}
 
@@ -41,38 +42,36 @@
 # throughout patched.assert_called unit tests.
 @pytest.mark.parametrize(
     "config_instance",
     ["_command_provisioner_section_with_cleanup_data"],
     indirect=True,
 )
 def test_execute(
-    mocker,
+    mocker: MockerFixture,
     _patched_ansible_cleanup,
-    patched_logger_info,
+    caplog,
     patched_config_validate,
-    config_instance,
+    config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "cleanup.yml")
     util.write_file(pb, "")
 
     cu = cleanup.Cleanup(config_instance)
     cu.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "cleanup" in args
+    assert "cleanup" in caplog.text
 
     _patched_ansible_cleanup.assert_called_once_with()
 
 
 def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning,
+    caplog,
     _patched_ansible_cleanup,
-    config_instance,
+    config_instance: config.Config,
 ):
     cu = cleanup.Cleanup(config_instance)
     cu.execute()
 
     msg = "Skipping, cleanup playbook not configured."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
     assert not _patched_ansible_cleanup.called
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_converge.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_converge.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,44 +14,48 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+from typing import Any
+from unittest.mock import Mock
+
 from click.testing import CliRunner
+from pytest import LogCaptureFixture
+from pytest_mock import MockerFixture
 
+from molecule import config
 from molecule.command import converge
 from molecule.shell import main
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 def test_execute(
-    mocker,
-    patched_logger_info,
-    patched_ansible_converge,
-    patched_config_validate,
-    config_instance,
-):
+    mocker: MockerFixture,
+    caplog: LogCaptureFixture,
+    patched_ansible_converge: Mock,
+    patched_config_validate: Any,
+    config_instance: config.Config,
+) -> None:
     c = converge.Converge(config_instance)
     c.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "converge" in args
+    assert "default" in caplog.text
+    assert "converge" in caplog.text
 
     patched_ansible_converge.assert_called_once_with()
 
     assert config_instance.state.converged
 
 
-def test_ansible_args_passed_to_scenarios_get_configs(mocker):
+def test_ansible_args_passed_to_scenarios_get_configs(mocker: MockerFixture) -> None:
     # Scenarios patch is needed to safely invoke CliRunner
     # in the test environment and block scenario execution
     mocker.patch("molecule.scenarios.Scenarios")
     patched_get_configs = mocker.patch("molecule.command.base.get_configs")
 
     runner = CliRunner()
     args = ("converge", "--", "-e", "testvar=testvalue")
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_create.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,77 +14,58 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+
 import pytest
+from pytest_mock import MockerFixture
 
+from molecule import config
 from molecule.command import create
 
 
 @pytest.fixture()
 def _patched_create_setup(mocker):
     return mocker.patch("molecule.command.create.Create._setup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.skip(reason="create not running for delegated")
 def test_execute(
-    mocker,
-    patched_logger_info,
+    mocker: MockerFixture,
+    caplog,
     command_patched_ansible_create,
     patched_config_validate,
-    config_instance,
+    config_instance: config.Config,
 ):
     c = create.Create(config_instance)
     c.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "converge" in args
+    assert "default" in caplog.text
+    assert "converge" in caplog.text
 
-    assert config_instance.state.driver == "delegated"
+    assert config_instance.state.driver == "default"
 
     command_patched_ansible_create.assert_called_once_with()
 
     assert config_instance.state.created
 
 
-@pytest.mark.parametrize(
-    "config_instance",
-    ["command_driver_delegated_section_data"],
-    indirect=True,
-)
-def test_execute_skips_when_delegated_driver(
-    _patched_create_setup,
-    patched_logger_warning,
-    command_patched_ansible_create,
-    config_instance,
-):
-    c = create.Create(config_instance)
-    c.execute()
-
-    msg = "Skipping, instances are delegated."
-    patched_logger_warning.assert_called_once_with(msg)
-
-    assert not command_patched_ansible_create.called
-
-
 @pytest.mark.skip(reason="create not running for delegated")
 def test_execute_skips_when_instances_already_created(
-    patched_logger_warning,
+    caplog,
     command_patched_ansible_create,
-    config_instance,
+    config_instance: config.Config,
 ):
     config_instance.state.change_state("created", True)
     c = create.Create(config_instance)
     c.execute()
 
     msg = "Skipping, instances already created."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
     assert not command_patched_ansible_create.called
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_dependency.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,15 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from molecule.command import dependency
+import pytest
 
+from molecule import shell
 
-# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
-# config.Config._validate from executing.  Thus preventing odd side-effects
-# throughout patched.assert_called unit tests.
-def test_execute(
-    mocker,
-    patched_logger_info,
-    patched_ansible_galaxy,
-    patched_config_validate,
-    config_instance,
-):
-    d = dependency.Dependency(config_instance)
-    d.execute()
 
-    patched_ansible_galaxy.assert_called_once_with()
-
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "dependency" in args
+def test_shell() -> None:
+    with pytest.raises(SystemExit):
+        shell.main()
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_destroy.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_side_effect.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,88 +14,70 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+import os
+
 import pytest
+from pytest_mock import MockerFixture
 
-from molecule.command import destroy
+from molecule import config, util
+from molecule.command import side_effect
 
 
 @pytest.fixture()
-def _patched_ansible_destroy(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.destroy")
+def _command_provisioner_section_with_side_effect_data():
+    return {
+        "provisioner": {
+            "name": "ansible",
+            "playbooks": {"side_effect": "side_effect.yml"},
+        },
+    }
 
 
 @pytest.fixture()
-def _patched_destroy_setup(mocker):
-    return mocker.patch("molecule.command.destroy.Destroy._setup")
+def _patched_ansible_side_effect(mocker):
+    return mocker.patch("molecule.provisioner.ansible.Ansible.side_effect")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.mark.skip(reason="destroy not running for delegated")
-def test_execute(
-    mocker,
-    patched_logger_info,
-    patched_config_validate,
-    _patched_ansible_destroy,
-    config_instance,
-):
-    d = destroy.Destroy(config_instance)
-    d.execute()
-
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "destroy" in args
-
-    assert "verify" in args
-
-    _patched_ansible_destroy.assert_called_once_with()
-
-    assert not config_instance.state.converged
-    assert not config_instance.state.created
-
-
 @pytest.mark.parametrize(
     "config_instance",
-    ["command_driver_delegated_section_data"],
+    ["_command_provisioner_section_with_side_effect_data"],
     indirect=True,
 )
-def test_execute_skips_when_destroy_strategy_is_never(
-    _patched_destroy_setup,
-    patched_logger_warning,
-    _patched_ansible_destroy,
-    config_instance,
+def test_execute(
+    mocker: MockerFixture,
+    _patched_ansible_side_effect,
+    caplog,
+    patched_config_validate,
+    config_instance: config.Config,
 ):
-    config_instance.command_args = {"destroy": "never"}
+    pb = os.path.join(config_instance.scenario.directory, "side_effect.yml")
+    util.write_file(pb, "")
 
-    d = destroy.Destroy(config_instance)
-    d.execute()
+    se = side_effect.SideEffect(config_instance)
+    se.execute()
 
-    msg = "Skipping, '--destroy=never' requested."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert "default" in caplog.text
+    assert "side_effect" in caplog.text
 
-    assert not _patched_ansible_destroy.called
+    _patched_ansible_side_effect.assert_called_once_with(None)
 
 
-@pytest.mark.parametrize(
-    "config_instance",
-    ["command_driver_delegated_section_data"],
-    indirect=True,
-)
-def test_execute_skips_when_delegated_driver(
-    _patched_destroy_setup,
-    patched_logger_warning,
-    _patched_ansible_destroy,
-    config_instance,
+def test_execute_skips_when_playbook_not_configured(
+    caplog,
+    _patched_ansible_side_effect,
+    config_instance: config.Config,
 ):
-    d = destroy.Destroy(config_instance)
-    d.execute()
+    se = side_effect.SideEffect(config_instance)
+    se.execute()
 
-    msg = "Skipping, instances are delegated."
-    patched_logger_warning.assert_called_once_with(msg)
+    msg = "Skipping, side effect playbook not configured."
+    assert msg in caplog.text
 
-    assert not _patched_ansible_destroy.called
+    assert not _patched_ansible_side_effect.called
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_idempotence.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_idempotence.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,86 +13,89 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
+
+from unittest.mock import Mock
+
 import pytest
+from pytest_mock import MockerFixture
 
+from molecule import config
 from molecule.command import idempotence
 
 
 @pytest.fixture()
-def _patched_is_idempotent(mocker):
+def _patched_is_idempotent(mocker: MockerFixture) -> Mock:
     return mocker.patch("molecule.command.idempotence.Idempotence._is_idempotent")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(patched_config_validate, config_instance):
+def _instance(patched_config_validate, config_instance: config.Config):
     config_instance.state.change_state("converged", True)
 
     return idempotence.Idempotence(config_instance)
 
 
 def test_execute(
-    mocker,
-    patched_logger_info,
+    mocker: MockerFixture,
+    caplog: pytest.LogCaptureFixture,
     patched_ansible_converge,
-    _patched_is_idempotent,
+    _patched_is_idempotent: Mock,
     _instance,
 ):
     _instance.execute()
 
-    assert len(patched_logger_info.mock_calls) == 2
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "idempotence" in args
+    assert "default" in caplog.text
+    assert "idempotence" in caplog.text
 
     patched_ansible_converge.assert_called_once_with()
 
     _patched_is_idempotent.assert_called_once_with("patched-ansible-converge-stdout")
 
     msg = "Idempotence completed successfully."
-    patched_logger_info.assert_any_call(msg)
+    assert msg in caplog.text
 
 
 def test_execute_raises_when_not_converged(
-    patched_logger_critical,
+    caplog: pytest.LogCaptureFixture,
     patched_ansible_converge,
     _instance,
 ):
     _instance._config.state.change_state("converged", False)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
     msg = "Instances not converged.  Please converge instances first."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_raises_when_fails_idempotence(
-    mocker,
-    patched_logger_critical,
+    mocker: MockerFixture,
+    caplog: pytest.LogCaptureFixture,
     patched_ansible_converge,
-    _patched_is_idempotent,
+    _patched_is_idempotent: Mock,
     _instance,
 ):
     _patched_is_idempotent.return_value = False
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
     msg = "Idempotence test failed because of the following tasks:\n"
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_is_idempotent(_instance):
     output = """
 PLAY RECAP ***********************************************************
 check-command-01: ok=3    changed=0    unreachable=0    failed=0
     """
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_list.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,32 +14,33 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+from molecule import config
 from molecule.command import list
 from molecule.driver import base
 
 
-def test_execute(capsys, config_instance):
+def test_execute(capsys, config_instance: config.Config):
     l = list.List(config_instance)
     x = [
         base.Status(
             instance_name="instance-1",
-            driver_name="delegated",
+            driver_name="default",
             provisioner_name="ansible",
             scenario_name="default",
             created="false",
             converged="false",
         ),
         base.Status(
             instance_name="instance-2",
-            driver_name="delegated",
+            driver_name="default",
             provisioner_name="ansible",
             scenario_name="default",
             created="false",
             converged="false",
         ),
     ]
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_login.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_login.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,65 +14,68 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+
 import pytest
+from pytest_mock import MockerFixture
 
+from molecule import config
 from molecule.command import login
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     config_instance.state.change_state("created", True)
 
     return login.Login(config_instance)
 
 
-def test_execute(mocker, _instance):
+def test_execute(mocker: MockerFixture, _instance):
     _instance._config.command_args = {"host": "instance-1"}
     m = mocker.patch("molecule.command.login.Login._get_login")
     _instance.execute()
 
     m.assert_called_once_with("instance-1")
 
 
 @pytest.mark.skip(reason="needs rewrite after switch to delegated")
 @pytest.mark.parametrize(
     "config_instance",
     ["command_driver_delegated_managed_section_data"],
     indirect=True,
 )
-def test_execute_raises_when_not_created(patched_logger_critical, _instance):
+def test_execute_raises_when_not_created(caplog, _instance):
     _instance._config.state.change_state("created", False)
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
     msg = "Instances not created.  Please create instances first."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
-def test_get_hostname_does_not_match(patched_logger_critical, _instance):
+def test_get_hostname_does_not_match(caplog, _instance):
     _instance._config.command_args = {"host": "invalid"}
     hosts = ["instance-1"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
     assert e.value.code == 1
 
     msg = (
         "There are no hosts that match 'invalid'.  You "
         "can only login to valid hosts."
     )
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_get_hostname_exact_match_with_one_host(_instance):
     _instance._config.command_args = {"host": "instance-1"}
     hosts = ["instance-1"]
 
     assert _instance._get_hostname(hosts) == "instance-1"
@@ -96,15 +99,15 @@
     _instance._config.command_args = {"host": "foo"}
     hosts = ["foo", "fooo"]
 
     assert _instance._get_hostname(hosts) == "foo"
 
 
 def test_get_hostname_partial_match_with_multiple_hosts_raises(
-    patched_logger_critical,
+    caplog,
     _instance,
 ):
     _instance._config.command_args = {"host": "inst"}
     hosts = ["instance-1", "instance-2"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
@@ -113,27 +116,27 @@
     msg = (
         "There are 2 hosts that match 'inst'. "
         "You can only login to one at a time.\n\n"
         "Available hosts:\n"
         "instance-1\n"
         "instance-2"
     )
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_get_hostname_no_host_flag_specified_on_cli(_instance):
     _instance._config.command_args = {}
     hosts = ["instance-1"]
     _instance._get_hostname(hosts)
 
     assert _instance._get_hostname(hosts) == "instance-1"
 
 
 def test_get_hostname_no_host_flag_specified_on_cli_with_multiple_hosts_raises(
-    patched_logger_critical,
+    caplog,
     _instance,
 ):
     _instance._config.command_args = {}
     hosts = ["instance-1", "instance-2"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
@@ -142,8 +145,8 @@
     msg = (
         "There are 2 running hosts. Please specify "
         "which with --host.\n\n"
         "Available hosts:\n"
         "instance-1\n"
         "instance-2"
     )
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_matrix.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_prepare.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_prepare.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,84 +17,83 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
+from pytest_mock import MockerFixture
 
-from molecule import util
+from molecule import config, util
 from molecule.command import prepare
 
 
 @pytest.fixture()
 def _patched_ansible_prepare(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.prepare")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 def test_execute(
-    mocker,
-    patched_logger_info,
+    mocker: MockerFixture,
+    caplog,
     _patched_ansible_prepare,
     patched_config_validate,
-    config_instance,
+    config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "prepare.yml")
     util.write_file(pb, "")
 
     p = prepare.Prepare(config_instance)
     p.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "prepare" in args
+    assert "default" in caplog.text
+    assert "prepare" in caplog.text
 
     _patched_ansible_prepare.assert_called_once_with()
 
     assert config_instance.state.prepared
 
 
 def test_execute_skips_when_instances_already_prepared(
-    patched_logger_warning,
+    caplog,
     _patched_ansible_prepare,
-    config_instance,
+    config_instance: config.Config,
 ):
     config_instance.state.change_state("prepared", True)
     p = prepare.Prepare(config_instance)
     p.execute()
 
     msg = "Skipping, instances already prepared."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
     assert not _patched_ansible_prepare.called
 
 
 def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning,
+    caplog,
     _patched_ansible_prepare,
-    config_instance,
+    config_instance: config.Config,
 ):
     p = prepare.Prepare(config_instance)
     p.execute()
 
     msg = "Skipping, prepare playbook not configured."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
     assert not _patched_ansible_prepare.called
 
 
 def test_execute_when_instances_already_prepared_but_force_provided(
-    mocker,
-    patched_logger_warning,
+    mocker: MockerFixture,
+    caplog,
     _patched_ansible_prepare,
-    config_instance,
+    config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "prepare.yml")
     util.write_file(pb, "")
 
     config_instance.state.change_state("prepared", True)
     config_instance.command_args = {"force": True}
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_side_effect.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_verifier_section.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,71 +14,50 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import os
-
 import pytest
 
-from molecule import util
-from molecule.command import side_effect
+from molecule.model import schema_v3
+
+
+def test_verifier(_config):
+    assert not schema_v3.validate(_config)
 
 
 @pytest.fixture()
-def _command_provisioner_section_with_side_effect_data():
+def _model_verifier_errors_section_data():
     return {
-        "provisioner": {
-            "name": "ansible",
-            "playbooks": {"side_effect": "side_effect.yml"},
+        "verifier": {
+            "name": 0,
         },
     }
 
 
+@pytest.mark.parametrize(
+    "_config",
+    ["_model_verifier_errors_section_data"],
+    indirect=True,
+)
+def test_verifier_has_errors(_config):
+    x = ["0 is not one of ['ansible', 'goss', 'inspec', 'testinfra']"]
+
+    assert x == schema_v3.validate(_config)
+
+
 @pytest.fixture()
-def _patched_ansible_side_effect(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.side_effect")
+def _model_verifier_allows_ansible_section_data():
+    return {"verifier": {"name": "ansible"}}
 
 
-# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
-# config.Config._validate from executing.  Thus preventing odd side-effects
-# throughout patched.assert_called unit tests.
 @pytest.mark.parametrize(
-    "config_instance",
-    ["_command_provisioner_section_with_side_effect_data"],
+    "_config",
+    [
+        ("_model_verifier_allows_ansible_section_data"),
+    ],
     indirect=True,
 )
-def test_execute(
-    mocker,
-    _patched_ansible_side_effect,
-    patched_logger_info,
-    patched_config_validate,
-    config_instance,
-):
-    pb = os.path.join(config_instance.scenario.directory, "side_effect.yml")
-    util.write_file(pb, "")
-
-    se = side_effect.SideEffect(config_instance)
-    se.execute()
-
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "side_effect" in args
-
-    _patched_ansible_side_effect.assert_called_once_with(None)
-
-
-def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning,
-    _patched_ansible_side_effect,
-    config_instance,
-):
-    se = side_effect.SideEffect(config_instance)
-    se.execute()
-
-    msg = "Skipping, side effect playbook not configured."
-    patched_logger_warning.assert_called_once_with(msg)
-
-    assert not _patched_ansible_side_effect.called
+def test_verifier_allows_name(_config):
+    assert not schema_v3.validate(_config)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_syntax.py` & `molecule-6.0.0a0/src/molecule/command/init/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,37 +13,30 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
+"""Base class used by init command."""
 
-import pytest
+import abc
+import logging
+import os
 
-from molecule.command import syntax
+from molecule import util
 
+LOG = logging.getLogger(__name__)
 
-@pytest.fixture()
-def _patched_ansible_syntax(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.syntax")
-
-
-# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
-# config.Config._validate from executing.  Thus preventing odd side-effects
-# throughout patched.assert_called unit tests.
-def test_execute(
-    mocker,
-    patched_logger_info,
-    _patched_ansible_syntax,
-    patched_config_validate,
-    config_instance,
-):
-    s = syntax.Syntax(config_instance)
-    s.execute()
-
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "syntax" in args
 
-    _patched_ansible_syntax.assert_called_once_with()
+class Base:
+    """Init Command Base Class."""
+
+    __metaclass__ = abc.ABCMeta
+
+    def _validate_template_dir(self, template_dir):
+        if not os.path.isdir(template_dir):
+            util.sysexit_with_message(
+                "The specified template directory ("
+                + str(template_dir)
+                + ") does not exist",
+            )
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_test.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/command/test_verify.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_platforms_section.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,27 +14,19 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from molecule.command import verify
+import pytest
 
+from molecule.model import schema_v3
 
-# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
-# config.Config._validate from executing.  Thus preventing odd side-effects
-# throughout patched.assert_called unit tests.
-def test_execute(
-    mocker,
-    patched_logger_info,
-    patched_default_verifier,
-    patched_config_validate,
-    config_instance,
-):
-    v = verify.Verify(config_instance)
-    v.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "verify" in args
+@pytest.mark.parametrize(
+    "_config",
+    ["_model_platforms_delegated_section_data"],
+    indirect=True,
+)
+def test_platforms_delegated(_config):
+    assert not schema_v3.validate(_config)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/conftest.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 import copy
 import os
 import shutil
 from collections.abc import Generator
 from pathlib import Path
 from subprocess import CompletedProcess
 from typing import Any
+from unittest.mock import Mock
 from uuid import uuid4
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import config, util
 from molecule.test.conftest import (
     molecule_directory,
     molecule_ephemeral_directory,
     molecule_file,
     molecule_scenario_directory,
@@ -52,15 +54,15 @@
 @pytest.fixture()
 def _molecule_dependency_galaxy_section_data():
     return {"dependency": {"name": "galaxy"}}
 
 
 @pytest.fixture()
 def _molecule_driver_section_data():
-    return {"driver": {"name": "delegated", "options": {"managed": True}}}
+    return {"driver": {"name": "default", "options": {"managed": True}}}
 
 
 @pytest.fixture()
 def _molecule_platforms_section_data():
     return {
         "platforms": [
             {"name": "instance-1", "groups": ["foo", "bar"], "children": ["child1"]},
@@ -181,43 +183,33 @@
 
 @pytest.fixture()
 def patched_logger_debug(mocker):
     return mocker.patch("logging.Logger.debug")
 
 
 @pytest.fixture()
-def patched_logger_warning(mocker):
-    return mocker.patch("logging.Logger.warning")
-
-
-@pytest.fixture()
 def patched_logger_error(mocker):
     return mocker.patch("logging.Logger.error")
 
 
 @pytest.fixture()
-def patched_logger_critical(mocker):
-    return mocker.patch("logging.Logger.critical")
-
-
-@pytest.fixture()
 def patched_run_command(mocker):
     m = mocker.patch("molecule.util.run_command")
     m.return_value = CompletedProcess(
         args="foo",
         returncode=0,
         stdout="patched-run-command-stdout",
         stderr="",
     )
 
     return m
 
 
 @pytest.fixture()
-def patched_ansible_converge(mocker):
+def patched_ansible_converge(mocker: MockerFixture) -> Mock:
     m = mocker.patch("molecule.provisioner.ansible.Ansible.converge")
     m.return_value = "patched-ansible-converge-stdout"
 
     return m
 
 
 @pytest.fixture()
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/cookiecutter/test_molecule.py` & `molecule-6.0.0a0/src/molecule/command/converge.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,69 +13,48 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
+"""Converge Command Module."""
+from __future__ import annotations
 
-import os
+import logging
 
-import pytest
+import click
 
-from molecule import util
-from molecule.command.init import base
-from molecule.model import schema_v3
+from molecule.command import base
 
+LOG = logging.getLogger(__name__)
 
-class CommandBase(base.Base):
-    """CommandBase Class."""
 
+class Converge(base.Base):
+    """Converge Command Class."""
 
-@pytest.fixture()
-def _base_class():
-    return CommandBase
+    def execute(self, action_args: list[str] | None = None) -> None:
+        """Execute the actions necessary to perform a `molecule converge` and \
+        returns None.
 
+        :return: None
+        """
+        self._config.provisioner.converge()
+        self._config.state.change_state("converged", True)
 
-@pytest.fixture()
-def _instance(_base_class):
-    return _base_class()
 
+@base.click_command_ex()
+@click.pass_context
+@click.option(
+    "--scenario-name",
+    "-s",
+    default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
+    help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
+)
+@click.argument("ansible_args", nargs=-1, type=click.UNPROCESSED)
+def converge(ctx, scenario_name, ansible_args):  # pragma: no cover
+    """Use the provisioner to configure instances (dependency, create, prepare converge)."""
+    args = ctx.obj.get("args")
+    subcommand = base._get_subcommand(__name__)
+    command_args = {"subcommand": subcommand}
 
-@pytest.fixture()
-def _role_directory():
-    return "."
-
-
-@pytest.fixture()
-def _command_args():
-    return {
-        "dependency_name": "galaxy",
-        "driver_name": "delegated",
-        "provisioner_name": "ansible",
-        "scenario_name": "default",
-        "role_name": "test-role",
-        "verifier_name": "ansible",
-    }
-
-
-@pytest.fixture()
-def _molecule_file(_role_directory):
-    return os.path.join(
-        _role_directory,
-        "test-role",
-        "molecule",
-        "default",
-        "molecule.yml",
-    )
-
-
-def test_valid(temp_dir, _molecule_file, _role_directory, _command_args, _instance):
-    _instance._process_templates("molecule", _command_args, _role_directory)
-
-    data = util.safe_load_file(_molecule_file)
-
-    assert not schema_v3.validate(data)
-
-    cmd = ["yamllint", "-s", _molecule_file]
-    result = util.run_command(cmd)
-    assert result.returncode == 0
+    base.execute_cmdline_scenarios(scenario_name, args, command_args, ansible_args)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,34 +48,33 @@
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(_dependency_section_data, patched_config_validate, config_instance):
+def _instance(
+    _dependency_section_data,
+    patched_config_validate,
+    config_instance: config.Config,
+):
     return collections.Collections(config_instance)
 
 
 @pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "collections.yml")
 
 
-@pytest.fixture()
-def roles_path(_instance):
-    return os.path.join(_instance._config.scenario.ephemeral_directory, "collections")
-
-
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance, role_file, roles_path):
-    x = {"requirements-file": role_file, "collections-path": roles_path, "force": True}
+def test_default_options_property(_instance, role_file):
+    x = {"requirements-file": role_file, "force": True}
 
     assert x == _instance.default_options
 
 
 def test_default_env_property(_instance):
     env = _instance.default_env
 
@@ -90,127 +89,115 @@
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property(_instance, role_file, roles_path):
+def test_options_property(_instance, role_file):
     x = {
         "force": True,
         "requirements-file": role_file,
-        "collections-path": roles_path,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property_handles_cli_args(role_file, roles_path, _instance):
+def test_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
         "force": True,
         "requirements-file": role_file,
-        "collections-path": roles_path,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_collections_bake(_instance, role_file, roles_path):
+def test_collections_bake(_instance, role_file):
     _instance.bake()
     args = [
         "ansible-galaxy",
         "collection",
         "install",
-        "--collections-path",
-        roles_path,
         "--foo",
         "bar",
         "--force",
         "--requirements-file",
         role_file,
         "-v",
     ]
-    assert _instance._sh_command.cmd == args
+    assert _instance._sh_command == args
 
 
 def test_execute(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
-    patched_logger_info,
+    caplog,
     _instance,
 ):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
-    role_directory = os.path.join(
-        _instance._config.scenario.directory,
-        _instance.options["collections-path"],
-    )
-    assert os.path.isdir(role_directory)
-
     patched_run_command.assert_called_once_with(
         "patched-command",
         debug=False,
         check=True,
     )
 
     msg = "Dependency completed successfully."
-    patched_logger_info.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute_when_disabled(
     patched_run_command,
-    patched_logger_warning,
+    caplog,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute_when_no_requirements_file(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
-    patched_logger_warning,
+    caplog,
     _instance,
 ):
     _patched_ansible_galaxy_has_requirements_file.return_value = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, missing the requirements file."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_bakes(
     patched_run_command,
     _instance,
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
-    roles_path,
 ):
     _instance.execute()
-    assert _instance._sh_command is not None
 
     assert patched_run_command.call_count == 1
 
 
 def test_collections_executes_catches_and_exits_return_code(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
@@ -220,24 +207,16 @@
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
 
 def test_setup(_instance):
-    role_directory = os.path.join(
-        _instance._config.scenario.directory,
-        _instance.options["collections-path"],
-    )
-    assert not os.path.isdir(role_directory)
-
     _instance._setup()
 
-    assert os.path.isdir(role_directory)
-
 
 def test_role_file(role_file, _instance):
     assert role_file == _instance.requirements_file
 
 
 def test_has_requirements_file(_instance):
     assert not _instance._has_requirements_file()
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,34 +47,33 @@
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(_dependency_section_data, patched_config_validate, config_instance):
+def _instance(
+    _dependency_section_data,
+    patched_config_validate,
+    config_instance: config.Config,
+):
     return roles.Roles(config_instance)
 
 
 @pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "requirements.yml")
 
 
-@pytest.fixture()
-def roles_path(_instance):
-    return os.path.join(_instance._config.scenario.ephemeral_directory, "roles")
-
-
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance, role_file, roles_path):
-    x = {"role-file": role_file, "roles-path": roles_path, "force": True}
+def test_default_options_property(_instance, role_file):
+    x = {"role-file": role_file, "force": True}
 
     assert x == _instance.default_options
 
 
 def test_default_env_property(_instance):
     env = _instance.default_env
 
@@ -89,123 +88,112 @@
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property(_instance, role_file, roles_path):
+def test_options_property(_instance, role_file):
     x = {
         "force": True,
         "role-file": role_file,
-        "roles-path": roles_path,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property_handles_cli_args(role_file, roles_path, _instance):
+def test_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
         "force": True,
         "role-file": role_file,
-        "roles-path": roles_path,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_galaxy_bake(_instance, role_file, roles_path):
+def test_galaxy_bake(_instance, role_file):
     _instance.bake()
     args = [
         "ansible-galaxy",
         "install",
         "--foo",
         "bar",
         "--force",
         "--role-file",
         role_file,
-        "--roles-path",
-        roles_path,
         "-v",
     ]
-    assert _instance._sh_command.cmd == args
+    assert _instance._sh_command == args
 
 
 def test_execute(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
-    patched_logger_info,
+    caplog,
     _instance,
 ):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
-    role_directory = os.path.join(
-        _instance._config.scenario.directory,
-        _instance.options["roles-path"],
-    )
-    assert os.path.isdir(role_directory)
-
     patched_run_command.assert_called_once_with(
         "patched-command",
         debug=False,
         check=True,
     )
 
     msg = "Dependency completed successfully."
-    patched_logger_info.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute_when_disabled(
     patched_run_command,
-    patched_logger_warning,
+    caplog,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute_when_no_requirements_file(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
-    patched_logger_warning,
+    caplog,
     _instance,
 ):
     _patched_ansible_galaxy_has_requirements_file.return_value = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, missing the requirements file."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_bakes(
     patched_run_command,
     _instance,
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
-    roles_path,
 ):
     _instance.execute()
     assert _instance._sh_command is not None
 
     assert patched_run_command.call_count == 1
 
 
@@ -217,25 +205,13 @@
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
 
-def test_setup(_instance):
-    role_directory = os.path.join(
-        _instance._config.scenario.directory,
-        _instance.options["roles-path"],
-    )
-    assert not os.path.isdir(role_directory)
-
-    _instance._setup()
-
-    assert os.path.isdir(role_directory)
-
-
 def test_role_file(role_file, _instance):
     assert role_file == _instance.requirements_file
 
 
 def test_has_requirements_file(_instance):
     assert not _instance._has_requirements_file()
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/dependency/test_shell.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/test_shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+
 import pytest
 
 from molecule import config
 from molecule.dependency import shell
 
 
 @pytest.fixture()
@@ -36,15 +37,19 @@
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(_dependency_section_data, patched_config_validate, config_instance):
+def _instance(
+    _dependency_section_data,
+    patched_config_validate,
+    config_instance: config.Config,
+):
     return shell.Shell(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
@@ -86,47 +91,45 @@
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
-def test_execute(patched_run_command, patched_logger_info, _instance):
+def test_execute(patched_run_command, caplog: pytest.LogCaptureFixture, _instance):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
     patched_run_command.assert_called_once_with(
         "patched-command",
         debug=False,
         check=True,
     )
 
     msg = "Dependency completed successfully."
-    patched_logger_info.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute_when_disabled(
     patched_run_command,
-    patched_logger_warning,
+    caplog: pytest.LogCaptureFixture,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_execute_bakes(patched_run_command, _instance):
     _instance.execute()
-    assert _instance._sh_command is not None
-
     assert patched_run_command.call_count == 1
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_dep_executes_catches_and_exits_return_code(patched_run_command, _instance):
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/driver/test_delegated.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/driver/test_delegated.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,62 +17,56 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import config
 from molecule.driver import delegated
 from molecule.test.conftest import is_subset
 
 
 @pytest.fixture()
 def _driver_managed_section_data():
     return {
         "driver": {
-            "name": "delegated",
+            "name": "default",
             "options": {
                 "managed": True,
             },
         },
     }
 
 
 @pytest.fixture()
 def _driver_unmanaged_section_data():
     return {
         "driver": {
-            "name": "delegated",
+            "name": "default",
             "options": {
                 "managed": False,
             },
         },
     }
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     return delegated.Delegated(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_testinfra_options_property(_instance):
-    assert {
-        "connection": "ansible",
-        "ansible-inventory": _instance._config.provisioner.inventory_directory,
-    } == _instance.testinfra_options
-
-
 def test_name_property(_instance):
-    assert _instance.name == "delegated"
+    assert _instance.name == "default"
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_unmanaged_section_data"],
     indirect=True,
 )
@@ -169,15 +163,15 @@
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_managed_section_data"],
     indirect=True,
 )
-def test_login_options_when_managed(mocker, _instance):
+def test_login_options_when_managed(mocker: MockerFixture, _instance):
     m = mocker.patch("molecule.driver.delegated.Delegated._get_instance_config")
     m.return_value = {
         "instance": "foo",
         "address": "172.16.0.2",
         "user": "cloud-user",
         "port": 22,
         "become_method": "su",
@@ -210,15 +204,15 @@
 
 @pytest.mark.xfail(reason="Needs rewrite since switch to delegated")
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_managed_section_data"],
     indirect=True,
 )
-def test_ansible_connection_options_when_managed(mocker, _instance):
+def test_ansible_connection_options_when_managed(mocker: MockerFixture, _instance):
     assert _instance.managed is True
 
     ssh_case_data = mocker.patch(
         "molecule.driver.delegated.Delegated._get_instance_config",
     )
     ssh_case_data.return_value = {
         "instance": "foo",
@@ -269,25 +263,25 @@
         "ansible_connection": "winrm",
     }
 
     assert winrm_expected_data == _instance.ansible_connection_options("foo")
 
 
 def test_ansible_connection_options_handles_missing_instance_config_managed(
-    mocker,
+    mocker: MockerFixture,
     _instance,
 ):
     m = mocker.patch("molecule.util.safe_load_file")
     m.side_effect = IOError
 
     assert {} == _instance.ansible_connection_options("foo")
 
 
 def test_ansible_connection_options_handles_missing_results_key_when_managed(
-    mocker,
+    mocker: MockerFixture,
     _instance,
 ):
     m = mocker.patch("molecule.util.safe_load_file")
     m.side_effect = StopIteration
 
     assert {} == _instance.ansible_connection_options("foo")
 
@@ -306,28 +300,28 @@
     ["_driver_unmanaged_section_data"],
     indirect=True,
 )
 def test_ssh_connection_options_property(_instance):
     assert [] == _instance.ssh_connection_options
 
 
-def test_status(mocker, _instance):
+def test_status(mocker: MockerFixture, _instance):
     result = _instance.status()
 
     assert len(result) == 2
 
     assert result[0].instance_name == "instance-1"
-    assert result[0].driver_name == "delegated"
+    assert result[0].driver_name == "default"
     assert result[0].provisioner_name == "ansible"
     assert result[0].scenario_name == "default"
     assert result[0].created == "false"
     assert result[0].converged == "false"
 
     assert result[1].instance_name == "instance-2"
-    assert result[1].driver_name == "delegated"
+    assert result[1].driver_name == "default"
     assert result[1].provisioner_name == "ansible"
     assert result[1].scenario_name == "default"
     assert result[1].created == "false"
     assert result[1].converged == "false"
 
 
 def test_created(_instance):
@@ -351,13 +345,13 @@
     assert _instance._created() == "unknown"
 
 
 def test_property(_instance):
     assert _instance._converged() == "false"
 
 
-def test_get_instance_config(mocker, _instance):
+def test_get_instance_config(mocker: MockerFixture, _instance):
     m = mocker.patch("molecule.util.safe_load_file")
     m.return_value = [{"instance": "foo"}, {"instance": "bar"}]
 
     x = {"instance": "foo"}
     assert x == _instance._get_instance_config("foo")
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/model/v2/conftest.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/model/v2/test_dependency_section.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_dependency_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/model/v2/test_driver_section.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_driver_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from molecule.model import schema_v3
 
 
 @pytest.fixture()
 def _model_driver_section_data():
     return {
         "driver": {
-            "name": "delegated",
+            "name": "default",
             "provider": {"name": None},
             "options": {"managed": True},
             "ssh_connection_options": ["foo", "bar"],
             "safe_files": ["foo", "bar"],
         },
     }
 
@@ -91,15 +91,15 @@
 )
 def test_driver_provider_name_nullable(_config):
     assert not schema_v3.validate(_config)
 
 
 @pytest.fixture()
 def _model_driver_allows_delegated_section_data():
-    return {"driver": {"name": "delegated"}}
+    return {"driver": {"name": "default"}}
 
 
 @pytest.fixture()
 def _model_driver_allows_molecule_section_data1():
     return {"driver": {"name": "molecule-test_driver.name"}}
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/model/v2/test_platforms_section.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#  Copyright (c) 2019 Red Hat, Inc.
 #  Copyright (c) 2015-2018 Cisco Systems, Inc.
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to
 #  deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 #  sell copies of the Software, and to permit persons to whom the Software is
@@ -14,19 +15,29 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
+from molecule import api
 
-from molecule.model import schema_v3
 
+def test_api_molecule_drivers_as_attributes():
+    results = api.drivers()
+    assert hasattr(results, "default")
+    assert isinstance(results.default, api.Driver)
 
-@pytest.mark.parametrize(
-    "_config",
-    ["_model_platforms_delegated_section_data"],
-    indirect=True,
-)
-def test_platforms_delegated(_config):
-    assert not schema_v3.validate(_config)
+
+def test_api_drivers():
+    results = api.drivers()
+
+    for result in results:
+        assert isinstance(result, api.Driver)
+
+    assert "default" in results
+
+
+def test_api_verifiers():
+    x = ["ansible"]
+
+    assert all(elem in api.verifiers() for elem in x)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/model/v2/test_provisioner_section.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_provisioner_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import collections
 import os
 import re
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import config, util
 from molecule.provisioner import ansible, ansible_playbooks
-from molecule.test.unit.conftest import os_split
+from molecule.test.a_unit.conftest import os_split
 
 
 @pytest.fixture()
 def _patched_ansible_playbook(mocker):
     m = mocker.patch("molecule.provisioner.ansible_playbook.AnsiblePlaybook")
     m.return_value.execute.return_value = b"patched-ansible-playbook-stdout"
 
@@ -83,15 +84,15 @@
                 },
             },
         },
     }
 
 
 @pytest.fixture()
-def _instance(_provisioner_section_data, config_instance):
+def _instance(_provisioner_section_data, config_instance: config.Config):
     return ansible.Ansible(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
@@ -208,37 +209,14 @@
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
     indirect=True,
 )
 def test_env_appends_env_property(_instance):
-    os.environ["ANSIBLE_ROLES_PATH"] = ""
-
-    expected = [
-        util.abs_path(os.path.join(_instance._config.runtime.cache_dir, "roles")),
-        util.abs_path(
-            os.path.join(_instance._config.scenario.ephemeral_directory, "roles"),
-        ),
-        util.abs_path(
-            os.path.join(_instance._config.project_directory, os.path.pardir),
-        ),
-        util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
-        "/usr/share/ansible/roles",
-        "/etc/ansible/roles",
-        util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
-    ]
-
-    # molecule could decide to add extra paths, so we only want to check
-    # that those that we need are kept inside the list with exact order
-
-    roles_path_list = _instance.env["ANSIBLE_ROLES_PATH"].split(":")
-
-    assert roles_path_list == expected
-
     x = _instance._get_modules_directories()
     x.append(
         util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
     )
     assert x == _instance.env["ANSIBLE_LIBRARY"].split(":")
 
     x = [
@@ -263,46 +241,14 @@
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
     indirect=True,
 )
-def test_env_appends_env_property_with_os_env(_instance):
-    os.environ["ANSIBLE_ROLES_PATH"] = "/foo/bar:/foo/baz"
-
-    expected = [
-        util.abs_path(os.path.join(_instance._config.runtime.cache_dir, "roles")),
-        util.abs_path(
-            os.path.join(_instance._config.scenario.ephemeral_directory, "roles"),
-        ),
-        util.abs_path(
-            os.path.join(_instance._config.project_directory, os.path.pardir),
-        ),
-        util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
-        "/usr/share/ansible/roles",
-        "/etc/ansible/roles",
-        "/foo/bar",
-        "/foo/baz",
-        util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
-    ]
-
-    # molecule could decide to add extra paths, so we only want to check
-    # that those that we need are kept inside the list
-
-    roles_path_list = _instance.env["ANSIBLE_ROLES_PATH"].split(":")
-
-    assert roles_path_list == expected
-
-
-@pytest.mark.parametrize(
-    "config_instance",
-    ["_provisioner_section_data"],
-    indirect=True,
-)
 def test_host_vars_property(_instance):
     x = {"instance-1": [{"foo": "bar"}], "localhost": [{"foo": "baz"}]}
 
     assert x == _instance.host_vars
 
 
 @pytest.mark.parametrize(
@@ -377,130 +323,134 @@
     assert x == _instance.playbooks.converge
 
 
 def test_playbooks_side_effect_property(_instance):
     assert _instance.playbooks.side_effect is None
 
 
-def test_check(_instance, mocker, _patched_ansible_playbook):
+def test_check(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.check()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.converge,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.add_cli_arg.assert_called_once_with(
         "check",
         True,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_converge(_instance, mocker, _patched_ansible_playbook):
+def test_converge(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     result = _instance.converge()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.converge,
         _instance._config,
         False,
     )
     # NOTE(retr0h): This is not the true return type.  This is a mock return
     #               which didn't go through str.decode().
     assert result == b"patched-ansible-playbook-stdout"
 
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_converge_with_playbook(_instance, mocker, _patched_ansible_playbook):
+def test_converge_with_playbook(
+    _instance,
+    mocker: MockerFixture,
+    _patched_ansible_playbook,
+):
     result = _instance.converge("playbook")
 
     _patched_ansible_playbook.assert_called_once_with(
         "playbook",
         _instance._config,
         False,
     )
     # NOTE(retr0h): This is not the true return type.  This is a mock return
     #               which didn't go through str.decode().
     assert result == b"patched-ansible-playbook-stdout"
 
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_cleanup(_instance, mocker, _patched_ansible_playbook):
+def test_cleanup(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.cleanup()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.cleanup,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_destroy(_instance, mocker, _patched_ansible_playbook):
+def test_destroy(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.destroy()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.destroy,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_side_effect(_instance, mocker, _patched_ansible_playbook):
+def test_side_effect(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.side_effect()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.side_effect,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_create(_instance, mocker, _patched_ansible_playbook):
+def test_create(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.create()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.create,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_prepare(_instance, mocker, _patched_ansible_playbook):
+def test_prepare(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.prepare()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.prepare,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_syntax(_instance, mocker, _patched_ansible_playbook):
+def test_syntax(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.syntax()
 
     _patched_ansible_playbook.assert_called_once_with(
         _instance._config.provisioner.playbooks.converge,
         _instance._config,
         False,
     )
     _patched_ansible_playbook.return_value.add_cli_arg.assert_called_once_with(
         "syntax-check",
         True,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_verify(_instance, mocker, _patched_ansible_playbook):
+def test_verify(_instance, mocker: MockerFixture, _patched_ansible_playbook):
     _instance.verify()
 
     if _instance._config.provisioner.playbooks.verify:
         _patched_ansible_playbook.assert_called_once_with(
             _instance._config.provisioner.playbooks.verify,
             _instance._config,
         )
@@ -700,45 +650,45 @@
     _instance._link_or_update_vars()
 
     assert os.path.lexists(target_hosts)
     assert os.path.lexists(target_group_vars)
     assert os.path.lexists(target_host_vars)
 
 
-def test_link_vars_raises_when_source_not_found(_instance, patched_logger_critical):
+def test_link_vars_raises_when_source_not_found(_instance, caplog):
     c = _instance._config.config
     c["provisioner"]["inventory"]["links"] = {"foo": "../bar"}
 
     with pytest.raises(SystemExit) as e:
         _instance._link_or_update_vars()
 
     assert e.value.code == 1
 
     source = os.path.join(_instance._config.scenario.directory, os.path.pardir, "bar")
     msg = f"The source path '{source}' does not exist."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_verify_inventory(_instance):
     _instance._verify_inventory()
 
 
 def test_verify_inventory_raises_when_missing_hosts(
     temp_dir,
-    patched_logger_critical,
+    caplog,
     _instance,
 ):
     _instance._config.config["platforms"] = []
     with pytest.raises(SystemExit) as e:
         _instance._verify_inventory()
 
     assert e.value.code == 1
 
     msg = "Instances missing from the 'platform' section of molecule.yml."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_vivify(_instance):
     d = _instance._vivify()
     d["bar"]["baz"] = "qux"
 
     assert str(d["bar"]["baz"]) == "qux"
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible_playbook.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pytest
 
 from molecule import config
 from molecule.provisioner import ansible_playbook
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     _instance = ansible_playbook.AnsiblePlaybook("playbook", config_instance)
 
     return _instance
 
 
 @pytest.fixture()
 def _provisioner_section_data():
@@ -48,15 +48,15 @@
     return {
         "provisioner": {"name": "ansible", "env": {"FOO": "bar"}},
         "verifier": {"name": "ansible", "env": {"FOO": "baz"}},
     }
 
 
 @pytest.fixture()
-def _instance_for_verifier_env(config_instance):
+def _instance_for_verifier_env(config_instance: config.Config):
     _instance = ansible_playbook.AnsiblePlaybook("playbook", config_instance, True)
     return _instance
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
@@ -108,15 +108,15 @@
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest",
         pb,
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
 def test_bake_removes_non_interactive_options_from_non_converge_playbooks(
     _inventory_directory,
     _instance,
 ):
     _instance.bake()
@@ -126,15 +126,15 @@
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest",
         "playbook",
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
 def test_bake_has_ansible_args(_inventory_directory, _instance):
     _instance._config.ansible_args = ("foo", "bar")
     _instance._config.config["provisioner"]["ansible_args"] = ("frob", "nitz")
     _instance.bake()
 
@@ -147,15 +147,15 @@
         "frob",
         "nitz",
         "foo",
         "bar",
         "playbook",
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
 def test_bake_does_not_have_ansible_args(_inventory_directory, _instance):
     for action in ["create", "destroy"]:
         _instance._config.ansible_args = ("foo", "bar")
         _instance._config.action = action
         _instance.bake()
@@ -165,15 +165,15 @@
             "--inventory",
             _inventory_directory,
             "--skip-tags",
             "molecule-notest,notest",
             "playbook",
         ]
 
-        assert _instance._ansible_command.cmd == args
+        assert _instance._ansible_command == args
 
 
 def test_bake_idem_does_have_skip_tag(_inventory_directory, _instance):
     _instance._config.action = "idempotence"
     _instance.bake()
 
     args = [
@@ -181,22 +181,20 @@
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest,molecule-idempotence-notest",
         "playbook",
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
-def test_execute(patched_run_command, _instance):
+def test_execute_playbook(patched_run_command, _instance):
     _instance._ansible_command = "patched-command"
     result = _instance.execute()
-
-    patched_run_command.assert_called_once_with("patched-command", debug=False)
     assert result == "patched-run-command-stdout"
 
 
 def test_execute_bakes(_inventory_directory, patched_run_command, _instance):
     _instance.execute()
 
     assert _instance._ansible_command is not None
@@ -206,15 +204,15 @@
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest",
         "playbook",
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
 def test_execute_bakes_with_ansible_args(
     _inventory_directory,
     patched_run_command,
     _instance,
 ):
@@ -225,27 +223,24 @@
 
     args = [
         "ansible-playbook",
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest",
-        # "--foo",
-        # "--bar",
         "-o",
         "--syntax-check",
         "playbook",
     ]
 
-    assert _instance._ansible_command.cmd == args
+    assert _instance._ansible_command == args
 
 
 def test_executes_catches_and_exits_return_code(
     patched_run_command,
-    patched_logger_critical,
     _instance,
 ):
     patched_run_command.side_effect = [
         CompletedProcess(
             args="ansible-playbook",
             returncode=1,
             stdout="out",
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/provisioner/test_ansible_playbooks.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,49 +18,49 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
 
-from molecule import util
+from molecule import config, util
 from molecule.provisioner import ansible_playbooks
-from molecule.test.unit.conftest import os_split
+from molecule.test.a_unit.conftest import os_split
 
 
 @pytest.fixture()
 def _provisioner_section_data():
     return {"provisioner": {"name": "ansible", "options": {}, "config_options": {}}}
 
 
 @pytest.fixture()
-def _instance(_provisioner_section_data, config_instance):
+def _instance(_provisioner_section_data, config_instance: config.Config):
     return ansible_playbooks.AnsiblePlaybooks(config_instance)
 
 
 def test_cleanup_property_is_optional(_instance):
     assert _instance._config.provisioner.playbooks.cleanup is None
 
 
 @pytest.mark.skip(reason="create not running for delegated")
 def test_create_property(_instance):
-    x = os.path.join(_instance._get_playbook_directory(), "delegated", "create.yml")
+    x = os.path.join(_instance._get_playbook_directory(), "default", "create.yml")
 
     assert x == _instance._config.provisioner.playbooks.create
 
 
 def test_converge_property(_instance):
     x = os.path.join(_instance._config.scenario.directory, "converge.yml")
 
     assert x == _instance._config.provisioner.playbooks.converge
 
 
 @pytest.mark.skip(reason="destroy not running for delegated")
 def test_destroy_property(_instance):
-    x = os.path.join(_instance._get_playbook_directory(), "delegated", "destroy.yml")
+    x = os.path.join(_instance._get_playbook_directory(), "default", "destroy.yml")
 
     assert x == _instance._config.provisioner.playbooks.destroy
 
 
 def test_prepare_property(_instance):
     assert _instance._config.provisioner.playbooks.prepare is None
 
@@ -89,15 +89,15 @@
 
 
 @pytest.mark.skip(reason="create not running for delegated")
 def test_get_playbook_returns_bundled_driver_playbook_when_local_not_found(
     tmpdir,
     _instance,
 ):
-    x = os.path.join(_instance._get_playbook_directory(), "delegated", "create.yml")
+    x = os.path.join(_instance._get_playbook_directory(), "default", "create.yml")
 
     assert x == _instance._get_playbook("create")
 
 
 @pytest.fixture()
 def _provisioner_driver_section_data():
     return {
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_config.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,330 +17,343 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import config, platforms, scenario, state, util
 from molecule.dependency import ansible_galaxy, shell
 from molecule.provisioner import ansible
 from molecule.verifier.ansible import Ansible as AnsibleVerifier
 
 
-def test_molecule_file_private_member(molecule_file_fixture, config_instance):
+def test_molecule_file_private_member(
+    molecule_file_fixture,
+    config_instance: config.Config,
+):
     assert molecule_file_fixture == config_instance.molecule_file
 
 
-def test_args_member(config_instance):
+def test_args_member(config_instance: config.Config):
     assert {} == config_instance.args
 
 
-def test_command_args_member(config_instance):
+def test_command_args_member(config_instance: config.Config):
     x = {"subcommand": "test"}
 
     assert x == config_instance.command_args
 
 
-def test_debug_property(config_instance):
+def test_debug_property(config_instance: config.Config):
     assert not config_instance.debug
 
 
-def test_env_file_property(config_instance):
+def test_env_file_property(config_instance: config.Config):
     config_instance.args = {"env_file": ".env"}
     result = config_instance.env_file
 
-    assert util.abs_path(config_instance.args.get("env_file")) == result
+    x = config_instance.args.get("env_file")
+    assert isinstance(x, str)
+    assert util.abs_path(x) == result
 
 
-def test_subcommand_property(config_instance):
+def test_subcommand_property(config_instance: config.Config):
     assert config_instance.subcommand == "test"
 
 
-def test_action_property(config_instance):
+def test_action_property(config_instance: config.Config):
     assert config_instance.action is None
 
 
-def test_action_setter(config_instance):
+def test_action_setter(config_instance: config.Config):
     config_instance.action = "foo"
 
     assert config_instance.action == "foo"
 
 
-def test_init_calls_validate(patched_config_validate, config_instance):
+def test_init_calls_validate(patched_config_validate, config_instance: config.Config):
     patched_config_validate.assert_called_once_with()
 
 
-def test_project_directory_property(config_instance):
+def test_project_directory_property(config_instance: config.Config):
     assert os.getcwd() == config_instance.project_directory
 
 
-def test_molecule_directory_property(config_instance):
+def test_molecule_directory_property(config_instance: config.Config):
     x = os.path.join(os.getcwd(), "molecule")
 
     assert x == config_instance.molecule_directory
 
 
-def test_dependency_property(config_instance):
+def test_dependency_property(config_instance: config.Config):
     assert isinstance(config_instance.dependency, ansible_galaxy.AnsibleGalaxy)
 
 
 @pytest.fixture()
 def _config_dependency_shell_section_data():
     return {"dependency": {"name": "shell", "command": "bin/command"}}
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_config_dependency_shell_section_data"],
     indirect=True,
 )
-def test_dependency_property_is_shell(config_instance):
+def test_dependency_property_is_shell(config_instance: config.Config):
     assert isinstance(config_instance.dependency, shell.Shell)
 
 
 @pytest.fixture()
 def _config_driver_delegated_section_data():
-    return {"driver": {"name": "delegated", "options": {"managed": False}}}
+    return {"driver": {"name": "default", "options": {"managed": False}}}
 
 
-def test_env(config_instance):
+def test_env(config_instance: config.Config):
     config_instance.args = {"env_file": ".env"}
+    env_file = config_instance.args.get("env_file")
+    assert isinstance(env_file, str)
     x = {
         "MOLECULE_DEBUG": "False",
         "MOLECULE_FILE": config_instance.config_file,
-        "MOLECULE_ENV_FILE": util.abs_path(config_instance.args.get("env_file")),
+        "MOLECULE_ENV_FILE": util.abs_path(env_file),
         "MOLECULE_INVENTORY_FILE": config_instance.provisioner.inventory_file,
         "MOLECULE_EPHEMERAL_DIRECTORY": config_instance.scenario.ephemeral_directory,
         "MOLECULE_SCENARIO_DIRECTORY": config_instance.scenario.directory,
         "MOLECULE_PROJECT_DIRECTORY": config_instance.project_directory,
         "MOLECULE_INSTANCE_CONFIG": config_instance.driver.instance_config,
         "MOLECULE_DEPENDENCY_NAME": "galaxy",
-        "MOLECULE_DRIVER_NAME": "delegated",
+        "MOLECULE_DRIVER_NAME": "default",
         "MOLECULE_PROVISIONER_NAME": "ansible",
         "MOLECULE_SCENARIO_NAME": "default",
         "MOLECULE_STATE_FILE": config_instance.state.state_file,
         "MOLECULE_VERIFIER_NAME": "ansible",
         "MOLECULE_VERIFIER_TEST_DIRECTORY": config_instance.verifier.directory,
     }
 
     assert x == config_instance.env
 
 
-def test_platforms_property(config_instance):
+def test_platforms_property(config_instance: config.Config):
     assert isinstance(config_instance.platforms, platforms.Platforms)
 
 
-def test_provisioner_property(config_instance):
+def test_provisioner_property(config_instance: config.Config):
     assert isinstance(config_instance.provisioner, ansible.Ansible)
 
 
-def test_scenario_property(config_instance):
+def test_scenario_property(config_instance: config.Config):
     assert isinstance(config_instance.scenario, scenario.Scenario)
 
 
-def test_state_property(config_instance):
+def test_state_property(config_instance: config.Config):
     assert isinstance(config_instance.state, state.State)
 
 
-def test_verifier_property_is_ansible(config_instance):
+def test_verifier_property_is_ansible(config_instance: config.Config):
     assert isinstance(config_instance.verifier, AnsibleVerifier)
 
 
-def test_get_driver_name_from_state_file(config_instance, mocker):
+def test_get_driver_name_from_state_file(config_instance: config.Config, mocker):
     config_instance.state.change_state("driver", "state-driver")
 
     with pytest.raises(SystemExit):
         config_instance._get_driver_name()
 
     mocker.patch("molecule.api.drivers", return_value=["state-driver"])
     assert config_instance._get_driver_name() == "state-driver"
 
 
-def test_get_driver_name_from_cli(config_instance):
+def test_get_driver_name_from_cli(config_instance: config.Config):
     config_instance.command_args = {"driver_name": "cli-driver"}
 
     assert config_instance._get_driver_name() == "cli-driver"
 
 
-def test_get_driver_name(config_instance):
-    assert config_instance._get_driver_name() == "delegated"
+def test_get_driver_name(config_instance: config.Config):
+    assert config_instance._get_driver_name() == "default"
 
 
 def test_get_driver_name_raises_when_different_driver_used(
-    patched_logger_critical,
-    config_instance,
+    caplog: pytest.LogCaptureFixture,
+    config_instance: config.Config,
 ):
     config_instance.state.change_state("driver", "foo")
     config_instance.command_args = {"driver_name": "bar"}
     with pytest.raises(SystemExit) as e:
         config_instance._get_driver_name()
 
     assert e.value.code == 1
 
     msg = (
         "Instance(s) were created with the 'foo' driver, "
         "but the subcommand is using 'bar' driver."
     )
 
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
-def test_get_config(config_instance):
+def test_get_config(config_instance: config.Config):
     assert isinstance(config_instance._get_config(), dict)
 
 
-def test_get_config_with_base_config(config_instance):
+def test_get_config_with_base_config(config_instance: config.Config):
     config_instance.args = {"base_config": ["./foo.yml"]}
     contents = {"foo": "bar"}
     util.write_file(config_instance.args["base_config"][0], util.safe_dump(contents))
     result = config_instance._get_config()
 
     assert result["foo"] == "bar"
 
 
-def test_get_config_with_multiple_base_configs(config_instance):
+def test_get_config_with_multiple_base_configs(config_instance: config.Config):
     config_instance.args = {"base_config": ["./foo.yml", "./foo2.yml"]}
     contents = {"foo": "bar", "foo2": "bar"}
     util.write_file(config_instance.args["base_config"][0], util.safe_dump(contents))
     contents = {"foo2": "bar2"}
     util.write_file(config_instance.args["base_config"][1], util.safe_dump(contents))
     result = config_instance._get_config()
 
     assert result["foo"] == "bar"
     assert result["foo2"] == "bar2"
 
 
-def test_reget_config(config_instance):
+def test_reget_config(config_instance: config.Config):
     assert isinstance(config_instance._reget_config(), dict)
 
 
-def test_interpolate(patched_logger_critical, config_instance):
+def test_interpolate(config_instance: config.Config):
     string = "foo: $HOME"
     x = f"foo: {os.environ['HOME']}"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
-def test_interpolate_curly(patched_logger_critical, config_instance):
+def test_interpolate_curly(config_instance: config.Config):
     string = "foo: ${HOME}"
     x = f"foo: {os.environ['HOME']}"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
-def test_interpolate_default(patched_logger_critical, config_instance):
+def test_interpolate_default(config_instance: config.Config):
     string = "foo: ${NONE-default}"
     x = "foo: default"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
-def test_interpolate_default_colon(patched_logger_critical, config_instance):
+def test_interpolate_default_colon(config_instance: config.Config):
     string = "foo: ${NONE:-default}"
     x = "foo: default"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
-def test_interpolate_default_variable(patched_logger_critical, config_instance):
+def test_interpolate_default_variable(config_instance: config.Config):
     string = "foo: ${NONE:-$HOME}"
     x = f"foo: {os.environ['HOME']}"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
-def test_interpolate_curly_default_variable(patched_logger_critical, config_instance):
+def test_interpolate_curly_default_variable(config_instance: config.Config):
     string = "foo: ${NONE-$HOME}"
     x = f"foo: {os.environ['HOME']}"
 
-    assert x == config_instance._interpolate(string, os.environ, None)
+    assert x == config_instance._interpolate(string, os.environ, "")
 
 
 def test_interpolate_raises_on_failed_interpolation(
-    patched_logger_critical,
-    config_instance,
+    caplog: pytest.LogCaptureFixture,
+    config_instance: config.Config,
 ):
     string = "$6$8I5Cfmpr$kGZB"
 
     with pytest.raises(SystemExit) as e:
-        config_instance._interpolate(string, os.environ, None)
+        config_instance._interpolate(string, os.environ, "")
 
     assert e.value.code == 1
 
     msg = (
         f"parsing config file '{config_instance.molecule_file}'.\n\n"
         "Invalid placeholder in string: line 1, col 1\n"
         "$6$8I5Cfmpr$kGZB"
     )
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
-def test_get_defaults(config_instance, mocker):
+def test_get_defaults(config_instance: config.Config, mocker):
     mocker.patch.object(
         config_instance,
         "molecule_file",
         "/path/to/test_scenario_name/molecule.yml",
     )
     defaults = config_instance._get_defaults()
     assert defaults["scenario"]["name"] == "test_scenario_name"
 
 
-def test_validate(mocker, config_instance, patched_logger_debug):
+def test_validate(
+    mocker: MockerFixture,
+    config_instance: config.Config,
+    patched_logger_debug,
+):
     m = mocker.patch("molecule.model.schema_v3.validate")
     m.return_value = None
 
     config_instance._validate()
 
     assert patched_logger_debug.call_count == 1
 
     m.assert_called_with(config_instance.config)
 
 
 def test_validate_exists_when_validation_fails(
-    mocker,
-    patched_logger_critical,
-    config_instance,
+    mocker: MockerFixture,
+    caplog: pytest.LogCaptureFixture,
+    config_instance: config.Config,
 ):
     m = mocker.patch("molecule.model.schema_v3.validate")
     m.return_value = "validation errors"
 
     with pytest.raises(SystemExit) as e:
         config_instance._validate()
 
     assert e.value.code == 1
 
     msg = f"Failed to validate {config_instance.molecule_file}\n\nvalidation errors"
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_molecule_directory():
     assert config.molecule_directory("/foo/bar") == "/foo/bar/molecule"
 
 
 def test_molecule_file():
     assert config.molecule_file("/foo/bar") == "/foo/bar/molecule.yml"
 
 
-def test_set_env_from_file(config_instance):
+def test_set_env_from_file(config_instance: config.Config):
     config_instance.args = {"env_file": ".env"}
     contents = {"foo": "bar", "BAZ": "zzyzx"}
     env_file = config_instance.args.get("env_file")
+    assert isinstance(env_file, str)
     util.write_file(env_file, util.safe_dump(contents))
     env = config.set_env_from_file({}, env_file)
 
     assert contents == env
 
 
 def test_set_env_from_file_returns_original_env_when_env_file_not_found(
-    config_instance,
+    config_instance: config.Config,
 ):
     env = config.set_env_from_file({}, "file-not-found")
 
     assert {} == env
 
 
-def test_write_config(config_instance):
+def test_write_config(config_instance: config.Config):
     config_instance.write()
 
     assert os.path.isfile(config_instance.config_file)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_interpolation.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 def test_interpolate_with_molecule_yaml(_instance):
     data = """
 ---
 dependency:
     name: $DEPENDENCY_NAME
 driver:
-    name: delegated
+    name: default
 platforms:
   - name: instance-1
 provisioner:
     name: ansible
 verifier:
     name: ${VERIFIER_NAME}
     options:
@@ -112,15 +112,15 @@
 """.strip()
 
     x = """
 ---
 dependency:
     name: galaxy
 driver:
-    name: delegated
+    name: default
 platforms:
   - name: instance-1
 provisioner:
     name: ansible
 verifier:
     name: ansible
     options:
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_logger.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 #  DEALINGS IN THE SOFTWARE.
 
 
 import logging
 
 import pytest
 
+from molecule import config
 from molecule.command.base import Base
 from molecule.console import should_do_markup
 from molecule.logger import get_section_loggers
 
 
 # the dummy/instance fixtures are based on fixtures in test.unit.command.test_base
 class Dummy(Base):
     """ExtendedBase Class."""
 
     def execute(self, action_args=None):
         return True
 
 
 @pytest.fixture()
-def _dummy_class(patched_config_validate, config_instance):
+def _dummy_class(patched_config_validate, config_instance: config.Config):
     return Dummy
 
 
 @pytest.fixture()
 def _instance(_dummy_class, config_instance, _patched_logger_env):
     # _patched_logger_env included here to ensure pytest runs it first
     get_section_loggers.cache_clear()
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_platforms.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_platforms.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
-from molecule import platforms
+from molecule import config, platforms
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     return platforms.Platforms(config_instance)
 
 
 def test_instances_property(_instance):
     x = [
         {"groups": ["foo", "bar"], "name": "instance-1", "children": ["child1"]},
         {"groups": ["baz", "foo"], "name": "instance-2", "children": ["child2"]},
     ]
 
     assert x == _instance.instances
 
 
 @pytest.fixture()
-def platform_name(request, config_instance):
+def platform_name(request, config_instance: config.Config):
     return platforms.Platforms(config_instance, platform_name=request.param)
 
 
 @pytest.mark.parametrize("platform_name", ["instance-1"], indirect=True)
 def test_instances_property_with_platform_name_instance_1(platform_name):
     x = [
         {"groups": ["foo", "bar"], "name": "instance-1", "children": ["child1"]},
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_scenario.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from molecule import config, scenario, util
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(patched_config_validate, config_instance):
+def _instance(patched_config_validate, config_instance: config.Config):
     return scenario.Scenario(config_instance)
 
 
 def test_prune(_instance):
     e_dir = _instance.ephemeral_directory
     # prune data also includes files in the scenario inventory dir,
     # which is "<e_dir>/inventory" by default.
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_scenarios.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from molecule import config, scenario, scenarios
 from molecule.console import console
 from molecule.text import chomp, strip_ansi_escape
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     config_instance_1 = copy.deepcopy(config_instance)
 
     config_instance_2 = copy.deepcopy(config_instance)
     config_instance_2.config["scenario"]["name"] = "foo"
 
     return scenarios.Scenarios([config_instance_1, config_instance_2])
 
@@ -111,23 +111,23 @@
 
 def test_verify_does_not_raise_when_found(_instance):
     _instance._scenario_name = "default"
 
     assert _instance._verify() is None
 
 
-def test_verify_raises_when_scenario_not_found(_instance, patched_logger_critical):
+def test_verify_raises_when_scenario_not_found(_instance, caplog):
     _instance._scenario_name = "invalid"
     with pytest.raises(SystemExit) as e:
         _instance._verify()
 
     assert e.value.code == 1
 
     msg = "Scenario 'invalid' not found.  Exiting."
-    patched_logger_critical.assert_called_once_with(msg)
+    assert msg in caplog.text
 
 
 def test_filter_for_scenario(_instance):
     _instance._scenario_name = "default"
     result = _instance._filter_for_scenario()
     assert len(result) == 1
     assert result[0].name == "default"
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_scenarios_ordered.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios_ordered.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import copy
 
 import pytest
 
-from molecule import scenarios
+from molecule import config, scenarios
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     config_instance_1 = copy.deepcopy(config_instance)
     config_instance_1.config["scenario"]["name"] = "two"
     config_instance_1.molecule_file = config_instance_1.molecule_file.replace(
         "default",
         "02_foo",
     )
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_state.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 
 import pytest
 
-from molecule import state, util
+from molecule import config, state, util
 
 
 @pytest.fixture()
-def _instance(config_instance):
+def _instance(config_instance: config.Config):
     return state.State(config_instance)
 
 
 def test_state_file_property(_instance):
     x = os.path.join(_instance._config.scenario.ephemeral_directory, "state.yml")
 
     assert x == _instance.state_file
@@ -100,15 +100,19 @@
 
 
 def test_change_state_raises(_instance):
     with pytest.raises(state.InvalidState):
         _instance.change_state("invalid-state", True)
 
 
-def test_get_data_loads_existing_state_file(_instance, molecule_data, config_instance):
+def test_get_data_loads_existing_state_file(
+    _instance,
+    molecule_data,
+    config_instance: config.Config,
+):
     data = {"converged": False, "created": True, "driver": None, "prepared": None}
     util.write_file(_instance._state_file, util.safe_dump(data))
 
     s = state.State(config_instance)
 
     assert not s.converged
     assert s.created
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_status.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_status.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_text.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_text.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/test/unit/test_util.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/test_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 
 import binascii
-import io
 import os
 import warnings
 from pathlib import Path
+from typing import Any
 
 import pytest
+from pytest_mock import MockerFixture
 
 from molecule import util
 from molecule.api import IncompatibleMoleculeRuntimeWarning, MoleculeRuntimeWarning
 from molecule.console import console
 from molecule.constants import MOLECULE_HEADER
 from molecule.test.conftest import get_molecule_file, molecule_directory
 from molecule.text import strip_ansi_escape
@@ -40,15 +41,15 @@
     with console.capture() as capture:
         util.print_debug("test_title", "test_data")
 
     result = strip_ansi_escape(capture.get())
     assert result == expected
 
 
-def test_print_environment_vars(capsys):
+def test_print_environment_vars(capsys: pytest.CaptureFixture[str]) -> None:
     env = {
         "ANSIBLE_FOO": "foo",
         "ANSIBLE_BAR": "bar",
         "ANSIBLE": None,
         "MOLECULE_FOO": "foo",
         "MOLECULE_BAR": "bar",
         "MOLECULE": None,
@@ -81,87 +82,90 @@
 def test_sysexit_with_custom_code():
     with pytest.raises(SystemExit) as e:
         util.sysexit(2)
 
     assert e.value.code == 2
 
 
-def test_sysexit_with_message(patched_logger_critical):
+def test_sysexit_with_message(caplog: pytest.LogCaptureFixture):
     with pytest.raises(SystemExit) as e:
         util.sysexit_with_message("foo")
 
     assert e.value.code == 1
 
-    patched_logger_critical.assert_called_once_with("foo")
+    assert "foo" in caplog.text
 
 
-def test_sysexit_with_warns(patched_logger_critical, patched_logger_warning):
+def test_sysexit_with_warns(caplog: pytest.LogCaptureFixture):
     with pytest.raises(SystemExit) as e:
         with warnings.catch_warnings(record=True) as warns:
             warnings.filterwarnings("default", category=MoleculeRuntimeWarning)
             warnings.warn("xxx", category=IncompatibleMoleculeRuntimeWarning)
 
         util.sysexit_with_message("foo", warns=warns)
 
     assert e.value.code == 1
 
-    patched_logger_critical.assert_called_once_with("foo")
-    patched_logger_warning.assert_called_once_with("xxx")
+    assert "foo" in caplog.text
+    assert "xxx" in caplog.text
 
 
-def test_sysexit_with_message_and_custom_code(patched_logger_critical):
+def test_sysexit_with_message_and_custom_code(caplog: pytest.LogCaptureFixture):
     with pytest.raises(SystemExit) as e:
         util.sysexit_with_message("foo", 2)
 
     assert e.value.code == 2
 
-    patched_logger_critical.assert_called_once_with("foo")
+    assert "foo" in caplog.text
 
 
 def test_run_command():
     cmd = ["ls"]
     x = util.run_command(cmd)
 
     assert x.returncode == 0
 
 
-def test_run_command_with_debug(mocker, patched_print_debug):
+def test_run_command_with_debug(mocker: MockerFixture, patched_print_debug):
     env = {"ANSIBLE_FOO": "foo", "MOLECULE_BAR": "bar"}
     util.run_command(["ls"], debug=True, env=env)
     x = [
         mocker.call("ANSIBLE ENVIRONMENT", "ANSIBLE_FOO: foo\n"),
         mocker.call("MOLECULE ENVIRONMENT", "MOLECULE_BAR: bar\n"),
         mocker.call("SHELL REPLAY", "ANSIBLE_FOO=foo MOLECULE_BAR=bar"),
     ]
 
     assert x == patched_print_debug.mock_calls
 
 
 def test_run_command_baked_cmd_env():
-    cmd = util.BakedCommand(cmd=["printenv", "myvar"], env={"myvar": "myvalue"})
-    result = util.run_command(cmd, env={"myvar2": "value2"})
+    cmd = ["printenv", "myvar"]
+    result = util.run_command(cmd, env={"myvar": "value2"})
     assert result.returncode == 0
 
-    cmd = util.BakedCommand(cmd=["printenv", "myvar2"], env={"myvar": "myvalue"})
+    cmd = ["printenv", "myvar2"]
     result = util.run_command(cmd, env={"myvar2": "value2"})
     assert result.returncode == 0
 
     # negative test
-    cmd = util.BakedCommand(cmd=["printenv", "myvar"], env={})
+    cmd = ["printenv", "myvar"]
     result = util.run_command(cmd)
     assert result.returncode == 1
 
 
-def test_run_command_with_debug_handles_no_env(mocker, patched_print_debug):
-    cmd = "ls"
+def test_run_command_with_debug_handles_no_env(
+    mocker: MockerFixture,
+    patched_print_debug,
+):
+    cmd = ["ls"]
     util.run_command(cmd, debug=True)
     # when env is empty we expect not to print anything
-    x = []
+    empty_list: list[Any] = []
 
-    assert x == patched_print_debug.mock_calls
+    assert empty_list == patched_print_debug.mock_calls
 
 
 def test_os_walk(temp_dir):
     scenarios = ["scenario1", "scenario2", "scenario3"]
     mol_dir = molecule_directory()
     for scenario in scenarios:
         scenario_directory = os.path.join(mol_dir, scenario)
@@ -187,15 +191,15 @@
     assert util.render_template(template) == 'url = "quoted_str"'
 
 
 def test_write_file(temp_dir):
     dest_file = os.path.join(temp_dir.strpath, "test_util_write_file.tmp")
     contents = binascii.b2a_hex(os.urandom(15)).decode("utf-8")
     util.write_file(dest_file, contents)
-    with util.open_file(dest_file) as stream:
+    with open(dest_file) as stream:
         data = stream.read()
     x = f"# Molecule managed\n\n{contents}"
 
     assert x == data
 
 
 def test_molecule_prepender(tmp_path: Path) -> None:
@@ -223,104 +227,91 @@
 foo:
   - baz: zzyzx
     foo: bar
 """.lstrip()
     assert x == util.safe_dump(data)
 
 
-def test_safe_load():
+def test_safe_load() -> None:
     assert {"foo": "bar"} == util.safe_load("foo: bar")
 
 
-def test_safe_load_returns_empty_dict_on_empty_string():
+def test_safe_load_returns_empty_dict_on_empty_string() -> None:
     assert {} == util.safe_load("")
 
 
-def test_safe_load_exits_when_cannot_parse():
+def test_safe_load_exits_when_cannot_parse() -> None:
     data = """
 ---
 %foo:
 """.strip()
 
     with pytest.raises(SystemExit) as e:
         util.safe_load(data)
 
     assert e.value.code == 1
 
 
-def test_safe_load_file(temp_dir):
+def test_safe_load_file(temp_dir) -> None:
     path = os.path.join(temp_dir.strpath, "foo")
     util.write_file(path, "foo: bar")
 
     assert {"foo": "bar"} == util.safe_load_file(path)
 
 
-def test_open_file(temp_dir):
-    path = os.path.join(temp_dir.strpath, "foo")
-    util.write_file(path, "foo: bar")
-
-    with util.open_file(path) as stream:
-        try:
-            file_types = (file, io.IOBase)
-        except NameError:
-            file_types = io.IOBase
-
-        assert isinstance(stream, file_types)
-
-
-def test_instance_with_scenario_name():
+def test_instance_with_scenario_name() -> None:
     assert util.instance_with_scenario_name("foo", "bar") == "foo-bar"
 
 
-def test_verbose_flag():
+def test_verbose_flag() -> None:
     options = {"verbose": True, "v": True}
 
     assert ["-v"] == util.verbose_flag(options)
     # pylint: disable=use-implicit-booleaness-not-comparison
     assert {} == options
 
 
-def test_verbose_flag_extra_verbose():
+def test_verbose_flag_extra_verbose() -> None:
     options = {"verbose": True, "vvv": True}
 
     assert ["-vvv"] == util.verbose_flag(options)
     # pylint: disable=use-implicit-booleaness-not-comparison
     assert {} == options
 
 
-def test_verbose_flag_preserves_verbose_option():
+def test_verbose_flag_preserves_verbose_option() -> None:
     options = {"verbose": True}
 
     # pylint: disable=use-implicit-booleaness-not-comparison
     assert [] == util.verbose_flag(options)
     assert {"verbose": True} == options
 
 
-def test_filter_verbose_permutation():
+def test_filter_verbose_permutation() -> None:
     options = {
         "v": True,
         "vv": True,
         "vvv": True,
         "vfoo": True,
         "foo": True,
         "bar": True,
     }
 
     x = {"vfoo": True, "foo": True, "bar": True}
     assert x == util.filter_verbose_permutation(options)
 
 
-def test_abs_path(temp_dir):
+def test_abs_path(temp_dir) -> None:
     x = os.path.abspath(os.path.join(os.getcwd(), os.path.pardir, "foo", "bar"))
 
     assert x == util.abs_path(os.path.join(os.path.pardir, "foo", "bar"))
 
 
-def test_abs_path_with_none_path():
-    assert util.abs_path(None) is None
+def test_abs_path_with_none_path() -> None:
+    assert util.abs_path(None) is None  # type: ignore
 
 
 # pylint: disable=use-dict-literal
 @pytest.mark.parametrize(
     ("a", "b", "x"),
     [
         # Base of recursion scenarios
@@ -334,9 +325,9 @@
         (
             {"b": [{"c": 0}, {"c": 2}], "d": {"e": "aaa", "f": 3}},
             {"a": 1, "b": [{"c": 3}], "d": {"e": "bbb"}},
             {"a": 1, "b": [{"c": 3}], "d": {"e": "bbb", "f": 3}},
         ),
     ],
 )
-def test_merge_dicts(a, b, x):
+def test_merge_dicts(a, b, x) -> None:
     assert x == util.merge_dicts(a, b)
```

### Comparing `molecule-5.1.0/src/molecule/test/unit/verifier/test_ansible.py` & `molecule-6.0.0a0/src/molecule/test/a_unit/verifier/test_ansible.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,19 @@
     return {"verifier": {"name": "ansible", "env": {"FOO": "bar"}}}
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.fixture()
-def _instance(_verifier_section_data, patched_config_validate, config_instance):
+def _instance(
+    _verifier_section_data,
+    patched_config_validate,
+    config_instance: config.Config,
+):
     return ansible.Ansible(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
@@ -72,31 +76,31 @@
 def test_options_property_handles_cli_args(_instance):
     _instance._config.args = {"debug": True}
     x = {}
 
     assert x == _instance.options
 
 
-def test_execute(patched_logger_info, _patched_ansible_verify, _instance):
+def test_execute(caplog, _patched_ansible_verify, _instance):
     _instance.execute()
 
     _patched_ansible_verify.assert_called_once_with(None)
 
     msg = "Running Ansible Verifier"
-    patched_logger_info.assert_any_call(msg)
+    assert msg in caplog.text
 
     msg = "Verifier completed successfully."
-    patched_logger_info.assert_any_call(msg)
+    assert msg in caplog.text
 
 
 def test_execute_does_not_execute(
     patched_ansible_converge,
-    patched_logger_warning,
+    caplog: pytest.LogCaptureFixture,
     _instance,
 ):
     _instance._config.config["verifier"]["enabled"] = False
     _instance.execute()
 
     assert not patched_ansible_converge.called
 
     msg = "Skipping, verifier is disabled."
-    patched_logger_warning.assert_called_once_with(msg)
+    assert msg in caplog.text
```

### Comparing `molecule-5.1.0/src/molecule/text.py` & `molecule-6.0.0a0/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/util.py` & `molecule-6.0.0a0/src/molecule/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 """Molecule Utils Module."""
 
 
-import contextlib
 import copy
 import fnmatch
 import logging
 import os
 import re
 import sys
 from collections.abc import Iterable, MutableMapping
-from dataclasses import dataclass
 from subprocess import CalledProcessError, CompletedProcess
-from typing import Any, NoReturn, Optional, Union
+from typing import Any, NoReturn, Optional
 from warnings import WarningMessage
 
 import jinja2
 import yaml
 from ansible_compat.ports import cache
 from rich.syntax import Syntax
 
@@ -52,15 +50,15 @@
 
 
 def print_debug(title: str, data: str) -> None:
     """Print debug information."""
     console.print(f"DEBUG: {title}:\n{data}")
 
 
-def print_environment_vars(env: Optional[dict[str, str]]) -> None:
+def print_environment_vars(env: Optional[dict[str, Optional[str]]]) -> None:
     """Print ``Ansible`` and ``Molecule`` environment variables and returns None.
 
     :param env: A dict containing the shell's environment as collected by
     ``os.environ``.
     :return: None
     """
     if env:
@@ -104,48 +102,37 @@
 ) -> None:
     """Exit with an error message."""
     # detail is usually a multi-line string which is not suitable for normal
     # logger.
     if detail:
         detail_str = safe_dump(detail) if isinstance(detail, dict) else str(detail)
         print(detail_str)
-    LOG.critical(msg)
+    LOG.critical(msg, extra={"highlighter": False})
 
     for warn in warns:
         LOG.warning(warn.__dict__["message"].args[0])
     sysexit(code)
 
 
 def run_command(
-    cmd,
+    cmd: list[str],
     env=None,
     debug=False,
     echo=False,
     quiet=False,
     check=False,
     cwd=None,
 ) -> CompletedProcess:
     """Execute the given command and returns None.
 
     :param cmd: :
         - a string or list of strings (similar to subprocess.run)
-        - a BakedCommand object (
     :param debug: An optional bool to toggle debug output.
     """
-    args = []
-    if cmd.__class__.__name__ == "Command":
-        raise RuntimeError(
-            "Molecule 3.2.0 dropped use of sh library, update plugin code to use new API. "
-            "See https://github.com/ansible-community/molecule/issues/2678",
-        )
-    if cmd.__class__.__name__ == "BakedCommand":
-        env = dict(cmd.env, **env) if cmd.env and env else cmd.env or env
-        args = cmd.cmd
-    else:
-        args = cmd
+    args = cmd
 
     if debug:
         print_environment_vars(env)
 
     result = app.runtime.run(
         args=args,
         env=env,
@@ -193,15 +180,15 @@
     :param content: A string containing the data to be written.
     :param header: A header, if None it will use default header.
     :return: None
     """
     if header is None:
         content = MOLECULE_HEADER + "\n\n" + content
 
-    with open_file(filename, "w") as f:
+    with open(filename, "w") as f:
         f.write(content)
 
 
 def molecule_prepender(content: str) -> str:
     """Return molecule identification header."""
     return MOLECULE_HEADER + "\n\n" + content
 
@@ -209,15 +196,15 @@
 def file_prepender(filename: str) -> None:
     """Prepend an informational header on files managed by Molecule and returns \
     None.
 
     :param filename: A string containing the target filename.
     :return: None
     """
-    with open_file(filename, "r+") as f:
+    with open(filename, "r+") as f:
         content = f.read()
         f.seek(0, 0)
         f.write(molecule_prepender(content))
 
 
 def safe_dump(data: Any, explicit_start=True) -> str:
     """Dump the provided data to a YAML document and returns a string.
@@ -248,30 +235,18 @@
 
 def safe_load_file(filename: str):
     """Parse the provided YAML file and returns a dict.
 
     :param filename: A string containing an absolute path to the file to parse.
     :return: dict
     """
-    with open_file(filename) as stream:
+    with open(filename) as stream:
         return safe_load(stream)
 
 
-@contextlib.contextmanager
-def open_file(filename, mode="r"):
-    """Open the provide file safely and returns a file type.
-
-    :param filename: A string containing an absolute path to the file to open.
-    :param mode: A string describing the way in which the file will be used.
-    :return: file type
-    """
-    with open(filename, mode) as stream:
-        yield stream
-
-
 def instance_with_scenario_name(instance_name, scenario_name):
     """Format instance name that includes scenario."""
     return f"{instance_name}-{scenario_name}"
 
 
 def verbose_flag(options):
     """Return computed verbosity flag."""
@@ -388,25 +363,14 @@
         return False
 
     raise TypeError(
         f"The value '{value!s}' is not a valid boolean.  Valid booleans include: {', '.join(repr(i) for i in BOOLEANS)!s}",
     )
 
 
-@dataclass
-class BakedCommand:
-    """Define a subprocess command to be executed."""
-
-    cmd: Union[str, list[str]]
-    env: Optional[dict]
-    cwd: Optional[str] = None
-    stdout: Any = None
-    stderr: Any = None
-
-
 def dict2args(data: dict) -> list[str]:
     """Convert a dictionary of options to command like arguments."""
     result = []
     # keep sorting in order to achieve a predictable behavior
     for k, v in sorted(data.items()):
         if v is not False:
             prefix = "-" if len(k) == 1 else "--"
```

### Comparing `molecule-5.1.0/src/molecule/verifier/ansible.py` & `molecule-6.0.0a0/src/molecule/verifier/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/src/molecule/verifier/base.py` & `molecule-6.0.0a0/src/molecule/verifier/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Verifier Base Module."""
 
 import abc
 import os
 
-import molecule
 from molecule import util
 
 
 class Verifier:
     """Verifier Base Class."""
 
     __metaclass__ = abc.ABCMeta
@@ -117,19 +116,7 @@
     def __str__(self) -> str:
         """Return readable string representation of object."""
         return self.name
 
     def __repr__(self) -> str:
         """Return detailed string representation of object."""
         return self.name
-
-    def template_dir(self):
-        p = os.path.abspath(
-            os.path.join(
-                os.path.dirname(molecule.__file__),
-                "cookiecutter",
-                "scenario",
-                "verifier",
-                self.name,
-            ),
-        )
-        return p
```

### Comparing `molecule-5.1.0/src/molecule.egg-info/PKG-INFO` & `molecule-6.0.0a0/src/molecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.1.0
+Version: 6.0.0a0
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-5.1.0/src/molecule.egg-info/requires.txt` & `molecule-6.0.0a0/src/molecule.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ansible-compat>=4.1.2
 ansible-core>=2.12.10
 click<9,>=8.0
 click-help-colors>=0.9
-cookiecutter>=1.7.3
 enrich>=1.2.7
 jsonschema>=4.9.1
 Jinja2>=2.11.3
 packaging
 pluggy<2.0,>=0.7.1
 PyYAML>=5.1
 rich>=9.5.1
@@ -14,55 +13,44 @@
 [docs]
 mkdocs-ansible[lock]>=0.1.4
 pipdeptree>=2.4.0
 linkchecker
 
 [lock]
 ansible-compat==4.1.2
-ansible-core==2.14.4
-arrow==1.2.3
+ansible-core==2.15.1
 attrs==23.1.0
-binaryornot==0.4.4
-certifi==2022.12.7
 cffi==1.15.1
-chardet==5.1.0
-charset-normalizer==3.1.0
-click==8.1.3
+click==8.1.4
 click-help-colors==0.9.1
-cookiecutter==2.1.1
-cryptography==41.0.0
+cryptography==41.0.1
 enrich==1.2.7
-idna==3.4
+importlib-resources==5.0.7
 jinja2==3.1.2
-jinja2-time==0.2.0
-jsonschema==4.17.3
-markdown-it-py==2.2.0
-markupsafe==2.1.2
+jsonschema==4.18.0
+jsonschema-specifications==2023.6.1
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 mdurl==0.1.2
 packaging==23.1
-pluggy==1.0.0
+pluggy==1.2.0
 pycparser==2.21
 pygments==2.15.1
-pyrsistent==0.19.3
-python-dateutil==2.8.2
-python-slugify==8.0.1
 pyyaml==6.0
-requests==2.31.0
-resolvelib==0.8.1
-rich==13.3.4
-six==1.16.0
+referencing==0.29.1
+resolvelib==1.0.1
+rich==13.4.2
+rpds-py==0.8.10
 subprocess-tee==0.4.1
-text-unidecode==1.3
-urllib3==1.26.15
+typing-extensions==4.7.1
 
 [test]
 ansible-lint>=6.12.1
 ansi2html>=1.8.0
 coverage>=7.0.3
 filelock>=3.9.0
 pexpect<5,>=4.8.0
 pytest-mock>=3.10.0
 pytest-plus>=0.4.0
-pytest-testinfra>=7.0.0
 pytest-xdist>=3.1.0
 pytest>=7.2.0
 check-jsonschema
```

### Comparing `molecule-5.1.0/tools/test-setup.sh` & `molecule-6.0.0a0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-5.1.0/tox.ini` & `molecule-6.0.0a0/tox.ini`

 * *Files identical despite different names*

