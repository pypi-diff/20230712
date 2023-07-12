# Comparing `tmp/pyobs_gui-1.0.5.tar.gz` & `tmp/pyobs_gui-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_gui-1.0.5.tar", max compression
+gzip compressed data, was "pyobs_gui-1.0.6.tar", max compression
```

## Comparing `pyobs_gui-1.0.5.tar` & `pyobs_gui-1.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1099 2023-03-22 08:29:56.452652 pyobs_gui-1.0.5/LICENSE
--rw-r--r--   0        0        0      423 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/__init__.py
--rw-r--r--   0        0        0     9536 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/base.py
--rw-r--r--   0        0        0    14007 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/camerawidget.py
--rw-r--r--   0        0        0     1678 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/commandinputwidget.py
--rw-r--r--   0        0        0     2984 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/compassmovewidget.py
--rw-r--r--   0        0        0     2218 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/coolingwidget.py
--rw-r--r--   0        0        0     8626 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/datadisplaywidget.py
--rw-r--r--   0        0        0     6635 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/eventswidget.py
--rw-r--r--   0        0        0     4396 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/filterwidget.py
--rw-r--r--   0        0        0     2429 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/fitsheaderswidget.py
--rw-r--r--   0        0        0     5370 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/focuswidget.py
--rw-r--r--   0        0        0     2763 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/gui.py
--rw-r--r--   0        0        0     2945 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/logmodel.py
--rw-r--r--   0        0        0    14676 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/mainwindow.py
--rw-r--r--   0        0        0     3076 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/modulegui.py
--rw-r--r--   0        0        0        0 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/__init__.py
--rw-r--r--   0        0        0    42397 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/camerawidget.ui
--rw-r--r--   0        0        0    31606 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/camerawidget_ui.py
--rw-r--r--   0        0        0      928 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/compassmoveplugin.py
--rw-r--r--   0        0        0      227 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/compassmovewidget.py
--rw-r--r--   0        0        0     2553 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/compassmovewidget.ui
--rw-r--r--   0        0        0     3229 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/compassmovewidget_ui.py
--rwxr-xr-x   0        0        0      256 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/compile.sh
--rw-r--r--   0        0        0     3547 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/coolingwidget.ui
--rw-r--r--   0        0        0     3925 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/coolingwidget_ui.py
--rw-r--r--   0        0        0      928 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/datadisplayplugin.py
--rw-r--r--   0        0        0      227 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/datadisplaywidget.py
--rw-r--r--   0        0        0     4129 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/datadisplaywidget.ui
--rw-r--r--   0        0        0     4705 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/datadisplaywidget_ui.py
--rwxr-xr-x   0        0        0       43 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/designer.sh
--rw-r--r--   0        0        0     2509 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/eventswidget.ui
--rw-r--r--   0        0        0     2639 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/eventswidget_ui.py
--rw-r--r--   0        0        0     2305 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/filterwidget.ui
--rw-r--r--   0        0        0     2983 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/filterwidget_ui.py
--rw-r--r--   0        0        0     3165 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/fitsheaderswidget.ui
--rw-r--r--   0        0        0     4440 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/fitsheaderswidget_ui.py
--rw-r--r--   0        0        0     5796 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/focuswidget.ui
--rw-r--r--   0        0        0     7130 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/focuswidget_ui.py
--rw-r--r--   0        0        0    10262 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/mainwindow.py
--rw-r--r--   0        0        0    12065 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/mainwindow.ui
--rw-r--r--   0        0        0      502 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-alt-circle-down-solid.svg
--rw-r--r--   0        0        0      503 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-alt-circle-left-solid.svg
--rw-r--r--   0        0        0      499 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-alt-circle-right-solid.svg
--rw-r--r--   0        0        0      493 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-alt-circle-up-solid.svg
--rw-r--r--   0        0        0      892 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg
--rw-r--r--   0        0        0     1640 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrows-to-eye-solid.svg
--rw-r--r--   0        0        0      720 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/chart-line-solid.svg
--rw-r--r--   0        0        0      681 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/circle-question-solid.svg
--rw-r--r--   0        0        0     1283 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/cloud-sun-solid.svg
--rw-r--r--   0        0        0      735 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/edit-solid.svg
--rw-r--r--   0        0        0      577 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/search-solid.svg
--rw-r--r--   0        0        0      767 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources/undo-solid.svg
--rw-r--r--   0        0        0      528 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources.qrc
--rw-r--r--   0        0        0    28297 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/resources_rc.py
--rw-r--r--   0        0        0    45953 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/roofwidget.ui
--rw-r--r--   0        0        0    30193 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/roofwidget_ui.py
--rw-r--r--   0        0        0      915 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/shellwidget.ui
--rw-r--r--   0        0        0     1326 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/shellwidget_ui.py
--rw-r--r--   0        0        0    34768 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/spectrographwidget.ui
--rw-r--r--   0        0        0    23247 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/spectrographwidget_ui.py
--rw-r--r--   0        0        0    57305 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/telescopewidget.ui
--rw-r--r--   0        0        0    52536 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/telescopewidget_ui.py
--rw-r--r--   0        0        0     1917 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/temperaturesplotwidget.ui
--rw-r--r--   0        0        0     2769 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/temperaturesplotwidget_ui.py
--rw-r--r--   0        0        0     2114 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/temperatureswidget.ui
--rw-r--r--   0        0        0     2612 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/temperatureswidget_ui.py
--rw-r--r--   0        0        0    40308 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/videowidget.ui
--rw-r--r--   0        0        0    25634 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/videowidget_ui.py
--rw-r--r--   0        0        0     1511 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/weatherwidget.ui
--rw-r--r--   0        0        0     2290 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/qt/weatherwidget_ui.py
--rw-r--r--   0        0        0     2075 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/roofwidget.py
--rw-r--r--   0        0        0    12366 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/shellwidget.py
--rw-r--r--   0        0        0     5375 2023-03-22 08:29:56.456652 pyobs_gui-1.0.5/pyobs_gui/spectrographwidget.py
--rw-r--r--   0        0        0     6592 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/statuswidget.py
--rw-r--r--   0        0        0    26202 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/telescopewidget.py
--rw-r--r--   0        0        0     3382 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/temperaturesplotwidget.py
--rw-r--r--   0        0        0     2577 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/temperatureswidget.py
--rw-r--r--   0        0        0     2255 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/utils.py
--rw-r--r--   0        0        0     8063 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/videowidget.py
--rwxr-xr-x   0        0        0     2419 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/visplot.py
--rw-r--r--   0        0        0     5531 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyobs_gui/weatherwidget.py
--rw-r--r--   0        0        0      647 2023-03-22 08:29:56.460652 pyobs_gui-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 pyobs_gui-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-12 07:41:28.344539 pyobs_gui-1.0.6/LICENSE
+-rw-r--r--   0        0        0      423 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/__init__.py
+-rw-r--r--   0        0        0    10966 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/base.py
+-rw-r--r--   0        0        0    14024 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/camerawidget.py
+-rw-r--r--   0        0        0     1678 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/commandinputwidget.py
+-rw-r--r--   0        0        0     2984 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/compassmovewidget.py
+-rw-r--r--   0        0        0     2218 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/coolingwidget.py
+-rw-r--r--   0        0        0     8641 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/datadisplaywidget.py
+-rw-r--r--   0        0        0     6650 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/eventswidget.py
+-rw-r--r--   0        0        0     4405 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/filterwidget.py
+-rw-r--r--   0        0        0     2429 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/fitsheaderswidget.py
+-rw-r--r--   0        0        0     5385 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/focuswidget.py
+-rw-r--r--   0        0        0     2763 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/gui.py
+-rw-r--r--   0        0        0     2945 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/logmodel.py
+-rw-r--r--   0        0        0    15631 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/mainwindow.py
+-rw-r--r--   0        0        0     3079 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/modulegui.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/__init__.py
+-rw-r--r--   0        0        0    42397 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/camerawidget.ui
+-rw-r--r--   0        0        0    31606 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/camerawidget_ui.py
+-rw-r--r--   0        0        0      928 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/compassmoveplugin.py
+-rw-r--r--   0        0        0      227 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/compassmovewidget.py
+-rw-r--r--   0        0        0     2553 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/compassmovewidget.ui
+-rw-r--r--   0        0        0     3229 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/compassmovewidget_ui.py
+-rwxr-xr-x   0        0        0      256 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/compile.sh
+-rw-r--r--   0        0        0     3547 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/coolingwidget.ui
+-rw-r--r--   0        0        0     3925 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/coolingwidget_ui.py
+-rw-r--r--   0        0        0      928 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/datadisplayplugin.py
+-rw-r--r--   0        0        0      227 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/datadisplaywidget.py
+-rw-r--r--   0        0        0     4129 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/datadisplaywidget.ui
+-rw-r--r--   0        0        0     4705 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/datadisplaywidget_ui.py
+-rwxr-xr-x   0        0        0       43 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/designer.sh
+-rw-r--r--   0        0        0     2509 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/eventswidget.ui
+-rw-r--r--   0        0        0     2639 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/eventswidget_ui.py
+-rw-r--r--   0        0        0     2305 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/filterwidget.ui
+-rw-r--r--   0        0        0     2983 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/filterwidget_ui.py
+-rw-r--r--   0        0        0     3165 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/fitsheaderswidget.ui
+-rw-r--r--   0        0        0     4440 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/fitsheaderswidget_ui.py
+-rw-r--r--   0        0        0     5796 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/focuswidget.ui
+-rw-r--r--   0        0        0     7130 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/focuswidget_ui.py
+-rw-r--r--   0        0        0    10262 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/mainwindow.py
+-rw-r--r--   0        0        0    12065 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/mainwindow.ui
+-rw-r--r--   0        0        0      502 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-alt-circle-down-solid.svg
+-rw-r--r--   0        0        0      503 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-alt-circle-left-solid.svg
+-rw-r--r--   0        0        0      499 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-alt-circle-right-solid.svg
+-rw-r--r--   0        0        0      493 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-alt-circle-up-solid.svg
+-rw-r--r--   0        0        0      892 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg
+-rw-r--r--   0        0        0     1640 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrows-to-eye-solid.svg
+-rw-r--r--   0        0        0      720 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/chart-line-solid.svg
+-rw-r--r--   0        0        0      681 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/circle-question-solid.svg
+-rw-r--r--   0        0        0     1283 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/cloud-sun-solid.svg
+-rw-r--r--   0        0        0      735 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/edit-solid.svg
+-rw-r--r--   0        0        0      577 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/search-solid.svg
+-rw-r--r--   0        0        0      767 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources/undo-solid.svg
+-rw-r--r--   0        0        0      528 2023-07-12 07:41:28.348539 pyobs_gui-1.0.6/pyobs_gui/qt/resources.qrc
+-rw-r--r--   0        0        0    28297 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/resources_rc.py
+-rw-r--r--   0        0        0    45953 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/roofwidget.ui
+-rw-r--r--   0        0        0    30193 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/roofwidget_ui.py
+-rw-r--r--   0        0        0      915 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/shellwidget.ui
+-rw-r--r--   0        0        0     1326 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/shellwidget_ui.py
+-rw-r--r--   0        0        0    34768 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/spectrographwidget.ui
+-rw-r--r--   0        0        0    23247 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/spectrographwidget_ui.py
+-rw-r--r--   0        0        0    60514 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/telescopewidget.ui
+-rw-r--r--   0        0        0    55903 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/telescopewidget_ui.py
+-rw-r--r--   0        0        0     1917 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/temperaturesplotwidget.ui
+-rw-r--r--   0        0        0     2769 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/temperaturesplotwidget_ui.py
+-rw-r--r--   0        0        0     2114 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/temperatureswidget.ui
+-rw-r--r--   0        0        0     2612 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/temperatureswidget_ui.py
+-rw-r--r--   0        0        0    40308 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/videowidget.ui
+-rw-r--r--   0        0        0    25634 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/videowidget_ui.py
+-rw-r--r--   0        0        0     1511 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/weatherwidget.ui
+-rw-r--r--   0        0        0     2290 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/qt/weatherwidget_ui.py
+-rw-r--r--   0        0        0     2075 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/roofwidget.py
+-rw-r--r--   0        0        0    12375 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/shellwidget.py
+-rw-r--r--   0        0        0     5392 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/spectrographwidget.py
+-rw-r--r--   0        0        0     6608 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/statuswidget.py
+-rw-r--r--   0        0        0    27476 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/telescopewidget.py
+-rw-r--r--   0        0        0     3350 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/temperaturesplotwidget.py
+-rw-r--r--   0        0        0     2577 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/temperatureswidget.py
+-rw-r--r--   0        0        0     2255 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/utils.py
+-rw-r--r--   0        0        0     8080 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/videowidget.py
+-rwxr-xr-x   0        0        0     2419 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/visplot.py
+-rw-r--r--   0        0        0     5531 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyobs_gui/weatherwidget.py
+-rw-r--r--   0        0        0      681 2023-07-12 07:41:28.352539 pyobs_gui-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 pyobs_gui-1.0.6/PKG-INFO
```

### Comparing `pyobs_gui-1.0.5/LICENSE` & `pyobs_gui-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/base.py` & `pyobs_gui-1.0.6/pyobs_gui/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,20 +30,66 @@
 
 WidgetClass = TypeVar("WidgetClass")
 
 
 class BaseWindow:
     def __init__(self) -> None:
         """Base class for MainWindow and all widgets."""
