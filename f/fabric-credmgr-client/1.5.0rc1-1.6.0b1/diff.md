# Comparing `tmp/fabric-credmgr-client-1.5.0rc1.tar.gz` & `tmp/fabric-credmgr-client-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.5.0rc1.tar", last modified: Thu May 11 18:09:36 2023, max compression
+gzip compressed data, was "fabric-credmgr-client-1.6.0b1.tar", last modified: Wed Jul 12 19:47:38 2023, max compression
```

## Comparing `fabric-credmgr-client-1.5.0rc1.tar` & `fabric-credmgr-client-1.6.0b1.tar`

### file list

```diff
@@ -1,90 +1,98 @@
--rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.5.0rc1/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.5.0rc1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-05-11 18:03:22.616419 fabric-credmgr-client-1.5.0rc1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.5.0rc1/.travis.yml
--rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.5.0rc1/LICENSE
--rw-r--r--   0        0        0     4211 2023-05-11 18:03:22.617008 fabric-credmgr-client-1.5.0rc1/README.md
--rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.5.0rc1/docs/DefaultApi.md
--rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.5.0rc1/docs/Jwks.md
--rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.5.0rc1/docs/JwksKeys.md
--rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.5.0rc1/docs/Request.md
--rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContent.md
--rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContentData.md
--rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.5.0rc1/docs/Status200OkSingle.md
--rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequest.md
--rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequestErrors.md
--rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.5.0rc1/docs/Status401Unauthorized.md
--rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.5.0rc1/docs/Status401UnauthorizedErrors.md
--rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.5.0rc1/docs/Status403Forbidden.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.5.0rc1/docs/Status403ForbiddenErrors.md
--rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFound.md
--rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFoundErrors.md
--rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerError.md
--rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerErrorErrors.md
--rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.5.0rc1/docs/Success.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.619089 fabric-credmgr-client-1.5.0rc1/docs/Token.md
--rw-r--r--   0        0        0      339 2023-05-11 18:03:22.619217 fabric-credmgr-client-1.5.0rc1/docs/Tokens.md
--rw-r--r--   0        0        0     5090 2023-05-11 18:03:22.619366 fabric-credmgr-client-1.5.0rc1/docs/TokensApi.md
--rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.5.0rc1/docs/Version.md
--rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.5.0rc1/docs/VersionApi.md
--rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.5.0rc1/docs/VersionData.md
--rw-r--r--   0        0        0       50 2023-05-11 18:06:29.691397 fabric-credmgr-client-1.5.0rc1/fabric_cm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/__init__.py
--rw-r--r--   0        0        0     6006 2023-05-11 18:03:22.620379 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py
--rw-r--r--   0        0        0     2545 2023-05-11 18:03:22.620670 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py
--rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0        0        0    12548 2023-05-11 18:03:22.621635 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25120 2023-05-11 18:03:22.622136 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0        0        0     7980 2023-05-11 18:03:22.622439 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py
--rw-r--r--   0        0        0     2143 2023-05-11 18:03:22.622732 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     4831 2023-05-11 18:03:22.626321 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0        0        0     3394 2023-05-11 18:03:22.626505 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.5.0rc1/git_push.sh
--rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.628116 fabric-credmgr-client-1.5.0rc1/test/__init__.py
--rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.5.0rc1/test/test_default_api.py
--rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.5.0rc1/test/test_jwks.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py
--rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.5.0rc1/test/test_request.py
--rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.5.0rc1/test/test_token.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.5.0rc1/test/test_tokens.py
--rw-r--r--   0        0        0     1173 2023-05-11 18:03:22.632206 fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py
--rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.5.0rc1/test/test_version.py
--rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.5.0rc1/test/test_version_api.py
--rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.5.0rc1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.5.0rc1/tox.ini
--rw-r--r--   0        0        0     5196 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b1/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b1/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b1/LICENSE
+-rw-r--r--   0        0        0     4901 2023-07-03 21:15:47.092949 fabric-credmgr-client-1.6.0b1/README.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b1/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b1/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b1/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b1/docs/Request.md
+-rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b1/docs/RevokeList.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b1/docs/Status200OkPaginated.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b1/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b1/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b1/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b1/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b1/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b1/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b1/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b1/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b1/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b1/docs/Success.md
+-rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b1/docs/Token.md
+-rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b1/docs/TokenPost.md
+-rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b1/docs/Tokens.md
+-rw-r--r--   0        0        0    12455 2023-07-03 21:25:53.675903 fabric-credmgr-client-1.6.0b1/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b1/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b1/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b1/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-07-03 21:25:53.679973 fabric-credmgr-client-1.6.0b1/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0     9229 2023-07-05 18:31:15.572470 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    29459 2023-07-05 15:55:57.673036 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25120 2023-07-05 15:48:03.304939 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2387 2023-06-27 22:04:30.468722 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/revoke_list.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token_post.py
+-rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b1/git_push.sh
+-rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b1/test/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b1/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b1/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b1/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b1/test/test_request.py
+-rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b1/test/test_revoke_list.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b1/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b1/test/test_tokens.py
+-rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b1/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b1/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b1/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b1/tox.ini
+-rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b1/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.5.0rc1/.gitignore` & `fabric-credmgr-client-1.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/.swagger-codegen-ignore` & `fabric-credmgr-client-1.6.0b1/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/LICENSE` & `fabric-credmgr-client-1.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/README.md` & `fabric-credmgr-client-1.6.0b1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -76,43 +76,50 @@
 except ApiException as e:
     print("Exception when calling CredmgrProxy->revoke: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://127.0.0.1:7000/*
+All URIs are relative to *http://127.0.0.1:7000/credmgr/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**certs_get**](docs/DefaultApi.md#certs_get) | **GET** /certs | Return Public Keys to verify signature of the tokens
 *TokensApi* | [**tokens_create_post**](docs/TokensApi.md#tokens_create_post) | **POST** /tokens/create | Generate tokens for an user
+*TokensApi* | [**tokens_get**](docs/TokensApi.md#tokens_get) | **GET** /tokens | Get tokens
 *TokensApi* | [**tokens_refresh_post**](docs/TokensApi.md#tokens_refresh_post) | **POST** /tokens/refresh | Refresh tokens for an user
-*TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a refresh token for an user
+*TokensApi* | [**tokens_revoke_list_get**](docs/TokensApi.md#tokens_revoke_list_get) | **GET** /tokens/revoke_list | Get token revoke list i.e. list of revoked identity token hashes
+*TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a token for an user
+*TokensApi* | [**tokens_revokes_post**](docs/TokensApi.md#tokens_revokes_post) | **POST** /tokens/revokes | Revoke a token
+*TokensApi* | [**tokens_validate_post**](docs/TokensApi.md#tokens_validate_post) | **POST** /tokens/validate | Validate an identity token issued by Credential Manager
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
  - [Jwks](docs/Jwks.md)
  - [JwksKeys](docs/JwksKeys.md)
  - [Request](docs/Request.md)
+ - [RevokeList](docs/RevokeList.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
+ - [Status200OkPaginated](docs/Status200OkPaginated.md)
  - [Status200OkSingle](docs/Status200OkSingle.md)
  - [Status400BadRequest](docs/Status400BadRequest.md)
  - [Status400BadRequestErrors](docs/Status400BadRequestErrors.md)
  - [Status401Unauthorized](docs/Status401Unauthorized.md)
  - [Status401UnauthorizedErrors](docs/Status401UnauthorizedErrors.md)
  - [Status403Forbidden](docs/Status403Forbidden.md)
  - [Status403ForbiddenErrors](docs/Status403ForbiddenErrors.md)
  - [Status404NotFound](docs/Status404NotFound.md)
  - [Status404NotFoundErrors](docs/Status404NotFoundErrors.md)
  - [Status500InternalServerError](docs/Status500InternalServerError.md)
  - [Status500InternalServerErrorErrors](docs/Status500InternalServerErrorErrors.md)
  - [Token](docs/Token.md)
+ - [TokenPost](docs/TokenPost.md)
  - [Tokens](docs/Tokens.md)
  - [Version](docs/Version.md)
  - [VersionData](docs/VersionData.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
```

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/DefaultApi.md` & `fabric-credmgr-client-1.6.0b1/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/JwksKeys.md` & `fabric-credmgr-client-1.6.0b1/docs/JwksKeys.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContent.md` & `fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContent.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequestErrors.md` & `fabric-credmgr-client-1.6.0b1/docs/Status400BadRequestErrors.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status401Unauthorized.md` & `fabric-credmgr-client-1.6.0b1/docs/Status401Unauthorized.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status403Forbidden.md` & `fabric-credmgr-client-1.6.0b1/docs/Status403Forbidden.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status404NotFound.md` & `fabric-credmgr-client-1.6.0b1/docs/Status404NotFound.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerError.md` & `fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerError.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/docs/VersionApi.md` & `fabric-credmgr-client-1.6.0b1/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import enum
 import json
+import traceback
 from datetime import datetime
-from typing import Tuple, Any
+from typing import Tuple, Any, List, Union
 
 from atomicwrites import atomic_write
 
 from fabric_cm.credmgr import swagger_client
+from fabric_cm.credmgr.swagger_client import Token
 from fabric_cm.credmgr.swagger_client.rest import ApiException as CredMgrException
 
 
 @enum.unique
 class Status(enum.Enum):
     OK = 1
     INVALID_ARGUMENTS = 2
@@ -48,36 +50,87 @@
           }
         if exception is None:
             return interpretations[self.value]
         else:
             return str(exception) + ". " + interpretations[self.value]
 
 
+class TokenState(enum.Enum):
+    Nascent = enum.auto(),
+    Valid = enum.auto(),
+    Refreshed = enum.auto(),
+    Revoked = enum.auto(),
+    Expired = enum.auto(),
+
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return self.name
+
+    @staticmethod
+    def state_from_str(state: str):
+        if state is None:
+            return state
+
+        for t in TokenState:
+            if state == str(t):
+                return t
+
+        return None
+
+    @staticmethod
+    def state_list_to_str_list(states: list):
+        if states is None:
+            result = []
+
+            for t in TokenState:
+                result.append(str(t))
+            return result
+
+        result = []
+        for t in states:
+            result.append(str(t))
+
+        return result
+
+
 class CredmgrProxy:
     """
     Credential Manager Proxy
     """
     ID_TOKEN = "id_token"
     REFRESH_TOKEN = "refresh_token"
-    TIME_FORMAT = "%Y-%m-%d %H:%M:%S"
+    TIME_FORMAT = "%Y-%m-%d %H:%M:%S %z"
     CREATED_AT = "created_at"
     ERROR = "error"
+    PROP_AUTHORIZATION = 'Authorization'
+    PROP_BEARER = 'Bearer'
 
     def __init__(self, credmgr_host: str):
         self.host = credmgr_host
         self.tokens_api = None
         if credmgr_host is not None:
             # create an instance of the API class
             configuration = swagger_client.configuration.Configuration()
             configuration.host = f"https://{credmgr_host}/credmgr/"
             api_instance = swagger_client.ApiClient(configuration)
             self.tokens_api = swagger_client.TokensApi(api_client=api_instance)
             self.default_api = swagger_client.DefaultApi(api_client=api_instance)
             self.version_api = swagger_client.VersionApi(api_client=api_instance)
 
+    def __set_tokens(self, *, token: str):
+        """
+        Set tokens
+        @param token token
+        """
+        # Set the tokens
+        self.tokens_api.api_client.configuration.api_key[self.PROP_AUTHORIZATION] = token
+        self.tokens_api.api_client.configuration.api_key_prefix[self.PROP_AUTHORIZATION] = self.PROP_BEARER
+
     def refresh(self, project_id: str, scope: str, refresh_token: str,
                 file_name: str = None) -> Tuple[Status, dict]:
         """
         Refresh token
         @param project_id Project Id
         @param scope scope
         @param refresh_token refresh token
@@ -153,7 +206,52 @@
         Return Version
         """
         try:
             version = self.version_api.version_get()
             return Status.OK, version
         except CredMgrException as e:
             return Status.FAILURE, e.body
+
+    def tokens(self, *, token: str, project_id: str = None, expires: str = None, states: List[TokenState] = None,
+               limit: int = 200, offset: int = 0, token_hash: str = None,) -> Tuple[Status, Union[Exception, List[Token]]]:
+        """
+        Return list of tokens issued to a user
+        @return list of tokens
+        """
+        if token is None:
+            return Status.INVALID_ARGUMENTS, CredMgrException(f"Token {token} must be specified")
+
+        try:
+            # Set the tokens
+            self.__set_tokens(token=token)
+
+            if expires is not None:
+                expiry_time = datetime.strptime(expires, self.TIME_FORMAT)
+            else:
+                expiry_time = None
+
+            tokens = self.tokens_api.tokens_get(states=TokenState.state_list_to_str_list(states=states), limit=limit,
+                                                offset=offset, token_hash=token_hash, project_id=project_id,
+                                                expires=expiry_time)
+
+            return Status.OK, tokens.data if tokens.data is not None else []
+        except Exception as e:
+            return Status.FAILURE, e
+
+    def token_revoke_list(self, *, token: str, project_id: str) -> Tuple[Status, Union[Exception, List[str]]]:
+        """
+        Return list of revoked tokens for a user
+        @return list of revoked tokens
+        """
+        if token is None or project_id is None:
+            return Status.INVALID_ARGUMENTS, CredMgrException(f"Token {token} and "
+                                                              f"Project Id {project_id} must be specified")
+
+        try:
+            # Set the tokens
+            self.__set_tokens(token=token)
+
+            slices = self.tokens_api.tokens_revoke_list_get(project_id=project_id)
+
+            return Status.OK, slices.data if slices.data is not None else []
+        except Exception as e:
+            return Status.FAILURE, e
```

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 # import ApiClient
 from fabric_cm.credmgr.swagger_client.api_client import ApiClient
 from fabric_cm.credmgr.swagger_client.configuration import Configuration
 # import models into sdk package
 from fabric_cm.credmgr.swagger_client.models.jwks import Jwks
 from fabric_cm.credmgr.swagger_client.models.jwks_keys import JwksKeys
 from fabric_cm.credmgr.swagger_client.models.request import Request
+from fabric_cm.credmgr.swagger_client.models.revoke_list import RevokeList
 from fabric_cm.credmgr.swagger_client.models.status200_ok_no_content import Status200OkNoContent
 from fabric_cm.credmgr.swagger_client.models.status200_ok_no_content_data import Status200OkNoContentData
+from fabric_cm.credmgr.swagger_client.models.status200_ok_paginated import Status200OkPaginated
 from fabric_cm.credmgr.swagger_client.models.status200_ok_single import Status200OkSingle
 from fabric_cm.credmgr.swagger_client.models.status400_bad_request import Status400BadRequest
 from fabric_cm.credmgr.swagger_client.models.status400_bad_request_errors import Status400BadRequestErrors
 from fabric_cm.credmgr.swagger_client.models.status401_unauthorized import Status401Unauthorized
 from fabric_cm.credmgr.swagger_client.models.status401_unauthorized_errors import Status401UnauthorizedErrors
 from fabric_cm.credmgr.swagger_client.models.status403_forbidden import Status403Forbidden
 from fabric_cm.credmgr.swagger_client.models.status403_forbidden_errors import Status403ForbiddenErrors
 from fabric_cm.credmgr.swagger_client.models.status404_not_found import Status404NotFound
 from fabric_cm.credmgr.swagger_client.models.status404_not_found_errors import Status404NotFoundErrors
 from fabric_cm.credmgr.swagger_client.models.status500_internal_server_error import Status500InternalServerError
 from fabric_cm.credmgr.swagger_client.models.status500_internal_server_error_errors import Status500InternalServerErrorErrors
 from fabric_cm.credmgr.swagger_client.models.token import Token
+from fabric_cm.credmgr.swagger_client.models.token_post import TokenPost
 from fabric_cm.credmgr.swagger_client.models.tokens import Tokens
 from fabric_cm.credmgr.swagger_client.models.version import Version
 from fabric_cm.credmgr.swagger_client.models.version_data import VersionData
```

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,16 +224,26 @@
         ).get('authorization')
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
-        return {
-        }
+        result = {}
+        if self.get_api_key_with_prefix('Authorization') is not None:
+            result = {
+                'bearerAuth':
+                    {
+                        'type': 'api_key',
+                        'in': 'header',
+                        'key': 'Authorization',
+                        'value': self.get_api_key_with_prefix('Authorization')
+                    },
+            }
+        return result
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
```

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,27 @@
 
 from __future__ import absolute_import
 
 # import models into model package
 from fabric_cm.credmgr.swagger_client.models.jwks import Jwks
 from fabric_cm.credmgr.swagger_client.models.jwks_keys import JwksKeys
 from fabric_cm.credmgr.swagger_client.models.request import Request
+from fabric_cm.credmgr.swagger_client.models.revoke_list import RevokeList
 from fabric_cm.credmgr.swagger_client.models.status200_ok_no_content import Status200OkNoContent
 from fabric_cm.credmgr.swagger_client.models.status200_ok_no_content_data import Status200OkNoContentData
+from fabric_cm.credmgr.swagger_client.models.status200_ok_paginated import Status200OkPaginated
 from fabric_cm.credmgr.swagger_client.models.status200_ok_single import Status200OkSingle
 from fabric_cm.credmgr.swagger_client.models.status400_bad_request import Status400BadRequest
 from fabric_cm.credmgr.swagger_client.models.status400_bad_request_errors import Status400BadRequestErrors
 from fabric_cm.credmgr.swagger_client.models.status401_unauthorized import Status401Unauthorized
 from fabric_cm.credmgr.swagger_client.models.status401_unauthorized_errors import Status401UnauthorizedErrors
 from fabric_cm.credmgr.swagger_client.models.status403_forbidden import Status403Forbidden
 from fabric_cm.credmgr.swagger_client.models.status403_forbidden_errors import Status403ForbiddenErrors
 from fabric_cm.credmgr.swagger_client.models.status404_not_found import Status404NotFound
 from fabric_cm.credmgr.swagger_client.models.status404_not_found_errors import Status404NotFoundErrors
 from fabric_cm.credmgr.swagger_client.models.status500_internal_server_error import Status500InternalServerError
 from fabric_cm.credmgr.swagger_client.models.status500_internal_server_error_errors import Status500InternalServerErrorErrors
 from fabric_cm.credmgr.swagger_client.models.token import Token
+from fabric_cm.credmgr.swagger_client.models.token_post import TokenPost
 from fabric_cm.credmgr.swagger_client.models.tokens import Tokens
 from fabric_cm.credmgr.swagger_client.models.version import Version
 from fabric_cm.credmgr.swagger_client.models.version_data import VersionData
```

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,48 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from fabric_cm.credmgr.swagger_client.models.status200_ok_single import Status200OkSingle  # noqa: F401,E501
+from fabric_cm.credmgr.swagger_client.models.status200_ok_paginated import Status200OkPaginated  # noqa: F401,E501
 
-class Tokens(Status200OkSingle):
+class Tokens(Status200OkPaginated):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'data': 'list[Token]'
     }
-    if hasattr(Status200OkSingle, "swagger_types"):
-        swagger_types.update(Status200OkSingle.swagger_types)
+    if hasattr(Status200OkPaginated, "swagger_types"):
+        swagger_types.update(Status200OkPaginated.swagger_types)
 
     attribute_map = {
         'data': 'data'
     }
-    if hasattr(Status200OkSingle, "attribute_map"):
-        attribute_map.update(Status200OkSingle.attribute_map)
+    if hasattr(Status200OkPaginated, "attribute_map"):
+        attribute_map.update(Status200OkPaginated.attribute_map)
 
     def __init__(self, data=None, *args, **kwargs):  # noqa: E501
         """Tokens - a model defined in Swagger"""  # noqa: E501
-        Status200OkSingle.__init__(self, *args, **kwargs)
+        Status200OkPaginated.__init__(self, *args, **kwargs)
         self._data = None
         self.discriminator = None
         if data is not None:
             self.data = data
+        
 
     @property
     def data(self):
         """Gets the data of this Tokens.  # noqa: E501
 
 
         :return: The data of this Tokens.  # noqa: E501
```

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/git_push.sh` & `fabric-credmgr-client-1.6.0b1/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/pyproject.toml` & `fabric-credmgr-client-1.6.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_default_api.py` & `fabric-credmgr-client-1.6.0b1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_jwks.py` & `fabric-credmgr-client-1.6.0b1/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py` & `fabric-credmgr-client-1.6.0b1/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_request.py` & `fabric-credmgr-client-1.6.0b1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py` & `fabric-credmgr-client-1.6.0b1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_token.py` & `fabric-credmgr-client-1.6.0b1/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_tokens.py` & `fabric-credmgr-client-1.6.0b1/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py` & `fabric-credmgr-client-1.6.0b1/test/test_tokens_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,24 +30,52 @@
     def test_tokens_create_post(self):
         """Test case for tokens_create_post
 
         Generate tokens for an user  # noqa: E501
         """
         pass
 
+    def test_tokens_get(self):
+        """Test case for tokens_get
+
+        Get tokens  # noqa: E501
+        """
+        pass
+
     def test_tokens_refresh_post(self):
         """Test case for tokens_refresh_post
 
         Refresh tokens for an user  # noqa: E501
         """
         pass
 
+    def test_tokens_revoke_list_get(self):
+        """Test case for tokens_revoke_list_get
+
+        Get token revoke list i.e. list of revoked identity token hashes  # noqa: E501
+        """
+        pass
+
     def test_tokens_revoke_post(self):
         """Test case for tokens_revoke_post
 
-        Revoke a refresh token for an user  # noqa: E501
+        Revoke a token for an user  # noqa: E501
+        """
+        pass
+
+    def test_tokens_revokes_post(self):
+        """Test case for tokens_revokes_post
+
+        Revoke a token  # noqa: E501
+        """
+        pass
+
+    def test_tokens_validate_post(self):
+        """Test case for tokens_validate_post
+
+        Validate an identity token issued by Credential Manager  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_version.py` & `fabric-credmgr-client-1.6.0b1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_version_api.py` & `fabric-credmgr-client-1.6.0b1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/test/test_version_data.py` & `fabric-credmgr-client-1.6.0b1/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0rc1/PKG-INFO` & `fabric-credmgr-client-1.6.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: Fabric Control Framework
 Keywords: Fabric Credential Manager API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -102,43 +102,50 @@
 except ApiException as e:
     print("Exception when calling CredmgrProxy->revoke: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://127.0.0.1:7000/*
+All URIs are relative to *http://127.0.0.1:7000/credmgr/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**certs_get**](docs/DefaultApi.md#certs_get) | **GET** /certs | Return Public Keys to verify signature of the tokens
 *TokensApi* | [**tokens_create_post**](docs/TokensApi.md#tokens_create_post) | **POST** /tokens/create | Generate tokens for an user
+*TokensApi* | [**tokens_get**](docs/TokensApi.md#tokens_get) | **GET** /tokens | Get tokens
 *TokensApi* | [**tokens_refresh_post**](docs/TokensApi.md#tokens_refresh_post) | **POST** /tokens/refresh | Refresh tokens for an user
-*TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a refresh token for an user
+*TokensApi* | [**tokens_revoke_list_get**](docs/TokensApi.md#tokens_revoke_list_get) | **GET** /tokens/revoke_list | Get token revoke list i.e. list of revoked identity token hashes
+*TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a token for an user
+*TokensApi* | [**tokens_revokes_post**](docs/TokensApi.md#tokens_revokes_post) | **POST** /tokens/revokes | Revoke a token
+*TokensApi* | [**tokens_validate_post**](docs/TokensApi.md#tokens_validate_post) | **POST** /tokens/validate | Validate an identity token issued by Credential Manager
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
  - [Jwks](docs/Jwks.md)
  - [JwksKeys](docs/JwksKeys.md)
  - [Request](docs/Request.md)
+ - [RevokeList](docs/RevokeList.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
+ - [Status200OkPaginated](docs/Status200OkPaginated.md)
  - [Status200OkSingle](docs/Status200OkSingle.md)
  - [Status400BadRequest](docs/Status400BadRequest.md)
  - [Status400BadRequestErrors](docs/Status400BadRequestErrors.md)
  - [Status401Unauthorized](docs/Status401Unauthorized.md)
  - [Status401UnauthorizedErrors](docs/Status401UnauthorizedErrors.md)
  - [Status403Forbidden](docs/Status403Forbidden.md)
  - [Status403ForbiddenErrors](docs/Status403ForbiddenErrors.md)
  - [Status404NotFound](docs/Status404NotFound.md)
  - [Status404NotFoundErrors](docs/Status404NotFoundErrors.md)
  - [Status500InternalServerError](docs/Status500InternalServerError.md)
  - [Status500InternalServerErrorErrors](docs/Status500InternalServerErrorErrors.md)
  - [Token](docs/Token.md)
+ - [TokenPost](docs/TokenPost.md)
  - [Tokens](docs/Tokens.md)
  - [Version](docs/Version.md)
  - [VersionData](docs/VersionData.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
```

