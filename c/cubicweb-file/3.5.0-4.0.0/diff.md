# Comparing `tmp/cubicweb-file-3.5.0.tar.gz` & `tmp/cubicweb-file-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-file-3.5.0.tar", last modified: Thu Nov 24 01:05:13 2022, max compression
+gzip compressed data, was "cubicweb-file-4.0.0.tar", last modified: Wed Jul 12 14:15:27 2023, max compression
```

## Comparing `cubicweb-file-3.5.0.tar` & `cubicweb-file-4.0.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      569 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      965 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.556761 cubicweb-file-3.5.0/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     4550 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/ccplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.556761 cubicweb-file-3.5.0/cubicweb_file/data/
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/cubes.file.css
--rw-rw-rw-   0 root         (0) root         (0)      541 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/cubes.file.js
--rw-rw-rw-   0 root         (0) root         (0)     2070 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/file.png
--rw-rw-rw-   0 root         (0) root         (0)      274 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icon_file.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.560761 cubicweb-file-3.5.0/cubicweb_file/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)      116 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/README
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_javascript.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_pdf.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_rtf.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_vnd.ms-excel.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_vnd.ms-powerpoint.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_word.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_x-msdos-program.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_xml.ico
--rw-rw-rw-   0 root         (0) root         (0)     9662 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/application_zip.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/audio.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_mpeg.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_x-ms-wma.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_x-wav.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/default.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/image.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/image_gif.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/image_jpeg.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/image_png.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/image_x-ms-bmp.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/text.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/text_css.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/text_html.ico
--rw-rw-rw-   0 root         (0) root         (0)   161862 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/video.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/video_mpeg.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/video_quicktime.ico
--rw-rw-rw-   0 root         (0) root         (0)   161862 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/video_x-ms-wmv.ico
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/data/icons/video_x-msvideo.ico
--rw-rw-rw-   0 root         (0) root         (0)    14208 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/fsimport.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/hashtools.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.560761 cubicweb-file-3.5.0/cubicweb_file/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     1741 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     2304 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.560761 cubicweb-file-3.5.0/cubicweb_file/migration/
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/1.10.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/1.14.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/1.16.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/1.17.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/1.9.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/2.1.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/cubicweb_file/views/
--rw-rw-rw-   0 root         (0) root         (0)     2873 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3991 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/views/gallery.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/views/urlrewrite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/cubicweb_file/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      237 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/wdoc/ChangeLog_en
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/wdoc/ChangeLog_fr
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/wdoc/add_file_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/cubicweb_file/wdoc/toc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.556761 cubicweb-file-3.5.0/cubicweb_file.egg-info/
--rw-r--r--   0 root         (0) root         (0)      965 2022-11-24 01:05:12.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2682 2022-11-24 01:05:13.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:05:13.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-11-24 01:05:13.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:05:12.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-24 01:05:13.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-24 01:05:13.000000 cubicweb-file-3.5.0/cubicweb_file.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       84 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2627 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/data/20x20.gif
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      402 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:05:13.564761 cubicweb-file-3.5.0/test/data/toimport/
--rw-rw-rw-   0 root         (0) root         (0)   357916 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/data/toimport/IMG_8033.jpg
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/data/toimport/coucou.txt
--rw-rw-rw-   0 root         (0) root         (0)      283 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/test_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/unittest_cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/unittest_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/unittest_fsimport.py
--rw-rw-rw-   0 root         (0) root         (0)     8275 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2022-11-24 01:05:00.000000 cubicweb-file-3.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.311524 cubicweb-file-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      945 2023-07-12 14:15:27.311524 cubicweb-file-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.227523 cubicweb-file-4.0.0/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4466 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.235523 cubicweb-file-4.0.0/cubicweb_file/data/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/cubes.file.css
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/cubes.file.js
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/file.png
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icon_file.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.263523 cubicweb-file-4.0.0/cubicweb_file/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/README
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_javascript.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_pdf.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_rtf.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_vnd.ms-excel.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_vnd.ms-powerpoint.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_word.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_x-msdos-program.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_xml.ico
+-rw-rw-rw-   0 root         (0) root         (0)     9662 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/application_zip.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/audio.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_mpeg.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_x-ms-wma.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_x-wav.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/default.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/image.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/image_gif.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/image_jpeg.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/image_png.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/image_x-ms-bmp.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/text.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/text_css.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/text_html.ico
+-rw-rw-rw-   0 root         (0) root         (0)   161862 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/video.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/video_mpeg.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/video_quicktime.ico
+-rw-rw-rw-   0 root         (0) root         (0)   161862 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/video_x-ms-wmv.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/data/icons/video_x-msvideo.ico
+-rw-rw-rw-   0 root         (0) root         (0)    14149 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4257 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/fsimport.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/hashtools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.263523 cubicweb-file-4.0.0/cubicweb_file/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.271524 cubicweb-file-4.0.0/cubicweb_file/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/1.10.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/1.14.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/1.16.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/1.17.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/1.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/2.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.271524 cubicweb-file-4.0.0/cubicweb_file/views/
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3989 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/views/gallery.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/views/urlrewrite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.275524 cubicweb-file-4.0.0/cubicweb_file/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/wdoc/ChangeLog_fr
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/wdoc/add_file_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/cubicweb_file/wdoc/toc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.235523 cubicweb-file-4.0.0/cubicweb_file.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      945 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-07-12 14:15:27.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-12 14:15:26.000000 cubicweb-file-4.0.0/cubicweb_file.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:15:27.311524 cubicweb-file-4.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2609 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.283524 cubicweb-file-4.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.299524 cubicweb-file-4.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/data/20x20.gif
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:27.307524 cubicweb-file-4.0.0/test/data/toimport/
+-rw-rw-rw-   0 root         (0) root         (0)   357916 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/data/toimport/IMG_8033.jpg
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/data/toimport/coucou.txt
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/test_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/unittest_cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/unittest_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/unittest_fsimport.py
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-12 14:14:30.000000 cubicweb-file-4.0.0/tox.ini
```

### Comparing `cubicweb-file-3.5.0/MANIFEST.in` & `cubicweb-file-4.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/PKG-INFO` & `cubicweb-file-4.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-file
-Version: 3.5.0
+Version: 4.0.0
 Summary: file component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-file
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 This cube models `Files` (pdf document, word processor file, screenshots, etc).
 