-        self.module: Optional[Proxy] = None
+        self.modules: List[Proxy] = []
         self.comm: Optional[Comm] = None
         self.observer: Optional[Observer] = None
         self.vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None
         self._base_widgets: List[BaseWidget] = []
 
+    @property
+    def module(self) -> Optional[Proxy]:
+        """Returns the first module in the list or None, if list is empty"""
+        return self.modules[0] if len(self.modules) > 0 else None
+
+    def module_by_name(self, name: str) -> Optional[Proxy]:
+        """Return the module with the given name or None, if not exists.
+
+        Args:
+            name: Name of module to return.
+
+        Returns:
+            Module or None.
+        """
+
+        # loop all modules and check name
+        for module in self.modules:
+            if module.name == name:
+                return module
+
+        # nothing found
+        return None
+
+    def modules_by_interface(self, interface: Any) -> List[Proxy]:
+        """Returns all modules that implement the given interface.
+
+        Args:
+            interface: Interface that modules must implement.
+
+        Returns:
+            List of modules.
+        """
+        return list(filter(lambda m: isinstance(m, interface), self.modules))
+
+    def module_by_interface(self, interface: Any) -> Optional[Proxy]:
+        """Returns first modules that implement the given interface, or None, if no exist.
+
+        Args:
+            interface: Interface that module must implement.
+
+        Returns:
+            Module or None.
+        """
+        modules = self.modules_by_interface(interface)
+        return None if len(modules) == 0 else modules[0]
+
     def create_widget(self, config: Union[Dict[str, Any], type], **kwargs: Any) -> "BaseWidget":
         """Creates new widget.
 
         Args:
             config: Config to create widget from.
 
         Returns:
@@ -63,31 +109,31 @@
             self._base_widgets.append(widget)
             return widget
         else:
             raise ValueError("Invalid widget.")
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         # store
-        self.module = module
+        self.modules = [] if modules is None else modules
         self.vfs = vfs
         self.comm = comm
         self.observer = observer
 
         """Open all widgets."""
         for widget in self._base_widgets:
             await self._open_child(widget)
 
     async def _open_child(self, widget: BaseWidget):
-        await widget.open(module=self.module, vfs=self.vfs, comm=self.comm, observer=self.observer)
+        await widget.open(modules=self.modules, vfs=self.vfs, comm=self.comm, observer=self.observer)
 
 
 class BaseWidget(BaseWindow):
     _show_error = QtCore.pyqtSignal(str)
     _enable_buttons = QtCore.pyqtSignal(list, bool)
 
     def __init__(
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/camerawidget.py` & `pyobs_gui-1.0.6/pyobs_gui/camerawidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import logging
 import os
-from typing import Any, Optional, Union, Dict
+from typing import Any, Optional, Union, Dict, List
 from PyQt5 import QtWidgets, QtCore
 from astroplan import Observer
 
 from pyobs.comm import Proxy, Comm
 from pyobs.events import ExposureStatusChangedEvent, NewImageEvent, Event
 from pyobs.interfaces import (
     IAbortable,
@@ -49,22 +49,22 @@
         self.exposure_status = ExposureStatus.IDLE
         self.exposures_left = 0
         self.exposure_time_left = 0.0
         self.exposure_progress = 0.0
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
-        await self.datadisplay.open(module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
+        await self.datadisplay.open(modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # set exposure types
         image_types = sorted([it.name for it in ImageType])
         self.comboImageType.addItems(image_types)
 
         # before first update, disable mys
         self.setEnabled(False)
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/commandinputwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/commandinputwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/compassmovewidget.py` & `pyobs_gui-1.0.6/pyobs_gui/compassmovewidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/coolingwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/coolingwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/datadisplaywidget.py` & `pyobs_gui-1.0.6/pyobs_gui/datadisplaywidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-from typing import Any, Optional, cast, Union, Dict
+from typing import Any, Optional, cast, Union, Dict, List
 import numpy as np
 from PyQt5 import QtWidgets, QtCore
 from astroplan import Observer
 from astropy.io import fits
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
@@ -51,21 +51,21 @@
 
         # connect signals
         self.signal_update_gui.connect(self.update_gui)
         self.checkAutoSave.stateChanged.connect(lambda x: self.textAutoSavePath.setEnabled(x))
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # add image panel
         self.imageLayout = QtWidgets.QVBoxLayout(self.tabImage)
         if isinstance(self.module, ISpectrograph):
             self.figure, self.ax = plt.subplots()
             self.canvas = FigureCanvas(self.figure)
             self.plotTools = NavigationToolbar2QT(self.canvas, self.tabImage)
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/eventswidget.py` & `pyobs_gui-1.0.6/pyobs_gui/eventswidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from datetime import datetime
 from enum import Enum, EnumMeta
-from typing import Any, Type, Dict, Optional, Union, get_origin, get_args
+from typing import Any, Type, Dict, Optional, Union, get_origin, get_args, List
 from PyQt5 import QtWidgets, QtCore
 import inspect
 
 from astroplan import Observer
 
 import pyobs.events
 from pyobs.comm import Comm, Proxy
@@ -26,21 +26,21 @@
         self.tableEvents.setHorizontalHeaderLabels(["Time", "Sender", "Event", "Data"])
         self.tableEvents.setColumnWidth(0, 80)
         self.tableEvents.setColumnWidth(1, 100)
         self.tableEvents.setColumnWidth(2, 200)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # loop all event types
         for name, cls in pyobs.events.__dict__.items():
             if isinstance(cls, type):
                 # register event
                 await self.comm.register_event(cls, self._handle_event)
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/filterwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/filterwidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         self.signal_update_gui.connect(self.update_gui)
 
         # button colors
         self.colorize_button(self.buttonSetFilter, QtCore.Qt.green)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # subscribe to events
         await self.comm.register_event(FilterChangedEvent, self._on_filter_changed)
         await self.comm.register_event(MotionStatusChangedEvent, self._on_motion_status_changed)
 
     async def _init(self) -> None:
         # get current filter
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/fitsheaderswidget.py` & `pyobs_gui-1.0.6/pyobs_gui/fitsheaderswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/focuswidget.py` & `pyobs_gui-1.0.6/pyobs_gui/focuswidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Optional, Union, Dict
+from typing import Any, Optional, Union, Dict, List
 
 from PyQt5 import QtWidgets, QtCore
 from astroplan import Observer
 
 from pyobs.comm import Proxy, Comm
 from pyobs.events import MotionStatusChangedEvent, Event
 from pyobs.interfaces import IFocuser
@@ -39,21 +39,21 @@
         # button colors
         self.colorize_button(self.butSetFocusBase, QtCore.Qt.green)
         self.colorize_button(self.butSetFocusOffset, QtCore.Qt.green)
         self.colorize_button(self.buttonResetFocusOffset, QtCore.Qt.yellow)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # subscribe to events
         if self.comm is not None:
             await self.comm.register_event(MotionStatusChangedEvent, self._on_motion_status_changed)
 
     def _set_focus(self, offset: bool = False) -> None:
         """Asks user for new focus (offset) and sets it.
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/gui.py` & `pyobs_gui-1.0.6/pyobs_gui/gui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/logmodel.py` & `pyobs_gui-1.0.6/pyobs_gui/logmodel.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/mainwindow.py` & `pyobs_gui-1.0.6/pyobs_gui/mainwindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,29 @@
     IWeather: "fa5s.cloud-sun",
     IVideo: "fa5s.video",
     ISpectrograph: "ei.graph",
     IFilters: "ei.graph",
 }
 
 
