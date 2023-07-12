# Comparing `tmp/bl_hector-0.3.1.tar.gz` & `tmp/bl_hector-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.3.1.tar", max compression
+gzip compressed data, was "bl_hector-0.3.2.tar", max compression
```

## Comparing `bl_hector-0.3.1.tar` & `bl_hector-0.3.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.3.1/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.3.1/README.md
--rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     2044 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1971 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3729 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0     1505 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1630 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3039 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3547 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1694 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4531 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-23 15:58:56.080839 bl_hector-0.3.1/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2364 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4546 2023-06-21 11:30:42.251958 bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     4012 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3363 2023-06-21 11:30:42.251958 bl_hector-0.3.1/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1690 2023-06-21 11:30:42.255958 bl_hector-0.3.1/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     5448 2023-06-27 05:48:10.328996 bl_hector-0.3.1/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     6060 2023-06-27 05:48:10.332996 bl_hector-0.3.1/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1842 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    19488 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-21 11:30:42.255958 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4238 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2105 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     5746 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3633 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2045 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4768 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1845 2023-06-21 11:30:42.259958 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     5276 2023-06-21 11:30:42.259958 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.3.1/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1570 2023-06-27 05:48:27.768996 bl_hector-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4606 2023-06-27 05:49:30.255854 bl_hector-0.3.1/setup.py
--rw-r--r--   0        0        0     3048 2023-06-27 05:49:30.257588 bl_hector-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.3.2/README.md
+-rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.3.2/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.2/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.2/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.239958 bl_hector-0.3.2/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2044 2023-06-21 11:30:42.239958 bl_hector-0.3.2/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1971 2023-06-21 11:30:42.239958 bl_hector-0.3.2/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3729 2023-06-21 11:30:42.239958 bl_hector-0.3.2/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.243958 bl_hector-0.3.2/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-21 11:30:42.243958 bl_hector-0.3.2/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0     1505 2023-06-21 11:30:42.243958 bl_hector-0.3.2/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.3.2/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1630 2023-06-21 11:30:42.243958 bl_hector-0.3.2/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3039 2023-06-21 11:30:42.243958 bl_hector-0.3.2/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.3.2/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3547 2023-06-21 11:30:42.247958 bl_hector-0.3.2/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.3.2/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1694 2023-06-21 11:30:42.247958 bl_hector-0.3.2/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4531 2023-06-23 16:18:20.470332 bl_hector-0.3.2/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-23 15:58:56.080839 bl_hector-0.3.2/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    99653 2023-07-12 08:50:02.536425 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.9.min.js
+-rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2364 2023-06-21 11:30:42.247958 bl_hector-0.3.2/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-23 16:18:20.470332 bl_hector-0.3.2/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4546 2023-06-21 11:30:42.251958 bl_hector-0.3.2/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     4012 2023-06-23 16:18:20.470332 bl_hector-0.3.2/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3363 2023-06-21 11:30:42.251958 bl_hector-0.3.2/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.3.2/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1690 2023-06-21 11:30:42.255958 bl_hector-0.3.2/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     5448 2023-06-27 05:50:57.836996 bl_hector-0.3.2/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     6060 2023-06-27 05:50:57.840996 bl_hector-0.3.2/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1842 2023-06-23 16:18:20.474332 bl_hector-0.3.2/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    19488 2023-06-23 16:18:20.474332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-21 11:30:42.255958 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4238 2023-06-23 16:18:20.474332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2105 2023-06-23 16:18:20.478332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     5746 2023-06-23 16:18:20.478332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3633 2023-06-23 16:18:20.478332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2057 2023-07-12 08:50:19.860206 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4768 2023-06-23 16:18:20.478332 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1845 2023-06-21 11:30:42.259958 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.3.2/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5276 2023-06-21 11:30:42.259958 bl_hector-0.3.2/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.3.2/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-07-12 08:52:06.230867 bl_hector-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4606 2023-07-12 08:53:06.450489 bl_hector-0.3.2/setup.py
+-rw-r--r--   0        0        0     3048 2023-07-12 08:53:06.452951 bl_hector-0.3.2/PKG-INFO
```

### Comparing `bl_hector-0.3.1/LICENSE` & `bl_hector-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/README.md` & `bl_hector-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/__init__.py` & `bl_hector-0.3.2/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/__init__.py` & `bl_hector-0.3.2/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.3.2/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/configuration/__init__.py` & `bl_hector-0.3.2/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/configuration/cli.py` & `bl_hector-0.3.2/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/configuration/wsgi.py` & `bl_hector-0.3.2/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/__init__.py` & `bl_hector-0.3.2/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/__init__.py` & `bl_hector-0.3.2/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/entities.py` & `bl_hector-0.3.2/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.3.2/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/repositories.py` & `bl_hector-0.3.2/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/services.py` & `bl_hector-0.3.2/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.3.2/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/services.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.3.2/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.9.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -150,17 +150,17 @@
                 if (S() === "-" && q() === "-" && (n.isWhitespace(N(2)) || N(2) === "" || N(2) === "-") || S() === "/" && q() === "/" && (n.isWhitespace(N(2)) || N(2) === "" || N(2) === "/")) {
                     h()
                 } else if (S() === "/" && q() === "*" && (n.isWhitespace(N(2)) || N(2) === "" || N(2) === "*")) {
                     v()
                 } else {
                     if (n.isWhitespace(S())) {
                         r.push(R())
-                    } else if (!C() && S() === "." && (n.isAlpha(q()) || q() === "{" || q() === "-")) {
+                    } else if (!I() && S() === "." && (n.isAlpha(q()) || q() === "{" || q() === "-")) {
                         r.push(d())
-                    } else if (!C() && S() === "#" && (n.isAlpha(q()) || q() === "{")) {
+                    } else if (!I() && S() === "#" && (n.isAlpha(q()) || q() === "{")) {
                         r.push(k())
                     } else if (S() === "[" && q() === "@") {
                         r.push(E())
                     } else if (S() === "@") {
                         r.push(T())
                     } else if (S() === "*" && n.isAlpha(q())) {
                         r.push(y())
@@ -181,15 +181,15 @@
                             c++
                         }
                         if (S() === "}") {
                             c--
                         }
                         r.push(b())
                     } else if (f() || n.isReservedChar(S())) {
-                        r.push(p("RESERVED", I()))
+                        r.push(p("RESERVED", C()))
                     } else {
                         if (o < a.length) {
                             throw Error("Unknown token: " + S() + " ")
                         }
                     }
                 }
             }