@@ -21,9 +20,7 @@
 
 Please note that this thumbnail generation adaptor is not meant to be
 considered as a "public API" for thumbnail generation. This is just a
 simple solution waiting for a proper official API to manage such
 features as arbitrary content rendering.
 
 
-
-
```

### Comparing `cubicweb-file-3.5.0/README.rst` & `cubicweb-file-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/__pkginfo__.py` & `cubicweb-file-4.0.0/cubicweb_file/__pkginfo__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # pylint: disable-msg=W0622
 """cubicweb-file packaging information"""
 
 modname = "cubicweb_file"
 distname = "cubicweb-file"
 
-numversion = (3, 5, 0)
+numversion = (4, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "Logilab"
 author_email = "contact@logilab.fr"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 description = "file component for the CubicWeb framework"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python",
     "Programming Language :: JavaScript",
 ]
 
 __depends__ = {
-    "cubicweb": ">= 3.38.0, < 3.39.0",
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.1.0, < 2.0.0",
     "Pillow": None,
 }
 
 __recommends__ = {}
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/ccplugin.py` & `cubicweb-file-4.0.0/cubicweb_file/ccplugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 :organization: Logilab
 :copyright: 2010-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 import hashlib
 
+from cubicweb.cwconfig import CubicWebConfiguration
 from cubicweb.cwctl import CWCTL
 from cubicweb.toolsutils import Command
 
 
 class FSImportCommand(Command):
     """Import content of a directory on the file system as File entities.
     The instance must use the `file` cube.
@@ -46,20 +47,19 @@
                 "help": "put imported file into the folder entity of the given eid.",
             },
         ),
     )
 
     def run(self, args):
         """run the command with its specific arguments"""
-        from cubicweb.server.serverconfig import ServerConfiguration
         from cubicweb.server.serverctl import repo_cnx
         from cubicweb_file.fsimport import fsimport
 
         appid = args.pop(0)
-        config = ServerConfiguration.config_for(appid)
+        config = CubicWebConfiguration.config_for(appid)
         repo, cnx = repo_cnx(config)
         repo.hm.call_hooks("server_maintenance", repo=repo)
         with cnx:
             fsimport(
                 cnx,
                 args,
                 parenteid=self.config.filed_under,
@@ -114,19 +114,18 @@
                 "help": "Also refresh hash for entity types that inherit from File",
             },
         ),
     )
 
     def run(self, args):
         """run the command with its specific arguments"""
-        from cubicweb.server.serverconfig import ServerConfiguration
         from cubicweb.server.serverctl import repo_cnx
 
         appid = args.pop(0)
-        config = ServerConfiguration.config_for(appid)
+        config = CubicWebConfiguration.config_for(appid)
 
         repo, cnx = repo_cnx(config)
         if repo.vreg.config["compute-hash"] or self.config.force:
             repo.hm.call_hooks("server_maintenance", repo=repo)
             alg = self.config.hash_algorithm
 
             with cnx:
@@ -134,14 +133,14 @@
                     etypes = ["File"]
                     if self.config.subclasses:
                         etypes.extend(
                             cnx.repo.schema["File"].specialized_by(recursive=True)
                         )
                     print("ETYPES=", etypes)
                     for etype in etypes:
-                        for e in cnx.execute("Any X WHERE X is %s" % etype).entities():
+                        for e in cnx.execute(f"Any X WHERE X is {etype}").entities():
                             print("update hash for", e)
                             e.cw_set(data_hash=e.compute_hash(alg=alg))
                     cnx.commit()
 
 
 CWCTL.register(FSImportCommand)
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/cubes.file.js` & `cubicweb-file-4.0.0/cubicweb_file/data/cubes.file.js`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/file.png` & `cubicweb-file-4.0.0/cubicweb_file/data/file.png`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_javascript.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_javascript.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_pdf.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_pdf.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_rtf.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_rtf.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_vnd.ms-excel.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_vnd.ms-excel.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_vnd.ms-powerpoint.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_vnd.ms-powerpoint.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_word.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_word.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_x-msdos-program.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_x-msdos-program.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_xml.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_xml.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/application_zip.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/application_zip.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/audio.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/audio.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_mpeg.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_mpeg.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_x-ms-wma.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_x-ms-wma.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/audio_x-wav.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/audio_x-wav.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/default.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/default.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/image.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/image.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/image_gif.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/image_gif.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/image_jpeg.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/image_jpeg.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/image_png.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/image_png.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/image_x-ms-bmp.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/image_x-ms-bmp.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/text.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/text.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/text_css.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/text_css.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/text_html.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/text_html.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/video.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/video.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/video_mpeg.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/video_mpeg.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/video_quicktime.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/video_quicktime.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/video_x-ms-wmv.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/video_x-ms-wmv.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/data/icons/video_x-msvideo.ico` & `cubicweb-file-4.0.0/cubicweb_file/data/icons/video_x-msvideo.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/entities.py` & `cubicweb-file-4.0.0/cubicweb_file/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             if format:
                 self.cw_edited["data_format"] = str(format)
             if encoding:
                 self.cw_edited["data_encoding"] = str(encoding)
 
     def dc_title(self):
         if self.title:
-            return "%s (%s)" % (self.title, self.data_name)
+            return f"{self.title} ({self.data_name})"
         return self.data_name
 
     def size(self):
         rql = "Any LENGTH(D) WHERE X eid %(x)s, X data D"
         return self._cw.execute(rql, {"x": self.eid})[0][0]
 
     def read(self, size=-1):
@@ -119,15 +119,14 @@
 
         """
         if self.data_hash:
             return check_hash(self.data_hash, self.data and self.data.getvalue())
         return True
 
     def compute_hash(self, value=None, alg=None):