+DEFAULT_CONFIG = [
+    {"widget": ShellWidget, "label": "Shell", "always": True},
+    {"widget": EventsWidget, "label": "Events", "always": True},
+    {"widget": StatusWidget, "label": "Status", "always": True},
+    {"widget": CameraWidget, "interfaces": "ICamera", "icon": "fa5s.camera"},
+    {"widget": TelescopeWidget, "interfaces": "ITelescope", "icon": "msc.telescope"},
+    {"widget": RoofWidget, "interfaces": "IRoof", "icon": "ph.house"},
+    {"widget": FocusWidget, "interfaces": "IFocuser", "icon": "mdi.image-filter-center-focus"},
+    {"widget": WeatherWidget, "interfaces": "IWeather", "icon": "fa5s.cloud-sun"},
+    {"widget": VideoWidget, "interfaces": "IVideo", "icon": "fa5s.video"},
+    {"widget": SpectrographWidget, "interfaces": "ISpectrograph", "icon": "ei.graph"},
+    {"widget": FilterWidget, "interfaces": "IFilters", "icon": "mdi.air-filter"},
+]
+
+
 class PagesListWidgetItem(QtWidgets.QListWidgetItem):
     """ListWidgetItem for the pages list. Always sorts Shell and Events first"""
 
     def __lt__(self, other: QtWidgets.QListWidgetItem) -> bool:
         """Compare two items."""
 
         # special cases
