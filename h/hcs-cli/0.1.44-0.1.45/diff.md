# Comparing `tmp/hcs-cli-0.1.44.tar.gz` & `tmp/hcs-cli-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.44.tar", last modified: Tue Jul 11 08:49:07 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.45.tar", last modified: Wed Jul 12 01:23:09 2023, max compression
```

## Comparing `hcs-cli-0.1.44.tar` & `hcs-cli-0.1.45.tar`

### file list

```diff
@@ -1,288 +1,294 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.326897 hcs-cli-0.1.44/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.44/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.032033 hcs-cli-0.1.44/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2552 2023-07-11 08:44:46.000000 hcs-cli-0.1.44/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.44/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.44/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.44/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.44/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.44/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:49:07.325355 hcs-cli-0.1.44/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.44/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.040411 hcs-cli-0.1.44/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.44/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.44/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.44/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.44/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     2984 2023-07-11 07:26:34.000000 hcs-cli-0.1.44/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.045237 hcs-cli-0.1.44/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     6687 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:06.971597 hcs-cli-0.1.44/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.046337 hcs-cli-0.1.44/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.44/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.44/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.44/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-11 08:49:07.327459 hcs-cli-0.1.44/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 08:46:55.000000 hcs-cli-0.1.44/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.048289 hcs-cli-0.1.44/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.44/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.049528 hcs-cli-0.1.44/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.050659 hcs-cli-0.1.44/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.056552 hcs-cli-0.1.44/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.059623 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.062137 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.064769 hcs-cli-0.1.44/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.44/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.068410 hcs-cli-0.1.44/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.072290 hcs-cli-0.1.44/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.073408 hcs-cli-0.1.44/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.074446 hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.078529 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.080959 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.085839 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.090368 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.091476 hcs-cli-0.1.44/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.093642 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.094732 hcs-cli-0.1.44/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.099094 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     2272 2023-07-07 17:19:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/plan.py
--rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/validate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.102834 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     4917 2023-07-07 17:46:45.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.106401 hcs-cli-0.1.44/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.112104 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.113301 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.119489 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.130802 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.44/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:06.986245 hcs-cli-0.1.44/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.134175 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.137877 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.148221 hcs-cli-0.1.44/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.159370 hcs-cli-0.1.44/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1911 2023-07-11 08:31:05.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1699 2023-07-11 08:31:16.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/destroy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.162689 hcs-cli-0.1.44/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.171748 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      976 2023-07-11 08:42:49.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.179510 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.183674 hcs-cli-0.1.44/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.44/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.185166 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.190207 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.44/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.195442 hcs-cli-0.1.44/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.213706 hcs-cli-0.1.44/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.44/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.44/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.44/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.217753 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.44/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.44/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.44/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.44/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.44/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.44/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.44/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.44/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.44/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.44/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.228906 hcs-cli-0.1.44/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.44/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.44/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.44/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.44/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.44/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.44/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.44/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.232121 hcs-cli-0.1.44/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.44/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.238954 hcs-cli-0.1.44/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.44/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    13210 2023-07-11 08:32:49.000000 hcs-cli-0.1.44/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     4754 2023-07-11 00:52:21.000000 hcs-cli-0.1.44/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.44/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.240843 hcs-cli-0.1.44/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.44/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.250881 hcs-cli-0.1.44/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4432 2023-07-11 02:03:42.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1181 2023-07-11 01:23:30.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 01:23:47.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-07-11 01:23:57.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.255704 hcs-cli-0.1.44/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.263432 hcs-cli-0.1.44/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1027 2023-07-11 06:48:15.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1212 2023-07-11 01:24:36.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.268516 hcs-cli-0.1.44/vhcs/plan/provider/runtime/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     3396 2023-07-11 07:11:55.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/daas_tenant_calculation.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.270896 hcs-cli-0.1.44/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.278195 hcs-cli-0.1.44/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.44/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.44/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.44/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.44/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.44/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.44/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.280697 hcs-cli-0.1.44/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.44/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.44/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.285477 hcs-cli-0.1.44/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.288672 hcs-cli-0.1.44/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.44/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.44/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.292171 hcs-cli-0.1.44/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.44/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.44/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.44/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.295575 hcs-cli-0.1.44/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.44/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.44/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.44/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.297745 hcs-cli-0.1.44/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.44/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.44/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.300968 hcs-cli-0.1.44/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-07-11 03:25:14.000000 hcs-cli-0.1.44/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.44/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1236 2023-07-10 08:19:02.000000 hcs-cli-0.1.44/vhcs/service/portal/pool.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.303477 hcs-cli-0.1.44/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.44/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.44/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.305732 hcs-cli-0.1.44/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.44/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.311116 hcs-cli-0.1.44/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.44/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.44/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.44/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.44/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.008191 hcs-cli-0.1.44/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.316880 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-07-11 08:43:59.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.44/vhcs/support/daas/tenant.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.44/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.323999 hcs-cli-0.1.44/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.44/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.314222 hcs-cli-0.1.45/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.45/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.964324 hcs-cli-0.1.45/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2575 2023-07-11 22:53:30.000000 hcs-cli-0.1.45/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.45/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.45/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.45/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.45/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.45/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-12 01:23:09.313390 hcs-cli-0.1.45/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.45/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.973062 hcs-cli-0.1.45/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.45/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.45/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.45/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.45/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     3763 2023-07-11 20:40:34.000000 hcs-cli-0.1.45/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.981198 hcs-cli-0.1.45/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     6841 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.905978 hcs-cli-0.1.45/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.983219 hcs-cli-0.1.45/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.45/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.45/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.45/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-12 01:23:09.314554 hcs-cli-0.1.45/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-12 01:23:03.000000 hcs-cli-0.1.45/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.987826 hcs-cli-0.1.45/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.45/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.989835 hcs-cli-0.1.45/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.991711 hcs-cli-0.1.45/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.998246 hcs-cli-0.1.45/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.000978 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.003989 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.006774 hcs-cli-0.1.45/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.45/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.010230 hcs-cli-0.1.45/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.014609 hcs-cli-0.1.45/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.016288 hcs-cli-0.1.45/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.018703 hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.025652 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.028763 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.035232 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.040531 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.042573 hcs-cli-0.1.45/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.046452 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.047780 hcs-cli-0.1.45/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.052883 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2571 2023-07-11 23:45:56.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.059865 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4978 2023-07-12 00:02:14.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.068731 hcs-cli-0.1.45/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.075804 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.078752 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.106282 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.137168 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.45/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.921392 hcs-cli-0.1.45/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.139319 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.141544 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.148062 hcs-cli-0.1.45/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.152243 hcs-cli-0.1.45/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1777 2023-07-11 20:14:16.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-11 20:14:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1660 2023-07-11 23:15:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.154025 hcs-cli-0.1.45/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.158555 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-11 20:54:29.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.164345 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-11 20:55:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.169662 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 20:56:15.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-11 20:56:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      948 2023-07-11 20:56:50.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-11 20:56:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.171948 hcs-cli-0.1.45/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.45/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.173031 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.176356 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.45/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.181233 hcs-cli-0.1.45/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.200313 hcs-cli-0.1.45/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.45/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.45/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.45/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.204096 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.45/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.45/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.45/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.45/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.45/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.45/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.45/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.45/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.45/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.45/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.211971 hcs-cli-0.1.45/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.45/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.45/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.45/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.45/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.45/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.45/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.45/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.214942 hcs-cli-0.1.45/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.45/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.221082 hcs-cli-0.1.45/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       74 2023-07-11 20:07:10.000000 hcs-cli-0.1.45/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14123 2023-07-12 01:16:46.000000 hcs-cli-0.1.45/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6729 2023-07-11 20:34:43.000000 hcs-cli-0.1.45/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.45/vhcs/plan/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.222776 hcs-cli-0.1.45/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.45/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.234079 hcs-cli-0.1.45/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4831 2023-07-12 00:07:32.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-11 21:11:11.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 21:13:28.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1259 2023-07-12 00:09:22.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.237646 hcs-cli-0.1.45/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.246338 hcs-cli-0.1.45/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-11 08:52:37.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1227 2023-07-12 00:45:19.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-11 21:01:33.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.248657 hcs-cli-0.1.45/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.255410 hcs-cli-0.1.45/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.45/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.45/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.45/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.45/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.45/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.45/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.258001 hcs-cli-0.1.45/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.45/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.45/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.264172 hcs-cli-0.1.45/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.266484 hcs-cli-0.1.45/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.45/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.45/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.270067 hcs-cli-0.1.45/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.45/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.45/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.45/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.273806 hcs-cli-0.1.45/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.45/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.45/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.45/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.276046 hcs-cli-0.1.45/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.45/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.45/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.280580 hcs-cli-0.1.45/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.45/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.45/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-07-11 20:55:47.000000 hcs-cli-0.1.45/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1336 2023-07-11 21:02:10.000000 hcs-cli-0.1.45/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.282783 hcs-cli-0.1.45/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.45/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.45/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.286390 hcs-cli-0.1.45/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.45/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.298156 hcs-cli-0.1.45/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.45/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3580 2023-07-12 00:03:12.000000 hcs-cli-0.1.45/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.45/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1280 2023-07-11 23:26:50.000000 hcs-cli-0.1.45/vhcs/support/daas/infra_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.45/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.944477 hcs-cli-0.1.45/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.305229 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)      394 2023-07-11 23:33:48.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      133 2023-07-11 21:03:36.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3645 2023-07-11 23:24:50.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.45/vhcs/support/daas/tenant.py.xx
+-rw-r--r--   0 nanw       (501) staff       (20)     3401 2023-07-12 00:05:12.000000 hcs-cli-0.1.45/vhcs/support/daas/tenant_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.45/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.45/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.312008 hcs-cli-0.1.45/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.45/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.44/.gitignore` & `hcs-cli-0.1.45/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/.vscode/launch.json` & `hcs-cli-0.1.45/.vscode/launch.json`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,22 @@
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["daas", "tenant", "plan", "nanw",]
         },
         {
-            "name": "hcs profile use",
+            "name": "hcs daas infra plan",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
-            "justMyCode": true,
+            "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["profile", "use"]
+            "args" : ["daas", "infra", "plan", "westus2"]
         },
         {
             "name": "hcs plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
```

