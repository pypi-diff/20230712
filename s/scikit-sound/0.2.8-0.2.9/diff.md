# Comparing `tmp/scikit-sound-0.2.8.tar.gz` & `tmp/scikit-sound-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-sound-0.2.8.tar", last modified: Fri Apr  2 17:05:34 2021, max compression
+gzip compressed data, was "scikit-sound-0.2.9.tar", last modified: Fri Apr  2 18:50:29 2021, max compression
```

## Comparing `scikit-sound-0.2.8.tar` & `scikit-sound-0.2.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.329428 scikit-sound-0.2.8/
--rw-rw-rw-   0        0        0     1118 2021-04-02 17:05:02.000000 scikit-sound-0.2.8/CHANGES.txt
--rw-rw-rw-   0        0        0     1483 2017-02-19 16:49:52.000000 scikit-sound-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2017-02-20 10:41:28.000000 scikit-sound-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2182 2021-04-02 17:05:34.328428 scikit-sound-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2021-04-02 17:05:10.000000 scikit-sound-0.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.218402 scikit-sound-0.2.8/docs/
--rw-rw-rw-   0        0        0      213 2017-02-18 21:19:40.000000 scikit-sound-0.2.8/docs/FAQ.txt
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.201399 scikit-sound-0.2.8/docs/_build/
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.222404 scikit-sound-0.2.8/docs/_build/doctrees/
--rw-rw-rw-   0        0        0    46859 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/doctrees/environment.pickle
--rw-rw-rw-   0        0        0    21779 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/doctrees/index.doctree
--rw-rw-rw-   0        0        0    39420 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/doctrees/misc.doctree
--rw-rw-rw-   0        0        0    65278 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/doctrees/sounds.doctree
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.234407 scikit-sound-0.2.8/docs/_build/html/
--rw-rw-rw-   0        0        0      234 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/.buildinfo
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.237407 scikit-sound-0.2.8/docs/_build/html/_modules/
--rw-rw-rw-   0        0        0     3465 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_modules/index.html
--rw-rw-rw-   0        0        0    25452 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_modules/misc.html
--rw-rw-rw-   0        0        0    68274 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_modules/sounds.html
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.244409 scikit-sound-0.2.8/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     2817 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0      572 2018-03-23 20:07:54.000000 scikit-sound-0.2.8/docs/_build/html/_sources/misc.rst.txt
--rw-rw-rw-   0        0        0      634 2017-02-19 16:08:05.000000 scikit-sound-0.2.8/docs/_build/html/_sources/sounds.rst.txt
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.281417 scikit-sound-0.2.8/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      673 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/ajax-loader.gif
--rw-rw-rw-   0        0        0    14502 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/basic.css
--rw-rw-rw-   0        0        0     4816 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/classic.css
--rw-rw-rw-   0        0        0      756 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/comment-bright.png
--rw-rw-rw-   0        0        0      829 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/comment-close.png
--rw-rw-rw-   0        0        0      641 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/comment.png
--rw-rw-rw-   0        0        0     9913 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/doctools.js
--rw-rw-rw-   0        0        0      366 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      222 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/down-pressed.png
--rw-rw-rw-   0        0        0      202 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/down.png
--rw-rw-rw-   0        0        0      286 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0   273841 2021-03-28 12:58:13.000000 scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.1.0.js
--rw-rw-rw-   0        0        0   278292 2021-03-28 12:58:13.000000 scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0   298502 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89478 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/jquery.js
--rw-rw-rw-   0        0        0    11151 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0     4919 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/pygments.css
--rw-rw-rw-   0        0        0    17104 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/searchtools.js
--rw-rw-rw-   0        0        0     4961 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/sidebar.js
--rw-rw-rw-   0        0        0    13566 2017-02-18 17:50:43.000000 scikit-sound-0.2.8/docs/_build/html/_static/sksound.ico
--rw-rw-rw-   0        0        0    21455 2017-02-19 14:24:35.000000 scikit-sound-0.2.8/docs/_build/html/_static/sksound.png
--rw-rw-rw-   0        0        0    69719 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/underscore-1.12.0.js
--rw-rw-rw-   0        0        0    36167 2021-03-28 12:58:13.000000 scikit-sound-0.2.8/docs/_build/html/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    19363 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/_static/underscore.js
--rw-rw-rw-   0        0        0      214 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/up-pressed.png
--rw-rw-rw-   0        0        0      203 2017-01-28 15:45:18.000000 scikit-sound-0.2.8/docs/_build/html/_static/up.png
--rw-rw-rw-   0        0        0    26163 2021-03-28 12:58:13.000000 scikit-sound-0.2.8/docs/_build/html/_static/websupport.js
--rw-rw-rw-   0        0        0     7300 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/genindex.html
--rw-rw-rw-   0        0        0    13217 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/index.html
--rw-rw-rw-   0        0        0    18519 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/misc.html
--rw-rw-rw-   0        0        0      485 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/objects.inv
--rw-rw-rw-   0        0        0     4178 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/py-modindex.html
--rw-rw-rw-   0        0        0     3611 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/search.html
--rw-rw-rw-   0        0        0     4557 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/searchindex.js
--rw-rw-rw-   0        0        0    29705 2021-03-28 12:58:14.000000 scikit-sound-0.2.8/docs/_build/html/sounds.html
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.283417 scikit-sound-0.2.8/docs/_static/
--rw-rw-rw-   0        0        0    13566 2017-02-18 17:50:43.000000 scikit-sound-0.2.8/docs/_static/sksound.ico
--rw-rw-rw-   0        0        0    21455 2017-02-19 14:24:35.000000 scikit-sound-0.2.8/docs/_static/sksound.png
--rw-rw-rw-   0        0        0     8878 2021-04-02 17:05:22.000000 scikit-sound-0.2.8/docs/conf.py
--rw-rw-rw-   0        0        0     2817 2021-04-02 17:05:26.000000 scikit-sound-0.2.8/docs/index.rst
--rwxrwxrwx   0        0        0     6711 2016-04-10 20:17:54.000000 scikit-sound-0.2.8/docs/make.bat
--rw-rw-rw-   0        0        0      572 2018-03-23 20:07:54.000000 scikit-sound-0.2.8/docs/misc.rst
--rw-rw-rw-   0        0        0      634 2017-02-19 16:08:05.000000 scikit-sound-0.2.8/docs/sounds.rst
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.307423 scikit-sound-0.2.8/scikit_sound.egg-info/
--rw-rw-rw-   0        0        0     2182 2021-04-02 17:05:34.000000 scikit-sound-0.2.8/scikit_sound.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2462 2021-04-02 17:05:34.000000 scikit-sound-0.2.8/scikit_sound.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-02 17:05:34.000000 scikit-sound-0.2.8/scikit_sound.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2021-04-02 17:05:34.000000 scikit-sound-0.2.8/scikit_sound.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-04-02 17:05:34.000000 scikit-sound-0.2.8/scikit_sound.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-04-02 17:05:34.329428 scikit-sound-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2888 2021-04-02 17:05:16.000000 scikit-sound-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.310423 scikit-sound-0.2.8/sksound/
--rw-rw-rw-   0        0        0      557 2021-04-02 17:05:29.000000 scikit-sound-0.2.8/sksound/__init__.py
--rw-rw-rw-   0        0        0     6264 2021-04-02 14:53:45.000000 scikit-sound-0.2.8/sksound/misc.py
--rw-rw-rw-   0        0        0    18973 2021-04-02 15:10:25.000000 scikit-sound-0.2.8/sksound/sounds.py
-drwxrwxrwx   0        0        0        0 2021-04-02 17:05:34.327428 scikit-sound-0.2.8/sksound/tests/
--rw-rw-rw-   0        0        0   125805 2011-03-12 18:11:58.000000 scikit-sound-0.2.8/sksound/tests/YouAreNotIt.mp3
--rw-rw-rw-   0        0        0  1387086 2021-04-02 13:04:11.000000 scikit-sound-0.2.8/sksound/tests/YouAreNotIt.wav
--rw-rw-rw-   0        0        0       70 2015-11-18 21:10:18.000000 scikit-sound-0.2.8/sksound/tests/__init__.py
--rw-rw-rw-   0        0        0    54186 2007-10-29 15:29:06.000000 scikit-sound-0.2.8/sksound/tests/a1.wav
--rw-rw-rw-   0        0        0  1843258 2017-04-12 17:03:10.000000 scikit-sound-0.2.8/sksound/tests/float_sound.wav
--rw-rw-rw-   0        0        0   266422 2004-04-16 05:37:22.000000 scikit-sound-0.2.8/sksound/tests/peas.wav
--rw-rw-rw-   0        0        0      431 2018-03-23 19:29:17.000000 scikit-sound-0.2.8/sksound/tests/test_sksound.py
--rw-rw-rw-   0        0        0     2383 2019-04-07 15:32:53.000000 scikit-sound-0.2.8/sksound/tests/test_sound.py
--rw-rw-rw-   0        0        0   921686 2011-03-12 18:21:24.000000 scikit-sound-0.2.8/sksound/tests/tiger.wav
--rw-rw-rw-   0        0        0    22094 2017-02-19 17:40:43.000000 scikit-sound-0.2.8/sksound/tests/tmp.wav
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.603791 scikit-sound-0.2.9/
+-rw-rw-rw-   0        0        0     1154 2021-04-02 18:47:56.000000 scikit-sound-0.2.9/CHANGES.txt
+-rw-rw-rw-   0        0        0     1483 2017-02-19 16:49:52.000000 scikit-sound-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2017-02-20 10:41:28.000000 scikit-sound-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2182 2021-04-02 18:50:29.603791 scikit-sound-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2021-04-02 18:48:00.000000 scikit-sound-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.503768 scikit-sound-0.2.9/docs/
+-rw-rw-rw-   0        0        0      213 2017-02-18 21:19:40.000000 scikit-sound-0.2.9/docs/FAQ.txt
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.486765 scikit-sound-0.2.9/docs/_build/
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.507768 scikit-sound-0.2.9/docs/_build/doctrees/
+-rw-rw-rw-   0        0        0    46859 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0    21779 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0    39420 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/doctrees/misc.doctree
+-rw-rw-rw-   0        0        0    65278 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/doctrees/sounds.doctree
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.519771 scikit-sound-0.2.9/docs/_build/html/
+-rw-rw-rw-   0        0        0      234 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/.buildinfo
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.523772 scikit-sound-0.2.9/docs/_build/html/_modules/
+-rw-rw-rw-   0        0        0     3465 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_modules/index.html
+-rw-rw-rw-   0        0        0    25452 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_modules/misc.html
+-rw-rw-rw-   0        0        0    68274 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_modules/sounds.html
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.525773 scikit-sound-0.2.9/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     2817 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0      572 2018-03-23 20:07:54.000000 scikit-sound-0.2.9/docs/_build/html/_sources/misc.rst.txt
+-rw-rw-rw-   0        0        0      634 2017-02-19 16:08:05.000000 scikit-sound-0.2.9/docs/_build/html/_sources/sounds.rst.txt
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.562782 scikit-sound-0.2.9/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      673 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/ajax-loader.gif
+-rw-rw-rw-   0        0        0    14502 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/basic.css
+-rw-rw-rw-   0        0        0     4816 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/classic.css
+-rw-rw-rw-   0        0        0      756 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/comment-bright.png
+-rw-rw-rw-   0        0        0      829 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/comment-close.png
+-rw-rw-rw-   0        0        0      641 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/comment.png
+-rw-rw-rw-   0        0        0     9913 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      366 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      222 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/down-pressed.png
+-rw-rw-rw-   0        0        0      202 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/down.png
+-rw-rw-rw-   0        0        0      286 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0   273841 2021-03-28 12:58:13.000000 scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.1.0.js
+-rw-rw-rw-   0        0        0   278292 2021-03-28 12:58:13.000000 scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0   298502 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89478 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/jquery.js
+-rw-rw-rw-   0        0        0    11151 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4919 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    17104 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0     4961 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/sidebar.js
+-rw-rw-rw-   0        0        0    13566 2017-02-18 17:50:43.000000 scikit-sound-0.2.9/docs/_build/html/_static/sksound.ico
+-rw-rw-rw-   0        0        0    21455 2017-02-19 14:24:35.000000 scikit-sound-0.2.9/docs/_build/html/_static/sksound.png
+-rw-rw-rw-   0        0        0    69719 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/underscore-1.12.0.js
+-rw-rw-rw-   0        0        0    36167 2021-03-28 12:58:13.000000 scikit-sound-0.2.9/docs/_build/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    19363 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0      214 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/up-pressed.png
+-rw-rw-rw-   0        0        0      203 2017-01-28 15:45:18.000000 scikit-sound-0.2.9/docs/_build/html/_static/up.png
+-rw-rw-rw-   0        0        0    26163 2021-03-28 12:58:13.000000 scikit-sound-0.2.9/docs/_build/html/_static/websupport.js
+-rw-rw-rw-   0        0        0     7300 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/genindex.html
+-rw-rw-rw-   0        0        0    13217 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/index.html
+-rw-rw-rw-   0        0        0    18519 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/misc.html
+-rw-rw-rw-   0        0        0      485 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/objects.inv
+-rw-rw-rw-   0        0        0     4178 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/py-modindex.html
+-rw-rw-rw-   0        0        0     3611 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/search.html
+-rw-rw-rw-   0        0        0     4557 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/searchindex.js
+-rw-rw-rw-   0        0        0    29705 2021-03-28 12:58:14.000000 scikit-sound-0.2.9/docs/_build/html/sounds.html
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.564782 scikit-sound-0.2.9/docs/_static/
+-rw-rw-rw-   0        0        0    13566 2017-02-18 17:50:43.000000 scikit-sound-0.2.9/docs/_static/sksound.ico
+-rw-rw-rw-   0        0        0    21455 2017-02-19 14:24:35.000000 scikit-sound-0.2.9/docs/_static/sksound.png
+-rw-rw-rw-   0        0        0     8878 2021-04-02 18:50:15.000000 scikit-sound-0.2.9/docs/conf.py
+-rw-rw-rw-   0        0        0     2817 2021-04-02 18:48:34.000000 scikit-sound-0.2.9/docs/index.rst
+-rwxrwxrwx   0        0        0     6711 2016-04-10 20:17:54.000000 scikit-sound-0.2.9/docs/make.bat
+-rw-rw-rw-   0        0        0      572 2018-03-23 20:07:54.000000 scikit-sound-0.2.9/docs/misc.rst
+-rw-rw-rw-   0        0        0      634 2017-02-19 16:08:05.000000 scikit-sound-0.2.9/docs/sounds.rst
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.584786 scikit-sound-0.2.9/scikit_sound.egg-info/
+-rw-rw-rw-   0        0        0     2182 2021-04-02 18:50:29.000000 scikit-sound-0.2.9/scikit_sound.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2462 2021-04-02 18:50:29.000000 scikit-sound-0.2.9/scikit_sound.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-02 18:50:29.000000 scikit-sound-0.2.9/scikit_sound.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2021-04-02 18:50:29.000000 scikit-sound-0.2.9/scikit_sound.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-04-02 18:50:29.000000 scikit-sound-0.2.9/scikit_sound.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-04-02 18:50:29.603791 scikit-sound-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2888 2021-04-02 18:49:47.000000 scikit-sound-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.586787 scikit-sound-0.2.9/sksound/
+-rw-rw-rw-   0        0        0      557 2021-04-02 18:48:38.000000 scikit-sound-0.2.9/sksound/__init__.py
+-rw-rw-rw-   0        0        0     6515 2021-04-02 18:46:24.000000 scikit-sound-0.2.9/sksound/misc.py
+-rw-rw-rw-   0        0        0    18965 2021-04-02 18:44:09.000000 scikit-sound-0.2.9/sksound/sounds.py
+drwxrwxrwx   0        0        0        0 2021-04-02 18:50:29.602791 scikit-sound-0.2.9/sksound/tests/
+-rw-rw-rw-   0        0        0   125805 2011-03-12 18:11:58.000000 scikit-sound-0.2.9/sksound/tests/YouAreNotIt.mp3
+-rw-rw-rw-   0        0        0  1387086 2021-04-02 13:04:11.000000 scikit-sound-0.2.9/sksound/tests/YouAreNotIt.wav
+-rw-rw-rw-   0        0        0       70 2015-11-18 21:10:18.000000 scikit-sound-0.2.9/sksound/tests/__init__.py
+-rw-rw-rw-   0        0        0    54186 2007-10-29 15:29:06.000000 scikit-sound-0.2.9/sksound/tests/a1.wav
+-rw-rw-rw-   0        0        0  1843258 2017-04-12 17:03:10.000000 scikit-sound-0.2.9/sksound/tests/float_sound.wav
+-rw-rw-rw-   0        0        0   266422 2004-04-16 05:37:22.000000 scikit-sound-0.2.9/sksound/tests/peas.wav
+-rw-rw-rw-   0        0        0      431 2018-03-23 19:29:17.000000 scikit-sound-0.2.9/sksound/tests/test_sksound.py
+-rw-rw-rw-   0        0        0     2383 2019-04-07 15:32:53.000000 scikit-sound-0.2.9/sksound/tests/test_sound.py
+-rw-rw-rw-   0        0        0   921686 2011-03-12 18:21:24.000000 scikit-sound-0.2.9/sksound/tests/tiger.wav
+-rw-rw-rw-   0        0        0    22094 2017-02-19 17:40:43.000000 scikit-sound-0.2.9/sksound/tests/tmp.wav
```

### Comparing `scikit-sound-0.2.8/CHANGES.txt` & `scikit-sound-0.2.9/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 v0.2.2, 11-Mar-2019 -- Update the documentation
 v0.2.3, 28-March-2019 -- problem with Sound.write() when used without input fixed
 v0.2.3b, 05-April-2019 -- Documentation updated
 v0.2.4, 13-April-2019 -- Try to keep file-/dir-selection windows in the front
 v0.2.5, 13-April-2019 -- Exit gracefully if user cancels file selection
 v0.2.6, 28-March-2021 -- updated docu; renamed self.info -> self.ffmpeg_info
 v0.2.7, 02-April-2021 -- left tkinter root window visible to avoid some crashes
