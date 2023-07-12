# Comparing `tmp/no-comment-0.1.0a9.tar.gz` & `tmp/no-comment-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no-comment-0.1.0a9.tar", max compression
+gzip compressed data, was "no-comment-0.1.1.tar", max compression
```

## Comparing `no-comment-0.1.0a9.tar` & `no-comment-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    34523 2023-01-04 16:29:03.268951 no-comment-0.1.0a9/LICENSE
--rw-r--r--   0        0        0     1806 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/README.md
--rw-r--r--   0        0        0      822 2023-01-04 16:29:03.268951 no-comment-0.1.0a9/no_comment/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 13:32:42.026352 no-comment-0.1.0a9/no_comment/application/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 13:33:05.026067 no-comment-0.1.0a9/no_comment/application/use_cases/__init__.py
--rw-r--r--   0        0        0     2217 2023-07-01 09:50:20.258247 no-comment-0.1.0a9/no_comment/application/use_cases/add_comment.py
--rw-r--r--   0        0        0     2334 2023-07-01 09:49:57.074519 no-comment-0.1.0a9/no_comment/application/use_cases/create_stream.py
--rw-r--r--   0        0        0     2347 2023-07-01 09:49:30.058835 no-comment-0.1.0a9/no_comment/application/use_cases/display_stream.py
--rw-r--r--   0        0        0      963 2023-06-28 08:05:43.226481 no-comment-0.1.0a9/no_comment/configuration/__init__.py
--rw-r--r--   0        0        0     1020 2023-06-28 08:25:18.860334 no-comment-0.1.0a9/no_comment/configuration/cli.py
--rw-r--r--   0        0        0     1025 2023-06-28 08:05:47.150433 no-comment-0.1.0a9/no_comment/configuration/wsgi.py
--rw-r--r--   0        0        0      736 2023-01-07 14:02:19.276425 no-comment-0.1.0a9/no_comment/domain/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 14:02:22.416386 no-comment-0.1.0a9/no_comment/domain/commenting/__init__.py
--rw-r--r--   0        0        0     1147 2023-07-01 09:34:32.001345 no-comment-0.1.0a9/no_comment/domain/commenting/entities.py
--rw-r--r--   0        0        0      914 2023-07-01 10:00:43.526842 no-comment-0.1.0a9/no_comment/domain/commenting/exceptions.py
--rw-r--r--   0        0        0     1482 2023-06-28 15:11:18.695494 no-comment-0.1.0a9/no_comment/domain/commenting/repositories.py
--rw-r--r--   0        0        0      989 2023-06-28 08:05:47.162433 no-comment-0.1.0a9/no_comment/domain/commenting/services.py
--rw-r--r--   0        0        0     1715 2023-07-01 10:03:27.048971 no-comment-0.1.0a9/no_comment/domain/commenting/value_objects.py
--rw-r--r--   0        0        0      736 2023-01-04 16:29:03.272951 no-comment-0.1.0a9/no_comment/infrastructure/__init__.py
--rw-r--r--   0        0        0     2504 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/click/__init__.py
--rw-r--r--   0        0        0     1550 2023-06-30 14:44:39.649471 no-comment-0.1.0a9/no_comment/infrastructure/click/services.py
--rw-r--r--   0        0        0     3034 2023-07-11 07:43:46.196223 no-comment-0.1.0a9/no_comment/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1680 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-11 07:38:42.327993 no-comment-0.1.0a9/no_comment/infrastructure/flask/ip/__init__.py
--rw-r--r--   0        0        0     2491 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-16 06:00:11.291713 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0      213 2023-07-01 10:10:02.572179 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/no-comment.css
--rw-r--r--   0        0        0     1467 2023-06-16 07:14:41.219262 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/favicon.svg
--rw-r--r--   0        0        0      551 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/feed.svg
--rw-r--r--   0        0        0      361 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/filter-off.svg
--rw-r--r--   0        0        0      338 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/filter.svg
--rw-r--r--   0        0        0    42819 2023-06-16 06:00:11.291713 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-28 06:33:12.566707 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     3512 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/streams.py
--rw-r--r--   0        0        0     2003 2023-07-11 07:18:44.097988 no-comment-0.1.0a9/no_comment/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1415 2023-06-30 14:40:26.308668 no-comment-0.1.0a9/no_comment/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     2374 2023-07-11 07:32:00.081972 no-comment-0.1.0a9/no_comment/infrastructure/settings.py
--rw-r--r--   0        0        0      736 2023-06-28 08:05:43.230481 no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4621 2023-07-02 16:52:08.051300 no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2154 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/__init__.py
--rw-r--r--   0        0        0     1426 2023-02-15 08:17:41.803550 no-comment-0.1.0a9/no_comment/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0     7432 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-11 07:44:32.735568 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     1878 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1130 2023-01-29 14:29:41.635851 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
--rw-r--r--   0        0        0      860 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug
--rw-r--r--   0        0        0     5333 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/display.pug
--rw-r--r--   0        0        0      980 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/root.pug
--rw-r--r--   0        0        0      967 2023-07-11 07:12:10.045688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug
--rw-r--r--   0        0        0     1772 2023-07-11 07:12:10.045688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     3578 2023-07-01 09:36:21.732089 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_json.py
--rw-r--r--   0        0        0     6006 2023-07-01 09:36:02.516311 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_xml.py
--rw-r--r--   0        0        0      869 2023-06-30 13:42:06.404624 no-comment-0.1.0a9/no_comment/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-30 13:42:06.404624 no-comment-0.1.0a9/no_comment/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1810 2023-06-30 13:43:27.787615 no-comment-0.1.0a9/no_comment/test_factories.py
--rw-r--r--   0        0        0     1238 2023-07-11 07:45:30.430797 no-comment-0.1.0a9/pyproject.toml
--rw-r--r--   0        0        0     3936 2023-07-11 07:46:34.919464 no-comment-0.1.0a9/setup.py
--rw-r--r--   0        0        0     2710 2023-07-11 07:46:34.920215 no-comment-0.1.0a9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-12 08:47:42.782193 no-comment-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1806 2023-07-12 08:47:42.786193 no-comment-0.1.1/README.md
+-rw-r--r--   0        0        0      822 2023-07-12 08:47:42.786193 no-comment-0.1.1/no_comment/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.786193 no-comment-0.1.1/no_comment/application/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.786193 no-comment-0.1.1/no_comment/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-12 08:47:42.786193 no-comment-0.1.1/no_comment/application/use_cases/add_comment.py
+-rw-r--r--   0        0        0     2334 2023-07-12 08:47:42.790192 no-comment-0.1.1/no_comment/application/use_cases/create_stream.py
+-rw-r--r--   0        0        0     2347 2023-07-12 08:47:42.790192 no-comment-0.1.1/no_comment/application/use_cases/display_stream.py
+-rw-r--r--   0        0        0      963 2023-07-12 08:47:42.790192 no-comment-0.1.1/no_comment/configuration/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-12 08:47:42.790192 no-comment-0.1.1/no_comment/configuration/cli.py
+-rw-r--r--   0        0        0     1025 2023-07-12 08:47:42.790192 no-comment-0.1.1/no_comment/configuration/wsgi.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/__init__.py
+-rw-r--r--   0        0        0     1147 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/entities.py
+-rw-r--r--   0        0        0      914 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/exceptions.py
+-rw-r--r--   0        0        0     1482 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/repositories.py
+-rw-r--r--   0        0        0      989 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/services.py
+-rw-r--r--   0        0        0     1715 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/domain/commenting/value_objects.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.794192 no-comment-0.1.1/no_comment/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2504 2023-07-12 08:47:42.798192 no-comment-0.1.1/no_comment/infrastructure/click/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-12 08:47:42.798192 no-comment-0.1.1/no_comment/infrastructure/click/services.py
+-rw-r--r--   0        0        0     3034 2023-07-12 08:47:42.798192 no-comment-0.1.1/no_comment/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     2058 2023-07-12 10:21:18.879122 no-comment-0.1.1/no_comment/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     1610 2023-07-12 10:01:25.930005 no-comment-0.1.1/no_comment/infrastructure/flask/ip/__init__.py
+-rw-r--r--   0        0        0     2491 2023-07-12 08:47:42.798192 no-comment-0.1.1/no_comment/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0      213 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/css/no-comment.css
+-rw-r--r--   0        0        0     1467 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/img/favicon.svg
+-rw-r--r--   0        0        0      551 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/img/feed.svg
+-rw-r--r--   0        0        0      361 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/img/filter-off.svg
+-rw-r--r--   0        0        0      338 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/img/filter.svg
+-rw-r--r--   0        0        0    42819 2023-07-12 08:47:42.802192 no-comment-0.1.1/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    99653 2023-07-12 08:47:42.806192 no-comment-0.1.1/no_comment/infrastructure/flask/static/js/hyperscript@0.9.9.min.js
+-rw-r--r--   0        0        0     3512 2023-07-12 08:47:42.806192 no-comment-0.1.1/no_comment/infrastructure/flask/streams.py
+-rw-r--r--   0        0        0     1900 2023-07-12 10:01:38.989842 no-comment-0.1.1/no_comment/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-12 08:47:42.806192 no-comment-0.1.1/no_comment/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     2374 2023-07-12 08:47:42.806192 no-comment-0.1.1/no_comment/infrastructure/settings.py
+-rw-r--r--   0        0        0      736 2023-07-12 08:47:42.806192 no-comment-0.1.1/no_comment/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4621 2023-07-12 08:47:42.810192 no-comment-0.1.1/no_comment/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2154 2023-07-12 08:47:42.810192 no-comment-0.1.1/no_comment/interfaces/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-12 08:47:42.810192 no-comment-0.1.1/no_comment/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0     7432 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1348 2023-07-12 09:21:08.856637 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     1878 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1177 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
+-rw-r--r--   0        0        0      860 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug
+-rw-r--r--   0        0        0     5333 2023-07-12 10:06:26.438248 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/display.pug
+-rw-r--r--   0        0        0      980 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/root.pug
+-rw-r--r--   0        0        0      967 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug
+-rw-r--r--   0        0        0     1787 2023-07-12 09:21:18.560513 no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     3578 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_json.py
+-rw-r--r--   0        0        0     6006 2023-07-12 08:47:42.814192 no-comment-0.1.1/no_comment/interfaces/to_http/as_xml.py
+-rw-r--r--   0        0        0      869 2023-07-12 08:47:42.818192 no-comment-0.1.1/no_comment/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-12 08:47:42.818192 no-comment-0.1.1/no_comment/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1810 2023-07-12 08:47:42.818192 no-comment-0.1.1/no_comment/test_factories.py
+-rw-r--r--   0        0        0     1230 2023-07-12 10:23:51.945222 no-comment-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3934 2023-07-12 10:24:42.071826 no-comment-0.1.1/setup.py
+-rw-r--r--   0        0        0     2708 2023-07-12 10:24:42.072924 no-comment-0.1.1/PKG-INFO
```

### Comparing `no-comment-0.1.0a9/LICENSE` & `no-comment-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/README.md` & `no-comment-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/__init__.py` & `no-comment-0.1.1/no_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/application/__init__.py` & `no-comment-0.1.1/no_comment/application/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/application/use_cases/__init__.py` & `no-comment-0.1.1/no_comment/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/application/use_cases/add_comment.py` & `no-comment-0.1.1/no_comment/application/use_cases/add_comment.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/application/use_cases/create_stream.py` & `no-comment-0.1.1/no_comment/application/use_cases/create_stream.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/application/use_cases/display_stream.py` & `no-comment-0.1.1/no_comment/application/use_cases/display_stream.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/configuration/__init__.py` & `no-comment-0.1.1/no_comment/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/configuration/cli.py` & `no-comment-0.1.1/no_comment/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/configuration/wsgi.py` & `no-comment-0.1.1/no_comment/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/__init__.py` & `no-comment-0.1.1/no_comment/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/__init__.py` & `no-comment-0.1.1/no_comment/domain/commenting/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/entities.py` & `no-comment-0.1.1/no_comment/domain/commenting/entities.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/exceptions.py` & `no-comment-0.1.1/no_comment/domain/commenting/exceptions.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/repositories.py` & `no-comment-0.1.1/no_comment/domain/commenting/repositories.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/services.py` & `no-comment-0.1.1/no_comment/domain/commenting/services.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/domain/commenting/value_objects.py` & `no-comment-0.1.1/no_comment/domain/commenting/value_objects.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/click/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/click/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/click/services.py` & `no-comment-0.1.1/no_comment/infrastructure/click/services.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/auth/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/ip/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Hector --- A collection manager.
+# No Comment --- Comment any resource on the web!
 # Copyright © 2023 Bioneland
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -12,38 +12,33 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any
 
