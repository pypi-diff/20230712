# Comparing `tmp/htrc_topicexplorer-1.0b4.tar.gz` & `tmp/htrc_topicexplorer-1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htrc_topicexplorer-1.0b4.tar", last modified: Thu Mar 30 18:10:22 2023, max compression
+gzip compressed data, was "htrc_topicexplorer-1.0b5.tar", last modified: Wed Jul 12 19:02:07 2023, max compression
```

## Comparing `htrc_topicexplorer-1.0b4.tar` & `htrc_topicexplorer-1.0b5.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.277456 htrc_topicexplorer-1.0b4/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       45 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/.coveragerc
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1135 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/.travis.yml
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      808 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/AUTHORS
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    14225 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/CHANGELOG.md
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    53523 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/ChangeLog
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1743 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/LICENSE.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      139 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/MANIFEST.in
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1233 2023-03-30 18:10:22.277612 htrc_topicexplorer-1.0b4/PKG-INFO
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    12937 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/README.md
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      447 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/add_pagenos.py
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     3792 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/app.wsgi
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2699 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/appveyor.yml
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      353 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/benchmark.sh
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1779 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/citation.bib
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.248192 htrc_topicexplorer-1.0b4/config/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      474 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/config/ap.ini
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      462 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/config/htrc.datacapsule.ini
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      786 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/config/htrc.ini
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      605 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/config/sep.ini
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      705 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/config/sep.prod.ini
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1620 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/coverage.ps1
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     4267 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/coverage.sh
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.248330 htrc_topicexplorer-1.0b4/demo/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      737 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/demo/ap.md
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.250832 htrc_topicexplorer-1.0b4/docs/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     7704 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/Makefile
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     9420 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/conf.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      187 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/contributing.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1196 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/cookbook.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     8447 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/htrc.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1205 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/import_export.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      571 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/index.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       84 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/init.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4611 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/intro.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       90 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/launch.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     7010 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/make.bat
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       96 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/metadata.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      186 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/modules.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       96 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/notebook.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       84 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/prep.rst
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       87 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/docs/train.rst
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.251948 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1233 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/PKG-INFO
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4610 2023-03-30 18:10:22.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)        1 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      144 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/entry_points.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)        1 2023-03-30 18:04:21.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/not-zip-safe
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       47 2023-03-30 18:10:21.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/pbr.json
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      664 2023-03-30 18:10:22.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/requires.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       14 2023-03-30 18:10:22.000000 htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/top_level.txt
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.252541 htrc_topicexplorer-1.0b4/ipynb/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    18472 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/ipynb/Topic-Explorer-Tutorial.py2.ipynb
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    20278 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/ipynb/Topic-Explorer-Tutorial.py3.ipynb
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1959 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/ipynb/corpus.tmpl.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.253882 htrc_topicexplorer-1.0b4/mmseg/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    33180 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/mmseg/ancient_words.dic
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)   100818 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/mmseg/chars.dic
--rw-r--r--   0 samithaliyanage   (501) staff       (20)  1183760 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/mmseg/modern_words.dic
--rw-r--r--   0 samithaliyanage   (501) staff       (20)  1183760 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/mmseg/words.dic
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      440 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/ob_ids.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4843 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/release.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      660 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/requirements.txt
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1545 2023-03-30 18:10:22.278199 htrc_topicexplorer-1.0b4/setup.cfg
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      628 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/setup.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.255043 htrc_topicexplorer-1.0b4/tests/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/tests/__init__.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4150 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/tests/test_prep.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1675 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/tests/test_topicexplorer_lib_pdf.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.258150 htrc_topicexplorer-1.0b4/topicexplorer/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)       72 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/__init__.py
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    10389 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/__main__.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     5454 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/cluster.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1041 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/config.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      382 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/debug.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3587 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/demo.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      403 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/etag.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     5625 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/export.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2868 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/export_html.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.259679 htrc_topicexplorer-1.0b4/topicexplorer/extensions/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/__init__.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      767 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/ap.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1388 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/bibtex.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2470 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/htrc.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3459 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/htrc_features.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2013 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/inpho.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      815 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/jeff.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2686 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/jeffcombo.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      827 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/oldbailey.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1600 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/sep.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      969 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/extensions/title.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    22452 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/init.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.261111 htrc_topicexplorer-1.0b4/topicexplorer/lib/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/__init__.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4354 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/chinese.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1579 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/color.py
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    10658 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/hathitrust.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3986 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/mmseg.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4870 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/pdf.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1425 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/ssl.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     6296 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/util.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1363 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/lib/win32.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     9687 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/metadata.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3767 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/notebook.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    25898 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/prep.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    37998 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/server.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3481 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/tezimport.py
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.261250 htrc_topicexplorer-1.0b4/topicexplorer/tokenizer/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1168 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/tokenizer/__init__.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    15317 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/train.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     8389 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topicexplorer/update.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      919 2023-03-30 18:10:15.000000 htrc_topicexplorer-1.0b4/topicexplorer/version.py
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   125750 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/topics.zip
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      505 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/update-docs.sh
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.266866 htrc_topicexplorer-1.0b4/www/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     6148 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/.DS_Store
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     6265 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/bars.mustache.html
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    54623 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/bootstrap-tour.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      869 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/cluster.local.mustache.html
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     1876 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/cluster.mustache.html
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.267705 htrc_topicexplorer-1.0b4/www/css/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2700 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/bars.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      337 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/cluster.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      737 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/inpho-font.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1254 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/master.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2742 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/simple-sidebar.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     4649 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/css/splash.css
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.268384 htrc_topicexplorer-1.0b4/www/fonts/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     6104 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fonts/cc-icons.ttf
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1852 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fonts/inpho-font.eot
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1937 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fonts/inpho-font.svg
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1676 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fonts/inpho-font.ttf
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1052 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fonts/inpho-font.woff
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     8573 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/fulltext.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2048 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/help-home.md
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2839 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/help-hypershelf.md
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1239 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/help-topics.md
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     2020 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/htrc.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     8603 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/icons.js
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.270158 htrc_topicexplorer-1.0b4/www/img/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1131 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/ap.jpg
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    32038 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/htrc.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      212 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/icon-book.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      752 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/icon-doi.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      599 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/icon-fingerprint.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      547 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/icon-law.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      801 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/icon-wos.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      912 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/inpho.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    18689 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/inpho_logo.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      468 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/link.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      300 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/pdf.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      811 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/img/sep.png
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.271854 htrc_topicexplorer-1.0b4/www/lib/
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.243317 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.272307 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/css/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    16840 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/css/bootstrap-responsive.min.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   106006 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/css/bootstrap.min.css
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.272647 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/img/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     8777 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/img/glyphicons-halflings-white.png
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    12799 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/img/glyphicons-halflings.png
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.272885 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/js/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    28631 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/js/bootstrap.min.js
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.243536 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.274728 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    26132 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    47706 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css.map
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    23409 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     5532 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css.map
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   146082 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   389227 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.css.map
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   121260 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.min.css
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    54416 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.min.css.map
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.275960 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    20127 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   108738 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    45404 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    23424 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    18028 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.276481 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    68954 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/bootstrap.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    36868 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/bootstrap.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      484 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/npm.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1872 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/d3.promise.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      498 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/d3.promise.min.js
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)   126781 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/d3.v3.min.js
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.276629 htrc_topicexplorer-1.0b4/www/lib/inpho/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1985 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/inpho/util.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    96381 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/jquery-1.11.0.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    85578 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/jquery-2.2.4.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1267 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/jquery.cookie.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     7548 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/jquery.superdom.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    16469 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/mustache.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)    28193 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/lib/showdown.min.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     7067 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/master.local.mustache.html
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     9854 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/master.mustache.html
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    12785 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/nodes.js
-drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:10:22.277033 htrc_topicexplorer-1.0b4/www/papers/
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     1779 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/papers/aaai15-topic-explorer-demo.bib
--rw-r--r--   0 samithaliyanage   (501) staff       (20)   487014 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/papers/aaai15-topic-explorer-demo.pdf
--rw-r--r--   0 samithaliyanage   (501) staff       (20)      854 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/popover.content.mustache
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)       37 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/serve.sh
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     8210 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/splash.mustache.html
--rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    45504 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/topicprint.js
--rw-r--r--   0 samithaliyanage   (501) staff       (20)     3264 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b4/www/tour.js
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.641933 htrc_topicexplorer-1.0b5/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       45 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/.coveragerc
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1135 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/.travis.yml
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      835 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/AUTHORS
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    14225 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/CHANGELOG.md
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    53568 2023-07-12 19:02:06.000000 htrc_topicexplorer-1.0b5/ChangeLog
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1743 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/LICENSE.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      139 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/MANIFEST.in
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1233 2023-07-12 19:02:07.642131 htrc_topicexplorer-1.0b5/PKG-INFO
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    12937 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/README.md
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      447 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/add_pagenos.py
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     3792 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/app.wsgi
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2699 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/appveyor.yml
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      353 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/benchmark.sh
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1779 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/citation.bib
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.597381 htrc_topicexplorer-1.0b5/config/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      474 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/config/ap.ini
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      462 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/config/htrc.datacapsule.ini
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      786 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/config/htrc.ini
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      605 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/config/sep.ini
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      705 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/config/sep.prod.ini
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1620 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/coverage.ps1
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     4267 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/coverage.sh
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.597574 htrc_topicexplorer-1.0b5/demo/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      737 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/demo/ap.md
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.600544 htrc_topicexplorer-1.0b5/docs/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     7704 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/Makefile
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     9420 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/conf.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      187 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/contributing.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1196 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/cookbook.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     8447 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/htrc.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1205 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/import_export.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      571 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/index.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       84 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/init.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4611 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/intro.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       90 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/launch.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     7010 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/make.bat
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       96 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/metadata.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      186 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/modules.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       96 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/notebook.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       84 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/prep.rst
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       87 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/docs/train.rst
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.601685 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1233 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4610 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)        1 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      144 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/entry_points.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)        1 2023-03-30 18:04:21.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/not-zip-safe
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       47 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/pbr.json
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      664 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/requires.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       14 2023-07-12 19:02:07.000000 htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/top_level.txt
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.602280 htrc_topicexplorer-1.0b5/ipynb/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    18472 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/ipynb/Topic-Explorer-Tutorial.py2.ipynb
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    20278 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/ipynb/Topic-Explorer-Tutorial.py3.ipynb
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1959 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/ipynb/corpus.tmpl.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.605435 htrc_topicexplorer-1.0b5/mmseg/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    33180 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/mmseg/ancient_words.dic
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)   100818 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/mmseg/chars.dic
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)  1183760 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/mmseg/modern_words.dic
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)  1183760 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/mmseg/words.dic
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      440 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/ob_ids.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4843 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/release.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      660 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/requirements.txt
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1545 2023-07-12 19:02:07.642817 htrc_topicexplorer-1.0b5/setup.cfg
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      628 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/setup.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.607609 htrc_topicexplorer-1.0b5/tests/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/tests/__init__.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4150 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/tests/test_prep.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1675 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/tests/test_topicexplorer_lib_pdf.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.610929 htrc_topicexplorer-1.0b5/topicexplorer/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)       72 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/__init__.py
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    10389 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/__main__.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     5454 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/cluster.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1041 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/config.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      382 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/debug.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3587 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/demo.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      403 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/etag.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     5625 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/export.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2868 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/export_html.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.612962 htrc_topicexplorer-1.0b5/topicexplorer/extensions/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/__init__.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      767 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/ap.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1388 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/bibtex.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2470 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/htrc.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3459 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/htrc_features.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2013 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/inpho.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      815 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/jeff.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2686 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/jeffcombo.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      827 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/oldbailey.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1600 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/sep.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      969 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/extensions/title.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    22499 2023-07-12 16:00:38.000000 htrc_topicexplorer-1.0b5/topicexplorer/init.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.614296 htrc_topicexplorer-1.0b5/topicexplorer/lib/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)        0 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/__init__.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4354 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/chinese.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1579 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/color.py
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    10658 2023-07-12 18:43:48.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/hathitrust.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3986 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/mmseg.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4870 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/pdf.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1425 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/ssl.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     6296 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/util.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1363 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/lib/win32.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     9681 2023-07-12 18:45:22.000000 htrc_topicexplorer-1.0b5/topicexplorer/metadata.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3767 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/notebook.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    25898 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/prep.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    37998 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/server.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3481 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/tezimport.py
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.614429 htrc_topicexplorer-1.0b5/topicexplorer/tokenizer/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1168 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/tokenizer/__init__.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    15317 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/train.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     8389 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topicexplorer/update.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      919 2023-07-12 18:56:41.000000 htrc_topicexplorer-1.0b5/topicexplorer/version.py
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   125750 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/topics.zip
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      505 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/update-docs.sh
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.623804 htrc_topicexplorer-1.0b5/www/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     6148 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/.DS_Store
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     6265 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/bars.mustache.html
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    54623 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/bootstrap-tour.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      869 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/cluster.local.mustache.html
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     1876 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/cluster.mustache.html
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.624760 htrc_topicexplorer-1.0b5/www/css/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2700 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/bars.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      337 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/cluster.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      737 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/inpho-font.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1254 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/master.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2742 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/simple-sidebar.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     4649 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/css/splash.css
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.625985 htrc_topicexplorer-1.0b5/www/fonts/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     6104 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fonts/cc-icons.ttf
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1852 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fonts/inpho-font.eot
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1937 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fonts/inpho-font.svg
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1676 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fonts/inpho-font.ttf
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1052 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fonts/inpho-font.woff
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     8573 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/fulltext.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2048 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/help-home.md
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2839 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/help-hypershelf.md
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1239 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/help-topics.md
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     2020 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/htrc.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     8603 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/icons.js
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.628006 htrc_topicexplorer-1.0b5/www/img/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1131 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/ap.jpg
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    32038 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/htrc.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      212 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/icon-book.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      752 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/icon-doi.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      599 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/icon-fingerprint.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      547 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/icon-law.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      801 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/icon-wos.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      912 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/inpho.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    18689 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/inpho_logo.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      468 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/link.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      300 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/pdf.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      811 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/img/sep.png
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.630562 htrc_topicexplorer-1.0b5/www/lib/
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.591354 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.631132 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/css/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    16840 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/css/bootstrap-responsive.min.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   106006 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/css/bootstrap.min.css
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.631749 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/img/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     8777 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/img/glyphicons-halflings-white.png
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    12799 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/img/glyphicons-halflings.png
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.633798 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/js/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    28631 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/js/bootstrap.min.js
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.591579 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.637975 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    26132 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    47706 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css.map
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    23409 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     5532 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   146082 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   389227 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.css.map
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   121260 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.min.css
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    54416 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.min.css.map
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.639773 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    20127 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   108738 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    45404 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    23424 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    18028 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.640434 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    68954 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/bootstrap.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    36868 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/bootstrap.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      484 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/npm.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1872 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/d3.promise.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      498 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/d3.promise.min.js
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)   126781 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/d3.v3.min.js
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.640600 htrc_topicexplorer-1.0b5/www/lib/inpho/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1985 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/inpho/util.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    96381 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/jquery-1.11.0.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    85578 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/jquery-2.2.4.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1267 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/jquery.cookie.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     7548 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/jquery.superdom.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    16469 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/mustache.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)    28193 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/lib/showdown.min.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     7067 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/master.local.mustache.html
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     9854 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/master.mustache.html
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    12785 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/nodes.js
+drwxr-xr-x   0 samithaliyanage   (501) staff       (20)        0 2023-07-12 19:02:07.640892 htrc_topicexplorer-1.0b5/www/papers/
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     1779 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/papers/aaai15-topic-explorer-demo.bib
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)   487014 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/papers/aaai15-topic-explorer-demo.pdf
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)      854 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/popover.content.mustache
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)       37 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/serve.sh
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)     8210 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/splash.mustache.html
+-rwxr-xr-x   0 samithaliyanage   (501) staff       (20)    45504 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/topicprint.js
+-rw-r--r--   0 samithaliyanage   (501) staff       (20)     3264 2023-03-30 18:04:07.000000 htrc_topicexplorer-1.0b5/www/tour.js
```

### Comparing `htrc_topicexplorer-1.0b4/.travis.yml` & `htrc_topicexplorer-1.0b5/.travis.yml`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/AUTHORS` & `htrc_topicexplorer-1.0b5/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 colinallen <colallen@indiana.edu>
 colinallen <prof.colin.allen@gmail.com>
 gavinfreud <ramiyer1998@gmail.com>
 kirtansakariya <kirtansakariya@gmail.com>
 ramiyer1998 <ramiyer1998@gmail.com>
 rzawar <zawar.rohit@gmail.com>
 thomdaro <31260388+thomdaro@users.noreply.github.com>
+thomdaro <thomdaro@iu.edu>
 zhaoyang9425 <zhaoyang9425@gmail.com>
```

