# Comparing `tmp/control-lab-ly-1.1.1a1.tar.gz` & `tmp/control-lab-ly-1.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.1.1a1.tar", last modified: Tue Jun 27 03:19:45 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.1a2.tar", last modified: Wed Jul 12 02:31:34 2023, max compression
```

## Comparing `control-lab-ly-1.1.1a1.tar` & `control-lab-ly-1.1.1a2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.700366 control-lab-ly-1.1.1a1/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a1/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/MANIFEST.in
--rw-rw-rw-   0        0        0    20808 2023-06-27 03:19:45.701375 control-lab-ly-1.1.1a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.811404 control-lab-ly-1.1.1a1/docs/
--rw-rw-rw-   0        0        0     6576 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.1a1/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a1/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13114 2023-06-15 07:16:26.000000 control-lab-ly-1.1.1a1/docs/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.815913 control-lab-ly-1.1.1a1/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a1/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/pyproject.toml
--rw-rw-rw-   0        0        0     1500 2023-06-27 03:19:45.702909 control-lab-ly-1.1.1a1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.638387 control-lab-ly-1.1.1a1/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.834325 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    20808 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7087 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.839214 control-lab-ly-1.1.1a1/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.848094 control-lab-ly-1.1.1a1/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.855579 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.866374 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17618 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8197 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.910249 control-lab-ly-1.1.1a1/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.930520 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.970517 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16416 2023-06-23 06:16:42.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     3780 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.004680 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14530 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.1a1/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.030170 control-lab-ly-1.1.1a1/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.053481 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11192 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.068444 control-lab-ly-1.1.1a1/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9890 2023-06-21 10:05:07.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.073761 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.105185 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.139238 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.162356 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    10875 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.187936 control-lab-ly-1.1.1a1/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.204619 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.233919 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      359 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18010 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     1993 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.253997 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      287 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10637 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.265568 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.287848 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10372 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.298379 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.318543 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-06-26 05:50:00.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8358 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8199 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14473 2023-06-27 03:07:03.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.334434 control-lab-ly-1.1.1a1/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.355224 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9407 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3450 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     6355 2023-06-22 05:19:20.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/grbl_lib.py
--rw-rw-rw-   0        0        0     4858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.367626 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.382878 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.388912 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24280 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15776 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7128 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10566 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32385 2023-06-21 10:10:48.000000 control-lab-ly-1.1.1a1/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.401275 control-lab-ly-1.1.1a1/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.415877 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.424834 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.439487 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.453486 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    32163 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.464023 control-lab-ly-1.1.1a1/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.469661 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.482708 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8844 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.497957 control-lab-ly-1.1.1a1/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.504957 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.516813 control-lab-ly-1.1.1a1/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.528814 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.538781 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.550728 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.574636 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-06-22 09:26:34.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0     1836 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.588936 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2988 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    15898 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.633386 control-lab-ly-1.1.1a1/src/controllably/misc/
--rw-rw-rw-   0        0        0      627 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9596 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     7940 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17547 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4543 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.637386 control-lab-ly-1.1.1a1/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.651030 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.669039 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.687769 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.697770 control-lab-ly-1.1.1a1/tests/
--rw-rw-rw-   0        0        0     2365 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a1/tests/test_panels.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.510639 control-lab-ly-1.1.1a2/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a2/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/MANIFEST.in
+-rw-rw-rw-   0        0        0    22652 2023-07-12 02:31:34.510639 control-lab-ly-1.1.1a2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.374766 control-lab-ly-1.1.1a2/docs/
+-rw-rw-rw-   0        0        0     8422 2023-07-12 02:28:37.000000 control-lab-ly-1.1.1a2/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.1a2/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a2/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13112 2023-07-03 05:57:22.000000 control-lab-ly-1.1.1a2/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.379147 control-lab-ly-1.1.1a2/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a2/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/pyproject.toml
+-rw-rw-rw-   0        0        0     1500 2023-07-12 02:31:34.516964 control-lab-ly-1.1.1a2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.1a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.193040 control-lab-ly-1.1.1a2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.410646 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    22652 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7085 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.423055 control-lab-ly-1.1.1a2/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.432521 control-lab-ly-1.1.1a2/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.445309 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.495690 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17940 2023-07-10 07:55:52.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.504148 control-lab-ly-1.1.1a2/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.538952 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.607154 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16416 2023-06-23 06:16:42.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     3780 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.638900 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14530 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.1a2/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.654615 control-lab-ly-1.1.1a2/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.672235 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11192 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.687709 control-lab-ly-1.1.1a2/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9890 2023-06-21 10:05:07.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.708790 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.733749 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.762014 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.778346 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    11490 2023-07-12 02:08:44.000000 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.811272 control-lab-ly-1.1.1a2/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.825071 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.852389 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      359 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18010 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     1993 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.870927 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      287 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10637 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.880555 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.905328 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10508 2023-07-04 08:31:36.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.920497 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3549 2023-07-03 07:23:35.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.937808 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-06-26 05:50:00.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8358 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8199 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14473 2023-06-27 03:07:03.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.945409 control-lab-ly-1.1.1a2/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.977340 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9703 2023-07-12 02:05:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     6196 2023-07-12 02:12:03.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     6355 2023-06-22 05:19:20.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/grbl_lib.py
+-rw-rw-rw-   0        0        0     4942 2023-07-12 02:11:52.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.992587 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.024460 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.073979 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15969 2023-07-03 02:34:15.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7266 2023-07-06 09:52:37.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4324 2023-07-03 05:56:38.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10566 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32435 2023-07-06 09:48:51.000000 control-lab-ly-1.1.1a2/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.088180 control-lab-ly-1.1.1a2/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.110566 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.127031 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.154362 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.174683 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    32163 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.182616 control-lab-ly-1.1.1a2/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.195913 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.213987 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.261011 control-lab-ly-1.1.1a2/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.275873 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.292440 control-lab-ly-1.1.1a2/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.306759 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.319784 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.326364 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.388415 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-06-22 09:26:34.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0     1836 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.396163 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2988 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    15898 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.440271 control-lab-ly-1.1.1a2/src/controllably/misc/
+-rw-rw-rw-   0        0        0      627 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9533 2023-07-03 06:07:16.000000 control-lab-ly-1.1.1a2/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     8498 2023-07-03 06:52:23.000000 control-lab-ly-1.1.1a2/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    23175 2023-07-05 07:05:03.000000 control-lab-ly-1.1.1a2/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4543 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.446344 control-lab-ly-1.1.1a2/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.461248 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.477926 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.497052 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.507041 control-lab-ly-1.1.1a2/tests/
+-rw-rw-rw-   0        0        0      398 2023-07-03 06:53:18.000000 control-lab-ly-1.1.1a2/tests/test_init.py
```

### Comparing `control-lab-ly-1.1.1a1/LICENSE.md` & `control-lab-ly-1.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/PKG-INFO` & `control-lab-ly-1.1.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -244,17 +244,17 @@
 ```python
 from configs.MySetup import setup, LAYOUT_FILE
 setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
 > `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
 #### 2.2 Loading a Labware
