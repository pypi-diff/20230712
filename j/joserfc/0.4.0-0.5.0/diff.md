# Comparing `tmp/joserfc-0.4.0.tar.gz` & `tmp/joserfc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.4.0.tar", last modified: Thu Jul  6 13:29:56 2023, max compression
+gzip compressed data, was "joserfc-0.5.0.tar", last modified: Wed Jul 12 12:15:29 2023, max compression
```

## Comparing `joserfc-0.4.0.tar` & `joserfc-0.5.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.502500 joserfc-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 13:29:43.000000 joserfc-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 13:29:56.502500 joserfc-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-06 13:29:43.000000 joserfc-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-06 13:29:43.000000 joserfc-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:29:56.502500 joserfc-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 13:29:43.000000 joserfc-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.490499 joserfc-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/jwe_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/jwe_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/rfc7515/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/rfc7516/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7517/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/keyset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7518/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/derive_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7519/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7638/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc8037/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc8812/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.502500 joserfc-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-06 13:29:43.000000 joserfc-0.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-12 12:15:20.000000 joserfc-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-12 12:15:29.275596 joserfc-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 12:15:20.000000 joserfc-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-12 12:15:20.000000 joserfc-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:15:29.275596 joserfc-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 12:15:20.000000 joserfc-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.267596 joserfc-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/keyset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7797/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 12:15:20.000000 joserfc-0.5.0/tests/test_util.py
```

### Comparing `joserfc-0.4.0/LICENSE` & `joserfc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/PKG-INFO` & `joserfc-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.4.0
+Version: 0.5.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `joserfc-0.4.0/README.rst` & `joserfc-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/pyproject.toml` & `joserfc-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/drafts/jwe_chacha20.py` & `joserfc-0.5.0/src/joserfc/drafts/jwe_chacha20.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/drafts/jwe_ecdh_1pu.py` & `joserfc-0.5.0/src/joserfc/drafts/jwe_ecdh_1pu.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,36 +68,29 @@
         return self.__decrypt_agreed_upon_key(enc, recipient, None)
 
     def decrypt_agreed_upon_key_with_tag(self, enc: JWEEncModel, recipient: Recipient, tag: bytes) -> bytes:
         return self.__decrypt_agreed_upon_key(enc, recipient, tag)
 
     def __encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
         sender_key: CurveKey = recipient.sender_key
-        recipient_pubkey = recipient.recipient_key.get_op_key("deriveKey")
-        sender_shared_key = sender_key.exchange_shared_key(recipient_pubkey)
-        ephemeral_shared_key = recipient.ephemeral_key.exchange_shared_key(recipient_pubkey)
+        sender_shared_key = sender_key.exchange_derive_key(recipient.recipient_key)
+        ephemeral_shared_key = recipient.ephemeral_key.exchange_derive_key(recipient.recipient_key)
         shared_key = ephemeral_shared_key + sender_shared_key
         headers = recipient.headers()
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
     def __decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
         self._check_enc(enc)
-
         headers = recipient.headers()
         assert "epk" in headers
 
         recipient_key: CurveKey = recipient.recipient_key
-        sender_key: CurveKey = recipient.sender_key
-
         ephemeral_key = recipient_key.import_key(headers["epk"])
-        ephemeral_pubkey = ephemeral_key.get_op_key("deriveKey")
-        sender_pubkey = sender_key.get_op_key("deriveKey")
-
-        sender_shared_key = recipient_key.exchange_shared_key(sender_pubkey)
-        ephemeral_shared_key = recipient_key.exchange_shared_key(ephemeral_pubkey)
+        sender_shared_key = recipient_key.exchange_derive_key(recipient.sender_key)
+        ephemeral_shared_key = recipient_key.exchange_derive_key(ephemeral_key)
         shared_key = ephemeral_shared_key + sender_shared_key
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
 
 JWE_ALG_MODELS = [
     ECDH1PUAlgModel(None),    # ECDH-1PU
     ECDH1PUAlgModel(A128KW),  # ECDH-1PU+A128KW
```

### Comparing `joserfc-0.4.0/src/joserfc/errors.py` & `joserfc-0.5.0/src/joserfc/errors.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/jwe.py` & `joserfc-0.5.0/src/joserfc/jwe.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/jwk.py` & `joserfc-0.5.0/src/joserfc/jwk.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,10 +86,8 @@
 
     elif callable(key):
         rv_key = key(obj)
 
     else:
         raise ValueError("Invalid key")
 
-    if "alg" in headers:
-        rv_key.check_alg(headers["alg"])
     return rv_key