### Comparing `htrc_topicexplorer-1.0b4/CHANGELOG.md` & `htrc_topicexplorer-1.0b5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/ChangeLog` & `htrc_topicexplorer-1.0b5/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* possible fix for volume ID retrieval error
 * Prep for PyPI upload
 * Replicate changes on development fork
 * refactoring mouseout
 * refactoring bar\_mouseout
 * refactoriung mouseover
 * refactoring mouseover
 * fixing hover behavior
```

### Comparing `htrc_topicexplorer-1.0b4/LICENSE.txt` & `htrc_topicexplorer-1.0b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/PKG-INFO` & `htrc_topicexplorer-1.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htrc_topicexplorer
-Version: 1.0b4
+Version: 1.0b5
 Summary: InPhO Topic Explorer
 Home-page: https://www.hypershelf.org
 Download-URL: http://github.com/inpho/topic-explorer
 Author: The Indiana Philosophy Ontology (InPhO) Project
 Author-email: inpho@indiana.edu
 Maintainer: Jaimie Murdock
 Maintainer-email: jaimie@inphoproject.org
```

### Comparing `htrc_topicexplorer-1.0b4/README.md` & `htrc_topicexplorer-1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/app.wsgi` & `htrc_topicexplorer-1.0b5/app.wsgi`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/appveyor.yml` & `htrc_topicexplorer-1.0b5/appveyor.yml`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/citation.bib` & `htrc_topicexplorer-1.0b5/citation.bib`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/config/htrc.ini` & `htrc_topicexplorer-1.0b5/config/htrc.ini`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/config/sep.ini` & `htrc_topicexplorer-1.0b5/config/sep.ini`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/config/sep.prod.ini` & `htrc_topicexplorer-1.0b5/config/sep.prod.ini`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/coverage.ps1` & `htrc_topicexplorer-1.0b5/coverage.ps1`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/coverage.sh` & `htrc_topicexplorer-1.0b5/coverage.sh`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/demo/ap.md` & `htrc_topicexplorer-1.0b5/demo/ap.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/Makefile` & `htrc_topicexplorer-1.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/conf.py` & `htrc_topicexplorer-1.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/cookbook.rst` & `htrc_topicexplorer-1.0b5/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/htrc.rst` & `htrc_topicexplorer-1.0b5/docs/htrc.rst`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/import_export.rst` & `htrc_topicexplorer-1.0b5/docs/import_export.rst`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/index.rst` & `htrc_topicexplorer-1.0b5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/intro.rst` & `htrc_topicexplorer-1.0b5/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/docs/make.bat` & `htrc_topicexplorer-1.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/PKG-INFO` & `htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htrc-topicexplorer
-Version: 1.0b4
+Version: 1.0b5
 Summary: InPhO Topic Explorer
 Home-page: https://www.hypershelf.org
 Download-URL: http://github.com/inpho/topic-explorer
 Author: The Indiana Philosophy Ontology (InPhO) Project
 Author-email: inpho@indiana.edu
 Maintainer: Jaimie Murdock
 Maintainer-email: jaimie@inphoproject.org