-To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
+To load a `Labware` onto the deck, use the `loadLabware()` method of the `Deck` object.
 ```python
-setup.Mover.deck.load_labware(...)
+setup.Mover.deck.loadLabware(...)
 ``` 
 > This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
 
 ### 3. Managing project addresses
 A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
 ```yaml
@@ -357,14 +357,53 @@
 # Change Log
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
+## Version 1.1.1
+Bug fixes and patches. First released 30 Jun 2023.
+### Added
+- import `Device` classes in init files to view documentation
+- added library for GRBL status and error codes
+- add `update_root_direcctory()` function to Helper
+### Changed
+- fix bug with adding new rows into Dataframes
+- initialise `PiezoRoboticsDevice` upon connection
+- use `reset_input_buffer()` instead of `flushInput()` for `pyserial.Serial` objects
+- print the actual string sent to Serial devices
+- verbosity of `Measure` objects pass through to devices
+- update `Sartorius` class
+  - `tip_inset_mm` now an instance attribute with initialisation parameters
+  - set `tip_on` flag to False when performing `eject()`
+- update `Gantry` class
+  - read multiple flines in `_query()`
+  - check that commands end with newline before sending to device
+- update `Primitiv` class
+  - add `getStatus()` and `stop()` methods
+  - add `_get_settings()` method
+- update methods in `Deck`, `Labware`, and `Well` to camelCase
+- update `Deck.isExcluded()` to apply strict inequalities when determining out-of-range coordinates
+- update `LiquidMover` to insert a portion of tip into rack before ejecting
+- update `Spinner`
+  - fix bug with sending commands
+  - added `_query()` method
+  - pass verbosity to individual spinners
+- update `PiezoRoboticsDevice` to raise errors when encountering them
+- update `Mover`
+  - modify`setFlag()` to print kwargs instead of raising error if assigned values are not boolean
+  - use `safe_height` (if defined) instead of z-coordinate of home in `safeMoveTo()`
+  - added `getSettings()` method
+- fix bug in `M1Pro.setHandedness()`
+- update `Ender`
+  - added `getTemperature()`, `holdTemperature()`, `isAtTemperature()` methods
+  - modified `setTemperature()` to use Marlin code to wait for temperature
+
+
 ## Version 1.1.0
 Bug fixes and feature enhancements. First released 15 Jun 2023.
 ### Added
 - `ForceSensor` - DIY force sensor (#55)
 - `BioShake` - orbital shaker from QInstruments (#56)
 - `SentronProbe` - pH meter probe from Sentron (#75)
 - `Maker`
```

