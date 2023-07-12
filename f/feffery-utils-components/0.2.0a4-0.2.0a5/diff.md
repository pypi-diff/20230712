# Comparing `tmp/feffery_utils_components-0.2.0a4.tar.gz` & `tmp/feffery_utils_components-0.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_utils_components-0.2.0a4.tar", last modified: Mon Jul 10 09:50:53 2023, max compression
+gzip compressed data, was "feffery_utils_components-0.2.0a5.tar", last modified: Wed Jul 12 01:19:26 2023, max compression
```

## Comparing `feffery_utils_components-0.2.0a4.tar` & `feffery_utils_components-0.2.0a5.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.369332 feffery_utils_components-0.2.0a4/
--rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/LICENSE
--rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0      342 2023-07-10 09:50:53.369332 feffery_utils_components-0.2.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.357375 feffery_utils_components-0.2.0a4/feffery_utils_components/
--rw-rw-rw-   0        0        0     1877 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyAutoAnimate.py
--rw-rw-rw-   0        0        0     2015 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyBlockColorPicker.py
--rw-rw-rw-   0        0        0     2093 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCaptcha.py
--rw-rw-rw-   0        0        0     2207 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCircleColorPicker.py
--rw-rw-rw-   0        0        0     2784 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCompareSlider.py
--rw-rw-rw-   0        0        0     2049 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCookie.py
--rw-rw-rw-   0        0        0     1616 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountDown.py
--rw-rw-rw-   0        0        0     2508 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountUp.py
--rw-rw-rw-   0        0        0     1431 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCssVar.py
--rw-rw-rw-   0        0        0     2078 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDeviceDetect.py
--rw-rw-rw-   0        0        0     4313 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDiv.py
--rw-rw-rw-   0        0        0     1556 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDocumentVisibility.py
--rw-rw-rw-   0        0        0     1449 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExecuteJs.py
--rw-rw-rw-   0        0        0     1610 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalCss.py
--rw-rw-rw-   0        0        0     1602 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalJs.py
--rw-rw-rw-   0        0        0     2390 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExtraSpinner.py
--rw-rw-rw-   0        0        0     1526 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyEyeDropper.py
--rw-rw-rw-   0        0        0     2687 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyButton.py
--rw-rw-rw-   0        0        0     2816 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyMessage.py
--rw-rw-rw-   0        0        0     3737 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyNotification.py
--rw-rw-rw-   0        0        0     1733 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFullscreen.py
--rw-rw-rw-   0        0        0     1483 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGeolocation.py
--rw-rw-rw-   0        0        0     2037 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGithubColorPicker.py
--rw-rw-rw-   0        0        0     5043 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGrid.py
--rw-rw-rw-   0        0        0     1749 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGridItem.py
--rw-rw-rw-   0        0        0     3888 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGuide.py
--rw-rw-rw-   0        0        0     1727 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHexColorPicker.py
--rw-rw-rw-   0        0        0     2498 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHighlightWords.py
--rw-rw-rw-   0        0        0     1529 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyIdle.py
--rw-rw-rw-   0        0        0     1728 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyImagePaste.py
--rw-rw-rw-   0        0        0     1713 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyInViewport.py
--rw-rw-rw-   0        0        0     3879 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyJsonViewer.py
--rw-rw-rw-   0        0        0     1704 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyKeyPress.py
--rw-rw-rw-   0        0        0     2109 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLazyLoad.py
--rw-rw-rw-   0        0        0     1809 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenPaste.py
--rw-rw-rw-   0        0        0     1538 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenScroll.py
--rw-rw-rw-   0        0        0     1462 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenUnload.py
--rw-rw-rw-   0        0        0     1748 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocalStorage.py
--rw-rw-rw-   0        0        0     2108 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocation.py
--rw-rw-rw-   0        0        0     3312 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMotion.py
--rw-rw-rw-   0        0        0     1463 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMousePosition.py
--rw-rw-rw-   0        0        0     1577 2023-07-08 13:15:23.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyPopout.py
--rw-rw-rw-   0        0        0     2479 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyQRCode.py
--rw-rw-rw-   0        0        0     1449 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRawHTML.py
--rw-rw-rw-   0        0        0     1505 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyReload.py
--rw-rw-rw-   0        0        0     3724 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResizable.py
--rw-rw-rw-   0        0        0     1459 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResponsive.py
--rw-rw-rw-   0        0        0     1737 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRgbColorPicker.py
--rw-rw-rw-   0        0        0     2653 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScroll.py
--rw-rw-rw-   0        0        0     2531 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScrollbars.py
--rw-rw-rw-   0        0        0     1756 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySessionStorage.py
--rw-rw-rw-   0        0        0     1433 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySetTitle.py
--rw-rw-rw-   0        0        0     1753 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShadowDom.py
--rw-rw-rw-   0        0        0     3498 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShortcutPanel.py
--rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortable.py
--rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableContainer.py
--rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableItem.py
--rw-rw-rw-   0        0        0     3103 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableList.py
--rw-rw-rw-   0        0        0     2472 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplit.py
--rw-rw-rw-   0        0        0     1686 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplitPane.py
--rw-rw-rw-   0        0        0     1874 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySticky.py
--rw-rw-rw-   0        0        0     1433 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyStyle.py
--rw-rw-rw-   0        0        0     1533 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTimeout.py
--rw-rw-rw-   0        0        0     2845 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTopProgress.py
--rw-rw-rw-   0        0        0     2057 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTwitterColorPicker.py
--rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyUnmount.py
--rw-rw-rw-   0        0        0     2050 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyVirtualList.py
--rw-rw-rw-   0        0        0     2311 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWebSocket.py
--rw-rw-rw-   0        0        0     1629 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWheelColorPicker.py
--rw-rw-rw-   0        0        0     1528 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWindowSize.py
--rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/__init__.py
--rw-rw-rw-   0        0        0     4970 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/_imports_.py
--rw-rw-rw-   0        0        0  1380501 2023-07-10 09:50:49.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/feffery_utils_components.min.js
--rw-rw-rw-   0        0        0   209192 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/metadata.json
--rw-rw-rw-   0        0        0     4130 2023-07-10 09:50:50.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.367219 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/
--rw-rw-rw-   0        0        0      342 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3729 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4130 2023-07-10 09:17:35.000000 feffery_utils_components-0.2.0a4/package.json
--rw-rw-rw-   0        0        0       42 2023-07-10 09:50:53.370469 feffery_utils_components-0.2.0a4/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-16 02:41:22.000000 feffery_utils_components-0.2.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:26.037893 feffery_utils_components-0.2.0a5/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a5/LICENSE
+-rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0      342 2023-07-12 01:19:26.037893 feffery_utils_components-0.2.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:26.029074 feffery_utils_components-0.2.0a5/feffery_utils_components/
+-rw-rw-rw-   0        0        0     1877 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyAutoAnimate.py
+-rw-rw-rw-   0        0        0     2015 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyBlockColorPicker.py
+-rw-rw-rw-   0        0        0     2093 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCaptcha.py
+-rw-rw-rw-   0        0        0     2207 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCircleColorPicker.py
+-rw-rw-rw-   0        0        0     2784 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCompareSlider.py
+-rw-rw-rw-   0        0        0     2049 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCookie.py
+-rw-rw-rw-   0        0        0     1616 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCountDown.py
+-rw-rw-rw-   0        0        0     2508 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCountUp.py
+-rw-rw-rw-   0        0        0     1431 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCssVar.py
+-rw-rw-rw-   0        0        0     2078 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDeviceDetect.py
+-rw-rw-rw-   0        0        0     4313 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDiv.py
+-rw-rw-rw-   0        0        0     1556 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDocumentVisibility.py
+-rw-rw-rw-   0        0        0     1449 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExecuteJs.py
+-rw-rw-rw-   0        0        0     1610 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExternalCss.py
+-rw-rw-rw-   0        0        0     1602 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExternalJs.py
+-rw-rw-rw-   0        0        0     2390 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExtraSpinner.py
+-rw-rw-rw-   0        0        0     1526 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyEyeDropper.py
+-rw-rw-rw-   0        0        0     2687 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyButton.py
+-rw-rw-rw-   0        0        0     2816 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyMessage.py
+-rw-rw-rw-   0        0        0     3737 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyNotification.py
+-rw-rw-rw-   0        0        0     1733 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFullscreen.py
+-rw-rw-rw-   0        0        0     1483 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGeolocation.py
+-rw-rw-rw-   0        0        0     2037 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGithubColorPicker.py
+-rw-rw-rw-   0        0        0     5043 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGrid.py
+-rw-rw-rw-   0        0        0     1749 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGridItem.py
+-rw-rw-rw-   0        0        0     3888 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGuide.py
+-rw-rw-rw-   0        0        0     1727 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyHexColorPicker.py
+-rw-rw-rw-   0        0        0     2498 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyHighlightWords.py
+-rw-rw-rw-   0        0        0     1529 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyIdle.py
+-rw-rw-rw-   0        0        0     1728 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyImagePaste.py
+-rw-rw-rw-   0        0        0     1713 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyInViewport.py
+-rw-rw-rw-   0        0        0     3879 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyJsonViewer.py
+-rw-rw-rw-   0        0        0     1704 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyKeyPress.py
+-rw-rw-rw-   0        0        0     2109 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLazyLoad.py
+-rw-rw-rw-   0        0        0     1809 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenPaste.py
+-rw-rw-rw-   0        0        0     1538 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenScroll.py
+-rw-rw-rw-   0        0        0     1462 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenUnload.py
+-rw-rw-rw-   0        0        0     1748 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLocalStorage.py
+-rw-rw-rw-   0        0        0     2108 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLocation.py
+-rw-rw-rw-   0        0        0     3312 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyMotion.py
+-rw-rw-rw-   0        0        0     1463 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyMousePosition.py
+-rw-rw-rw-   0        0        0     1577 2023-07-08 13:15:23.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyPopout.py
+-rw-rw-rw-   0        0        0     2479 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyQRCode.py
+-rw-rw-rw-   0        0        0     1449 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyRawHTML.py
+-rw-rw-rw-   0        0        0     1505 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyReload.py
+-rw-rw-rw-   0        0        0     3724 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyResizable.py
+-rw-rw-rw-   0        0        0     1459 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyResponsive.py
+-rw-rw-rw-   0        0        0     1737 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyRgbColorPicker.py
+-rw-rw-rw-   0        0        0     2653 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyScroll.py
+-rw-rw-rw-   0        0        0     2531 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyScrollbars.py
+-rw-rw-rw-   0        0        0     1756 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySessionStorage.py
+-rw-rw-rw-   0        0        0     1433 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySetTitle.py
+-rw-rw-rw-   0        0        0     1753 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyShadowDom.py
+-rw-rw-rw-   0        0        0     3498 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyShortcutPanel.py
+-rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortable.py
+-rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableContainer.py
+-rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableItem.py
+-rw-rw-rw-   0        0        0     3103 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableList.py
+-rw-rw-rw-   0        0        0     2472 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySplit.py
+-rw-rw-rw-   0        0        0     1686 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySplitPane.py
+-rw-rw-rw-   0        0        0     1874 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySticky.py
+-rw-rw-rw-   0        0        0     1433 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyStyle.py
+-rw-rw-rw-   0        0        0     1820 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTextSelection.py
+-rw-rw-rw-   0        0        0     1533 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTimeout.py
+-rw-rw-rw-   0        0        0     2845 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTopProgress.py
+-rw-rw-rw-   0        0        0     2057 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTwitterColorPicker.py
+-rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyUnmount.py
+-rw-rw-rw-   0        0        0     2050 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyVirtualList.py
+-rw-rw-rw-   0        0        0     2311 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWebSocket.py
+-rw-rw-rw-   0        0        0     1629 2023-07-12 01:19:24.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWheelColorPicker.py
+-rw-rw-rw-   0        0        0     1528 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWindowSize.py
+-rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/__init__.py
+-rw-rw-rw-   0        0        0     5055 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/_imports_.py
+-rw-rw-rw-   0        0        0  1382766 2023-07-12 01:19:22.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/feffery_utils_components.min.js
+-rw-rw-rw-   0        0        0   211444 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/metadata.json
+-rw-rw-rw-   0        0        0     4065 2023-07-12 01:19:23.000000 feffery_utils_components-0.2.0a5/feffery_utils_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:26.035784 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3778 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-12 01:19:25.000000 feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4065 2023-07-11 14:18:26.000000 feffery_utils_components-0.2.0a5/package.json
+-rw-rw-rw-   0        0        0       42 2023-07-12 01:19:26.039031 feffery_utils_components-0.2.0a5/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-16 02:41:22.000000 feffery_utils_components-0.2.0a5/setup.py
```

### Comparing `feffery_utils_components-0.2.0a4/LICENSE` & `feffery_utils_components-0.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/README.md` & `feffery_utils_components-0.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyAutoAnimate.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyAutoAnimate.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyBlockColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyBlockColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCaptcha.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCaptcha.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCircleColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCircleColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCompareSlider.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCompareSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCookie.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCookie.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountDown.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCountDown.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountUp.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCountUp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCssVar.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyCssVar.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDeviceDetect.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDeviceDetect.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDiv.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDiv.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDocumentVisibility.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyDocumentVisibility.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExecuteJs.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExecuteJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalCss.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExternalCss.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalJs.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExternalJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExtraSpinner.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyExtraSpinner.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyEyeDropper.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyEyeDropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyButton.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyButton.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyMessage.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyNotification.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFancyNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFullscreen.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyFullscreen.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGeolocation.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGeolocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGithubColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGithubColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGrid.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGridItem.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGridItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGuide.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyGuide.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHexColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyHexColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHighlightWords.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyHighlightWords.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyIdle.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyIdle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyImagePaste.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyImagePaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyInViewport.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyInViewport.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyJsonViewer.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyJsonViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyKeyPress.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyKeyPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLazyLoad.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLazyLoad.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenPaste.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenPaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenScroll.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenUnload.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyListenUnload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocalStorage.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLocalStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocation.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyLocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMotion.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyMotion.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMousePosition.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyMousePosition.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyPopout.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyPopout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyQRCode.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyQRCode.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRawHTML.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyRawHTML.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyReload.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyReload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResizable.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyResizable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResponsive.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyResponsive.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRgbColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyRgbColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScroll.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScrollbars.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyScrollbars.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySessionStorage.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySessionStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySetTitle.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySetTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShadowDom.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyShadowDom.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShortcutPanel.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyShortcutPanel.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortable.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableContainer.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableContainer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableItem.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableList.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySortableList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplit.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySplit.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplitPane.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySplitPane.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySticky.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferySticky.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyStyle.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyStyle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTimeout.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTimeout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTopProgress.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTopProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTwitterColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyTwitterColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyUnmount.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyUnmount.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyVirtualList.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyVirtualList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWebSocket.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWebSocket.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWheelColorPicker.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWheelColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWindowSize.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/FefferyWindowSize.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/__init__.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/_imports_.py` & `feffery_utils_components-0.2.0a5/feffery_utils_components/_imports_.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from .FefferyKeyPress import FefferyKeyPress
 from .FefferyListenPaste import FefferyListenPaste
 from .FefferyListenScroll import FefferyListenScroll
 from .FefferyListenUnload import FefferyListenUnload
 from .FefferyLocation import FefferyLocation
 from .FefferyMousePosition import FefferyMousePosition
 from .FefferyResponsive import FefferyResponsive