-from flask import Blueprint, current_app, session, url_for
+from flask import Blueprint, flash, request, session, url_for
 
 from no_comment.infrastructure.flask import services
 from no_comment.infrastructure.flask.utils import presenter_to_response
-from no_comment.interfaces.to_http import Redirection, as_html
+from no_comment.interfaces.to_http import Redirection
 
-blueprint = Blueprint("auth", __name__)
-
-
-@blueprint.get("")
-@presenter_to_response
-def root() -> Any:
-    return Redirection(url_for("streams.root"))
+blueprint = Blueprint("ip", __name__)
 
 
 @blueprint.get("/login")
 @presenter_to_response
 def login() -> Any:
-    auth_links = current_app.auth_links  # type: ignore[attr-defined]
-    if not auth_links:
-        return Redirection(url_for("streams.root"))
-    if len(auth_links) == 1:
-        return Redirection(url_for(auth_links[0]["route"]))
-    return as_html.PugPresenter("auth/login", links=auth_links, user=services.get_user())
+    if not authorized():
+        flash("Error authenticating with IP.", "error")
+        return Redirection(url_for("auth.login"))
 
+    session["user_id"] = "anonymous"
 
-@blueprint.get("/logout")
-@presenter_to_response
-def logout() -> Any:
-    session.clear()
-    return Redirection(url_for("streams.root"))
+    flash("Success authenticating with IP.", "success")
+    return Redirection(url_for("auth.redirect"))
+
+
+def authorized() -> bool:
+    authorized_ip = services.get_settings().AUTHORIZED_IP
+    client_ip = request.headers.get("X-Remote-IP", request.remote_addr) or ""
+    return client_ip.startswith(authorized_ip.rstrip("*"))
```

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/services.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `no-comment-0.1.1/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/favicon.svg` & `no-comment-0.1.1/no_comment/infrastructure/flask/static/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/feed.svg` & `no-comment-0.1.1/no_comment/infrastructure/flask/static/img/feed.svg`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `no-comment-0.1.1/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `no-comment-0.1.1/no_comment/infrastructure/flask/static/js/hyperscript@0.9.9.min.js`

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

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/streams.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/streams.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/totp/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/totp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Hector --- A collection manager.
+# No Comment --- Comment any resource on the web!
 # Copyright © 2023 Bioneland
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -44,14 +44,8 @@
     if not totp.verify(request.form.get("password", "")):
         flash("Error authenticating with TOTP.", "error")
         return Redirection(url_for("totp.login"))
 
     session["user_id"] = "anonymous"
 
     flash("Success authenticating with TOTP.", "success")
