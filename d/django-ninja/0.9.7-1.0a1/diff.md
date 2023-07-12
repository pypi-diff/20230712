# Comparing `tmp/django-ninja-0.9.7.tar.gz` & `tmp/django_ninja-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ninja-0.9.7.tar", last modified: Fri Dec 25 12:49:03 2020, max compression
+gzip compressed data, was "django_ninja-1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django-ninja-0.9.7.tar` & `django_ninja-1.0a1.tar`

### file list

```diff
@@ -1,150 +1,276 @@
--rw-r--r--   0        0        0       35 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.coveragerc
--rw-r--r--   0        0        0       66 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.dockerignore
--rw-r--r--   0        0        0      554 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      617 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.github/workflows/test.yml
--rw-r--r--   0        0        0       85 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.gitignore
--rw-r--r--   0        0        0      930 2020-12-25 12:48:38.391175 django-ninja-0.9.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1086 2020-12-25 12:48:38.391175 django-ninja-0.9.7/LICENSE
--rw-r--r--   0        0        0     2816 2020-12-25 12:48:38.391175 django-ninja-0.9.7/README.md
--rw-r--r--   0        0        0     5904 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/async-support.md
--rw-r--r--   0        0        0     1001 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/help.md
--rw-r--r--   0        0        0    28154 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/auth-swagger-ui-prompt.png
--rw-r--r--   0        0        0    27900 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/auth-swagger-ui.png
--rw-r--r--   0        0        0    51900 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/benchmark.png
--rw-r--r--   0        0        0   654914 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-editor.gif
--rw-r--r--   0        0        0    46786 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0    55925 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0    44459 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/deprecated.png
--rw-r--r--   0        0        0     2717 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/docs-logo.png
--rw-r--r--   0        0        0     6234 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/favicon.png
--rw-r--r--   0        0        0     3439 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/github-star.png
--rw-r--r--   0        0        0    18865 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/hero.png
--rw-r--r--   0        0        0    95509 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/index-swagger-ui.png
--rw-r--r--   0        0        0    12028 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/logo-big.png
--rw-r--r--   0        0        0   122725 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/nested-routers-swagger.png
--rw-r--r--   0        0        0    45259 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_description.png
--rw-r--r--   0        0        0    53995 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_description_docstring.png
--rw-r--r--   0        0        0    28482 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_summary.png
--rw-r--r--   0        0        0    22627 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_summary_default.png
--rw-r--r--   0        0        0    48354 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_tags.png
--rw-r--r--   0        0        0    65000 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/simple-routers-swagger.png
--rw-r--r--   0        0        0   115803 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/tutorial-path-swagger.png
--rw-r--r--   0        0        0     3304 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/index.md
--rw-r--r--   0        0        0     2956 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/motivation.md
--rw-r--r--   0        0        0     4653 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/cbv.md
--rw-r--r--   0        0        0      492 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/index.md
--rw-r--r--   0        0        0     3873 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/models.md
--rw-r--r--   0        0        0      114 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/releases.md
--rw-r--r--   0        0        0     3991 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/authentication.md
--rw-r--r--   0        0        0     4569 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/body.md
--rw-r--r--   0        0        0     5805 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/crud.md
--rw-r--r--   0        0        0      816 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/csrf.md
--rw-r--r--   0        0        0     1800 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/index.md
--rw-r--r--   0        0        0     3221 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/operation_params.md
--rw-r--r--   0        0        0     2844 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     2812 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     5289 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/response-schema.md
--rw-r--r--   0        0        0     4145 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/routers.md
--rw-r--r--   0        0        0     1480 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/versioning.md
--rw-r--r--   0        0        0     1113 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/mkdocs.yml
--rw-r--r--   0        0        0      274 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/index001.py
--rw-r--r--   0        0        0      442 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey01.py
--rw-r--r--   0        0        0      322 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey02.py
--rw-r--r--   0        0        0      298 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey03.py
--rw-r--r--   0        0        0      314 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/basic01.py
--rw-r--r--   0        0        0      271 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/bearer01.py
--rw-r--r--   0        0        0      198 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/code001.py
--rw-r--r--   0        0        0      231 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/code002.py
--rw-r--r--   0        0        0      542 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/global01.py
--rw-r--r--   0        0        0      390 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/multiple01.py
--rw-r--r--   0        0        0        0 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/schema01.py
--rw-r--r--   0        0        0      195 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code01.py
--rw-r--r--   0        0        0      255 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code02.py
--rw-r--r--   0        0        0      272 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code03.py
--rw-r--r--   0        0        0       94 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code01.py
--rw-r--r--   0        0        0      325 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code010.py
--rw-r--r--   0        0        0       99 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code02.py
--rw-r--r--   0        0        0      209 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code01.py
--rw-r--r--   0        0        0      252 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code010.py
--rw-r--r--   0        0        0      281 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code02.py
--rw-r--r--   0        0        0      157 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code03.py
--rw-r--r--   0        0        0      233 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/__init__.py
--rw-r--r--   0        0        0       52 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/__init__.py
--rw-r--r--   0        0        0     1734 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/datastructures.py
--rw-r--r--   0        0        0     1326 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/request.py
--rw-r--r--   0        0        0       19 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/constants.py
--rw-r--r--   0        0        0      525 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/errors.py
--rw-r--r--   0        0        0     7751 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/main.py
--rw-r--r--   0        0        0       44 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/__init__.py
--rw-r--r--   0        0        0     6824 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/schema.py
--rw-r--r--   0        0        0      891 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/urls.py
--rw-r--r--   0        0        0     1424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/views.py
--rw-r--r--   0        0        0     8806 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/operation.py
--rw-r--r--   0        0        0     1631 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/params.py
--rw-r--r--   0        0        0     2213 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/params_models.py
--rw-r--r--   0        0        0      448 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/responses.py
--rw-r--r--   0        0        0     6510 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/router.py
--rw-r--r--   0        0        0     1135 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/schema.py
--rw-r--r--   0        0        0      209 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/__init__.py
--rw-r--r--   0        0        0      981 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/apikey.py
--rw-r--r--   0        0        0      693 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/base.py
--rw-r--r--   0        0        0     2171 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/http.py
--rw-r--r--   0        0        0      322 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/session.py
--rw-r--r--   0        0        0       93 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/__init__.py
--rw-r--r--   0        0        0     5115 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/details.py
--rw-r--r--   0        0        0     1429 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/utils.py
--rw-r--r--   0        0        0      956 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/templates/ninja/swagger.html
--rw-r--r--   0        0        0      440 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/utils.py
--rw-r--r--   0        0        0     1883 2020-12-25 12:48:38.403175 django-ninja-0.9.7/pyproject.toml
--rwxr-xr-x   0        0        0      131 2020-12-25 12:48:38.403175 django-ninja-0.9.7/scripts/build-docs.sh
--rw-r--r--   0        0        0     3774 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/client.py
--rw-r--r--   0        0        0      451 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/__init__.py
--rw-r--r--   0        0        0      424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/asgi.py
--rw-r--r--   0        0        0     1645 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/settings.py
--rw-r--r--   0        0        0      695 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/urls.py
--rw-r--r--   0        0        0      424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/wsgi.py
--rwxr-xr-x   0        0        0      657 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/manage.py
--rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/__init__.py
--rw-r--r--   0        0        0       63 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/admin.py
--rw-r--r--   0        0        0      707 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/api.py
--rw-r--r--   0        0        0      308 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/models.py
--rw-r--r--   0        0        0       63 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/views.py
--rw-r--r--   0        0        0     1519 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/Dockerfile
--rw-r--r--   0        0        0     1865 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/Dockerfile.backup
--rw-r--r--   0        0        0      291 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/README.md
--rw-r--r--   0        0        0     1136 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/create_docker.py
--rw-r--r--   0        0        0      111 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/docker-compose.yml
--rw-r--r--   0        0        0      245 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/install_env.sh
--rw-r--r--   0        0        0      132 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/run.sh
--rw-r--r--   0        0        0     4248 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/main.py
--rw-r--r--   0        0        0      106 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/pytest.ini
--rw-r--r--   0        0        0      459 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_api_instance.py
--rw-r--r--   0        0        0     2383 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_app.py
--rw-r--r--   0        0        0     1394 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_async.py
--rw-r--r--   0        0        0     4386 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_auth.py
--rw-r--r--   0        0        0     2208 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_auth_global.py
--rw-r--r--   0        0        0     1836 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_csrf.py
--rw-r--r--   0        0        0      810 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_django_models.py
--rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/__init__.py
--rw-r--r--   0        0        0     3607 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_auth.py
--rw-r--r--   0        0        0     1326 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_body.py
--rw-r--r--   0        0        0      197 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_index.py
--rw-r--r--   0        0        0     1182 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_path.py
--rw-r--r--   0        0        0     3259 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_query.py
--rw-r--r--   0        0        0     2545 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_enum.py
--rw-r--r--   0        0        0      932 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_inheritance_routers.py
--rw-r--r--   0        0        0     2377 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_lists.py
--rw-r--r--   0        0        0      247 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_misc.py
--rw-r--r--   0        0        0     3397 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_models.py
--rw-r--r--   0        0        0     1742 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_openapi_params.py
--rw-r--r--   0        0        0     2810 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_openapi_schema.py
--rw-r--r--   0        0        0     7643 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_path.py
--rw-r--r--   0        0        0     2168 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_query.py
--rw-r--r--   0        0        0     1410 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_request.py
--rw-r--r--   0        0        0     1985 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_response.py
--rw-r--r--   0        0        0     3783 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_response_multiple.py
--rw-r--r--   0        0        0     1823 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_schema.py
--rw-r--r--   0        0        0      465 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_union.py
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 django-ninja-0.9.7/setup.py
--rw-r--r--   0        0        0      221 1970-01-01 00:00:00.000000 django-ninja-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.coveragerc
+-rw-r--r--   0        0        0       66 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.dockerignore
+-rw-r--r--   0        0        0       89 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      566 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      118 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/dependabot.yml
+-rw-r--r--   0        0        0      748 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      542 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1593 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0       93 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.gitignore
+-rw-r--r--   0        0        0      734 2023-07-12 15:26:29.477943 django_ninja-1.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1286 2023-07-12 15:26:29.477943 django_ninja-1.0a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1086 2023-07-12 15:26:29.477943 django_ninja-1.0a1/LICENSE
+-rw-r--r--   0        0        0      744 2023-07-12 15:26:29.477943 django_ninja-1.0a1/Makefile
+-rw-r--r--   0        0        0     3638 2023-07-12 15:26:29.477943 django_ninja-1.0a1/README.md
+-rw-r--r--   0        0        0       12 2023-07-12 15:26:29.477943 django_ninja-1.0a1/WHATSNEW_V1.md
+-rw-r--r--   0        0        0       44 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/extra.css
+-rw-r--r--   0        0        0     2086 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/api-docs.md
+-rw-r--r--   0        0        0     6727 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/async-support.md
+-rw-r--r--   0        0        0     5175 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/authentication.md
+-rw-r--r--   0        0        0     2839 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/errors.md
+-rw-r--r--   0        0        0     4727 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/body.md
+-rw-r--r--   0        0        0     2179 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/file-params.md
+-rw-r--r--   0        0        0     7504 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/filtering.md
+-rw-r--r--   0        0        0     1847 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/form-params.md
+-rw-r--r--   0        0        0     1188 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/operations.md
+-rw-r--r--   0        0        0     4150 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/path-params.md
+-rw-r--r--   0        0        0     3074 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/query-params.md
+-rw-r--r--   0        0        0     1726 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/input/request-parsers.md
+-rw-r--r--   0        0        0     2297 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/config-pydantic.md
+-rw-r--r--   0        0        0     2877 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/django-pydantic-create-schema.md
+-rw-r--r--   0        0        0     2788 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/django-pydantic.md
+-rw-r--r--   0        0        0    11726 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/index.md
+-rw-r--r--   0        0        0     5230 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/pagination.md
+-rw-r--r--   0        0        0     3245 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/response-renderers.md
+-rw-r--r--   0        0        0     1436 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/response/temporal_response.md
+-rw-r--r--   0        0        0     4859 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/routers.md
+-rw-r--r--   0        0        0     1761 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/urls.md
+-rw-r--r--   0        0        0     1498 2023-07-12 15:26:29.477943 django_ninja-1.0a1/docs/docs/guides/versioning.md
+-rw-r--r--   0        0        0     1502 2023-07-12 15:26:29.481943 django_ninja-1.0a1/docs/docs/help.md
+-rw-r--r--   0        0        0    28154 2023-07-12 15:26:29.481943 django_ninja-1.0a1/docs/docs/img/auth-swagger-ui-prompt.png
+-rw-r--r--   0        0        0    27900 2023-07-12 15:26:29.481943 django_ninja-1.0a1/docs/docs/img/auth-swagger-ui.png
+-rw-r--r--   0        0        0    51900 2023-07-12 15:26:29.481943 django_ninja-1.0a1/docs/docs/img/benchmark.png
+-rw-r--r--   0        0        0   654914 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/body-editor.gif
+-rw-r--r--   0        0        0    46786 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0    55925 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0    44459 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/deprecated.png
+-rw-r--r--   0        0        0     2717 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/docs-logo.png
+-rw-r--r--   0        0        0     6234 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/favicon.png
+-rw-r--r--   0        0        0     3439 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/github-star.png
+-rw-r--r--   0        0        0    18865 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/hero.png
+-rw-r--r--   0        0        0    95509 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/index-swagger-ui.png
+-rw-r--r--   0        0        0    12028 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/logo-big.png
+-rw-r--r--   0        0        0   122725 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/nested-routers-swagger.png
+-rw-r--r--   0        0        0    45259 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/operation_description.png
+-rw-r--r--   0        0        0    53995 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/operation_description_docstring.png
+-rw-r--r--   0        0        0    28482 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/operation_summary.png
+-rw-r--r--   0        0        0    22627 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/operation_summary_default.png
+-rw-r--r--   0        0        0    48354 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/operation_tags.png
+-rw-r--r--   0        0        0    25489 2023-07-12 15:26:29.485943 django_ninja-1.0a1/docs/docs/img/servers.png
+-rw-r--r--   0        0        0    65000 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/img/simple-routers-swagger.png
+-rw-r--r--   0        0        0   115803 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/img/tutorial-path-swagger.png
+-rw-r--r--   0        0        0     3692 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/index.md
+-rw-r--r--   0        0        0     3453 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/motivation.md
+-rw-r--r--   0        0        0     4697 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/proposals/cbv.md
+-rw-r--r--   0        0        0      457 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/proposals/index.md
+-rw-r--r--   0        0        0      912 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/proposals/v1.md
+-rw-r--r--   0        0        0       94 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/pydantic-migration.md
+-rw-r--r--   0        0        0      110 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/reference/api.md
+-rw-r--r--   0        0        0      922 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/reference/csrf.md
+-rw-r--r--   0        0        0      307 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/reference/management-commands.md
+-rw-r--r--   0        0        0     6713 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/reference/operations-parameters.md
+-rw-r--r--   0        0        0      115 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/reference/settings.md
+-rw-r--r--   0        0        0      119 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/releases.md
+-rw-r--r--   0        0        0     1778 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/tutorial/index.md
+-rw-r--r--   0        0        0     6703 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/tutorial/other/crud.md
+-rw-r--r--   0        0        0      559 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/tutorial/other/video.md
+-rw-r--r--   0        0        0     3445 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/tutorial/step2.md
+-rw-r--r--   0        0        0     1400 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/docs/tutorial/step3.md
+-rw-r--r--   0        0        0     2790 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/mkdocs.yml
+-rw-r--r--   0        0        0      104 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/requirements.txt
+-rw-r--r--   0        0        0      274 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/index001.py
+-rw-r--r--   0        0        0      442 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/apikey01.py
+-rw-r--r--   0        0        0      322 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/apikey02.py
+-rw-r--r--   0        0        0      298 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/apikey03.py
+-rw-r--r--   0        0        0      314 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/basic01.py
+-rw-r--r--   0        0        0      271 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/bearer01.py
+-rw-r--r--   0        0        0      547 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/bearer02.py
+-rw-r--r--   0        0        0      198 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/code001.py
+-rw-r--r--   0        0        0      231 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/code002.py
+-rw-r--r--   0        0        0      542 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/global01.py
+-rw-r--r--   0        0        0      390 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/multiple01.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/authentication/schema01.py
+-rw-r--r--   0        0        0      195 2023-07-12 15:26:29.489943 django_ninja-1.0a1/docs/src/tutorial/body/code01.py
+-rw-r--r--   0        0        0      255 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/body/code02.py
+-rw-r--r--   0        0        0      272 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/body/code03.py
+-rw-r--r--   0        0        0      213 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/form/code01.py
+-rw-r--r--   0        0        0      288 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/form/code02.py
+-rw-r--r--   0        0        0      676 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/form/code03.py
+-rw-r--r--   0        0        0       94 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/path/code01.py
+-rw-r--r--   0        0        0      325 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/path/code010.py
+-rw-r--r--   0        0        0       99 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/path/code02.py
+-rw-r--r--   0        0        0      208 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/query/code01.py
+-rw-r--r--   0        0        0      367 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/query/code010.py
+-rw-r--r--   0        0        0      259 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/query/code02.py
+-rw-r--r--   0        0        0      157 2023-07-12 15:26:29.493943 django_ninja-1.0a1/docs/src/tutorial/query/code03.py
+-rw-r--r--   0        0        0      436 2023-07-12 15:26:29.493943 django_ninja-1.0a1/mypy.ini
+-rw-r--r--   0        0        0      614 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/compatibility/__init__.py
+-rw-r--r--   0        0        0     1734 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/compatibility/datastructures.py
+-rw-r--r--   0        0        0     1467 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/compatibility/request.py
+-rw-r--r--   0        0        0     1042 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/compatibility/util.py
+-rw-r--r--   0        0        0     1097 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/conf.py
+-rw-r--r--   0        0        0      344 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/constants.py
+-rw-r--r--   0        0        0     1274 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/decorators.py
+-rw-r--r--   0        0        0     2821 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/errors.py
+-rw-r--r--   0        0        0      903 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/files.py
+-rw-r--r--   0        0        0     4063 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/filter_schema.py
+-rw-r--r--   0        0        0    18510 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/main.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     2657 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/management/commands/export_openapi_schema.py
+-rw-r--r--   0        0        0     1887 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/management/utils.py
+-rw-r--r--   0        0        0       70 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/openapi/__init__.py
+-rw-r--r--   0        0        0    13884 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/openapi/schema.py
+-rw-r--r--   0        0        0     1175 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/openapi/urls.py
+-rw-r--r--   0        0        0     2474 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/openapi/views.py
+-rw-r--r--   0        0        0    15205 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/operation.py
+-rw-r--r--   0        0        0      132 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/orm/__init__.py
+-rw-r--r--   0        0        0     5660 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/orm/factory.py
+-rw-r--r--   0        0        0     5792 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/orm/fields.py
+-rw-r--r--   0        0        0     2961 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/orm/metaclass.py
+-rw-r--r--   0        0        0      554 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/orm/shortcuts.py
+-rw-r--r--   0        0        0     6913 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/pagination.py
+-rw-r--r--   0        0        0     2650 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/params.py
+-rw-r--r--   0        0        0     7249 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/params_functions.py
+-rw-r--r--   0        0        0     5513 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/params_models.py
+-rw-r--r--   0        0        0      710 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/parser.py
+-rw-r--r--   0        0        0        1 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/py.typed
+-rw-r--r--   0        0        0      781 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/renderers.py
+-rw-r--r--   0        0        0     1142 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/responses.py
+-rw-r--r--   0        0        0    12705 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/router.py
+-rw-r--r--   0        0        0     7675 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/schema.py
+-rw-r--r--   0        0        0      456 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/security/__init__.py
+-rw-r--r--   0        0        0     1841 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/security/apikey.py
+-rw-r--r--   0        0        0     1109 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/security/base.py
+-rw-r--r--   0        0        0     2756 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/security/http.py
+-rw-r--r--   0        0        0      960 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/security/session.py
+-rw-r--r--   0        0        0      134 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/signature/__init__.py
+-rw-r--r--   0        0        0    12568 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/signature/details.py
+-rw-r--r--   0        0        0     2948 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/signature/utils.py
+-rw-r--r--   0        0        0     6234 2023-07-12 15:26:29.493943 django_ninja-1.0a1/ninja/static/ninja/favicon.png
+-rw-r--r--   0        0        0  1042511 2023-07-12 15:26:29.501943 django_ninja-1.0a1/ninja/static/ninja/redoc.standalone.js
+-rw-r--r--   0        0        0  3726289 2023-07-12 15:26:29.517943 django_ninja-1.0a1/ninja/static/ninja/redoc.standalone.js.map
+-rw-r--r--   0        0        0  1061579 2023-07-12 15:26:29.525943 django_ninja-1.0a1/ninja/static/ninja/swagger-ui-bundle.js
+-rw-r--r--   0        0        0  1540291 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/static/ninja/swagger-ui-bundle.js.map
+-rw-r--r--   0        0        0      570 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/static/ninja/swagger-ui-init.js
+-rw-r--r--   0        0        0   144966 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/static/ninja/swagger-ui.css
+-rw-r--r--   0        0        0   251179 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/static/ninja/swagger-ui.css.map
+-rw-r--r--   0        0        0      308 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/templates/ninja/redoc.html
+-rw-r--r--   0        0        0      341 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/templates/ninja/redoc_cdn.html
+-rw-r--r--   0        0        0      615 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/templates/ninja/swagger.html
+-rw-r--r--   0        0        0      959 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/templates/ninja/swagger_cdn.html
+-rw-r--r--   0        0        0      106 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/testing/__init__.py
+-rw-r--r--   0        0        0     6060 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/testing/client.py
+-rw-r--r--   0        0        0      313 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/types.py
+-rw-r--r--   0        0        0     1940 2023-07-12 15:26:29.533943 django_ninja-1.0a1/ninja/utils.py
+-rw-r--r--   0        0        0     2698 2023-07-12 15:26:29.533943 django_ninja-1.0a1/pyproject.toml
+-rwxr-xr-x   0        0        0      109 2023-07-12 15:26:29.533943 django_ninja-1.0a1/scripts/build-docs.sh
+-rw-r--r--   0        0        0      610 2023-07-12 15:26:29.533943 django_ninja-1.0a1/setup.py
+-rw-r--r--   0        0        0      436 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/demo/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/demo/asgi.py
+-rw-r--r--   0        0        0     1638 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/demo/settings.py
+-rw-r--r--   0        0        0     1040 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/demo/urls.py
+-rw-r--r--   0        0        0      425 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/demo/wsgi.py
+-rwxr-xr-x   0        0        0      657 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/manage.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/__init__.py
+-rw-r--r--   0        0        0     5468 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/api.py
+-rw-r--r--   0        0        0      424 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/asgi.py
+-rw-r--r--   0        0        0      700 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/manage.py
+-rw-r--r--   0        0        0     2190 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/settings.py
+-rw-r--r--   0        0        0      225 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/urls.py
+-rw-r--r--   0        0        0      424 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/multi_param/wsgi.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/someapp/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/someapp/admin.py
+-rw-r--r--   0        0        0      839 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/someapp/api.py
+-rw-r--r--   0        0        0      495 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/someapp/models.py
+-rw-r--r--   0        0        0       63 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/demo_project/someapp/views.py
+-rw-r--r--   0        0        0     1519 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/Dockerfile
+-rw-r--r--   0        0        0     1865 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/Dockerfile.backup
+-rw-r--r--   0        0        0      292 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/README.md
+-rw-r--r--   0        0        0     1136 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/create_docker.py
+-rw-r--r--   0        0        0      111 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/docker-compose.yml
+-rw-r--r--   0        0        0      245 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/install_env.sh
+-rw-r--r--   0        0        0      132 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/env-matrix/run.sh
+-rw-r--r--   0        0        0     6709 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/main.py
+-rw-r--r--   0        0        0      106 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/pytest.ini
+-rw-r--r--   0        0        0      964 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_alias.py
+-rw-r--r--   0        0        0     1313 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_api_instance.py
+-rw-r--r--   0        0        0     2954 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_app.py
+-rw-r--r--   0        0        0     1400 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_async.py
+-rw-r--r--   0        0        0     6994 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_auth.py
+-rw-r--r--   0        0        0     4193 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_auth_async.py
+-rw-r--r--   0        0        0     2213 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_auth_global.py
+-rw-r--r--   0        0        0     1509 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_auth_inheritance_routers.py
+-rw-r--r--   0        0        0     1220 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_auth_routers.py
+-rw-r--r--   0        0        0      909 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_body.py
+-rw-r--r--   0        0        0      196 2023-07-12 15:26:29.533943 django_ninja-1.0a1/tests/test_conf.py
+-rw-r--r--   0        0        0     4062 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_csrf.py
+-rw-r--r--   0        0        0     1798 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_csrf_async.py
+-rw-r--r--   0        0        0     1499 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_decorators.py
+-rw-r--r--   0        0        0     1120 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_django_models.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/__init__.py
+-rw-r--r--   0        0        0     3738 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_auth.py
+-rw-r--r--   0        0        0     1373 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_body.py
+-rw-r--r--   0        0        0     1597 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_form.py
+-rw-r--r--   0        0        0      201 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_index.py
+-rw-r--r--   0        0        0     1583 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_path.py
+-rw-r--r--   0        0        0     4239 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_docs/test_query.py
+-rw-r--r--   0        0        0     4332 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_enum.py
+-rw-r--r--   0        0        0     2522 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1776 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_export_openapi_schema.py
+-rw-r--r--   0        0        0     4390 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_files.py
+-rw-r--r--   0        0        0     5953 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_filter_schema.py
+-rw-r--r--   0        0        0     2308 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_forms.py
+-rw-r--r--   0        0        0     1696 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_forms_and_files.py
+-rw-r--r--   0        0        0     2548 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_inheritance_routers.py
+-rw-r--r--   0        0        0     3336 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_lists.py
+-rw-r--r--   0        0        0     1398 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_misc.py
+-rw-r--r--   0        0        0     3317 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_models.py
+-rw-r--r--   0        0        0     1399 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_openapi_extra.py
+-rw-r--r--   0        0        0     3295 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_openapi_params.py
+-rw-r--r--   0        0        0    26165 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_openapi_schema.py
+-rw-r--r--   0        0        0     4396 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_orm_metaclass.py
+-rw-r--r--   0        0        0      978 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_orm_relations.py
+-rw-r--r--   0        0        0    18936 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_orm_schemas.py
+-rw-r--r--   0        0        0     7625 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_pagination.py
+-rw-r--r--   0        0        0     1511 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_pagination_router.py
+-rw-r--r--   0        0        0     1146 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_parser.py
+-rw-r--r--   0        0        0    11072 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_path.py
+-rw-r--r--   0        0        0      879 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_pydantic_migrate.py
+-rw-r--r--   0        0        0     2550 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_query.py
+-rw-r--r--   0        0        0     3694 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_query_schema.py
+-rw-r--r--   0        0        0     2799 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_renderer.py
+-rw-r--r--   0        0        0     1868 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_request.py
+-rw-r--r--   0        0        0     4089 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_response.py
+-rw-r--r--   0        0        0      544 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_response_cookies.py
+-rw-r--r--   0        0        0     5066 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_response_multiple.py
+-rw-r--r--   0        0        0     1281 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_response_params.py
+-rw-r--r--   0        0        0      323 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_reverse.py
+-rw-r--r--   0        0        0     2791 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_router_path_params.py
+-rw-r--r--   0        0        0     4430 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_schema.py
+-rw-r--r--   0        0        0      618 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_schema_context.py
+-rw-r--r--   0        0        0     1156 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_server.py
+-rw-r--r--   0        0        0     1791 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_signature_details.py
+-rw-r--r--   0        0        0     2694 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_test_client.py
+-rw-r--r--   0        0        0      560 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_union.py
+-rw-r--r--   0        0        0     1223 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-body-file.json
+-rw-r--r--   0        0        0     2334 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-body-form-file.json
+-rw-r--r--   0        0        0     2159 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-body-form.json
+-rw-r--r--   0        0        0     1361 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-body.json
+-rw-r--r--   0        0        0     2643 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-cookie.json
+-rw-r--r--   0        0        0     1596 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-form-body-file.json
+-rw-r--r--   0        0        0     1421 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-form-body.json
+-rw-r--r--   0        0        0     2362 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-form-file.json
+-rw-r--r--   0        0        0     2192 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-form.json
+-rw-r--r--   0        0        0     2540 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-header.json
+-rw-r--r--   0        0        0     2516 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-path.json
+-rw-r--r--   0        0        0     2528 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-query.json
+-rw-r--r--   0        0        0     5447 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_with_django/test_multi_param_parsing.py
+-rw-r--r--   0        0        0     2605 2023-07-12 15:26:29.537943 django_ninja-1.0a1/tests/test_wraps.py
+-rw-r--r--   0        0        0     6267 1970-01-01 00:00:00.000000 django_ninja-1.0a1/PKG-INFO
```

