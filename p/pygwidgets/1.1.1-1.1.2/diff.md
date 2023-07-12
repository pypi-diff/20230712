# Comparing `tmp/pygwidgets-1.1.1.tar.gz` & `tmp/pygwidgets-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwidgets-1.1.1.tar", last modified: Sun Jul  9 18:42:31 2023, max compression
+gzip compressed data, was "pygwidgets-1.1.2.tar", last modified: Wed Jul 12 18:02:01 2023, max compression
```

## Comparing `pygwidgets-1.1.1.tar` & `pygwidgets-1.1.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.063713 pygwidgets-1.1.1/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pygwidgets-1.1.1/LICENSE
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.1.1/MANIFEST.in
--rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-09 18:42:31.063464 pygwidgets-1.1.1/PKG-INFO
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1916 2023-07-08 02:58:02.000000 pygwidgets-1.1.1/README
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.032749 pygwidgets-1.1.1/pygwidgets/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.1.1/pygwidgets/__init__.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     5192 2023-07-09 18:40:24.000000 pygwidgets-1.1.1/pygwidgets/conf.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)   153339 2023-07-07 23:39:38.000000 pygwidgets-1.1.1/pygwidgets/pygwidgets.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.034354 pygwidgets-1.1.1/pygwidgets.egg-info/
--rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-09 18:42:30.000000 pygwidgets-1.1.1/pygwidgets.egg-info/PKG-INFO
--rw-r--r--   0 irvkalb    (501) staff       (20)     2582 2023-07-09 18:42:31.000000 pygwidgets-1.1.1/pygwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-09 18:42:30.000000 pygwidgets-1.1.1/pygwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       15 2023-07-09 18:42:30.000000 pygwidgets-1.1.1/pygwidgets.egg-info/requires.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-09 18:42:30.000000 pygwidgets-1.1.1/pygwidgets.egg-info/top_level.txt
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.035010 pygwidgets-1.1.1/pygwidgets_test/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    13561 2023-05-29 17:59:51.000000 pygwidgets-1.1.1/pygwidgets_test/Main_Test_pygwidgets.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.1.1/pygwidgets_test/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.056012 pygwidgets-1.1.1/pygwidgets_test/images/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.1.1/pygwidgets_test/images/background.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/dragMeDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/dragMeDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/dragMeOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/dragMeUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/extenDisabled.png
--rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.1.1/pygwidgets_test/images/frisbee.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.1.1/pygwidgets_test/images/imageDown.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/imageLeft.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.1.1/pygwidgets_test/images/imageRight.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.1.1/pygwidgets_test/images/imageStart.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.1.1/pygwidgets_test/images/imageUp.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.1.1/pygwidgets_test/images/pythonIcon.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioHighOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioLowOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/radioMedOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/restartButtonDisabled.png
--rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.1.1/pygwidgets_test/images/restartButtonDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/restartButtonOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/restartButtonUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/sliderExtent.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/sliderExtentDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/sliderThumb.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/sliderThumbDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/images/testImage.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:42:31.063039 pygwidgets-1.1.1/pygwidgets_test/sounds/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Anybutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Coin.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Item.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Jump.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Nextbutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/Warp.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/blip.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/boing.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/bonus.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.1.1/pygwidgets_test/sounds/dink.wav
--rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-09 18:42:31.063789 pygwidgets-1.1.1/setup.cfg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      748 2023-07-09 18:41:30.000000 pygwidgets-1.1.1/setup.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.451324 pygwidgets-1.1.2/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pygwidgets-1.1.2/LICENSE
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.1.2/MANIFEST.in
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-12 18:02:01.450120 pygwidgets-1.1.2/PKG-INFO
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1916 2023-07-08 02:58:02.000000 pygwidgets-1.1.2/README
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.396694 pygwidgets-1.1.2/pygwidgets/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.1.2/pygwidgets/__init__.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     5192 2023-07-12 17:59:47.000000 pygwidgets-1.1.2/pygwidgets/conf.py
+-rw-r--r--   0 irvkalb    (501) staff       (20)   153940 2023-07-11 20:25:19.000000 pygwidgets-1.1.2/pygwidgets/pygwidgets.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.398596 pygwidgets-1.1.2/pygwidgets.egg-info/
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-12 18:02:01.000000 pygwidgets-1.1.2/pygwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 irvkalb    (501) staff       (20)     2582 2023-07-12 18:02:01.000000 pygwidgets-1.1.2/pygwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-12 18:02:01.000000 pygwidgets-1.1.2/pygwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       15 2023-07-12 18:02:01.000000 pygwidgets-1.1.2/pygwidgets.egg-info/requires.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-12 18:02:01.000000 pygwidgets-1.1.2/pygwidgets.egg-info/top_level.txt
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.399792 pygwidgets-1.1.2/pygwidgets_test/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    13561 2023-05-29 17:59:51.000000 pygwidgets-1.1.2/pygwidgets_test/Main_Test_pygwidgets.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.1.2/pygwidgets_test/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.430158 pygwidgets-1.1.2/pygwidgets_test/images/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.1.2/pygwidgets_test/images/background.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/dragMeDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/dragMeDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/dragMeOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/dragMeUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/extenDisabled.png
+-rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.1.2/pygwidgets_test/images/frisbee.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.1.2/pygwidgets_test/images/imageDown.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/imageLeft.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.1.2/pygwidgets_test/images/imageRight.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.1.2/pygwidgets_test/images/imageStart.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.1.2/pygwidgets_test/images/imageUp.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.1.2/pygwidgets_test/images/pythonIcon.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioHighOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioLowOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/radioMedOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/restartButtonDisabled.png
+-rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.1.2/pygwidgets_test/images/restartButtonDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/restartButtonOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/restartButtonUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/sliderExtent.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/sliderExtentDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/sliderThumb.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/sliderThumbDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/images/testImage.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-12 18:02:01.449375 pygwidgets-1.1.2/pygwidgets_test/sounds/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Anybutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Coin.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Item.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Jump.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Nextbutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/Warp.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/blip.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/boing.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/bonus.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.1.2/pygwidgets_test/sounds/dink.wav
+-rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-12 18:02:01.451481 pygwidgets-1.1.2/setup.cfg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      748 2023-07-12 18:00:00.000000 pygwidgets-1.1.2/setup.py
```

### Comparing `pygwidgets-1.1.1/LICENSE` & `pygwidgets-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/PKG-INFO` & `pygwidgets-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.1.1
+Version: 1.1.2
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
 Keywords: pygame widgets user interface buttons text dragger animation image
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygwidgets-1.1.1/README` & `pygwidgets-1.1.2/README`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets/conf.py` & `pygwidgets-1.1.2/pygwidgets/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 project = 'pygwidgets'
 copyright = '2021, Irv Kalb'
 author = 'Irv Kalb'
 
 # The short X.Y version
 version = '1.1'
 # The full version, including alpha/beta/rc tags
-release = '1.1.1'
+release = '1.1.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '7.0.1'
```