### Comparing `control-lab-ly-1.1.1a1/docs/CHANGELOG.md` & `control-lab-ly-1.1.1a2/docs/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,53 @@
 # Change Log
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
+## Version 1.1.1
+Bug fixes and patches. First released 30 Jun 2023.
+### Added
+- import `Device` classes in init files to view documentation
+- added library for GRBL status and error codes
+- add `update_root_direcctory()` function to Helper
+### Changed
+- fix bug with adding new rows into Dataframes
+- initialise `PiezoRoboticsDevice` upon connection
+- use `reset_input_buffer()` instead of `flushInput()` for `pyserial.Serial` objects
+- print the actual string sent to Serial devices
+- verbosity of `Measure` objects pass through to devices
+- update `Sartorius` class
+  - `tip_inset_mm` now an instance attribute with initialisation parameters
+  - set `tip_on` flag to False when performing `eject()`
+- update `Gantry` class
+  - read multiple flines in `_query()`
+  - check that commands end with newline before sending to device
+- update `Primitiv` class
+  - add `getStatus()` and `stop()` methods
+  - add `_get_settings()` method
+- update methods in `Deck`, `Labware`, and `Well` to camelCase
+- update `Deck.isExcluded()` to apply strict inequalities when determining out-of-range coordinates
+- update `LiquidMover` to insert a portion of tip into rack before ejecting
+- update `Spinner`
+  - fix bug with sending commands
+  - added `_query()` method
+  - pass verbosity to individual spinners
+- update `PiezoRoboticsDevice` to raise errors when encountering them
+- update `Mover`
+  - modify`setFlag()` to print kwargs instead of raising error if assigned values are not boolean
+  - use `safe_height` (if defined) instead of z-coordinate of home in `safeMoveTo()`
+  - added `getSettings()` method
+- fix bug in `M1Pro.setHandedness()`
+- update `Ender`
+  - added `getTemperature()`, `holdTemperature()`, `isAtTemperature()` methods
+  - modified `setTemperature()` to use Marlin code to wait for temperature
+
+
 ## Version 1.1.0
 Bug fixes and feature enhancements. First released 15 Jun 2023.
 ### Added
 - `ForceSensor` - DIY force sensor (#55)
 - `BioShake` - orbital shaker from QInstruments (#56)
 - `SentronProbe` - pH meter probe from Sentron (#75)
 - `Maker`
```

### Comparing `control-lab-ly-1.1.1a1/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.1a2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/docs/LICENSE.md` & `control-lab-ly-1.1.1a2/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/docs/README.md` & `control-lab-ly-1.1.1a2/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -219,17 +219,17 @@
 ```python
 from configs.MySetup import setup, LAYOUT_FILE
 setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
 > `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
 #### 2.2 Loading a Labware
-To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
+To load a `Labware` onto the deck, use the `loadLabware()` method of the `Deck` object.
 ```python
-setup.Mover.deck.load_labware(...)
+setup.Mover.deck.loadLabware(...)
 ``` 
 > This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
 
 ### 3. Managing project addresses
 A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
 ```yaml
```

### Comparing `control-lab-ly-1.1.1a1/docs/assets/Documentation guide.png` & `control-lab-ly-1.1.1a2/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/setup.cfg` & `control-lab-ly-1.1.1a2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
-00000030: 2e31 2d61 310d 0a64 6573 6372 6970 7469  .1-a1..descripti
+00000030: 2e31 2d61 320d 0a64 6573 6372 6970 7469  .1-a2..descripti
 00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
 00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
 00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
 00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

### Comparing `control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -244,17 +244,17 @@
 ```python
 from configs.MySetup import setup, LAYOUT_FILE
 setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
 > `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
 #### 2.2 Loading a Labware
-To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
+To load a `Labware` onto the deck, use the `loadLabware()` method of the `Deck` object.
 ```python
-setup.Mover.deck.load_labware(...)
+setup.Mover.deck.loadLabware(...)
 ``` 
 > This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
 
 ### 3. Managing project addresses
 A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
 ```yaml
@@ -357,14 +357,53 @@
 # Change Log
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
+## Version 1.1.1
+Bug fixes and patches. First released 30 Jun 2023.
+### Added
+- import `Device` classes in init files to view documentation
+- added library for GRBL status and error codes
+- add `update_root_direcctory()` function to Helper
+### Changed
+- fix bug with adding new rows into Dataframes
+- initialise `PiezoRoboticsDevice` upon connection
+- use `reset_input_buffer()` instead of `flushInput()` for `pyserial.Serial` objects
+- print the actual string sent to Serial devices
+- verbosity of `Measure` objects pass through to devices
+- update `Sartorius` class
+  - `tip_inset_mm` now an instance attribute with initialisation parameters
+  - set `tip_on` flag to False when performing `eject()`
+- update `Gantry` class
+  - read multiple flines in `_query()`
+  - check that commands end with newline before sending to device
+- update `Primitiv` class
+  - add `getStatus()` and `stop()` methods
+  - add `_get_settings()` method
+- update methods in `Deck`, `Labware`, and `Well` to camelCase
+- update `Deck.isExcluded()` to apply strict inequalities when determining out-of-range coordinates
+- update `LiquidMover` to insert a portion of tip into rack before ejecting
+- update `Spinner`
+  - fix bug with sending commands
+  - added `_query()` method
+  - pass verbosity to individual spinners
+- update `PiezoRoboticsDevice` to raise errors when encountering them
+- update `Mover`
+  - modify`setFlag()` to print kwargs instead of raising error if assigned values are not boolean
+  - use `safe_height` (if defined) instead of z-coordinate of home in `safeMoveTo()`
+  - added `getSettings()` method
+- fix bug in `M1Pro.setHandedness()`
+- update `Ender`
+  - added `getTemperature()`, `holdTemperature()`, `isAtTemperature()` methods
+  - modified `setTemperature()` to use Marlin code to wait for temperature
+
+
 ## Version 1.1.0
 Bug fixes and feature enhancements. First released 15 Jun 2023.
 ### Added
 - `ForceSensor` - DIY force sensor (#55)
 - `BioShake` - orbital shaker from QInstruments (#56)
 - `SentronProbe` - pH meter probe from Sentron (#75)
 - `Maker`
```

### Comparing `control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,8 @@
 src/controllably/misc/templates/configs/__init__.py
 src/controllably/misc/templates/configs/registry.yaml
 src/controllably/misc/templates/configs/plugins/__init__.py
 src/controllably/misc/templates/configs/plugins/plugin_template.py
 src/controllably/misc/templates/setup/__init__.py
 src/controllably/misc/templates/setup/config.yaml
 src/controllably/misc/templates/setup/layout.json
-tests/test_panels.py
+tests/test_init.py
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
             offset (tuple[float], optional): additional x,y,z offset from tool tip. Defaults to (0,0,0).
         """
         coordinates = np.array(coordinates) - np.array(offset)
         if not self.mover.isFeasible(coordinates, transform_in=True, tool_offset=True):
             raise ValueError(f"Infeasible tool position! {coordinates}")
         self.mover.safeMoveTo(coordinates, ascent_speed=0.2*self.mover._speed_max, descent_speed=0.2*self.mover._speed_max)
         self.setFlag(at_rest=False)
+        time.sleep(1)
         return
     
     def aspirateAt(self, 
         coordinates: tuple[float], 
         volume: float, 
         speed: Optional[float] = None, 
         channel: Optional[int] = None, 
@@ -331,24 +332,24 @@
         tip_length = self.liquid.tip_length
         tip_offset = np.array((0,0,-tip_length + self.liquid.tip_inset_mm))
         self.mover.implement_offset = self.mover.implement_offset - tip_offset
         self.liquid.tip_length = 0
         self.liquid.setFlag(tip_on=False)
         return coordinates
     
-    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None):
+    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None, **kwargs):
         """
         Load Labware objects onto the deck from file or dictionary
         
         Args:
             layout_file (Optional[str], optional): filename of layout .json file. Defaults to None.
             layout_dict (Optional[dict], optional): dictionary of layout. Defaults to None.
         """
-        super().loadDeck(layout_file=layout_file, layout_dict=layout_dict)
-        self.mover.loadDeck(layout_file=layout_file, layout_dict=layout_dict)
+        super().loadDeck(layout_file=layout_file, layout_dict=layout_dict, **kwargs)
+        self.mover.loadDeck(layout_file=layout_file, layout_dict=layout_dict, **kwargs)
         return
     
     def reset(self):
         """Alias for `rest()`"""
         self.rest()
         return
     
@@ -360,42 +361,47 @@
         if rest_coordinates is None:
             self.mover.home()
         else:
             self.align(rest_coordinates)
         self.setFlag(at_rest=True)
         return
     
-    def returnTip(self) -> tuple[float]:
+    def returnTip(self, insert_mm:int = 18) -> tuple[float]:
         """
         Return current tip to its original rack position
+        
+        Args:
+            insert_mm (int, optional): length of tip to insert into rack before ejecting. Defaults to 18.
 
         Returns:
             tuple[float]: coordinates of eject tip location
         """
         coordinates = self.__dict__.pop('_temp_tip_home')
-        return self.ejectTipAt(coordinates=(*coordinates[:2],coordinates[2]-18))
+        coordinates = self.ejectTipAt(coordinates=(*coordinates[:2],coordinates[2]-insert_mm))
+        rack_coordinates = (*coordinates[:2],coordinates[2]+insert_mm)
+        return rack_coordinates
     
     def touchTip(self, well:Well, safe_move:bool = False) -> tuple[float]:
         """
         Touch the tip against the inner walls of the well
         
         Args:
             well (Well): Well object
             safe_move (bool, optional): whether to move safely (i.e. go back to safe height first). Defaults to False.
 
         Returns:
             tuple[float]: coordinates of well center
         """
         diameter = well.diameter
         if safe_move:
-            self.align(coordinates=well.from_top((0,0,-10)))
+            self.align(coordinates=well.fromTop((0,0,-10)))
         else:
             speed = self.mover.speed
             self.mover.setSpeed(speed=0.2*self.mover._speed_max)
-            self.mover.moveTo(coordinates=well.from_top((0,0,-10)))
+            self.mover.moveTo(coordinates=well.fromTop((0,0,-10)))
             self.mover.setSpeed(speed=speed)
         for axis in ('x','y'):
             self.mover.move(axis, diameter/2, speed=0.2*self.mover._speed_max)
             self.mover.move(axis, -diameter, speed=0.2*self.mover._speed_max)
             self.mover.move(axis, diameter/2, speed=0.2*self.mover._speed_max)
         self.mover.moveTo(coordinates=well.top)
         return well.top
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Compound/compound_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,27 +111,27 @@
         
         Args:
             coordinates (tuple[float]): target coordinates
 
         Returns:
             bool: whether the coordinates is feasible
         """
-        return not self.deck.is_excluded(coordinates)
+        return not self.deck.isExcluded(coordinates)
     
-    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None):
+    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None, **kwargs):
         """
         Load Labware objects onto the deck from file or dictionary
         
         Args:
             layout_file (Optional[str], optional): filename of layout .json file. Defaults to None.
             layout_dict (Optional[dict], optional): dictionary of layout. Defaults to None.
         """
-        self.deck.load_layout(layout_file=layout_file, layout_dict=layout_dict)
+        self.deck.loadLayout(layout_file=layout_file, layout_dict=layout_dict, **kwargs)
         for name in self.deck.names:
-            self.positions[name] = [(well.top, well.depth) for well in self.deck.get_slot(name=name).wells_list]
+            self.positions[name] = [(well.top, well.depth) for well in self.deck.getSlot(name=name).wells_list]
         return
     
     def resetFlags(self):
         """Reset all flags to class attribute `_default_flags`"""
         self.flags = self._default_flags.copy()
         return
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/__init__.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/maker_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/mover_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/loader_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/pop_ups.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/templates.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/guide_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/multichannel_panel.py` & `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,26 +130,26 @@
         """
         Executes a spin step
 
         Args:
             speed (int): spin speed in rpm
             time_s (int): spin time in seconds
         """
-        self._write(speed)
+        self._query(speed)
         self.speed = speed
         print(f"Duration   (channel {self.channel}): {time_s}s")
         interval = 1
         start_time = time.perf_counter()
         while(True):
             time.sleep(0.1)
             if (interval <= time.perf_counter() - start_time):
                 interval += 1
             if (time_s <= time.perf_counter() - start_time):
                 break
-        self._write(0)
+        self._query(0)
         self.speed = 0
         return
 
     # Protected method(s)
     def _connect(self, port:str, baudrate:int = 9600, timeout:int = 1):
         """
         Connection procedure for tool
@@ -182,22 +182,44 @@
     def _diagnostic(self):
         """Run diagnostic test"""
         thread = Thread(target=self.run, name=f'maker_diag_{self.channel}')
         thread.start()
         time.sleep(1)
         return
     
+    def _query(self, command:str) ->list[str]:
+        """
+        Write command to and read response from device
+
+        Args:
+            command (str): command string to send to device
+
+        Returns:
+            list[str]: list of response string(s) from device
+        """
+        responses = [b'']
+        self._write(command)
+        try:
+            responses = self.device.readlines()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        else:
+            if self.verbose:
+                print(responses)
+        return
+    
     def _write(self, speed:int):
         """
         Relay spin speed to spinner
 
         Args:
             speed (int): spin speed in rpm
         """
-        fstring = f"{speed}\n", 'utf-8'
+        fstring = f"{speed}\n"
         if self.verbose:
             print(fstring)
         try:
             self.device.write(fstring.encode('utf-8'))
         except AttributeError:
             pass
         print(f"Spin speed (channel {self.channel}): {speed}")
@@ -230,32 +252,32 @@
     
     _default_flags = {
         'busy': False,
         'connected': False
     }
     
     def __init__(self, 
-        ports:list[str], 
-        channels:list[int], 
-        positions:list[tuple[float]], 
+        ports: list[str], 
+        channels: list[int], 
+        positions: list[tuple[float]],
         **kwargs
     ):
         """
         Instantiate the class
 
         Args:
             ports (list[str]): COM port addresses
             channels (list[int]): channel ids
             positions (list[tuple[float]]): x,y,z positions of spinners
         """
         super().__init__(**kwargs)
         self.channels = {}
         self._threads = {}
         
-        self._connect(port=ports, channel=channels, position=positions)
+        self._connect(port=ports, channel=channels, position=positions, verbose=self.verbose)
         return
 
     def disconnect(self):
         """Disconnect from device"""
         for channel in self.channels.values():
             channel.disconnect()
         return super().disconnect()
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,17 @@
         low = lower[-1] if len(lower) else frequencies[0]
         high = higher[0] if len(higher) else frequencies[-1]
         return Frequency(low, high)
     
     def _read(self) -> str:
         """
         Read response from device
+        
+        Raises:
+            RuntimeError: errors from device
 
         Returns:
             str: response string
         """
         response = ''
         try:
             response = self.device.readline()
@@ -275,14 +278,15 @@
             if self.verbose:
                 print(e)
         else:
             if len(response) and (self.verbose or 'High-Voltage' in response):
                 print(response)
             if response in ErrorCode._member_names_:
                 print(ErrorCode[response].value)
+                raise RuntimeError(ErrorCode[response].value)
         return response
     
     def _write(self, command:str) -> bool:
         """
         Write command to device
 
         Args:
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     - `run`: run the measurement program
     
     ==========
     
     ### Parameters:
         low_frequency (float): lower frequency limit to test
         high_frequency (float): upper frequency limit to test
-        sample_thickness (float): thickness of measured sample. Defaults to 1E-3.
+        sample_thickness (float): thickness of measured sample in [m]. Defaults to 1E-3.
         repeat (int): number of times to run the measurement. Defaults to 1.
         pause (bool): whether to pause for loading samples. Defaults to True.
     """
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/force_sensor_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This module holds the base class for cartesian mover tools.
 
 Classes:
     Gantry (Mover)
 """
 # Standard library imports
 from __future__ import annotations
+from abc import abstractmethod
 import numpy as np
 import time
 from typing import Optional
 
 # Third party imports
 import serial # pip install pyserial
 
@@ -34,14 +35,15 @@
     
     ### Properties
     - `limits` (np.ndarray):lower and upper limits of gantry
     - `port` (str): COM port address
     
     ### Methods
     #### Abstract
+    - `getSettings`: get hardware settings
     - `home`: make the robot go home
     #### Public
     - `disconnect`: disconnect from device
     - `isFeasible`: checks and returns whether the target coordinate is feasible
     - `moveBy`: move the robot by target direction
     - `moveTo`: move the robot to target position
     - `reset`: reset the robot
@@ -74,14 +76,23 @@
         if safe_height is not None:
             self.setHeight(safe=safe_height)
         
         self._connect(port)
         self.home()
         return
     
+    @abstractmethod
+    def getSettings(self) -> list[str]:
+        """
+        Get hardware settings
+
+        Returns:
+            list[str]: hardware settings
+        """
+    
     # Properties
     @property
     def limits(self) -> np.ndarray:
         return np.array(self._limits)
     @limits.setter
     def limits(self, value:list):
         if len(value) != 2 or any([len(row)!=3 for row in value]):
@@ -122,15 +133,15 @@
         """
         if transform_in:
             coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
         coordinates = np.array(coordinates)
         l_bound, u_bound = self.limits
         
         if all(np.greater_equal(coordinates, l_bound)) and all(np.less_equal(coordinates, u_bound)):
-            return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
+            return not self.deck.isExcluded(self._transform_out(coordinates, tool_offset=True))
         print(f"Range limits reached! {self.limits}")
         return False
 
     def moveBy(self, vector:tuple[float], **kwargs) -> bool:
         """
         Move the robot by target direction
 
@@ -245,15 +256,16 @@
         self._write(command)
         try:
             responses = self.device.readlines()
         except Exception as e:
             if self.verbose:
                 print(e)
         else:
-            print(responses)
+            if self.verbose:
+                print(responses)
         # self._handle_alarms_and_errors(response=response.decode())
         return [r.decode().strip() for r in responses]
 
     def _write(self, command:str) -> bool:
         """
         Write command to device
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/grbl_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/grbl_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the class for movement tools based on Primitiv.
+This module holds the class for movement tools based on Primitiv. (Grbl firmware)
 
 Classes:
     Primitiv (Gantry)
 """
 # Standard library imports
 from __future__ import annotations
 import time
@@ -24,16 +24,17 @@
     Args:
         `port` (str): COM port address
         `limits` (tuple[tuple[float]], optional): lower and upper limits of gantry. Defaults to ((-410,-290,-120), (0,0,0)).
         `safe_height` (float, optional): height at which obstacles can be avoided. Defaults to -80.
         `max_speed` (float, optional): maximum travel speed. Defaults to 250.
     
     ### Methods
-    - `home`: make the robot go home
+    - `getSettings`: get hardware settings
     - `getStatus`: get the current status of the tool
+    - `home`: make the robot go home
     - `stop`: stop movement immediately
     """
     def __init__(self, 
         port: str, 
         limits: tuple[tuple[float]] = ((-410,-290,-120), (0,0,0)), 
         safe_height: float = -80, 
         max_speed: float = 250, # [mm/s] (i.e. 15,000 mm/min)
@@ -47,14 +48,25 @@
             limits (tuple[tuple[float]], optional): lower and upper limits of gantry. Defaults to ((-410,-290,-120), (0,0,0)).
             safe_height (float, optional): height at which obstacles can be avoided. Defaults to -80.
             max_speed (float, optional): maximum travel speed. Defaults to 250.
         """
         super().__init__(port=port, limits=limits, safe_height=safe_height, max_speed=max_speed, **kwargs)
         return
     
+    def getSettings(self) -> list[str]:
+        """
+        Get hardware settings
+
+        Returns:
+            list[str]: hardware settings
+        """
+        responses = self._query("$$\n")
+        print(responses)
+        return responses
+    
     def getStatus(self) -> list[str]:
         """
         Get the current status of the tool
 
         Returns:
             list[str]: status output
         """
@@ -102,24 +114,14 @@
         else:
             self.device.open()
             # Start grbl 
             self._write("\r\n\r\n")
             time.sleep(2)
             self.device.reset_input_buffer()
         return
-    
-    def _get_settings(self) -> list[str]:
-        """
-        Get hardware settings
-
-        Returns:
-            list[str]: hardware settings
-        """
-        responses = self._query("$$\n")
-        return responses
 
     # def _handle_alarms_and_errors(self, response:str):
     #     """
     #     Handle the alarms and errors arising from the tool
         
     #     Args:
     #         response (str): string response from the tool
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,15 @@
             time.sleep(move_time+MOVE_TIME_BUFFER_S)
         self.updatePosition(orientation=absolute_angles[3:])
         return True
 
     def reset(self):
         """Reset the robot"""
         try:
+            self.dashboard.DisableRobot()
             self.dashboard.ClearError()
             self.dashboard.EnableRobot()
         except (AttributeError, OSError):
             if self.verbose:
                 print("Not connected to arm.")
         return
 
@@ -403,16 +404,23 @@
             if time.perf_counter() - start_time > timeout:
                 raise Exception(f"Unable to connect to arm at {ip_address}")
         except Exception as e:
             print(e)
         else:
             self.device = Device(dashboard, feedback)
             self.reset()
+        
+        try:
             self.dashboard.User(0)
             self.dashboard.Tool(0)
+        except OSError as e:
+            print(e)
+        except AttributeError as e:
+            print(e)
+        else:
             self.setSpeed(speed=100)
             self.setFlag(connected=True)
         return
 
     def _freeze(self):
         """Halt and disable robot"""
         try:
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     - `stretchArm`: extend the arm to full reach
     """
     
     _default_flags = {
         'busy': False,
         'connected': False,
         'retract': False, 
-        'right_handed': None
+        'right_handed': False,
+        'stretched': False
     }
     def __init__(self, 
         ip_address: str, 
         right_handed: bool = True, 
         safe_height: float = 100,
         home_coordinates: tuple[float] = (0,300,100), 
         **kwargs
@@ -60,15 +61,15 @@
         super().__init__(
             ip_address=ip_address, 
             safe_height=safe_height,
             home_coordinates=home_coordinates, 
             **kwargs
         )
         self._speed_angular_max = 180
-        self.setHandedness(right_hand=right_handed, stretch=True)
+        self.setHandedness(right_hand=right_handed, stretch=False)
         self.home()
         return
     
     def home(self, safe:bool = True, tool_offset:bool = False) -> bool:
         """
         Make the robot go home
 
@@ -118,19 +119,19 @@
         # Space constraints
         # if x > 344: # front edge
         #     return False
         # if x < 76 and abs(y) < 150: # elevated structure
         #     return False
         
         grad = abs(y/(x+1E-6))
-        gradient_threshold = 0.1
+        gradient_threshold = 0.25
         if grad > gradient_threshold or x < 0:
             right_hand = (y>0)
             self.setHandedness(right_hand=right_hand, stretch=True) 
-        return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
+        return not self.deck.isExcluded(self._transform_out(coordinates, tool_offset=True))
     
     def moveCoordBy(self, 
         vector: tuple[float] = (0,0,0), 
         angles: tuple[float] = (0,0,0)
     ) -> bool:
         """
         Relative Cartesian movement and tool orientation, using robot coordinates
@@ -172,28 +173,31 @@
             self.dashboard.SetArmOrientation(int(right_hand),1,1,1)
         except (AttributeError, OSError):
             if self.verbose:
                 print("Not connected to arm!")
         else:
             time.sleep(2)
             if stretch:
-                self.stretchArm()
+                # self.stretchArm()
                 time.sleep(1)
-        self.setFlag(right_handed=right_hand)
+            self.setFlag(right_handed=right_hand)
         return True
             
     def stretchArm(self) -> bool:
         """
         Extend the arm to full reach
         
         Returns:
             bool: whether movement is successful
         """
+        if self.flags['stretched']:
+            return False
         x,y,z = self.coordinates
         y_stretch = math.copysign(240, y)
         z_home = self.home_coordinates[2]
         ret1 = self.moveCoordTo(coordinates=(x,y,z_home))
         ret2 = self.moveCoordTo(coordinates=(320,y_stretch,z_home))
         ret3 = self.moveCoordTo(coordinates=(x,y,z_home))
         ret4 = self.moveCoordTo(coordinates=(x,y,z))
+        self.setFlag(stretched=True)
         return all([ret1,ret2,ret3,ret4])
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             j1 += (180 * math.copysign(1, x))
         if abs(j1) > 160:
             return False
         
         # Z-axis
         if not (-150 < z < 230):
             return False
-        return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
+        return not self.deck.isExcluded(self._transform_out(coordinates, tool_offset=True))
     
     def retractArm(self, target:Optional[tuple[float]] = None) -> bool:
         """
         Tuck in arm, rotate about base, then extend again
 
         Args:
             target (Optional[tuple[float]], optional): x,y,z coordinates of destination. Defaults to None.
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Move/move_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             coordinates (tuple[float]): target coordinates
             transform_in (bool, optional): whether to convert to internal coordinates first. Defaults to False.
             tool_offset (bool, optional): whether to convert from tool tip coordinates first. Defaults to False.
 
         Returns:
             bool: whether the target coordinate is feasible
         """
-        return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
+        return not self.deck.isExcluded(self._transform_out(coordinates, tool_offset=True))
     
     @abstractmethod
     def moveBy(self, 
         vector: tuple[float] = (0,0,0), 
         angles: tuple[float] = (0,0,0), 
         **kwargs
     ) -> bool:
@@ -460,23 +460,23 @@
         Returns:
             bool: whether the device is connected
         """
         if not self.flags.get('connected', False):
             print(f"{self.__class__} is not connected. Details: {self.connection_details}")
         return self.flags.get('connected', False)
  
-    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None):
+    def loadDeck(self, layout_file:Optional[str] = None, layout_dict:Optional[dict] = None, **kwargs):
         """
         Load Labware objects onto the deck from file or dictionary
         
         Args:
             layout_file (Optional[str], optional): filename of layout .json file. Defaults to None.
             layout_dict (Optional[dict], optional): dictionary of layout. Defaults to None.
         """