@@ -148,16 +163,19 @@
         self.shell: Optional[ShellWidget] = None
         self.events: Optional[EventsWidget] = None
         self.status: Optional[StatusWidget] = None
 
     async def open(self, **kwargs: Any) -> None:
         """Open module."""
 
+        # get module
+        module = kwargs.pop("module")
+
         # open widgets
-        await BaseWindow.open(self, **kwargs)
+        await BaseWindow.open(self, modules=[module], **kwargs)
 
         # shell
         if self.show_shell:
             # add shell nav button and view
             self.shell = self.create_widget(ShellWidget)
             await self._add_client("Shell", qta.icon("msc.terminal-powershell"), self.shell, None)
         else:
@@ -225,15 +243,15 @@
         item.setSizeHint(QtCore.QSize(80, 80))
 
         # add to list and sort
         self.listPages.addItem(item)
         self.listPages.sortItems()
 
         # open and add widget
-        await widget.open(module=proxy, comm=self.comm, observer=self.observer, vfs=self.vfs)
+        await widget.open(modules=[proxy], comm=self.comm, observer=self.observer, vfs=self.vfs)
         self.stackedWidget.addWidget(widget)
 
         # store
         self._widgets[client] = widget
 
     def _change_page(self, idx: int) -> None:
         """Change page.
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/modulegui.py` & `pyobs_gui-1.0.6/pyobs_gui/modulegui.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         for interface, klass in DEFAULT_WIDGETS.items():
             if isinstance(module, interface):
                 widget = self.create_widget(klass)
                 self.setCentralWidget(widget)
                 break
 
         # open widgets
-        await BaseWindow.open(self, module=module, **kwargs)
+        await BaseWindow.open(self, modules=[module], **kwargs)
 
     def closeEvent(self, a0: QtGui.QCloseEvent) -> None:
         self.gui_module.quit()
 
 
 class ModuleGUI(Module, IFitsHeaderBefore):
     __module__ = "pyobs_gui"
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/camerawidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/camerawidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/camerawidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/camerawidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/compassmoveplugin.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/compassmoveplugin.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/compassmovewidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/compassmovewidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/compassmovewidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/compassmovewidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/coolingwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/coolingwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/coolingwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/coolingwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/datadisplayplugin.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/datadisplayplugin.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/datadisplaywidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/datadisplaywidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/datadisplaywidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/datadisplaywidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/eventswidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/eventswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/eventswidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/eventswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/filterwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/filterwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/filterwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/filterwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/fitsheaderswidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/fitsheaderswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/fitsheaderswidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/fitsheaderswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/focuswidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/focuswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/focuswidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/focuswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/mainwindow.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/mainwindow.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/mainwindow.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/arrows-to-eye-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/arrows-to-eye-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/chart-line-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/chart-line-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/circle-question-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/circle-question-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/cloud-sun-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/cloud-sun-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/edit-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/edit-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/search-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/search-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources/undo-solid.svg` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources/undo-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources.qrc` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources.qrc`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/resources_rc.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/resources_rc.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/roofwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/roofwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/roofwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/roofwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/shellwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/shellwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/shellwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/shellwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/spectrographwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/spectrographwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/spectrographwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/spectrographwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/telescopewidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/telescopewidget.ui`

 * *Files 2% similar despite different names*

#### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/telescopewidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/telescopewidget.ui`

```diff
@@ -624,15 +624,15 @@
                       </palette>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QStackedWidget" name="stackedMove">
                     <property name="currentIndex">
-                      <number>0</number>
+                      <number>3</number>
                     </property>
                     <widget class="QWidget" name="pageMoveEquatorial">
                       <layout class="QVBoxLayout" name="verticalLayout_9">
                         <item>
                           <layout class="QFormLayout" name="formLayout">
                             <item row="1" column="0">
                               <widget class="QLabel" name="label_11">
@@ -981,84 +981,169 @@
                               </size>
                             </property>
                           </spacer>
                         </item>
                       </layout>
                     </widget>
                     <widget class="QWidget" name="pageMoveHelioprojectiveRadial">
-                      <widget class="QWidget" name="widget_5" native="true">
-                        <property name="geometry">
-                          <rect>
-                            <x>10</x>
-                            <y>10</y>
-                            <width>342</width>
-                            <height>44</height>
-                          </rect>
-                        </property>
-                        <layout class="QGridLayout" name="gridLayout_13">
-                          <item row="0" column="2">
-                            <widget class="QLabel" name="label_39">
-                              <property name="text">
-                                <string>Psi:</string>
-                              </property>
-                            </widget>
-                          </item>
-                          <item row="0" column="1">
-                            <widget class="QDoubleSpinBox" name="spinMoveHelioprojectiveRadialMu">
-                              <property name="sizePolicy">
-                                <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
-                                  <horstretch>0</horstretch>
-                                  <verstretch>0</verstretch>
-                                </sizepolicy>
-                              </property>
-                              <property name="suffix">
-                                <string/>
-                              </property>
-                              <property name="minimum">
-                                <double>0.000000000000000</double>
-                              </property>
-                              <property name="maximum">
-                                <double>1.000000000000000</double>
-                              </property>
-                              <property name="singleStep">
-                                <double>0.100000000000000</double>
-                              </property>
-                              <property name="value">
-                                <double>1.000000000000000</double>
-                              </property>
-                            </widget>
-                          </item>
-                          <item row="0" column="0">
-                            <widget class="QLabel" name="label_40">
-                              <property name="text">
-                                <string>Mu:</string>
-                              </property>
-                            </widget>
-                          </item>
-                          <item row="0" column="3">
-                            <widget class="QDoubleSpinBox" name="spinMoveHelioprojectiveRadialPsi">
-                              <property name="sizePolicy">
-                                <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
-                                  <horstretch>0</horstretch>
-                                  <verstretch>0</verstretch>
-                                </sizepolicy>
-                              </property>
-                              <property name="suffix">
-                                <string>°</string>
-                              </property>
-                              <property name="minimum">
-                                <double>0.000000000000000</double>
-                              </property>
-                              <property name="maximum">
-                                <double>359.000000000000000</double>
-                              </property>
-                            </widget>
-                          </item>
-                        </layout>
-                      </widget>
+                      <layout class="QVBoxLayout" name="verticalLayout_10">
+                        <item>
+                          <layout class="QHBoxLayout" name="horizontalLayout_3">
+                            <item>
+                              <widget class="QLabel" name="label_42">
+                                <property name="text">
+                                  <string>Tx</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QSpinBox" name="spinMoveHelioProjectiveRadialTx">
+                                <property name="sizePolicy">
+                                  <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                                    <horstretch>0</horstretch>
+                                    <verstretch>0</verstretch>
+                                  </sizepolicy>
+                                </property>
+                                <property name="suffix">
+                                  <string>&quot;</string>
+                                </property>
+                                <property name="prefix">
+                                  <string/>
+                                </property>
+                                <property name="minimum">
+                                  <number>-9999</number>
+                                </property>
+                                <property name="maximum">
+                                  <number>9999</number>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QLabel" name="label_41">
+                                <property name="text">
+                                  <string>Ty</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QSpinBox" name="spinMoveHelioProjectiveRadialTy">
+                                <property name="sizePolicy">
+                                  <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                                    <horstretch>0</horstretch>
+                                    <verstretch>0</verstretch>
+                                  </sizepolicy>
+                                </property>
+                                <property name="suffix">
+                                  <string>&quot;</string>
+                                </property>
+                                <property name="minimum">
+                                  <number>-9999</number>
+                                </property>
+                                <property name="maximum">
+                                  <number>9999</number>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_7">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>240</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                      </layout>
+                    </widget>
+                    <widget class="QWidget" name="pageMoveHelioprojectiveMuPsi">
+                      <layout class="QVBoxLayout" name="verticalLayout_11">
+                        <item>
+                          <widget class="QWidget" name="widget_5" native="true">
+                            <layout class="QGridLayout" name="gridLayout_13">
+                              <item row="0" column="2">
+                                <widget class="QLabel" name="label_39">
+                                  <property name="text">
+                                    <string>Psi:</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item row="0" column="1">
+                                <widget class="QDoubleSpinBox" name="spinMoveHelioprojectiveRadialMu">
+                                  <property name="sizePolicy">
+                                    <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                                      <horstretch>0</horstretch>
+                                      <verstretch>0</verstretch>
+                                    </sizepolicy>
+                                  </property>
+                                  <property name="suffix">
+                                    <string/>
+                                  </property>
+                                  <property name="minimum">
+                                    <double>0.000000000000000</double>
+                                  </property>
+                                  <property name="maximum">
+                                    <double>1.000000000000000</double>
+                                  </property>
+                                  <property name="singleStep">
+                                    <double>0.100000000000000</double>
+                                  </property>
+                                  <property name="value">
+                                    <double>1.000000000000000</double>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item row="0" column="0">
+                                <widget class="QLabel" name="label_40">
+                                  <property name="text">
+                                    <string>Mu:</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item row="0" column="3">
+                                <widget class="QDoubleSpinBox" name="spinMoveHelioprojectiveRadialPsi">
+                                  <property name="sizePolicy">
+                                    <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                                      <horstretch>0</horstretch>
+                                      <verstretch>0</verstretch>
+                                    </sizepolicy>
+                                  </property>
+                                  <property name="suffix">
+                                    <string>°</string>
+                                  </property>
+                                  <property name="minimum">
+                                    <double>0.000000000000000</double>
+                                  </property>
+                                  <property name="maximum">
+                                    <double>359.000000000000000</double>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_8">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>230</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                      </layout>
                     </widget>
                     <widget class="QWidget" name="pageMoveOrbitElements">
                       <layout class="QGridLayout" name="gridLayout_8">
                         <item row="0" column="0">
                           <layout class="QHBoxLayout" name="horizontalLayout_8">
                             <item>
                               <widget class="QLabel" name="label_21">
@@ -1600,15 +1685,15 @@
                     </layout>
                   </widget>
                 </item>
               </layout>
             </widget>
           </item>
           <item>
-            <widget class="CompassMoveWidget" name="compassmovewidget"/>
+            <widget class="CompassMoveWidget" name="compassmovewidget" native="true"/>
           </item>
           <item>
             <spacer name="verticalSpacer_4">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
               <property name="sizeHint" stdset="0">
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/telescopewidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/telescopewidget_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from ..reading ui file 'telescopewidget.ui'
+# Form implementation generated from reading ui file 'telescopewidget.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.2
+# Created by: PyQt5 UI code generator 5.15.7
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_TelescopeWidget(object):
     def setupUi(self, TelescopeWidget):
@@ -424,19 +425,56 @@
         self.gridLayout_10.addWidget(self.spinMoveHGSLat, 0, 3, 1, 1)
         self.verticalLayout_4.addWidget(self.widget_4)
         spacerItem3 = QtWidgets.QSpacerItem(20, 147, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_4.addItem(spacerItem3)
         self.stackedMove.addWidget(self.pageMoveHeliographicStonyhurst)
         self.pageMoveHelioprojectiveRadial = QtWidgets.QWidget()
         self.pageMoveHelioprojectiveRadial.setObjectName("pageMoveHelioprojectiveRadial")
-        self.widget_5 = QtWidgets.QWidget(self.pageMoveHelioprojectiveRadial)
-        self.widget_5.setGeometry(QtCore.QRect(10, 10, 342, 44))
+        self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.pageMoveHelioprojectiveRadial)
+        self.verticalLayout_10.setObjectName("verticalLayout_10")
+        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
+        self.label_42 = QtWidgets.QLabel(self.pageMoveHelioprojectiveRadial)
+        self.label_42.setObjectName("label_42")
+        self.horizontalLayout_3.addWidget(self.label_42)
+        self.spinMoveHelioProjectiveRadialTx = QtWidgets.QSpinBox(self.pageMoveHelioprojectiveRadial)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.spinMoveHelioProjectiveRadialTx.sizePolicy().hasHeightForWidth())
+        self.spinMoveHelioProjectiveRadialTx.setSizePolicy(sizePolicy)
+        self.spinMoveHelioProjectiveRadialTx.setPrefix("")
+        self.spinMoveHelioProjectiveRadialTx.setMinimum(-9999)
+        self.spinMoveHelioProjectiveRadialTx.setMaximum(9999)
+        self.spinMoveHelioProjectiveRadialTx.setObjectName("spinMoveHelioProjectiveRadialTx")
+        self.horizontalLayout_3.addWidget(self.spinMoveHelioProjectiveRadialTx)
+        self.label_41 = QtWidgets.QLabel(self.pageMoveHelioprojectiveRadial)
+        self.label_41.setObjectName("label_41")
+        self.horizontalLayout_3.addWidget(self.label_41)
+        self.spinMoveHelioProjectiveRadialTy = QtWidgets.QSpinBox(self.pageMoveHelioprojectiveRadial)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.spinMoveHelioProjectiveRadialTy.sizePolicy().hasHeightForWidth())
+        self.spinMoveHelioProjectiveRadialTy.setSizePolicy(sizePolicy)
+        self.spinMoveHelioProjectiveRadialTy.setMinimum(-9999)
+        self.spinMoveHelioProjectiveRadialTy.setMaximum(9999)
+        self.spinMoveHelioProjectiveRadialTy.setObjectName("spinMoveHelioProjectiveRadialTy")
+        self.horizontalLayout_3.addWidget(self.spinMoveHelioProjectiveRadialTy)
+        self.verticalLayout_10.addLayout(self.horizontalLayout_3)
+        spacerItem4 = QtWidgets.QSpacerItem(20, 240, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_10.addItem(spacerItem4)
+        self.stackedMove.addWidget(self.pageMoveHelioprojectiveRadial)
+        self.pageMoveHelioprojectiveMuPsi = QtWidgets.QWidget()
+        self.pageMoveHelioprojectiveMuPsi.setObjectName("pageMoveHelioprojectiveMuPsi")
+        self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.pageMoveHelioprojectiveMuPsi)
+        self.verticalLayout_11.setObjectName("verticalLayout_11")
+        self.widget_5 = QtWidgets.QWidget(self.pageMoveHelioprojectiveMuPsi)
         self.widget_5.setObjectName("widget_5")
         self.gridLayout_13 = QtWidgets.QGridLayout(self.widget_5)
-        self.gridLayout_13.setContentsMargins(0, 0, 0, 0)
         self.gridLayout_13.setObjectName("gridLayout_13")
         self.label_39 = QtWidgets.QLabel(self.widget_5)
         self.label_39.setObjectName("label_39")
         self.gridLayout_13.addWidget(self.label_39, 0, 2, 1, 1)
         self.spinMoveHelioprojectiveRadialMu = QtWidgets.QDoubleSpinBox(self.widget_5)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
@@ -459,15 +497,18 @@
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.spinMoveHelioprojectiveRadialPsi.sizePolicy().hasHeightForWidth())
         self.spinMoveHelioprojectiveRadialPsi.setSizePolicy(sizePolicy)
         self.spinMoveHelioprojectiveRadialPsi.setMinimum(0.0)
         self.spinMoveHelioprojectiveRadialPsi.setMaximum(359.0)
         self.spinMoveHelioprojectiveRadialPsi.setObjectName("spinMoveHelioprojectiveRadialPsi")
         self.gridLayout_13.addWidget(self.spinMoveHelioprojectiveRadialPsi, 0, 3, 1, 1)
-        self.stackedMove.addWidget(self.pageMoveHelioprojectiveRadial)
+        self.verticalLayout_11.addWidget(self.widget_5)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 230, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_11.addItem(spacerItem5)
+        self.stackedMove.addWidget(self.pageMoveHelioprojectiveMuPsi)
         self.pageMoveOrbitElements = QtWidgets.QWidget()
         self.pageMoveOrbitElements.setObjectName("pageMoveOrbitElements")
         self.gridLayout_8 = QtWidgets.QGridLayout(self.pageMoveOrbitElements)
         self.gridLayout_8.setObjectName("gridLayout_8")
         self.horizontalLayout_8 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_8.setObjectName("horizontalLayout_8")
         self.label_21 = QtWidgets.QLabel(self.pageMoveOrbitElements)
@@ -626,16 +667,16 @@
         self.buttonMove = QtWidgets.QPushButton(self.groupBox_5)
         icon1 = QtGui.QIcon()
         icon1.addPixmap(QtGui.QPixmap(":/resources/arrow-alt-circle-right-solid.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.buttonMove.setIcon(icon1)
         self.buttonMove.setObjectName("buttonMove")
         self.verticalLayout_7.addWidget(self.buttonMove)
         self.verticalLayout_8.addWidget(self.groupBox_5)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_8.addItem(spacerItem4)
+        spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem6)
         self.horizontalLayout_7.addLayout(self.verticalLayout_8)
         self.verticalLayout_6 = QtWidgets.QVBoxLayout()
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.groupBox = QtWidgets.QGroupBox(TelescopeWidget)
         self.groupBox.setObjectName("groupBox")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.groupBox)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
@@ -729,25 +770,25 @@
         self.buttonResetHorizontalOffsets.setObjectName("buttonResetHorizontalOffsets")
         self.gridLayout_11.addWidget(self.buttonResetHorizontalOffsets, 0, 4, 2, 1)
         self.verticalLayout_5.addWidget(self.groupHorizontalOffsets)
         self.verticalLayout_6.addWidget(self.groupBox)
         self.compassmovewidget = CompassMoveWidget(TelescopeWidget)
         self.compassmovewidget.setObjectName("compassmovewidget")
         self.verticalLayout_6.addWidget(self.compassmovewidget)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem5)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem7)
         self.horizontalLayout_7.addLayout(self.verticalLayout_6)
-        spacerItem6 = QtWidgets.QSpacerItem(133, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_7.addItem(spacerItem6)
+        spacerItem8 = QtWidgets.QSpacerItem(133, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_7.addItem(spacerItem8)
         self.widgetSidebar = QtWidgets.QWidget(TelescopeWidget)
         self.widgetSidebar.setObjectName("widgetSidebar")
         self.horizontalLayout_7.addWidget(self.widgetSidebar)
 
         self.retranslateUi(TelescopeWidget)
-        self.stackedMove.setCurrentIndex(0)
+        self.stackedMove.setCurrentIndex(3)
         QtCore.QMetaObject.connectSlotsByName(TelescopeWidget)
         TelescopeWidget.setTabOrder(self.labelStatus, self.buttonInit)
         TelescopeWidget.setTabOrder(self.buttonInit, self.buttonPark)
         TelescopeWidget.setTabOrder(self.buttonPark, self.labelCurRA)
         TelescopeWidget.setTabOrder(self.labelCurRA, self.labelCurDec)
         TelescopeWidget.setTabOrder(self.labelCurDec, self.labelCurAlt)
         TelescopeWidget.setTabOrder(self.labelCurAlt, self.labelCurAz)
@@ -783,14 +824,18 @@
         self.label_25.setText(_translate("TelescopeWidget", "Az:"))
         self.label_24.setText(_translate("TelescopeWidget", "Alt:"))
         self.spinMoveAlt.setSuffix(_translate("TelescopeWidget", " °"))
         self.spinMoveAz.setSuffix(_translate("TelescopeWidget", " °"))
         self.label_37.setText(_translate("TelescopeWidget", "Lat:"))
         self.label_38.setText(_translate("TelescopeWidget", "Lon:"))
         self.spinMoveHGSLat.setSuffix(_translate("TelescopeWidget", " °"))
+        self.label_42.setText(_translate("TelescopeWidget", "Tx"))
+        self.spinMoveHelioProjectiveRadialTx.setSuffix(_translate("TelescopeWidget", "\""))
+        self.label_41.setText(_translate("TelescopeWidget", "Ty"))
+        self.spinMoveHelioProjectiveRadialTy.setSuffix(_translate("TelescopeWidget", "\""))
         self.label_39.setText(_translate("TelescopeWidget", "Psi:"))
         self.label_40.setText(_translate("TelescopeWidget", "Mu:"))
         self.spinMoveHelioprojectiveRadialPsi.setSuffix(_translate("TelescopeWidget", " °"))
         self.label_21.setText(_translate("TelescopeWidget", "JPL Horizons:"))
         self.buttonHorizonsQuery.setText(_translate("TelescopeWidget", "..."))
         self.label_29.setText(_translate("TelescopeWidget", "Ω:"))
         self.label_32.setText(_translate("TelescopeWidget", "e:"))
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/temperaturesplotwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/temperaturesplotwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/temperaturesplotwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/temperaturesplotwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/temperatureswidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/temperatureswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/temperatureswidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/temperatureswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/videowidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/videowidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/videowidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/videowidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/weatherwidget.ui` & `pyobs_gui-1.0.6/pyobs_gui/qt/weatherwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/qt/weatherwidget_ui.py` & `pyobs_gui-1.0.6/pyobs_gui/qt/weatherwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/roofwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/roofwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/shellwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/shellwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,21 +125,21 @@
         # signals/slots
         self.add_command_log.connect(self.textCommandLog.append)
         self.textCommandInput.commandExecuted.connect(self.execute_command)
         self.textCommandInput.textChanged.connect(self._update_docs)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # commands
         self.command_model = CommandModel(self.comm)
 
         # create completer
         self.completer = QtWidgets.QCompleter(self)
         self.completer.setCompletionMode(QtWidgets.QCompleter.PopupCompletion)
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/spectrographwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/spectrographwidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Optional, Any, Union, Dict
+from typing import Optional, Any, Union, Dict, List
 from PyQt5 import QtCore, QtWidgets
 from astroplan import Observer
 from astropy.io import fits
 
 from pyobs.comm import Proxy, Comm
 from pyobs.events import ExposureStatusChangedEvent, Event
 from pyobs.interfaces import IAbortable, ISpectrograph, IExposureTime
@@ -45,22 +45,22 @@
         self.butAbort.setVisible(isinstance(self.module, IAbortable))
 
         # connect signals
         self.signal_update_gui.connect(self.update_gui)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
-        await self.datadisplay.open(module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
+        await self.datadisplay.open(modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # subscribe to events
         await self.comm.register_event(ExposureStatusChangedEvent, self._on_exposure_status_changed)
 
     async def _init(self) -> None:
         # get status
         if isinstance(self.module, ISpectrograph):
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/statuswidget.py` & `pyobs_gui-1.0.6/pyobs_gui/statuswidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from asyncio import Task
 from datetime import datetime
-from typing import Any, Type, Dict, Optional, cast, Union
+from typing import Any, Type, Dict, Optional, cast, Union, List
 from PyQt5 import QtWidgets, QtCore
 import inspect
 
 from astroplan import Observer
 
 import pyobs.events
 from pyobs.comm import Comm, Proxy
@@ -105,32 +105,32 @@
         self.verticalHeader().hide()
 
         # stuff
         self._status_task: Optional[Task] = None
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
 
         # register events
         await self.comm.register_event(ModuleOpenedEvent, self._module_opened)
         await self.comm.register_event(ModuleClosedEvent, self._module_closed)
 
         # add all existing modules
         for mod in self.comm.clients:
             await self._module_opened(ModuleOpenedEvent(), mod)
 
         # trigger status updates
-        #self._status_task = asyncio.create_task(self._update_status())
+        # self._status_task = asyncio.create_task(self._update_status())
 
     async def _module_opened(self, event: Event, sender: str) -> bool:
         """Called when module was opened."""
         if not isinstance(event, ModuleOpenedEvent):
             return False
 
         # add module
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/telescopewidget.py` & `pyobs_gui-1.0.6/pyobs_gui/telescopewidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any, Tuple, Optional, Union, Dict
+from typing import Any, Tuple, Optional, Union, Dict, List
 
 import numpy as np
 from PyQt5 import QtWidgets, QtCore
 from astroplan import Observer
 from astropy.coordinates import SkyCoord, ICRS, AltAz, get_sun
 import astropy.units as u
 import logging
@@ -12,14 +12,15 @@
 from sunpy.coordinates.frames import Helioprojective, HeliographicStonyhurst
 
 from pyobs.comm import Proxy, Comm
 from pyobs.events import MotionStatusChangedEvent, Event
 from pyobs.interfaces import (
     IPointingRaDec,
     IPointingAltAz,
+    IPointingHelioprojective,
     IPointingHGS,
     IOffsetsRaDec,
     IOffsetsAltAz,
     IFilters,
     IFocuser,
     ITemperatures,
     IMotion,
@@ -40,14 +41,15 @@
 
 class COORDS(Enum):
     EQUITORIAL = "Equitorial"
     HORIZONTAL = "Horizontal"
     ORBIT_ELEMENTS = "Orbit Elements"
     HELIOGRAPHIC_STONYHURST = "Heliographic Stonyhurst"
     HELIOPROJECTIVE_RADIAL = "Helioprojective Radial"
+    HELIOPROJECTIVE_MUPSI = "Helioprojective Mu/Psi"
 
 
 class TelescopeWidget(QtWidgets.QWidget, BaseWidget, Ui_TelescopeWidget):
     signal_update_gui = QtCore.pyqtSignal()
 
     def __init__(self, **kwargs: Any):
         QtWidgets.QWidget.__init__(self)
@@ -68,23 +70,25 @@
 
         # move widgets
         self._MOVE_WIDGETS = {
             COORDS.EQUITORIAL: self.pageMoveEquatorial,
             COORDS.HORIZONTAL: self.pageMoveHorizontal,
             COORDS.HELIOGRAPHIC_STONYHURST: self.pageMoveHeliographicStonyhurst,
             COORDS.HELIOPROJECTIVE_RADIAL: self.pageMoveHelioprojectiveRadial,
+            COORDS.HELIOPROJECTIVE_MUPSI: self.pageMoveHelioprojectiveRadial,
             COORDS.ORBIT_ELEMENTS: self.pageMoveOrbitElements,
         }
 
         # calculate dest coordinates
         self._DEST_CALC = {
             COORDS.EQUITORIAL: self._calc_dest_equatorial,
             COORDS.HORIZONTAL: self._calc_dest_horizontal,
             COORDS.HELIOGRAPHIC_STONYHURST: self._calc_dest_heliographic_stonyhurst,
             COORDS.HELIOPROJECTIVE_RADIAL: self._calc_dest_helioprojective_radial,
+            COORDS.HELIOPROJECTIVE_MUPSI: self._calc_dest_helioprojective_radial,
             COORDS.ORBIT_ELEMENTS: self._calc_dest_orbit_elements,
         }
 
         # plot
         # self.figure = plt.figure()
         # self.plot = VisPlot(self.figure, self.environment)
         # self.canvas = FigureCanvas(self.figure)
@@ -108,37 +112,38 @@
         self.colorize_button(self.buttonHorizonsQuery, QtCore.Qt.green)
 
         # connect signals
         self.signal_update_gui.connect(self.update_gui)
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
-        await self.compassmovewidget.open(module=module, comm=comm, observer=observer, vfs=vfs)
-        self.compassmovewidget.show_extract_button(CompassMoveWidget, f'Offset "{module.name}"')
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
+        await self.compassmovewidget.open(modules=modules, comm=comm, observer=observer, vfs=vfs)
+        self.compassmovewidget.show_extract_button(CompassMoveWidget, f'Offset "{modules[0].name}"')
 
         # subscribe to events
         if self.comm is not None:
             await self.comm.register_event(MotionStatusChangedEvent, self._on_motion_status_changed)
 
         # add coord types
         if isinstance(self.module, IPointingRaDec):
             self.comboMoveType.addItem(COORDS.EQUITORIAL.value)
             # self.comboMoveType.addItem(COORDS.ORBIT_ELEMENTS.value)
         if isinstance(self.module, IPointingAltAz):
             self.comboMoveType.addItem(COORDS.HORIZONTAL.value)
-        if isinstance(self.module, IPointingHGS):
+        if isinstance(self.module, IPointingHGS) or isinstance(self.module, IPointingHelioprojective):
             self.comboMoveType.addItem(COORDS.HELIOGRAPHIC_STONYHURST.value)
             self.comboMoveType.addItem(COORDS.HELIOPROJECTIVE_RADIAL.value)
+            self.comboMoveType.addItem(COORDS.HELIOPROJECTIVE_MUPSI.value)
         if self.comboMoveType.count() > 0:
             self.comboMoveType.setCurrentIndex(0)
 
         # offsets
         self.groupEquatorialOffsets.setVisible(isinstance(self.module, IOffsetsRaDec))
         self.groupHorizontalOffsets.setVisible(isinstance(self.module, IOffsetsAltAz))
 
@@ -338,14 +343,29 @@
             # move
             if isinstance(self.module, IPointingHGS):
                 self.run_background(self.module.move_hgs_lon_lat, lon, lat)
             else:
                 QtWidgets.QMessageBox.critical(self, "pyobs", "Telescope does not support stonyhurst coordinates.")
 
         elif coord == COORDS.HELIOPROJECTIVE_RADIAL:
+            # get theta x/y in degrees
+            theta_x = self.spinMoveHelioProjectiveRadialTx.value() / 3600.0
+            theta_y = self.spinMoveHelioProjectiveRadialTy.value() / 3600.0
+
+            # move
+            if isinstance(self.module, IPointingHelioprojective):
+                # run it
+                self.run_background(self.module.move_helioprojective, theta_x, theta_y)
+
+            else:
+                QtWidgets.QMessageBox.critical(
+                    self, "pyobs", "Telescope does not support helioprojective radial coordinates."
+                )
+
+        elif coord == COORDS.HELIOPROJECTIVE_MUPSI:
             # get mu and psi (in rad)
             mu = self.spinMoveHelioprojectiveRadialMu.value()
             psi = np.deg2rad(self.spinMoveHelioprojectiveRadialPsi.value())
 
             # to stonyhurst lat/lon
             alpha = np.arccos(mu)
             dsun = get_sun(Time.now()).distance  # distance earth <-> sun
@@ -357,23 +377,28 @@
             theta = np.arctan(rsun * np.sin(alpha) / (dsun - (rsun * mu)))
 
             # calculate helio projective cartesian coordinates
             tx = -theta * np.sin(psi)
             ty = theta * np.cos(psi)
             heliproj = SkyCoord(tx, ty, obstime=Time.now(), frame=Helioprojective, observer="earth")
 
-            # convert helio projective coordinates to Heliographic Stonyhurst
-            stony = heliproj.transform_to(HeliographicStonyhurst)
-            lon, lat = float(stony.lon.to(u.degree).value), float(stony.lat.to(u.degree).value)
-
             # move
-            if isinstance(self.module, IPointingHGS):
+            if isinstance(self.module, IPointingHelioprojective):
+                # run it
+                self.run_background(self.module.move_helioprojective, heliproj.Tx.degrees, heliproj.Ty.degrees)
+
+            elif isinstance(self.module, IPointingHGS):
+                # alternatively, convert helio projective coordinates to Heliographic Stonyhurst
+                stony = heliproj.transform_to(HeliographicStonyhurst)
+                lon, lat = float(stony.lon.to(u.degree).value), float(stony.lat.to(u.degree).value)
+
+                # run it
                 self.run_background(self.module.move_hgs_lon_lat, lon, lat)
             else:
-                QtWidgets.QMessageBox.critical(self, "pyobs", "Telescope does not support stonyhurst coordinates.")
+                QtWidgets.QMessageBox.critical(self, "pyobs", "Telescope does not support Mu/Psi coordinates.")
 
     async def _on_motion_status_changed(self, event: Event, sender: str) -> bool:
         """Called when motion status of module changed.
 
         Args:
             event: Status change event.
             sender: Name of sender.
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/temperaturesplotwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/temperaturesplotwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         self.data = pd.concat([self.data, df], ignore_index=True, axis=0)
 
         # save?
         if self.checkLogFile.isChecked() and self.log_file != "":
             self.data.to_csv(self.log_file, index=False)
 
         # what to plot?