### Comparing `pygwidgets-1.1.1/pygwidgets/pygwidgets.py` & `pygwidgets-1.1.2/pygwidgets/pygwidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,30 +117,30 @@
 ******************************************************************************************
 
 
 
 History:
 
 7/23  Version 1.1
--        SpriteSheetAnimationCollection class added
--        AnimationCollection class added
--        TextRadioButton: Added optional color for text and circle (radio button)
--        Added ability to work with PyInstaller to create executable application
--                    (builds proper paths on-the-fly)
--        SoundEffect class added
--        BackgroundSound class added
--        Button classes: added activationKeysList to press a button based on any list of keys
--            (enterToActivate still works and builds the list of activation keys for you)
--        CheckBox classes: Added toggleValue() method
+        SpriteSheetAnimationCollection class added
+        AnimationCollection class added
+        TextRadioButton: Added optional color for text and circle (radio button)
+        Added ability to work with PyInstaller to create executable application
+                    (builds proper paths on-the-fly)
+        SoundEffect class added
+        BackgroundSound class added
+        Button classes: added activationKeysList to press a button based on any list of keys
+            (enterToActivate still works and builds the list of activation keys for you)
+        CheckBox classes: Added toggleValue() method
         
 3/23 Version 1.0.4
--        Image - fixed two scale and rotate bugs (thanks to Lando Chan)
--        TextInput - add setLoc to work correctly when moving an input field (thanks to Renato Monteiro)
--        SpriteSheetAnimation - fixed bug in splitting images (thanks to Alex Stamps)
--        Button classes: 'soundOnClick' didn't do anything ... now plays the sound on click
+        Image - fixed two scale and rotate bugs (thanks to Lando Chan)
+        TextInput - add setLoc to work correctly when moving an input field (thanks to Renato Monteiro)
+        SpriteSheetAnimation - fixed bug in splitting images (thanks to Alex Stamps)
+        Button classes: 'soundOnClick' didn't do anything ... now plays the sound on click
 
 11/5/21  Version 1.0.3
         Changed DisplayText.setValue to also allow passing in tuple or list - displayed one element per line
         Added __all__ to define what gets imported when you import *
         Changed SpriteSheetAnimation to calculate number of columns in SpriteSheet.
         Added ImageCollection.getCurrentKey()
         Use abc module to implement abstract classes and abstract methods