-
         """Compute the hash "value" data using "alg" hash algorithm.
         Returns a string "{ALG}HASH"
 
         If value is None, use stored data value.
 
         If alg is None, use currently configured hash algorithm (hash-algorithm
         in instance config options).
@@ -208,15 +207,15 @@
         if "small" in kwargs:
             warn(
                 "[1.15.0] `small` keyword is deprecated, you should use "
                 "FileThumbnailAdapter.download_thumbnail instead",
                 DeprecationWarning,
             )
         name = self._cw.url_quote(self.download_file_name())
-        path = "%s/raw/%s" % (self.entity.rest_path(), name)
+        path = f"{self.entity.rest_path()}/raw/{name}"
         return self._cw.build_url(path, **kwargs)
 
     def download_content_type(self):
         return self.entity.data_format
 
     def download_encoding(self):
         return self.entity.data_encoding
@@ -290,35 +289,35 @@
         done with the 'hash' hooks disabled).
 
         """
         cachedir = thumb_cache_dir(self._cw.vreg.config)
         if cachedir:
             hashhex = self.entity.hash_value
             size = self._cw.vreg.config["image-thumb-size"]
-            return join(cachedir, "%s_%s.png" % (hashhex, size))
+            return join(cachedir, f"{hashhex}_{size}.png")
         return None
 
     def thumbnail_file_name(self):
         name, _ext = splitext(self.entity.data_name)
         size = self._cw.vreg.config["image-thumb-size"]
