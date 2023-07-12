# Comparing `tmp/thipster-0.23.2.tar.gz` & `tmp/thipster-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.2.tar", last modified: Mon Jul  3 07:18:40 2023, max compression
+gzip compressed data, was "thipster-0.23.3.tar", last modified: Wed Jul 12 09:15:15 2023, max compression
```

## Comparing `thipster-0.23.2.tar` & `thipster-0.23.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.544182 thipster-0.23.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-07-03 07:18:36.000000 thipster-0.23.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-03 07:18:36.000000 thipster-0.23.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-03 07:18:40.544182 thipster-0.23.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4544 2023-07-03 07:18:36.000000 thipster-0.23.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-07-03 07:18:36.000000 thipster-0.23.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-03 07:18:36.000000 thipster-0.23.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 07:18:40.544182 thipster-0.23.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-07-03 07:18:37.000000 thipster-0.23.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.532181 thipster-0.23.2/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.532181 thipster-0.23.2/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.532181 thipster-0.23.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.536182 thipster-0.23.2/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    18947 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    14360 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.536182 thipster-0.23.2/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     8033 2023-07-03 07:18:36.000000 thipster-0.23.2/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.536182 thipster-0.23.2/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.536182 thipster-0.23.2/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.540182 thipster-0.23.2/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6551 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6285 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.540182 thipster-0.23.2/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.544182 thipster-0.23.2/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13040 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14699 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3283 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    24598 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.544182 thipster-0.23.2/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.544182 thipster-0.23.2/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26119 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-07-03 07:18:36.000000 thipster-0.23.2/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:18:40.536182 thipster-0.23.2/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-03 07:18:40.000000 thipster-0.23.2/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-07-03 07:18:40.000000 thipster-0.23.2/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 07:18:40.000000 thipster-0.23.2/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-03 07:18:40.000000 thipster-0.23.2/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-03 07:18:40.000000 thipster-0.23.2/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-12 09:15:11.000000 thipster-0.23.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-12 09:15:11.000000 thipster-0.23.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-07-12 09:15:15.130450 thipster-0.23.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-07-12 09:15:11.000000 thipster-0.23.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-07-12 09:15:11.000000 thipster-0.23.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-12 09:15:11.000000 thipster-0.23.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:15:15.130450 thipster-0.23.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-07-12 09:15:12.000000 thipster-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    18947 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    14360 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     8033 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13040 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14699 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    24598 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26119 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.2/LICENSE` & `thipster-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/PKG-INFO` & `thipster-0.23.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.2
+Version: 0.23.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: google
 Provides-Extra: doc
-Provides-Extra: test
 Provides-Extra: dev
-Provides-Extra: google
+Provides-Extra: test
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.2 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.3 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
-test Provides-Extra: dev Provides-Extra: google License-File: LICENSE #
-THipster THipster is a tool dedicated to simplifying the difficulty associated
-with writing Terraform files. It allows users to write infrastructure as code
-in a simplified format, using either YAML (with JINJA) or the dedicated
-Thipster DSL. Written entirely in Python, it leverages the Python CDK for
-Terraform to create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
+doc Provides-Extra: dev Provides-Extra: test License-File: LICENSE # THipster
+THipster is a tool dedicated to simplifying the difficulty associated with
+writing Terraform files. It allows users to write infrastructure as code in a
+simplified format, using either YAML (with JINJA) or the dedicated Thipster
+DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
+create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                versions] [Ruff]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.23.2/README.md` & `thipster-0.23.3/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/pyproject.toml` & `thipster-0.23.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/setup.py` & `thipster-0.23.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.2'
+__version__ = '0.23.3'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.2/tests/engine/test_engine.py` & `thipster-0.23.3/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/engine/test_generation.py` & `thipster-0.23.3/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.3/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.3/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.3/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.3/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.3/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/test_parsedfile.py` & `thipster-0.23.3/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/test_parserfactory.py` & `thipster-0.23.3/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/parser/test_yamlparser.py` & `thipster-0.23.3/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/repository/test_github_repository.py` & `thipster-0.23.3/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/repository/test_local_repository.py` & `thipster-0.23.3/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/repository/test_resourcemodel.py` & `thipster-0.23.3/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/test_e2e.py` & `thipster-0.23.3/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/tests/test_tools.py` & `thipster-0.23.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/auth/google.py` & `thipster-0.23.3/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/engine.py` & `thipster-0.23.3/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/i_parser.py` & `thipster-0.23.3/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/i_repository.py` & `thipster-0.23.3/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/i_terraform.py` & `thipster-0.23.3/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/parsed_file.py` & `thipster-0.23.3/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/engine/resource_model.py` & `thipster-0.23.3/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/helpers.py` & `thipster-0.23.3/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.3/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.3/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.3/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.3/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.3/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.3/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/token.py` & `thipster-0.23.3/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.3/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/exceptions.py` & `thipster-0.23.3/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/parser_factory.py` & `thipster-0.23.3/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/parser/yaml_parser.py` & `thipster-0.23.3/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/repository/exceptions.py` & `thipster-0.23.3/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/repository/github.py` & `thipster-0.23.3/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/repository/json.py` & `thipster-0.23.3/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/repository/local.py` & `thipster-0.23.3/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/terraform/cdk.py` & `thipster-0.23.3/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster/terraform/exceptions.py` & `thipster-0.23.3/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.2/thipster.egg-info/PKG-INFO` & `thipster-0.23.3/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.2
+Version: 0.23.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: google
 Provides-Extra: doc
-Provides-Extra: test
 Provides-Extra: dev
-Provides-Extra: google
+Provides-Extra: test
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.2 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.3 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
-test Provides-Extra: dev Provides-Extra: google License-File: LICENSE #
-THipster THipster is a tool dedicated to simplifying the difficulty associated
-with writing Terraform files. It allows users to write infrastructure as code
-in a simplified format, using either YAML (with JINJA) or the dedicated
-Thipster DSL. Written entirely in Python, it leverages the Python CDK for
-Terraform to create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
+doc Provides-Extra: dev Provides-Extra: test License-File: LICENSE # THipster
+THipster is a tool dedicated to simplifying the difficulty associated with
+writing Terraform files. It allows users to write infrastructure as code in a
+simplified format, using either YAML (with JINJA) or the dedicated Thipster
+DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
+create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                versions] [Ruff]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.23.2/thipster.egg-info/SOURCES.txt` & `thipster-0.23.3/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