-    return Redirection(url_for("streams.root"))
-
-
-@blueprint.get("/logout")
-@presenter_to_response
-def logout() -> Any:
-    return Redirection(url_for("auth.logout"))
+    return Redirection(url_for("auth.redirect"))
```

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/flask/utils.py` & `no-comment-0.1.1/no_comment/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/settings.py` & `no-comment-0.1.1/no_comment/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/__init__.py` & `no-comment-0.1.1/no_comment/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/repositories.py` & `no-comment-0.1.1/no_comment/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/__init__.py` & `no-comment-0.1.1/no_comment/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/__init__.py` & `no-comment-0.1.1/no_comment/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/__init__.py` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/auth/login.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-//- Hector --- A collection manager.
+//- No Comment --- Comment any resource on the web!
 //- Copyright © 2023 Bioneland
 //-
 //- This program is free software: you can redistribute it and/or modify
 //- it under the terms of the GNU Affero General Public License as
 //- published by the Free Software Foundation, either version 3 of the
 //- License, or (at your option) any later version.
 //-
```

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/layout.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     link(rel="icon" type="image/svg" href=url_for("static", filename="img/favicon.svg"))
     link(rel="stylesheet" href=url_for("static", filename="css/bulma@0.9.4.min.css"))
     link(rel="stylesheet" href=url_for("static", filename="css/no-comment.css"))
     block links
 
     script(src=url_for("static", filename="js/htmx@1.9.2.min.js") defer)
-    script(src=url_for("static", filename="js/hyperscript@0.9.8.min.js") defer)
+    script(src=url_for("static", filename="js/hyperscript@0.9.9.min.js") defer)
     block head_scripts
   body
     .page
       - var messages = get_flashed_messages(with_categories=true)
       +flash_messages(messages)
 
       block content
```

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 mixin flash_messages(messages)
   - var alert_classes = {"success": "is-success", "error": "is-danger", "info": "is-info", "warning": "is-warning"}
   if messages
     .container
       .notifications
         each category, message in messages
           p.notification.is-light(class=alert_classes[category])