-        return "%s_%s.png" % (name, size)
+        return f"{name}_{size}.png"
 
     def thumbnail_url(self):
         name = self._cw.url_quote(self.thumbnail_file_name())
-        path = "%s/thumb/%s" % (self.entity.rest_path(), name)
+        path = f"{self.entity.rest_path()}/thumb/{name}"
         return self._cw.build_url(path)
 
     def thumbnail_data(self):
         thumbpath = self._thumbnail_path()
         # use cache if it exists
         if thumbpath is not None:
             if isfile(thumbpath):
                 try:
                     return open(thumbpath, "rb").read()
-                except IOError:
+                except OSError:
                     self.warning("Failed to load cached thumbnail file %s", thumbpath)
         iimage = self.entity.cw_adapt_to("IImage")
         try:
             data = iimage.thumbnail().getvalue()
         except UnResizeable:
             self.info("Failed to generate thumbnail for %s", self.entity.eid)
             return ""
@@ -330,15 +329,15 @@
                 ) as tmp:
                     tmp.write(data)
                 try:
                     os.rename(tmp.name, thumbpath)
                 except Exception:
                     os.unlink(tmp.name)
                     raise
-            except EnvironmentError:
+            except OSError:
                 self.warning("Failed to save thumbnail in %s", thumbpath)
         return data
 
     def thumbnail_path(self):
         path = self._thumbnail_path()
         if path and exists(path):
             return path
@@ -350,15 +349,15 @@
 
 
 class IImageAdapter(EntityAdapter):
     __regid__ = "IImage"
     __select__ = has_mimetype("image/")
 
     def __init__(self, *args, **kwargs):