### Comparing `hcs-cli-0.1.44/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.45/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.45/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/GOVERNANCE.md` & `hcs-cli-0.1.45/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/LICENSE` & `hcs-cli-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/Makefile` & `hcs-cli-0.1.45/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/PKG-INFO` & `hcs-cli-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.44
+Version: 0.1.45
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.44/README.md` & `hcs-cli-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/doc/az-cheatsheet.md` & `hcs-cli-0.1.45/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/doc/dev-setup.md` & `hcs-cli-0.1.45/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.45/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.45/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/doc/hcs-plan.md` & `hcs-cli-0.1.45/doc/hcs-plan.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # HCS Plan
 
+- [HCS Plan](#hcs-plan)
+  - [File Types](#file-types)
+    - [Blueprint](#blueprint)
+    - [Variable File](#variable-file)
+    - [Plan File](#plan-file)
+    - [State File](#state-file)
+  - [Principles](#principles)
+    - [Provider](#provider)
+  - [Syntax](#syntax)
+    - [Sections Explained](#sections-explained)
+  - [Cheatsheet](#cheatsheet)
+
+
 HCS Plan is the deployment engine to manage HCS resources in a declarative way.
 
 ## File Types
 
 ### Blueprint
 A file that consists of the resources to be deployed, normally with varieties of variables.
 
@@ -21,54 +34,72 @@
 ### Provider
 - Each provider should focus on a single API
 - Resources should represent a single API object
 - Resource and attribute schema should closely match the underlying API
 
 
 ## Syntax
-### Sections
-#### deploymentId
-The unique deployment ID to distinguish one deployment from another. Resources will be tagged based on the deploymentId if possible, and smart refresh should also consider deploymentId to identify related resource, upon missing previous state.
+### Sections Explained
 
-#### vars
-The input of the blueprint. All top-level variables are specified here.
+```yml
+# ------------
+# deploymentId
+# ------------
+# The unique deployment ID to distinguish one deployment 
+# from another. Resources will be tagged based on the deploymentId 
+# if possible, and smart refresh should also consider deploymentId 
+# to identify related resource, upon missing previous state.
+deploymentId: myCustomer1
+
+# ------------
+# vars
+# ------------
+# The vars section is the input of the blueprint. All top-level variables are specified here.
+# 
+vars:
+  provider: 0123
+  userEmails:
+  - a@b.com
+  - c@d.com
 
-#### defaults
-A section to help deduplicate common variables.
 
-#### resources
-The resources to be created. A map from unique resource name to resource definition.
+# ------------------------
+# Custom sections
+# ------------------------
+
+# Custom sections can be defined to manipulate the variables.
+# For example, the common 'defaults' section is used to define
+# shared variable calculation, to avoid duplicated calculation
+# in each resource.
+# Variables are quoted by "${}"
+defaults:
+  name: titan-lite-${deploymentId}
+
+# ------------------------
+# The resources section
+# ------------------------
+# The resources to be created. A map from unique resource 
+# name to resource definition.
 
-### Repeated Items
-Example:
-```
-vars:
-  tenantId: <the-tenant-id>
-  userEmails:
-  - u1@mydomain.com
-  - u2@mydomain.com
 resources:
   myAADGroup:
     kind: azure/aad-group
     data:
         tenant: ${vars.tenantId}
   myAADUsers:
     kind: azure/aad-user
     for: email in vars.userEmails
     data:
       group: ${myAADGroup.id}
-```
-
-In azure/aad-user resource handler, the received data object will have 'email' added, as declared in the 'for' statement:
-```
-    {
-        'group': '<group-id>'
-        'email': '<one-of-the-emails>
-    }
-```
+# In azure/aad-user resource handler, the received data object
+# will have 'email' added, as declared in the 'for' statement:
+#    {
+#        'group': '<group-id>'
+#        'email': '<one-of-the-emails>
+#    }
 
 ### Map list to a new list
 ```
 vars:
   tenantId: <the-tenant-id>
   userEmails:
   - u1@mydomain.com
```

### Comparing `hcs-cli-0.1.44/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.45/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.44
+Version: 0.1.45
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.44/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.45/hcs_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -62,17 +62,15 @@
 vhcs/cli/cmds/auth/__init__.py
 vhcs/cli/cmds/auth/admin/__init__.py
 vhcs/cli/cmds/auth/admin/get_org_idp_map.py
 vhcs/cli/cmds/daas/__init__.py
 vhcs/cli/cmds/daas/infra/__init__.py
 vhcs/cli/cmds/daas/infra/basic.py
 vhcs/cli/cmds/daas/infra/plan.py
-vhcs/cli/cmds/daas/infra/validate.py
 vhcs/cli/cmds/daas/tenant/__init__.py
-vhcs/cli/cmds/daas/tenant/basic.py
 vhcs/cli/cmds/daas/tenant/plan.py
 vhcs/cli/cmds/ims/__init__.py
 vhcs/cli/cmds/ims/list.py
 vhcs/cli/cmds/ims/list_copies.py
 vhcs/cli/cmds/inventory/__init__.py
 vhcs/cli/cmds/inventory/get.py
 vhcs/cli/cmds/inventory/list.py
@@ -96,22 +94,29 @@
 vhcs/cli/cmds/pki/get_org_cert.py
 vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/cli/cmds/pki/sign_resource_cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/plan/__init__.py
 vhcs/cli/cmds/plan/deploy.py
 vhcs/cli/cmds/plan/destroy.py
+vhcs/cli/cmds/plan/graph.py
 vhcs/cli/cmds/portal/__init__.py
 vhcs/cli/cmds/portal/entitlement/__init__.py
 vhcs/cli/cmds/portal/entitlement/delete.py
 vhcs/cli/cmds/portal/entitlement/get.py
 vhcs/cli/cmds/portal/entitlement/list.py
 vhcs/cli/cmds/portal/pool/__init__.py
+vhcs/cli/cmds/portal/pool/delete.py
 vhcs/cli/cmds/portal/pool/get.py
 vhcs/cli/cmds/portal/pool/list.py
+vhcs/cli/cmds/portal/site/__init__.py
+vhcs/cli/cmds/portal/site/create.py
+vhcs/cli/cmds/portal/site/delete.py
+vhcs/cli/cmds/portal/site/get.py
+vhcs/cli/cmds/portal/site/list.py
 vhcs/cli/cmds/profile/__init__.py
 vhcs/cli/cmds/profile/init.py
 vhcs/cli/cmds/vmhub/__init__.py
 vhcs/cli/cmds/vmhub/otp/__init__.py
 vhcs/cli/cmds/vmhub/otp/redeem.py
 vhcs/cli/cmds/vmhub/otp/request.py
 vhcs/common/__init__.py
@@ -162,18 +167,15 @@
 vhcs/plan/provider/dev/dummy.py
 vhcs/plan/provider/hcs/__init__.py
 vhcs/plan/provider/hcs/_prepare.py
 vhcs/plan/provider/hcs/entitlement.py
 vhcs/plan/provider/hcs/launch_item.py
 vhcs/plan/provider/hcs/pool_group.py
 vhcs/plan/provider/hcs/pool_template.py
-vhcs/plan/provider/runtime/__init__.py
-vhcs/plan/provider/runtime/_prepare.py
-vhcs/plan/provider/runtime/daas_tenant_calculation.py
-vhcs/plan/provider/runtime/dummy.py
+vhcs/plan/provider/hcs/site.py
 vhcs/service/__init__.py
 vhcs/service/_util.py
 vhcs/service/admin/__init__.py
 vhcs/service/admin/azure_infra.py
 vhcs/service/admin/edge.py
 vhcs/service/admin/helper.py
 vhcs/service/admin/provider.py
@@ -193,23 +195,27 @@
 vhcs/service/org_service/datacenter.py
 vhcs/service/org_service/details.py
 vhcs/service/pki/__init__.py
 vhcs/service/pki/certificate.py
 vhcs/service/portal/__init__.py
 vhcs/service/portal/entitlement.py
 vhcs/service/portal/pool.py
+vhcs/service/portal/site.py
 vhcs/service/vmhub/__init__.py
 vhcs/service/vmhub/otp.py
 vhcs/support/__init__.py
+vhcs/support/plan_util.py
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
+vhcs/support/daas/infra_calc.py
 vhcs/support/daas/template.py
-vhcs/support/daas/tenant.py
+vhcs/support/daas/tenant.py.xx
+vhcs/support/daas/tenant_calc.py
 vhcs/support/daas/templates/v1/infra.blueprint.yml
 vhcs/support/daas/templates/v1/infra.vars.yml
 vhcs/support/daas/templates/v1/tenant.blueprint.yml
 vhcs/support/daas/templates/v1/tenant.vars.yml
 vhcs/util/__init__.py
 vhcs/util/check_license.py
 vhcs/util/duration.py
```

### Comparing `hcs-cli-0.1.44/payload/lcm/zero.json` & `hcs-cli-0.1.45/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/pyproject.toml` & `hcs-cli-0.1.45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/setup.py` & `hcs-cli-0.1.45/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.44"
+VERSION = "0.1.45"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.44/tests/conftest.py` & `hcs-cli-0.1.45/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/test_utils.py` & `hcs-cli-0.1.45/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/__main__.py` & `hcs-cli-0.1.45/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,34 +10,39 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
+import yaml
 import vhcs.common.ctxp as ctxp
 from vhcs.common.ctxp import panic, choose
 from vhcs.plan.provider.azure import _az_facade
 from vhcs.support.daas import infra
 from vhcs.service import admin
+from vhcs.support.daas import infra, helper
 
+file_name = '.plan.yml'
 
 @click.command()
-def plan():
+@click.argument("name", type=str, required=True)
+def plan(name: str):
     """Interactive setup for shared infrastructure."""
-    
-    data = infra.all()
-
-    _select_provider(data['provider'])
-    _input_azure_sp(data['provider'])
-    _select_vnet(data['network'])
 
-    infra.save(data)
+    def collect_information(data):
+        vars = data['vars']
+        _select_provider(vars['provider'])
+        _input_azure_sp(vars['provider'])
+        _select_vnet(vars['network'])
 
+        infra.save(data)
 
+    return helper.prepare_plan_file(name, 'v1/infra.blueprint.yml', collect_information)
+    
 
 def _select_provider(data):
     providers = admin.provider.list(label='azure')
     if not providers:
         panic("No provider configured. Configure in HCS admin console first.")
 
     fn_provider_text = lambda p: f"{p['providerDetails']['data']['region']}, {p['name']}/{p['id']}"
@@ -48,16 +53,16 @@
     else:
         p = choose("Select region and provider", providers, fn_provider_text)
         if not p:
             return
     data['id'] = p['id']
 
 def _input_azure_sp(data):
-    data['applicationId'] = click.prompt("Input Azure service principle application ID:", default=data['applicationId'])
-    data['applicationSecret'] = click.prompt("Input Azure service principle application secret:", default=data['applicationSecret'])
+    data['applicationId'] = click.prompt("Input Azure service principle application ID", default=data['applicationId'] or "")
+    data['applicationSecret'] = click.prompt("Input Azure service principle application secret", default=data['applicationSecret'] or "")
 
 def _select_vnet(data):
-    vnets = _az_facade.list_vnets()
+    vnets = _az_facade.network.vnet.list()
     fn_get_text = lambda vnet: f"{vnet['name']} ({','.join(vnet['addressSpace']['addressPrefixes'])})"
     selected = choose("Select vNet:", vnets, fn_get_text)
     data['vNetId'] = selected['id']
     data['tenantCIDRs'] = ctxp.util.input_array("Tenant CIDRs", default=data['tenantCIDRs'])
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/validate.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.ctxp as ctxp
+from vhcs.service import portal
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
-_config_name = "daas-infra"
 
 @click.command()
-def validate():
-    """Validate the infra config"""
-
+@click.argument("id", type=str, required=True)
+@option_org_id
+def delete(id: str, org: str):
+    """Delete pool by ID"""
+    org_id=get_org_id(org)
+    ret = portal.pool.delete(id, org_id)
+    return ret
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/basic.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/plan/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,25 +9,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.support.daas import tenant
-
-@click.command("list")
-def list_tenants():
-    """List tenant configurations"""
-    return tenant.list()
-
-@click.command()
-@click.argument("text")
-def find(text: str):
-    """Get tenant by ID or customer name"""
-    t = tenant.get(text)
-    if t:
-        return t
-    return tenant.find_by_customer_name(text)
-
-
+help = "Horizon Plan manages deployments by files."
+hidden = True
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,92 +9,84 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import yaml
 import click
 from vhcs.service import admin, ims_catalog
 from vhcs.common.ctxp import choose, util as cli_util
-from vhcs.common import util as data_util
-from vhcs.support.daas import infra, template
+from vhcs.support.daas import infra, helper
 
 
-_surfix = '.plan.yml'
-
 @click.command()
 @click.argument("name", type=str, required=True)
 def plan(name: str):
     """Interactive command to request a DaaS tenant"""
-    
-    if name.endswith(_surfix):
-        name = name[:-len(_surfix)]
+    return helper.prepare_plan_file(name, 'v1/tenant.blueprint.yml', _collect_info)
 
-    data = _load_data(name)
-    
+def _collect_info(data):
+    #_fill_info_from_infra()
     vars = data['vars']
     _config_desktop(vars)
     _input_user_emails(vars)
 
-    _save_plan(data)
-
-def _save_plan(vars):
-    deployment_id = vars['deploymentId']
-    file_name = _get_file_name(deployment_id)
-    blueprint_file = 'v1/tenant.blueprint.yml'
-    blueprint = template.get(blueprint_file)
-    text = "\n".join([
-        yaml.safe_dump(vars, sort_keys=False),
-        "",
-        "# ----------------------------------",
-        "# Blueprint: " + blueprint_file,
-        "",
-        yaml.safe_dump(blueprint, sort_keys=False)
-    ])
-
-    with open(file_name, "w") as file:
-        file.write(text)
-
-    print("Plan saved as file: " + file_name)
-    print(f"To deploy the plan, use 'hcs plan deploy --file {file_name}'")
-
-def _load_data(deployment_id):
-
-    data = template.get('v1/tenant.vars.yml')
-    if not data['deploymentId']:
-        data['deploymentId'] = deployment_id
-    data['vars']['orgId'] = _get_org_id()
-
-    _apply_previous_input(data, deployment_id)
-
-    # Add defaults from shared infra config, if anything missing
-    data_util.deep_apply_defaults(data['vars'], infra.all())
-
-    return data
-
-def _apply_previous_input(data: dict, tenant_id: str):
-    file_name = _get_file_name(tenant_id)
-    prev = data_util.load_data_file(file_name)
-    if not prev:
-        return
-    prev_vars = prev.get('vars')
-    if not prev_vars:
-        return
+# def _save_plan(vars):
+#     blueprint_file = 'v1/tenant.blueprint.yml'
+#     blueprint = template.get(blueprint_file)
+#     text = "\n".join([
+#         yaml.safe_dump(vars, sort_keys=False),
+#         "",
+#         "# ----------------------------------",
+#         "# Blueprint: " + blueprint_file,
+#         "",
+#         yaml.safe_dump(blueprint, sort_keys=False)
+#     ])
+
+#     deployment_id = vars['deploymentId']
+#     file_name = _get_file_name(deployment_id)
+#     with open(file_name, "w") as file:
+#         file.write(text)
+
+#     print("Plan saved as file: " + file_name)
+#     print(f"To view the plan, use 'hcs plan graph -f {file_name}'")
+#     print(f"To deploy the plan, use 'hcs plan deploy -f {file_name}'")
+
+# def _load_data(deployment_id):
+
+#     data = template.get('v1/tenant.vars.yml')
+#     data['deploymentId'] = deployment_id
+#     data['vars']['orgId'] = _get_org_id()
+
+#     _apply_previous_input(data, deployment_id)
+
+#     # Add defaults from shared infra config, if anything missing
+#     data_util.deep_apply_defaults(data['vars'], infra.all())
+
+#     return data
+
+# def _apply_previous_input(data: dict, deployment_id: str):
+#     file_name = _get_file_name(deployment_id)
+#     prev = data_util.load_data_file(file_name)
+#     if not prev:
+#         return
+#     prev_vars = prev.get('vars')
+#     if not prev_vars:
+#         return
     
-    data_util.deep_apply_defaults(data['vars'], prev_vars)
+#     data_util.deep_apply_defaults(data['vars'], prev_vars)
 
-def _get_org_id():
-    from vhcs.common.sglib import auth
-    auth_info = auth.details(get_org_details=False)
-    return auth_info.org.id
+# def _get_org_id():
+#     from vhcs.common.sglib import auth
+#     auth_info = auth.details(get_org_details=False)
+#     return auth_info.org.id
 
-def _get_file_name(customer_id: str) -> str:
-    return customer_id + '.plan.yml'
+# def _get_file_name(customer_id: str) -> str:
+#     return 'tenant.' + customer_id + '.plan.yml'
 
 
 def _config_desktop(data):
 
     def _select_image_and_vm_sku(data):
         images = ims_catalog.helper.get_images_by_provider_instance_with_asset_details(data['provider']['id'])
         fn_get_text = lambda d: f"{d['name']}: {d['description']}"
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-help = "Horizon Plan manages deployments by files."
-hidden = True
+help = "Pool commands."
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/plan/deploy.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,27 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import vhcs.plan as plan
-import yaml
-from vhcs.common.ctxp import profile
+import vhcs.support.plan_util as util
 
 @click.command()
-@click.option("--file", "-f", type=click.File("rt"), required=True, help="Specified the combined plan file.")
+@click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
 def deploy(file, resource: str, parallel: bool):
 
-    with file:
-        payload = file.read()
-    data = yaml.safe_load(payload)
-    try:
-        concurrency = 10 if parallel else 1
-        extra = {
-            'profile': profile.current(exclude_secret=True)
-        }
-        return plan.deploy(data, resource, concurrency, extra)
+    data, extra = util.load_plan(file)
+    concurrency = 10 if parallel else 1
+
+    try:        
+        return plan.deploy(data, extra, resource, concurrency)
     except (FileNotFoundError, plan.PlanException) as e:
         return str(e), 1
 
 # def _identify_files(file: list[str], name: str):
 #     if not file and not name:
 #         panic("Either --file or --name must be specified")
 #     if file and name:
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/plan/destroy.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import yaml
 import vhcs.plan as plan
-from vhcs.common.ctxp import profile
+import vhcs.support.plan_util as util
 
 @click.command()
-@click.option("--file", "-f", type=click.File("rt"), required=True, help="Specified the combined plan file.")
+@click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
 def destroy(file, resource: str, parallel: bool, force: bool):
 
-    with file:
-        payload = file.read()
-    data = yaml.safe_load(payload)
+    data, extra = util.load_plan(file)
+    concurrency = 10 if parallel else 1
     try:
-        concurrency = 10 if parallel else 1
-        extra = {
-            'profile': profile.current(exclude_secret=True)
-        }
         return plan.destroy(data, force, resource, concurrency, extra)
     except (FileNotFoundError, plan.PlanException) as e:
         return str(e), 1
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,10 +21,8 @@
 @click.command()
 @click.argument("id", type=str, required=True)
 @option_org_id
 def delete(id: str, org: str):
     """Get entitlement by ID"""
     org_id = get_org_id(org)
     ret = portal.entitlement.delete(id, org_id)
-    if ret:
-        return ret
-    return ret, 1
+    return ret
```

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/cli/main.py` & `hcs-cli-0.1.45/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.45/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/jsondot.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,14 +43,22 @@
     """dot.notation access to dictionary attributes"""
 
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
+# TODO: how to remove the lib-specific dependency from this utility class?
+# Register the represent_dict function with SafeDumper
+def _represent_dict(dumper, data):
+    return dumper.represent_dict(data.items())
+import yaml
+yaml.SafeDumper.add_representer(dotdict, _represent_dict)
+
+
 def dotify(target: Any) -> Any:
     """Deeply convert an object from dict to dotdict"""
 
     # If already dotified, skip
     if isinstance(target, dotdict):
         return target
     if isinstance(target, list):
```

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.45/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/duration.py` & `hcs-cli-0.1.45/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/logger.py` & `hcs-cli-0.1.45/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.45/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.45/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.45/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.45/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.45/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.45/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/sglib/util.py` & `hcs-cli-0.1.45/vhcs/common/sglib/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/common/util.py` & `hcs-cli-0.1.45/vhcs/common/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.45/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/core.py` & `hcs-cli-0.1.45/vhcs/plan/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,46 @@
     blueprint, pending = helper.process_template(data)
     deployment_id = blueprint['deploymentId']
     state_file = deployment_id + '.state.yml'
     prev = _load_state(state_file)
     state = {'pending': pending}
     state.update(blueprint)
     state.update(prev)
-    state['log']['deploy'] = []    # clear log
+
+    # try solving more variables
+    for k, v in state['output'].items():
+        if not v:
+            continue
+        if not _has_successful_deployment(state, k):
+            continue
+        _resolve_pending_keys(state, k)
     
     return blueprint, state, state_file
 
-def deploy(data: dict, resource_name: str = None, concurrency: int = 4, additional_context: dict = None):
+def _has_successful_deployment(state, name):
+    for v in state['log']['deploy']:
+        if v['name'] != name:
+            continue
+        if v['action'] == 'success':
+            return True
+        
+def deploy(data: dict, additional_context: dict = None, resource_name: str = None, concurrency: int = 4):
     
     blueprint, state, state_file = _prepare_data(data, additional_context)
+    state['log']['deploy'] = []    # clear deploy log
 
     def process_resource(name: str, res_data: dict):
         if name == 'defaults':
             return
         if res_data.get('type'):    #provider
             return
         
         _deploy_res(name, res_data, state)
-        _resolve_pending_keys(blueprint, state, name)
+        _resolve_pending_keys(state, name)
+        util.save_data_file(state, state_file)
         if resource_name and name == resource_name:
             return False
 
     try:
         dag.process_blueprint(blueprint, process_resource, concurrency)
     except CalledProcessError as e:
         raise PlanException(str(e))
@@ -129,29 +145,33 @@
 
 
 def _deploy_res(name, res, state):
     def add_log(action: str, details: str = None):
         _add_log(state, 'deploy', res['kind'], name, action, details)
 
     def fn_deploy1(handler, res_data, res_state, fn_set_state):
-        if res_state:
+        if res_state and not _is_runtime(res):
             add_log('skipped')
             return
         
         add_log('start')
         if _has_save_state(handler.deploy):
             new_state = handler.deploy(res_data, fn_set_state)
         else:
             new_state = handler.deploy(res_data)
         if new_state:
             fn_set_state(new_state)
         add_log('success')
     
     _handle_resource(name, res, state, True, add_log, fn_deploy1)
 
+def _is_runtime(res):
+    kind = res.get('kind')
+    return kind and kind.startswith('runtime/')
+
 def _has_save_state(fn):
     signature = inspect.signature(fn)
     args = list(signature.parameters.keys())
     if len(args) < 2:
         return False
     name = args[1]
     if name == 'save_state':
@@ -166,29 +186,29 @@
 #         i = int(match.group(1))
 #         name = state['resources'][i]['name']
 #         n = attr_path.index(']')
 #         readable_path = 'resources.' + name + attr_path[n + 1:]
 #         return readable_path
 #     return attr_path
 
-def _resolve_pending_keys(blueprint, state, resource_name):
+def _resolve_pending_keys(state, resource_name):
     prefix = resource_name + "."
     for attr_path, var_name in state['pending'].items():
         if not var_name.startswith(prefix) and var_name != resource_name:
             continue
         # found a key to solve
         
         # update that key
-        expr = util.deep_get_attr(blueprint, attr_path)
+        expr = util.deep_get_attr(state, attr_path)
         def _get_value(path):
             return _get_value_by_path(state, path, attr_path), True
         resolved_value, _pending_var = util.resolve_expression(expr, _get_value)
 
         log.debug('Resolved. %s: %s -> %s', attr_path, var_name, resolved_value)
-        util.deep_set_attr(blueprint, attr_path, resolved_value)
+        util.deep_set_attr(state, attr_path, resolved_value)
 
 def _assert_all_vars_resolved(data, name):
     def fn_on_value(path, value):
         if isinstance(value, str) and value.find('${') >= 0:
             raise PlanException(f"Unresolved variable '{path}' for plugin '{name}'. Value={value}")
         return value
     util.deep_update_object_value(data, fn_on_value)
@@ -196,28 +216,29 @@
 _providers = {}
 _provider_lock = threading.Lock()
 def _get_resource_handler(kind: str, state: dict):
     provider_type, res_handler_type = kind.split('/')
     res_handler_type = res_handler_type.replace('-', '_')
     # Ensure provider initialized
     with _provider_lock:
+        if provider_type == 'runtime':
+            return import_module(res_handler_type)
         if not provider_type in _providers:
             provider = import_module("vhcs.plan.provider." + provider_type)
             # Get provider data
             filter_by_type = lambda m: m['type'] == provider_type
             providers = state.get('providers', {})
             meta = next(filter(filter_by_type, providers), None)
             data = meta.get('data') if meta else None
             if data:
                 _assert_all_vars_resolved(data, provider_type)
             log.info("[init] Provider: %s", provider_type)
             state['output'][provider_type] = provider.prepare(data)
             log.info("[ok  ] Provider: %s", provider_type)
             _providers[provider_type] = 1
-
     module_name = f"vhcs.plan.provider.{provider_type}.{res_handler_type}"
     return import_module(module_name)
 
 def get_common_items(iter1, iter2):
     return set(iter1).intersection(set(iter2))
 
 def _handle_resource(name, res, state, vars_must_resolve: bool, add_log: typing.Callable, fn_process: typing.Callable):
@@ -226,15 +247,15 @@
         data = res.get('data', {})
         if data:
             if vars_must_resolve:
                 _assert_all_vars_resolved(data, name)
 
         handler = _get_resource_handler(kind, state)
         def _handle_resource_1(resource_data, resource_state, fn_set_state):
-            if _is_runtime(kind):   # runtime has no refresh
+            if _is_runtime(res):   # runtime has no refresh
                 pass
             else:
                 new_state = handler.refresh(resource_data, resource_state)
                 if new_state:
                     fn_set_state(new_state)
                     resource_state = new_state
 
@@ -329,20 +350,18 @@
                 pass
             else:
                 # add_log('error', e) will be handled by framework.
                 raise
 
     _handle_resource(name, res, state, False, add_log, fn_destroy1)
 
-def _is_runtime(kind: str):
-    return kind.startswith('runtime/')
-
 def destroy(data, force: bool, resource_name: str = None, concurrency: int = 4, additional_context: dict = None):
     
     blueprint, state, state_file = _prepare_data(data, additional_context)
+    state['log']['destroy'] = []    # clear destroy log
 
     def destroy_resource(node_name, node):
         # skip provider
         if 'type' in node:  
             return
         kind = node.get('kind')
         # skip non-resources, e.g. 'defaults'
@@ -352,17 +371,22 @@
         if kind.startswith('runtime/'):
             return
         
         res = state['resources'].get(node_name)
         if not res:
             res = blueprint['resources'][node_name]
         _destroy_res(node_name, res, state, force)
+        util.save_data_file(state, state_file)
         if resource_name and resource_name == node_name:
             return True
 
     try:
         dag.reverse_traverse(blueprint, destroy_resource)
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
         util.save_data_file(state, state_file)
 
+def graph(data: dict, additional_context: dict = None, simplify: bool = True):
+    blueprint, state, state_file = _prepare_data(data, additional_context)
+    g = dag.graph(blueprint, state, simplify)
+    return g
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/dag.py` & `hcs-cli-0.1.45/vhcs/plan/dag.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 import threading
 from graphlib import TopologicalSorter
+from graphviz import Digraph
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable
 from vhcs.common import util
 
 class Node:
     id: str
     dependencies: list[str] = []
@@ -91,20 +92,19 @@
     defaults = blueprint.get('defaults')
     if defaults:
         add_node('defaults', defaults)
     providers = blueprint.get('providers')
     if providers:
         for p in providers:
             add_node(p['type'], p)
+    
+    dag.validate()
     return dag
 
 def _walkthrough(dag: DAG, fn_process_node: Callable, concurrency: int):
-
-    dag.validate()
-
     topological_sorter = TopologicalSorter(dag.graph)
     topological_sorter.prepare()
     lock = threading.Lock()
 
     flags = {
         'err': None,
         'stop': False
@@ -136,14 +136,78 @@
                 continue
             for node in read_nodes:
                 executor.submit(process_node, node)
         executor.shutdown(wait=True)
         if flags['err']:
             raise flags['err']
 
+def _has_indirect_dependency(tree: dict, from_node: str, to_node: str):
+    deps = list(tree[from_node])
+    deps.remove(to_node)
+    while deps:
+        n = deps.pop()
+        new_deps = tree[n]
+        if to_node in new_deps:
+            return True
+        deps += new_deps
+    return False
+
+def graph(blueprint: dict, state: dict, simplify: bool) -> Digraph:
+    dag = _build_graph(blueprint)
+    topological_sorter = TopologicalSorter(dag.graph)
+    sorted_nodes = list(topological_sorter.static_order())
+    graph = Digraph(name=f"Deployment {blueprint['deploymentId']}", comment="Simplified" if simplify else None)
+    
+    class styles:
+        deployed = {
+            'style': 'filled',
+            'fillcolor': 'lightgrey'
+        }
+        runtime = {
+            'shape': 'hexagon'
+        }
+        provider = {
+            'shape': 'component'
+        }
+        resource = {
+        }
+        vars = {
+            'shape': 'note'
+        }
+
+    def _get_node_style(node_name):
+        n = dag.data[node_name]
+        attr = {}
+        if 'type' in n:
+            attr |= styles.provider
+        elif node_name in blueprint['resources']:
+            if n['kind'].startswith('runtime/'):
+                attr |= styles.runtime
+            else:
+                attr |= styles.resource
+        elif node_name in state:
+            attr |= styles.vars
+        if state['output'].get(node):
+            attr |= styles.deployed
+        return attr
+        
+    
+    for node in sorted_nodes:
+        attrs = _get_node_style(node)
+        graph.node(node, **attrs)
+
+    # Add the edges based on the dependencies
+    for node, dependencies in dag.graph.items():
+        for dependency in dependencies:
+            if simplify and _has_indirect_dependency(dag.graph, from_node=node, to_node=dependency):
+                continue    #simplify the diagram by removing ommitable 
+            graph.edge(dependency, node)
+
+    return graph
+
 # dag = DAG()
 # dag.add("b", "b")
 # dag.add("a", "a", {"b", "c"})
 # dag.add("c", "c")
 
 # def fn_proc(id, data):
 #     print("processing", id, data)
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/helper.py` & `hcs-cli-0.1.45/vhcs/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_user.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/nsg.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 def deploy(data: dict) -> dict:
     name = data['name']
     location = data['location']
     resourceGroup = data['resourceGroup']
     tags = data.get('tags')
 
-    return az.create_nsg(resourceGroup, name, location, tags)
+    return az.network.nsg.create(resourceGroup, name, location, tags)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def destroy(data: dict, state: dict) -> dict:
     if state.get('NewNSG'):
         id = state.get('NewNSG')['id']
-        return az.delete_nsg_by_id(id)
+        return az.network.nsg.delete_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
-    return az.delete_nsg(name, resourceGroup)
+    return az.network.nsg.delete(name, resourceGroup)
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/resource_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from . import _az_facade as az
 
 def deploy(data: dict) -> dict:
     name = data['name']
     location = data['location']
     tags = data.get('tags')
-    return az.create_resource_group(name, location, tags)
+    return az.resource_group.create(name, location, tags)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def destroy(data: dict, state: dict) -> dict:
     name = data['name']
-    return az.delete_resource_group(name)
+    return az.resource_group.delete(name)
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.45/vhcs/plan/provider/azure/subnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 def deploy(data: dict) -> dict:
     name = data['name']
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
     cidr = data['cidr']
     nsgName = data['nsgName']
 
-    return az.create_subnet(resourceGroup, vNetName, name, cidr, nsgName)
+    return az.network.subnet.create(resourceGroup, vNetName, name, cidr, nsgName)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def destroy(data: dict, state: dict) -> dict:
     id = state.get('id')
     if id:
-        return az.delete_subnet_by_id(id)
+        return az.network.subnet.delete_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
-    az.delete_subnet(resourceGroup, vNetName, name)
+    az.network.subnet.delete(resourceGroup, vNetName, name)
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.45/vhcs/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.45/vhcs/plan/provider/hcs/entitlement.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         if id:
             return portal.entitlement.get(id, data['orgId'])
     
     # Fall back with smart find by users
     # TODO
 
 def destroy(data: dict, state: dict) -> dict:
-    return portal.entitlement.delete(state['id'])
+    return portal.entitlement.delete(state['id'], data['orgId'])
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.45/vhcs/plan/provider/hcs/launch_item.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,9 @@
         return pools[0]
     return state
 
 def destroy(data: dict, state: dict) -> dict:
     if state:
         id = state.get('id')
         if id:
-            return portal.pool.delete(id)
+            return portal.pool.delete(id, data['orgId'])
     return state
```

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/plan/provider/runtime/daas_tenant_calculation.py` & `hcs-cli-0.1.45/vhcs/support/daas/tenant_calc.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         'uag_deployment_id': uag_deployment_id,
         'edge_deployment_id': edge_deployment_id,
         'vm_sku': vm_skus[0]
     }
 
     org_idp_map = auth.admin.get_org_idp_map()
     return {
-        'location': 'westus2',
+        'location': region,
         'cidr': _calculate_cidr(),
-        'vNet': az.get_vnet(data['network']['vNetId']),
+        'vNet': az.network.vnet.get(data['network']['vNetId']),
         'providerInstance': providerInstance,
         'template': template,
         'number_of_users': number_of_users,
         'orgIdpMap': org_idp_map
     }
 
 def _generate_password():
```

### Comparing `hcs-cli-0.1.44/vhcs/service/_util.py` & `hcs-cli-0.1.45/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.45/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/admin/edge.py` & `hcs-cli-0.1.45/vhcs/service/admin/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/admin/helper.py` & `hcs-cli-0.1.45/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/admin/provider.py` & `hcs-cli-0.1.45/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/admin/template.py` & `hcs-cli-0.1.45/vhcs/service/admin/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/auth/admin.py` & `hcs-cli-0.1.45/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.45/vhcs/service/ims_catalog/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.45/vhcs/service/ims_catalog/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.45/vhcs/service/ims_catalog/images.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.45/vhcs/service/inventory/vm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.45/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/lcm/template.py` & `hcs-cli-0.1.45/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.45/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/org_service/details.py` & `hcs-cli-0.1.45/vhcs/service/org_service/details.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.45/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.45/vhcs/service/portal/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/service/portal/pool.py` & `hcs-cli-0.1.45/vhcs/service/portal/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 
 def list(**kwargs):
     def _get_page(query_string):
         url = "/v2/pools?" + query_string
         return _client.get(url)
     return PageRequest(_get_page, **kwargs).get()
 
-def delete(id: str):
-    url = "/v2/pools/" + id
+def delete(id: str, org_id: str):
+    url = f"/v2/pools/{id}?org_id={org_id}"
     return _client.delete(url)
```

### Comparing `hcs-cli-0.1.44/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.45/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/support/daas/infra.py` & `hcs-cli-0.1.45/vhcs/support/daas/infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # 'defaults' is a group of variables that are calculated and referenced by multiple resources.
 # The defaults helps to deduplicate calculated variables, and 
 defaults:
   name: titan-lite-${deploymentId}
   tags:
-    - deploymentId=${deploymentId}
+    deployment: ${deploymentId}
+    managed-by: titan-lite
 
 # The providers section specifies provider-specific data. Normally this required to initialize
 # a provider.
 providers:
   - type: azure
     data: ${vars.provider}
   - type: hcs
     data:
 
 resources:
   myRuntime:
-    kind: runtime/daas-tenant-calculation # Utilize a custom hcs resource to calculate dynamic values
+    kind: runtime/vhcs.support.daas.tenant_calc # Custom calculation of values
     data: ${vars} # Take the entire unchanged vars as input
 
   myRg:
     kind: azure/resource-group
     data:
       name: ${defaults.name}
       location: ${myRuntime.location}
```

### Comparing `hcs-cli-0.1.44/vhcs/support/daas/tenant.py` & `hcs-cli-0.1.45/vhcs/support/daas/tenant.py.xx`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/support/profile.py` & `hcs-cli-0.1.45/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/util/check_license.py` & `hcs-cli-0.1.45/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/util/duration.py` & `hcs-cli-0.1.45/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/util/pki_util.py` & `hcs-cli-0.1.45/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/util/query_util.py` & `hcs-cli-0.1.45/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.44/vhcs/util/versions.py` & `hcs-cli-0.1.45/vhcs/util/versions.py`

 * *Files identical despite different names*