-        print(self.show_option)
         if self.show_option == "All":
             d = self.data
         elif self.show_option == "Last minute":
             d = self.data[self.data["time"] >= datetime.datetime.utcnow() - datetime.timedelta(minutes=1)]
         elif self.show_option == "Last 5 minutes":
             d = self.data[self.data["time"] >= datetime.datetime.utcnow() - datetime.timedelta(minutes=5)]
         else:
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/temperatureswidget.py` & `pyobs_gui-1.0.6/pyobs_gui/temperatureswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/utils.py` & `pyobs_gui-1.0.6/pyobs_gui/utils.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/videowidget.py` & `pyobs_gui-1.0.6/pyobs_gui/videowidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Any, Optional, cast, Union, Dict
+from typing import Any, Optional, cast, Union, Dict, List
 from urllib.parse import urlparse
 from PyQt5 import QtWidgets, QtCore, QtGui, QtNetwork
 from astroplan import Observer
 
 from pyobs.comm import Proxy, Comm
 
 from pyobs.interfaces import IExposureTime, IImageType, IImageFormat, IVideo, IGain
@@ -71,22 +71,22 @@
         self.comboImageType.setCurrentText("OBJECT")
 
         # initial values
         self.comboImageType.setCurrentIndex(image_types.index("OBJECT"))
 
     async def open(
         self,
-        module: Optional[Proxy] = None,
+        modules: Optional[List[Proxy]] = None,
         comm: Optional[Comm] = None,
         observer: Optional[Observer] = None,
         vfs: Optional[Union[VirtualFileSystem, Dict[str, Any]]] = None,
     ) -> None:
         """Open module."""