### Comparing `django-ninja-0.9.7/CONTRIBUTING.md` & `django_ninja-1.0a1/CONTRIBUTING.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,42 +11,76 @@
 Once you have it - to install all dependencies required for development and testing  use this command:
 
 
 ```
 flit install --deps develop --symlink
 ```
 
- Once done you can check if all works with 
- 
- ```
- pytest .
- ```
- 
- 
- Now you are ready to make your contribution
- 
- 
- When you done:
- 
- Please make sure you made tests to cover your functionality 
- 
- and finally check the resulting coverage of your contribution did not suffer
- 
- ```
- pytest --cov=ninja --cov-report term-missing tests
- ```
+Once done you can check if all works with 
+
+```
+pytest .
+```
+
+or using Makefile:
+
+```
+make test
+```
+
+Now you are ready to make your contribution
+
+
+When you done:
+
+Please make sure you made tests to cover your functionality 
+
+and finally check the resulting coverage of your contribution did not suffer
+
+```
+pytest --cov=ninja --cov-report term-missing tests
+```
+
+or using Makefile:
+
+```
+make test-cov
+```
  
 ## Code style
 
-Django Ninja uses `black` for style check
+Django Ninja uses `black`, `ruff`, and `mypy` for style checks.
+
+Run `pre-commit install` to create a git hook to fix your styles before you commit.
+
+Alternatively, manually check your code with:
+
+```
+black --check ninja tests
+ruff ninja tests
+mypy ninja
+```
+
+or using Makefile:
+
+```
+make lint
+```
+
+Or reformat your code with:
+
+```
+black ninja tests
+ruff ninja tests --fix
+```
 
-Before your commit please check/format your code with:
+or using Makefile:
 
 ```
-black ./ninja
+make fmt
 ```
  
 ## Docs
 Please do not forget to document your contribution
 
 Django Ninja uses `mkdocs`:
```

### Comparing `django-ninja-0.9.7/LICENSE` & `django_ninja-1.0a1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 Vitaliy Kucheryaviy
+Copyright (c) 2023 Vitaliy Kucheryaviy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-ninja-0.9.7/README.md` & `django_ninja-1.0a1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,42 @@
+<a href="https://github.com/vitalik/django-ninja/issues/383"><img width="814" alt="SCR-20230123-m1t" src="https://user-images.githubusercontent.com/95222/214056666-585c0479-c122-4cb3-add4-b8844088ccdd.png"></a>
+
+
+
+<a href="https://github.com/vitalik/django-ninja/issues/383">^ Please read ^</a>
+
+
+
+
 <p align="center">
   <a href="https://django-ninja.rest-framework.com/"><img src="https://django-ninja.rest-framework.com/img/logo-big.png"></a>
 </p>
 <p align="center">
     <em>Fast to learn, fast to code, fast to run</em>
 </p>
 
 
 ![Test](https://github.com/vitalik/django-ninja/workflows/Test/badge.svg)
 ![Coverage](https://img.shields.io/codecov/c/github/vitalik/django-ninja)
 [![PyPI version](https://badge.fury.io/py/django-ninja.svg)](https://badge.fury.io/py/django-ninja)
+[![Downloads](https://static.pepy.tech/personalized-badge/django-ninja?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/django-ninja)
 
 # Django Ninja - Fast Django REST Framework
 
-**Django Ninja** is a web framework for building APIs with **Django** and Python 3.6+ based **type hints**.
+**Django Ninja** is a web framework for building APIs with **Django** and Python 3.6+ **type hints**.
 
-**Key features**
 
- - **Easy**: Designed to be easy to use and intuitive.
- - **Fast**: Very high performance thanks to Pydantic and **<a href="https://django-ninja.rest-framework.com/async-support/">async support</a>**. 
- - **Fast to code**: Type hints and automatic docs let's you focus only on business logic.
- - **Standards-based**: Based on the open standards for APIs: **OpenAPI** (previously known as Swagger) and **JSON Schema**.
- - **Django friendly**: (obviously) have good integration with Django core an ORM.
- - **Production ready**: Used by multiple companies on live projects (If you use django-ninja and would like to publish your feedback - please email to ppr.vitaly@gmail.com)
+ **Key features:**
+
+  - **Easy**: Designed to be easy to use and intuitive.
+  - **FAST execution**: Very high performance thanks to **<a href="https://pydantic-docs.helpmanual.io" target="_blank">Pydantic</a>** and **<a href="/docs/docs/guides/async-support.md">async support</a>**.
+  - **Fast to code**: Type hints and automatic docs lets you focus only on business logic.
+  - **Standards-based**: Based on the open standards for APIs: **OpenAPI** (previously known as Swagger) and **JSON Schema**.
+  - **Django friendly**: (obviously) has good integration with the Django core and ORM.
+  - **Production ready**: Used by multiple companies on live projects (If you use django-ninja and would like to publish your feedback, please email ppr.vitaly@gmail.com).
 
 
 
 ![Django Ninja REST Framework](docs/docs/img/benchmark.png)
 
 **Documentation**: https://django-ninja.rest-framework.com
 
@@ -67,27 +78,29 @@
     path("admin/", admin.site.urls),
     path("api/", api.urls),  # <---------- !
 ]
 ```
 
 **That's it !**
 
-And you already have:
- - API that receives HTTP GET request at /api/add
- - Takes, validates and type-casts GET parameters `a` and `b`
- - Decodes to JSON operation result
- - Generates an **OpenAPI schema** for defined operation
+Now you've just created an API that:
+
+ - receives an HTTP GET request at `/api/add`
+ - takes, validates and type-casts GET parameters `a` and `b`
+ - decodes the result to JSON
+ - generates an OpenAPI schema for defined operation
 
 ### Interactive API docs
 
 Now go to <a href="http://127.0.0.1:8000/api/docs" target="_blank">http://127.0.0.1:8000/api/docs</a>
 
-You will see the automatic interactive API documentation (provided by <a href="https://github.com/swagger-api/swagger-ui" target="_blank">Swagger UI</a>):
+You will see the automatic interactive API documentation (provided by <a href="https://github.com/swagger-api/swagger-ui" target="_blank">Swagger UI</a> or <a href="https://github.com/Redocly/redoc" target="_blank">Redoc</a>):
 
 
 ![Swagger UI](docs/docs/img/index-swagger-ui.png)
 
-## Next
+## What next?
 
- - Read full documentation here - **Documentation**: https://django-ninja.rest-framework.com
- - To support this project - just simply give it a star on github. ![github star](docs/docs/img/github-star.png)
- - If you already using django-ninja - please share your feedback to ppr.vitaly@gmail.com
+ - Read the full documentation here - https://django-ninja.rest-framework.com
+ - To support this project, please give star it on Github. ![github star](docs/docs/img/github-star.png)
+ - Share it [via Twitter](https://twitter.com/intent/tweet?text=Check%20out%20Django%20Ninja%20-%20Fast%20Django%20REST%20Framework%20-%20https%3A%2F%2Fdjango-ninja.rest-framework.com)
+ - If you already using django-ninja, please share your feedback to ppr.vitaly@gmail.com
```

#### html2text {}

```diff
@@ -1,33 +1,40 @@
+[SCR-20230123-m1t] ^_Please_read_^
           [https://django-ninja.rest-framework.com/img/logo-big.png]
                    Fast to learn, fast to code, fast to run
 ![Test](https://github.com/vitalik/django-ninja/workflows/Test/badge.svg) !
 [Coverage](https://img.shields.io/codecov/c/github/vitalik/django-ninja) [!
 [PyPI version](https://badge.fury.io/py/django-ninja.svg)](https://
-badge.fury.io/py/django-ninja) # Django Ninja - Fast Django REST Framework
-**Django Ninja** is a web framework for building APIs with **Django** and
-Python 3.6+ based **type hints**. **Key features** - **Easy**: Designed to be
-easy to use and intuitive. - **Fast**: Very high performance thanks to Pydantic
-and **async_support**. - **Fast to code**: Type hints and automatic docs let's
-you focus only on business logic. - **Standards-based**: Based on the open
-standards for APIs: **OpenAPI** (previously known as Swagger) and **JSON
-Schema**. - **Django friendly**: (obviously) have good integration with Django
-core an ORM. - **Production ready**: Used by multiple companies on live
-projects (If you use django-ninja and would like to publish your feedback -
-please email to ppr.vitaly@gmail.com) ![Django Ninja REST Framework](docs/docs/
-img/benchmark.png) **Documentation**: https://django-ninja.rest-framework.com -
--- ## Installation ``` pip install django-ninja ``` ## Usage In your django
-project next to urls.py create new `api.py` file: ```Python from ninja import
-NinjaAPI api = NinjaAPI() @api.get("/add") def add(request, a: int, b: int):
-return {"result": a + b} ``` Now go to `urls.py` and add the following:
-```Python hl_lines="3 7" ... from .api import api urlpatterns = [ path("admin/
-", admin.site.urls), path("api/", api.urls), # <---------- ! ] ``` **That's it
-!** And you already have: - API that receives HTTP GET request at /api/add -
-Takes, validates and type-casts GET parameters `a` and `b` - Decodes to JSON
-operation result - Generates an **OpenAPI schema** for defined operation ###
-Interactive API docs Now go to http://127.0.0.1:8000/api/docs You will see the
-automatic interactive API documentation (provided by Swagger_UI): ![Swagger UI]
-(docs/docs/img/index-swagger-ui.png) ## Next - Read full documentation here -
-**Documentation**: https://django-ninja.rest-framework.com - To support this
-project - just simply give it a star on github. ![github star](docs/docs/img/
-github-star.png) - If you already using django-ninja - please share your
-feedback to ppr.vitaly@gmail.com
+badge.fury.io/py/django-ninja) [![Downloads](https://static.pepy.tech/
+personalized-badge/django-
+ninja?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/
+month)](https://pepy.tech/project/django-ninja) # Django Ninja - Fast Django
+REST Framework **Django Ninja** is a web framework for building APIs with
+**Django** and Python 3.6+ **type hints**. **Key features:** - **Easy**:
+Designed to be easy to use and intuitive. - **FAST execution**: Very high
+performance thanks to **Pydantic** and **async_support**. - **Fast to code**:
+Type hints and automatic docs lets you focus only on business logic. -
+**Standards-based**: Based on the open standards for APIs: **OpenAPI**
+(previously known as Swagger) and **JSON Schema**. - **Django friendly**:
+(obviously) has good integration with the Django core and ORM. - **Production
+ready**: Used by multiple companies on live projects (If you use django-ninja
+and would like to publish your feedback, please email ppr.vitaly@gmail.com). !
+[Django Ninja REST Framework](docs/docs/img/benchmark.png) **Documentation**:
+https://django-ninja.rest-framework.com --- ## Installation ``` pip install
+django-ninja ``` ## Usage In your django project next to urls.py create new
+`api.py` file: ```Python from ninja import NinjaAPI api = NinjaAPI() @api.get
+("/add") def add(request, a: int, b: int): return {"result": a + b} ``` Now go
+to `urls.py` and add the following: ```Python hl_lines="3 7" ... from .api
+import api urlpatterns = [ path("admin/", admin.site.urls), path("api/",
+api.urls), # <---------- ! ] ``` **That's it !** Now you've just created an API
+that: - receives an HTTP GET request at `/api/add` - takes, validates and type-
+casts GET parameters `a` and `b` - decodes the result to JSON - generates an
+OpenAPI schema for defined operation ### Interactive API docs Now go to http://
+127.0.0.1:8000/api/docs You will see the automatic interactive API
+documentation (provided by Swagger_UI or Redoc): ![Swagger UI](docs/docs/img/
+index-swagger-ui.png) ## What next? - Read the full documentation here - https:
+//django-ninja.rest-framework.com - To support this project, please give star
+it on Github. ![github star](docs/docs/img/github-star.png) - Share it [via
+Twitter](https://twitter.com/intent/tweet?text=Check%20out%20Django%20Ninja%20-
+%20Fast%20Django%20REST%20Framework%20-%20https%3A%2F%2Fdjango-ninja.rest-
+framework.com) - If you already using django-ninja, please share your feedback
+to ppr.vitaly@gmail.com
```

### Comparing `django-ninja-0.9.7/docs/docs/async-support.md` & `django_ninja-1.0a1/docs/docs/guides/async-support.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 ## Intro
-Since **version 3.1** Django comes with **async views support**. This allows you run efficiently concurrent views that are network/IO-bound.
+
+Since **version 3.1**, Django comes with **async views support**. This allows you run efficient concurrent views that are network and/or IO bound.
 
 ```
-pip install Django==3.1 django-ninja
+pip install Django>=3.1 django-ninja
 ```
 
 Async views work more efficiently when it comes to:
 
- - calling external APIs over the network
- - executing/waiting for database queries
- - processing disk data
-
-
-**Django Ninja** takes full advantage of async views and makes  working with it very easy.
+- calling external APIs over the network
+- executing/waiting for database queries
+- reading/writing from/to disk drives
 
+**Django Ninja** takes full advantage of async views and makes it very easy to work with them.
 
 ## Quick example
 
 ### Code
 
-Let's take an example - we have an api operation that does some work (currently just sleeps for provided number of seconds) and returns a word
+Let's take an example.  We have an API operation that does some work (currently just sleeps for provided number of seconds) and returns a word:
 
 ```Python hl_lines="5"
 import time
 
 @api.get("/say-after")
 def say_after(request, delay: int, word: str):
     time.sleep(delay)
     return {"saying": word}
 ```
 
-To make this code asynchronous - all you have to do is add **`async`** keyword to a function (and use async aware libraries for work processing - in our case we will replace stdlib `sleep` with `asyncio.sleep`): 
-
+To make this code asynchronous, all you have to do is add the **`async`** keyword to a function (and use async aware libraries for work processing - in our case we will replace the stdlib `sleep` with `asyncio.sleep`):
 
 ```Python hl_lines="1 4 5"
 import asyncio
 
 @api.get("/say-after")
 async def say_after(request, delay: int, word: str):
     await asyncio.sleep(delay)
     return {"saying": word}
 ```
 
 ### Run
 
-To run this code you need an ASGI server like <a href="https://www.uvicorn.org/" target="_blank">Uvicorn</a> or <a href="https://github.com/django/daphne" target="_blank">Daphne</a>. Let's use uvicorn for example:
+To run this code you need an ASGI server like <a href="https://www.uvicorn.org/" target="_blank">Uvicorn</a> or <a href="https://github.com/django/daphne" target="_blank">Daphne</a>. Let's use Uvicorn for, example:
+
+To install Uvicorn, use:
 
-To install uvicorn use:
 ```
 pip install uvicorn
 ```
 
-And now to start the server:
+Then start the server:
 
 ```
 uvicorn your_project.asgi:application --reload
 ```
 
-
 > <small>
 > *Note: replace `your_project` with your project package name*<br>
 > *`--reload` flag used to automatically reload server if you do any changes to the code (do not use on production)*
 > </small>
 
 !!! note
-    You can run async views with `manage.py runserver` but it does not work well with some libraries. So at this time (July 2020) it is recommended to use ASGI servers like Uvicorn or Daphne.
+    You can run async views with `manage.py runserver`, but it does not work well with some libraries, so at this time (July 2020) it is recommended to use ASGI servers like Uvicorn or Daphne.
 
 ### Test
 
-Go to your browser and open <a href="http://127.0.0.1:8000/api/say-after?delay=3&word=hello" target="_blank">http://127.0.0.1:8000/api/say-after?delay=3&word=hello</a> (**delay=3**) - after a 3 seconds wait you should see "hello" message.
-
-But now let's flood this operation with **100 parallel requests**:
+Go to your browser and open <a href="<<<<<<<http://127.0.0.1:8000/api/say-after?delay=3&word=hello>>>>>>>" target="_blank">http://127.0.0.1:8000/api/say-after?delay=3&word=hello</a> (**delay=3**)
+After a 3-second wait you should see the "hello" message.
 
+Now let's flood this operation with **100 parallel requests**:
 
 ```
 ab -c 100 -n 100 "http://127.0.0.1:8000/api/say-after?delay=3&word=hello"
 ```
 
-will result to something like this:
+which will result in something like this:
+
 ```
 Connection Times (ms)
               min  mean[+/-sd] median   max
 Connect:        0    1   1.1      1       4
 Processing:  3008 3063  16.2   3069    3082
 Waiting:     3008 3062  15.7   3068    3079
 Total:       3008 3065  16.3   3070    3083
@@ -94,52 +93,44 @@
   90%   3081
   95%   3082
   98%   3083
   99%   3083
  100%   3083 (longest request)
 ```
 
-Based on the numbers - our service was able to handle each of the 100 concurrent requests with just a little of overhead.
-
-To achieve the same concurrency with wsgi and sync operation you would need to spin f.e. 10 workers with 10 threads each.
+Based on the numbers, our service was able to handle each of the 100 concurrent requests with just a little overhead.
 
+To achieve the same concurrency with WSGI and sync operations you would need to spin up about 10 workers with 10 threads each!
 
 ## Mixing sync and async operations
 
-Keep in mind that you can use **both sync and async operations** in your project - **Django Ninja** will route it automatically:
-
+Keep in mind that you can use **both sync and async operations** in your project, and **Django Ninja** will route it automatically:
 
 ```Python hl_lines="2 7"
 
 @api.get("/say-sync")
 def say_after_sync(request, delay: int, word: str):
     time.sleep(delay)
     return {"saying": word}
 
 @api.get("/say-async")
 async def say_after_async(request, delay: int, word: str):
     await asyncio.sleep(delay)
     return {"saying": word}
 ```
 
-
-
-
 ## Elasticsearch example
 
-Let's take a real life case. For this example let's use latest version of elasticsearch that comes with async support:
-
-
+Let's take a real world use case. For this example, let's use the latest version of Elasticsearch that now comes with async support:
 
 ```
 pip install elasticsearch>=7.8.0
 ```
 
-And now instead of `Elasticsearch` class  use `AsyncElasticsearch` and `await` results:
-
+And now instead of the `Elasticsearch` class, use the `AsyncElasticsearch` class and `await` the results:
 
 ```Python hl_lines="2 7 11 12"
 from ninja import NinjaAPI
 from elasticsearch import AsyncElasticsearch
 
 
 api = NinjaAPI()
@@ -153,70 +144,81 @@
         index="documents", 
         body={"query": {"query_string": {"query": q}}},
         size=20,
     )
     return resp["hits"]
 ```
 
-
 ## Using ORM
 
-Currently (July 2020) Certain key parts of Django are not able to operate safely in an async environment, as they have global state that is not coroutine-aware. These parts of Django are classified as “async-unsafe”, and are protected from execution in an async environment. **The ORM** is the main example, but there are other parts that are also protected in this way.
+Currently, certain key parts of Django are not able to operate safely in an async environment, as they have global state that is not coroutine-aware. These parts of Django are classified as “async-unsafe”, and are protected from execution in an async environment. **The ORM** is the main example, but there are other parts that are also protected in this way.
 
-Learn more about async safety here <a href="https://docs.djangoproject.com/en/3.1/topics/async/#async-safety" target="_blank">https://docs.djangoproject.com/en/3.1/topics/async/#async-safety</a>
+Learn more about async safety here in the <a href="https://docs.djangoproject.com/en/stable/topics/async/#async-safety" target="_blank">official Django docs</a>.
 
-
-So if you do this:
+So, if you do this:
 
 ```Python hl_lines="3"
 @api.get("/blog/{post_id}")
 async def search(request, post_id: int):
     blog = Blog.objects.get(pk=post_id)
     ...
 ```
-It throws an error. Until async ORM is implemented you can use `sync_to_async()` adapter:
+
+it throws an error. Until the async ORM is implemented, you can use the `sync_to_async()` adapter:
 
 ```Python hl_lines="1 3 9"
 from asgiref.sync import sync_to_async
 
 @sync_to_async
 def get_blog(post_id):
     return Blog.objects.get(pk=post_id)
 
 @api.get("/blog/{post_id}")
 async def search(request, post_id: int):
     blog = await get_blog(post_id)
     ...
 ```
 
-or shorter:
+or even shorter:
 
 ```Python hl_lines="3"
 @api.get("/blog/{post_id}")
 async def search(request, post_id: int):
     blog = await sync_to_async(Blog.objects.get)(pk=post_id)
     ...
 ```
 
-There is a common **GOTCHA**: Django querysets are lazy evaluated (database query happens only when you start iterating):
-
-so this will *not work*:
+There is a common **GOTCHA**: Django queryset's are lazily evaluated (database query happens only when you start iterating), so this will **not** work:
 
 ```Python
 all_blogs = await sync_to_async(Blog.objects.all)()
-# it will throw an error later when you try iterate over all_blogs
+# it will throw an error later when you try to iterate over all_blogs
 ...
 ```
 
-Instead - use evaluation (with `list`):
+Instead, use evaluation (with `list`):
 
 ```Python
 all_blogs = await sync_to_async(list)(Blog.objects.all())
 ...
 ```
 
+Since Django **version 4.1**, Django comes with asynchronous versions of ORM operations.
+These eliminate the need to use `sync_to_async` in most cases.
+The async operations have the same names as their sync counterparts but are prepended with *a*. So using
+the example above, you can rewrite it as:
 
+```Python hl_lines="3"
+@api.get("/blog/{post_id}")
+async def search(request, post_id: int):
+    blog = await Blog.objects.aget(pk=post_id)
+    ...
+```
 
+When working with querysets, use `async for` paired with list comprehension:
 
+```Python
+all_blogs = [blog async for blog in Blog.objects.all()]
+...
+```
 
-
-
+Learn more about the async ORM interface in the <a href="https://docs.djangoproject.com/en/4.1/releases/4.1/#asynchronous-orm-interface" target="_blank">official Django docs</a>.
```

### Comparing `django-ninja-0.9.7/docs/docs/help.md` & `django_ninja-1.0a1/docs/docs/help.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Help / Get Help
 
-## Do you like Django Ninja ?
+## Do you like Django Ninja?
 
-If you do like this project - there is a tiny thing you can do to let us know that we are moving in the right direction.
+If you like this project, there is a tiny thing you can do to let us know that we're moving in the right direction.
 
 Simply give django-ninja a <a href="https://github.com/vitalik/django-ninja" target="_blank">star on github</a> <a href="https://github.com/vitalik/django-ninja" target="_blank">![github star](img/github-star.png)</a>
 
-OR share this url on social media: 
+or share this URL on social media: 
 ```
-http://django-ninja.rest-framework.com
+https://django-ninja.rest-framework.com
 ```
+Follow updates on twitter <a href="https://twitter.com/django_ninja">@django_ninja</a>
 
 ## Do you want to help us?
 
-You can inspect our docs for typos and spelling mistakes - and create pull requests or <a href="https://github.com/vitalik/django-ninja/issues" target="_blank">open an issue</a>
+Pull requests are always welcome.
 
-Also you can put to issues suggestions to improve **django ninja**
+You can inspect our docs for typos and spelling mistakes, and create pull requests or <a href="https://github.com/vitalik/django-ninja/issues" target="_blank">open an issue</a>.
+
+If you have any suggestions to improve **Django Ninja**, please create them as <a href="https://github.com/vitalik/django-ninja/issues" target="_blank">issues</a> on GitHub.
 
-Pull requests are always welcome.
 
 ## Do you need help?
 
-Do not hesitate - go to <a href="https://github.com/vitalik/django-ninja/issues" target="_blank">github issues</a> and create your question or describe a problem. Will try to address quickly.
+Do not hesitate.  Go to <a href="https://github.com/vitalik/django-ninja/issues" target="_blank">GitHub issues</a> and describe your question or problem.  We'll attempt to address them quickly.
 
+Join the chat at our <a href="https://discord.gg/dgE4SNUDTB" target="_blank">Discord</a> server.
 
+[Code-on the webdesign and web development company](https://code-on.be/) gives commercial consulting for Django-Ninja. If you are looking for support please contact Code-on and we will be in touch with you soon.
```

#### html2text {}

```diff
@@ -1,9 +1,14 @@
-# Help / Get Help ## Do you like Django Ninja ? If you do like this project -
-there is a tiny thing you can do to let us know that we are moving in the right
+# Help / Get Help ## Do you like Django Ninja? If you like this project, there
+is a tiny thing you can do to let us know that we're moving in the right
 direction. Simply give django-ninja a star_on_github ![github_star](img/github-
-star.png) OR share this url on social media: ``` http://django-ninja.rest-
-framework.com ``` ## Do you want to help us? You can inspect our docs for typos
-and spelling mistakes - and create pull requests or open_an_issue Also you can
-put to issues suggestions to improve **django ninja** Pull requests are always
-welcome. ## Do you need help? Do not hesitate - go to github_issues and create
-your question or describe a problem. Will try to address quickly.
+star.png) or share this URL on social media: ``` https://django-ninja.rest-
+framework.com ``` Follow updates on twitter @django_ninja ## Do you want to
+help us? Pull requests are always welcome. You can inspect our docs for typos
+and spelling mistakes, and create pull requests or open_an_issue. If you have
+any suggestions to improve **Django Ninja**, please create them as issues on
+GitHub. ## Do you need help? Do not hesitate. Go to GitHub_issues and describe
+your question or problem. We'll attempt to address them quickly. Join the chat
+at our Discord server. [Code-on the webdesign and web development company]
+(https://code-on.be/) gives commercial consulting for Django-Ninja. If you are
+looking for support please contact Code-on and we will be in touch with you
+soon.
```

### Comparing `django-ninja-0.9.7/docs/docs/img/auth-swagger-ui-prompt.png` & `django_ninja-1.0a1/docs/docs/img/auth-swagger-ui-prompt.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/auth-swagger-ui.png` & `django_ninja-1.0a1/docs/docs/img/auth-swagger-ui.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/benchmark.png` & `django_ninja-1.0a1/docs/docs/img/benchmark.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/body-editor.gif` & `django_ninja-1.0a1/docs/docs/img/body-editor.gif`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/body-schema-doc.png` & `django_ninja-1.0a1/docs/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/body-schema-doc2.png` & `django_ninja-1.0a1/docs/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/deprecated.png` & `django_ninja-1.0a1/docs/docs/img/deprecated.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/docs-logo.png` & `django_ninja-1.0a1/docs/docs/img/docs-logo.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/favicon.png` & `django_ninja-1.0a1/docs/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/github-star.png` & `django_ninja-1.0a1/docs/docs/img/github-star.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/hero.png` & `django_ninja-1.0a1/docs/docs/img/hero.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/index-swagger-ui.png` & `django_ninja-1.0a1/docs/docs/img/index-swagger-ui.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/logo-big.png` & `django_ninja-1.0a1/docs/docs/img/logo-big.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/nested-routers-swagger.png` & `django_ninja-1.0a1/docs/docs/img/nested-routers-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/operation_description.png` & `django_ninja-1.0a1/docs/docs/img/operation_description.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/operation_description_docstring.png` & `django_ninja-1.0a1/docs/docs/img/operation_description_docstring.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/operation_summary.png` & `django_ninja-1.0a1/docs/docs/img/operation_summary.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/operation_summary_default.png` & `django_ninja-1.0a1/docs/docs/img/operation_summary_default.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/operation_tags.png` & `django_ninja-1.0a1/docs/docs/img/operation_tags.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/simple-routers-swagger.png` & `django_ninja-1.0a1/docs/docs/img/simple-routers-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/img/tutorial-path-swagger.png` & `django_ninja-1.0a1/docs/docs/img/tutorial-path-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/docs/docs/index.md` & `django_ninja-1.0a1/docs/docs/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # Django Ninja - Fast Django REST Framework
 
+<div style="background-color: black; color: red; font-size: 16px; padding: 8px;">
+ RUSSIA INVADED UKRAINE - <a href="https://github.com/vitalik/django-ninja/issues/383">Please read</a>
+</div>
+
+
 ![Django Ninja](img/hero.png)
 
-Django Ninja is a web framework for building APIs with Django and Python 3.6+ based type hints.
+Django Ninja is a web framework for building APIs with Django and Python 3.6+ type hints.
 
-Key features
+Key features:
 
  - **Easy**: Designed to be easy to use and intuitive.
- - **Fast**: Very high performance thanks to Pydantic and **<a href="/async-support/">async support</a>**. 
- - **Fast to code**: Type hints and automatic docs let's you focus only on business logic.
+ - **FAST execution**: Very high performance thanks to **<a href="https://pydantic-docs.helpmanual.io" target="_blank">Pydantic</a>** and **<a href="guides/async-support/">async support</a>**. 
+ - **Fast to code**: Type hints and automatic docs lets you focus only on business logic.
  - **Standards-based**: Based on the open standards for APIs: **OpenAPI** (previously known as Swagger) and **JSON Schema**.
- - **Django friendly**: (obviously) have good integration with Django core an ORM.
- - **Production ready**: Used by multiple companies on live projects (If you use django-ninja and would like to publish your feedback - please email to ppr.vitaly@gmail.com)
+ - **Django friendly**: (obviously) has good integration with the Django core and ORM.
+ - **Production ready**: Used by multiple companies on live projects (If you use Django Ninja and would like to publish your feedback, please email ppr.vitaly@gmail.com).
 
 <a href="https://github.com/vitalik/django-ninja-benchmarks" target="_blank">Benchmarks</a>:
 
 ![Django Ninja REST Framework](img/benchmark.png)
 
 ## Installation
 
 ```
 pip install django-ninja
 ```
 
 ## Quick Example
 
-Start a new django project (or use existing)
+Start a new Django project (or use an existing one)
 ```
 django-admin startproject apidemo
 ```
 
 in `urls.py`
 
 ```Python hl_lines="3 5 8 9 10 15"
@@ -37,81 +42,80 @@
 ```
 
 Now, run it as usual:
 ```
 ./manage.py runserver
 ```
 
-note: you don't have to add django-ninja to your intalled apps.
+Note: You don't have to add Django Ninja to your installed apps for it to work.
 
 ## Check it
 
 Open your browser at <a href="http://127.0.0.1:8000/api/add?a=1&b=2" target="_blank">http://127.0.0.1:8000/api/add?a=1&b=2</a>
 
 You will see the JSON response as:
 ```JSON
 {"result": 3}
 ```
-You already created an API that:
+Now you've just created an API that:
 
- - Receives HTTP GET request at `/api/add`
- - Takes, validates and type-casts GET parameters `a` and `b`
- - Decodes to JSON operation result
- - Generates an OpenAPI schema for defined operation
+ - receives an HTTP GET request at `/api/add`
+ - takes, validates and type-casts GET parameters `a` and `b`
+ - decodes the result to JSON
+ - generates an OpenAPI schema for defined operation
 
 ## Interactive API docs
 
 Now go to <a href="http://127.0.0.1:8000/api/docs" target="_blank">http://127.0.0.1:8000/api/docs</a>
 
-You will see the automatic interactive API documentation (provided by <a href="https://github.com/swagger-api/swagger-ui" target="_blank">Swagger UI</a>):
-
+You will see the automatic, interactive API documentation (provided by the <a href="https://github.com/swagger-api/swagger-ui" target="_blank">OpenAPI / Swagger UI</a> or <a href="https://github.com/Redocly/redoc" target="_blank">Redoc</a>):
 
 ![Swagger UI](img/index-swagger-ui.png)
 
 
 ## Recap
 
-In summary, you declare **once** the types of parameters, body, etc. as function parameters. 
+In summary, you declare the types of parameters, body, etc. **once only**, as function parameters. 
 
 You do that with standard modern Python types.
 
 You don't have to learn a new syntax, the methods or classes of a specific library, etc.
 
 Just standard **Python 3.6+**.
 
 For example, for an `int`:
 
 ```Python
 a: int
 ```
 
-or for a more complex `Item` model:
+or, for a more complex `Item` model:
 
 ```Python
 class Item(Schema):
     foo: str
     bar: float
 
 def operation(a: Item):
     ...
 ```
 
-...and with that single declaration you get:
+... and with that single declaration you get:
 
 * Editor support, including:
-    * Completion.
-    * Type checks.
+    * Completion
+    * Type checks
 * Validation of data:
-    * Automatic and clear errors when the data is invalid.
-    * Validation even for deeply nested JSON objects.
-* <abbr title="also known as: serialization, parsing, marshalling">Conversion</abbr> of input data: coming from the network to Python data and types. Reading from:
-    * JSON.
-    * Path parameters.
-    * Query parameters.
-    * Cookies.
-    * Headers.
-    * Forms.
-    * Files.
-* Automatic interactive API documentation
+    * Automatic and clear errors when the data is invalid
+    * Validation, even for deeply nested JSON objects
+* <abbr title="also known as: serialization, parsing, marshalling">Conversion</abbr> of input data coming from the network, to Python data and types, and reading from:
+    * JSON
+    * Path parameters
+    * Query parameters
+    * Cookies
+    * Headers
+    * Forms
+    * Files
+* Automatic, interactive API documentation
 
 This project was heavily inspired by <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a> (developed by <a href="https://github.com/tiangolo" target="_blank">Sebastián Ramírez</a>)
```

### Comparing `django-ninja-0.9.7/docs/docs/motivation.md` & `django_ninja-1.0a1/docs/docs/motivation.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Motivation
 
 !!! quote
-    **Django Ninja** looks basically the same as **FastAPI**. So, why not just FastAPI?
+    **Django Ninja** looks basically the same as **FastAPI**, so why not just use FastAPI?
 
-Indeed **Django Ninja** is heavily inspired by <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a> (developed by <a href="https://github.com/tiangolo" target="_blank">Sebastián Ramírez</a>)
+Indeed, **Django Ninja** is heavily inspired by <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a> (developed by <a href="https://github.com/tiangolo" target="_blank">Sebastián Ramírez</a>)
 
-But there are few issues when it comes to join FastAPI and Django
+That said, there are few issues when it comes to getting FastAPI and Django to work together properly:
 
-1) **FastAPI** declares to be ORM agnostic (meaning you can use it with SqlAlchemy or DjangoORM). But in reality Django ORM is not yet ready for async use (will be in version 3.2). And if you use it in sync mode - you can have a [closed connection issue](https://github.com/tiangolo/fastapi/issues/716) which you will have to overcome with lot's of crunches.
+1) **FastAPI** declares to be ORM agnostic (meaning you can use it with SQLAlchemy or the Django ORM), but in reality the Django ORM is not yet ready for async use (it may be in version 4.0 or 4.1), and if you use it in sync mode, you can have a [closed connection issue](https://github.com/tiangolo/fastapi/issues/716) which you will have to overcome with a **lot** of effort.
 
-2) The dependency injection with arguments makes your code too much verbose when you rely on authentication and database session in your operations (which for some projects makes it like 99% of all operations)
+2) The dependency injection with arguments makes your code too verbose when you rely on authentication and database sessions in your operations (which for some projects is about 99% of all operations).
 
 ```Python hl_lines="25 26"
 ...
 
 app = FastAPI()
 
 
@@ -38,23 +38,29 @@
         task_id: int,
         db: Session = Depends(get_db), 
         current_user: User = Depends(get_current_user),
     ):
         ... use db with current_user ....
 ```
 
-3) Since word `model` in django is "reserved" for ORM = it becomes very unclear when you mix django orm into Pydantic/FastAPI model naming convention. 
+3) Since the word `model` in Django is "reserved" for use by the ORM, it becomes very confusing when you mix the Django ORM with Pydantic/FastAPI model naming conventions. 
 
 ### Django Ninja
 
-Django Ninja addresses all those issues and includes a great integration with Django (ORM, urls, views, auth and more...)
+Django Ninja addresses all those issues, and integrates very well with Django (ORM, urls, views, auth and more)
+
+Working at [Code-on a Django webdesign webedevelopment studio](https://code-on.be/) I get all sorts of challenges and to solve these I started Django-Ninja in 2020.
+
+Note: **Django Ninja is a production ready project** - my estimation is at this time already 100+ companies using it in production and 500 new developers joining every month. 
+
+Some companies already looking for developers with django ninja experince.
 
 #### Main Features
 
-1) Since you can have multiple NinjaAPI instances - you can run [multiple API versions](/tutorial/versioning) inside one django project
+1) Since you can have multiple Django Ninja API instances - you can run [multiple API versions](/tutorial/versioning) inside one Django project.
 
 ```Python
 api_v1 = NinjaAPI(version='1.0', auth=token_auth)
 ...
 api_v2 = NinjaAPI(version='2.0', auth=token_auth)
 ...
 api_private = NinjaAPI(auth=session_auth, urls_namespace='private_api')
@@ -65,23 +71,23 @@
     ...
     path('api/v1/', api_v1.urls),
     path('api/v2/', api_v2.urls),
     path('internal-api/', api_private.urls),
 ]
 ```
 
-2) Django Ninja Schema - is integrated with ORM so you [can serialize querysets](/tutorial/response-schema/#returning-querysets) or ORM objects:
+2) The Django Ninja 'Schema' class is integrated with the ORM, so you can [serialize querysets](/tutorial/response-schema/#returning-querysets) or ORM objects:
 
 ```Python
 @api.get("/tasks", response=List[TaskSchema])
 def tasks(request):
     return Task.objects.all()
 
 
 @api.get("/tasks", response=TaskSchema)
 def tasks_details(request):
     task = Task.objects.first()
     return task
 ```
-3) Soon you should be able to [create Schema's from Django Models](/proposals/models/)
+3) [Create Schema's from Django Models](/guides/response/django-pydantic/).
 
-4) Instead of dependency arguments **Django Ninja** uses `request` instance attributes (same way as regular django views) - see more details on [Authentication](/tutorial/authentication/)
+4) Instead of dependency arguments, **Django Ninja** uses `request` instance attributes (in the same way as regular Django views) - more detail at [Authentication](/guides/authentication/).
```

### Comparing `django-ninja-0.9.7/docs/docs/proposals/cbv.md` & `django_ninja-1.0a1/docs/docs/proposals/cbv.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Class Based Operations
 
 
 !!! warning ""
-    This is just a proposal and it is **not present in library code**. But eventually this can be a part of Django Ninja.
+    This is just a proposal and it is **not present in library code**, but eventually this can be a part of Django Ninja.
 
     Please consider adding likes/dislikes or comments in [github issue](https://github.com/vitalik/django-ninja/issues/15) to express your feeling about this proposal
 
 
 ## Problem
 
-An API operation is a callable which takes a request and parameters and returns a response. 
-But it is often a case in real world when you need to reuse same pieces of code in multiple operations.
+An API operation is a callable which takes a request and parameters and returns a response, but it is often a case in real world when you need to reuse the same pieces of code in multiple operations.
 
 Let's take the following example:
 
- - We have a TODO application with Projects and Tasks
- - Each project have multiple tasks
- - and as well each project may have an owner(user)
- - other users should not be able to access project they not owe
+ - we have a Todo application with Projects and Tasks
+ - each project has multiple tasks
+ - each project may also have an owner (user)
+ - users should not be able to access projects they do not own
 
 Model structure is something like this:
 
 ```Python
 class Project(models.Model):
     title = models.CharField(max_length=100)
     owner = models.ForeignKey('auth.User', on_delete=models.CASCADE)
@@ -29,21 +28,21 @@
 class Task(models.Model):
     project = models.ForeignKey(Project, on_delete=models.CASCADE)
     title = models.CharField(max_length=100)
     completed = models.BooleanField()
 ```
 
 
-Let's now create few API operations for it:
+Now, let's create a few API operations for it:
 
- - list of tasks for project
- - task details
- - complete task action
+ - a list of tasks for the project
+ - some task details
+ - a 'complete task' action
 
-All should validate that user can only access his/her project's tasks (otherwise return 404)
+The code should validate that a user can only access his/her own project's tasks (otherwise, return 404)
 
 It can be something like this:
 
 
 ```Python
 router = Router()
 
@@ -69,86 +68,79 @@
     task = get_object_or_404(user_tasks, id=task_id)
     task.completed = True
     task.save()
     return task
 ```
 
 
-As you can see - these lines are getting repeated pretty often to check permission:
+As you can see, these lines are getting repeated pretty often to check permission:
 
-```Python hl_lines="1 2 "
+```Python hl_lines="1 2"
 user_projects = request.user.project_set
 project = get_object_or_404(user_projects, id=project_id))
 ```
 
-You can extract it to a function, but it will just make it 3 lines smaller and still be pretty polluted...
+You can extract it to a function, but it will just make it 3 lines smaller, and it will still be pretty polluted ...
 
 
 ## Solution
 
-The proposal is to have alternative called "Class Based Operation" where you can decorate with `path` decorator entire class:
+The proposal is to have alternative called "Class Based Operation" where you can decorate the entire class with a `path` decorator:
 
 
 ```Python hl_lines="7 8"
 from ninja import Router
 
 
 router = Router()
 
 
 @router.path('/project/{project_id}/tasks')
 class Tasks:
-
     def __init__(self, request, project_id=int):
         user_projects = request.user.project_set
         self.project = get_object_or_404(user_projects, id=project_id))
         self.tasks = self.project.task_set.all()
     
-
     @router.get('/', response=List[TaskOut])
     def task_list(self, request):
         return self.tasks
 
     @router.get('/{task_id}/', response=TaskOut)
     def details(self, request, task_id: int):
         return get_object_or_404(self.tasks, id=task_id)
 
-
     @router.post('/{task_id}/complete', response=TaskOut)
     def complete(self, request, task_id: int):
         task = get_object_or_404(self.tasks, id=task_id)
         task.completed = True
         task.save()
         return task
-
 ```
 
-All common initiation and permission check landed in constructor:
-```Python hl_lines="5 6 7"
+All common initiation and permission checks are placed in the constructor:
+
+```Python hl_lines="4 5 6"
 @router.path('/project/{project_id}/tasks')
 class Tasks:
-
     def __init__(self, request, project_id=int):
         user_projects = request.user.project_set
         self.project = get_object_or_404(user_projects, id=project_id))
         self.tasks = self.project.task_set.all()
-    
 ```
-Which made main business operation focus only on tasks (that was exposed as `self.tasks` attribute)
 
-you can use both `api` and `router` instances to support class paths
+This makes the main business operation focus only on tasks (exposed as the `self.tasks` attribute)
+
+You can use both `api` and `router` instances to support class paths.
 
 ## Issue
 
 The `__init__` method:
 
 ```def __init__(self, request, project_id=int):```
 
-Python do not support `async` keyword for `__init__`, so to support async operations - we need some other method for initialization, but `__init__` sounds most logical
+Python doesn't support the `async` keyword for `__init__`, so to support async operations we need some other method for initialization, but `__init__` sounds the most logical.
 
 
 ## Your thoughts/proposals
 
 Please give you thoughts/likes/dislikes about this proposal in the [github issue](https://github.com/vitalik/django-ninja/issues/15)
-
-
-
```

### Comparing `django-ninja-0.9.7/docs/docs/proposals/models.md` & `django_ninja-1.0a1/docs/docs/guides/response/django-pydantic.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,184 +1,108 @@
-# Models to Schemas
+# Schemas from Django models
 
-!!! warning ""
-    This is just a proposal and it is **not present in library code**. But eventually this can be a part of Django Ninja.
 
-    Please consider adding likes/dislikes or comments in [github issue](https://github.com/vitalik/django-ninja/issues/17) to express your feeling about this proposal
+Schemas are very useful to define your validation rules and responses, but sometimes you need to reflect your database models into schemas and keep changes in sync.
 
+## ModelSchema 
 
-## Problem
+`ModelSchema` is a special base class that can automatically generate schemas from your models.
 
-Schemas are very useful to define your validation rules and responses.
+All you need is to set `model` and `model_fields` attributes on your schema `Config`:
 
-But sometimes you need to reflect your database models into schemas and keep changes in sync.
-
-Like if you have model and schema:
-
-```Python
-
-class User(models.Model):
-    email = models.EmailFiled(max_length=100)
-    name = models.CharField(max_length=100, null=True, blank=True)
-
-
-...
-
-class UserOut(Schema):
-    email: str
-    name: str = None
-```
-
-and then you need to extend a database field, you need to not forget to add it to schema as well:
-
-```Python hl_lines="4 11"
-
-class User(models.Model):
-    email = models.EmailFiled(max_length=100)
-    name = models.CharField(max_length=100, null=True, blank=True)
-    birthdate = models.DateField(null=True, blank=True)
-
-...
-
-class UserOut(Schema):
-    email: str
-    name: str = None
-    birthdate: date = None
-
-```
-
-
-
-## Solution
-
-
-### ModelSchema
-
-Introduce a **ModelSchema** that can reflect Django model:
-
-
-```Python
 
+```Python hl_lines="2 5 6 7"
+from django.contrib.auth.models import User
 from ninja import ModelSchema
 
-class UserOut(ModelSchema):
-    class Meta:
+class UserSchema(ModelSchema):
+    class Config:
         model = User
-        fields = ['email', 'name']
+        model_fields = ['id', 'username', 'first_name', 'last_name']
 
-
-# which will create a schema equivalent to:
-
-# class UserOut(Schema):
-#     email: str
-#     name: str = None
+# Will create schema like this:
+# 
+# class UserSchema(Schema):
+#     id: int
+#     username: str
+#     first_name: str
+#     last_name: str
 ```
 
-### Passing all models fields
+### Using ALL model fields
 
-If you want to create schema with **ALL** fields, pass `'__all__'`:
+To use all fields from a model - you can pass `__all__` to `model_fields`:
 
 ```Python hl_lines="4"
-class UserOut(ModelSchema):
-    class Meta:
+class UserSchema(ModelSchema):
+    class Config:
         model = User
-        fields = '__all__'
+        model_fields = "__all__"
 ```
+!!! Warning
+    Using __all__ is not recommended.
+    <br>
+    This can lead to accidental unwanted data exposure (like hashed password, in the above example).
+    <br>
+    General advice - use `model_fields` to explicitly define list of fields that you want to be visible in API.
 
-OR if you want to pass all fields but **exclude** few - use `exclude`:
-
-```Python hl_lines="4"
-class UserOut(ModelSchema):
-    class Meta:
-        model = User
-        exclude = ['birthdate'] 
-        # ^ resulting schema will have only `name` and `email`
-```
-
-
-### Required/Not-required fields
+### Excluding model fields
 
-For some cases you might want to override which fields are **required or not required** in API:
+To use all fields **except** a few, you can use `model_exclude` configuration:
 
-```Python
-class UserCreate(ModelSchema):
-    class Meta:
-        model = User
-        fields = '__all__'
-        required = '__all__'
-
-
-class UserPatch(ModelSchema):
-    class Meta:
+```Python hl_lines="4"
+class UserSchema(ModelSchema):
+    class Config:
         model = User
-        fields = '__all__'
-        not_required = '__all__'
+        model_exclude = ['password', 'last_login', 'user_permissions']
 
-# will result to these schemas:
-#
-# class UserCreate(Schema):
-#     email: str
-#     name: str
-#     birthdate: date
+# Will create schema like this:
 # 
-# class UserPatch(Schema):
-#     email: str = None
-#     name: str = None
-#     birthdate: date = None
+# class UserSchema(Schema):
+#     id: int
+#     username: str
+#     first_name: str
+#     last_name: str
+#     email: str
+#     is_superuser: bool
+#     ... and the rest
 
 ```
 
-You can use `UserPatch` to update only few fields that were provided in request
+### Overriding fields
 
+To change default annotation for some field, or to add a new field, just use annotated attributes as usual. 
 
-### Relational fields
+```Python hl_lines="1 2 3 4 8"
+class GroupSchema(ModelSchema):
+    class Config:
+        model = Group
+        model_fields = ['id', 'name']
 
-If you have fields that are ForeignKey's or ManyToManyField - by default it will map to it's primary keys:
 
-```Python hl_lines="4 5 14 20 21"
-# model 
-class Post():
-    titie = models.CharField(...)
-    owner = models.ForeignKey('auth.User', ...)
-    tags = models.ManyToManyField('blog.Tag', blank=True)
+class UserSchema(ModelSchema):
+    groups: List[GroupSchema] = []
 
-...
+    class Config:
+        model = User
+        model_fields = ['id', 'username', 'first_name', 'last_name']
 
-# schemas
+```
 
-class PostSchema(ModelSchema):
-    class Meta:
-        model = Post
-        fields = '__all__'
 
-# this will produce schema like this:
+### Making fields optional
 
-class PostSchema(ModelSchema):
-    title: str
-    owner: int
-    tags: List[int]
+Pretty often for PATCH API operations you need to make all fields of your schema optional. To do that you can use config model_fields_optional
 
+```Python hl_lines="5"
+class PatchGroupSchema(ModelSchema):
+    class Config:
+        model = Group
+        model_fields = ['id', 'name', 'description'] # Note: all these fields are required on model level
+        model_fields_optional = '__all__'
 ```
 
-If you need to expand to nested models - define needed schemas:
-
-```Python hl_lines="2 3"
-class PostSchema(ModelSchema):
-    owner: UserSchema
-    tags: List[TagSchema]
+also you can define just a few optional fields instead of all:
 
-    class Meta:
-        model = Post
-        fields = '__all__'
 ```
-
-
-## Issues
-
-The issue that by using model generated schemas you will loose that nice IDE support and type checks, but on the other hand you might not use the attributes directly
-
-
-## Your thoughts/proposals
-
-Please give you thoughts/likes/dislikes about this proposal in the [github issue](https://github.com/vitalik/django-ninja/issues/17)
-
-
+     model_fields_optional = ['description']
+```
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/authentication.md` & `django_ninja-1.0a1/docs/docs/guides/authentication.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # Authentication
 
 ## Intro
 
-**Django Ninja** provides several tools to help you deal with authentication and authorization easily, rapidly, in a standard way, without having to study and learn <a href="https://swagger.io/docs/specification/authentication/" target="_blank">all the security specifications</a>.
+**Django Ninja** provides several tools to help you deal with authentication and authorization easily, rapidly, in a standard way, and without having to study and learn <a href="https://swagger.io/docs/specification/authentication/" target="_blank">all the security specifications</a>.
 
-The core concept is that when you describe an api operation you can define an authentication object
+The core concept is that when you describe an API operation, you can define an authentication object.
 
 ```Python hl_lines="2 7"
 {!./src/tutorial/authentication/code001.py!}
 ```
 
-In this example client will be able to call the `pets` method only if it uses django session authentication (default is cookie based). Otherwise, a HTTP-401 error will be returned.
+In this example, the client will only be able to call the `pets` method if it uses Django session authentication (the default is cookie based), otherwise an HTTP-401 error will be returned.
 
-## Automatic Openapi schema
+If you need to authorize only a superuser, you can use `from ninja.security import django_auth_superuser` instead.
 
-Let's create an example where client in order to authenticate needs to pass a header :
+## Automatic OpenAPI schema
+
+Here's an example where the client, in order to authenticate, needs to pass a header:
 
 `Authorization: Bearer supersecret`
 
 ```Python hl_lines="4 5 6 7 10"
 {!./src/tutorial/authentication/bearer01.py!}
 ```
 
-Now go to docs at <a href="http://localhost:8000/api/docs" target="_blank">http://localhost:8000/api/docs</a>:
+Now go to the docs at <a href="http://localhost:8000/api/docs" target="_blank">http://localhost:8000/api/docs</a>.
 
 
 ![Swagger UI Auth](../img/auth-swagger-ui.png)
 
-When you click **Authorize** button you will get a prompt to input your authentication token
+Now, when you click the **Authorize** button, you will get a prompt to input your authentication token.
 
 ![Swagger UI Auth](../img/auth-swagger-ui-prompt.png)
 
-Now if you do test calls - the Authorization header will passed for every request.
+When you do test calls, the Authorization header will be passed for every request.
 
 
-## Global authentication 
+## Global authentication
 
-In case you need to secure **all** methods of your api - you can pass `auth` argument to a `NinjaAPI` constructor:
+In case you need to secure **all** methods of your API, you can pass the `auth` argument to the `NinjaAPI` constructor:
 
 
 ```Python hl_lines="11 19"
 from ninja import NinjaAPI, Form
 from ninja.security import HttpBearer
 
 
@@ -55,35 +57,35 @@
 # @api.get(...)
 # def ...
 
 # @api.post(...)
 # def ...
 ```
 
-And if you need to overrule some of those methods you can do that on the operation level again by passing the `auth` argument. In this example authentication will be disabled for `/token` operation:
+And, if you need to overrule some of those methods, you can do that on the operation level again by passing the `auth` argument. In this example, authentication will be disabled for the `/token` operation:
 
 ```Python hl_lines="19"
 {!./src/tutorial/authentication/global01.py!}
 ```
 
 ## Available auth options
 
 ### Custom function
 
 
-The "`auth=`" argument accepts any Callable object. **NinjaAPI** passes authentication only if callable object returns a **not None** value. This return value will be assigned to `request.auth` attribute.
+The "`auth=`" argument accepts any Callable object. **NinjaAPI** passes authentication only if the callable object returns a value that can be **converted to boolean True**. This return value will be assigned to the `request.auth` attribute.
 
 ```Python hl_lines="1 2 3 6"
 {!./src/tutorial/authentication/code002.py!}
 ```
 
 
 ### API Key
 
-Some APIs use API keys for authorization. An API key is a token that a client provides when making API calls. The key can be sent in the query string:
+Some API's use API keys for authorization. An API key is a token that a client provides when making API calls to identify itself. The key can be sent in the query string:
 ```
 GET /something?api_key=abcdef12345
 ```
 
 or as a request header:
 
 ```
@@ -94,26 +96,26 @@
 or as a cookie:
 
 ```
 GET /something HTTP/1.1
 Cookie: X-API-KEY=abcdef12345
 ```
 
-Django Ninja comes with builtin classes to help you handle these cases.
+**Django Ninja** comes with built-in classes to help you handle these cases.
 
 
 #### in Query
 
 ```Python hl_lines="1 2 5 6 7 8 9 10 11 12"
 {!./src/tutorial/authentication/apikey01.py!}
 ```
 
-In this example we take a token from `GET['api_key']` and find a `Client` in database that corresponds to this key. The Client instance will be set to `request.auth` attribute
+In this example we take a token from `GET['api_key']` and find a `Client` in the database that corresponds to this key. The Client instance will be set to the `request.auth` attribute.
 
-Note: **`param_name`** - is the name of GET parameter that will be checked for. If not set - default "`key`" will be used.
+Note: **`param_name`** is the name of the GET parameter that will be checked for. If not set, the default of "`key`" will be used.
 
 
 #### in Header
 
 ```Python hl_lines="1 4"
 {!./src/tutorial/authentication/apikey02.py!}
 ```
@@ -137,16 +139,57 @@
 ```Python hl_lines="1 4 5 6 7"
 {!./src/tutorial/authentication/basic01.py!}
 ```
 
 
 ## Multiple authenticators
 
-The **`auth`** argument allows also to pass multiple authenticators:
+The **`auth`** argument also allows you to pass multiple authenticators:
 
 ```Python hl_lines="18"
 {!./src/tutorial/authentication/multiple01.py!}
 ```
 
-In this case **Django Ninja** will first check the api key `GET`, and if not set or invalid will check the `header` key. And if both invalid will raise authentication error to response.
+In this case **Django Ninja** will first check the API key `GET`, and if not set or invalid will check the `header` key.
+If both are invalid, it will raise an authentication error to the response.
+
+
+## Router authentication
+
+Use `auth` argument on Router to apply authenticator to all operations declared in it:
+
+```Python
+api.add_router("/events/", events_router, auth=BasicAuth())
+```
+
+or using router constructor
+```Python
+router = Router(auth=BasicAuth())
+```
+
+
+## Custom exceptions
+
+Raising an exception that has an exception handler will return the response from that handler in
+the same way an operation would:
+
+```Python hl_lines="1 4"
+{!./src/tutorial/authentication/bearer02.py!}
+```
+
+
+## Async authentication
+
+**Django Ninja** has basic support for asynchronous authentication. While the default authentication classes are not async-compatible, you can still define your custom asynchronous authentication callables and pass them in using `auth`.
+
+```python
+async def async_auth(request):
+    ...
+
+
+@api.get("/pets", auth=async_auth)
+def pets(request):
+    ...
+```
 
 
+See [Handling errors](errors.md) for more information.
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/body.md` & `django_ninja-1.0a1/docs/docs/guides/input/body.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Request Body
 
-Request bodies are typically used with “create” and “update” operations (POST, PUT, PATCH). For example, when creating a resource using POST or PUT, the request body usually contains the representation of the resource to be created.
+Request bodies are typically used with “create” and “update” operations (POST, PUT, PATCH).
+For example, when creating a resource using POST or PUT, the request body usually contains the representation of the resource to be created.
 
-To declare a **request body**, you need to use **NinjaAPI `Schema`**.
+To declare a **request body**, you need to use **Django Ninja `Schema`**.
 
 !!! info
-    Under the hood **NinjaAPI** uses <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> models with all their power and benefits.
-    The alias `Schema` was picked to avoid confusion in code with Django models.
+    Under the hood **Django Ninja** uses <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> models with all their power and benefits.
+    The alias `Schema` was chosen to avoid confusion in code when using Django models, as Pydantic's model class is called Model by default, and conflicts with Django's Model class.
 
 ## Import Schema
 
 First, you need to import `Schema` from `ninja`:
 
 ```Python hl_lines="1"
 {!./src/tutorial/body/code01.py!}
@@ -22,15 +23,15 @@
 
 Use standard Python types for all the attributes:
 
 ```Python hl_lines="4 5 6 7 8"
 {!./src/tutorial/body/code01.py!}
 ```
 
-Note: if you use **`None`** as default value for an attribute - it will become optional in the request body.
+Note: if you use **`None`** as the default value for an attribute, it will become optional in the request body.
 For example, this model above declares a JSON "`object`" (or Python `dict`) like:
 
 ```JSON
 {
     "name": "Katana",
     "description": "An optional description",
     "price": 299.00,
@@ -46,55 +47,57 @@
     "price": 299.00,
     "quantity": 10
 }
 ```
 
 ## Declare it as a parameter
 
-To add it to your *path operation*, declare it the same way you declared path and query parameters:
+To add it to your *path operation*, declare it the same way you declared the path and query parameters:
 
 ```Python hl_lines="12"
 {!./src/tutorial/body/code01.py!}
 ```
 
-...and declare its type as the model you created, `Item`.
+... and declare its type as the model you created, `Item`.
 
 ## Results
 
-With just that Python type declaration, **NinjaAPI** will:
+With just that Python type declaration, **Django Ninja** will:
 
 * Read the body of the request as JSON.
 * Convert the corresponding types (if needed).
 * Validate the data.
-    * If the data is invalid, it will return a nice and clear error, indicating exactly where and what was the incorrect data.
+    * If the data is invalid, it will return a nice and meaningful error, indicating exactly where and what the incorrect data was.
 * Give you the received data in the parameter `item`.
-    * As you declared it in the function to be of type `Item`, you will also have all the editor support (completion, etc) for all of the attributes and their types.
-* Generate <a href="http://json-schema.org" class="external-link" target="_blank">JSON Schema</a> definitions for your model, you can also use them anywhere else you like if it makes sense for your project.
-* Those schemas will be part of the generated OpenAPI schema, and used by the automatic documentation <abbr title="User Interfaces">UIs</abbr>.
+    * Because you declared it in the function to be of type `Item`, you will also have all the editor support
+      (completion, etc.) for all the attributes and their types.
+* Generate <a href="https://json-schema.org" class="external-link" target="_blank">JSON Schema</a> definitions for
+  your models, and you can also use them anywhere else you like if it makes sense for your project.
+* Those schemas will be part of the generated OpenAPI schema, and used by the automatic documentation <abbr title="User Interfaces">UI's</abbr>.
 
 ## Automatic docs
 
 The JSON Schemas of your models will be part of your OpenAPI generated schema, and will be shown in the interactive API docs:
 
-![Openapi schema](../img/body-schema-doc.png)
+![Openapi schema](../../img/body-schema-doc.png)
 
-And will be also used in the API docs inside each *path operation* that needs them:
+... and they will be also used in the API docs inside each *path operation* that needs them:
 
-![Openapi schema](../img/body-schema-doc2.png)
+![Openapi schema](../../img/body-schema-doc2.png)
 
 ## Editor support
 
 In your editor, inside your function you will get type hints and completion everywhere (this wouldn't happen if you received a `dict` instead of a Schema object):
 
-![Type hints](../img/body-editor.gif)
+![Type hints](../../img/body-editor.gif)
 
 
 The previous screenshots were taken with <a href="https://code.visualstudio.com" class="external-link" target="_blank">Visual Studio Code</a>.
 
-But you would get the same editor support with <a href="https://www.jetbrains.com/pycharm/" class="external-link" target="_blank">PyCharm</a> and most of the other Python editors.
+You would get the same editor support with <a href="https://www.jetbrains.com/pycharm/" class="external-link" target="_blank">PyCharm</a> and most of the other Python editors.
 
 
 ## Request body + path parameters
 
 You can declare path parameters **and** body requests at the same time.
 
 **Django Ninja** will recognize that the function parameters that match path parameters should be **taken from the path**, and that function parameters that are declared with `Schema` should be **taken from the request body**.
@@ -112,9 +115,9 @@
 ```Python hl_lines="11 12"
 {!./src/tutorial/body/code03.py!}
 ```
 
 The function parameters will be recognized as follows:
 
 * If the parameter is also declared in the **path**, it will be used as a path parameter.
-* If the parameter is of a **singular type** (like `int`, `float`, `str`, `bool`, etc) it will be interpreted as a **query** parameter.
-* If the parameter is declared to be of the type of a **Schema** (or Pydantic `BaseModel`), it will be interpreted as a request **body**.
+* If the parameter is of a **singular type** (like `int`, `float`, `str`, `bool`, etc.), it will be interpreted as a **query** parameter.
+* If the parameter is declared to be of the type of **Schema** (or Pydantic `BaseModel`), it will be interpreted as a request **body**.
```

#### html2text {}

```diff
@@ -1,54 +1,56 @@
 # Request Body Request bodies are typically used with âcreateâ and
 âupdateâ operations (POST, PUT, PATCH). For example, when creating a
 resource using POST or PUT, the request body usually contains the
 representation of the resource to be created. To declare a **request body**,
-you need to use **NinjaAPI `Schema`**. !!! info Under the hood **NinjaAPI**
-uses Pydantic models with all their power and benefits. The alias `Schema` was
-picked to avoid confusion in code with Django models. ## Import Schema First,
-you need to import `Schema` from `ninja`: ```Python hl_lines="1" {!./src/
-tutorial/body/code01.py!} ``` ## Create your data model Then you declare your
-data model as a class that inherits from `Schema`. Use standard Python types
-for all the attributes: ```Python hl_lines="4 5 6 7 8" {!./src/tutorial/body/
-code01.py!} ``` Note: if you use **`None`** as default value for an attribute -
-it will become optional in the request body. For example, this model above
-declares a JSON "`object`" (or Python `dict`) like: ```JSON { "name": "Katana",
-"description": "An optional description", "price": 299.00, "quantity": 10 } ```
-...as `description` is optional (with a default value of `None`), this JSON
-"`object`" would also be valid: ```JSON { "name": "Katana", "price": 299.00,
-"quantity": 10 } ``` ## Declare it as a parameter To add it to your *path
-operation*, declare it the same way you declared path and query parameters:
-```Python hl_lines="12" {!./src/tutorial/body/code01.py!} ``` ...and declare
-its type as the model you created, `Item`. ## Results With just that Python
-type declaration, **NinjaAPI** will: * Read the body of the request as JSON. *
-Convert the corresponding types (if needed). * Validate the data. * If the data
-is invalid, it will return a nice and clear error, indicating exactly where and
-what was the incorrect data. * Give you the received data in the parameter
-`item`. * As you declared it in the function to be of type `Item`, you will
-also have all the editor support (completion, etc) for all of the attributes
-and their types. * Generate JSON_Schema definitions for your model, you can
-also use them anywhere else you like if it makes sense for your project. *
-Those schemas will be part of the generated OpenAPI schema, and used by the
-automatic documentation UIs. ## Automatic docs The JSON Schemas of your models
-will be part of your OpenAPI generated schema, and will be shown in the
-interactive API docs: ![Openapi schema](../img/body-schema-doc.png) And will be
+you need to use **Django Ninja `Schema`**. !!! info Under the hood **Django
+Ninja** uses Pydantic models with all their power and benefits. The alias
+`Schema` was chosen to avoid confusion in code when using Django models, as
+Pydantic's model class is called Model by default, and conflicts with Django's
+Model class. ## Import Schema First, you need to import `Schema` from `ninja`:
+```Python hl_lines="1" {!./src/tutorial/body/code01.py!} ``` ## Create your
+data model Then you declare your data model as a class that inherits from
+`Schema`. Use standard Python types for all the attributes: ```Python
+hl_lines="4 5 6 7 8" {!./src/tutorial/body/code01.py!} ``` Note: if you use
+**`None`** as the default value for an attribute, it will become optional in
+the request body. For example, this model above declares a JSON "`object`" (or
+Python `dict`) like: ```JSON { "name": "Katana", "description": "An optional
+description", "price": 299.00, "quantity": 10 } ``` ...as `description` is
+optional (with a default value of `None`), this JSON "`object`" would also be
+valid: ```JSON { "name": "Katana", "price": 299.00, "quantity": 10 } ``` ##
+Declare it as a parameter To add it to your *path operation*, declare it the
+same way you declared the path and query parameters: ```Python hl_lines="12"
+{!./src/tutorial/body/code01.py!} ``` ... and declare its type as the model you
+created, `Item`. ## Results With just that Python type declaration, **Django
+Ninja** will: * Read the body of the request as JSON. * Convert the
+corresponding types (if needed). * Validate the data. * If the data is invalid,
+it will return a nice and meaningful error, indicating exactly where and what
+the incorrect data was. * Give you the received data in the parameter `item`. *
+Because you declared it in the function to be of type `Item`, you will also
+have all the editor support (completion, etc.) for all the attributes and their
+types. * Generate JSON_Schema definitions for your models, and you can also use
+them anywhere else you like if it makes sense for your project. * Those schemas
+will be part of the generated OpenAPI schema, and used by the automatic
+documentation UI's. ## Automatic docs The JSON Schemas of your models will be
+part of your OpenAPI generated schema, and will be shown in the interactive API
+docs: ![Openapi schema](../../img/body-schema-doc.png) ... and they will be
 also used in the API docs inside each *path operation* that needs them: !
-[Openapi schema](../img/body-schema-doc2.png) ## Editor support In your editor,
-inside your function you will get type hints and completion everywhere (this
-wouldn't happen if you received a `dict` instead of a Schema object): ![Type
-hints](../img/body-editor.gif) The previous screenshots were taken with Visual
-Studio_Code. But you would get the same editor support with PyCharm and most of
-the other Python editors. ## Request body + path parameters You can declare
-path parameters **and** body requests at the same time. **Django Ninja** will
-recognize that the function parameters that match path parameters should be
-**taken from the path**, and that function parameters that are declared with
-`Schema` should be **taken from the request body**. ```Python hl_lines="11 12"
-{!./src/tutorial/body/code02.py!} ``` ## Request body + path + query parameters
-You can also declare **body**, **path** and **query** parameters, all at the
-same time. **Django Ninja** will recognize each of them and take the data from
-the correct place. ```Python hl_lines="11 12" {!./src/tutorial/body/code03.py!}
-``` The function parameters will be recognized as follows: * If the parameter
-is also declared in the **path**, it will be used as a path parameter. * If the
-parameter is of a **singular type** (like `int`, `float`, `str`, `bool`, etc)
-it will be interpreted as a **query** parameter. * If the parameter is declared
-to be of the type of a **Schema** (or Pydantic `BaseModel`), it will be
-interpreted as a request **body**.
+[Openapi schema](../../img/body-schema-doc2.png) ## Editor support In your
+editor, inside your function you will get type hints and completion everywhere
+(this wouldn't happen if you received a `dict` instead of a Schema object): !
+[Type hints](../../img/body-editor.gif) The previous screenshots were taken
+with Visual_Studio_Code. You would get the same editor support with PyCharm and
+most of the other Python editors. ## Request body + path parameters You can
+declare path parameters **and** body requests at the same time. **Django
+Ninja** will recognize that the function parameters that match path parameters
+should be **taken from the path**, and that function parameters that are
+declared with `Schema` should be **taken from the request body**. ```Python
+hl_lines="11 12" {!./src/tutorial/body/code02.py!} ``` ## Request body + path +
+query parameters You can also declare **body**, **path** and **query**
+parameters, all at the same time. **Django Ninja** will recognize each of them
+and take the data from the correct place. ```Python hl_lines="11 12" {!./src/
+tutorial/body/code03.py!} ``` The function parameters will be recognized as
+follows: * If the parameter is also declared in the **path**, it will be used
+as a path parameter. * If the parameter is of a **singular type** (like `int`,
+`float`, `str`, `bool`, etc.), it will be interpreted as a **query** parameter.
+* If the parameter is declared to be of the type of **Schema** (or Pydantic
+`BaseModel`), it will be interpreted as a request **body**.
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/crud.md` & `django_ninja-1.0a1/docs/docs/tutorial/other/crud.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # CRUD example
 
 
 **CRUD**  - **C**reate, **R**etrieve, **U**pdate, **D**elete are the four basic functions of persistent storage.
 
-This example will show you how to implement these functions with **Django Ninja**
+This example will show you how to implement these functions with **Django Ninja**.
 
-Let's say you have the following django models that you need to perform these operations with:
+Let's say you have the following Django models that you need to perform these operations on:
 
 
 ```Python
 
 class Department(models.Model):
     title = models.CharField(max_length=100)
 
 class Employee(models.Model):
     first_name = models.CharField(max_length=100)
     last_name = models.CharField(max_length=100)
-    department = models.ForeignKey(Department)
+    department = models.ForeignKey(Department, on_delete=models.CASCADE)
     birthdate = models.DateField(null=True, blank=True)
+    cv = models.FileField(null=True, blank=True)
 ```
 
-Now let's create CRUD operations for Employee model
+Now let's create CRUD operations for the Employee model.
 
 ## Create
 
-To create an employee lets define a INPUT schema:
+To create an employee lets define an INPUT schema:
 
 ```Python
 from datetime import date
 from ninja import Schema
 
 class EmployeeIn(Schema):
     first_name: str
@@ -41,129 +42,155 @@
 This schema will be our input payload:
 
 ```Python hl_lines="2"
 @api.post("/employees")
 def create_employee(request, payload: EmployeeIn):
     employee = Employee.objects.create(**payload.dict())
     return {"id": employee.id}
-
 ```
 
 !!! tip
-    `Schema` objects have `.dict()` attribute with all the schema attributes represented as dict
+    `Schema` objects have `.dict()` method with all the schema attributes represented as a dict.
+
+    You can pass it as `**kwargs` to the Django model's `create` method (or model `__init__`).
+
+See the recipe below for handling the file upload (when using Django models):
+
+```Python hl_lines="2"
+from ninja import UploadedFile, File
+
+@api.post("/employees")
+def create_employee(request, payload: EmployeeIn, cv: UploadedFile = File(...)):
+    payload_dict = payload.dict()
+    employee = Employee(**payload_dict)
+    employee.cv.save(cv.name, cv) # will save model instance as well
+    return {"id": employee.id}
+```
 
-    You can pass it as `**kwargs` to django model `create` meothod (or model `__init__`)
+If you just need to handle a file upload:
+
+```Python hl_lines="2"
+from django.core.files.storage import FileSystemStorage
+from ninja import UploadedFile, File
+
+STORAGE = FileSystemStorage()
+
+@api.post("/upload")
+def create_upload(request, cv: UploadedFile = File(...)):
+    filename = STORAGE.save(cv.name, cv)
+    # Handle things further
+```
 
 ## Retrieve
 
 ### Single object
 
-Now to get employee we will define schema that will describe how our responses will look like. Here we will basically use same schema as `EmployeeIn` but will add extra attribute `id`:
+Now to get employee we will define a schema that will describe what our responses will look like. Here we will basically use the same schema as `EmployeeIn`, but will add an extra attribute `id`:
 
 
 ```Python hl_lines="2"
 class EmployeeOut(Schema):
     id: int
     first_name: str
     last_name: str
     department_id: int = None
     birthdate: date = None
 ```
 
 !!! note
-    Defining response schemas are not really required. But when you do define it you will get results validation, documentation and automatic ORM objects to JSON converting.
+    Defining response schemas are not really required, but when you do define it you will get results validation, documentation and automatic ORM objects to JSON conversions.
 
-We will use this schema as `response` type for our get employee view:
+We will use this schema as the `response` type for our `GET` employee view:
 
 
 ```Python hl_lines="1"
 @api.get("/employees/{employee_id}", response=EmployeeOut)
 def get_employee(request, employee_id: int):
     employee = get_object_or_404(Employee, id=employee_id)
     return employee
 ```
 
-Notice that we simply returned employee ORM object, without a need to convert it to dict. The `response` schema does automatic result validation and converting to JSON:
+Notice that we simply returned an employee ORM object, without a need to convert it to a dict. The `response` schema does automatic result validation and conversion to JSON:
 ```Python hl_lines="4"
 @api.get("/employees/{employee_id}", response=EmployeeOut)
 def get_employee(request, employee_id: int):
     employee = get_object_or_404(Employee, id=employee_id)
     return employee
 ```
 
 ### List of objects
 
-To output list of employees we can reuse the same schema `EmployeeOut`. We will just set `response` schema to a *List* or `EmployeeOut`
+To output a list of employees, we can reuse the same `EmployeeOut` schema. We will just set the `response` schema to a *List* of `EmployeeOut`.
 ```Python hl_lines="3"
 from typing import List
 
 @api.get("/employees", response=List[EmployeeOut])
 def list_employees(request):
     qs = Employee.objects.all()
     return qs
 ```
 
-Another cool trick - notice we just returned a ORM queryset:
+Another cool trick - notice we just returned a Django ORM queryset:
 
 ```Python hl_lines="4"
 @api.get("/employees", response=List[EmployeeOut])
 def list_employees(request):
     qs = Employee.objects.all()
     return qs
 ```
-But it automatically getting evaluated, validated and converted to JSON list
+It automatically gets evaluated, validated and converted to a JSON list!
 
 
 
 ## Update
 
-The update is pretty trivial, we just use `PUT` method and also pass employee_id:
+Update is pretty trivial. We just use the `PUT` method and also pass `employee_id`:
 
 ```Python hl_lines="1"
 @api.put("/employees/{employee_id}")
 def update_employee(request, employee_id: int, payload: EmployeeIn):
     employee = get_object_or_404(Employee, id=employee_id)
     for attr, value in payload.dict().items():
         setattr(employee, attr, value)
     employee.save()
     return {"success": True}
 ```
 
 **Note**
 
-Here we used `payload.dict` function to set all object attribute:
+Here we used the `payload.dict` method to set all object attributes:
 
 `for attr, value in payload.dict().items()`
 
-You can also do this more implicit:
+You can also do this more explicit:
 
 ```Python
 employee.first_name = payload.first_name
 employee.last_name = payload.last_name
 employee.department_id = payload.department_id
 employee.birthdate = payload.birthdate
 ```
 
 
 ## Delete
 
-The deletion is pretty simple - we just get employee by id and delete it from DB:
+Delete is also pretty simple. We just get employee by `id` and delete it from the DB:
 
 
 ```Python hl_lines="1 2 4"
 @api.delete("/employees/{employee_id}")
 def delete_employee(request, employee_id: int):
     employee = get_object_or_404(Employee, id=employee_id)
     employee.delete()
     return {"success": True}
 ```
 
 ## Final code
 
-Here is a full CRUD code:
+Here's a full CRUD example:
 
 
 ```Python
 from datetime import date
 from typing import List
 from ninja import NinjaAPI, Schema
 from django.shortcuts import get_object_or_404
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/query-params.md` & `django_ninja-1.0a1/docs/docs/guides/input/query-params.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,98 +2,108 @@
 
 When you declare other function parameters that are not part of the path parameters, they are automatically interpreted as "query" parameters.
 
 ```Python hl_lines="5"
 {!./src/tutorial/query/code01.py!}
 ```
 
-To query this operation we would use url like
+To query this operation, you use a URL like:
 
 ```
 http://localhost:8000/api/weapons?offset=0&limit=10
 ```
-By default all GET parameters are strings, and when you annotate your function arguments with types, they are converted to that type and validated against it.
+By default, all GET parameters are strings, and when you annotate your function arguments with types, they are converted to that type and validated against it.
 
-All the same process that applied for path parameters also applies for query parameters:
+The same benefits that apply to path parameters also apply to query parameters:
 
 - Editor support (obviously)
 - Data "parsing"
 - Data validation
 - Automatic documentation
 
 
-Note: if you do not annotate your arguments - it will be treated as `str` types:
+Note: if you do not annotate your arguments, they will be treated as `str` types:
 
 ```Python hl_lines="2"
 @api.get("/weapons")
 def list_weapons(request, limit, offset):
-    return weapons[offset : offset + limit]
+    # type(limit) == str
+    # type(offset) == str
 ```
 
 ### Defaults
 
-As query parameters are not a fixed part of a path, they can be optional and can have default values.
+As query parameters are not a fixed part of a path, they are optional and can have default values:
 
-In the example above they have default values of `offset=0` and `limit=10`.
+```Python hl_lines="2"
+@api.get("/weapons")
+def list_weapons(request, limit: int = 10, offset: int = 0):
+    return weapons[offset : offset + limit]
+```
+
+In the example above we set default values of `offset=0` and `limit=10`.
 
 So, going to the URL:
 ```
 http://localhost:8000/api/weapons
 ```
 would be the same as going to:
 ```
 http://localhost:8000/api/weapons?offset=0&limit=10
 ```
-But if you go to, for example:
+If you go to, for example:
 ```
 http://localhost:8000/api/weapons?offset=20
 ```
 
-The parameter values in your function will be:
+the parameter values in your function will be:
 
- - `offset=20`: because you set it in the URL
- - `limit=10`: because that was the default value
+ - `offset=20`  (because you set it in the URL)
+ - `limit=10`  (because that was the default value)
 
 
 ### Required and optional parameters
 
-You can declare required or optional GET parameters same way as you declare python function arguments:
+You can declare required or optional GET parameters in the same way as declaring Python function arguments:
 
 ```Python hl_lines="5"
 {!./src/tutorial/query/code02.py!}
 ```
 
-In this case Django Ninja will always validate that you pass `q` param in GET, and `offset` param is optional integer
+In this case, **Django Ninja** will always validate that you pass the `q` param in the GET, and the `offset` param is an optional integer.
 
 ### GET parameters type conversion
 
 Let's declare multiple type arguments:
 ```Python hl_lines="5"
 {!./src/tutorial/query/code03.py!}
 ```
-The `str` type is passed as is
+The `str` type is passed as is.
 
-For `bool` type all of the following:s
+For the `bool` type, all the following:
 ```
 http://localhost:8000/api/example?b=1
 http://localhost:8000/api/example?b=True
 http://localhost:8000/api/example?b=true
 http://localhost:8000/api/example?b=on
 http://localhost:8000/api/example?b=yes
 ```
-or any other case variation (uppercase, first letter in uppercase, etc), your function will see the parameter `b` with a `bool` value of `True`. Otherwise as `False`.
+or any other case variation (uppercase, first letter in uppercase, etc.), your function will see
+the parameter `b` with a `bool` value of `True`, otherwise as `False`.
 
 Date can be both date string and integer (unix timestamp):
 
 <pre style="font-size: .85em; background-color:rgb(245, 245, 245);">
-http://localhost:8000/api/example?d=<strong>1577836800</strong>  # = 2020-01-01
+http://localhost:8000/api/example?d=<strong>1577836800</strong>  # same as 2020-01-01
 http://localhost:8000/api/example?d=<strong>2020-01-01</strong>
 </pre>
 
 
 ### Using Schema
 
-You can as well use Schema to encapsulate GET parameters:
+You can also use Schema to encapsulate GET parameters:
 
 ```Python hl_lines="1 2  5 6 7 8"
 {!./src/tutorial/query/code010.py!}
 ```
+
+For more complex filtering scenarios please refer to [filtering](./filtering.md).
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/routers.md` & `django_ninja-1.0a1/docs/docs/guides/routers.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Routers
 
-Real world applications almost never can fit all logic into a single file. 
+Real world applications can almost never fit all logic into a single file. 
 
-**Django Ninja** comes with an easy way to split your API into multiple modules.
+**Django Ninja** comes with an easy way to split your API into multiple modules using Routers.
 
-Let's say you have a django project with structure like this:
+Let's say you have a Django project with a structure like this:
 
 
 ```
 ├── myproject
 │   └── settings.py
 ├── events/
 │   ├── __init__.py
@@ -18,15 +18,15 @@
 │   └── models.py
 ├── blogs/
 │   ├── __init__.py
 │   └── models.py
 └── manage.py
 ```
 
-To add APIs to each of the application, lets create an `api.py` module in each:
+To add API's to each of the Django applications, create an `api.py` module in each app:
 
 ``` hl_lines="5 9 13"
 ├── myproject
 │   └── settings.py
 ├── events/
 │   ├── __init__.py
 │   ├── api.py
@@ -38,15 +38,15 @@
 ├── blogs/
 │   ├── __init__.py
 │   ├── api.py
 │   └── models.py
 └── manage.py
 ```
 
-Now lets add few operations to `events/api.py`. The trick is that instead of NinjaAPI class you need to use **Router** class:
+Now let's add a few operations to `events/api.py`. The trick is that instead of using the `NinjaAPI` class, you use the **Router** class:
 
 ```python  hl_lines="1 4 6 13"
 from ninja import Router
 from .models import Event
 
 router = Router()
 
@@ -59,84 +59,113 @@
 
 @router.get('/{event_id}')
 def event_details(request, event_id: int):
     event = Event.objects.get(id=event_id)
     return {"title": event.title, "details": event.details}
 ```
 
-Then do the same for news:
+Then do the same for the `news` app with `news/api.py`:
 
 ```python  hl_lines="1 4"
 from ninja import Router
 from .models import News
 
 router = Router()
 
 @router.get('/')
 def list_news(request):
     ...
 
 @router.get('/{news_id}')
-def news_details(request, event_id: int):
+def news_details(request, news_id: int):
     ...
 ```
-and blogs.
+and then also `blogs/api.py`.
 
 
-Finally let's group this together, in your project folder (next to urls.py) create another api.py file with main NinjaAPI instance:
+Finally, let's group them together.
+In your top level project folder (next to `urls.py`), create another `api.py` file with the main `NinjaAPI` instance:
 
 ``` hl_lines="2"
 ├── myproject
 │   ├── api.py
 │   └── settings.py
 ├── events/
 │   ...
 ├── news/
 │   ...
 ├── blogs/
 │   ...
 
 ```
 
-this will be like:
+It should look like this:
 
 ```Python
 from ninja import NinjaAPI
 
 api = NinjaAPI()
 
 ```
 
-Now we import all the routers from apps, and include them into main api instance:
+Now we import all the routers from the various apps, and include them into the main API instance:
 
 ```Python hl_lines="2 3 4 8 9 10"
 from ninja import NinjaAPI
 from events.api import router as events_router
 from news.api import router as news_router
 from blogs.api import router as blogs_router
 
 api = NinjaAPI()
 
 api.add_router("/events/", events_router)
 api.add_router("/news/", news_router)
 api.add_router("/blogs/", blogs_router)
 ```
 
-Now include api to your urls as usual and open your browser at `/api/docs` - you should see all your routers combined into single api:
+Now, include `api` to your urls as usual and open your browser at `/api/docs`, and you should see all your routers combined into a single API:
 
 
 ![Swagger UI Simple Routers](../img/simple-routers-swagger.png)
 
 
+## Router authentication
+
+Use `auth` argument to apply authenticator to all operations declared by router:
+
+```Python
+api.add_router("/events/", events_router, auth=BasicAuth())
+```
+
+or using router constructor
+```Python
+router = Router(auth=BasicAuth())
+```
+
+## Router tags
+
+You can use `tags` argument to apply tags to all operations declared by router:
+
+```Python
+api.add_router("/events/", events_router, tags=["events"])
+```
+
+or using router constructor
+```Python
+router = Router(tags=["events"])
+```
+
+
 ## Nested routers
 
-There also times when you need to split your logic even more. **Django Ninja** make is possible to include router into other router as many times as you like and finally include top router into main api instance.
+There are also times when you need to split your logic up even more.
+**Django Ninja** makes it possible to include a router into another router as many times as you like, and finally include the top level router into the main api instance.
 
 
-Basically what it means that you have `add_router` both on `api` instance and `router` instance:
+Basically, what that means is that you have `add_router` both on the `api` instance and on the `router` instance:
 
 
 
 ```Python hl_lines="7 8 9 32 33 34"
 from django.contrib import admin
 from django.urls import path
 from ninja import NinjaAPI, Router
@@ -182,10 +211,11 @@
 
 ```
 /api/add
 /api/l1/add
 /api/l1/l2/add
 /api/l1/l2/l3/add
 ```
-See the automatically generated docs:
+
+Great! Now go have a look at the automatically generated docs:
 
 ![Swagger UI Nested Routers](../img/nested-routers-swagger.png)
```

### Comparing `django-ninja-0.9.7/docs/docs/tutorial/versioning.md` & `django_ninja-1.0a1/docs/docs/guides/versioning.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # Versioning
 
-## Different version numbers
+## Different API version numbers
 
-With Django Ninja it's easy to run multiple API version from a single django project.
+With **Django Ninja** it's easy to run multiple API versions from a single Django project.
 
-All you have to do is to create two or more NinjaAPI instance with different `version` argument:
+All you have to do is create two or more NinjaAPI instances with different `version` arguments:
 
 
-file  **api_v1.py**:
+**api_v1.py**:
 
 ```Python hl_lines="4"
 from ninja import NinjaAPI
 
 
 api = NinjaAPI(version='1.0.0')
 
 @api.get('/hello')
 def hello(request):
     return {'message': 'Hello from V1'}
 
 ```
 
 
-file  api_**v2**.py:
+api_**v2**.py:
+
 ```Python hl_lines="4"
 from ninja import NinjaAPI
 
 
 api = NinjaAPI(version='2.0.0')
 
 @api.get('/hello')
 def hello(request):
     return {'message': 'Hello from V2'}
 ```
 
-and then in **urs.py**:
+
+and then in **urls.py**:
 
 ```Python hl_lines="8 9"
 ...
 from api_v1 import api as api_v1
 from api_v2 import api as api_v2
 
 
@@ -46,24 +48,25 @@
     ...
     path('api/v1/', api_v1.urls),
     path('api/v2/', api_v2.urls),
 ]
 
 ```
 
-Now you can go to different docs pages for each version:
+
+Now you can go to different OpenAPI docs pages for each version:
 
  - http://127.0.0.1/api/**v1**/docs
  - http://127.0.0.1/api/**v2**/docs
 
 
 
 ## Different business logic
 
-Same way you can define different API for different components or areas:
+In the same way, you can define a different API for different components or areas:
 
 ```Python hl_lines="4 7"
 ...
 
 
 api = NinjaAPI(auth=token_auth, urls_namespace='public_api')
 ...
@@ -76,8 +79,8 @@
     ...
     path('api/', api.urls),
     path('internal-api/', api_private.urls),
 ]
 
 ```
 !!! note
-    if you use different **NinjaAPI** instances - you need to define different `version`s or different `urls_namespace`s
+    If you use different **NinjaAPI** instances, you need to define different `version`s or different `urls_namespace`s.
```

### Comparing `django-ninja-0.9.7/docs/src/tutorial/authentication/global01.py` & `django_ninja-1.0a1/docs/src/tutorial/authentication/global01.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/ninja/compatibility/datastructures.py` & `django_ninja-1.0a1/ninja/compatibility/datastructures.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/ninja/compatibility/request.py` & `django_ninja-1.0a1/ninja/compatibility/request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import Callable
+
 import django
+from django.http import HttpRequest
 
 try:
     from django.utils.datastructures import CaseInsensitiveMapping
 except ImportError:
     from .datastructures import CaseInsensitiveMapping
 
 
@@ -23,25 +26,28 @@
     def __getitem__(self, key):
         """Allow header lookup using underscores in place of hyphens."""
         return super().__getitem__(key.replace("_", "-"))
 
     @classmethod
     def parse_header_name(cls, header):
         if header.startswith(cls.HTTP_PREFIX):
-            header = header[len(cls.HTTP_PREFIX) :]
+            start = len(cls.HTTP_PREFIX)
+            header = header[start:]
         elif header not in cls.UNPREFIXED_HEADERS:
             return None
         return header.replace("_", "-").title()
 
 
 def get_headers_old(request):
     return HttpHeaders(request.META)
 
 
 def get_headers_v3(request):
     return request.headers
 
 
+get_headers: Callable[[HttpRequest], HttpHeaders]
+
 if django.VERSION[0] < 3:
     get_headers = get_headers_old
 else:
     get_headers = get_headers_v3
```

### Comparing `django-ninja-0.9.7/ninja/openapi/views.py` & `django_ninja-1.0a1/tests/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from ninja.responses import Response
-from django.http import Http404
-from django.urls import reverse
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    # if anyone knows a cleaner way to make mypy happy - welcome
-    from ninja import NinjaAPI  # pragma: no cover
-
-
-def default_home(request, api: "NinjaAPI"):
-    "This view is mainly needed to determine the full path for API operations"
-    docs_url = f"{request.path}{api.docs_url}".replace("//", "/")
-    raise Http404(f"docs_url = {docs_url}")
-
-
-def openapi_json(request, api: "NinjaAPI"):
-    schema = api.get_openapi_schema()
-    return Response(schema)
-
-
-def swagger(request, api: "NinjaAPI"):
-    return render(
-        request,
-        "ninja/swagger.html",
-        {
-            "api": api,
-            "openapi_json_url": reverse(f"{api.urls_namespace}:openapi-json"),
-        },
-    )
-
-
-def render(request, template_name: str, context=None):
-    """
-    I do not really want ninja to be required in INSTALLED_APPS for now
-    that is why for now we use this render function to simulate django render
-    """
-    import os
-    from django.template import Template, RequestContext
-    from django.http import HttpResponse
-
-    tpl_file = os.path.join(os.path.dirname(__file__), "../templates", template_name)
-    with open(tpl_file) as f:
-        tpl = Template(f.read())
-    html = tpl.render(RequestContext(request, context))
-    return HttpResponse(html)
+from typing import List
+
+from django.http import HttpRequest, QueryDict
+
+from ninja import NinjaAPI
+from ninja.parser import Parser
+from ninja.testing import TestClient
+
+
+class MyParser(Parser):
+    "Default json parser"
+
+    def parse_body(self, request: HttpRequest):
+        "just splitting body to lines"
+        return request.body.encode().splitlines()
+
+    def parse_querydict(
+        self, data: QueryDict, list_fields: List[str], request: HttpRequest
+    ):
+        "Turning empty Query params to None instead of empty string"
+        result = super().parse_querydict(data, list_fields, request)
+        for k, v in list(result.items()):
+            if v == "":
+                del result[k]
+        return result
+
+
+api = NinjaAPI(parser=MyParser())
+
+
+@api.post("/test")
+def operation(request, body: List[str], emptyparam: str = None):
+    return {"emptyparam": emptyparam, "body": body}
+
+
+def test_parser():
+    client = TestClient(api)
+    response = client.post("/test?emptyparam", body="test\nbar")
+    assert response.status_code == 200, response.content
+    assert response.json() == {"emptyparam": None, "body": ["test", "bar"]}
```

### Comparing `django-ninja-0.9.7/ninja/params.py` & `django_ninja-1.0a1/ninja/params.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from pydantic.fields import FieldInfo, ModelField
-from pydantic import BaseConfig
-from typing import Any
+from typing import Any, Dict, Optional
+
+from pydantic.fields import FieldInfo
+
 from ninja import params_models
 
+__all__ = ["Param", "Path", "Query", "Header", "Cookie", "Body", "Form", "File"]
+
 
 class Param(FieldInfo):
     def __init__(
         self,
         default: Any,
         *,
         alias: str = None,
@@ -15,42 +18,58 @@
         gt: float = None,
         ge: float = None,
         lt: float = None,
         le: float = None,
         min_length: int = None,
         max_length: int = None,
         regex: str = None,
+        example: Any = None,
+        examples: Optional[Dict[str, Any]] = None,
         deprecated: bool = None,
+        include_in_schema: bool = True,
         # param_name: str = None,
         # param_type: Any = None,
         **extra: Any,
     ):
-        # print('alias = ', alias)
         self.deprecated = deprecated
         # self.param_name: str = None
         # self.param_type: Any = None
-        self.model_field: ModelField = None
+        self.model_field: Optional[FieldInfo] = None
+        json_schema_extra = {}
+        if example:
+            json_schema_extra["example"] = example
+        if examples:
+            json_schema_extra["examples"] = examples
+        if deprecated:
+            json_schema_extra["deprecated"] = deprecated
+        if not include_in_schema:
+            json_schema_extra["include_in_schema"] = include_in_schema
+        if alias and not extra.get("validation_alias"):
+            extra["validation_alias"] = alias
+        if alias and not extra.get("serialization_alias"):
+            extra["serialization_alias"] = alias
         super().__init__(
-            default,
+            default=default,
             alias=alias,
             title=title,
             description=description,
             gt=gt,
             ge=ge,
             lt=lt,
             le=le,
             min_length=min_length,
             max_length=max_length,
             regex=regex,
+            json_schema_extra=json_schema_extra,
             **extra,
         )
 
     @classmethod
-    def _in(cls):
-        "Openapi param.in value"
+    def _param_source(cls) -> str:
+        "Openapi param.in value or body type"
         return cls.__name__.lower()
 
 
 class Path(Param):
     _model = params_models.PathModel
 
 
@@ -68,7 +87,19 @@
 
 class Body(Param):
     _model = params_models.BodyModel
 
 
 class Form(Param):
     _model = params_models.FormModel
+
+
+class File(Param):
+    _model = params_models.FileModel
+
+
+class _MultiPartBody(Param):
+    _model = params_models._MultiPartBodyModel
+
+    @classmethod
+    def _param_source(cls) -> str:
+        return "body"
```

### Comparing `django-ninja-0.9.7/ninja/security/base.py` & `django_ninja-1.0a1/ninja/security/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+from abc import ABC, abstractmethod
+from typing import Any, Optional
+
+from django.http import HttpRequest
+
 from ninja.errors import ConfigError
+from ninja.utils import is_async_callable
+
+__all__ = ["SecuritySchema", "AuthBase"]
 
 
 class SecuritySchema(dict):
-    def __init__(self, type: str, **kwargs):
+    def __init__(self, type: str, **kwargs: Any) -> None:
         super().__init__(type=type, **kwargs)
 
 
-class AuthBase:
-    def __init__(self):
+class AuthBase(ABC):
+    def __init__(self) -> None:
         if not hasattr(self, "openapi_type"):
             raise ConfigError("If you extend AuthBase you need to define openapi_type")
 
         kwargs = {}
         for attr in dir(self):
             if attr.startswith("openapi_"):
                 name = attr.replace("openapi_", "", 1)
                 kwargs[name] = getattr(self, attr)
         self.openapi_security_schema = SecuritySchema(**kwargs)
 
-    def __call__(self, request):
-        raise NotImplementedError("Please implement call")
+        self.is_async = False
+        if hasattr(self, "authenticate"):  # pragma: no branch
+            self.is_async = is_async_callable(self.authenticate)  # type: ignore
+
+    @abstractmethod
+    def __call__(self, request: HttpRequest) -> Optional[Any]:
+        pass  # pragma: no cover
```

### Comparing `django-ninja-0.9.7/tests/demo_project/demo/settings.py` & `django_ninja-1.0a1/tests/demo_project/demo/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,74 @@
-
 import os
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 
-SECRET_KEY = '$v8ppoke(!-cus95vxzg04d@63ut)5c5jo6p&&^gffy=yy0k8a'
+SECRET_KEY = "NOT-SUPER-SECRET-DO-NOT-USE-ME"
 
 
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
 
 INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'someapp',
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "ninja",
+    "someapp",
+    "multi_param",
 ]
 
 MIDDLEWARE = [
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
 
-ROOT_URLCONF = 'demo.urls'
+ROOT_URLCONF = "demo.urls"
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
             ],
         },
     },
 ]
 
-WSGI_APPLICATION = 'demo.wsgi.application'
+WSGI_APPLICATION = "demo.wsgi.application"
 
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": os.path.join(BASE_DIR, "db.sqlite3"),
     }
 }
 
 