```

### Comparing `joserfc-0.4.0/src/joserfc/jws.py` & `joserfc-0.5.0/src/joserfc/jws.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,24 @@
     JWSAlgModel,
     HeaderMember,
     CompactSignature,
     JSONSignature,
 )
 from .rfc7515.registry import (
     JWSRegistry,
-    default_registry,
+    construct_registry,
 )
 from .rfc7515.compact import (
     sign_compact,
     extract_compact,
     verify_compact,
     detach_compact_content,
 )
 from .rfc7515.json import (
+    construct_json_signature,
     sign_json,
     verify_json,
     extract_json,
     detach_json_content,
 )
 from .rfc7515.types import (
     HeaderDict,
@@ -34,26 +35,26 @@
 from .util import to_bytes, urlsafe_b64encode
 from .registry import Header
 
 __all__ = [
     "types",
     "JWSAlgModel",
     "JWSRegistry",
+    "HeaderMember",
     "CompactSignature",
     "JSONSignature",
     "serialize_compact",
     "deserialize_compact",
     "extract_compact",
     "validate_compact",
     "serialize_json",
     "deserialize_json",
     "extract_json",
     "validate_json",
     "detach_content",
-    "default_registry",
 ]
 
 
 # register supported alg models
 def __register():
     # register alg in RFC7518
     for _alg in JWS_ALGORITHMS:
@@ -86,23 +87,23 @@
     :param protected: protected header part of the JWS, in dict
     :param payload: payload data of the JWS, in bytes
     :param private_key: a flexible private key to sign the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :return: JWS in str
     """
-    if algorithms:
-        registry = JWSRegistry(algorithms=algorithms)
-    elif registry is None:
-        registry = default_registry
+    if registry is None:
+        registry = construct_registry(algorithms)
 
     registry.check_header(protected)
     obj = CompactSignature(protected, to_bytes(payload))
     alg: JWSAlgModel = registry.get_alg(protected["alg"])
     key: Key = guess_key(private_key, obj)
+    key.check_use("sig")
+    key.check_alg(protected["alg"])
     out = sign_compact(obj, alg, key)
     return out.decode("utf-8")
 
 
 def validate_compact(
         obj: CompactSignature,
         public_key: KeyFlexible,
@@ -113,22 +114,22 @@
 
     :param obj: object of the JWS Compact Serialization
     :param public_key: a flexible public key to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :raise: ValueError or BadSignatureError
     """
-    if algorithms:
-        registry = JWSRegistry(algorithms=algorithms)
-    elif registry is None:
-        registry = default_registry
+    if registry is None:
+        registry = construct_registry(algorithms)
 
     headers = obj.headers()
-    alg: JWSAlgModel = registry.get_alg(headers["alg"])
+    registry.check_header(headers)
     key: Key = guess_key(public_key, obj)
+    key.check_use("sig")
+    alg: JWSAlgModel = registry.get_alg(headers["alg"])
     if not verify_compact(obj, alg, key):
         raise BadSignatureError()
 
 
 def deserialize_compact(
         value: t.AnyStr,
         public_key: KeyFlexible,
@@ -186,36 +187,21 @@
         {
             "payload":"<payload contents>",
             "protected":"<integrity-protected header contents>",
             "header":<non-integrity-protected header contents>,
             "signature":"<signature contents>"
         }
     """
-    if algorithms:
-        registry = JWSRegistry(algorithms=algorithms)
-    elif registry is None:
-        registry = default_registry
-
-    if isinstance(members, dict):
-        flatten = True
-        __check_member(registry, members)
-        members = [members]
-    else:
-        flatten = False
-        for member in members:
-            __check_member(registry, member)
-
-    members = [HeaderMember(**member) for member in members]
-    payload = to_bytes(payload)
-    obj = JSONSignature(members, payload)
-    obj.segments["payload"] = urlsafe_b64encode(payload)
-    obj.flattened = flatten
+    if registry is None:
+        registry = construct_registry(algorithms)
 
+    obj = construct_json_signature(members, payload, registry)
+    obj.segments["payload"] = urlsafe_b64encode(obj.payload)
     find_key = lambda d: guess_key(private_key, d)
-    return sign_json(obj, registry.get_alg, find_key)
+    return sign_json(obj, registry, find_key)
 
 
 def validate_json(
         obj: JSONSignature,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWSRegistry] = None):
@@ -224,20 +210,18 @@
 
     :param obj: object of the JWS JSON Serialization
     :param public_key: a flexible public key to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :raise: ValueError or BadSignatureError
     """
-    if algorithms:
-        registry = JWSRegistry(algorithms=algorithms)
-    elif registry is None:
-        registry = default_registry
+    if registry is None:
+        registry = construct_registry(algorithms)
     find_key = lambda d: guess_key(public_key, d)
-    if not verify_json(obj, registry.get_alg, find_key):
+    if not verify_json(obj, registry, find_key):
         raise BadSignatureError()
 
 
 def deserialize_json(
         value: JSONSerialization,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
@@ -276,16 +260,7 @@
         >>> obj = jws.serialize_json({"protected": {"alg": "HS256"}}, b"hello", "secret")
         >>> jws.detach_content(obj)
         {'payload': '', 'signature': 'UYmO_lPAY5V0Wf4KZsfhiYs1SxqXPhxvjuYqellDV5A', 'protected': 'eyJhbGciOiJIUzI1NiJ9'}
     """
     if isinstance(value, str):
         return detach_compact_content(value)
     return detach_json_content(value)
-
-
-def __check_member(registry: JWSRegistry, member: HeaderDict):
-    header = {}
-    if "protected" in member:
-        header.update(member["protected"])
-    if "header" in member:
-        header.update(member["header"])
-    registry.check_header(header)
```

### Comparing `joserfc-0.4.0/src/joserfc/jwt.py` & `joserfc-0.5.0/src/joserfc/jwt.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/registry.py` & `joserfc-0.5.0/src/joserfc/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,35 +174,28 @@
 def check_supported_header(registry: HeaderRegistryDict, header: Header):
     allowed_keys = set(registry.keys())
     unsupported_keys = set(header.keys()) - allowed_keys
     if unsupported_keys:
         raise ValueError(f'Unsupported {unsupported_keys} in header')
 
 
-def check_registry_header(registry: HeaderRegistryDict, header: Header):
+def validate_registry_header(
+        registry: HeaderRegistryDict,
+        header: Header,
+        check_required: bool = True):
     for key in registry:
         reg: HeaderParameter = registry[key]
-        if reg.required and key not in header:
+        if check_required and reg.required and key not in header:
             raise ValueError(f'Required "{key}" is missing in header')
         if key in header:
             try:
                 reg.validate(header[key])
             except ValueError as error:
                 raise ValueError(f'"{key}" in header {error}')
 
 
-def check_registry_header_types(registry: HeaderRegistryDict, header: Header):
-    for key in registry:
-        if key in header:
-            try:
-                reg: HeaderParameter = registry[key]
-                reg.validate(header[key])
-            except ValueError as error:
-                raise ValueError(f'"{key}" in header {error}')
-
-
 def check_crit_header(header: Header):
     # check crit header
     if "crit" in header:
         for k in header["crit"]:
             if k not in header:
                 raise ValueError(f'"{k}" is a critical header')
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.5.0/src/joserfc/rfc7515/compact.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 
 
 def sign_compact(obj: CompactSignature, alg: JWSAlgModel, key) -> bytes:
-    key.check_use("sig")
     header_segment = json_b64encode(obj.headers())
     payload_segment = urlsafe_b64encode(obj.payload)
     signing_input = header_segment + b"." + payload_segment
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
     return signing_input + b"." + signature
 
 
@@ -25,20 +24,15 @@
     :raise: DecodeError
     """
     parts = value.split(b".")
     if len(parts) != 3:
         raise ValueError("Invalid JSON Web Signature")
 
     header_segment, payload_segment, signature_segment = parts
-    try:
-        protected = json_b64decode(header_segment)
-        if "alg" not in protected:
-            raise MissingAlgorithmError()
-    except (TypeError, ValueError, binascii.Error):
-        raise DecodeError("Invalid header")
+    protected = decode_header(header_segment)
 
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
         raise DecodeError("Invalid payload")
 
     obj = CompactSignature(protected, payload)
@@ -47,18 +41,27 @@
         "payload": payload_segment,
         "signature": signature_segment,
     })
     return obj
 
 
 def verify_compact(obj: CompactSignature, alg: JWSAlgModel, key) -> bool:
-    key.check_use("sig")
     signing_input = obj.segments["header"] + b"." + obj.segments["payload"]
     sig = urlsafe_b64decode(obj.segments["signature"])
     return alg.verify(signing_input, sig, key)
 
 
 def detach_compact_content(value: str) -> str:
     # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
     parts = value.split(".")
     parts[1] = ""
     return ".".join(parts)
+
+
+def decode_header(header_segment: bytes):
+    try:
+        protected = json_b64decode(header_segment)
+        if "alg" not in protected:
+            raise MissingAlgorithmError()
+    except (TypeError, ValueError, binascii.Error):
+        raise DecodeError("Invalid header")
+    return protected
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7515/json.py` & `joserfc-0.5.0/src/joserfc/rfc7515/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,81 @@
 import typing as t
 import binascii
 from .model import JWSAlgModel, HeaderMember, JSONSignature
 from .types import (
+    HeaderDict,
     JSONSignatureDict,
     JSONSerialization,
     GeneralJSONSerialization,
     FlattenedJSONSerialization,
 )
+from .registry import JWSRegistry
 from ..util import (
+    to_bytes,
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 from ..errors import DecodeError
 
-FindAlgorithm = t.Callable[[str], JWSAlgModel]
+
+def construct_json_signature(
+        members: t.Union[HeaderDict, t.List[HeaderDict]],
+        payload: t.AnyStr,
+        registry: JWSRegistry) -> JSONSignature:
+    if isinstance(members, dict):
+        flattened = True
+        __check_member(registry, members)
+        members = [members]
+    else:
+        flattened = False
+        for member in members:
+            __check_member(registry, member)
+
+    members = [HeaderMember(**member) for member in members]
+    payload = to_bytes(payload)
+    obj = JSONSignature(members, payload)
+    obj.flattened = flattened
+    return obj
+
+
+def __check_member(registry: JWSRegistry, member: HeaderDict):
+    header = {}
+    if "protected" in member:
+        header.update(member["protected"])
+    if "header" in member:
+        header.update(member["header"])
+    registry.check_header(header)
 
 
-def sign_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> JSONSerialization:
+def sign_json(obj: JSONSignature, registry: JWSRegistry, find_key) -> JSONSerialization:
     signatures: t.List[JSONSignatureDict] = []
 
     payload_segment = obj.segments["payload"]
     for member in obj.members:
         headers = member.headers()
-        alg = find_alg(headers["alg"])
+        registry.check_header(headers)
+        alg = registry.get_alg(headers["alg"])
         key = find_key(member)
         key.check_use("sig")
-        signature = _sign_member(payload_segment, member, alg, key)
+        signature = __sign_member(payload_segment, member, alg, key)
         signatures.append(signature)
 
     rv = {"payload": payload_segment.decode("utf-8")}
     if obj.flattened and len(signatures) == 1:
         rv.update(dict(signatures[0]))
     else:
         rv["signatures"] = signatures
 
     obj.signatures = signatures
     return rv
 
 
-def _sign_member(payload_segment, member: HeaderMember, alg: JWSAlgModel, key) -> JSONSignatureDict:
+def __sign_member(payload_segment, member: HeaderMember, alg: JWSAlgModel, key) -> JSONSignatureDict:
     if member.protected:
         protected_segment = json_b64encode(member.protected)
     else:
         protected_segment = b""
     signing_input = b".".join([protected_segment, payload_segment])
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
     rv: JSONSignatureDict = {"signature": signature.decode("utf-8")}
@@ -64,19 +95,19 @@
 
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
         raise DecodeError("Invalid payload")
 
     if "signatures" in value:
-        flatten = False
+        flattened = False
         value: GeneralJSONSerialization
         signatures: t.List[JSONSignatureDict] = value["signatures"]
     else:
-        flatten = True
+        flattened = True
         value: FlattenedJSONSerialization
         _sig: JSONSignatureDict = {
             "protected": value["protected"],
             "signature": value["signature"],
         }
         if "header" in value:
             _sig["header"] = value["header"]
@@ -90,32 +121,33 @@
             member.protected = json_b64decode(protected_segment)
         if "header" in sig:
             member.header = sig["header"]
         members.append(member)
 
     obj = JSONSignature(members, payload)
     obj.segments.update({"payload": payload_segment})
-    obj.flattened = flatten
+    obj.flattened = flattened
     obj.signatures = signatures
     return obj
 
 
-def verify_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> bool:
+def verify_json(obj: JSONSignature, registry: JWSRegistry, find_key) -> bool:
     """Verify the signature of this JSON serialization with the given
     algorithm and key.
 
     :param obj: instance of the SignatureData
     :param find_alg: a function to return "alg" model
     :param find_key: a function to return public key
     """
     payload_segment = obj.segments["payload"]
     for index, signature in enumerate(obj.signatures):
         member = obj.members[index]
         headers = member.headers()
-        alg = find_alg(headers["alg"])
+        registry.check_header(headers)
+        alg = registry.get_alg(headers["alg"])
         key = find_key(member)
         key.check_use("sig")
         if not _verify_signature(signature, payload_segment, alg, key):
             return False
     return True
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7515/model.py` & `joserfc-0.5.0/src/joserfc/rfc7515/model.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7515/registry.py` & `joserfc-0.5.0/src/joserfc/rfc7515/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from typing import Dict, List, Optional
 from .model import JWSAlgModel
 from ..registry import (
     JWS_HEADER_REGISTRY,
     Header,
     HeaderRegistryDict,
-    check_registry_header,
+    validate_registry_header,
     check_crit_header,
     check_supported_header,
 )
 
 
 class JWSRegistry(object):
     """A registry for JSON Web Signature to keep all the supported algorithms.
     An instance of ``JWSRegistry`` is usually used together with methods in
     ``joserfc.jws``.
 
     :param header_registry: extra header parameters registry
     :param algorithms: allowed algorithms to be used
     :param strict_check_header: only allow header key in the registry to be used
     """
+    default_header_registry: HeaderRegistryDict = JWS_HEADER_REGISTRY
     algorithms: Dict[str, JWSAlgModel] = {}
     recommended: List[str] = []
 
     def __init__(
             self,
             header_registry: Optional[HeaderRegistryDict] = None,
             algorithms: Optional[List[str]] = None,
             strict_check_header: bool = True):
         self.header_registry: HeaderRegistryDict = {}
-        self.header_registry.update(JWS_HEADER_REGISTRY)
+        self.header_registry.update(self.default_header_registry)
         if header_registry is not None:
             self.header_registry.update(header_registry)
         self.allowed = algorithms
         self.strict_check_header = strict_check_header
 
     @classmethod
     def register(cls, alg: JWSAlgModel):
@@ -56,14 +57,22 @@
         if name not in allowed:
             raise ValueError(f'Algorithm of "{name}" is not allowed')
         return self.algorithms[name]
 
     def check_header(self, header: Header):
         """Check and validate the fields in header part of a JWS object."""
         check_crit_header(header)
-        check_registry_header(self.header_registry, header)
+        validate_registry_header(self.header_registry, header)
         if self.strict_check_header:
             check_supported_header(self.header_registry, header)
 
 
 #: default JWS registry
 default_registry = JWSRegistry()
+
+
+def construct_registry(algorithms: Optional[List[str]] = None):
+    if algorithms:
+        registry = JWSRegistry(algorithms=algorithms)
+    else:
+        registry = default_registry
+    return registry
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7515/types.py` & `joserfc-0.5.0/src/joserfc/rfc7515/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/compact.py` & `joserfc-0.5.0/src/joserfc/rfc7516/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/json.py` & `joserfc-0.5.0/src/joserfc/rfc7516/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if recipient.header:
             item["header"] = recipient.header
         if recipient.encrypted_key:
             item["encrypted_key"] = to_unicode(urlsafe_b64encode(recipient.encrypted_key))
         if data:
             recipients.append(item)
 
-    if obj.flatten and len(recipients) == 1:
+    if obj.flattened and len(recipients) == 1:
         data.update(recipients[0])
     else:
         data["recipients"] = recipients
     return data
 
 
 def extract_json(data: JSONSerialization) -> JSONEncryption:
@@ -53,18 +53,20 @@
     obj.bytes_segments["ciphertext"] = urlsafe_b64decode(obj.base64_segments["ciphertext"])
     obj.bytes_segments["tag"] = urlsafe_b64decode(obj.base64_segments["tag"])
 
     if "aad" in data:
         obj.aad = urlsafe_b64decode(to_bytes(data["aad"]))
 
     if "recipients" in data:
-        obj.flatten = False
+        obj.flattened = False
         for item in data["recipients"]:
             recipient = Recipient(obj, item.get("header"))
-            recipient.encrypted_key = urlsafe_b64decode(to_bytes(item["encrypted_key"]))
+            if "encrypted_key" in item:
+                recipient.encrypted_key = urlsafe_b64decode(to_bytes(item["encrypted_key"]))
             obj.recipients.append(recipient)
     else:
-        obj.flatten = True
+        obj.flattened = True
         recipient = Recipient(obj, data.get("header"))
-        recipient.encrypted_key = urlsafe_b64decode(to_bytes(data["encrypted_key"]))
+        if "encrypted_key" in data:
+            recipient.encrypted_key = urlsafe_b64decode(to_bytes(data["encrypted_key"]))
         obj.recipients.append(recipient)
     return obj
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/message.py` & `joserfc-0.5.0/src/joserfc/rfc7516/message.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/models.py` & `joserfc-0.5.0/src/joserfc/rfc7516/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,25 +91,25 @@
     """
     def __init__(
             self,
             protected: Header,
             plaintext: t.Optional[bytes] = None,
             unprotected: t.Optional[Header] = None,
             aad: t.Optional[bytes] = None,
-            flatten: bool = False):
+            flattened: bool = False):
         #: protected header in dict
         self.protected: Header = protected
         #: the plaintext in bytes
         self.plaintext: bytes = plaintext
         #: unprotected header in dict
         self.unprotected: t.Optional[Header] = unprotected
         #: an optional additional authenticated data
         self.aad: t.Optional[bytes] = aad
         #: represents if the object is in flatten syntax
-        self.flatten: bool = flatten
+        self.flattened: bool = flattened
         #: a list of recipients
         self.recipients: t.List[Recipient] = []
 
         self.bytes_segments: t.Dict[str, bytes] = {}  # store the decoded segments
         self.base64_segments: t.Dict[str, bytes] = {}  # store the encoded segments
 
     def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[Key] = None):
@@ -141,15 +141,15 @@
 
     def check_iv(self, iv: bytes) -> bytes:
         if len(iv) * 8 != self.iv_size:
             raise ValueError('Invalid "iv" size')
         return iv
 
     @abstractmethod
-    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> t.Tuple[bytes, bytes]:
         pass
 
     @abstractmethod
     def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
         pass
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.5.0/src/joserfc/rfc7516/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import typing as t
 from .models import JWEAlgModel, JWEEncModel, JWEZipModel
 from ..registry import (
     Header,
     HeaderRegistryDict,
     JWE_HEADER_REGISTRY,
     check_supported_header,
-    check_registry_header,
-    check_registry_header_types,
+    validate_registry_header,
     check_crit_header,
 )
 
 JWEAlgorithm = t.Union[JWEAlgModel, JWEEncModel, JWEZipModel]
 
 AlgorithmsDict = t.TypedDict("AlgorithmsDict", {
     "alg": t.Dict[str, JWEAlgModel],
@@ -58,22 +57,19 @@
         cls.algorithms[location][model.name] = model
         if model.recommended:
             cls.recommended.append(model.name)
 
     def check_header(self, header: Header, check_more=False):
         """Check and validate the fields in header part of a JWS object."""
         check_crit_header(header)
-        check_registry_header(self.header_registry, header)
+        validate_registry_header(self.header_registry, header)
 
         alg = self.get_alg(header["alg"])
         if alg.more_header_registry:
-            if check_more:
-                check_registry_header(alg.more_header_registry, header)
-            else:
-                check_registry_header_types(alg.more_header_registry, header)
+            validate_registry_header(alg.more_header_registry, header, check_more)
 
             if self.strict_check_header:
                 allowed_registry = self.header_registry.copy()
                 allowed_registry.update(alg.more_header_registry)
                 check_supported_header(allowed_registry, header)
         elif self.strict_check_header:
             check_supported_header(self.header_registry, header)
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7516/types.py` & `joserfc-0.5.0/src/joserfc/rfc7516/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing as t
 
 __all__ = [
     "JSONSerialization",
     "FlattenJSONSerialization",
-    "CompleteJSONSerialization",
+    "GeneralJSONSerialization",
 ]
 
 JSONRecipientDict = t.TypedDict("JSONRecipientDict", {
     "header": t.Dict[str, any],
     "encrypted_key": str,
 }, total=False)
 
-CompleteJSONSerialization = t.TypedDict("CompleteJSONSerialization", {
+GeneralJSONSerialization = t.TypedDict("GeneralJSONSerialization", {
     "protected": str,
     "unprotected": t.Dict[str, any],
     "iv": str,
     "aad": str,
     "ciphertext": str,
     "tag": str,
     "recipients": t.List[JSONRecipientDict],
@@ -28,8 +28,8 @@
     "encrypted_key": str,
     "iv": str,
     "aad": str,
     "ciphertext": str,
     "tag": str,
 }, total=False)
 
-JSONSerialization = t.Union[CompleteJSONSerialization, FlattenJSONSerialization]
+JSONSerialization = t.Union[GeneralJSONSerialization, FlattenJSONSerialization]
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7517/keyset.py` & `joserfc-0.5.0/src/joserfc/rfc7517/keyset.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7517/models.py` & `joserfc-0.5.0/src/joserfc/rfc7517/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     @classmethod
     @abstractmethod
     def import_from_dict(cls, value: KeyDict):
         pass
 
     @classmethod
     @abstractmethod
-    def import_from_bytes(cls, value: bytes):
+    def import_from_bytes(cls, value: bytes, password=None):
         pass
 
     @staticmethod
     def as_bytes(key: "BaseKey", encoding=None, private=None, password=None) -> bytes:  # pragma: no cover
         return key.raw_value
 
     @classmethod
@@ -103,19 +103,19 @@
         if not kid:
             kid = self.thumbprint()
             self._dict_value["kid"] = kid
         return kid
 
     @property
     def raw_value(self):
-        return self._raw_value
+        raise NotImplementedError()
 
     @property
     def is_private(self) -> bool:
-        return False
+        raise NotImplementedError()
 
     @property
     def dict_value(self) -> KeyDict:
         """Property of the Key in Dict (JSON)."""
         if self._dict_value:
             return self._dict_value
 
@@ -212,21 +212,21 @@
     @classmethod
     def validate_dict_key(cls, data: KeyDict):
         cls.binding.validate_dict_key_registry(data, cls.param_registry)
         cls.binding.validate_dict_key_registry(data, cls.value_registry)
         cls.binding.validate_dict_key_use_operations(data)
 
     @classmethod
-    def import_key(cls, value: KeyAny, parameters: KeyParameters = None) -> "BaseKey":
+    def import_key(cls, value: KeyAny, parameters: KeyParameters = None, password=None) -> "BaseKey":
         if isinstance(value, dict):
             cls.validate_dict_key(value)
             raw_key = cls.binding.import_from_dict(value)
             return cls(raw_key, value, parameters)
 
-        raw_key = cls.binding.import_from_bytes(to_bytes(value))
+        raw_key = cls.binding.import_from_bytes(to_bytes(value), password)
         return cls(raw_key, value, parameters)
 
     @classmethod
     def generate_key(cls, size_or_crv, parameters: KeyParameters = None, private: bool = True) -> "BaseKey":
         raise NotImplementedError()
 
 
@@ -274,12 +274,12 @@
 class CurveKey(AsymmetricKey[NativePublicKey, NativePrivateKey]):
     @property
     @abstractmethod
     def curve_name(self) -> str:
         pass
 
     @abstractmethod
-    def exchange_shared_key(self, pubkey) -> bytes:
+    def exchange_derive_key(self, key: "CurveKey") -> bytes:
         pass
 
 
 Key = t.Union[SymmetricKey, AsymmetricKey, CurveKey]
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.5.0/src/joserfc/rfc7517/pem.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,16 +85,18 @@
     @classmethod
     def import_from_dict(cls, value: KeyDict):
         if "d" in value:
             return cls.import_private_key(value)
         return cls.import_public_key(value)
 
     @classmethod
-    def import_from_bytes(cls, value: bytes):
-        return load_pem_key(value, cls.ssh_type)
+    def import_from_bytes(cls, value: bytes, password=None):
+        if password is not None:
+            password = to_bytes(password)
+        return load_pem_key(value, cls.ssh_type, password)
 
     @staticmethod
     def as_bytes(key, encoding=None, private=None, password=None) -> bytes:
         if private is True:
             return dump_pem_key(key.private_key, encoding, private, password)
         elif private is False:
             return dump_pem_key(key.public_key, encoding, private, password)
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7517/registry.py` & `joserfc-0.5.0/src/joserfc/rfc7517/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7517/types.py` & `joserfc-0.5.0/src/joserfc/rfc7517/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/derive_key.py` & `joserfc-0.5.0/src/joserfc/rfc7518/derive_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.5.0/src/joserfc/rfc7518/ec_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         "crv": KeyParameter("Curve", "str", private=False, required=True),
         "x": KeyParameter("X Coordinate", "str", private=False, required=True),
         "y": KeyParameter("Y Coordinate", "str", private=False, required=True),
         "d": KeyParameter("EC Private Key", "str", private=True, required=False),
     }
     binding = ECBinding
 
-    def exchange_shared_key(self, pubkey: EllipticCurvePublicKey) -> bytes:
-        # used in ECDHESAlgorithm
-        if self.private_key:
+    def exchange_derive_key(self, key: "ECKey") -> bytes:
+        pubkey = key.get_op_key("deriveKey")
+        if self.private_key and self.curve_name == key.curve_name:
             return self.private_key.exchange(ECDH(), pubkey)
         raise ValueError("Invalid key for exchanging shared key")
 
     @property
     def is_private(self) -> bool:
         return isinstance(self.raw_value, EllipticCurvePrivateKey)
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.5.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,27 +191,25 @@
             self.key_size = key_wrapping.key_size
             self.recommended = key_wrapping.recommended
         self.key_wrapping = key_wrapping
 
     def encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient):
         recipient_key: CurveKey = recipient.recipient_key
         ephemeral_key: CurveKey = recipient.ephemeral_key
-        pubkey = recipient_key.get_op_key("deriveKey")
-        shared_key = ephemeral_key.exchange_shared_key(pubkey)
+        shared_key = ephemeral_key.exchange_derive_key(recipient_key)
         headers = recipient.headers()
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
     def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
         headers = recipient.headers()
         assert "epk" in headers
 
         recipient_key: CurveKey = self.check_recipient_key(recipient.recipient_key)
-        epk = recipient_key.import_key(headers["epk"])
-        pubkey = epk.get_op_key("deriveKey")
-        shared_key = recipient_key.exchange_shared_key(pubkey)
+        ephemeral_key = recipient_key.import_key(headers["epk"])
+        shared_key = recipient_key.exchange_derive_key(ephemeral_key)
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
 
 class PBES2HSAlgModel(JWEKeyEncryption):
     # https://www.rfc-editor.org/rfc/rfc7518#section-4.8
     more_header_registry = {
         "p2s": HeaderParameter("PBES2 Salt Input", "str", True),
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.5.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     ~~~~~~~~~~~~~~~~~~~~
 
     Cryptographic Models for Cryptographic Models for Content
     Encryption per `Section 5`_.
 
     .. _`Section 5`: https://tools.ietf.org/html/rfc7518#section-5
 """
+import typing as t
 import hmac
 import hashlib
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import GCM, CBC
 from cryptography.hazmat.primitives.padding import PKCS7
@@ -40,15 +41,15 @@
 
     def _hmac(self, ciphertext: bytes, aad: bytes, iv: bytes, key: bytes) -> bytes:
         al = encode_int(len(aad) * 8, 64)
         msg = aad + iv + ciphertext + al
         d = hmac.new(key, msg, self.hash_alg).digest()
         return d[: self.key_len]
 
-    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> t.Tuple[bytes, bytes]:
         """Key Encryption with AES_CBC_HMAC_SHA2."""
         hkey = cek[:self.key_len]
         ekey = cek[self.key_len:]
 
         pad = PKCS7(AES.block_size).padder()
         padded_data = pad.update(plaintext) + pad.finalize()
 
@@ -82,15 +83,15 @@
 
     def __init__(self, key_size: int):
         self.name = f"A{key_size}GCM"
         self.description = f"AES GCM using {key_size}-bit key"
         self.key_size = key_size
         self.cek_size = key_size
 
-    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> t.Tuple[bytes, bytes]:
         """Key Encryption with AES GCM"""
         cipher = Cipher(AES(cek), GCM(iv), backend=default_backend())
         enc = cipher.encryptor()
         enc.authenticate_additional_data(aad)
         ciphertext = enc.update(plaintext) + enc.finalize()
         return ciphertext, enc.tag
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.5.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.5.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.5.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return {"k": k}
 
     @classmethod
     def import_from_dict(cls, value: KeyDict):
         return urlsafe_b64decode(to_bytes(value["k"]))
 
     @classmethod
-    def import_from_bytes(cls, value: bytes):
+    def import_from_bytes(cls, value: bytes, password=None):
         # security check
         if value.startswith(POSSIBLE_UNSAFE_KEYS):
             raise ValueError("This key may not be safe to import")
         return value
 
 
 class OctKey(SymmetricKey[bytes, bytes]):
```

### Comparing `joserfc-0.4.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.5.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.5.0/src/joserfc/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc7519/registry.py` & `joserfc-0.5.0/src/joserfc/rfc7519/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc8037/jws_eddsa.py` & `joserfc-0.5.0/src/joserfc/rfc8037/jws_eddsa.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.5.0/src/joserfc/rfc8037/okp_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,17 +75,18 @@
         "x": KeyParameter("X Coordinate", "str", private=False, required=True),
         "d": KeyParameter("OKP Private Key", "str", private=True, required=False),
     }
     binding = OKPBinding
     required_fields = frozenset(["crv", "x"])
     private_only_fields = frozenset(["d"])
 
-    def exchange_shared_key(self, pubkey: Union[X25519PublicKey, X448PublicKey]) -> bytes:
+    def exchange_derive_key(self, key: "OKPKey") -> bytes:
         # used in ECDHESAlgorithm
-        if self.private_key and isinstance(self.private_key, (X25519PrivateKey, X448PrivateKey)):
+        pubkey = key.get_op_key("deriveKey")
+        if self.private_key and self.curve_name in ("X25519", "X448") and self.curve_name == key.curve_name:
             return self.private_key.exchange(pubkey)
         raise ValueError("Invalid key for exchanging shared key")
 
     @property
     def is_private(self) -> bool:
         return isinstance(self.raw_value, PrivateKeyTypes)
 
@@ -126,8 +127,8 @@
         return "Ed25519"
     elif isinstance(key, (Ed448PublicKey, Ed448PrivateKey)):
         return "Ed448"
     elif isinstance(key, (X25519PublicKey, X25519PrivateKey)):
         return "X25519"
     elif isinstance(key, (X448PublicKey, X448PrivateKey)):
         return "X448"
-    raise ValueError("Invalid key")
+    raise ValueError("Invalid key")  # pragma: no cover
```

### Comparing `joserfc-0.4.0/src/joserfc/util.py` & `joserfc-0.5.0/src/joserfc/util.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.4.0/src/joserfc.egg-info/PKG-INFO` & `joserfc-0.5.0/src/joserfc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.4.0
+Version: 0.5.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `joserfc-0.4.0/src/joserfc.egg-info/SOURCES.txt` & `joserfc-0.5.0/src/joserfc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,16 @@
 src/joserfc/rfc7518/oct_key.py
 src/joserfc/rfc7518/rsa_key.py
 src/joserfc/rfc7518/util.py
 src/joserfc/rfc7519/__init__.py
 src/joserfc/rfc7519/claims.py
 src/joserfc/rfc7519/registry.py
 src/joserfc/rfc7638/__init__.py
+src/joserfc/rfc7797/__init__.py
+src/joserfc/rfc7797/compact.py
+src/joserfc/rfc7797/json.py
+src/joserfc/rfc7797/registry.py
 src/joserfc/rfc8037/__init__.py
 src/joserfc/rfc8037/jws_eddsa.py
 src/joserfc/rfc8037/okp_key.py
 src/joserfc/rfc8812/__init__.py
 tests/test_util.py
```

### Comparing `joserfc-0.4.0/tests/test_util.py` & `joserfc-0.5.0/tests/test_util.py`

 * *Files identical despite different names*