```

### Comparing `htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/SOURCES.txt` & `htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/htrc_topicexplorer.egg-info/requires.txt` & `htrc_topicexplorer-1.0b5/htrc_topicexplorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/ipynb/Topic-Explorer-Tutorial.py2.ipynb` & `htrc_topicexplorer-1.0b5/ipynb/Topic-Explorer-Tutorial.py2.ipynb`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/ipynb/Topic-Explorer-Tutorial.py3.ipynb` & `htrc_topicexplorer-1.0b5/ipynb/Topic-Explorer-Tutorial.py3.ipynb`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/ipynb/corpus.tmpl.py` & `htrc_topicexplorer-1.0b5/ipynb/corpus.tmpl.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/mmseg/ancient_words.dic` & `htrc_topicexplorer-1.0b5/mmseg/ancient_words.dic`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/mmseg/chars.dic` & `htrc_topicexplorer-1.0b5/mmseg/chars.dic`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/mmseg/modern_words.dic` & `htrc_topicexplorer-1.0b5/mmseg/modern_words.dic`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/mmseg/words.dic` & `htrc_topicexplorer-1.0b5/mmseg/words.dic`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/release.py` & `htrc_topicexplorer-1.0b5/release.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/requirements.txt` & `htrc_topicexplorer-1.0b5/requirements.txt`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/setup.cfg` & `htrc_topicexplorer-1.0b5/setup.cfg`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/setup.py` & `htrc_topicexplorer-1.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/tests/test_prep.py` & `htrc_topicexplorer-1.0b5/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/tests/test_topicexplorer_lib_pdf.py` & `htrc_topicexplorer-1.0b5/tests/test_topicexplorer_lib_pdf.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/__main__.py` & `htrc_topicexplorer-1.0b5/topicexplorer/__main__.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/cluster.py` & `htrc_topicexplorer-1.0b5/topicexplorer/cluster.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/config.py` & `htrc_topicexplorer-1.0b5/topicexplorer/config.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/demo.py` & `htrc_topicexplorer-1.0b5/topicexplorer/demo.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/export.py` & `htrc_topicexplorer-1.0b5/topicexplorer/export.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/export_html.py` & `htrc_topicexplorer-1.0b5/topicexplorer/export_html.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/ap.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/ap.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/bibtex.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/bibtex.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/htrc.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/htrc.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/htrc_features.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/htrc_features.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/inpho.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/inpho.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/jeff.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/jeff.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/jeffcombo.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/jeffcombo.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/oldbailey.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/oldbailey.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/sep.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/sep.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/extensions/title.py` & `htrc_topicexplorer-1.0b5/topicexplorer/extensions/title.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/init.py` & `htrc_topicexplorer-1.0b5/topicexplorer/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,15 +524,15 @@
     if args.corpus_path[-4:] == '.pdf' or contains_pattern(args.corpus_path, '*.pdf'):
         config.set("www", "pdf", "true")
 
     config.add_section("logging")
     config.set("logging", "path", "logs/%s/{0}.log" % args.corpus_name)
 
     if args.htrc:
-        config = add_htrc_metadata(config, corpus_filename=os.path.abspath(args.corpus_filename))
+        config = add_htrc_metadata(config, corpus_filename=os.path.abspath(args.corpus_filename), corpus_path=os.path.abspath(args.corpus_path))
         if not args.corpus_print_name:
             config.set("www", "corpus_name", "HTRC Data Capsule")
 
     if args.tokenizer in ['zh','ltc','och']:
         config.set("main", "lang", "cn")
 
     if config_file is None:
```

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/chinese.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/chinese.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/color.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/color.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/hathitrust.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/hathitrust.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/mmseg.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/mmseg.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/pdf.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/pdf.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/ssl.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/ssl.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/util.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/util.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/lib/win32.py` & `htrc_topicexplorer-1.0b5/topicexplorer/lib/win32.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/metadata.py` & `htrc_topicexplorer-1.0b5/topicexplorer/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 from future import standard_library
 standard_library.install_aliases()
 from builtins import str
 
 from ast import literal_eval
 from codecs import open 
 import csv
-import os.path
+import os
 
 import topicexplorer.config
 from topicexplorer.lib.util import isint, is_valid_configfile, bool_prompt
 from sortedcontainers import SortedDict
 from unidecode import unidecode
 
 from vsm import Corpus
@@ -213,15 +213,15 @@
         else:
             data = [d[field] for d in new_data]
         corpus.context_data[i][field] = data
 
     return corpus
 
 
-def add_htrc_metadata(config, corpus=None, corpus_filename=None):
+def add_htrc_metadata(config, corpus=None, corpus_filename=None, corpus_path=None):
     import htrc.metadata
 
     config.set("main", "label_module", "topicexplorer.extensions.htrc")
     config.set("www", "doc_title_format", '<a href="{1}">{0}</a>')
     config.set("www", "doc_url_format", 'http://hdl.handle.net/2027/{0}')
     config.set("www", "icons", "htrcbook,link")
     config.set("main", "htrc", "True")
@@ -229,15 +229,15 @@
     if corpus_filename:
         corpus = Corpus.load(corpus_filename)
         config.set("main", "context_type", corpus.context_types[0])
     
     if corpus:
         ctx_type = config.get("main", "context_type")
         label_name = doc_label_name(ctx_type)
-        ids = corpus.view_metadata(ctx_type)[label_name]
+        ids = os.listdir(corpus_path)
         
         htrc_metapath = os.path.abspath(config.get("main", "corpus_file"))
         htrc_metapath = os.path.join(
             os.path.dirname(htrc_metapath),
             os.path.basename(htrc_metapath) + '.metadata.json')
 
         print("Downloading metadata to ", htrc_metapath)
```

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/notebook.py` & `htrc_topicexplorer-1.0b5/topicexplorer/notebook.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/prep.py` & `htrc_topicexplorer-1.0b5/topicexplorer/prep.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/server.py` & `htrc_topicexplorer-1.0b5/topicexplorer/server.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/tezimport.py` & `htrc_topicexplorer-1.0b5/topicexplorer/tezimport.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/tokenizer/__init__.py` & `htrc_topicexplorer-1.0b5/topicexplorer/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/train.py` & `htrc_topicexplorer-1.0b5/topicexplorer/train.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/update.py` & `htrc_topicexplorer-1.0b5/topicexplorer/update.py`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/topicexplorer/version.py` & `htrc_topicexplorer-1.0b5/topicexplorer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 
 class _VersionModule(types.ModuleType):
 
     @property
     def __version__(self):
-        return "1.0b4"
+        return "1.0b5"
 
     @property
     def __pretty_version__(self):
         from topicexplorer.update import get_dist
         try:
             from pip.utils import dist_is_editable
         except ImportError:
```