@@ -299,25 +299,28 @@
     'PygwidgetsFontManager',
     'SpriteSheetAnimation',
     'SpriteSheetAnimationCollection',
     'SoundEffect',
     'TextButton',
     'TextCheckBox',
     'TextRadioButton',
+    'getPygwidgetsVersion',
+    'buildPathFromRelativePath',
+    'loadImage',
 ]
 
 import pygame
 import time
 from pygame.locals import *
 from abc import ABC, abstractmethod
 import os
 import sys
 
 
-__version__ = "x1.1"
+__version = "1.1"
 
 PYGWIDGETS_BLACK = (0, 0, 0)
 PYGWIDGETS_WHITE = (255, 255, 255)
 PYGWIDGETS_DARK_GRAY = (64, 64, 64)
 PYGWIDGETS_GRAY = (128, 128, 128)
 PYGWIDGETS_DOWN_GRAY = (140, 140, 140)
 PYGWIDGETS_NORMAL_GRAY = (170, 170, 170)
@@ -330,38 +333,55 @@
     PYGWIDGETS_CUSTOM_EVENT = pygame.USEREVENT  # older approach
 else:  # pygame version 2 and later
     PYGWIDGETS_CUSTOM_EVENT = pygame.event.custom_type() # new in pygame 2.0
 PYGWIDGETS_MOUSE_EVENTS_DICT = (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN)
 
 
 
