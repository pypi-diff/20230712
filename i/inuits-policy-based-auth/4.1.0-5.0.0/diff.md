# Comparing `tmp/inuits_policy_based_auth-4.1.0.tar.gz` & `tmp/inuits_policy_based_auth-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-4.1.0.tar", last modified: Mon Jul  3 08:17:26 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-5.0.0.tar", last modified: Wed Jul 12 13:54:23 2023, max compression
```

## Comparing `inuits_policy_based_auth-4.1.0.tar` & `inuits_policy_based_auth-5.0.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/
--rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/LICENSE
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7133 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/README.md
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1881 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     8856 2023-07-03 08:15:33.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2744 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      571 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/
--rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1435 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2942 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1591 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)    10620 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-07-03 08:17:26.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-07-03 08:17:26.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-07-03 08:17:26.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-07-03 08:17:26.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-07-03 08:17:26.000000 inuits_policy_based_auth-4.1.0/inuits_policy_based_auth.egg-info/top_level.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/setup.cfg
--rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-07-03 08:16:10.000000 inuits_policy_based_auth-4.1.0/setup.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.612867 inuits_policy_based_auth-4.1.0/tests/
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/tests/integration/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.616200 inuits_policy_based_auth-4.1.0/tests/integration/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/integration/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1947 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/custom_token.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1508 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/flask_process.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/integration/test_api/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/test_api/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1793 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/test_api/app.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2593 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3480 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/unit/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/unit/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/unit/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1040 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-07-03 08:17:26.619534 inuits_policy_based_auth-4.1.0/tests/unit/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)    11998 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.1.0/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.826527 inuits_policy_based_auth-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.826527 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/custom_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/flask_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-4.1.0/LICENSE` & `inuits_policy_based_auth-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/PKG-INFO` & `inuits_policy_based_auth-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: inuits_policy_based_auth
-Version: 4.1.0
-Summary: Module for securing API endpoints based on policies.
-Author: Inuits
-Author-email: developers@inuits.eu
-License: GPLv2
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Provides: inuits_policy_based_auth
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # inuits_policy_based_auth
 inuits_policy_based_auth is a python package for securing API endpoints based on policies.
 
 ## Installation
 Install inuits_policy_based_auth as follows:
 ```
 pip install inuits-policy-based-auth
```

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         used as an interface for concrete implementations of authorization policies
     RequestContext
         contains data about the context of a request
     PolicyFactory
         the main class, used to apply policies
 """
 
-
 from inuits_policy_based_auth.authentication.base_authentication_policy import (
     BaseAuthenticationPolicy,
 )
 from inuits_policy_based_auth.authorization.base_authorization_policy import (
     BaseAuthorizationPolicy,
 )
 from inuits_policy_based_auth.contexts import RequestContext
```

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/request_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/user_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/inuits_policy_based_auth/policy_factory.py` & `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/setup.py` & `inuits_policy_based_auth-5.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,53 @@
-from setuptools import setup, find_packages
+# pyproject.toml
 
+[build-system]
+requires      = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
 
-with open("README.md", "r") as readme_file:
-    long_desc = readme_file.read()
+[project]
+name = "inuits_policy_based_auth"
+version = "5.0.0"
+description = "Module for securing API endpoints based on policies."
+readme = "README.md"
+authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+keywords = ["inuits", "policy", "auth"]
+dependencies = [
+    "Authlib>=1.2.0",
+    "cffi>=1.15.1",
+    "click>=8.1.3",
+    "cryptography>=40.0.2",
+    "MarkupSafe>=2.1.2",
+    "pycparser>=2.21",
+    "requests>=2.28.2",
+    "Werkzeug>=2.2.3",
+]
 
-setup(
-    author="Inuits",
-    author_email="developers@inuits.eu",
-    classifiers=[
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-    ],
-    description="Module for securing API endpoints based on policies.",
-    install_requires=[
-        "Authlib>=1.2.0",
-        "cffi>=1.15.1",
-        "click>=8.1.3",
-        "cryptography>=40.0.2",
-        "MarkupSafe>=2.1.2",
-        "pycparser>=2.21",
-        "requests>=2.28.2",
-        "Werkzeug>=2.2.3",
-    ],
-    license="GPLv2",
-    long_description=long_desc,
-    long_description_content_type="text/markdown",
-    name="inuits_policy_based_auth",
-    packages=find_packages(exclude=["tests"]),
-    provides=["inuits_policy_based_auth"],
-    version="4.1.0",
-)
+[project.optional-dependencies]
+dev = [
+    "black==23.7.0",
+    "build==0.10.0",
+    "coverage==7.2.7",
+    "Flask-RESTful==0.3.10",
+    "Flask==2.3.2",
+    "mypy-extensions==1.0.0",
+    "pathspec==0.11.1",
+    "platformdirs==3.8.1",
+    "pyjwt==2.7.0",
+    "pytest==7.4.0",
+    "python-dotenv==1.0.0",
+    "tomli==2.0.1",
+    "twine==4.0.2",
+]
+
+[project.urls]
+Homepage = "https://github.com/inuits/inuits-policy-based-auth"
```

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/custom_token.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/flask_process.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/flask_process.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/test_api/app.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/app.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/policy_loader.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-5.0.0/src/tests/integration/test_policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-4.1.0/tests/unit/test_policy_factory.py` & `inuits_policy_based_auth-5.0.0/src/tests/unit/test_policy_factory.py`

 * *Files identical despite different names*