-v0.2.8, 02-April-2021 -- same problem as before: now I move the box to the top
+v0.2.8, 02-April-2021 -- [erroneous fix]
+v0.2.9, 02-April-2021 -- moved the tkinter root to the top to be visible
```

### Comparing `scikit-sound-0.2.8/LICENSE.txt` & `scikit-sound-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/PKG-INFO` & `scikit-sound-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-sound
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python utilites for working with sound signals
 Home-page: http://work.thaslwanter.at/sksound/html
 Author: Thomas Haslwanter
 Author-email: thomas.haslwanter@fh-linz.at
 License: http://opensource.org/licenses/BSD-2-Clause
 Download-URL: https://github.com/thomas-haslwanter/scikit-sound
 Description: ============
@@ -19,15 +19,15 @@
         
         Homepage
         --------
         http://work.thaslwanter.at/sksound/html/
         
         :Author:  Thomas Haslwanter
         :Date:    02-04-2021
-        :Ver:     0.2.8
+        :Ver:     0.2.9
         :Licence: BSD 2-Clause License (http://opensource.org/licenses/BSD-2-Clause)
         :Copyright:
             |copy| 2021, Thomas Haslwanter, all rights reserved.
         
         .. |copy|   unicode:: U+000A9 .. COPYRIGHT SIGN
         
         Installation
```

### Comparing `scikit-sound-0.2.8/README.rst` & `scikit-sound-0.2.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Homepage
 --------
 http://work.thaslwanter.at/sksound/html/
 
 :Author:  Thomas Haslwanter
 :Date:    02-04-2021
-:Ver:     0.2.8
+:Ver:     0.2.9
 :Licence: BSD 2-Clause License (http://opensource.org/licenses/BSD-2-Clause)
 :Copyright:
     |copy| 2021, Thomas Haslwanter, all rights reserved.
 
 .. |copy|   unicode:: U+000A9 .. COPYRIGHT SIGN
 
 Installation
```

### Comparing `scikit-sound-0.2.8/docs/_build/doctrees/environment.pickle` & `scikit-sound-0.2.9/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/doctrees/index.doctree` & `scikit-sound-0.2.9/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/doctrees/misc.doctree` & `scikit-sound-0.2.9/docs/_build/doctrees/misc.doctree`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/doctrees/sounds.doctree` & `scikit-sound-0.2.9/docs/_build/doctrees/sounds.doctree`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_modules/index.html` & `scikit-sound-0.2.9/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_modules/misc.html` & `scikit-sound-0.2.9/docs/_build/html/_modules/misc.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_modules/sounds.html` & `scikit-sound-0.2.9/docs/_build/html/_modules/sounds.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_sources/index.rst.txt` & `scikit-sound-0.2.9/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_sources/misc.rst.txt` & `scikit-sound-0.2.9/docs/_build/html/_sources/misc.rst.txt`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_sources/sounds.rst.txt` & `scikit-sound-0.2.9/docs/_build/html/_sources/sounds.rst.txt`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/ajax-loader.gif` & `scikit-sound-0.2.9/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/basic.css` & `scikit-sound-0.2.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/classic.css` & `scikit-sound-0.2.9/docs/_build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/comment-bright.png` & `scikit-sound-0.2.9/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/comment-close.png` & `scikit-sound-0.2.9/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/comment.png` & `scikit-sound-0.2.9/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/doctools.js` & `scikit-sound-0.2.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.1.0.js` & `scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.2.1.js` & `scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/jquery-3.5.1.js` & `scikit-sound-0.2.9/docs/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/jquery.js` & `scikit-sound-0.2.9/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/language_data.js` & `scikit-sound-0.2.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/pygments.css` & `scikit-sound-0.2.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/searchtools.js` & `scikit-sound-0.2.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/sidebar.js` & `scikit-sound-0.2.9/docs/_build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/sksound.ico` & `scikit-sound-0.2.9/docs/_build/html/_static/sksound.ico`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/sksound.png` & `scikit-sound-0.2.9/docs/_build/html/_static/sksound.png`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/underscore-1.12.0.js` & `scikit-sound-0.2.9/docs/_build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/underscore-1.3.1.js` & `scikit-sound-0.2.9/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/underscore.js` & `scikit-sound-0.2.9/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/_static/websupport.js` & `scikit-sound-0.2.9/docs/_build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/genindex.html` & `scikit-sound-0.2.9/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/index.html` & `scikit-sound-0.2.9/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/misc.html` & `scikit-sound-0.2.9/docs/_build/html/misc.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/py-modindex.html` & `scikit-sound-0.2.9/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/search.html` & `scikit-sound-0.2.9/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/searchindex.js` & `scikit-sound-0.2.9/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_build/html/sounds.html` & `scikit-sound-0.2.9/docs/_build/html/sounds.html`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_static/sksound.ico` & `scikit-sound-0.2.9/docs/_static/sksound.ico`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/_static/sksound.png` & `scikit-sound-0.2.9/docs/_static/sksound.png`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/conf.py` & `scikit-sound-0.2.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 copyright = u'2021, thomas haslwanter'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.2.8'
+version = '0.2.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.2.7'
+release = '0.2.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `scikit-sound-0.2.8/docs/index.rst` & `scikit-sound-0.2.9/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -81,13 +81,13 @@
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 .. note::
     | *Author:*     Thomas Haslwanter
-    | *Version:*    0.2.8
+    | *Version:*    0.2.9
     | *Date:*       April 2021
     | *email:*      thomas.haslwanter@fh-linz.at
     | *Copyright (c):*      2021, Thomas Haslwanter. All rights reserved.
     | *Licence:*    This work is licensed under the `BSD 2-Clause License <http://opensource.org/licenses/BSD-2-Clause>`_
```

### Comparing `scikit-sound-0.2.8/docs/make.bat` & `scikit-sound-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/misc.rst` & `scikit-sound-0.2.9/docs/misc.rst`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/docs/sounds.rst` & `scikit-sound-0.2.9/docs/sounds.rst`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/scikit_sound.egg-info/PKG-INFO` & `scikit-sound-0.2.9/scikit_sound.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-sound
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python utilites for working with sound signals
 Home-page: http://work.thaslwanter.at/sksound/html
 Author: Thomas Haslwanter
 Author-email: thomas.haslwanter@fh-linz.at
 License: http://opensource.org/licenses/BSD-2-Clause
 Download-URL: https://github.com/thomas-haslwanter/scikit-sound
 Description: ============
@@ -19,15 +19,15 @@
         
         Homepage
         --------
         http://work.thaslwanter.at/sksound/html/
         
         :Author:  Thomas Haslwanter
         :Date:    02-04-2021
-        :Ver:     0.2.8
+        :Ver:     0.2.9
         :Licence: BSD 2-Clause License (http://opensource.org/licenses/BSD-2-Clause)
         :Copyright:
             |copy| 2021, Thomas Haslwanter, all rights reserved.
         
         .. |copy|   unicode:: U+000A9 .. COPYRIGHT SIGN
         
         Installation
```

### Comparing `scikit-sound-0.2.8/scikit_sound.egg-info/SOURCES.txt` & `scikit-sound-0.2.9/scikit_sound.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/setup.py` & `scikit-sound-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import sys
 
 # Only need "pygame" on linux
 if sys.platform == 'linux':
     setup(
         name='scikit-sound',
-        version="0.2.8",
+        version="0.2.9",
         packages=find_packages(),
     
         include_package_data=True,
         package_data = {'tests': ['*.wav', '*.mp3']},
     
         # Project uses reStructuredText, so ensure that the docutils get
         # installed or upgraded on the target machine
@@ -33,15 +33,15 @@
         test_suite   = 'nose.collector',
         tests_require=['nose'],
     )
     
 else:
     setup(
         name='scikit-sound',
-        version="0.2.8",
+        version="0.2.9",
         packages=find_packages(),
     
         include_package_data=True,
         package_data = {'tests': ['*.wav', '*.mp3']},
     
         # Project uses reStructuredText, so ensure that the docutils get
         # installed or upgraded on the target machine
```

### Comparing `scikit-sound-0.2.8/sksound/__init__.py` & `scikit-sound-0.2.9/sksound/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 '''
 
 import importlib
 
 __author__ = "Thomas Haslwanter <thomas.haslwanter@fh-linz.at"
 __license__ = "BSD 2-Clause License"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 __all__ = ['misc', 'sounds']
 
 for _m in __all__:
     importlib.import_module('.'+_m, package='sksound')
```

### Comparing `scikit-sound-0.2.8/sksound/misc.py` & `scikit-sound-0.2.9/sksound/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,15 +215,20 @@
     >>> my_wish = sksound.misc.askquestion('Work or Play', 'Do you want to go home?')
     
     """
     
     root = tkinter.Tk()
     root.withdraw()
     
-    yes_no = messagebox.askyesno(title=DialogTitle, message=Question)
+    # On some systems, this dialog remains in the back
+    # To overcome that, move it up. Unfortunately, this somehow also makes the
+    # "root" visible again :(
+    # To be fixed sometime ...
+    to_top = tkinter.Toplevel(root)
+    yes_no = messagebox.askyesno(title=DialogTitle, message=Question, master=to_top)
     
     # Close the Tk-window manager again
     root.destroy()
     
     return yes_no
```

### Comparing `scikit-sound-0.2.8/sksound/sounds.py` & `scikit-sound-0.2.9/sksound/sounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,19 +30,16 @@
     - Mac:  	"/usr/local/bin/" (is already included in the default paths of the Mac terminal.)
     - Linux:	"/usr/bin/"
 
 Compatible with Python >=3.5
 
 """
 
-'''
-Date:   March-2021
-Author: thomas haslwanter
-
-'''
+# Author: thomas haslwanter
+# Date:   March-2021
 
 
 # "ffmpeg" has to be installed externally, into the location listed below
 # You can obtain it for free from http://ffmpeg.org
 
 import numpy as np
```

### Comparing `scikit-sound-0.2.8/sksound/tests/YouAreNotIt.mp3` & `scikit-sound-0.2.9/sksound/tests/YouAreNotIt.mp3`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/YouAreNotIt.wav` & `scikit-sound-0.2.9/sksound/tests/YouAreNotIt.wav`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/a1.wav` & `scikit-sound-0.2.9/sksound/tests/a1.wav`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/float_sound.wav` & `scikit-sound-0.2.9/sksound/tests/float_sound.wav`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/peas.wav` & `scikit-sound-0.2.9/sksound/tests/peas.wav`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/test_sound.py` & `scikit-sound-0.2.9/sksound/tests/test_sound.py`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/tiger.wav` & `scikit-sound-0.2.9/sksound/tests/tiger.wav`

 * *Files identical despite different names*

### Comparing `scikit-sound-0.2.8/sksound/tests/tmp.wav` & `scikit-sound-0.2.9/sksound/tests/tmp.wav`

 * *Files identical despite different names*