@@ -210,73 +210,73 @@
                     column: s,
                     line: u
                 }
             }
 
             function h() {
                 while (S() && !n.isNewline(S())) {
-                    I()
+                    C()
                 }
-                I()
+                C()
             }
 
             function v() {
                 while (S() && !(S() === "*" && q() === "/")) {
-                    I()
+                    C()
                 }
-                I();
-                I()
+                C();
+                C()
             }
 
             function d() {
                 var e = p("CLASS_REF");
-                var t = I();
+                var t = C();
                 if (S() === "{") {
                     e.template = true;
-                    t += I();
+                    t += C();
                     while (S() && S() !== "}") {
-                        t += I()
+                        t += C()
                     }
                     if (S() !== "}") {
                         throw Error("Unterminated class reference")
                     } else {
-                        t += I()
+                        t += C()
                     }
                 } else {
                     while (n.isValidCSSClassChar(S())) {
-                        t += I()
+                        t += C()
                     }
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function E() {
                 var e = p("ATTRIBUTE_REF");
-                var t = I();
+                var t = C();
                 while (o < a.length && S() !== "]") {
-                    t += I()
+                    t += C()
                 }
                 if (S() === "]") {
-                    t += I()
+                    t += C()
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function T() {
                 var e = p("ATTRIBUTE_REF");
-                var t = I();
+                var t = C();
                 while (n.isValidCSSIDChar(S())) {
-                    t += I()
+                    t += C()
                 }
                 if (S() === "=") {
-                    t += I();
+                    t += C();
                     if (S() === '"' || S() === "'") {
                         let e = w();
                         t += e.value
                     } else if (n.isAlpha(S()) || n.isNumeric(S()) || n.isIdentifierChar(S())) {
                         let e = x();
                         t += e.value
                     }
@@ -284,109 +284,109 @@
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function y() {
                 var e = p("STYLE_REF");
-                var t = I();
+                var t = C();
                 while (n.isAlpha(S()) || S() === "-") {
-                    t += I()
+                    t += C()
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function k() {
                 var e = p("ID_REF");
-                var t = I();
+                var t = C();
                 if (S() === "{") {
                     e.template = true;
-                    t += I();
+                    t += C();
                     while (S() && S() !== "}") {
-                        t += I()
+                        t += C()
                     }
                     if (S() !== "}") {
                         throw Error("Unterminated id reference")
                     } else {
-                        I()
+                        C()
                     }
                 } else {
                     while (n.isValidCSSIDChar(S())) {
-                        t += I()
+                        t += C()
                     }
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function x() {
                 var e = p("IDENTIFIER");
-                var t = I();
+                var t = C();
                 while (n.isAlpha(S()) || n.isNumeric(S()) || n.isIdentifierChar(S())) {
-                    t += I()
+                    t += C()
                 }
                 if (S() === "!" && t === "beep") {
-                    t += I()
+                    t += C()
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function g() {
                 var e = p("NUMBER");
-                var t = I();
+                var t = C();
                 while (n.isNumeric(S())) {
-                    t += I()
+                    t += C()
                 }
                 if (S() === "." && n.isNumeric(q())) {
-                    t += I()
+                    t += C()
                 }
                 while (n.isNumeric(S())) {
-                    t += I()
+                    t += C()
                 }
                 if (S() === "e" || S() === "E") {
                     if (n.isNumeric(q())) {
-                        t += I()
+                        t += C()
                     } else if (q() === "-") {
-                        t += I();
-                        t += I()
+                        t += C();
+                        t += C()
                     }
                 }
                 while (n.isNumeric(S())) {
-                    t += I()
+                    t += C()
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function b() {
                 var e = m();
-                var t = I();
+                var t = C();
                 while (S() && n.OP_TABLE[t + S()]) {
-                    t += I()
+                    t += C()
                 }
                 e.type = n.OP_TABLE[t];
                 e.value = t;
                 e.end = o;
                 return e
             }
 
             function w() {
                 var e = p("STRING");
-                var t = I();
+                var t = C();
                 var r = "";
                 while (S() && S() !== t) {
                     if (S() === "\\") {
-                        I();
-                        let e = I();
+                        C();
+                        let e = C();
                         if (e === "b") {
                             r += "\b"
                         } else if (e === "f") {
                             r += "\f"
                         } else if (e === "n") {
                             r += "\n"
                         } else if (e === "r") {
@@ -395,21 +395,21 @@
                             r += "\t"
                         } else if (e === "v") {
                             r += "\v"
                         } else {
                             r += e
                         }
                     } else {
-                        r += I()
+                        r += C()
                     }
                 }
                 if (S() !== t) {
                     throw Error("Unterminated string at " + n.positionString(e))
                 } else {
-                    I()
+                    C()
                 }
                 e.value = r;
                 e.end = o;
                 e.template = t === "`";
                 return e
             }
 
@@ -421,34 +421,34 @@
                 return a.charAt(o + 1)
             }
 
             function N(e = 1) {
                 return a.charAt(o + e)
             }
 
-            function I() {
+            function C() {
                 l = S();
                 o++;
                 s++;
                 return l
             }
 
-            function C() {
+            function I() {
                 return n.isAlpha(l) || n.isNumeric(l) || l === ")" || l === '"' || l === "'" || l === "`" || l === "}" || l === "]"
             }
 
             function R() {
                 var e = p("WHITESPACE");
                 var t = "";
                 while (S() && n.isWhitespace(S())) {
                     if (n.isNewline(S())) {
                         s = 0;
                         u++
                     }
-                    t += I()
+                    t += C()
                 }
                 e.value = t;
                 e.end = o;
                 return e
             }
         }
         tokenize(e, t) {
@@ -898,15 +898,15 @@
             }
             n.next = r
         }
     }
     class o {
         constructor(e, t) {
             this.lexer = e ?? new n;
-            this.parser = t ?? new a(this).use(h).use(v);
+            this.parser = t ?? new a(this).use(T).use(y);
             this.parser.runtime = this
         }
         matchesSelector(e, t) {
             var r = e.matches || e.matchesSelector || e.msMatchesSelector || e.mozMatchesSelector || e.webkitMatchesSelector || e.oMatchesSelector;
             return r && r.call(e, t)
         }
         makeEvent(t, r) {
@@ -933,15 +933,15 @@
         isArrayLike(e) {
             return Array.isArray(e) || typeof NodeList !== "undefined" && (e instanceof NodeList || e instanceof HTMLCollection)
         }
         isIterable(e) {
             return typeof e === "object" && Symbol.iterator in e && typeof e[Symbol.iterator] === "function"
         }
         shouldAutoIterate(e) {
-            return e != null && e[l] || this.isArrayLike(e)
+            return e != null && e[p] || this.isArrayLike(e)
         }
         forEach(e, t) {
             if (e == null) {} else if (this.isIterable(e)) {
                 for (const r of e) {
                     t(r)
                 }
             } else if (this.isArrayLike(e)) {
@@ -1143,15 +1143,15 @@
         addFeatures(e, t) {
             if (e) {
                 Object.assign(t.locals, this.getHyperscriptFeatures(e));
                 this.addFeatures(e.parentElement, t)
             }
         }
         makeContext(e, t, r, n) {
-            return new s(e, t, r, n, this)
+            return new f(e, t, r, n, this)
         }
         getScriptSelector() {
             return this.getScriptAttributes().map((function(e) {
                 return "[" + e + "]"
             })).join(", ")
         }
         convertValue(e, r) {
@@ -1289,25 +1289,25 @@
             var t = e.meta && e.meta.owner;
             if (t) {
                 var r = this.getInternalData(t);
                 var n = "elementScope";
                 if (e.meta.feature && e.meta.feature.behavior) {
                     n = e.meta.feature.behavior + "Scope"
                 }
-                var i = c(r, n);
+                var i = h(r, n);
                 return i
             } else {
                 return {}
             }
         }
         isReservedWord(e) {
             return ["meta", "it", "result", "locals", "event", "target", "detail", "sender", "body"].includes(e)
         }
         isHyperscriptContext(e) {
-            return e instanceof s
+            return e instanceof f
         }
         resolveSymbol(t, r, n) {
             if (t === "me" || t === "my" || t === "I") {
                 return r.me
             }
             if (t === "it" || t === "its" || t === "result") {
                 return r.result
@@ -1522,44 +1522,147 @@
                     queue: [],
                     executing: false
                 };
                 n.set(t, i)
             }
             return i
         }
+        beepValueToConsole(e, t, r) {
+            if (this.triggerEvent(e, "hyperscript:beep", {
+                    element: e,
+                    expression: t,
+                    value: r
+                })) {
+                var n;
+                if (r) {
+                    if (r instanceof m) {
+                        n = "ElementCollection"
+                    } else if (r.constructor) {
+                        n = r.constructor.name
+                    } else {
+                        n = "unknown"
+                    }
+                } else {
+                    n = "object (null)"
+                }
+                var a = r;
+                if (n === "String") {
+                    a = '"' + a + '"'
+                } else if (r instanceof m) {
+                    a = Array.from(r)
+                }
+                console.log("///_ BEEP! The expression (" + i.sourceFor.call(t).replace("beep! ", "") + ") evaluates to:", a, "of type " + n)
+            }
+        }
         hyperscriptUrl = "document" in e && document.currentScript ? document.currentScript.src : null
     }
-    class s {
+
+    function s() {
+        let e = document.cookie.split("; ").map((e => {
+            let t = e.split("=");
+            return {
+                name: t[0],
+                value: decodeURIComponent(t[1])
+            }
+        }));
+        return e
+    }
+
+    function u(e) {
+        document.cookie = e + "=;expires=Thu, 01 Jan 1970 00:00:00 GMT"
+    }
+
+    function l() {
+        for (const e of s()) {
+            u(e.name)
+        }
+    }
+    const c = new Proxy({}, {
+        get(e, t) {
+            if (t === "then" || t === "asyncWrapper") {
+                return null
+            } else if (t === "length") {
+                return s().length
+            } else if (t === "clear") {
+                return u
+            } else if (t === "clearAll") {
+                return l
+            } else if (typeof t === "string") {
+                if (!isNaN(t)) {
+                    return s()[parseInt(t)]
+                } else {
+                    let e = document.cookie.split("; ").find((e => e.startsWith(t + "=")))?.split("=")[1];
+                    if (e) {
+                        return decodeURIComponent(e)
+                    }
+                }
+            } else if (t === Symbol.iterator) {
+                return s()[t]
+            }
+        },
+        set(e, t, r) {
+            var n = null;
+            if ("string" === typeof r) {
+                n = encodeURIComponent(r);
+                n += ";samesite=lax"
+            } else {
+                n = encodeURIComponent(r.value);
+                if (r.expires) {
+                    n += ";expires=" + r.maxAge
+                }
+                if (r.maxAge) {
+                    n += ";max-age=" + r.maxAge
+                }
+                if (r.partitioned) {
+                    n += ";partitioned=" + r.partitioned
+                }
+                if (r.path) {
+                    n += ";path=" + r.path
+                }
+                if (r.samesite) {
+                    n += ";samesite=" + r.path
+                }
+                if (r.secure) {
+                    n += ";secure=" + r.path
+                }
+            }
+            document.cookie = t + "=" + r;
+            return true
+        }
+    });
+    class f {
         constructor(t, r, n, i, a) {
             this.meta = {
                 parser: a.parser,
                 lexer: a.lexer,
                 runtime: a,
                 owner: t,
                 feature: r,
                 iterators: {},
                 ctx: this
             };
-            this.locals = {};
+            this.locals = {
+                cookies: c
+            };
             this.me = n, this.you = undefined;
             this.result = undefined;
             this.event = i;
             this.target = i ? i.target : null;
             this.detail = i ? i.detail : null;
             this.sender = i ? i.detail ? i.detail.sender : null : null;
             this.body = "document" in e ? document.body : null;
             a.addFeatures(t, this)
         }
     }
-    class u {
+    class m {
         constructor(e, t, r) {
             this._css = e;
             this.relativeToElement = t;
             this.escape = r;
-            this[l] = true
+            this[p] = true
         }
         get css() {
             if (this.escape) {
                 return o.prototype.escapeSelector(this._css)
             } else {
                 return this._css
             }
@@ -1585,49 +1688,49 @@
             return e[Symbol.iterator]()
         }
         selectMatches() {
             let e = o.prototype.getRootNode(this.relativeToElement).querySelectorAll(this.css);
             return e
         }
     }
-    const l = Symbol();
+    const p = Symbol();
 
-    function c(e, t) {
+    function h(e, t) {
         var r = e[t];
         if (r) {
             return r
         } else {
             var n = {};
             e[t] = n;
             return n
         }
     }
 
-    function f(e) {
+    function v(e) {
         try {
             return JSON.parse(e)
         } catch (e) {
-            m(e);
+            d(e);
             return null
         }
     }
 
-    function m(e) {
+    function d(e) {
         if (console.error) {
             console.error(e)
         } else if (console.log) {
             console.log("ERROR: ", e)
         }
     }
 
-    function p(e, t) {
+    function E(e, t) {
         return new(e.bind.apply(e, [e].concat(t)))
     }
 
-    function h(t) {
+    function T(t) {
         t.addLeafExpression("parenthesized", (function(e, t, r) {
             if (r.matchOpToken("(")) {
                 var n = r.clearFollows();
                 try {
                     var i = e.requireElement("expression", r)
                 } finally {
                     r.restoreFollows(n)
@@ -1737,32 +1840,32 @@
                 var a = i.value.substring(2);
                 var o = n.tokenize(a);
                 var s = e.requireElement("expression", o);
                 return {
                     type: "classRefTemplate",
                     args: [s],
                     op: function(e, t) {
-                        return new u("." + t, e.me, true)
+                        return new m("." + t, e.me, true)
                     },
                     evaluate: function(e) {
                         return t.unifiedEval(this, e)
                     }
                 }
             } else {
                 const e = i.value;
                 return {
                     type: "classRef",
                     css: e,
                     evaluate: function(t) {
-                        return new u(e, t.me, true)
+                        return new m(e, t.me, true)
                     }
                 }
             }
         }));
-        class r extends u {
+        class r extends m {
             constructor(e, t, r) {
                 super(e, t);
                 this.templateParts = r;
                 this.elements = r.filter((e => e instanceof Element))
             }
             get css() {
                 let e = "",
@@ -1789,29 +1892,29 @@
             var s = o.map((function(e) {
                 if (e.type === "STRING") {
                     return '"' + e.value + '"'
                 } else {
                     return e.value
                 }
             })).join("");
-            var l, c, f;
+            var u, l, c;
             if (s.indexOf("$") >= 0) {
-                l = true;
-                c = n.tokenize(s, true);
-                f = e.parseStringTemplate(c)
+                u = true;
+                l = n.tokenize(s, true);
+                c = e.parseStringTemplate(l)
             }
             return {
                 type: "queryRef",
                 css: s,
-                args: f,
+                args: c,
                 op: function(e, ...t) {
-                    if (l) {
+                    if (u) {
                         return new r(s, e.me, t)
                     } else {
-                        return new u(s, e.me)
+                        return new m(s, e.me)
                     }
                 },
                 evaluate: function(e) {
                     return t.unifiedEval(this, e)
                 }
             }
         }));
@@ -2536,43 +2639,19 @@
             return e.parseAnyOf(["beepExpression", "logicalNot", "relativePositionalExpression", "positionalExpression", "noExpression", "negativeNumber", "postfixExpression"], r)
         }));
         t.addGrammarElement("beepExpression", (function(e, t, r) {
             if (!r.matchToken("beep!")) return;
             var n = e.parseElement("unaryExpression", r);
             if (n) {
                 n["booped"] = true;
-                var a = n.evaluate;
+                var i = n.evaluate;
                 n.evaluate = function(e) {
-                    let r = a.apply(n, arguments);
-                    let o = e.me;
-                    if (t.triggerEvent(o, "hyperscript:beep", {
-                            element: o,
-                            expression: n,
-                            value: r
-                        })) {
-                        var s;
-                        if (r) {
-                            if (r instanceof u) {
-                                s = "ElementCollection"
-                            } else if (r.constructor) {
-                                s = r.constructor.name
-                            } else {
-                                s = "unknown"
-                            }
-                        } else {
-                            s = "object (null)"
-                        }
-                        var l = r;
-                        if (s === "String") {
-                            l = '"' + l + '"'
-                        } else if (r instanceof u) {
-                            l = Array.from(r)
-                        }
-                        console.log("///_ BEEP! The expression (" + i.sourceFor.call(n).substr(6) + ") evaluates to:", l, "of type " + s)
-                    }
+                    let r = i.apply(n, arguments);
+                    let a = e.me;
+                    t.beepValueToConsole(a, n, r);
                     return r
                 };
                 return n
             }
         }));
         var s = function(e, t, r, n) {
             var i = t.querySelectorAll(r);
@@ -2582,27 +2661,27 @@
                     return o
                 }
             }
             if (n) {
                 return i[0]
             }
         };
-        var l = function(e, t, r, n) {
+        var u = function(e, t, r, n) {
             var i = t.querySelectorAll(r);
             for (var a = i.length - 1; a >= 0; a--) {
                 var o = i[a];
                 if (o.compareDocumentPosition(e) === Node.DOCUMENT_POSITION_FOLLOWING) {
                     return o
                 }
             }
             if (n) {
                 return i[i.length - 1]
             }
         };
-        var f = function(e, t, r, n) {
+        var l = function(e, t, r, n) {
             var i = [];
             o.prototype.forEach(t, (function(t) {
                 if (t.matches(r) || t === e) {
                     i.push(t)
                 }
             }));
             for (var a = 0; a < i.length - 1; a++) {
@@ -2614,76 +2693,76 @@
             if (n) {
                 var u = i[0];
                 if (u && u.matches(r)) {
                     return u
                 }
             }
         };
-        var m = function(e, t, r, n) {
-            return f(e, Array.from(t).reverse(), r, n)
+        var c = function(e, t, r, n) {
+            return l(e, Array.from(t).reverse(), r, n)
         };
         t.addGrammarElement("relativePositionalExpression", (function(e, t, r) {
             var n = r.matchAnyToken("next", "previous");
             if (!n) return;
-            var i = n.value === "next";
-            var a = e.parseElement("expression", r);
+            var a = n.value === "next";
+            var o = e.parseElement("expression", r);
             if (r.matchToken("from")) {
                 r.pushFollow("in");
                 try {
-                    var o = e.requireElement("unaryExpression", r)
+                    var f = e.requireElement("unaryExpression", r)
                 } finally {
                     r.popFollow()
                 }
             } else {
-                var o = e.requireElement("implicitMeTarget", r)
+                var f = e.requireElement("implicitMeTarget", r)
             }
-            var u = false;
-            var c;
+            var m = false;
+            var p;
             if (r.matchToken("in")) {
-                u = true;
-                var p = e.requireElement("unaryExpression", r)
+                m = true;
+                var h = e.requireElement("unaryExpression", r)
             } else if (r.matchToken("within")) {
-                c = e.requireElement("unaryExpression", r)
+                p = e.requireElement("unaryExpression", r)
             } else {
-                c = document.body
+                p = document.body
             }
-            var h = false;
+            var v = false;
             if (r.matchToken("with")) {
                 r.requireToken("wrapping");
-                h = true
+                v = true
             }
             return {
                 type: "relativePositionalExpression",
-                from: o,
-                forwardSearch: i,
-                inSearch: u,
-                wrapping: h,
-                inElt: p,
-                withinElt: c,
+                from: f,
+                forwardSearch: a,
+                inSearch: m,
+                wrapping: v,
+                inElt: h,
+                withinElt: p,
                 operator: n.value,
-                args: [a, o, p, c],
-                op: function(e, t, r, n, a) {
-                    var o = t.css;
-                    if (o == null) {
-                        throw "Expected a CSS value"
+                args: [o, f, h, p],
+                op: function(e, t, r, n, f) {
+                    var p = t.css;
+                    if (p == null) {
+                        throw "Expected a CSS value to be returned by " + i.sourceFor.apply(o)
                     }
-                    if (u) {
+                    if (m) {
                         if (n) {
-                            if (i) {
-                                return f(r, n, o, h)
+                            if (a) {
+                                return l(r, n, p, v)
                             } else {
-                                return m(r, n, o, h)
+                                return c(r, n, p, v)
                             }
                         }
                     } else {
-                        if (a) {
-                            if (i) {
-                                return s(r, a, o, h)
+                        if (f) {
+                            if (a) {
+                                return s(r, f, p, v)
                             } else {
-                                return l(r, a, o, h)
+                                return u(r, f, p, v)
                             }
                         }
                     }
                 },
                 evaluate: function(e) {
                     return t.unifiedEval(this, e)
                 }
@@ -2761,25 +2840,25 @@
             }
             return n
         }));
         t.addGrammarElement("mathExpression", (function(e, t, r) {
             return e.parseAnyOf(["mathOperator", "unaryExpression"], r)
         }));
 
-        function h(e, t, r) {
+        function f(e, t, r) {
             if (t["contains"]) {
                 return t.contains(r)
             } else if (t["includes"]) {
                 return t.includes(r)
             } else {
                 throw Error("The value of " + e.sourceFor() + " does not have a contains or includes method on it")
             }
         }
 
-        function v(e, t, r) {
+        function p(e, t, r) {
             if (t["match"]) {
                 return !!t.match(r)
             } else if (t["matches"]) {
                 return t.matches(r)
             } else {
                 throw Error("The value of " + e.sourceFor() + " does not have a match or matches method on it")
             }
@@ -2798,15 +2877,22 @@
                         } else if (r.matchToken("a")) {
                             a = "not a";
                             s = true
                         } else if (r.matchToken("empty")) {
                             a = "not empty";
                             o = false
                         } else {
-                            a = "!="
+                            if (r.matchToken("really")) {
+                                a = "!=="
+                            } else {
+                                a = "!="
+                            }
+                            if (r.matchToken("equal")) {
+                                r.matchToken("to")
+                            }
                         }
                     } else if (r.matchToken("in")) {
                         a = "in"
                     } else if (r.matchToken("a")) {
                         a = "a";
                         s = true
                     } else if (r.matchToken("empty")) {
@@ -2827,16 +2913,28 @@
                             r.requireToken("equal");
                             r.requireToken("to");
                             a = ">="
                         } else {
                             a = ">"
                         }
                     } else {
-                        a = "=="
+                        if (r.matchToken("really")) {
+                            a = "==="
+                        } else {
+                            a = "=="
+                        }
+                        if (r.matchToken("equal")) {
+                            r.matchToken("to")
+                        }
                     }
+                } else if (r.matchToken("equals")) {
+                    a = "=="
+                } else if (r.matchToken("really")) {
+                    r.requireToken("equals");
+                    a = "==="
                 } else if (r.matchToken("exist") || r.matchToken("exists")) {
                     a = "exist";
                     o = false
                 } else if (r.matchToken("matches") || r.matchToken("match")) {
                     a = "match"
                 } else if (r.matchToken("contains") || r.matchToken("contain")) {
                     a = "contain"
@@ -2865,52 +2963,57 @@
                     l = !r.matchOpToken("!")
                 } else if (o) {
                     c = e.requireElement("mathExpression", r);
                     if (a === "match" || a === "not match") {
                         c = c.css ? c.css : c
                     }
                 }
-                var f = n;
+                var m = n;
                 n = {
                     type: "comparisonOperator",
                     operator: a,
                     typeName: u,
                     nullOk: l,
                     lhs: n,
                     rhs: c,
                     args: [n, c],
                     op: function(e, r, n) {
                         if (a === "==") {
                             return r == n
                         } else if (a === "!=") {
                             return r != n
                         }
+                        if (a === "===") {
+                            return r === n
+                        } else if (a === "!==") {
+                            return r !== n
+                        }
                         if (a === "match") {
-                            return r != null && v(f, r, n)
+                            return r != null && p(m, r, n)
                         }
                         if (a === "not match") {
-                            return r == null || !v(f, r, n)
+                            return r == null || !p(m, r, n)
                         }
                         if (a === "in") {
-                            return n != null && h(c, n, r)
+                            return n != null && f(c, n, r)
                         }
                         if (a === "not in") {
-                            return n == null || !h(c, n, r)
+                            return n == null || !f(c, n, r)
                         }
                         if (a === "contain") {
-                            return r != null && h(f, r, n)
+                            return r != null && f(m, r, n)
                         }
                         if (a === "not contain") {
-                            return r == null || !h(f, r, n)
+                            return r == null || !f(m, r, n)
                         }
                         if (a === "include") {
-                            return r != null && h(f, r, n)
+                            return r != null && f(m, r, n)
                         }
                         if (a === "not include") {
-                            return r == null || !h(f, r, n)
+                            return r == null || !f(m, r, n)
                         }
                         if (a === "===") {
                             return r === n
                         } else if (a === "!==") {
                             return r !== n
                         } else if (a === "<") {
                             return r < n
@@ -3028,15 +3131,15 @@
                 apply: function(e, t, r) {
                     for (const i of n) {
                         i.install(e, t, r)
                     }
                 }
             }
         }));
-        var d = function(e) {
+        var v = function(e) {
             var t = [];
             if (e.token(0).value === "(" && (e.token(1).value === ")" || e.token(2).value === "," || e.token(2).value === ")")) {
                 e.matchOpToken("(");
                 do {
                     t.push(e.requireTokenType("IDENTIFIER"))
                 } while (e.matchOpToken(","));
                 e.requireOpToken(")")
@@ -3055,15 +3158,15 @@
                 var o = e.requireElement("eventName", r, "Expected event name");
                 var s = o.evaluate();
                 if (a) {
                     a = a + " or " + s
                 } else {
                     a = "on " + s
                 }
-                var u = d(r);
+                var u = v(r);
                 var l = null;
                 if (r.matchOpToken("[")) {
                     l = e.requireElement("expression", r);
                     r.requireOpToken("]")
                 }
                 var c, f, m;
                 if (r.currentToken().type === "NUMBER") {
@@ -3075,26 +3178,26 @@
                         if (!h.value) return;
                         f = parseInt(h.value)
                     } else if (r.matchToken("and")) {
                         m = true;
                         r.requireToken("on")
                     }
                 }
-                var v, E;
+                var d, E;
                 if (s === "intersection") {
-                    v = {};
+                    d = {};
                     if (r.matchToken("with")) {
-                        v["with"] = e.requireElement("expression", r).evaluate()
+                        d["with"] = e.requireElement("expression", r).evaluate()
                     }
                     if (r.matchToken("having")) {
                         do {
                             if (r.matchToken("margin")) {
-                                v["rootMargin"] = e.requireElement("stringLike", r).evaluate()
+                                d["rootMargin"] = e.requireElement("stringLike", r).evaluate()
                             } else if (r.matchToken("threshold")) {
-                                v["threshold"] = e.requireElement("expression", r).evaluate()
+                                d["threshold"] = e.requireElement("expression", r).evaluate()
                             } else {
                                 e.raiseParseError(r, "Unknown intersection config specification")
                             }
                         } while (r.matchToken("and"))
                     }
                 } else if (s === "mutation") {
                     E = {};
@@ -3178,58 +3281,58 @@
                     elsewhere: k,
                     startCount: c,
                     endCount: f,
                     unbounded: m,
                     debounceTime: b,
                     throttleTime: w,
                     mutationSpec: E,
-                    intersectionSpec: v,
+                    intersectionSpec: d,
                     debounced: undefined,
                     lastExec: undefined
                 })
             } while (r.matchToken("or"));
             var S = true;
             if (!n) {
                 if (r.matchToken("queue")) {
                     if (r.matchToken("all")) {
                         var q = true;
                         var S = false
                     } else if (r.matchToken("first")) {
                         var N = true
                     } else if (r.matchToken("none")) {
-                        var I = true
+                        var C = true
                     } else {
                         r.requireToken("last")
                     }
                 }
             }
-            var C = e.requireElement("commandList", r);
-            e.ensureTerminated(C);
+            var I = e.requireElement("commandList", r);
+            e.ensureTerminated(I);
             var R, A;
             if (r.matchToken("catch")) {
                 R = r.requireTokenType("IDENTIFIER").value;
                 A = e.requireElement("commandList", r);
                 e.ensureTerminated(A)
             }
             if (r.matchToken("finally")) {
                 var O = e.requireElement("commandList", r);
                 e.ensureTerminated(O)
             }
             var L = {
                 displayName: a,
                 events: i,
-                start: C,
+                start: I,
                 every: n,
                 execCount: 0,
                 errorHandler: A,
                 errorSymbol: R,
                 execute: function(e) {
                     let r = t.getEventQueueFor(e.me, L);
                     if (r.executing && n === false) {
-                        if (I || N && r.queue.length > 0) {
+                        if (C || N && r.queue.length > 0) {
                             return
                         }
                         if (S) {
                             r.queue.length = 0
                         }
                         r.queue.push(e);
                         return
@@ -3251,15 +3354,15 @@
                         if (n) {
                             n.print()
                         }
                         t.triggerEvent(e.me, "exception", {
                             error: r
                         })
                     };
-                    C.execute(e)
+                    I.execute(e)
                 },
                 install: function(e, r) {
                     for (const r of L.events) {
                         var n;
                         if (r.elsewhere) {
                             n = [document]
                         } else if (r.from) {
@@ -3381,15 +3484,15 @@
                                 }
                                 L.execute(s)
                             }))
                         }))
                     }
                 }
             };
-            e.setParent(C, L);
+            e.setParent(I, L);
             return L
         }));
         t.addFeature("def", (function(e, t, r) {
             if (!r.matchToken("def")) return;
             var n = e.requireElement("dotOrColonPath", r);
             var i = n.evaluate();
             var a = i.split(".");
@@ -3519,22 +3622,22 @@
                 do {
                     s.push(n.requireTokenType("IDENTIFIER").value)
                 } while (n.matchOpToken(","));
                 n.requireOpToken(")")
             }
             var u = t.requireElement("hyperscript", n);
             for (var l = 0; l < u.features.length; l++) {
-                var f = u.features[l];
-                f.behavior = i
+                var c = u.features[l];
+                c.behavior = i
             }
             return {
                 install: function(t, n) {
                     r.assignToNamespace(e.document && e.document.body, a, o, (function(e, t, n) {
                         var a = r.getInternalData(e);
-                        var o = c(a, i + "Scope");
+                        var o = h(a, i + "Scope");
                         for (var l = 0; l < s.length; l++) {
                             o[s[l]] = n[s[l]]
                         }
                         u.apply(e, t)
                     }))
                 }
             }
@@ -3619,15 +3722,15 @@
                         i.push(a.value)
                     } while (n.matchOpToken(","));
                     n.requireOpToken(")")
                 }
             }
             var o = t.requireElement("jsBody", n);
             n.matchToken("end");
-            var s = p(Function, i.concat([o.jsSource]));
+            var s = E(Function, i.concat([o.jsSource]));
             var u = {
                 jsSource: o.jsSource,
                 function: s,
                 inputs: i,
                 op: function(t) {
                     var n = [];
                     i.forEach((function(e) {
@@ -3727,15 +3830,15 @@
                     if (a.type === "NUMBER" || a.type === "L_PAREN") {
                         i.push({
                             time: e.requireElement("expression", r).evaluate()
                         })
                     } else {
                         i.push({
                             name: e.requireElement("dotOrColonPath", r, "Expected event name").evaluate(),
-                            args: d(r)
+                            args: v(r)
                         })
                     }
                 } while (r.matchToken("or"));
                 if (r.matchToken("from")) {
                     var o = e.requireElement("expression", r)
                 }
                 n = {
@@ -3825,45 +3928,45 @@
                         return n.value
                     }
                 }
             }
             return e.parseElement("dotOrColonPath", r)
         }));
 
-        function E(e, t, r, n) {
+        function d(e, t, r, n) {
             var i = t.requireElement("eventName", n);
             var a = t.parseElement("namedArgumentList", n);
             if (e === "send" && n.matchToken("to") || e === "trigger" && n.matchToken("on")) {
                 var o = t.requireElement("expression", n)
             } else {
                 var o = t.requireElement("implicitMeTarget", n)
             }
             var s = {
                 eventName: i,
                 details: a,
                 to: o,
                 args: [o, i, a],
                 op: function(e, t, n, i) {
                     r.nullCheck(t, o);
-                    r.forEach(t, (function(t) {
+                    r.implicitLoop(t, (function(t) {
                         r.triggerEvent(t, n, i, e.me)
                     }));
                     return r.findNext(s, e)
                 }
             };
             return s
         }
         t.addCommand("trigger", (function(e, t, r) {
             if (r.matchToken("trigger")) {
-                return E("trigger", e, t, r)
+                return d("trigger", e, t, r)
             }
         }));
         t.addCommand("send", (function(e, t, r) {
             if (r.matchToken("send")) {
-                return E("send", e, t, r)
+                return d("send", e, t, r)
             }
         }));
         var T = function(e, t, r, n) {
             if (n) {
                 if (e.commandBoundary(r.currentToken())) {
                     e.raiseParseError(r, "'return' commands must return a value.  If you do not wish to return a value, use 'exit' instead.")
                 } else {
@@ -3960,14 +4063,34 @@
                         console.log.apply(null, n)
                     }
                     return t.findNext(this, e)
                 }
             };
             return a
         }));
+        t.addCommand("beep!", (function(e, t, r) {
+            if (!r.matchToken("beep!")) return;
+            var n = [e.parseElement("expression", r)];
+            while (r.matchOpToken(",")) {
+                n.push(e.requireElement("expression", r))
+            }
+            var i = {
+                exprs: n,
+                args: [n],
+                op: function(e, r) {
+                    for (let i = 0; i < n.length; i++) {
+                        const a = n[i];
+                        const o = r[i];
+                        t.beepValueToConsole(e.me, a, o)
+                    }
+                    return t.findNext(this, e)
+                }
+            };
+            return i
+        }));
         t.addCommand("throw", (function(e, t, r) {
             if (!r.matchToken("throw")) return;
             var n = e.requireElement("expression", r);
             var i = {
                 expr: n,
                 args: [n],
                 op: function(e, r) {
@@ -4041,15 +4164,15 @@
                     }
                 };
                 return o
             } else {
                 o = {
                     args: [n, i],
                     op: function(e, r, n) {
-                        e.result = p(r, n);
+                        e.result = E(r, n);
                         if (a) {
                             t.setSymbol(a.name, e, a.scope, e.result)
                         }
                         return t.findNext(this, e)
                     }
                 };
                 return o
@@ -4741,15 +4864,15 @@
                     }))
                 }
             };
             return u
         }))
     }
 
-    function v(e) {
+    function y(e) {
         e.addCommand("settle", (function(e, t, r) {
             if (r.matchToken("settle")) {
                 if (!e.commandBoundary(r.currentToken())) {
                     var n = e.requireElement("expression", r)
                 } else {
                     var n = e.requireElement("implicitMeTarget", r)
                 }
@@ -5270,44 +5393,80 @@
                         return t.findNext(this, e)
                     }
                 }
             }
         }));
         e.addCommand("take", (function(e, t, r) {
             if (r.matchToken("take")) {
-                var n = e.requireElement("classRef", r);
+                var n = e.parseElement("classRef", r);
+                var i = null;
+                var a = null;
+                if (n == null) {
+                    i = e.parseElement("attributeRef", r);
+                    if (i == null) {
+                        e.raiseParseError(r, "Expected either a class reference or attribute expression")
+                    }
+                    if (r.matchToken("with")) {
+                        a = e.requireElement("expression", r)
+                    }
+                }
                 if (r.matchToken("from")) {
-                    var i = e.requireElement("expression", r)
+                    var o = e.requireElement("expression", r)
                 } else {
-                    var i = n
+                    var o = n
                 }
                 if (r.matchToken("for")) {
-                    var a = e.requireElement("expression", r)
+                    var s = e.requireElement("expression", r)
                 } else {
-                    var a = e.requireElement("implicitMeTarget", r)
+                    var s = e.requireElement("implicitMeTarget", r)
+                }
+                if (n) {
+                    var u = {
+                        classRef: n,
+                        from: o,
+                        forElt: s,
+                        args: [n, o, s],
+                        op: function(e, r, n, i) {
+                            t.nullCheck(n, o);
+                            t.nullCheck(i, s);
+                            var a = r.className;
+                            t.implicitLoop(n, (function(e) {
+                                e.classList.remove(a)
+                            }));
+                            t.implicitLoop(i, (function(e) {
+                                e.classList.add(a)
+                            }));
+                            return t.findNext(this, e)
+                        }
+                    };
+                    return u
+                } else {
+                    var u = {
+                        attributeRef: i,
+                        from: o,
+                        forElt: s,
+                        args: [o, s, a],
+                        op: function(e, r, n, a) {
+                            t.nullCheck(r, o);
+                            t.nullCheck(n, s);
+                            t.implicitLoop(r, (function(e) {
+                                if (!a) {
+                                    e.removeAttribute(i.name)
+                                } else {
+                                    e.setAttribute(i.name, a)
+                                }
+                            }));
+                            t.implicitLoop(n, (function(e) {
+                                e.setAttribute(i.name, i.value || "")
+                            }));
+                            return t.findNext(this, e)
+                        }
+                    };
+                    return u
                 }
-                var o = {
-                    classRef: n,
-                    from: i,
-                    forElt: a,
-                    args: [n, i, a],
-                    op: function(e, r, n, o) {
-                        t.nullCheck(n, i);
-                        t.nullCheck(o, a);
-                        var s = r.className;
-                        t.implicitLoop(n, (function(e) {
-                            e.classList.remove(s)
-                        }));
-                        t.implicitLoop(o, (function(e) {
-                            e.classList.add(s)
-                        }));
-                        return t.findNext(this, e)
-                    }
-                };
-                return o
             }
         }));
 
         function a(t, r, n, i) {
             if (n != null) {
                 var a = t.resolveSymbol(n, r)
             } else {
@@ -5903,79 +6062,79 @@
                     t.innerHTML = e;
                     r.append(t.content)
                 }
             }));
             return r
         }
     }
-    const d = new o,
-        E = d.lexer,
-        T = d.parser;
+    const k = new o,
+        x = k.lexer,
+        g = k.parser;
 
-    function y(e, t) {
-        return d.evaluate(e, t)
+    function b(e, t) {
+        return k.evaluate(e, t)
     }
 
-    function k() {
+    function w() {
         var t = Array.from(e.document.querySelectorAll("script[type='text/hyperscript'][src]"));
         Promise.all(t.map((function(e) {
             return fetch(e.src).then((function(e) {
                 return e.text()
             }))
-        }))).then((e => e.forEach((e => x(e))))).then((() => n((function() {
+        }))).then((e => e.forEach((e => S(e))))).then((() => n((function() {
             a();
-            d.processNode(document.documentElement);
+            k.processNode(document.documentElement);
             e.document.addEventListener("htmx:load", (function(e) {
-                d.processNode(e.detail.elt)
+                k.processNode(e.detail.elt)
             }))
         }))));
 
         function n(e) {
             if (document.readyState !== "loading") {
                 setTimeout(e)
             } else {
                 document.addEventListener("DOMContentLoaded", e)
             }
         }
 
         function i() {
             var e = document.querySelector('meta[name="htmx-config"]');
             if (e) {
-                return f(e.content)
+                return v(e.content)
             } else {
                 return null
             }
         }
 
         function a() {
             var e = i();
             if (e) {
                 Object.assign(r, e)
             }
         }
     }
-    const x = Object.assign(y, {
+    const S = Object.assign(b, {
         config: r,
         use(e) {
-            e(x)
+            e(S)
         },
         internals: {
-            lexer: E,
-            parser: T,
-            runtime: d,
+            lexer: x,
+            parser: g,
+            runtime: k,
             Lexer: n,
             Tokens: i,
             Parser: a,
             Runtime: o
         },
-        ElementCollection: u,
-        addFeature: T.addFeature.bind(T),
-        addCommand: T.addCommand.bind(T),
-        addLeafExpression: T.addLeafExpression.bind(T),
-        addIndirectExpression: T.addIndirectExpression.bind(T),
-        evaluate: d.evaluate.bind(d),
-        parse: d.parse.bind(d),
-        processNode: d.processNode.bind(d),
-        browserInit: k
+        ElementCollection: m,
+        addFeature: g.addFeature.bind(g),
+        addCommand: g.addCommand.bind(g),
+        addLeafExpression: g.addLeafExpression.bind(g),
+        addIndirectExpression: g.addIndirectExpression.bind(g),
+        evaluate: k.evaluate.bind(k),
+        parse: k.parse.bind(k),
+        processNode: k.processNode.bind(k),
+        browserInit: w
     });
-    return x
+    return S
 }));
```

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.3.2/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/settings.py` & `bl_hector-0.3.2/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.3.2/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.3.2/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.3.2/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.3.2/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/exceptions.py` & `bl_hector-0.3.2/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/from_dict.py` & `bl_hector-0.3.2/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/from_json.py` & `bl_hector-0.3.2/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.3.2/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.3.2/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     link(rel="icon" type="image/svg" href="#{url_for('static', filename='favicon.svg')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
     block links
 
-    script(src="#{url_for('static', filename='js/hyperscript@0.9.8.min.js')}")
-    script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}")
+    script(src="#{url_for('static', filename='js/hyperscript@0.9.9.min.js')}" defer)
+    script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}" defer)
     block head_scripts
 
   body(hx-boost="true")
     +navbar()
 
     .page
       - var messages = get_flashed_messages(with_categories=true)
```

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.3.2/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/bl_hector/interfaces/utils.py` & `bl_hector-0.3.2/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.1/pyproject.toml` & `bl_hector-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.3.1"
+version = "0.3.2"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
```

### Comparing `bl_hector-0.3.1/setup.py` & `bl_hector-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.easter-eggs.org/bioneland/hector',
```

### Comparing `bl_hector-0.3.1/PKG-INFO` & `bl_hector-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection manager.
 Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