+LANGUAGE_CODE = "en-us"
 
-LANGUAGE_CODE = 'en-us'
-
-TIME_ZONE = 'UTC'
+TIME_ZONE = "UTC"
 
 USE_I18N = True
 
-USE_L10N = True
-
 USE_TZ = True
 
 
-STATIC_URL = '/static/'
+STATIC_URL = "/static/"
```

### Comparing `django-ninja-0.9.7/tests/demo_project/manage.py` & `django_ninja-1.0a1/tests/demo_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/tests/demo_project/someapp/api.py` & `django_ninja-1.0a1/tests/demo_project/someapp/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from datetime import date
-from ninja import Router
 from typing import List
-from pydantic import BaseModel
+
 from django.shortcuts import get_object_or_404
+from pydantic import BaseModel
+
+from ninja import Router
+
 from .models import Event
 
 router = Router()
 
 
 class EventSchema(BaseModel):
     title: str
     start_date: date
     end_date: date
 
     class Config:
-        orm_mode = True
+        from_attributes = True
 
 
-@router.post("/create")
+@router.post("/create", url_name="event-create-url-name")
 def create_event(request, event: EventSchema):
-    Event.objects.create(**event.dict())
+    Event.objects.create(**event.model_dump())
     return event
 
 
 @router.get("", response=List[EventSchema])
 def list_events(request):
     return list(Event.objects.all())
 
 
