# Comparing `tmp/11x_wagtail_blog-0.0.0.tar.gz` & `tmp/11x_wagtail_blog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "11x_wagtail_blog-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "11x_wagtail_blog-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `11x_wagtail_blog-0.0.0.tar` & `11x_wagtail_blog-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,30 @@
--rw-r--r--   0        0        0      242 2023-07-03 17:25:55.411469 11x_wagtail_blog-0.0.0/.gitignore
--rw-r--r--   0        0        0       22 2023-07-03 17:39:21.047490 11x_wagtail_blog-0.0.0/.python-version
--rw-r--r--   0        0        0     1087 2023-07-03 16:57:20.371425 11x_wagtail_blog-0.0.0/LICENSE
--rw-r--r--   0        0        0      104 2023-07-03 19:43:21.079682 11x_wagtail_blog-0.0.0/README.rst
--rw-r--r--   0        0        0      634 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.0.0/docs/Makefile
--rw-r--r--   0        0        0     1788 2023-07-03 18:19:38.219552 11x_wagtail_blog-0.0.0/docs/conf.py
--rw-r--r--   0        0        0      498 2023-07-03 18:22:21.651556 11x_wagtail_blog-0.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.0.0/docs/make.bat
--rw-r--r--   0        0        0     1527 2023-07-03 21:00:24.088901 11x_wagtail_blog-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      672 2023-07-03 19:25:36.803654 11x_wagtail_blog-0.0.0/tox.ini
--rw-r--r--   0        0        0       38 2023-07-03 18:41:23.339586 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/__init__.py
--rw-r--r--   0        0        0      164 2023-07-03 18:43:43.887589 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/apps.py
--rw-r--r--   0        0        0        0 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/models.py
--rw-r--r--   0        0        0      116 2023-07-03 21:06:42.156911 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/tests.py
--rw-r--r--   0        0        0       63 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.0.0/x11x_wagtail_blog/views.py
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 11x_wagtail_blog-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-07-03 17:25:55.411469 11x_wagtail_blog-0.1.0/.gitignore
+-rw-r--r--   0        0        0       22 2023-07-03 17:39:21.047490 11x_wagtail_blog-0.1.0/.python-version
+-rw-r--r--   0        0        0     1087 2023-07-03 16:57:20.371425 11x_wagtail_blog-0.1.0/LICENSE
+-rw-r--r--   0        0        0      186 2023-07-12 20:26:51.147945 11x_wagtail_blog-0.1.0/README.rst
+-rw-r--r--   0        0        0      634 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1788 2023-07-03 18:19:38.219552 11x_wagtail_blog-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      498 2023-07-03 18:22:21.651556 11x_wagtail_blog-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1608 2023-07-12 20:25:36.959943 11x_wagtail_blog-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-04 16:31:02.906578 11x_wagtail_blog-0.1.0/tox.ini
+-rw-r--r--   0        0        0       38 2023-07-12 20:24:13.887941 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-03 18:43:43.887589 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/apps.py
+-rw-r--r--   0        0        0     1153 2023-07-11 00:03:16.100737 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/fakers.py
+-rw-r--r--   0        0        0     3962 2023-07-11 00:07:25.992743 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:20:08.564577 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/migrations/__init__.py
+-rw-r--r--   0        0        0     3237 2023-07-12 15:33:06.386469 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/models.py
+-rw-r--r--   0        0        0      229 2023-07-04 18:49:03.415909 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/about_the_author.html
+-rw-r--r--   0        0        0      659 2023-07-04 17:26:31.071781 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/tests/testing_models/testing_article_page.html
+-rw-r--r--   0        0        0        0 2023-07-04 17:12:17.795760 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templatetags/__init__.py
+-rw-r--r--   0        0        0      612 2023-07-04 18:08:01.615846 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templatetags/x11x_wagtail_blog.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:48:47.780714 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/__init__.py
+-rw-r--r--   0        0        0     5239 2023-07-12 15:37:19.206475 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/test_extensible_article_page.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:48:45.748714 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-10 23:53:51.440722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/apps.py
+-rw-r--r--   0        0        0      565 2023-07-10 23:50:54.984717 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/fakers.py
+-rw-r--r--   0        0        0     1155 2023-07-10 23:54:08.428722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:54:08.320722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/migrations/__init__.py
+-rw-r--r--   0        0        0      270 2023-07-11 00:01:20.236734 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/models.py
+-rw-r--r--   0        0        0       63 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/views.py
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 11x_wagtail_blog-0.1.0/PKG-INFO
```

### Comparing `11x_wagtail_blog-0.0.0/LICENSE` & `11x_wagtail_blog-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.0.0/docs/Makefile` & `11x_wagtail_blog-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.0.0/docs/conf.py` & `11x_wagtail_blog-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.0.0/docs/make.bat` & `11x_wagtail_blog-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.0.0/pyproject.toml` & `11x_wagtail_blog-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [project]
 name = "11x-wagtail-blog"
 authors = [
     { name = "The Magnificant Nick", email = "it@11x.engineering" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
+    "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -28,36 +29,37 @@
 readme = { file = "README.rst", content-type = "text/x-rst" }
 keywords = [
     "wagtail",
     "blog",
 ]
 dynamic = [ "version", "description" ]
 dependencies = [
-    "wagtail >=4.0,<6"
+    "wagtail >=4.0,<6",
 ]
 
 
 [project.optional-dependencies]
 doc = [
     "sphinx",
     "sphinx-rtd-theme",
 ]
 
 test = [
     "black",
     "tox >=4.6.3",
+    "faker >=18.11.2",
 ]
 
 github = [
     "tox-gh-actions >=3.0",
 ]
 
 
 [project.urls]
-Home = "https://www.11x.engineering/blog/"
+Home = "https://github.com/11x-engineering/11x-wagtail-blog"
 Documentation = "https://11x-wagtail-blog.readthedocs.io/en/latest/"
 Source = "https://github.com/11x-engineering/11x-wagtail-blog"
 
 
 [tool.black]
 line-length = 120
```

### Comparing `11x_wagtail_blog-0.0.0/tox.ini` & `11x_wagtail_blog-0.1.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tox]
 # Ensuring that the wagtail app will work on python versions 3.7-3.11 and on wagtail 4 and 5.
 envlist =
-  py{37,38,39,310,311}-wagtail{4,5}
+  py{38,39,310,311}-wagtail{4,5}
+  py37-wagtail4
 
 basepython =
   py37: python3.7
   py38: python3.8
   py39: python3.9
   py310: python3.10
   py311: python3.11
@@ -26,11 +27,12 @@
 
 [testenv]
 setenv =
   DJANGO_SETTINGS_MODULE = conf.settings.tests
   PYTHONPATH = {toxinidir}
 
 commands = python testapp/manage.py test x11x_wagtail_blog
+extras = test
 
 deps =
   py3{7,8,9,10,11}-wagtail4: wagtail >=4.0,<5
-  py3{7,8,9,10,11}-wagtail5: wagtail >=5.0,<6
+  py3{8,9,10,11}-wagtail5: wagtail >=5.0,<6
```

### Comparing `11x_wagtail_blog-0.0.0/PKG-INFO` & `11x_wagtail_blog-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: 11x-wagtail-blog
-Version: 0.0.0
+Version: 0.1.0
 Summary: Docstring
 Keywords: wagtail,blog
 Author-email: The Magnificant Nick <it@11x.engineering>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,19 +21,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: wagtail >=4.0,<6
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Requires-Dist: tox-gh-actions >=3.0 ; extra == "github"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: tox >=4.6.3 ; extra == "test"
+Requires-Dist: faker >=18.11.2 ; extra == "test"
 Project-URL: Documentation, https://11x-wagtail-blog.readthedocs.io/en/latest/
-Project-URL: Home, https://www.11x.engineering/blog/
+Project-URL: Home, https://github.com/11x-engineering/11x-wagtail-blog
 Project-URL: Source, https://github.com/11x-engineering/11x-wagtail-blog
 Provides-Extra: doc
 Provides-Extra: github
 Provides-Extra: test
 
 11x Wagtail Blog
 ================
 
 An blog feature for 11x.Engineering featured as its first blog post.
 
+Set development status to Alpha. Status bump up to Beta when docs are published.
+
```