+from .FefferyTextSelection import FefferyTextSelection
 from .FefferyWindowSize import FefferyWindowSize
 from .FefferyResizable import FefferyResizable
 from .FefferySortableList import FefferySortableList
 from .FefferySplit import FefferySplit
 from .FefferySplitPane import FefferySplitPane
 from .FefferyCookie import FefferyCookie
 from .FefferyLocalStorage import FefferyLocalStorage
@@ -118,14 +119,15 @@
     "FefferyKeyPress",
     "FefferyListenPaste",
     "FefferyListenScroll",
     "FefferyListenUnload",
     "FefferyLocation",
     "FefferyMousePosition",
     "FefferyResponsive",
+    "FefferyTextSelection",
     "FefferyWindowSize",
     "FefferyResizable",
     "FefferySortableList",
     "FefferySplit",
     "FefferySplitPane",
     "FefferyCookie",
     "FefferyLocalStorage",
```

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/feffery_utils_components.min.js` & `feffery_utils_components-0.2.0a5/feffery_utils_components/feffery_utils_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         return Object.defineProperty(o, "p", {
             get: (e = i().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return e
             })
         }), "undefined" != typeof jsonpScriptSrc && (a = jsonpScriptSrc, jsonpScriptSrc = function(e) {
             var t, n = /\/_dash-component-suites\//.test(i().src),
                 e = a(e);
-            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a4m1688982631"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
+            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a5m1689124743"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
         }), o(o.s = 493)
     }([function(e, t) {
                 e.exports = window.PropTypes
             }, function(e, t) {
                 e.exports = window.React
             }, function(e, t, n) {
                 "use strict";
@@ -7474,32 +7474,32 @@
                                 h(o, i)
                             }(e.sham || i && i.sham) && f(o, "sham", !0), d(n, r, o, e)
                         }
                 }
             }, function(e, t, n) {
                 var r = n(13),
                     o = n(49),
-                    i = n(16),
+                    i = n(17),
                     a = n(84),
                     s = n(47),
                     n = n(171),
                     l = r.Symbol,
                     c = o("wks"),
                     u = n ? l.for || l : l && l.withoutSetter || a;
                 e.exports = function(e) {
                     return i(c, e) || (c[e] = s && i(l, e) ? l[e] : u("Symbol." + e)), c[e]
                 }
-            }, function(e, t, n) {
+            }, , function(e, t, n) {
                 var r = n(6),
                     o = n(39),
                     i = r({}.hasOwnProperty);
                 e.exports = Object.hasOwn || function(e, t) {
                     return i(o(e), t)
                 }
-            }, , function(I, e, t) {
+            }, function(I, e, t) {
                 "use strict";
                 Object.defineProperty(e, "__esModule", {
                     value: !0
                 });
 
                 function n(e) {
                     return a.setUA(e)
@@ -8510,15 +8510,15 @@
                     return null == e
                 }
             }, function(e, t, n) {
                 var r, o, i, a, s = n(176),
                     l = n(13),
                     c = n(20),
                     u = n(67),
-                    f = n(16),
+                    f = n(17),
                     d = n(116),
                     p = n(85),
                     n = n(68),
                     h = l.TypeError,
                     l = l.WeakMap,
                     g = s || d.state ? ((i = d.state || (d.state = new l)).get = i.get, i.has = i.has, i.set = i.set, r = function(e, t) {
                         if (i.has(e)) throw h("Object already initialized");
@@ -11173,15 +11173,15 @@
                         try {
                             return e[t]
                         } catch (e) {}
                     }(e = s(e), a)) ? t : l ? i(e) : "Object" == (t = i(e)) && o(e.callee) ? "Arguments" : t
                 }
             }, function(e, t, n) {
                 var r = n(25).f,
-                    o = n(16),
+                    o = n(17),
                     i = n(15)("toStringTag");
                 e.exports = function(e, t, n) {
                     (e = e && !n ? e.prototype : e) && !o(e, i) && r(e, i, {
                         configurable: !0,
                         value: t
                     })
                 }
@@ -11996,15 +11996,15 @@
             }, function(e, t, n) {
                 var r = n(22),
                     o = n(19),
                     i = n(114),
                     a = n(62),
                     s = n(40),
                     l = n(82),
-                    c = n(16),
+                    c = n(17),
                     u = n(172),
                     f = Object.getOwnPropertyDescriptor;
                 t.f = r ? f : function(e, t) {
                     if (e = s(e), t = l(t), u) try {
                         return f(e, t)
                     } catch (e) {}
                     if (c(e, t)) return a(!o(i.f, e, t), e[t])
@@ -12054,15 +12054,15 @@
                     o = r.document,
                     i = n(o) && n(o.createElement);
                 e.exports = function(e) {
                     return i ? o.createElement(e) : {}
                 }
             }, function(e, t, n) {
                 var r = n(22),
-                    n = n(16),
+                    n = n(17),
                     o = Function.prototype,
                     i = r && Object.getOwnPropertyDescriptor,
                     n = n(o, "name"),
                     a = n && "something" === function() {}.name,
                     r = n && (!r || i(o, "name").configurable);
                 e.exports = {
                     EXISTS: n,
@@ -12163,15 +12163,15 @@
                     }, "values"), i.Arguments = i.Array);
                 if (o("keys"), o("values"), o("entries"), !u && n && "values" !== a.name) try {
                     s(a, "name", {
                         value: "values"
                     })
                 } catch (e) {}
             }, function(e, t, n) {
-                var r = n(16),
+                var r = n(17),
                     o = n(9),
                     i = n(39),
                     a = n(85),
                     n = n(190),
                     s = a("IE_PROTO"),
                     l = Object,
                     c = l.prototype;
@@ -12202,15 +12202,15 @@
                         }
                     })
                 }
                 var a = n(14),
                     s = n(6),
                     o = n(68),
                     i = n(20),
-                    l = n(16),
+                    l = n(17),
                     c = n(25).f,
                     u = n(86),
                     f = n(196),
                     d = n(308),
                     p = n(84),
                     h = n(194),
                     g = !1,
@@ -14616,15 +14616,15 @@
                         writable: !1
                     }).prototype
                 })
             }, function(e, t, n) {
                 var r = n(6),
                     o = n(7),
                     i = n(9),
-                    a = n(16),
+                    a = n(17),
                     s = n(22),
                     l = n(119).CONFIGURABLE,
                     c = n(175),
                     n = n(42),
                     u = n.enforce,
                     f = n.get,
                     d = String,
@@ -14666,27 +14666,27 @@
                 }), e.exports = n.inspectSource
             }, function(e, t, n) {
                 var r = n(13),
                     n = n(9),
                     r = r.WeakMap;
                 e.exports = n(r) && /native code/.test(String(r))
             }, function(e, t, n) {
-                var l = n(16),
+                var l = n(17),
                     c = n(287),
                     u = n(113),
                     f = n(25);
                 e.exports = function(e, t, n) {
                     for (var r = c(t), o = f.f, i = u.f, a = 0; a < r.length; a++) {
                         var s = r[a];
                         l(e, s) || n && l(n, s) || o(e, s, i(t, s))
                     }
                 }
             }, function(e, t, n) {
                 var r = n(6),
-                    a = n(16),
+                    a = n(17),
                     s = n(40),
                     l = n(288).indexOf,
                     c = n(68),
                     u = r([].push);
                 e.exports = function(e, t) {
                     var n, r = s(e),
                         o = 0,
@@ -15396,15 +15396,15 @@
                 n = n(6);
                 e.exports = n([].slice)
             }, function(e, t, n) {
                 n = n(15);
                 t.f = n
             }, function(e, t, n) {
                 var r = n(459),
-                    o = n(16),
+                    o = n(17),
                     i = n(229),
                     a = n(25).f;
                 e.exports = function(e) {
                     var t = r.Symbol || (r.Symbol = {});
                     o(t, e) || a(t, e, {
                         value: i.f(e)
                     })
@@ -27405,15 +27405,15 @@
                     u = n(128).getWeakData,
                     f = n(199),
                     d = n(21),
                     p = n(41),
                     h = n(20),
                     g = n(197),
                     a = n(124),
-                    b = n(16),
+                    b = n(17),
                     n = n(42),
                     m = n.set,
                     v = n.getterFor,
                     s = a.find,
                     y = a.findIndex,
                     w = i([].splice),
                     _ = 0;
@@ -30324,15 +30324,15 @@
                     }
                 })
             }, function(e, t, n) {
                 "use strict";
                 var r = n(6),
                     o = n(48),
                     i = n(20),
-                    u = n(16),
+                    u = n(17),
                     f = n(228),
                     n = n(61),
                     d = Function,
                     p = r([].concat),
                     h = r([].join),
                     g = {};
                 e.exports = n ? d.bind : function(a) {
@@ -30436,15 +30436,15 @@
                     c = e(13),
                     u = e(19),
                     N = e(6),
                     U = e(66),
                     f = e(22),
                     d = e(47),
                     B = e(7),
-                    p = e(16),
+                    p = e(17),
                     F = e(63),
                     h = e(21),
                     g = e(40),
                     b = e(82),
                     W = e(30),
                     m = e(62),
                     v = e(50),
@@ -30580,15 +30580,15 @@
                     }, {
                         arity: 1
                     })
                 }
             }, function(e, t, n) {
                 var r = n(14),
                     o = n(38),
-                    i = n(16),
+                    i = n(17),
                     a = n(30),
                     s = n(49),
                     n = n(231),
                     l = s("string-to-symbol-registry"),
                     c = s("symbol-to-string-registry");
                 r({
                     target: "Symbol",
@@ -30598,15 +30598,15 @@
                     for: function(e) {
                         var t, e = a(e);
                         return i(l, e) ? l[e] : (t = o("Symbol")(e), l[e] = t, c[t] = e, t)
                     }
                 })
             }, function(e, t, n) {
                 var r = n(14),
-                    o = n(16),
+                    o = n(17),
                     i = n(83),
                     a = n(65),
                     s = n(49),
                     n = n(231),
                     l = s("symbol-to-string-registry");
                 r({
                     target: "Symbol",
@@ -30718,15 +30718,15 @@
                 })
             }, function(e, t, n) {
                 "use strict";
                 var r, o, i, a, s, l, c, u = n(14),
                     f = n(22),
                     d = n(13),
                     p = n(6),
-                    h = n(16),
+                    h = n(17),
                     g = n(9),
                     b = n(63),
                     m = n(30),
                     v = n(130),
                     n = n(177),
                     y = d.Symbol,
                     w = y && y.prototype;
@@ -39663,34 +39663,30 @@
                         unhighlightStyle: f,
                         autoEscape: !s,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
 
                 function gl(e) {
-                    var t, n, r, o = e.id,
-                        i = e.setProps,
-                        e = e.loading_state,
-                        a = (t = Object(L.e)(Object(ze.useState)(function() {
+                    e.id;
+                    var t, n, r = e.setProps,
+                        o = (e.loading_state, e = Object(L.e)(Object(ze.useState)(function() {
                             return jl()
-                        }), 2), n = t[0], r = t[1], Sl("visibilitychange", function() {
-                            r(jl())
+                        }), 2), t = e[0], n = e[1], Sl("visibilitychange", function() {
+                            n(jl())
                         }, {
                             target: function() {
                                 return document
                             }
-                        }), n);
+                        }), t);
                     return Object(ze.useEffect)(function() {
-                        i({
-                            documentVisibility: a
+                        r({
+                            documentVisibility: o
                         })
-                    }, [a]), xe.a.createElement("div", {
-                        id: o,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [o]), xe.a.createElement(xe.a.Fragment, null)
                 }
 
                 function bl(l, c) {
                     var e = Object(L.e)(Object(ze.useState)(l ? "loading" : "unset"), 2),
                         t = e[0],
                         u = e[1],
                         f = Object(ze.useRef)();
@@ -40091,34 +40087,30 @@
                             if (e) throw e.error
                         }
                     }
                     o && (Ml = r)
                 }
 
                 function Ul(e) {
-                    var t, n, r, o = e.id,
-                        i = e.setProps,
-                        e = e.loading_state,
-                        a = (er && !Ll && (Ml = {}, Nl(), window.addEventListener("resize", Il), Ll = !0), t = Object(L.e)(Object(ze.useState)(Ml), 2), n = t[0], r = t[1], Object(ze.useEffect)(function() {
+                    e.id;
+                    var t, n, r = e.setProps,
+                        o = (e.loading_state, er && !Ll && (Ml = {}, Nl(), window.addEventListener("resize", Il), Ll = !0), e = Object(L.e)(Object(ze.useState)(Ml), 2), t = e[0], n = e[1], Object(ze.useEffect)(function() {
                             var e;
                             if (er) return Ll || window.addEventListener("resize", Il), Rl.add(e = function() {
-                                    r(Ml)
+                                    n(Ml)
                                 }),
                                 function() {
                                     Rl.delete(e), 0 === Rl.size && (window.removeEventListener("resize", Il), Ll = !1)
                                 }
-                        }, []), n);
+                        }, []), t);
                     return Object(ze.useEffect)(function() {
-                        i({
-                            responsive: a
+                        r({
+                            responsive: o
                         })
-                    }, [a]), React.createElement("div", {
-                        id: o,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [o]), React.createElement(React.Fragment, null)
                 }
 
                 function Bl(e) {
                     function t(e) {
                         s && a({
                             loading: !1,
                             accuracy: e.coords.accuracy,
@@ -40159,26 +40151,22 @@
                             function() {
                                 s = !1, navigator.geolocation.clearWatch(r)
                             }
                     }, []), i
                 }
 
                 function Fl(e) {
-                    var t = e.id,
-                        n = e.setProps,
-                        e = e.loading_state,
-                        r = Bl();
+                    e.id;
+                    var t = e.setProps,
+                        n = (e.loading_state, Bl());
                     return Object(ze.useEffect)(function() {
-                        n({
-                            geoLocationInfo: r
+                        t({
+                            geoLocationInfo: n
                         })
-                    }, [r]), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [n]), React.createElement(React.Fragment, null)
                 }
                 Ul.propTypes = {
                     id: t.a.string,
                     responsive: t.a.object,
                     setProps: t.a.func,
                     loading_state: t.a.shape({
                         is_loading: t.a.bool,
@@ -40249,68 +40237,60 @@
                                 for (var e = 0; e < m.length; e++) $l(window, m[e], o);
                                 $l(document, "visibilitychange", i)
                             }
                     }, [b, m]), v
                 }
 
                 function Yl(e) {
-                    var t = e.id,
-                        n = e.waitDuration,
-                        r = e.setProps,
-                        e = e.loading_state,
-                        o = ql(n);
+                    e.id;
+                    var t = e.waitDuration,
+                        n = e.setProps,
+                        r = (e.loading_state, ql(t));
                     return Object(ze.useEffect)(function() {
-                        r({
-                            isIdle: o
+                        n({
+                            isIdle: r
                         })
-                    }, [o]), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [r]), React.createElement(React.Fragment, null)
                 }
 
                 function Kl(e) {
                     var t = Object(ze.useRef)(e);
                     t.current = e, Object(ze.useEffect)(function() {
                         return function() {
                             return t.current()
                         }
                     }, [])
                 }
 
                 function Xl(e) {
-                    var t, n, r = e.id,
-                        o = e.setProps,
-                        e = e.loading_state;
-                    void 0 === i && (i = 1 / 0), void 0 === t && (t = 1 / 0), i = Ql({
-                        width: Gl ? window.innerWidth : i,
-                        height: Gl ? window.innerHeight : t
-                    }), t = i[0], n = i[1], Object(ze.useEffect)(function() {
+                    e.id;
+                    var t, n, r, o = e.setProps;
+                    e.loading_state, void 0 === t && (t = 1 / 0), void 0 === n && (n = 1 / 0), t = Ql({
+                        width: Gl ? window.innerWidth : t,
+                        height: Gl ? window.innerHeight : n
+                    }), n = t[0], r = t[1], Object(ze.useEffect)(function() {
                         var e;
                         if (Gl) return e = function() {
-                                n({
+                                r({
                                     width: window.innerWidth,
                                     height: window.innerHeight
                                 })
                             }, Vl(window, "resize", e),
                             function() {
                                 $l(window, "resize", e)
                             }
                     }, []);
-                    var i, a = (i = t).width,
-                        s = i.height;
+                    var i = (e = n).width,
+                        a = e.height;
                     return Object(ze.useEffect)(function() {
                         o({
-                            _width: a,
-                            _height: s
+                            _width: i,
+                            _height: a
                         })
-                    }, [a, s]), React.createElement("div", {
-                        id: r,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [i, a]), React.createElement(React.Fragment, null)
                 }
                 var Gl = "undefined" != typeof window,
                     Jl = ["mousemove", "mousedown", "resize", "keydown", "touchstart", "wheel"],
                     Zl = (Yl.propTypes = {
                         id: t.a.string,
                         isIdle: t.a.bool,
                         waitDuration: t.a.number,
@@ -40561,27 +40541,23 @@
                                 }
                             }
                         }
                     }, [l], c)
                 }
 
                 function sc(e) {
-                    var t = e.id,
-                        n = e.keys,
-                        r = e.pressedCounts,
-                        o = e.setProps,
-                        e = e.loading_state;
-                    return ac(n, function(e) {
-                        e.preventDefault(), o({
-                            pressedCounts: r + 1
+                    e.id;
+                    var t = e.keys,
+                        n = e.pressedCounts,
+                        r = e.setProps;
+                    return e.loading_state, ac(t, function(e) {
+                        e.preventDefault(), r({
+                            pressedCounts: n + 1
                         })
-                    }), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }), React.createElement(React.Fragment, null)
                 }
 
                 function lc(e) {
                     var t, n, r, o, i = e.id,
                         a = e.delay,
                         s = e.timeoutCount,
                         l = e.setProps,
@@ -45062,19 +45038,18 @@
                     }, [a]), React.createElement("div", {
                         id: t,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
 
                 function sp(e) {
-                    var t = e.id,
-                        n = e.setProps,
-                        e = e.loading_state;
-                    return Object(ze.useEffect)(function() {
-                        n({
+                    e.id;
+                    var t = e.setProps;
+                    return e.loading_state, Object(ze.useEffect)(function() {
+                        t({
                             deviceInfo: {
                                 isMobile: cp.isMobile,
                                 isAndroid: cp.isAndroid,
                                 isIOS: cp.isIOS,
                                 isChrome: cp.isChrome,
                                 isFirefox: cp.isFirefox,
                                 isSafari: cp.isSafari,
@@ -45085,18 +45060,15 @@
                                 browserVersion: cp.browserVersion,
                                 fullBrowserVersion: cp.fullBrowserVersion,
                                 browserName: cp.browserName,
                                 ua: cp.getUA,
                                 deviceType: cp.deviceType
                             }
                         })
-                    }, []), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, []), React.createElement(React.Fragment, null)
                 }
                 ap.propTypes = {
                     id: t.a.string,
                     targetId: t.a.string.isRequired,
                     isFullscreen: t.a.bool,
                     loading_state: t.a.shape({
                         is_loading: t.a.bool,
@@ -49822,74 +49794,65 @@
                         scrollSpyOnce: f,
                         separator: d,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
 
                 function Yv(e) {
-                    var t = e.id,
-                        n = e.setProps,
-                        e = e.loading_state;
-                    return Object(ze.useEffect)(function() {
+                    e.id;
+                    var t = e.setProps;
+                    return e.loading_state, Object(ze.useEffect)(function() {
                         function e(e) {
-                            n({
+                            t({
                                 unloaded: !0
                             })
                         }
                         return window.addEventListener("beforeunload", e),
                             function() {
                                 window.removeEventListener("beforeunload", e)
                             }
-                    }, []), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, []), React.createElement(React.Fragment, null)
                 }
 
                 function Kv(e) {
-                    var n, t, r, o, i, a = e.id,
-                        s = e.target,
-                        l = e.setProps,
-                        e = e.loading_state,
-                        c = (n = s ? document.getElementById(s) : document, void 0 === t && (t = function() {
+                    e.id;
+                    var n, t, r, o, i = e.target,
+                        a = e.setProps,
+                        s = (e.loading_state, n = i ? document.getElementById(i) : document, void 0 === t && (t = function() {
                             return !0
-                        }), s = Object(L.e)(Fu(), 2), r = s[0], o = s[1], i = tr(t), ir(function() {
+                        }), e = Object(L.e)(Fu(), 2), i = e[0], r = e[1], o = tr(t), ir(function() {
                             var e, t = N(n, document);
                             if (t) return (e = function() {
                                     var e = t === document ? document.scrollingElement ? {
                                         left: document.scrollingElement.scrollLeft,
                                         top: document.scrollingElement.scrollTop
                                     } : {
                                         left: Math.max(window.pageXOffset, document.documentElement.scrollLeft, document.body.scrollLeft),
                                         top: Math.max(window.pageYOffset, document.documentElement.scrollTop, document.body.scrollTop)
                                     } : {
                                         left: t.scrollLeft,
                                         top: t.scrollTop
                                     };
-                                    i.current(e) && o(e)
+                                    o.current(e) && r(e)
                                 })(), t.addEventListener("scroll", e),
                                 function() {
                                     t.removeEventListener("scroll", e)
                                 }
-                        }, [], n), r);
+                        }, [], n), i);
                     return Object(ze.useEffect)(function() {
-                        c && l({
-                            position: c
+                        s && a({
+                            position: s
                         })
-                    }, [c]), React.createElement("div", {
-                        id: a,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [s]), React.createElement(React.Fragment, null)
                 }
 
                 function Xv(e) {
-                    var t, n, s, r = e.id,
-                        o = e.setProps,
-                        e = e.loading_state,
-                        i = (n = (t = Object(L.e)(Fu(iy), 2))[0], s = t[1], Sl("mousemove", function(e) {
+                    e.id;
+                    var t, s, n = e.setProps,
+                        r = (e.loading_state, t = (e = Object(L.e)(Fu(iy), 2))[0], s = e[1], Sl("mousemove", function(e) {
                             var t, n = e.screenX,
                                 r = e.screenY,
                                 o = e.clientX,
                                 i = e.clientY,
                                 a = e.pageX,
                                 e = e.pageY,
                                 n = {
@@ -49908,57 +49871,50 @@
                                 },
                                 r = N(void 0);
                             r && (i = (o = r.getBoundingClientRect()).left, r = o.top, t = o.width, o = o.height, n.elementPosX = i + window.pageXOffset, n.elementPosY = r + window.pageYOffset, n.elementX = a - n.elementPosX, n.elementY = e - n.elementPosY, n.elementW = t, n.elementH = o), s(n)
                         }, {
                             target: function() {
                                 return document
                             }
-                        }), n);
+                        }), t);
                     return Object(ze.useEffect)(function() {
-                        i && o({
+                        r && n({
                             position: {
-                                screenX: i.screenX,
-                                screenY: i.screenY,
-                                clientX: i.clientX,
-                                clientY: i.clientY,
-                                pageX: i.pageX,
-                                pageY: i.pageY
+                                screenX: r.screenX,
+                                screenY: r.screenY,
+                                clientX: r.clientX,
+                                clientY: r.clientY,
+                                pageX: r.pageX,
+                                pageY: r.pageY
                             }
                         })
-                    }, [i]), React.createElement("div", {
-                        id: r,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [r]), React.createElement(React.Fragment, null)
                 }
 
                 function Gv(e) {
-                    var t = e.id,
-                        n = e.pasteCount,
-                        r = e.enableListenPaste,
-                        o = e.targetContainerId,
-                        i = e.setProps,
-                        e = e.loading_state,
-                        a = Du(function() {
-                            return document.getElementById(o)
-                        }),
-                        s = Object(ze.useCallback)(function(e) {
-                            (r || o && a) && (e = e.clipboardData.getData("text")) && i({
+                    e.id;
+                    var t = e.pasteCount,
+                        n = e.enableListenPaste,
+                        r = e.targetContainerId,
+                        o = e.setProps,
+                        i = (e.loading_state, Du(function() {
+                            return document.getElementById(r)
+                        })),
+                        a = Object(ze.useCallback)(function(e) {
+                            (n || r && i) && (e = e.clipboardData.getData("text")) && o({
                                 pasteText: e,
-                                pasteCount: n + 1
+                                pasteCount: t + 1
                             })
-                        }, [n, r, o, a]);
+                        }, [t, n, r, i]);
                     return Object(ze.useEffect)(function() {
-                        return document.addEventListener("paste", s),
+                        return document.addEventListener("paste", a),
                             function() {
-                                document.removeEventListener("paste", s)
+                                document.removeEventListener("paste", a)
                             }
-                    }, [s]), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [a]), React.createElement(React.Fragment, null)
                 }
 
                 function Jv(r) {
                     var e = window.history,
                         o = e[r];
                     e[r] = function(e) {
                         var t = o.apply(this, arguments),
@@ -49984,34 +49940,30 @@
                         port: r.port,
                         protocol: r.protocol,
                         search: r.search
                     }
                 }
 
                 function Qv(e) {
-                    var t = e.id,
-                        n = e.setProps,
-                        e = e.loading_state,
-                        r = ly();
+                    e.id;
+                    var t = e.setProps,
+                        n = (e.loading_state, ly());
                     return Object(ze.useEffect)(function() {
-                        r && n({
-                            href: r.href,
-                            pathname: r.pathname,
-                            search: r.search,
-                            hash: r.hash,
-                            host: r.host,
-                            hostname: r.hostname,
-                            port: r.port,
-                            protocol: r.protocol,
-                            trigger: r.trigger
+                        n && t({
+                            href: n.href,
+                            pathname: n.pathname,
+                            search: n.search,
+                            hash: n.hash,
+                            host: n.host,
+                            hostname: n.hostname,
+                            port: n.port,
+                            protocol: n.protocol,
+                            trigger: n.trigger
                         })
-                    }, [r]), React.createElement("div", {
-                        id: t,
-                        "data-dash-is-loading": e && e.is_loading || void 0
-                    })
+                    }, [n]), React.createElement(React.Fragment, null)
                 }
                 $v.propTypes = {
                     id: t.a.string,
                     children: t.a.node,
                     style: t.a.object,
                     className: t.a.string,
                     duration: t.a.number,
@@ -54754,15 +54706,122 @@
                             prop_name: t.a.string,
                             component_name: t.a.string
                         }),
                         setProps: t.a.func
                     }, nx.defaultProps = {
                         initialSync: !1
                     }, nx),
-                    ax = (o.d(e, "FefferyCaptcha", function() {
+                    ax = {
+                        top: NaN,
+                        left: NaN,
+                        bottom: NaN,
+                        right: NaN,
+                        height: NaN,
+                        width: NaN
+                    },
+                    sx = Object(L.a)({
+                        text: ""
+                    }, ax);
+
+                function lx(e) {
+                    return (lx = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                        return typeof e
+                    } : function(e) {
+                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                    })(e)
+                }
+
+                function cx(t, e) {
+                    var n, r = Object.keys(t);
+                    return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(t), e && (n = n.filter(function(e) {
+                        return Object.getOwnPropertyDescriptor(t, e).enumerable
+                    })), r.push.apply(r, n)), r
+                }
+
+                function ux(r) {
+                    for (var e = 1; e < arguments.length; e++) {
+                        var o = null != arguments[e] ? arguments[e] : {};
+                        e % 2 ? cx(Object(o), !0).forEach(function(e) {
+                            var t, n;
+                            t = r, e = o[n = e], (n = function() {
+                                var e = function(e) {
+                                    if ("object" !== lx(e) || null === e) return e;
+                                    var t = e[Symbol.toPrimitive];
+                                    if (void 0 === t) return String(e);
+                                    t = t.call(e, "string");
+                                    if ("object" !== lx(t)) return t;
+                                    throw new TypeError("@@toPrimitive must return a primitive value.")
+                                }(n);
+                                return "symbol" === lx(e) ? e : String(e)
+                            }()) in t ? Object.defineProperty(t, n, {
+                                value: e,
+                                enumerable: !0,
+                                configurable: !0,
+                                writable: !0
+                            }) : t[n] = e
+                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(r, Object.getOwnPropertyDescriptors(o)) : cx(Object(o)).forEach(function(e) {
+                            Object.defineProperty(r, e, Object.getOwnPropertyDescriptor(o, e))
+                        })
+                    }
+                    return r
+                }
+
+                function fx(e) {
+                    var r, o, i, a, s, t = e.targetId,
+                        n = e.targetSelector,
+                        l = e.targetType,
+                        c = e.setProps,
+                        u = (r = "selector" === l ? document.querySelector(n) : document.getElementById(t), e = Object(L.e)(Object(ze.useState)(sx), 2), o = e[0], i = e[1], a = Object(ze.useRef)(o), s = Object(ze.useRef)(!1), a.current = o, ir(function() {
+                            var e, t, n = N(r, document);
+                            if (n) return t = function(e) {
+                                    var t;
+                                    window.getSelection && (a.current.text && i(Object(L.a)({}, sx)), s.current = !1, t = window.getSelection()) && (t.removeAllRanges(), s.current = n.contains(e.target))
+                                }, n.addEventListener("mouseup", e = function() {
+                                    var e, t = null,
+                                        n = ax;
+                                    window.getSelection && (e = (t = window.getSelection()) ? t.toString() : "") && s.current && (n = !(t = t) || t.rangeCount < 1 ? ax : {
+                                        height: (t = t.getRangeAt(0).getBoundingClientRect()).height,
+                                        width: t.width,
+                                        top: t.top,
+                                        left: t.left,
+                                        right: t.right,
+                                        bottom: t.bottom
+                                    }, i(Object(L.a)(Object(L.a)(Object(L.a)({}, o), {
+                                        text: e
+                                    }), n)))
+                                }), document.addEventListener("mousedown", t),
+                                function() {
+                                    n.removeEventListener("mouseup", e), document.removeEventListener("mousedown", t)
+                                }
+                        }, [], r), o);
+                    return Object(ze.useEffect)(function() {
+                        null != u && u.text && c({
+                            selectedTextInfo: ux({
+                                timestamp: Date.now()
+                            }, u)
+                        })
+                    }, [u]), xe.a.createElement(xe.a.Fragment, null)
+                }
+                fx.propTypes = {
+                    id: t.a.string,
+                    targetId: t.a.string,
+                    targetSelector: t.a.string,
+                    targetType: t.a.oneOf(["id", "selector"]),
+                    selectedTextInfo: t.a.object,
+                    setProps: t.a.func,
+                    loading_state: t.a.shape({
+                        is_loading: t.a.bool,
+                        prop_name: t.a.string,
+                        component_name: t.a.string
+                    })
+                }, fx.defaultProps = {
+                    targetType: "id"
+                };
+                var dx = xe.a.memo(fx),
+                    px = (o.d(e, "FefferyCaptcha", function() {
                         return A
                     }), o.d(e, "FefferyTopProgress", function() {
                         return G
                     }), o.d(e, "FefferyShortcutPanel", function() {
                         return J.a
                     }), o.d(e, "FefferyGuide", function() {
                         return Z.a
@@ -54884,22 +54943,24 @@
                         return Uy
                     }), o.d(e, "FefferyCompareSlider", function() {
                         return o1
                     }), o.d(e, "FefferySortableList", function() {
                         return ox
                     }), o.d(e, "FefferyLocalStorage", function() {
                         return ix
+                    }), o.d(e, "FefferyTextSelection", function() {
+                        return dx
                     }), sessionStorage.setItem),
-                    sx = (sessionStorage.setItem = function(e, t) {
-                        ax.apply(this, [e, t]);
+                    hx = (sessionStorage.setItem = function(e, t) {
+                        px.apply(this, [e, t]);
                         var n = new Event("sessionStorageSetItem");
                         n.triggerKey = e, n[e] = t, window.dispatchEvent(n)
                     }, localStorage.setItem);
                 localStorage.setItem = function(e, t) {
-                    sx.apply(this, [e, t]);
+                    hx.apply(this, [e, t]);
                     var n = new Event("localStorageSetItem");
                     n.triggerKey = e, n[e] = t, window.dispatchEvent(n)
                 }
             }, function(I, L, e) {
                 "use strict";
                 const o = window,
                     N = o.ShadowRoot && (void 0 === o.ShadyCSS || o.ShadyCSS.nativeShadow) && "adoptedStyleSheets" in Document.prototype && "replace" in CSSStyleSheet.prototype,
```

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/metadata.json` & `feffery_utils_components-0.2.0a5/feffery_utils_components/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9848484848484849%*

 * *Differences: {"'src/lib/components/listeners/FefferyTextSelection.react.js'": "OrderedDict([('description', "*

 * *                                                                 "''), ('displayName', "*

 * *                                                                 "'FefferyTextSelection'), "*

 * *                                                                 "('methods', []), ('props', "*

 * *                                                                 "OrderedDict([('id', "*

 * *                                                   […]*

```diff
@@ -7233,14 +7233,101 @@
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             }
         }
     },
+    "src/lib/components/listeners/FefferyTextSelection.react.js": {
+        "description": "",
+        "displayName": "FefferyTextSelection",
+        "methods": [],
+        "props": {
+            "id": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "loading_state": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "shape",
+                    "value": {
+                        "component_name": {
+                            "description": "Holds the name of the component that is loading",
+                            "name": "string",
+                            "required": false
+                        },
+                        "is_loading": {
+                            "description": "Determines if the component is loading or not",
+                            "name": "bool",
+                            "required": false
+                        },
+                        "prop_name": {
+                            "description": "Holds which property is loading",
+                            "name": "string",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "selectedTextInfo": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "setProps": {
+                "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "targetId": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "targetSelector": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "targetType": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'id'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'id'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'selector'"
+                        }
+                    ]
+                }
+            }
+        }
+    },
     "src/lib/components/listeners/FefferyWindowSize.react.js": {
         "description": "",
         "displayName": "FefferyWindowSize",
         "methods": [],
         "props": {
             "_height": {
                 "description": "",
```

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components/package-info.json` & `feffery_utils_components-0.2.0a5/feffery_utils_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652482269503546%*

 * *Differences: {"'dependencies'": "{delete: ['react-popout', 'react-popout-v2']}", "'version'": "'0.2.0-a5'"}*

```diff
@@ -42,16 +42,14 @@
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
         "react-lazy-load": "^3.1.14",
-        "react-popout": "^3.0.0",
-        "react-popout-v2": "^0.0.8",
         "react-resize-detector": "^7.1.2",
         "react-scroll": "^1.8.6",
         "react-shadow": "^19.0.3",
         "react-spinners-kit": "^1.9.1",
         "react-split": "^2.0.14",
         "react-stickynode": "^4.1.0",
         "react-syntax-highlighter": "^15.4.4",
@@ -115,9 +113,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a4"
+    "version": "0.2.0-a5"
 }
```

### Comparing `feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/SOURCES.txt` & `feffery_utils_components-0.2.0a5/feffery_utils_components.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 feffery_utils_components/FefferySortableContainer.py
 feffery_utils_components/FefferySortableItem.py
 feffery_utils_components/FefferySortableList.py
 feffery_utils_components/FefferySplit.py
 feffery_utils_components/FefferySplitPane.py
 feffery_utils_components/FefferySticky.py
 feffery_utils_components/FefferyStyle.py
+feffery_utils_components/FefferyTextSelection.py
 feffery_utils_components/FefferyTimeout.py
 feffery_utils_components/FefferyTopProgress.py
 feffery_utils_components/FefferyTwitterColorPicker.py
 feffery_utils_components/FefferyUnmount.py
 feffery_utils_components/FefferyVirtualList.py
 feffery_utils_components/FefferyWebSocket.py
 feffery_utils_components/FefferyWheelColorPicker.py
```

### Comparing `feffery_utils_components-0.2.0a4/package.json` & `feffery_utils_components-0.2.0a5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652482269503546%*

 * *Differences: {"'dependencies'": "{delete: ['react-popout', 'react-popout-v2']}", "'version'": "'0.2.0-a5'"}*

```diff
@@ -42,16 +42,14 @@
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
         "react-lazy-load": "^3.1.14",
-        "react-popout": "^3.0.0",
-        "react-popout-v2": "^0.0.8",
         "react-resize-detector": "^7.1.2",
         "react-scroll": "^1.8.6",
         "react-shadow": "^19.0.3",
         "react-spinners-kit": "^1.9.1",
         "react-split": "^2.0.14",
         "react-stickynode": "^4.1.0",
         "react-syntax-highlighter": "^15.4.4",
@@ -115,9 +113,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a4"
+    "version": "0.2.0-a5"
 }
```

### Comparing `feffery_utils_components-0.2.0a4/setup.py` & `feffery_utils_components-0.2.0a5/setup.py`

 * *Files identical despite different names*