+@router.delete("")
+def delete_events(request):
+    Event.objects.all().delete()
+
+
 @router.get("/{id}", response=EventSchema)
 def get_event(request, id: int):
     event = get_object_or_404(Event, id=id)
     return event
```

### Comparing `django-ninja-0.9.7/tests/env-matrix/Dockerfile` & `django_ninja-1.0a1/tests/env-matrix/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/tests/env-matrix/Dockerfile.backup` & `django_ninja-1.0a1/tests/env-matrix/Dockerfile.backup`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/tests/env-matrix/create_docker.py` & `django_ninja-1.0a1/tests/env-matrix/create_docker.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.7/tests/test_app.py` & `django_ninja-1.0a1/tests/test_test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,98 @@
-import os
-import pytest
-from ninja import NinjaAPI
-from ninja.main import ConfigError
-from django.http import HttpResponse
-from client import NinjaClient
-
-
-api = NinjaAPI()
-
-
-# TODO: check if you add  operation to the same path - it should raise a ConfigError that this path already exist
-# make sure to check how this will work with versioning
-# and also check what will happen if you add same path in different routers
-#  api.add_router("", router1)
-#  api.add_router("", router2)
-# and both routers have same path defined
-
-
-@api.get("")
-def emptypath(request):
-    return "/"
-
-
-@api.get("/get")
-def get(request):
-    return f"this is {request.method}"
+from datetime import datetime
+from http import HTTPStatus
+from unittest import mock
 
+import pytest
+from django.utils import timezone
 
-@api.post("/post")
-def post(request):
-    return f"this is {request.method}"
+from ninja import Router
+from ninja.schema import Schema
+from ninja.testing import TestClient
 
+router = Router()
 
-@api.put("/put")
-def put(request):
-    return f"this is {request.method}"
 
+@router.get("/request/build_absolute_uri")
+def request_build_absolute_uri(request):
+    return request.build_absolute_uri()
 
-@api.patch("/patch")
-def patch(request):
-    return f"this is {request.method}"
 
+@router.get("/request/build_absolute_uri/location")
+def request_build_absolute_uri_location(request):
+    return request.build_absolute_uri("location")
 
-@api.delete("/delete")
-def delete(request):
-    return f"this is {request.method}"
 
+@router.get("/test")
+def simple_get(request):
+    return "test"
 
-@api.api_operation(["GET", "POST"], "/multi")
-def multiple(request):
-    return f"this is {request.method}"
 
+client = TestClient(router)
 
-@api.get("/html")
-def html(request):
-    return HttpResponse("html")
 
+@pytest.mark.parametrize(
+    "path,expected_status,expected_response",
+    [
+        ("/request/build_absolute_uri", HTTPStatus.OK, "http://testlocation/"),
+        (
+            "/request/build_absolute_uri/location",
+            HTTPStatus.OK,
+            "http://testlocation/location",
+        ),
+    ],
+)
+def test_sync_build_absolute_uri(path, expected_status, expected_response):
+    response = client.get(path)
 
-client = NinjaClient(api)
+    assert response.status_code == expected_status
+    assert response.json() == expected_response
 
 
 @pytest.mark.parametrize(
-    # fmt: off
-    "method,path,expected_status,expected_data",
+    "version, has_headers",
     [
-        ("get",    "/",       200, "/"),
-        ("get",    "/get",    200, "this is GET"),
-        ("post",   "/post",   200, "this is POST"),
-        ("put",    "/put",    200, "this is PUT"),
-        ("patch",  "/patch",  200, "this is PATCH"),
-        ("delete", "/delete", 200, "this is DELETE"),
-        ("get",    "/multi",  200, "this is GET"),
-        ("post",   "/multi",  200, "this is POST"),
-        ("patch",  "/multi",  405, b"Method not allowed"),
-        ("get",    "/html",   200, b"html"),
+        ((2, 0), False),
+        ((2, 1), False),
+        ((2, 2), True),
+        ((3, 0), True),
     ],
-    # fmt: on
 )
-def test_method(method, path, expected_status, expected_data):
-    func = getattr(client, method)
-    response = func(path)
-    assert response.status_code == expected_status
-    try:
-        data = response.json()
-    except Exception:
-        data = response.content
-    assert data == expected_data
-
-
-def test_validates():
-    api1 = NinjaAPI()
-    try:
-        os.environ["NINJA_SKIP_REGISTRY"] = ""
-        with pytest.raises(ConfigError):
-            api2 = NinjaAPI()
-            urls = api2.urls
-    finally:
-        os.environ["NINJA_SKIP_REGISTRY"] = "yes"
+def test_django_2_2_plus_headers(version, has_headers):
+    with mock.patch("ninja.testing.client.django", VERSION=version):
+        with mock.patch.object(client, "_call") as call:
+            client.get("/test")
+            request = call.call_args[0][1]
+            # for Django >= 2.2 we apply a HttpHeaders instance to .headers
+            assert isinstance(request.headers, mock.Mock) != has_headers
+
+
+class ClientTestSchema(Schema):
+    time: datetime
+
+
+def test_schema_as_data():
+    schema_instance = ClientTestSchema(time=timezone.now().replace(microsecond=0))
+
+    with mock.patch.object(client, "_call") as call:
+        client.post("/test", json=schema_instance)
+        request = call.call_args[0][1]
+        assert (
+            ClientTestSchema.model_validate_json(request.body).model_dump_json()
+            == schema_instance.model_dump_json()
+        )
+
+
+def test_json_as_body():
+    schema_instance = ClientTestSchema(time=timezone.now().replace(microsecond=0))
+
+    with mock.patch.object(client, "_call") as call:
+        client.post(
+            "/test",
+            data=schema_instance.model_dump_json(),
+            content_type="application/json",
+        )
+        request = call.call_args[0][1]
+        assert (
+            ClientTestSchema.model_validate_json(request.body).model_dump_json()
+            == schema_instance.model_dump_json()
+        )
```