-        self.deck.load_layout(layout_file=layout_file, layout_dict=layout_dict)
+        self.deck.loadLayout(layout_file=layout_file, layout_dict=layout_dict, **kwargs)
         return
     
     def move(self, axis:str, value:float, speed:Optional[float] = None, **kwargs) -> bool:
         """
         Move the robot in a specific axis by a specific value
 
         Args:
@@ -546,15 +546,16 @@
         if coordinates is None:
             coordinates = self.tool_position if tool_offset else self.user_position
         if orientation is None:
             orientation = self.orientation
         coordinates = np.array(coordinates)
         orientation = np.array(orientation)
         
-        ret = self.move('z', max(0, self.home_coordinates[2]-self.coordinates[2]), speed=ascent_speed)
+        safe_height = self.home_coordinates[2] if 'safe' in self.heights else self.heights['safe']
+        ret = self.move('z', max(0, safe_height-self.coordinates[2]), speed=ascent_speed)
         success.append(ret)
         
         intermediate_position = self.tool_position if tool_offset else self.user_position
         ret = self.moveTo(
             coordinates=list(coordinates[:2])+[float(intermediate_position[0][2])], 
             orientation=orientation, 
             tool_offset=tool_offset
@@ -576,18 +577,17 @@
         """
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
-            raise ValueError("Ensure all assigned flag values are boolean.")
+            print(kwargs)
+            # raise ValueError("Ensure all assigned flag values are boolean.")
         self.flags.update(kwargs)