-def getVersion():
-    """Returns the current version number of the pygwidgets package"""
-    version = "x1.1"
-    return version
-
-def loadImage(path):
-    """This function is used to resolve the path to an external image file, and load the contents.
-         It returns an image ready to be shown in the window.
-         It is a wrapper for the internal function _loadImageAndConvert()
-         """
-    return _loadImageAndConvert(path)
+def getPygwidgetsVersion():
+    """Called to retrieve the current version of pygwidgets
+
+    Returns:
+        |     the current major version of pygwidgets
+
+    """
+    return __version
+
+def loadImage(relativePath):
+    """Resolves a path to an image file and loads it.
+    This is typically used to load an image so you can then get its rect -
+    with a call to theImage.get_rect(), then extract the width and height
 
-def buildPathFromRelativePath(relPath):
+    Parameter:
+        |    relativePath - relative path to the image file
+
+    Returns:
+        |     an image
+
+    """
+    return _loadImageAndConvert(relativePath)
+
+def buildPathFromRelativePath(relativePath):
     """This function is needed because of the way that PyInstaller works.
-        PyInstaller creates a temp folder and stores the path in _MEIPASS
-        When running as an executable, this function modifies the path
-        to look for assets in this temporary folder, instead of the current
-        relative folder.
+    PyInstaller creates a temp folder and stores the path in _MEIPASS.
+    When running as an executable, it builds a path to this temporary folder.
+    When running in development, it just builds the full absolute path from the relative path.
+
+    Parameter:
+        |    relativePath - relative path to the image file
+
+    Returns:
+        |     an absolute path that can be used during development or from an executable file
+
     """
     try:
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.abspath(".")
-    absolutePath = os.path.join(base_path, relPath)
+    absolutePath = os.path.join(base_path, relativePath)
     #print('absolutePath is', absolutePath)
     return absolutePath
 
 def _loadImageAndConvert(path):
     # This call allows for running inside a development environment
     # and also works when running as an application built using PyInstaller.
     path = buildPathFromRelativePath(path)
@@ -503,30 +523,37 @@
         return self.rect
 
     # Left in for historical reasons
     def overlaps(self, otherRect):
         collided = otherRect.colliderect(self.rect)
         return collided
 
-    def overlapsRect(self, otherRect):
-        """Returns True if the rect object overlaps another rect
+    """def overlapsRect(self, otherRect):
+        Checks for overlap of two rectangles
 
         Parameter:
-            |   otherRect - a second rectangle to compare to           
+            |    oOtherRect - a second rectangle to compare to    
 
-        """
+        Returns:
+            |     True or False if the rect overlaps with the other rectangle
+            
         
         overlaps = self.rect.colliderect(otherRect)
         return overlaps
+        
+        """
 
     def overlapsObject(self, oOther):
-        """Returns True if the rect of this object overlaps with rect of another pygwidgets object
+        """Checks for overlap of two pygwidgets objects
         
         Parameter:
-            |    oOther - a second object to compare to           
+            |    oOther - a second object to compare to
+
+        Returns:
+            |     True or False if the rect of this object overlaps with the rect of another pygwidgets object
 
         """
         
         otherRect = oOther.getRect()
         overlaps = self.rect.colliderect(otherRect)
         return overlaps
 
@@ -2344,15 +2371,15 @@
         | oNextFieldOnTab - an InputText object that should gain focus if user hits TAB
 
         """
 
         self.oNextFieldOnTab = oNextFieldOnTab
 
     def setLoc(self, loc):
-        '''Move the field to some other location'''
+        """Move the field to some other location"""
         super().setLoc(loc)
         self.imageRect = pygame.Rect(self.loc[0], self.loc[1], self.width, self.height)
         self.rect = pygame.Rect(self.loc[0], self.loc[1], self.width, self.height)
         # Set the rect of the focus highlight rectangle (when the text has been clicked on and has focus)
         self.focusedImageRect = pygame.Rect(self.loc[0] - 3, self.loc[1] - 3, self.width + 6, self.height + 6)
         self.cursorLoc = [self.loc[0], self.loc[1]]  # this is a list because element 0 will change as the user edits
 
@@ -3547,15 +3574,15 @@
         pygame.mixer.init()
         try:
             self.oSound = pygame.mixer.Sound(fullPath)
         except FileNotFoundError:
             raise FileNotFoundError(f'Trying to create SoundEffect, but the file {relativePath} count not be found')
 
     def play(self):
-        '''Starts the sound effect playing'''
+        """Starts the sound effect playing"""
         self.oSound.play()
 
 class BackgroundSound():
     """BackgroundSound - allows you to play a long background file - typically music.
            Each is typically a .mp3 file.
 
     Typical use:
@@ -3591,32 +3618,32 @@
             | start - how far into the music to start (default is 0.0 meaning start at the beginning)
 
         """
         pygame.mixer.music.play(nLoops, start)
         self.musicPlaying = True
 
     def play(self, nLoops=-1, start=0.0):