### Comparing `htrc_topicexplorer-1.0b4/topics.zip` & `htrc_topicexplorer-1.0b5/topics.zip`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/.DS_Store` & `htrc_topicexplorer-1.0b5/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/bars.mustache.html` & `htrc_topicexplorer-1.0b5/www/bars.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/bootstrap-tour.js` & `htrc_topicexplorer-1.0b5/www/bootstrap-tour.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/cluster.local.mustache.html` & `htrc_topicexplorer-1.0b5/www/cluster.local.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/cluster.mustache.html` & `htrc_topicexplorer-1.0b5/www/cluster.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/css/bars.css` & `htrc_topicexplorer-1.0b5/www/css/bars.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/css/inpho-font.css` & `htrc_topicexplorer-1.0b5/www/css/inpho-font.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/css/master.css` & `htrc_topicexplorer-1.0b5/www/css/master.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/css/simple-sidebar.css` & `htrc_topicexplorer-1.0b5/www/css/simple-sidebar.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/css/splash.css` & `htrc_topicexplorer-1.0b5/www/css/splash.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fonts/cc-icons.ttf` & `htrc_topicexplorer-1.0b5/www/fonts/cc-icons.ttf`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fonts/inpho-font.eot` & `htrc_topicexplorer-1.0b5/www/fonts/inpho-font.eot`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fonts/inpho-font.svg` & `htrc_topicexplorer-1.0b5/www/fonts/inpho-font.svg`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fonts/inpho-font.ttf` & `htrc_topicexplorer-1.0b5/www/fonts/inpho-font.ttf`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fonts/inpho-font.woff` & `htrc_topicexplorer-1.0b5/www/fonts/inpho-font.woff`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/fulltext.js` & `htrc_topicexplorer-1.0b5/www/fulltext.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/help-home.md` & `htrc_topicexplorer-1.0b5/www/help-home.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/help-hypershelf.md` & `htrc_topicexplorer-1.0b5/www/help-hypershelf.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/help-topics.md` & `htrc_topicexplorer-1.0b5/www/help-topics.md`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/htrc.js` & `htrc_topicexplorer-1.0b5/www/htrc.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/icons.js` & `htrc_topicexplorer-1.0b5/www/icons.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/ap.jpg` & `htrc_topicexplorer-1.0b5/www/img/ap.jpg`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/htrc.png` & `htrc_topicexplorer-1.0b5/www/img/htrc.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/icon-doi.png` & `htrc_topicexplorer-1.0b5/www/img/icon-doi.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/icon-fingerprint.png` & `htrc_topicexplorer-1.0b5/www/img/icon-fingerprint.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/icon-law.png` & `htrc_topicexplorer-1.0b5/www/img/icon-law.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/icon-wos.png` & `htrc_topicexplorer-1.0b5/www/img/icon-wos.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/inpho.png` & `htrc_topicexplorer-1.0b5/www/img/inpho.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/inpho_logo.png` & `htrc_topicexplorer-1.0b5/www/img/inpho_logo.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/img/sep.png` & `htrc_topicexplorer-1.0b5/www/img/sep.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/css/bootstrap-responsive.min.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/css/bootstrap.min.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/img/glyphicons-halflings-white.png` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/img/glyphicons-halflings.png` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-2.3.2/js/bootstrap.min.js` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-2.3.2/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css.map` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css.map` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.css.map` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.min.css` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/css/bootstrap.min.css.map` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.eot` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.svg` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.ttf` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff2` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/bootstrap.js` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/bootstrap-3.3.6/js/bootstrap.min.js` & `htrc_topicexplorer-1.0b5/www/lib/bootstrap-3.3.6/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/d3.promise.js` & `htrc_topicexplorer-1.0b5/www/lib/d3.promise.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/d3.v3.min.js` & `htrc_topicexplorer-1.0b5/www/lib/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/inpho/util.js` & `htrc_topicexplorer-1.0b5/www/lib/inpho/util.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/jquery-1.11.0.min.js` & `htrc_topicexplorer-1.0b5/www/lib/jquery-1.11.0.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/jquery-2.2.4.min.js` & `htrc_topicexplorer-1.0b5/www/lib/jquery-2.2.4.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/jquery.cookie.min.js` & `htrc_topicexplorer-1.0b5/www/lib/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/jquery.superdom.min.js` & `htrc_topicexplorer-1.0b5/www/lib/jquery.superdom.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/mustache.js` & `htrc_topicexplorer-1.0b5/www/lib/mustache.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/lib/showdown.min.js` & `htrc_topicexplorer-1.0b5/www/lib/showdown.min.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/master.local.mustache.html` & `htrc_topicexplorer-1.0b5/www/master.local.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/master.mustache.html` & `htrc_topicexplorer-1.0b5/www/master.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/nodes.js` & `htrc_topicexplorer-1.0b5/www/nodes.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/papers/aaai15-topic-explorer-demo.bib` & `htrc_topicexplorer-1.0b5/www/papers/aaai15-topic-explorer-demo.bib`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/papers/aaai15-topic-explorer-demo.pdf` & `htrc_topicexplorer-1.0b5/www/papers/aaai15-topic-explorer-demo.pdf`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/popover.content.mustache` & `htrc_topicexplorer-1.0b5/www/popover.content.mustache`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/splash.mustache.html` & `htrc_topicexplorer-1.0b5/www/splash.mustache.html`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/topicprint.js` & `htrc_topicexplorer-1.0b5/www/topicprint.js`

 * *Files identical despite different names*

### Comparing `htrc_topicexplorer-1.0b4/www/tour.js` & `htrc_topicexplorer-1.0b5/www/tour.js`

 * *Files identical despite different names*