-        # for key, value in kwargs.items():
-        #     self.flags[key] = value
         return
     
     def setHeight(self, overwrite:bool = False, **kwargs):
         """
         Set predefined heights using keyword arguments
 
         Args:
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/image.py` & `control-lab-ly-1.1.1a2/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/factory.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 import importlib
 import inspect
 import numpy as np
 import pprint
 import sys
 from typing import Callable, Optional
 
-# Third party imports
-import yaml     # pip install pyyaml
-
 # Local application imports
 print(f"Import: OK <{__name__}>")
 
 HOME_PACKAGES = ['controllably','lab']
 """Names and aliases of base package"""
 
 class DottableDict(dict):
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/helper.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,28 @@
     get_plans
     get_ports
     is_overrun
     pretty_print_duration
     read_json
     read_yaml
     safety_measures (decorator)
+    update_root_directory
     zip_inputs
 
 Other constants and variables:
     safety_countdown (int)
     safety_mode (Optional[str])
 """
 # Standard library imports
 from __future__ import annotations
 from datetime import datetime
 import json
 import os
 import pandas as pd
+from pathlib import Path
 import pkgutil
 import time
 from typing import Callable, Optional
 import uuid
 
 # Third party imports
 import serial.tools.list_ports      # pip install pyserial
@@ -221,14 +223,29 @@
         func (Callable): function to be wrapped
 
     Returns:
         Callable: wrapped function
     """
     return decorators.safety_measures(mode=safety_mode, countdown=safety_countdown)(func=func)
 
+def update_root_directory(d: dict, repo:str):
+    """
+    Updates relative filepaths in library with root directory
+
+    Args:
+        d (dict): library of relative filepaths
+        repo (str): name of repository
+    """
+    root = str(Path().absolute()).split(repo)[0].replace('\\','/')
+    for k,v in list(d.items()):
+        if isinstance(v, dict):
+            update_root_directory(v, repo)
+        elif type(v) == str:
+            d[k] = v.replace(repo, f"{root}{repo}")
+            
 def zip_inputs(primary_keyword:str, **kwargs) -> dict:
     """
     Checks and zips multiple keyword arguments of lists into dictionary
     
     Args:
         primary_keyword (str): primary keyword to be used as key
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/layout.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/layout.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Deck
     Labware
     Well
 """
 # Standard library imports
 from __future__ import annotations
 import numpy as np
+from pathlib import Path
 from typing import Optional, Union
 
 # Local application imports
 from . import helper
 print(f"Import: OK <{__name__}>")
 
 class Well:
@@ -37,17 +38,17 @@
     - `depth` (float): well depth
     - `diameter` (float): well diameter
     - `middle` (np.ndarray): middle of well
     - `offset` (np.ndarray): well offset from Labware reference point
     - `top` (np.ndarray): top of well
     
     ### Methods
-    - `from_bottom`: offset from bottom of well
-    - `from_middle`: offset from middle of well
-    - `from_top`: offset from top of well
+    - `fromBottom`: offset from bottom of well
+    - `fromMiddle`: offset from middle of well
+    - `fromTop`: offset from top of well
     """
     
     def __init__(self, 
         labware_info: dict, 
         name: str, 
         details: dict[str, Union[float, tuple[float]]]
     ):