-        await BaseWidget.open(self, module=module, comm=comm, observer=observer, vfs=vfs)
-        await self.datadisplay.open(module=module, comm=comm, observer=observer, vfs=vfs)
+        await BaseWidget.open(self, modules=modules, comm=comm, observer=observer, vfs=vfs)
+        await self.datadisplay.open(modules=modules, comm=comm, observer=observer, vfs=vfs)
 
     async def _init(self) -> None:
         # hide single controls, if necessary
         self.labelImageType.setVisible(isinstance(self.module, IImageType))
         self.comboImageType.setVisible(isinstance(self.module, IImageType))
         self.groupExposure.setVisible(isinstance(self.module, IExposureTime))
         self.groupGain.setVisible(isinstance(self.module, IGain))
```

### Comparing `pyobs_gui-1.0.5/pyobs_gui/visplot.py` & `pyobs_gui-1.0.6/pyobs_gui/visplot.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/pyobs_gui/weatherwidget.py` & `pyobs_gui-1.0.6/pyobs_gui/weatherwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.5/PKG-INFO` & `pyobs_gui-1.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyobs-gui
-Version: 1.0.5
+Version: 1.0.6
 Summary: A remote GUI for pyobs
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyQt5 (>=5.14,<6.0)
-Requires-Dist: QtAwesome (>=1.1,<2.0)
-Requires-Dist: colour (>=0.1,<0.2)
-Requires-Dist: matplotlib (>=3.4,<4.0)
-Requires-Dist: pyobs-core (>=1.0,<2.0)
-Requires-Dist: qasync (>=0.22,<0.23)
-Requires-Dist: qfitswidget (>=0.8,<0.9)
-Requires-Dist: sunpy (>=3.1,<4.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyQt5 (>=5.15.9,<6.0.0)
+Requires-Dist: QtAwesome (>=1.2.3,<2.0.0)
+Requires-Dist: colour (>=0.1.5,<0.2.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: qasync (>=0.22.0,<0.23.0)
+Requires-Dist: qfitswidget (>=0.8.2,<0.9.0)
+Requires-Dist: sunpy (>=3.1.8,<4.0.0)
```