### Comparing `django-ninja-0.9.7/tests/test_async.py` & `django_ninja-1.0a1/tests/test_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import pytest
 import asyncio
+
 import django
+import pytest
+
 from ninja import NinjaAPI
 from ninja.security import APIKeyQuery
-from client import NinjaAsyncClient
+from ninja.testing import TestAsyncClient
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 @pytest.mark.asyncio
 async def test_asyncio_operations():
     api = NinjaAPI()
 
@@ -21,15 +23,15 @@
         await asyncio.sleep(0)
         return {"async": True}
 
     @api.post("/async")
     def sync_post_to_async_view(request):
         return {"sync": True}
 
-    client = NinjaAsyncClient(api)
+    client = TestAsyncClient(api)
 
     # Actual tests --------------------------------------------------
 
     # without auth:
     res = await client.get("/async?payload=1")
     assert res.status_code == 401
 
@@ -37,14 +39,14 @@
     res = await client.get("/async?payload=1&key=secret")
     assert res.json() == {"async": True}
 
     # async innvalid input
     res = await client.get("/async?payload=str&key=secret")
     assert res.status_code == 422
 
-    # async call to sync method for path that hahve async operations
+    # async call to sync method for path that have async operations
     res = await client.post("/async")
     assert res.json() == {"sync": True}
 
     # invalid method
     res = await client.put("/async")
     assert res.status_code == 405
```

### Comparing `django-ninja-0.9.7/tests/test_auth_global.py` & `django_ninja-1.0a1/tests/test_auth_global.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ninja import NinjaAPI, Router
 from ninja.security import APIKeyQuery
-from client import NinjaClient
+from ninja.testing import TestClient
 
 
 class KeyQuery1(APIKeyQuery):
     def authenticate(self, request, key):
         if key == "k1":
             return key
 
@@ -48,15 +48,15 @@
     return {"auth": str(request.auth)}
 
 
 api.add_router("", router)
 
 # ---- end router --------------------
 
-client = NinjaClient(api)
+client = TestClient(api)
 
 
 def test_multi():
     assert client.get("/default").status_code == 401
     assert client.get("/default?key=k1").json() == {"auth": "k1"}
 
     assert client.post("/multi-method-no-auth").status_code == 401
```

### Comparing `django-ninja-0.9.7/tests/test_docs/test_auth.py` & `django_ninja-1.0a1/tests/test_docs/test_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import pytest
 from unittest.mock import Mock, patch
+
+import pytest
+
 from ninja import NinjaAPI
-from client import NinjaClient
+from ninja.testing import TestClient
 
 
 def test_intro():
     from docs.src.tutorial.authentication.code001 import api
 
-    client = NinjaClient(api)
+    client = TestClient(api)
     assert client.get("/pets").status_code == 401
 
     user = Mock()
     user.is_authenticated = True
 
     response = client.get("/pets", user=user)
     assert response.status_code == 200
@@ -21,25 +23,25 @@
 def test_examples():
     from someapp.models import Client
 
     api = NinjaAPI(csrf=True)
     Client.objects.create(key="12345")
 
     with patch("builtins.api", api, create=True):
-        import docs.src.tutorial.authentication.code002
-        import docs.src.tutorial.authentication.apikey01
-        import docs.src.tutorial.authentication.apikey02
-        import docs.src.tutorial.authentication.apikey03
-        import docs.src.tutorial.authentication.basic01
-        import docs.src.tutorial.authentication.bearer01
-        import docs.src.tutorial.authentication.code001
-        import docs.src.tutorial.authentication.schema01
-        import docs.src.tutorial.authentication.multiple01
+        import docs.src.tutorial.authentication.apikey01  # noqa: F401
+        import docs.src.tutorial.authentication.apikey02  # noqa: F401
+        import docs.src.tutorial.authentication.apikey03  # noqa: F401
+        import docs.src.tutorial.authentication.basic01  # noqa: F401
+        import docs.src.tutorial.authentication.bearer01  # noqa: F401
+        import docs.src.tutorial.authentication.code001  # noqa: F401
+        import docs.src.tutorial.authentication.code002  # noqa: F401
+        import docs.src.tutorial.authentication.multiple01  # noqa: F401
+        import docs.src.tutorial.authentication.schema01  # noqa: F401
 
-        client = NinjaClient(api)
+        client = TestClient(api)
 
         response = client.get("/ipwhiltelist", META={"REMOTE_ADDR": "127.0.0.1"})
         assert response.status_code == 401
         response = client.get("/ipwhiltelist", META={"REMOTE_ADDR": "8.8.8.8"})
         assert response.status_code == 200
 
         # Api key --------------------------------
@@ -90,15 +92,15 @@
 def test_global():
     from docs.src.tutorial.authentication.global01 import api
 
     @api.get("/somemethod")
     def mustbeauthed(request):
         return {"auth": request.auth}
 
-    client = NinjaClient(api)
+    client = TestClient(api)
 
     assert client.get("/somemethod").status_code == 401
 
     resp = client.post(
         "/token", POST={"username": "admin", "password": "giraffethinnknslong"}
     )
     assert resp.status_code == 200
```

### Comparing `django-ninja-0.9.7/tests/test_docs/test_body.py` & `django_ninja-1.0a1/tests/test_docs/test_body.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from unittest.mock import patch
+
 from ninja import NinjaAPI
-from client import NinjaClient
+from ninja.testing import TestClient
 
 
 def test_examples():
-
     api = NinjaAPI()
 
     with patch("builtins.api", api, create=True):
-        import docs.src.tutorial.body.code01
-        import docs.src.tutorial.body.code02
-        import docs.src.tutorial.body.code03
+        import docs.src.tutorial.body.code01  # noqa: F401
+        import docs.src.tutorial.body.code02  # noqa: F401
+        import docs.src.tutorial.body.code03  # noqa: F401
 