@@ -100,49 +101,88 @@
         return np.array((x,y,z))
     
     @property
     def top(self) -> np.ndarray:
         depth = self.details.get('depth', 0)
         return self.center + np.array((0,0,depth))
     
-    def from_bottom(self, offset:tuple[float]) -> np.ndarray:
+    def fromBottom(self, offset:tuple[float]) -> np.ndarray:
         """
         Offset from bottom of well
 
         Args:
             offset (tuple): x,y,z offset
 
         Returns:
             tuple: bottom of well with offset
         """
         return self.bottom + np.array(offset)
     
-    def from_middle(self, offset:tuple[float]) -> np.ndarray:
+    def fromMiddle(self, offset:tuple[float]) -> np.ndarray:
         """
         Offset from middle of well
 
         Args:
             offset (tuple): x,y,z offset
 
         Returns:
             tuple: middle of well with offset
         """
         return self.middle + np.array(offset)
     
-    def from_top(self, offset:tuple[float]) -> np.ndarray:
+    def fromTop(self, offset:tuple[float]) -> np.ndarray:
         """
         Offset from top of well
 
         Args:
             offset (tuple): x,y,z offset
 
         Returns:
             tuple: top of well with offset
         """
         return self.top + np.array(offset)
+    
+    def from_bottom(self, offset:tuple[float]) -> np.ndarray:
+        """
+        Offset from bottom of well
+
+        Args:
+            offset (tuple): x,y,z offset
+
+        Returns:
+            tuple: bottom of well with offset
+        """
+        print("'from_bottom()' method to be deprecated. Use 'fromBottom()' instead.")
+        return self.fromBottom(offset=offset)
+    
+    def from_middle(self, offset:tuple[float]) -> np.ndarray:
+        """
+        Offset from middle of well
+
+        Args:
+            offset (tuple): x,y,z offset
+
+        Returns:
+            tuple: middle of well with offset
+        """
+        print("'from_middle()' method to be deprecated. Use 'fromMiddle()' instead.")
+        return self.fromMiddle(offset=offset)
+    
+    def from_top(self, offset:tuple[float]) -> np.ndarray:
+        """
+        Offset from top of well
+
+        Args:
+            offset (tuple): x,y,z offset
+
+        Returns:
+            tuple: top of well with offset
+        """
+        print("'from_top()' method to be deprecated. Use 'fromTop()' instead.")
+        return self.fromTop(offset=offset)
 
 
 class Labware:
     """
     Labware represents a single Labware on the Deck
 
     ### Constructor
@@ -166,16 +206,16 @@
     - `reference_point` (np.ndarray): coordinates of bottom left corner of Labware
     - `rows` (dict[str, int]): Labware rows
     - `rows_list` (list[list[int]]): Labware rows as list
     - `wells` (dict[str, Well]): Labware wells
     - `wells_list` (list[Well]): Labware wells as list
     
     ### Methods
-    - `at`: alias for `get_well()`
-    - `get_well`: get `Well` using its name
+    - `at`: alias for `getWell()`
+    - `getWell`: get `Well` using its name
     """
     
     def __init__(self, 
         slot: str, 
         bottom_left_coordinates: tuple[float], 
         labware_file: str, 
         package: Optional[str] = None
@@ -256,36 +296,49 @@
     @property
     def wells_list(self) -> list[Well]:
         return [self._wells[well] for well in self.details.get('wells',{})]
 
     def at(self, name:str) -> Well:
         """
         Get `Well` using its name.
-        Alias for `get_well()`.
+        Alias for `getWell()`.
 
         Args:
             name (str): name of well
 
         Returns:
             Well: `Well` object
         """
-        return self.get_well(name=name)
+        return self.getWell(name=name)
     
-    def get_well(self, name:str) -> Well:
+    def getWell(self, name:str) -> Well:
         """
         Get `Well` using its name
 
         Args:
             name (str): name of well
 
         Returns:
             Well: `Well` object
         """
         return self.wells.get(name)
     
+    def get_well(self, name:str) -> Well:
+        """
+        Get `Well` using its name
+
+        Args:
+            name (str): name of well
+
+        Returns:
+            Well: `Well` object
+        """
+        print("'get_well()' method to be deprecated. Use 'getWell()' instead.")
+        return self.getWell(name=name)
+    
     # Protected method(s)
     def _load_wells(self):
         """Load wells into memory"""
         wells = self.details.get('wells',{})
         for well in wells:
             self._wells[well] = Well(labware_info=self.info, name=well, details=wells[well])
         return
@@ -305,65 +358,66 @@
     - `exclusion_zones` (dict): dictionary of cuboidal zones to avoid
     - `names` (dict): labels for deck slots
     
     ### Properties
     - `slots` (dict[str, Labware]): loaded Labware in slots
     
     ### Methods
-    - `at`: alias for `get_slot()`, with mixed input
-    - `get_slot`: get Labware in slot using slot id or name
-    - `is_excluded`: checks and returns whether the coordinates are in an excluded region
-    - `load_labware`: load Labware into slot
-    - `load_layout`: load deck layout from layout file
-    - `remove_labware`: remove Labware in slot using slot id or name
+    - `at`: alias for `getSlot()`, with mixed input
+    - `getSlot`: get Labware in slot using slot id or name
+    - `isExcluded`: checks and returns whether the coordinates are in an excluded region
+    - `loadLabware`: load Labware into slot
+    - `loadLayout`: load deck layout from layout file
+    - `removeLabware`: remove Labware in slot using slot id or name
     """
     
-    def __init__(self, layout_file:Optional[str] = None, package:Optional[str] = None):
+    def __init__(self, layout_file:Optional[str] = None, package:Optional[str] = None, repository:Optional[str] = None):
         """
         Instantiate the class
 
         Args:
             layout_file (Optional[str], optional): filepath of deck layout JSON file. Defaults to None.
             package (Optional[str], optional): name of package to look in. Defaults to None.
+            repository (Optional[str], optional): name of repository to look in. Defaults to None.
         """
         self.details = {}
         self._slots = {}
         self.names = {}
         self.exclusion_zones = {}
-        self.load_layout(layout_file=layout_file, package=package)
+        self.loadLayout(layout_file=layout_file, package=package, repository=repository)
         pass
     
     def __repr__(self) -> str:
         labwares = [''] + [repr(labware) for labware in self.slots.values()]
         labware_string = '\n'.join(labwares)
         return f"Deck with Labwares:{labware_string}" 
     
     @property
     def slots(self) -> dict[str, Labware]:
         return self._slots
     
     def at(self, slot:Union[int, str]) -> Optional[Labware]:
         """
         Get Labware in slot using slot id or name, with mixed input.
-        Alias for `get_slot()`.
+        Alias for `getSlot()`.
 
         Args:
             slot (Union[int, str]): id or name of slot
 
         Returns:
             Optional[Labware]: Labware in slot
         """
         if type(slot) == int:
-            return self.get_slot(index=slot)
+            return self.getSlot(index=slot)
         elif type(slot) == str:
-            return self.get_slot(name=slot)
+            return self.getSlot(name=slot)
         print("Input a valid slot id or name of Labware in slot.")
         return
     
-    def get_slot(self, index:Optional[int] = None, name:Optional[str] = None) -> Optional[Labware]:
+    def getSlot(self, index:Optional[int] = None, name:Optional[str] = None) -> Optional[Labware]:
         """
         Get Labware in slot using slot id or name
 
         Args:
             index (Optional[int], optional): slot id number. Defaults to None.
             name (Optional[str], optional): nickname of Labware. Defaults to None.
 
@@ -375,39 +429,39 @@
         """
         if not any((index, name)) or all((index, name)):
             raise ValueError('Please input either slot id or name.')
         if index is None and name is not None:
             index = self.names.get(name)
         return self._slots.get(str(index))
     
-    def is_excluded(self, coordinates:tuple[float]) -> bool:
+    def isExcluded(self, coordinates:tuple[float]) -> bool:
         """
         Checks and returns whether the coordinates are in an excluded region.
 
         Args:
             coordinates (tuple[float]): target coordinates
 
         Returns:
             bool: whether the coordinates are in an excluded region
         """
         coordinates = np.array(coordinates)
         for key, value in self.exclusion_zones.items():
             l_bound, u_bound = value
             if key == 'boundary':
-                if any(np.less_equal(coordinates, l_bound)) and any(np.greater_equal(coordinates, u_bound)):
+                if any(np.less(coordinates, l_bound)) and any(np.greater(coordinates, u_bound)):
                     print(f"Deck limits reached! {value}")
                     return True
                 continue
-            if all(np.greater_equal(coordinates, l_bound)) and all(np.less_equal(coordinates, u_bound)):
+            if all(np.greater(coordinates, l_bound)) and all(np.less(coordinates, u_bound)):
                 name = [k for k,v in self.names.items() if str(v)==key][0] if key in self.names.values() else f'Labware in Slot {key}'
                 print(f"{name} is in the way! {value}")
                 return True
         return False
     
-    def load_labware(self, 
+    def loadLabware(self, 
         slot: int, 
         labware_file: str, 
         package: Optional[str] = None, 
         name: Optional[str] = None, 
         exclusion_height: Optional[float] = None
     ):
         """
@@ -426,54 +480,57 @@
         labware = Labware(slot=str(slot), bottom_left_coordinates=bottom_left_coordinates, labware_file=labware_file, package=package)
         self._slots[str(slot)] = labware
         if exclusion_height is not None:
             top_right_coordinates= tuple(map(sum, zip(bottom_left_coordinates, labware.dimensions, (0,0,exclusion_height))))
             self.exclusion_zones[str(slot)] = (bottom_left_coordinates, top_right_coordinates)
         return
     
-    def load_layout(
+    def loadLayout(
         self, 
         layout_file: Optional[str] = None, 
         layout_dict: Optional[dict] = None, 
         package: Optional[str] = None, 
-        labware_package: Optional[str] = None
+        labware_package: Optional[str] = None,
+        repository: str = 'control-lab-le'
     ):
         """
         Load deck layout from layout file
 
         Args:
             layout_file (Optional[str], optional): filepath of deck layout JSON file. Defaults to None.
             layout_dict (Optional[dict], optional): layout details. Defaults to None.
             package (Optional[str], optional): name of package to look in for layout file. Defaults to None.
             labware_package (Optional[str], optional): name of package to look in for Labware file. Defaults to None.
+            repository (str, optional): name of repository to look in. Defaults to 'control-lab-le'.
 
         Raises:
             Exception: lease input either `layout_file` or `layout_dict`
         """
         if layout_file is None and layout_dict is None:
             return
         elif layout_file is not None and layout_dict is not None:
             raise Exception("Please input either `layout_file` or `layout_dict`.")
-            print()
         elif layout_file is not None:
             self.details = helper.read_json(json_file=layout_file, package=package)
         else:
             self.details = layout_dict
         
         slots = self.details.get('slots', {})
+        root = str(Path().absolute()).split(repository)[0].replace('\\','/')
         for slot in sorted(list(slots)):
             info = slots[slot]
             name = info.get('name')
             labware_file = info.get('filepath','')
+            labware_file = labware_file if Path(labware_file).is_absolute() else f"{root}{repository}/{labware_file.split(repository)[1]}"
             exclusion_height = info.get('exclusion_height', -1)
             exclusion_height = exclusion_height if exclusion_height >= 0 else None
-            self.load_labware(slot=slot, name=name, exclusion_height=exclusion_height, labware_file=labware_file, package=labware_package)
+            self.loadLabware(slot=slot, name=name, exclusion_height=exclusion_height, labware_file=labware_file, package=labware_package)
         return
 
-    def remove_labware(self, index:Optional[int] = None, name:Optional[str] = None):
+    def removeLabware(self, index:Optional[int] = None, name:Optional[str] = None):
         """
         Remove Labware in slot using slot id or name
 
         Args:
             index (Optional[int], optional): slot id. Defaults to None.
             name (Optional[str], optional): nickname of Labware. Defaults to None.
 
@@ -486,11 +543,97 @@
             index = self.names.get(name)
         elif index is not None and name is None:
             name = [k for k,v in self.names.items() if v==index][0]
         self.names.pop(name)
         self._slots.pop(str(index))
         self.exclusion_zones.pop(str(index))
         return
+    
+    def get_slot(self, index:Optional[int] = None, name:Optional[str] = None) -> Optional[Labware]:
+        """
+        Get Labware in slot using slot id or name
+
+        Args:
+            index (Optional[int], optional): slot id number. Defaults to None.
+            name (Optional[str], optional): nickname of Labware. Defaults to None.
+
+        Raises:
+            ValueError: Please input either slot id or name
+
+        Returns:
+            Optional[Labware]: Labware in slot
+        """
+        print("'get_slot()' method to be deprecated. Use 'getSlot()' instead.")
+        return self.getSlot(index=index, name=name)
+    
+    def is_excluded(self, coordinates:tuple[float]) -> bool:
+        """
+        Checks and returns whether the coordinates are in an excluded region.
+
+        Args:
+            coordinates (tuple[float]): target coordinates
+
+        Returns:
+            bool: whether the coordinates are in an excluded region
+        """
+        print("'is_excluded()' method to be deprecated. Use 'isExcluded()' instead.")
+        return self.isExcluded(coordinates=coordinates)
+    
+    def load_labware(self, 
+        slot: int, 
+        labware_file: str, 
+        package: Optional[str] = None, 
+        name: Optional[str] = None, 
+        exclusion_height: Optional[float] = None
+    ):
+        """
+        Load Labware into slot
+
+        Args:
+            slot (int): slot id
+            labware_file (str): filepath Labware JSON file
+            package (Optional[str], optional): name of package to look in. Defaults to None.
+            name (Optional[str], optional): nickname of Labware. Defaults to None.
+            exclusion_height (Optional[float], optional): height clearance from top of Labware. Defaults to None.
+        """
+        print("'load_labware()' method to be deprecated. Use 'loadLabware()' instead.")
+        return self.loadLabware(slot=slot, labware_file=labware_file, package=package, name=name, exclusion_height=exclusion_height)
+    
+    def load_layout(
+        self, 
+        layout_file: Optional[str] = None, 
+        layout_dict: Optional[dict] = None, 
+        package: Optional[str] = None, 
+        labware_package: Optional[str] = None
+    ):
+        """
+        Load deck layout from layout file
+
+        Args:
+            layout_file (Optional[str], optional): filepath of deck layout JSON file. Defaults to None.
+            layout_dict (Optional[dict], optional): layout details. Defaults to None.
+            package (Optional[str], optional): name of package to look in for layout file. Defaults to None.
+            labware_package (Optional[str], optional): name of package to look in for Labware file. Defaults to None.
+
+        Raises:
+            Exception: lease input either `layout_file` or `layout_dict`
+        """
+        print("'load_layout()' method to be deprecated. Use 'loadLayout()' instead.")
+        return self.loadLayout(layout_file=layout_file, layout_dict=layout_dict, package=package, labware_package=labware_package)
+
+    def remove_labware(self, index:Optional[int] = None, name:Optional[str] = None):
+        """
+        Remove Labware in slot using slot id or name
+
+        Args:
+            index (Optional[int], optional): slot id. Defaults to None.
+            name (Optional[str], optional): nickname of Labware. Defaults to None.
+
+        Raises:
+            Exception: Please input either slot id or name
+        """
+        print("'remove_labware()' method to be deprecated. Use 'removeLabware()' instead.")
+        return self.removeLabware(index=index, name=name)
 
 __where__ = "misc.Layout"
 from .factory import include_this_module
 include_this_module(get_local_only=True)
```

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/logger.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