-        super(IImageAdapter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         idownloadable = self.entity.cw_adapt_to("IDownloadable")
         for meth in (
             "download_url",
             "download_content_type",
             "download_encoding",
             "download_file_name",
             "download_data",
@@ -386,15 +385,15 @@
         if size is None:
             size = self._cw.vreg.config["image-thumb-size"]
         size = tuple(int(s) for s in size.split("x"))
         idownloadable = self.entity.cw_adapt_to("IDownloadable")
         data = idownloadable.download_data()
         try:
             pilimg = pilopen(Binary(data))
-        except IOError:
+        except OSError:
             raise UnResizeable
         if shadow:
             self.warning(
                 "[1.15.0] the shadow parameter is now unused "
                 "and you should use css rules to lay shadows out",
                 DeprecationWarning,
             )
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/fsimport.py` & `cubicweb-file-4.0.0/cubicweb_file/fsimport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import print_function
-
 import sys
 from os import listdir, path as osp
 
 from cubicweb import Binary
 
 
 def fsimport(
@@ -21,17 +19,17 @@
     if parenteid is not None:
         parent = cw.execute("Any X WHERE X eid %(x)s", {"x": parenteid}).get_entity(
             0, 0
         )
     else:
         parent = None
     # XXX what if not bfss?
-    alreadyimported = set(
+    alreadyimported = {
         x.getvalue() for x, in cw.execute("Any fspath(D) WHERE X data D, X is File")
-    )
+    }
     for fspath in fspaths:
         fspath = osp.abspath(osp.normpath(fspath))
         if osp.isdir(fspath):
             import_directory(
                 cw,
                 fspath,
                 parent,
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/hashtools.py` & `cubicweb-file-4.0.0/cubicweb_file/hashtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 import hashlib
 
 
 def compute_hash(value, alg):
     hashvalue = compute_row_hash(value, alg)
     if hashvalue:
-        return "{%s}%s" % (alg, hashvalue)
+        return f"{{{alg}}}{hashvalue}"
 
 
 def compute_row_hash(value, alg):
     if value is not None:
         hasher = hashlib.new(alg, value)
         return str(hasher.hexdigest())
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/hooks.py` & `cubicweb-file-4.0.0/cubicweb_file/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/i18n/en.po` & `cubicweb-file-4.0.0/cubicweb_file/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/i18n/fr.po` & `cubicweb-file-4.0.0/cubicweb_file/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/migration/2.1.0_Any.py` & `cubicweb-file-4.0.0/cubicweb_file/migration/2.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/schema.py` & `cubicweb-file-4.0.0/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/site_cubicweb.py` & `cubicweb-file-4.0.0/cubicweb_file/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/cubicweb_file/views/__init__.py` & `cubicweb-file-4.0.0/cubicweb_file/views/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 
 
 class FileOneLine(baseviews.OneLineView):
     __select__ = is_instance("File")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        self.w('<img src="{}" alt=""/>'.format(entity.icon_url()))
-        super(FileOneLine, self).cell_call(row, col)
+        self.w(f'<img src="{entity.icon_url()}" alt=""/>')
+        super().cell_call(row, col)
 
 
 class FileInContext(baseviews.InContextView):
     __select__ = is_instance("File")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        self.w('<img src="{}" alt=""/>'.format(entity.icon_url()))
-        super(FileInContext, self).cell_call(row, col)
+        self.w(f'<img src="{entity.icon_url()}" alt=""/>')
+        super().cell_call(row, col)
 
 
 class FileOutOfContext(baseviews.OutOfContextView):
     __select__ = is_instance("File")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        self.w('<img src="{}" alt=""/>'.format(entity.icon_url()))
-        super(FileOutOfContext, self).cell_call(row, col)
+        self.w(f'<img src="{entity.icon_url()}" alt=""/>')
+        super().cell_call(row, col)
 
 
 class FileIcon(EntityView):
     __select__ = is_instance("File")
     __regid__ = "icon"
 
     def cell_call(self, row, col):
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file/views/gallery.py` & `cubicweb-file-4.0.0/cubicweb_file/views/gallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 lines.append([])
             lines[-1].append(self._make_cell(idx, 0))
         while len(lines[-1]) != nbcol:
             lines[-1].append("&#160;")
         self.w('<table class="album">')
         for line in lines:
             self.w("<tr>")
-            self.w("".join("<td>%s</td>" % cell for cell in line))
+            self.w("".join(f"<td>{cell}</td>" for cell in line))
             self.w("</tr>")
         self.w("</table>")
 
     def _make_cell(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
         icon = xml_escape(entity.cw_adapt_to("IThumbnail").thumbnail_url())
         title = xml_escape(entity.dc_title())
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file.egg-info/PKG-INFO` & `cubicweb-file-4.0.0/cubicweb_file.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-file
-Version: 3.5.0
+Version: 4.0.0
 Summary: file component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-file
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 This cube models `Files` (pdf document, word processor file, screenshots, etc).
 
@@ -21,9 +20,7 @@
 
 Please note that this thumbnail generation adaptor is not meant to be
 considered as a "public API" for thumbnail generation. This is just a
 simple solution waiting for a proper official API to manage such
 features as arbitrary content rendering.
 
 
-
-
```

### Comparing `cubicweb-file-3.5.0/cubicweb_file.egg-info/SOURCES.txt` & `cubicweb-file-4.0.0/cubicweb_file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/setup.py` & `cubicweb-file-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,17 +50,15 @@
 
 # get optional metadatas
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-file-3.5.0/test/data/toimport/IMG_8033.jpg` & `cubicweb-file-4.0.0/test/data/toimport/IMG_8033.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-file-3.5.0/test/unittest_cwctl.py` & `cubicweb-file-4.0.0/test/unittest_cwctl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from cubicweb import Binary
-from cubicweb.devtools import testlib, ApptestConfiguration
+from cubicweb.cwconfig import CubicWebConfiguration
+
 from cubicweb_file.ccplugin import FileRefreshHashCommand
-from cubicweb.server.serverconfig import ServerConfiguration
+from cubicweb_web.devtools.testlib import WebCWTC, WebApptestConfiguration
 
 
-class FileRefreshCommandTC(testlib.CubicWebTC):
+class FileRefreshCommandTC(WebCWTC):
     def setUp(self):
-        super(FileRefreshCommandTC, self).setUp()
-        self.orig_config_for = ServerConfiguration.config_for
+        super().setUp()
+        self.orig_config_for = CubicWebConfiguration.config_for
 
         def config_for(appid):
-            return ApptestConfiguration(appid, __file__)
+            return WebApptestConfiguration(appid, __file__)
 
-        ServerConfiguration.config_for = staticmethod(config_for)
+        CubicWebConfiguration.config_for = staticmethod(config_for)
 
     def tearDown(self):
-        ServerConfiguration.config_for = self.orig_config_for
-        super(FileRefreshCommandTC, self).tearDown()
+        CubicWebConfiguration.config_for = self.orig_config_for
+        super().tearDown()
 
     def test_refresh(self):
         with self.admin_access.repo_cnx() as cnx:
             cnx.vreg.config["compute-hash"] = 0
             for i in range(10):
                 fobj = cnx.create_entity(
                     "File",
@@ -28,15 +29,15 @@
                     data_format="text/plain",
                     data=Binary(b"xxx"),
                 )
                 self.assertEqual(None, fobj.data_hash)
             for i in range(10):
                 fobj = cnx.create_entity(
                     "MyFile",
-                    data_name="foo%s.png" % i,
+                    data_name=f"foo{i}.png",
                     data_format="image/png",
                     data=Binary(b"xxx"),
                 )
                 self.assertEqual(None, fobj.data_hash)
             cnx.commit()
         FileRefreshHashCommand(None).run([self.appid])
         with self.admin_access.repo_cnx() as cnx:
```

### Comparing `cubicweb-file-3.5.0/test/unittest_file.py` & `cubicweb-file-4.0.0/test/unittest_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# coding: utf-8
-
 from os.path import join, dirname, isfile, exists
 import shutil
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
-
 from cubicweb import NoSelectableObject, Binary, Unauthorized
 from cubicweb_web import NotFound
+from cubicweb_web.devtools.testlib import WebCWTC
 
 from cubicweb_file.entities import thumb_cache_dir
 
 
-class FileTC(CubicWebTC):
+class FileTC(WebCWTC):
     icon = "text.ico"
     mime_type = "text/plain"
 
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             create = cnx.create_entity
             self.fobj = create(
@@ -189,32 +186,32 @@
             )
             obj.cw_clear_all_caches()
             # note the absence of the hash algo "header" here:
             self.assertEqual("b60d121b438a380c343d5ec3c2037564b82ffef3", obj.data_hash)
             self.assertTrue(obj.check_hash())
 
 
-class ImageTC(CubicWebTC):
+class ImageTC(WebCWTC):
     icon = "image_png.ico"
     mime_type = "image/png"
 
     @property
     def data(self):
         with open(join(dirname(__file__), "data", "20x20.gif"), "rb") as fobj:
             return fobj.read()
 
     def setUp(self):
-        super(ImageTC, self).setUp()
+        super().setUp()
         cachedir = thumb_cache_dir(self.repo.vreg.config)
         if exists(cachedir):
             shutil.rmtree(cachedir)
         self.cachedir = cachedir
 
     def tearDown(self):
-        super(ImageTC, self).tearDown()
+        super().tearDown()
         if exists(self.cachedir):
             shutil.rmtree(self.cachedir)
 
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             create = cnx.create_entity
             self.fobj = create(
@@ -281,15 +278,15 @@
             cachepath = thumbadapter.thumbnail_path()
             self.assertTrue(isfile(cachepath))
             self.assertEqual(
                 open(cachepath, "rb").read(), thumbadapter.thumbnail_data()
             )
 
 
-class MimeTypeDetectionTC(CubicWebTC):
+class MimeTypeDetectionTC(WebCWTC):
     def test_extra_dot(self):
         with self.admin_access.client_cnx() as cnx:
             fobj = cnx.create_entity(
                 "File", data_name="foo.toto.pdf", data=Binary(b"xxx")
             )
             self.assertEqual(fobj.data_format, "application/pdf")
```

### Comparing `cubicweb-file-3.5.0/test/unittest_fsimport.py` & `cubicweb-file-4.0.0/test/unittest_fsimport.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class importDirectoryTC(CubicWebTC):
     def setup_database(self):
         storages.set_attribute_storage(self.repo, "File", "data", STORAGE)
 
     def tearDown(self):
         storages.unset_attribute_storage(self.repo, "File", "data")
-        super(importDirectoryTC, self).tearDown()
+        super().tearDown()
 
     def test_folder_bfss(self):
         with self.admin_access.repo_cnx() as cnx:
             fsimport(cnx, [join(HERE, "data", "toimport")], bfss=True, quiet=True)
             self.assertEqual(cnx.execute("Any COUNT(F) WHERE F is Folder")[0][0], 1)
             self.assertEqual(cnx.execute("Any COUNT(F) WHERE F is File")[0][0], 2)
             fpath = cnx.execute(
```

### Comparing `cubicweb-file-3.5.0/test/unittest_hooks.py` & `cubicweb-file-4.0.0/test/unittest_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 from os.path import join, dirname
 from PIL.Image import open as pilopen
 
 from cubicweb import Binary, Unauthorized
 from cubicweb.devtools.testlib import CubicWebTC
```

### Comparing `cubicweb-file-3.5.0/tox.ini` & `cubicweb-file-4.0.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
 envlist = py3, flake8, check-manifest, black, safety, yamllint
 
 [testenv]
 deps =
   pytest
+  webtest
   -rdev-requirements.txt
 commands =
   {envpython} -m pytest {posargs}
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
@@ -36,15 +37,15 @@
 deps = safety
 commands =
   {envpython} -msafety check --full-report
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -58,16 +59,16 @@
 commands =
   yamllint .
 
 [testenv:black]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black .
```