-        client = NinjaClient(api)
+        client = TestClient(api)
 
         assert client.post(
             "/items", json={"name": "Katana", "price": 299.00, "quantity": 10}
         ).json() == {
             "name": "Katana",
             "description": None,
             "price": 299.0,
```

### Comparing `django-ninja-0.9.7/tests/test_docs/test_path.py` & `django_ninja-1.0a1/tests/test_docs/test_path.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 from unittest.mock import patch
+
 from ninja import NinjaAPI
-from client import NinjaClient
+from ninja.testing import TestClient
 
 
 def test_examples():
+    api = NinjaAPI()
+
+    with patch("builtins.api", api, create=True):
+        import docs.src.tutorial.path.code01  # noqa: F401
+
+        client = TestClient(api)
+
+        response = client.get("/items/123")
+        assert response.json() == {"item_id": "123"}
 
     api = NinjaAPI()
 
     with patch("builtins.api", api, create=True):
-        import docs.src.tutorial.path.code010
+        import docs.src.tutorial.path.code010  # noqa: F401
+        import docs.src.tutorial.path.code02  # noqa: F401
+
+        client = TestClient(api)
 
-        client = NinjaClient(api)
+        response = client.get("/items/123")
+        assert response.json() == {"item_id": 123}
 
         response = client.get("/events/2020/1/1")
         assert response.json() == {"date": "2020-01-01"}
         schema = api.get_openapi_schema("")
         events_params = schema["paths"]["/events/{year}/{month}/{day}"]["get"][
             "parameters"
         ]
-        # print(events_params, "!!")
         assert events_params == [
             {
                 "in": "path",
                 "name": "year",
-                "required": True,
                 "schema": {"title": "Year", "type": "integer"},
+                "required": True,
             },
             {
                 "in": "path",
                 "name": "month",
-                "required": True,
                 "schema": {"title": "Month", "type": "integer"},
+                "required": True,
             },
             {
                 "in": "path",
                 "name": "day",
-                "required": True,
                 "schema": {"title": "Day", "type": "integer"},
+                "required": True,
             },
         ]
```

### Comparing `django-ninja-0.9.7/tests/test_docs/test_query.py` & `django_ninja-1.0a1/tests/test_docs/test_query.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from unittest.mock import patch
+
 from ninja import NinjaAPI
-from client import NinjaClient
+from ninja.testing import TestClient
 
 
 def test_examples():
-
     api = NinjaAPI()
 
     with patch("builtins.api", api, create=True):
-        import docs.src.tutorial.query.code01
-        import docs.src.tutorial.query.code02
-        import docs.src.tutorial.query.code03
-        import docs.src.tutorial.query.code010
+        import docs.src.tutorial.query.code01  # noqa: F401
+        import docs.src.tutorial.query.code010  # noqa: F401
+        import docs.src.tutorial.query.code02  # noqa: F401
+        import docs.src.tutorial.query.code03  # noqa: F401
 
-        client = NinjaClient(api)
+        client = TestClient(api)
 
         # Defaults
         assert client.get("/weapons").json() == [
             "Ninjato",
             "Shuriken",
             "Katana",
             "Kama",
@@ -59,41 +59,75 @@
         assert client.get("/example?d=1577836800").json() == [None, None, "2020-01-01", None]
         assert client.get("/example?d=2020-01-01").json() == [None, None, "2020-01-01", None]
         # fmt: on
 
         # Schema
 
         assert client.get("/filter").json() == {
-            "filters": {"limit": 100, "offset": None, "query": None}
+            "filters": {
+                "limit": 100,
+                "offset": None,
+                "query": None,
+                "category__in": None,
+            }
         }
         assert client.get("/filter?limit=10").json() == {
-            "filters": {"limit": 10, "offset": None, "query": None}
+            "filters": {
+                "limit": 10,
+                "offset": None,
+                "query": None,
+                "category__in": None,
+            }
         }
         assert client.get("/filter?offset=10").json() == {
-            "filters": {"limit": 100, "offset": 10, "query": None}
+            "filters": {"limit": 100, "offset": 10, "query": None, "category__in": None}
         }
         assert client.get("/filter?query=10").json() == {
-            "filters": {"limit": 100, "offset": None, "query": "10"}
+            "filters": {
+                "limit": 100,
+                "offset": None,
+                "query": "10",
+                "category__in": None,
+            }
+        }
+        assert client.get("/filter?categories=a&categories=b").json() == {
+            "filters": {
+                "limit": 100,
+                "offset": None,
+                "query": None,
+                "category__in": ["a", "b"],
+            }
         }
 
         schema = api.get_openapi_schema("")
         params = schema["paths"]["/filter"]["get"]["parameters"]
+        # print(params)
         assert params == [
             {
                 "in": "query",
                 "name": "limit",
+                "schema": {"default": 100, "title": "Limit", "type": "integer"},
                 "required": False,
-                "schema": {"title": "Limit", "default": 100, "type": "integer"},
             },
             {
                 "in": "query",
                 "name": "offset",
-                "required": False,
                 "schema": {"title": "Offset", "type": "integer"},
+                "required": False,
             },
             {
                 "in": "query",
                 "name": "query",
-                "required": False,
                 "schema": {"title": "Query", "type": "string"},
+                "required": False,
+            },
+            {
+                "in": "query",
+                "name": "categories",
+                "schema": {
+                    "items": {"type": "string"},
+                    "title": "Categories",
+                    "type": "array",
+                },
+                "required": False,
             },
         ]
```

### Comparing `django-ninja-0.9.7/tests/test_enum.py` & `django_ninja-1.0a1/tests/test_exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from datetime import date
-from enum import Enum
-from json import encoder
-from pydantic import BaseModel
-from ninja import NinjaAPI
-from client import NinjaClient
-
-
-class RoomEnum(str, Enum):
-    double = "double"
-    twin = "twin"
-    single = "single"
-
-
-class Booking(BaseModel):
-    start: date
-    end: date
-    room: RoomEnum = RoomEnum.double
+import django
+import pytest
+from django.http import Http404
 
+from ninja import NinjaAPI, Schema
+from ninja.testing import TestAsyncClient, TestClient
 
 api = NinjaAPI()
 
 
-@api.post("/book")
-def create_booking(request, booking: Booking):
-    return booking
+class CustomException(Exception):
+    pass
 
 
-@api.get("/search")
-def booking_search(request, room: RoomEnum):
-    return {"room": room}
+@api.exception_handler(CustomException)
+def on_custom_error(request, exc):
+    return api.create_response(request, {"custom": True}, status=422)
 
 
-client = NinjaClient(api)
+class Payload(Schema):
+    test: int
 
 
-def test_enums():
-    response = client.post(
-        "/book", json={"start": "2020-01-01", "end": "2020-01-02", "room": "double"}
-    )
-    assert response.status_code == 200, response.content
-    assert response.json() == {
-        "start": "2020-01-01",
-        "end": "2020-01-02",
-        "room": "double",
-    }
-
-    response = client.post(
-        "/book", json={"start": "2020-01-01", "end": "2020-01-02", "room": "triple"}
-    )
-    assert response.status_code == 422
-
-    response = client.get("/search?room=twin")
-    assert response.status_code == 200
-    assert response.json() == {"room": "twin"}
-
-    response = client.get("/search?room=other")
-    assert response.status_code == 422
+@api.post("/error/{code}")
+def err_thrower(request, code: str, payload: Payload = None):
+    if code == "base":
+        raise RuntimeError("test")
+    if code == "404":
+        raise Http404("test")
+    if code == "custom":
+        raise CustomException("test")
 
 
-def test_schema():
-    schema = api.get_openapi_schema()
+client = TestClient(api)
 
-    from pprint import pprint
 
-    pprint(schema)
+def test_default_handler(settings):
+    settings.DEBUG = True
 
-    booking_schema = schema["components"]["schemas"]["Booking"]
-    room_prop = booking_schema["properties"]["room"]
+    response = client.post("/error/base")
+    assert response.status_code == 500
+    assert b"RuntimeError: test" in response.content
 
-    if "allOf" in room_prop:
-        # pydantic 1.7+ change:
-        assert room_prop["allOf"] == [{"$ref": "#/components/schemas/RoomEnum"}]
-    else:
-        assert room_prop == {"$ref": "#/components/schemas/RoomEnum"}
+    response = client.post("/error/404")
+    assert response.status_code == 404
+    assert response.json() == {"detail": "Not Found: test"}
 
-    assert schema["components"]["schemas"]["RoomEnum"] == {
-        "description": "An enumeration.",
-        "enum": ["double", "twin", "single"],
-        "title": "RoomEnum",
-        "type": "string",
+    response = client.post("/error/custom", body="invalid_json")
+    assert response.status_code == 400
+    assert response.json() == {
+        "detail": "Cannot parse request body (Expecting value: line 1 column 1 (char 0))",
     }
 
-    book_operation = schema["paths"]["/api/book"]["post"]
-    assert book_operation["requestBody"]["content"]["application/json"]["schema"] == {
-        "$ref": "#/components/schemas/Booking"
-    }
+    settings.DEBUG = False
+    with pytest.raises(RuntimeError):
+        response = client.post("/error/base")
+
+    response = client.post("/error/custom", body="invalid_json")
+    assert response.status_code == 400
+    assert response.json() == {"detail": "Cannot parse request body"}
+
+
+@pytest.mark.parametrize(
+    "route,status_code,json",
+    [
+        ("/error/404", 404, {"detail": "Not Found"}),
+        ("/error/custom", 422, {"custom": True}),
+    ],
+)
+def test_exceptions(route, status_code, json):
+    response = client.post(route)
+    assert response.status_code == status_code
+    assert response.json() == json
+
+
+@pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
+@pytest.mark.asyncio
+async def test_asyncio_exceptions():
+    api = NinjaAPI()
+
+    @api.get("/error")
+    async def thrower(request):
+        raise Http404("test")
+
+    client = TestAsyncClient(api)
+    response = await client.get("/error")
+    assert response.status_code == 404
+
+
+def test_no_handlers():
+    api = NinjaAPI()
+    api._exception_handlers = {}
+
+    @api.get("/error")
+    def thrower(request):
+        raise RuntimeError("test")
 
-    search_operation = schema["paths"]["/api/search"]["get"]
-    room_param = search_operation["parameters"][0]
-    assert room_param == {
-        "in": "query",
-        "name": "room",
-        "required": True,
-        "schema": {
-            "title": "RoomEnum",
-            "description": "An enumeration.",
-            "enum": ["double", "twin", "single"],
-            "type": "string",
-        },
-    }
+    client = TestClient(api)
+
+    with pytest.raises(RuntimeError):
+        client.get("/error")
```

### Comparing `django-ninja-0.9.7/tests/test_models.py` & `django_ninja-1.0a1/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
-from ninja import Router, Form, Body, Query
 from pydantic import BaseModel
-from client import NinjaClient
+
+from ninja import Form, Query, Router
+from ninja.testing import TestClient
 
 
 class SomeModel(BaseModel):
     i: int
     s: str
     f: float
 
@@ -16,15 +17,15 @@
 
 
 class SelfReference(BaseModel):
     a: int = 123
     sibling: "SelfReference" = None
 
 
-SelfReference.update_forward_refs()
+SelfReference.model_rebuild()
 
 
 router = Router()
 
 
 @router.post("/test1")
 def view1(request, some: SomeModel):
@@ -66,20 +67,20 @@
 @router.post("/model-default")
 def view6(request, obj: OtherModel = None):
     assert isinstance(obj, (OtherModel, None.__class__))
     return obj
 
 
 @router.post("/model-default2")
-def view6(request, obj: OtherModel = OtherModel(x=1, y=1)):
+def view7(request, obj: OtherModel = OtherModel(x=1, y=1)):
     assert isinstance(obj, OtherModel)
     return obj
 
 
-client = NinjaClient(router)
+client = TestClient(router)
 
 
 @pytest.mark.parametrize(
     # fmt: off
     "path,kwargs,expected_response",
     [
         (
@@ -123,25 +124,22 @@
             None,
         ),
         (
             "model-default2",
             dict(json=None),
             {"x": 1, "y": 1},
         ),
-        
     ],
     # fmt: on
 )
 def test_models(path, kwargs, expected_response):
     response = client.post(path, **kwargs)
     assert response.status_code == 200, response.content
     assert response.json() == expected_response
 
 
 def test_invalid_body():
     response = client.post("/test1", body="invalid")
-    assert response.status_code == 422, response.content
+    assert response.status_code == 400, response.content
     assert response.json() == {
-        "detail": [
-            {"loc": ["body"], "msg": "Invalid JSON", "type": "json.parse_error",}
-        ]
+        "detail": "Cannot parse request body",
     }
```

### Comparing `django-ninja-0.9.7/tests/test_openapi_schema.py` & `django_ninja-1.0a1/tests/test_with_django/schema_fixtures/test-multi-form-file.json`

 * *Files 19% similar despite different names*

```diff
@@ -1,176 +1,148 @@
-00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000010: 7274 204c 6973 740a 6672 6f6d 206e 696e  rt List.from nin
-00000020: 6a61 2069 6d70 6f72 7420 4e69 6e6a 6141  ja import NinjaA
-00000030: 5049 2c20 5363 6865 6d61 0a66 726f 6d20  PI, Schema.from 
-00000040: 646a 616e 676f 2e74 6573 7420 696d 706f  django.test impo
-00000050: 7274 2043 6c69 656e 740a 0a0a 6170 6920  rt Client...api 
-00000060: 3d20 4e69 6e6a 6141 5049 2829 0a0a 0a63  = NinjaAPI()...c
-00000070: 6c61 7373 2050 6179 6c6f 6164 2853 6368  lass Payload(Sch
-00000080: 656d 6129 3a0a 2020 2020 693a 2069 6e74  ema):.    i: int
-00000090: 0a20 2020 2066 3a20 666c 6f61 740a 0a0a  .    f: float...
-000000a0: 636c 6173 7320 5265 7370 6f6e 7365 2853  class Response(S
-000000b0: 6368 656d 6129 3a0a 2020 2020 693a 2069  chema):.    i: i
-000000c0: 6e74 0a20 2020 2066 3a20 666c 6f61 740a  nt.    f: float.
-000000d0: 0a0a 4061 7069 2e70 6f73 7428 222f 7465  ..@api.post("/te
-000000e0: 7374 222c 2072 6573 706f 6e73 653d 5265  st", response=Re
-000000f0: 7370 6f6e 7365 290a 6465 6620 6d65 7468  sponse).def meth
-00000100: 6f64 2872 6571 7565 7374 2c20 6461 7461  od(request, data
-00000110: 3a20 5061 796c 6f61 6429 3a0a 2020 2020  : Payload):.    
-00000120: 7265 7475 726e 2064 6174 612e 6469 6374  return data.dict
-00000130: 2829 0a0a 0a40 6170 692e 706f 7374 2822  ()...@api.post("
-00000140: 2f74 6573 745f 6c69 7374 222c 2072 6573  /test_list", res
-00000150: 706f 6e73 653d 4c69 7374 5b52 6573 706f  ponse=List[Respo
-00000160: 6e73 655d 290a 6465 6620 6d65 7468 6f64  nse]).def method
-00000170: 5f6c 6973 7428 7265 7175 6573 742c 2064  _list(request, d
-00000180: 6174 613a 204c 6973 745b 5061 796c 6f61  ata: List[Payloa
-00000190: 645d 293a 0a20 2020 2072 6574 7572 6e20  d]):.    return 
-000001a0: 5b5d 0a0a 0a64 6566 2074 6573 745f 7363  []...def test_sc
-000001b0: 6865 6d61 5f76 6965 7773 2863 6c69 656e  hema_views(clien
-000001c0: 743a 2043 6c69 656e 7429 3a0a 2020 2020  t: Client):.    
-000001d0: 6173 7365 7274 2063 6c69 656e 742e 6765  assert client.ge
-000001e0: 7428 222f 6170 692f 2229 2e73 7461 7475  t("/api/").statu
-000001f0: 735f 636f 6465 203d 3d20 3430 340a 2020  s_code == 404.  
-00000200: 2020 6173 7365 7274 2063 6c69 656e 742e    assert client.
-00000210: 6765 7428 222f 6170 692f 646f 6373 2229  get("/api/docs")
-00000220: 2e73 7461 7475 735f 636f 6465 203d 3d20  .status_code == 
-00000230: 3230 300a 2020 2020 6173 7365 7274 2063  200.    assert c
-00000240: 6c69 656e 742e 6765 7428 222f 6170 692f  lient.get("/api/
-00000250: 6f70 656e 6170 692e 6a73 6f6e 2229 2e73  openapi.json").s
-00000260: 7461 7475 735f 636f 6465 203d 3d20 3230  tatus_code == 20
-00000270: 300a 0a0a 6465 6620 7465 7374 5f73 6368  0...def test_sch
-00000280: 656d 6128 293a 0a20 2020 2073 6368 656d  ema():.    schem
-00000290: 6120 3d20 6170 692e 6765 745f 6f70 656e  a = api.get_open
-000002a0: 6170 695f 7363 6865 6d61 2829 0a20 2020  api_schema().   
-000002b0: 2066 726f 6d20 7070 7269 6e74 2069 6d70   from pprint imp
-000002c0: 6f72 7420 7070 7269 6e74 0a0a 2020 2020  ort pprint..    
-000002d0: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-000002e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000002f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000310: 0a20 2020 206d 6574 686f 6420 3d20 7363  .    method = sc
-00000320: 6865 6d61 5b22 7061 7468 7322 5d5b 222f  hema["paths"]["/
-00000330: 6170 692f 7465 7374 225d 5b22 706f 7374  api/test"]["post
-00000340: 225d 0a0a 2020 2020 6173 7365 7274 206d  "]..    assert m
-00000350: 6574 686f 645b 2272 6571 7565 7374 426f  ethod["requestBo
-00000360: 6479 225d 203d 3d20 7b0a 2020 2020 2020  dy"] == {.      
-00000370: 2020 2263 6f6e 7465 6e74 223a 207b 0a20    "content": {. 
-00000380: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
-00000390: 6963 6174 696f 6e2f 6a73 6f6e 223a 207b  ication/json": {
-000003a0: 2273 6368 656d 6122 3a20 7b22 2472 6566  "schema": {"$ref
-000003b0: 223a 2022 232f 636f 6d70 6f6e 656e 7473  ": "#/components
-000003c0: 2f73 6368 656d 6173 2f50 6179 6c6f 6164  /schemas/Payload
-000003d0: 227d 7d0a 2020 2020 2020 2020 7d2c 0a20  "}}.        },. 
-000003e0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000003f0: 223a 2054 7275 652c 0a20 2020 207d 0a20  ": True,.    }. 
-00000400: 2020 2061 7373 6572 7420 6d65 7468 6f64     assert method
-00000410: 5b22 7265 7370 6f6e 7365 7322 5d20 3d3d  ["responses"] ==
-00000420: 207b 0a20 2020 2020 2020 2032 3030 3a20   {.        200: 
-00000430: 7b0a 2020 2020 2020 2020 2020 2020 2263  {.            "c
-00000440: 6f6e 7465 6e74 223a 207b 0a20 2020 2020  ontent": {.     
-00000450: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
-00000460: 6963 6174 696f 6e2f 6a73 6f6e 223a 207b  ication/json": {
-00000470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000480: 2020 2020 2022 7363 6865 6d61 223a 207b       "schema": {
-00000490: 2224 7265 6622 3a20 2223 2f63 6f6d 706f  "$ref": "#/compo
-000004a0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-000004b0: 7370 6f6e 7365 227d 0a20 2020 2020 2020  sponse"}.       
-000004c0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000004d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000004e0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000004f0: 6f6e 223a 2022 4f4b 222c 0a20 2020 2020  on": "OK",.     
-00000500: 2020 207d 0a20 2020 207d 0a0a 2020 2020     }.    }..    
-00000510: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000550: 0a20 2020 206d 6574 686f 645f 6c69 7374  .    method_list
-00000560: 203d 2073 6368 656d 615b 2270 6174 6873   = schema["paths
-00000570: 225d 5b22 2f61 7069 2f74 6573 745f 6c69  "]["/api/test_li
-00000580: 7374 225d 5b22 706f 7374 225d 0a0a 2020  st"]["post"]..  
-00000590: 2020 6173 7365 7274 206d 6574 686f 645f    assert method_
-000005a0: 6c69 7374 5b22 7265 7175 6573 7442 6f64  list["requestBod
-000005b0: 7922 5d20 3d3d 207b 0a20 2020 2020 2020  y"] == {.       
-000005c0: 2022 636f 6e74 656e 7422 3a20 7b0a 2020   "content": {.  
-000005d0: 2020 2020 2020 2020 2020 2261 7070 6c69            "appli
-000005e0: 6361 7469 6f6e 2f6a 736f 6e22 3a20 7b0a  cation/json": {.
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2273 6368 656d 6122 3a20 7b0a 2020 2020  "schema": {.    
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2269 7465 6d73 223a 207b 2224 7265 6622  "items": {"$ref"
-00000630: 3a20 2223 2f63 6f6d 706f 6e65 6e74 732f  : "#/components/
-00000640: 7363 6865 6d61 732f 5061 796c 6f61 6422  schemas/Payload"
-00000650: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00000660: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
-00000670: 2244 6174 6122 2c0a 2020 2020 2020 2020  "Data",.        
-00000680: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00000690: 6522 3a20 2261 7272 6179 222c 0a20 2020  e": "array",.   
-000006a0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-000006b0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000006c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000006d0: 2272 6571 7569 7265 6422 3a20 5472 7565  "required": True
-000006e0: 2c0a 2020 2020 7d0a 2020 2020 6173 7365  ,.    }.    asse
-000006f0: 7274 206d 6574 686f 645f 6c69 7374 5b22  rt method_list["
-00000700: 7265 7370 6f6e 7365 7322 5d20 3d3d 207b  responses"] == {
-00000710: 0a20 2020 2020 2020 2032 3030 3a20 7b0a  .        200: {.
-00000720: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00000730: 7465 6e74 223a 207b 0a20 2020 2020 2020  tent": {.       
-00000740: 2020 2020 2020 2020 2022 6170 706c 6963           "applic
-00000750: 6174 696f 6e2f 6a73 6f6e 223a 207b 0a20  ation/json": {. 
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2022 7363 6865 6d61 223a 207b 0a20     "schema": {. 
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 2022 6974 656d 7322 3a20         "items": 
-000007a0: 7b22 2472 6566 223a 2022 232f 636f 6d70  {"$ref": "#/comp
-000007b0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-000007c0: 6573 706f 6e73 6522 7d2c 0a20 2020 2020  esponse"},.     
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 2020 2022 7469 746c 6522 3a20 2252 6573     "title": "Res
-000007f0: 706f 6e73 6522 2c0a 2020 2020 2020 2020  ponse",.        
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000810: 2274 7970 6522 3a20 2261 7272 6179 222c  "type": "array",
-00000820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000830: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00000840: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00000850: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000860: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000870: 223a 2022 4f4b 222c 0a20 2020 2020 2020  ": "OK",.       
-00000880: 207d 0a20 2020 207d 0a0a 2020 2020 6173   }.    }..    as
-00000890: 7365 7274 2073 6368 656d 615b 2263 6f6d  sert schema["com
-000008a0: 706f 6e65 6e74 7322 5d5b 2273 6368 656d  ponents"]["schem
-000008b0: 6173 225d 203d 3d20 7b0a 2020 2020 2020  as"] == {.      
-000008c0: 2020 2250 6179 6c6f 6164 223a 207b 0a20    "Payload": {. 
-000008d0: 2020 2020 2020 2020 2020 2022 7072 6f70             "prop
-000008e0: 6572 7469 6573 223a 207b 0a20 2020 2020  erties": {.     
-000008f0: 2020 2020 2020 2020 2020 2022 6622 3a20             "f": 
-00000900: 7b22 7469 746c 6522 3a20 2246 222c 2022  {"title": "F", "
-00000910: 7479 7065 223a 2022 6e75 6d62 6572 227d  type": "number"}
-00000920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000930: 2020 2269 223a 207b 2274 6974 6c65 223a    "i": {"title":
-00000940: 2022 4922 2c20 2274 7970 6522 3a20 2269   "I", "type": "i
-00000950: 6e74 6567 6572 227d 2c0a 2020 2020 2020  nteger"},.      
-00000960: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000970: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00000980: 205b 2269 222c 2022 6622 5d2c 0a20 2020   ["i", "f"],.   
-00000990: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-000009a0: 3a20 2250 6179 6c6f 6164 222c 0a20 2020  : "Payload",.   
-000009b0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000009c0: 2022 6f62 6a65 6374 222c 0a20 2020 2020   "object",.     
-000009d0: 2020 207d 2c0a 2020 2020 2020 2020 2252     },.        "R
-000009e0: 6573 706f 6e73 6522 3a20 7b0a 2020 2020  esponse": {.    
-000009f0: 2020 2020 2020 2020 2270 726f 7065 7274          "propert
-00000a00: 6965 7322 3a20 7b0a 2020 2020 2020 2020  ies": {.        
-00000a10: 2020 2020 2020 2020 2266 223a 207b 2274          "f": {"t
-00000a20: 6974 6c65 223a 2022 4622 2c20 2274 7970  itle": "F", "typ
-00000a30: 6522 3a20 226e 756d 6265 7222 7d2c 0a20  e": "number"},. 
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000a50: 6922 3a20 7b22 7469 746c 6522 3a20 2249  i": {"title": "I
-00000a60: 222c 2022 7479 7065 223a 2022 696e 7465  ", "type": "inte
-00000a70: 6765 7222 7d2c 0a20 2020 2020 2020 2020  ger"},.         
-00000a80: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000a90: 2020 2272 6571 7569 7265 6422 3a20 5b22    "required": ["
-00000aa0: 6922 2c20 2266 225d 2c0a 2020 2020 2020  i", "f"],.      
-00000ab0: 2020 2020 2020 2274 6974 6c65 223a 2022        "title": "
-00000ac0: 5265 7370 6f6e 7365 222c 0a20 2020 2020  Response",.     
-00000ad0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000ae0: 6f62 6a65 6374 222c 0a20 2020 2020 2020  object",.       
-00000af0: 207d 2c0a 2020 2020 7d0a                  },.    }.
+00000000: 7b0a 2020 2270 6f73 7422 3a20 7b0a 2020  {.  "post": {.  
+00000010: 2020 226f 7065 7261 7469 6f6e 4964 223a    "operationId":
+00000020: 2022 6d75 6c74 695f 7061 7261 6d5f 6170   "multi_param_ap
+00000030: 695f 7465 7374 5f6d 756c 7469 5f66 6f72  i_test_multi_for
+00000040: 6d5f 6669 6c65 222c 0a20 2020 2022 7375  m_file",.    "su
+00000050: 6d6d 6172 7922 3a20 2254 6573 7420 4d75  mmary": "Test Mu
+00000060: 6c74 6920 466f 726d 2046 696c 6522 2c0a  lti Form File",.
+00000070: 2020 2020 2270 6172 616d 6574 6572 7322      "parameters"
+00000080: 3a20 5b5d 2c0a 2020 2020 2272 6573 706f  : [],.    "respo
+00000090: 6e73 6573 223a 207b 0a20 2020 2020 2022  nses": {.      "
+000000a0: 3230 3022 3a20 7b0a 2020 2020 2020 2020  200": {.        
+000000b0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000000c0: 4f4b 222c 0a20 2020 2020 2020 2022 636f  OK",.        "co
+000000d0: 6e74 656e 7422 3a20 7b0a 2020 2020 2020  ntent": {.      
+000000e0: 2020 2020 2261 7070 6c69 6361 7469 6f6e      "application
+000000f0: 2f6a 736f 6e22 3a20 7b0a 2020 2020 2020  /json": {.      
+00000100: 2020 2020 2020 2273 6368 656d 6122 3a20        "schema": 
+00000110: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000120: 2224 7265 6622 3a20 2223 2f63 6f6d 706f  "$ref": "#/compo
+00000130: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00000140: 7370 6f6e 7365 4461 7461 220a 2020 2020  sponseData".    
+00000150: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000160: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00000170: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000180: 2020 2022 7265 7175 6573 7442 6f64 7922     "requestBody"
+00000190: 3a20 7b0a 2020 2020 2020 2263 6f6e 7465  : {.      "conte
+000001a0: 6e74 223a 207b 0a20 2020 2020 2020 2022  nt": {.        "
+000001b0: 6d75 6c74 6970 6172 742f 666f 726d 2d64  multipart/form-d
+000001c0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+000001d0: 2020 2273 6368 656d 6122 3a20 7b0a 2020    "schema": {.  
+000001e0: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+000001f0: 223a 2022 4d75 6c74 6950 6172 7442 6f64  ": "MultiPartBod
+00000200: 7950 6172 616d 7322 2c0a 2020 2020 2020  yParams",.      
+00000210: 2020 2020 2020 2274 7970 6522 3a20 226f        "type": "o
+00000220: 626a 6563 7422 2c0a 2020 2020 2020 2020  bject",.        
+00000230: 2020 2020 2270 726f 7065 7274 6965 7322      "properties"
+00000240: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000250: 2020 2266 696c 6522 3a20 7b0a 2020 2020    "file": {.    
+00000260: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+00000270: 6c65 223a 2022 4669 6c65 222c 0a20 2020  le": "File",.   
+00000280: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00000290: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000002b0: 666f 726d 6174 223a 2022 6269 6e61 7279  format": "binary
+000002c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000002d0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000002e0: 2022 6922 3a20 7b0a 2020 2020 2020 2020   "i": {.        
+000002f0: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
+00000300: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
+00000310: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
+00000320: 6e74 6567 6572 220a 2020 2020 2020 2020  nteger".        
+00000330: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000340: 2020 2020 2020 2022 7322 3a20 7b0a 2020         "s": {.  
+00000350: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00000360: 6974 6c65 223a 2022 5322 2c0a 2020 2020  itle": "S",.    
+00000370: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+00000380: 6175 6c74 223a 2022 612d 7374 7222 2c0a  ault": "a-str",.
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+000003b0: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
+000003c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000003d0: 2266 6f6f 3422 3a20 7b0a 2020 2020 2020  "foo4": {.      
+000003e0: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+000003f0: 223a 2022 466f 6f34 2054 6974 6c65 222c  ": "Foo4 Title",
+00000400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000410: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00000420: 2246 6f6f 3420 4465 7363 222c 0a20 2020  "Foo4 Desc",.   
+00000430: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00000440: 6661 756c 7422 3a20 3434 2c0a 2020 2020  fault": 44,.    
+00000450: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00000460: 6522 3a20 2269 6e74 6567 6572 220a 2020  e": "integer".  
+00000470: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000480: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+00000490: 7234 223a 207b 0a20 2020 2020 2020 2020  r4": {.         
+000004a0: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
+000004b0: 2242 6172 3422 2c0a 2020 2020 2020 2020  "Bar4",.        
+000004c0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+000004d0: 223a 2022 3434 6261 7222 2c0a 2020 2020  ": "44bar",.    
+000004e0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000004f0: 6522 3a20 2273 7472 696e 6722 0a20 2020  e": "string".   
+00000500: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000510: 2020 2020 2020 2020 2020 2020 2266 6f6f              "foo
+00000520: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000530: 2020 2020 2022 7469 746c 6522 3a20 2246       "title": "F
+00000540: 6f6f 222c 0a20 2020 2020 2020 2020 2020  oo",.           
+00000550: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
+00000560: 7465 6765 7222 0a20 2020 2020 2020 2020  teger".         
+00000570: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000580: 2020 2020 2020 2262 6172 223a 207b 0a20        "bar": {. 
+00000590: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000005a0: 7469 746c 6522 3a20 2242 6172 222c 0a20  title": "Bar",. 
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000005c0: 6465 6661 756c 7422 3a20 2231 3162 6172  default": "11bar
+000005d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000005e0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+000005f0: 6e67 220a 2020 2020 2020 2020 2020 2020  ng".            
+00000600: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00000610: 2020 2022 666f 6f32 223a 207b 0a20 2020     "foo2": {.   
+00000620: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
+00000630: 746c 6522 3a20 2246 6f6f 3220 5469 746c  tle": "Foo2 Titl
+00000640: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00000650: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000660: 223a 2022 466f 6f32 2044 6573 6322 2c0a  ": "Foo2 Desc",.
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2264 6566 6175 6c74 223a 2032 322c 0a20  "default": 22,. 
+00000690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000006a0: 7479 7065 223a 2022 696e 7465 6765 7222  type": "integer"
+000006b0: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
+000006c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000006d0: 2262 6172 3222 3a20 7b0a 2020 2020 2020  "bar2": {.      
+000006e0: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+000006f0: 223a 2022 4261 7232 222c 0a20 2020 2020  ": "Bar2",.     
+00000700: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00000710: 223a 2022 7374 7269 6e67 220a 2020 2020  ": "string".    
+00000720: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000730: 2020 2020 2020 2020 2020 2022 666f 6f33             "foo3
+00000740: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000750: 2020 2020 2022 7469 746c 6522 3a20 2246       "title": "F
+00000760: 6f6f 3320 5469 746c 6522 2c0a 2020 2020  oo3 Title",.    
+00000770: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00000780: 6372 6970 7469 6f6e 223a 2022 466f 6f33  cription": "Foo3
+00000790: 2044 6573 6322 2c0a 2020 2020 2020 2020   Desc",.        
+000007a0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+000007b0: 2269 6e74 6567 6572 220a 2020 2020 2020  "integer".      
+000007c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000007d0: 2020 2020 2020 2020 2022 6261 7233 223a           "bar3":
+000007e0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000007f0: 2020 2022 7469 746c 6522 3a20 2242 6172     "title": "Bar
+00000800: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
+00000810: 2020 2020 2264 6566 6175 6c74 223a 2022      "default": "
+00000820: 3333 6261 7222 2c0a 2020 2020 2020 2020  33bar",.        
+00000830: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000840: 2273 7472 696e 6722 0a20 2020 2020 2020  "string".       
+00000850: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000860: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000870: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00000880: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00000890: 2266 696c 6522 2c0a 2020 2020 2020 2020  "file",.        
+000008a0: 2020 2020 2020 2269 222c 0a20 2020 2020        "i",.     
+000008b0: 2020 2020 2020 2020 2022 666f 6f22 2c0a           "foo",.
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+000008d0: 6172 3222 2c0a 2020 2020 2020 2020 2020  ar2",.          
+000008e0: 2020 2020 2266 6f6f 3322 0a20 2020 2020      "foo3".     
+000008f0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00000900: 2020 207d 0a20 2020 2020 2020 207d 0a20     }.        }. 
+00000910: 2020 2020 207d 2c0a 2020 2020 2020 2272       },.      "r
+00000920: 6571 7569 7265 6422 3a20 7472 7565 0a20  equired": true. 
+00000930: 2020 207d 0a20 207d 0a7d                    }.  }.}
```

### Comparing `django-ninja-0.9.7/tests/test_path.py` & `django_ninja-1.0a1/tests/test_path.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,176 @@
 import pytest
 from main import router
-from client import NinjaClient
 
+from ninja import Router
+from ninja.testing import TestClient
 
-client = NinjaClient(router)
+client = TestClient(router)
 
 
 def test_text_get():
     response = client.get("/text")
     assert response.status_code == 200, response.text
     assert response.json() == "Hello World"
 
 
 response_not_valid_bool = {
     "detail": [
         {
+            "type": "bool_parsing",
             "loc": ["path", "item_id"],
-            "msg": "value could not be parsed to a boolean",
-            "type": "type_error.bool",
+            "msg": "Input should be a valid boolean, unable to interpret input",
         }
     ]
 }
 
 response_not_valid_int = {
     "detail": [
         {
+            "type": "int_parsing",
             "loc": ["path", "item_id"],
-            "msg": "value is not a valid integer",
-            "type": "type_error.integer",
+            "msg": "Input should be a valid integer, unable to parse string as an integer",
+        }
+    ]
+}
+
+response_not_valid_int_float = {
+    "detail": [
+        {
+            "type": "int_parsing",
+            "loc": ["path", "item_id"],
+            "msg": "Input should be a valid integer, unable to parse string as an integer",
         }
     ]
 }
 
 response_not_valid_float = {
     "detail": [
         {
+            "type": "float_parsing",
             "loc": ["path", "item_id"],
-            "msg": "value is not a valid float",
-            "type": "type_error.float",
+            "msg": "Input should be a valid number, unable to parse string as a number",
         }
     ]
 }
 
 response_at_least_3 = {
     "detail": [
         {
+            "type": "string_too_short",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value has at least 3 characters",
-            "type": "value_error.any_str.min_length",
-            "ctx": {"limit_value": 3},
+            "msg": "String should have at least 3 characters",
+            "ctx": {"min_length": 3},
         }
     ]
 }
 
 
 response_at_least_2 = {
     "detail": [
         {
+            "type": "string_too_short",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value has at least 2 characters",
-            "type": "value_error.any_str.min_length",
-            "ctx": {"limit_value": 2},
+            "msg": "String should have at least 2 characters",
+            "ctx": {"min_length": 2},
         }
     ]
 }
 
 
 response_maximum_3 = {
     "detail": [
         {
+            "type": "string_too_long",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value has at most 3 characters",
-            "type": "value_error.any_str.max_length",
-            "ctx": {"limit_value": 3},
+            "msg": "String should have at most 3 characters",
+            "ctx": {"max_length": 3},
         }
     ]
 }
 
 
 response_greater_than_3 = {
     "detail": [
         {
+            "type": "greater_than",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is greater than 3",
-            "type": "value_error.number.not_gt",
-            "ctx": {"limit_value": 3},
+            "msg": "Input should be greater than 3",
+            "ctx": {"gt": 3.0},
         }
     ]
 }
 
 
 response_greater_than_0 = {
     "detail": [
         {
+            "type": "greater_than",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is greater than 0",
-            "type": "value_error.number.not_gt",
-            "ctx": {"limit_value": 0},
+            "msg": "Input should be greater than 0",
+            "ctx": {"gt": 0.0},
         }
     ]
 }
 
 
 response_greater_than_1 = {
     "detail": [
         {
+            "type": "greater_than",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is greater than 1",
-            "type": "value_error.number.not_gt",
-            "ctx": {"limit_value": 1},
+            "msg": "Input should be greater than 1",
+            "ctx": {"gt": 1},
         }
     ]
 }
 
 
 response_greater_than_equal_3 = {
     "detail": [
         {
+            "type": "greater_than_equal",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is greater than or equal to 3",
-            "type": "value_error.number.not_ge",
-            "ctx": {"limit_value": 3},
+            "msg": "Input should be greater than or equal to 3",
+            "ctx": {"ge": 3.0},
         }
     ]
 }
 
 
 response_less_than_3 = {
     "detail": [
         {
+            "type": "less_than",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is less than 3",
-            "type": "value_error.number.not_lt",
-            "ctx": {"limit_value": 3},
+            "msg": "Input should be less than 3",
+            "ctx": {"lt": 3.0},
         }
     ]
 }
 
 
 response_less_than_0 = {
     "detail": [
         {
+            "type": "less_than",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is less than 0",
-            "type": "value_error.number.not_lt",
-            "ctx": {"limit_value": 0},
+            "msg": "Input should be less than 0",
+            "ctx": {"lt": 0.0},
         }
     ]
 }
 
-
 response_less_than_equal_3 = {
     "detail": [
         {
+            "type": "less_than_equal",
             "loc": ["path", "item_id"],
-            "msg": "ensure this value is less than or equal to 3",
-            "type": "value_error.number.not_le",
-            "ctx": {"limit_value": 3},
+            "msg": "Input should be less than or equal to 3",
+            "ctx": {"le": 3.0},
         }
     ]
 }
 
 
 @pytest.mark.parametrize(
     "path,expected_status,expected_response",
@@ -168,15 +178,15 @@
         ("/path/foobar", 200, "foobar"),
         ("/path/str/foobar", 200, "foobar"),
         ("/path/str/42", 200, "42"),
         ("/path/str/True", 200, "True"),
         ("/path/int/foobar", 422, response_not_valid_int),
         ("/path/int/True", 422, response_not_valid_int),
         ("/path/int/42", 200, 42),
-        ("/path/int/42.5", 422, response_not_valid_int),
+        ("/path/int/42.5", 422, response_not_valid_int_float),
         ("/path/float/foobar", 422, response_not_valid_float),
         ("/path/float/True", 422, response_not_valid_float),
         ("/path/float/42", 200, 42),
         ("/path/float/42.5", 200, 42.5),
         ("/path/bool/foobar", 422, response_not_valid_bool),
         ("/path/bool/True", 200, True),
         ("/path/bool/42", 422, response_not_valid_bool),
@@ -214,34 +224,117 @@
         ("/path/param-lt-gt/0", 422, response_greater_than_1),
         ("/path/param-le-ge/2", 200, 2),
         ("/path/param-le-ge/1", 200, 1),
         ("/path/param-le-ge/3", 200, 3),
         ("/path/param-le-ge/4", 422, response_less_than_equal_3),
         ("/path/param-lt-int/2", 200, 2),
         ("/path/param-lt-int/42", 422, response_less_than_3),
-        ("/path/param-lt-int/2.7", 422, response_not_valid_int),
+        ("/path/param-lt-int/2.7", 422, response_not_valid_int_float),
         ("/path/param-gt-int/42", 200, 42),
         ("/path/param-gt-int/2", 422, response_greater_than_3),
-        ("/path/param-gt-int/2.7", 422, response_not_valid_int),
+        ("/path/param-gt-int/2.7", 422, response_not_valid_int_float),
         ("/path/param-le-int/42", 422, response_less_than_equal_3),
         ("/path/param-le-int/3", 200, 3),
         ("/path/param-le-int/2", 200, 2),
-        ("/path/param-le-int/2.7", 422, response_not_valid_int),
+        ("/path/param-le-int/2.7", 422, response_not_valid_int_float),
         ("/path/param-ge-int/42", 200, 42),
         ("/path/param-ge-int/3", 200, 3),
         ("/path/param-ge-int/2", 422, response_greater_than_equal_3),
-        ("/path/param-ge-int/2.7", 422, response_not_valid_int),
+        ("/path/param-ge-int/2.7", 422, response_not_valid_int_float),
         ("/path/param-lt-gt-int/2", 200, 2),
         ("/path/param-lt-gt-int/4", 422, response_less_than_3),
         ("/path/param-lt-gt-int/0", 422, response_greater_than_1),
-        ("/path/param-lt-gt-int/2.7", 422, response_not_valid_int),
+        ("/path/param-lt-gt-int/2.7", 422, response_not_valid_int_float),
         ("/path/param-le-ge-int/2", 200, 2),
         ("/path/param-le-ge-int/1", 200, 1),
         ("/path/param-le-ge-int/3", 200, 3),
         ("/path/param-le-ge-int/4", 422, response_less_than_equal_3),
-        ("/path/param-le-ge-int/2.7", 422, response_not_valid_int),
+        ("/path/param-le-ge-int/2.7", 422, response_not_valid_int_float),
     ],
 )
 def test_get_path(path, expected_status, expected_response):
     response = client.get(path)
+    print(path, response.json())
     assert response.status_code == expected_status
     assert response.json() == expected_response
+
+
+@pytest.mark.parametrize(
+    "path,expected_status,expected_response",
+    [
+        ("/path/param-django-str/42", 200, "42"),
+        ("/path/param-django-str/-1", 200, "-1"),
+        ("/path/param-django-str/foobar", 200, "foobar"),
+        ("/path/param-django-int/0", 200, 0),
+        ("/path/param-django-int/42", 200, 42),
+        ("/path/param-django-int/42.5", "Cannot resolve", Exception),
+        ("/path/param-django-int/-1", "Cannot resolve", Exception),
+        ("/path/param-django-int/True", "Cannot resolve", Exception),
+        ("/path/param-django-int/foobar", "Cannot resolve", Exception),
+        ("/path/param-django-int/not-an-int", 200, "Found not-an-int"),
+        # ("/path/param-django-int-str/42", 200, "42"), # https://github.com/pydantic/pydantic/issues/5993
+        ("/path/param-django-int-str/42.5", "Cannot resolve", Exception),
+        (
+            "/path/param-django-slug/django-ninja-is-the-best",
+            200,
+            "django-ninja-is-the-best",
+        ),
+        ("/path/param-django-slug/42.5", "Cannot resolve", Exception),
+        (
+            "/path/param-django-uuid/31ea378c-c052-4b4c-bf0b-679ce5cfcc2a",
+            200,
+            "31ea378c-c052-4b4c-bf0b-679ce5cfcc2a",
+        ),
+        (
+            "/path/param-django-uuid/31ea378c-c052-4b4c-bf0b-679ce5cfcc2",
+            "Cannot resolve",
+            Exception,
+        ),
+        (
+            "/path/param-django-uuid-str/31ea378c-c052-4b4c-bf0b-679ce5cfcc2a",
+            200,
+            "31ea378c-c052-4b4c-bf0b-679ce5cfcc2a",
+        ),
+        ("/path/param-django-path/some/path/things/after", 200, "some/path/things"),
+        ("/path/param-django-path/less/path/after", 200, "less/path"),
+        ("/path/param-django-path/plugh/after", 200, "plugh"),
+        ("/path/param-django-path//after", "Cannot resolve", Exception),
+        ("/path/param-django-custom-int/42", 200, 24),
+        ("/path/param-django-custom-int/x42", "Cannot resolve", Exception),
+        ("/path/param-django-custom-float/42", 200, 0.24),
+        ("/path/param-django-custom-float/x42", "Cannot resolve", Exception),
+    ],
+)
+def test_get_path_django(path, expected_status, expected_response):
+    if expected_response == Exception:
+        with pytest.raises(Exception, match=expected_status):
+            client.get(path)
+    else:
+        response = client.get(path)
+        print(response.json())
+        assert response.status_code == expected_status
+        assert response.json() == expected_response
+
+
+def test_path_signature_asserts_default():
+    test_router = Router()
+
+    match = "'item_id' is a path param, default not allowed"
+    with pytest.raises(AssertionError, match=match):
+
+        @test_router.get("/path/{item_id}")
+        def get_path_item_id(request, item_id="1"):
+            pass
+
+
+def test_path_signature_warns_missing():
+    test_router = Router()
+
+    match = (
+        r"Field\(s\) \('a_path_param', 'another_path_param'\) are in "
+        r"the view path, but were not found in the view signature."
+    )
+    with pytest.warns(UserWarning, match=match):
+
+        @test_router.get("/path/{a_path_param}/{another_path_param}")
+        def get_path_item_id(request):
+            pass
```

### Comparing `django-ninja-0.9.7/tests/test_query.py` & `django_ninja-1.0a1/tests/test_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import pytest
 from main import router
-from client import NinjaClient
 
+from ninja.testing import TestClient
 
 response_missing = {
     "detail": [
         {
+            "type": "missing",
             "loc": ["query", "query"],
-            "msg": "field required",
-            "type": "value_error.missing",
+            "msg": "Field required",
         }
     ]
 }
 
 response_not_valid_int = {
     "detail": [
         {
+            "type": "int_parsing",
             "loc": ["query", "query"],
-            "msg": "value is not a valid integer",
-            "type": "type_error.integer",
+            "msg": "Input should be a valid integer, unable to parse string as an integer",
+        }
+    ]
+}
+
+response_not_valid_int_float = {
+    "detail": [
+        {
+            "type": "int_parsing",
+            "loc": ["query", "query"],
+            "msg": "Input should be a valid integer, unable to parse string as an integer",
         }
     ]
 }
 
 
-client = NinjaClient(router)
+client = TestClient(router)
 
 
 @pytest.mark.parametrize(
     "path,expected_status,expected_response",
     [
         ("/query", 422, response_missing),
         ("/query?query=baz", 200, "foo bar baz"),
         ("/query?not_declared=baz", 422, response_missing),
         ("/query/optional", 200, "foo bar"),
         ("/query/optional?query=baz", 200, "foo bar baz"),
         ("/query/optional?not_declared=baz", 200, "foo bar"),
         ("/query/int", 422, response_missing),
         ("/query/int?query=42", 200, "foo bar 42"),
-        ("/query/int?query=42.5", 422, response_not_valid_int),
+        ("/query/int?query=42.5", 422, response_not_valid_int_float),
         ("/query/int?query=baz", 422, response_not_valid_int),
         ("/query/int?not_declared=baz", 422, response_missing),
         ("/query/int/optional", 200, "foo bar"),
         ("/query/int/optional?query=50", 200, "foo bar 50"),
         ("/query/int/optional?query=foo", 422, response_not_valid_int),
         ("/query/int/default", 200, "foo bar 10"),
         ("/query/int/default?query=50", 200, "foo bar 50"),
@@ -50,13 +60,16 @@
         ("/query/param", 200, "foo bar"),
         ("/query/param?query=50", 200, "foo bar 50"),
         ("/query/param-required", 422, response_missing),
         ("/query/param-required?query=50", 200, "foo bar 50"),
         ("/query/param-required/int", 422, response_missing),
         ("/query/param-required/int?query=50", 200, "foo bar 50"),
         ("/query/param-required/int?query=foo", 422, response_not_valid_int),
+        ("/query/aliased-name?aliased.-_~name=foo", 200, "foo bar foo"),
     ],
 )
 def test_get_path(path, expected_status, expected_response):
     response = client.get(path)
+    resp = response.json()
+    print(resp)
     assert response.status_code == expected_status
-    assert response.json() == expected_response
+    assert resp == expected_response
```

### Comparing `django-ninja-0.9.7/tests/test_request.py` & `django_ninja-1.0a1/tests/test_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
-from ninja import Router, Cookie, Header
-from client import NinjaClient
+
+from ninja import Cookie, Header, Router
+from ninja.testing import TestClient
 
 router = Router()
 
 
 @router.get("/headers1")
 def headers1(request, user_agent: str = Header(...)):
     return user_agent
@@ -21,39 +22,58 @@
 
 
 @router.get("/headers4")
 def headers4(request, c_len: int = Header(..., alias="Content-length")):
     return c_len
 
 
+@router.get("/headers5")
+def headers5(request, missing: int = Header(...)):
+    return missing
+
+
 @router.get("/cookies1")
 def cookies1(request, weapon: str = Cookie(...)):
     return weapon
 
 
 @router.get("/cookies2")
 def cookies2(request, wpn: str = Cookie(..., alias="weapon")):
     return wpn
 
 
-client = NinjaClient(router)
+client = TestClient(router)
 
 
 @pytest.mark.parametrize(
     "path,expected_status,expected_response",
     [
         ("/headers1", 200, "Ninja"),
         ("/headers2", 200, "Ninja"),
         ("/headers3", 200, 10),
         ("/headers4", 200, 10),
+        (
+            "/headers5",
+            422,
+            {
+                "detail": [
+                    {
+                        "type": "missing",
+                        "loc": ["header", "missing"],
+                        "msg": "Field required",
+                    }
+                ]
+            },
+        ),
         ("/cookies1", 200, "shuriken"),
         ("/cookies2", 200, "shuriken"),
     ],
 )
 def test_headers(path, expected_status, expected_response):
     response = client.get(
         path,
         headers={"User-Agent": "Ninja", "Content-Length": "10"},
         COOKIES={"weapon": "shuriken"},
     )
     assert response.status_code == expected_status, response.content
+    print(response.json())
     assert response.json() == expected_response
```

### Comparing `django-ninja-0.9.7/tests/test_response_multiple.py` & `django_ninja-1.0a1/tests/test_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,159 @@
-from ninja.errors import ConfigError
-import pytest
-from pydantic import ValidationError, BaseModel
-from ninja import NinjaAPI
-from client import NinjaClient
+import json
+from ipaddress import IPv4Address, IPv6Address
 from typing import List, Union
 
+import pytest
+from django.http import HttpResponse
+from pydantic import BaseModel, ValidationError
+
+from ninja import Router
+from ninja.responses import Response
+from ninja.testing import TestClient
 
-api = NinjaAPI()
+router = Router()
 
 
-@api.get("/check_int", response={200: int})
+@router.get("/check_int", response=int)
 def check_int(request):
-    return 200, "1"
+    return "1"
 
 
-@api.get("/check_int2", response={200: int})
+@router.get("/check_int2", response=int)
 def check_int2(request):
-    return 200, "str"
-
-
-@api.get("/check_single_with_status", response=int)
-def check_single_with_status(request):
-    return 302, 1
-
-
-@api.get("/check_response_schema", response={400: int})
-def check_response_schema(request):
-    return 200, 1
+    return "str"
 
 
 class User:
-    def __init__(self, id, name, password):
+    def __init__(self, id, user_name, password):
         self.id = id
-        self.name = name
+        self.user_name = user_name
         self.password = password
 
 
+def to_camel(string: str) -> str:
+    return "".join(word.capitalize() for word in string.split("_"))
+
+
 class UserModel(BaseModel):
     id: int
-    name: str
+    user_name: str
     # skipping password output to responses
 
     class Config:
-        orm_mode = True
-
+        from_attributes = True
+        alias_generator = to_camel
+        populate_by_name = True
 
-class ErrorModel(BaseModel):
-    detail: str
 
-
-@api.get("/check_model", response={200: UserModel, 202: UserModel})
+@router.get("/check_model", response=UserModel)
 def check_model(request):
-    return 202, User(1, "John", "Password")
+    return User(1, "John", "Password")
 
 
-@api.get("/check_list_model", response={200: List[UserModel]})
+@router.get("/check_list_model", response=List[UserModel])
 def check_list_model(request):
-    return 200, [User(1, "John", "Password")]
+    return [User(1, "John", "Password")]
+
 
+@router.get("/check_model_alias", response=UserModel, by_alias=True)
+def check_model_alias(request):
+    return User(1, "John", "Password")
 
-@api.get("/check_union", response={200: Union[int, UserModel], 400: ErrorModel})
+
+@router.get("/check_union", response=Union[int, UserModel])
 def check_union(request, q: int):
     if q == 0:
-        return 200, 1
+        return 1
     if q == 1:
-        return 200, User(1, "John", "Password")
-    if q == 2:
-        return 400, {"detail": "error"}
+        return User(1, "John", "Password")
     return "invalid"
 
 
-client = NinjaClient(api)
+@router.get("/check_set_header")
+def check_set_header(request, response: HttpResponse):
+    response["Cache-Control"] = "no-cache"
+    return 1
+
+
+@router.get("/check_set_cookie")
+def check_set_cookie(request, set: bool, response: HttpResponse):
+    if set:
+        response.set_cookie("test", "me")
+    return 1
+
+
+@router.get("/check_del_cookie")
+def check_del_cookie(request, response: HttpResponse):
+    response.delete_cookie("test")
+    return 1
+
+
+client = TestClient(router)
 
 
 @pytest.mark.parametrize(
-    "path,expected_status,expected_response",
+    "path,expected_response",
     [
-        ("/check_int", 200, 1),
-        ("/check_single_with_status", 302, 1),
-        ("/check_model", 202, {"id": 1, "name": "John"}),  # the password is skipped
+        ("/check_int", 1),
+        ("/check_model", {"id": 1, "user_name": "John"}),  # the password is skipped
         (
             "/check_list_model",
-            200,
-            [{"id": 1, "name": "John"}],
+            [{"id": 1, "user_name": "John"}],
         ),  # the password is skipped
-        ("/check_union?q=0", 200, 1),
-        ("/check_union?q=1", 200, {"id": 1, "name": "John"}),
-        ("/check_union?q=2", 400, {"detail": "error"}),
+        ("/check_model", {"id": 1, "user_name": "John"}),  # the password is skipped
+        ("/check_model_alias", {"Id": 1, "UserName": "John"}),  # result is Camal Case
+        ("/check_union?q=0", 1),
+        ("/check_union?q=1", {"id": 1, "user_name": "John"}),
     ],
 )
-def test_responses(path, expected_status, expected_response):
+def test_responses(path, expected_response):
     response = client.get(path)
-    assert response.status_code == expected_status, response.content
+    assert response.status_code == 200, response.content
     assert response.json() == expected_response
 
 
-def test_schema():
-    checks = [
-        ("/api/check_int", {200}),
-        ("/api/check_int2", {200}),
-        ("/api/check_single_with_status", {200}),
-        ("/api/check_response_schema", {400}),
-        ("/api/check_model", {200, 202}),
-        ("/api/check_list_model", {200}),
-        ("/api/check_union", {200, 400}),
-    ]
-    schema = api.get_openapi_schema()
-
-    # checking codes
-    for path, codes in checks:
-        responses = schema["paths"][path]["get"]["responses"]
-        responses_codes = set(responses.keys())
-        assert codes == responses_codes, f"{codes} != {responses_codes}"
-
-    # checking model
-    check_model_responses = schema["paths"]["/api/check_model"]["get"]["responses"]
-
-    assert check_model_responses == {
-        200: {
-            "content": {
-                "application/json": {
-                    "schema": {"$ref": "#/components/schemas/UserModel"}
-                }
-            },
-            "description": "OK",
-        },
-        202: {
-            "content": {
-                "application/json": {
-                    "schema": {"$ref": "#/components/schemas/UserModel"}
-                }
-            },
-            "description": "OK",
-        },
-    }
-
-
 def test_validates():
     with pytest.raises(ValidationError):
         client.get("/check_int2")
 
     with pytest.raises(ValidationError):
-        client.get("/check_union?q=3")
+        client.get("/check_union?q=2")
+
+
+def test_set_header():
+    response = client.get("/check_set_header")
+    assert response.status_code == 200
+    assert response.content == b"1"
+    assert response["Cache-Control"] == "no-cache"
+
+
+def test_set_cookie():
+    response = client.get("/check_set_cookie?set=0")
+    assert "test" not in response.cookies
+
+    response = client.get("/check_set_cookie?set=1")
+    cookie = response.cookies.get("test")
+    assert cookie
+    assert cookie.value == "me"
+
+
+def test_del_cookie():
+    response = client.get("/check_del_cookie")
+    cookie = response.cookies.get("test")
+    assert cookie
+    assert cookie["expires"] == "Thu, 01 Jan 1970 00:00:00 GMT"
+    assert cookie["max-age"] == 0
+
+
+def test_ipv4address_encoding():
+    data = {"ipv4": IPv4Address("127.0.0.1")}
+    response = Response(data)
+    response_data = json.loads(response.content)
+    assert response_data["ipv4"] == str(data["ipv4"])
+
 
-    with pytest.raises(ConfigError):
-        client.get("/check_response_schema")
+def test_ipv6address_encoding():
+    data = {"ipv6": IPv6Address("::1")}
+    response = Response(data)
+    response_data = json.loads(response.content)
+    assert response_data["ipv6"] == str(data["ipv6"])
```