-            button.delete
+            button.delete(_="on click remove the closest .notification")
             | #{message}
```

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/display.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/display.pug`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/root.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/root.pug`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/totp/login.pug` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-//- Hector --- A collection manager.
+//- No Comment --- Comment any resource on the web!
 //- Copyright © 2023 Bioneland
 //-
 //- This program is free software: you can redistribute it and/or modify
 //- it under the terms of the GNU Affero General Public License as
 //- published by the Free Software Foundation, either version 3 of the
 //- License, or (at your option) any later version.
 //-
```

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_json.py` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_json.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_xml.py` & `no-comment-0.1.1/no_comment/interfaces/to_http/as_xml.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_terminal/__init__.py` & `no-comment-0.1.1/no_comment/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/interfaces/to_terminal/as_text.py` & `no-comment-0.1.1/no_comment/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/no_comment/test_factories.py` & `no-comment-0.1.1/no_comment/test_factories.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a9/pyproject.toml` & `no-comment-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "no-comment"
-version = "0.1.0-alpha.9"
+version = "0.1.1"
 description = "Comment any resource on the web!"
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
```

### Comparing `no-comment-0.1.0a9/setup.py` & `no-comment-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['no-comment = no_comment.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'no-comment',
-    'version': '0.1.0a9',
+    'version': '0.1.1',
     'description': 'Comment any resource on the web!',
     'long_description': '# NoComment\n\nComment any resource on the web!\n\n\n## Install\n\nNoComment is available on PyPI under the name `no-comment`.\nTo install, just run `python -m pip install no-comment`.\n\n\n## Configure\n\nNoComment is configured using environment variables.\nSee [the `settings` module](no_comment/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `NO_COMMENT_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export NO_COMMENT_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export NO_COMMENT_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`no-comment[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export NO_COMMENT_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise NoComment\'s database with the dedicated command:\n\n```console\n$ no-comment init-db\n```\n\n\n## Run\n\nNoComment being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "no_comment.configuration.wsgi:app()"\n```\n\nYou can now access the service at <http://127.0.0.1:3000/MY_STREAM_NAME>.\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `no-comment-0.1.0a9/PKG-INFO` & `no-comment-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-comment
-Version: 0.1.0a9
+Version: 0.1.1
 Summary: Comment any resource on the web!
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