-        '''Starts the music playing (same as start)'''
+        """Starts the music playing (same as start)"""
         pygame.mixer.music.play(nLoops, start)
         self.musicPlaying = True
 
     def pause(self):
-        '''If music is playing, pause the music'''
+        """If music is playing, pause the music"""
         if self.musicPlaying:
             pygame.mixer.music.pause()
             self.musicPaused = True
 
     def unPause(self):
-        '''If music is playing, but is paused, unpause the music to let it play again'''
+        """If music is playing, but is paused, unpause the music to let it play again"""
         if self.musicPlaying and self.musicPaused:
             pygame.mixer.music.unpause()
             self.musicPaused = False
 
     def stop(self):
-        '''Stops the current music that is playing'''
+        """Stops the current music that is playing"""
         pygame.mixer.music.stop()
         self.musicPlaying = False
         self.musicPaused = False
 
     def getPlaying(self):
-        '''Returns True if the music is playing, or False if it is not'''
+        """Returns True if the music is playing, or False if it is not"""
         return self.musicPlaying
```

### Comparing `pygwidgets-1.1.1/pygwidgets.egg-info/PKG-INFO` & `pygwidgets-1.1.2/pygwidgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.1.1
+Version: 1.1.2
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
 Keywords: pygame widgets user interface buttons text dragger animation image
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygwidgets-1.1.1/pygwidgets.egg-info/SOURCES.txt` & `pygwidgets-1.1.2/pygwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/Main_Test_pygwidgets.py` & `pygwidgets-1.1.2/pygwidgets_test/Main_Test_pygwidgets.py`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/background.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/background.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOff.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOff.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOffDisabled.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOffDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOffDown.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOffDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOn.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOn.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOnDisabled.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOnDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/checkBoxOnDown.png` & `pygwidgets-1.1.2/pygwidgets_test/images/checkBoxOnDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/dragMeDisabled.png` & `pygwidgets-1.1.2/pygwidgets_test/images/dragMeDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/dragMeDown.png` & `pygwidgets-1.1.2/pygwidgets_test/images/dragMeDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/dragMeOver.png` & `pygwidgets-1.1.2/pygwidgets_test/images/dragMeOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/dragMeUp.png` & `pygwidgets-1.1.2/pygwidgets_test/images/dragMeUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/frisbee.png` & `pygwidgets-1.1.2/pygwidgets_test/images/frisbee.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/imageDown.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/imageDown.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/imageLeft.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/imageLeft.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/imageRight.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/imageRight.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/imageStart.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/imageStart.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/imageUp.jpg` & `pygwidgets-1.1.2/pygwidgets_test/images/imageUp.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/pythonIcon.png` & `pygwidgets-1.1.2/pygwidgets_test/images/pythonIcon.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/restartButtonDisabled.png` & `pygwidgets-1.1.2/pygwidgets_test/images/restartButtonDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/restartButtonDown.png` & `pygwidgets-1.1.2/pygwidgets_test/images/restartButtonDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/restartButtonOver.png` & `pygwidgets-1.1.2/pygwidgets_test/images/restartButtonOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/images/restartButtonUp.png` & `pygwidgets-1.1.2/pygwidgets_test/images/restartButtonUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Anybutton.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Anybutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Coin.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Coin.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Item.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Item.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Jump.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Jump.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Nextbutton.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Nextbutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/Warp.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/Warp.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/blip.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/blip.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/boing.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/boing.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/bonus.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/bonus.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/pygwidgets_test/sounds/dink.wav` & `pygwidgets-1.1.2/pygwidgets_test/sounds/dink.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.1.1/setup.py` & `pygwidgets-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pygwidgets',
-    version='1.1.1',
+    version='1.1.2',
     author='Irv Kalb',
     author_email='Irv@furrypants.com',
     description='User interface widgets for use with Pygame',
     long_description='User interface widgets for building programs using Pygame',
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
```

