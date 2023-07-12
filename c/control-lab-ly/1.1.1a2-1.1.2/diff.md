# Comparing `tmp/control-lab-ly-1.1.1a2.tar.gz` & `tmp/control-lab-ly-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.1.1a2.tar", last modified: Wed Jul 12 02:31:34 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.2.tar", last modified: Wed Jul 12 08:31:31 2023, max compression
```

## Comparing `control-lab-ly-1.1.1a2.tar` & `control-lab-ly-1.1.2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.510639 control-lab-ly-1.1.1a2/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a2/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/MANIFEST.in
--rw-rw-rw-   0        0        0    22652 2023-07-12 02:31:34.510639 control-lab-ly-1.1.1a2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.374766 control-lab-ly-1.1.1a2/docs/
--rw-rw-rw-   0        0        0     8422 2023-07-12 02:28:37.000000 control-lab-ly-1.1.1a2/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.1a2/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a2/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13112 2023-07-03 05:57:22.000000 control-lab-ly-1.1.1a2/docs/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.379147 control-lab-ly-1.1.1a2/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a2/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/pyproject.toml
--rw-rw-rw-   0        0        0     1500 2023-07-12 02:31:34.516964 control-lab-ly-1.1.1a2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.193040 control-lab-ly-1.1.1a2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.410646 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    22652 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7085 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 02:31:33.000000 control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.423055 control-lab-ly-1.1.1a2/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.432521 control-lab-ly-1.1.1a2/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.445309 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.495690 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17940 2023-07-10 07:55:52.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.1.1a2/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.504148 control-lab-ly-1.1.1a2/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.538952 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.607154 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16416 2023-06-23 06:16:42.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     3780 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.638900 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14530 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.1a2/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.654615 control-lab-ly-1.1.1a2/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.672235 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11192 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.687709 control-lab-ly-1.1.1a2/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9890 2023-06-21 10:05:07.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.708790 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.733749 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.762014 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.778346 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    11490 2023-07-12 02:08:44.000000 control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.811272 control-lab-ly-1.1.1a2/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.825071 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.852389 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      359 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18010 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     1993 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.870927 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      287 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10637 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.880555 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.905328 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10508 2023-07-04 08:31:36.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.920497 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3549 2023-07-03 07:23:35.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.937808 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-06-26 05:50:00.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8358 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8199 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14473 2023-06-27 03:07:03.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.945409 control-lab-ly-1.1.1a2/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.977340 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9703 2023-07-12 02:05:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     6196 2023-07-12 02:12:03.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     6355 2023-06-22 05:19:20.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/grbl_lib.py
--rw-rw-rw-   0        0        0     4942 2023-07-12 02:11:52.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:33.992587 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.024460 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.073979 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24280 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15969 2023-07-03 02:34:15.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7266 2023-07-06 09:52:37.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4324 2023-07-03 05:56:38.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10566 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32435 2023-07-06 09:48:51.000000 control-lab-ly-1.1.1a2/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.088180 control-lab-ly-1.1.1a2/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.110566 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.127031 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.154362 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.174683 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    32163 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.182616 control-lab-ly-1.1.1a2/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.195913 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.213987 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8844 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.261011 control-lab-ly-1.1.1a2/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.275873 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.292440 control-lab-ly-1.1.1a2/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.306759 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.319784 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.326364 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.388415 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-06-22 09:26:34.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0     1836 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.396163 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2988 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    15898 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.440271 control-lab-ly-1.1.1a2/src/controllably/misc/
--rw-rw-rw-   0        0        0      627 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9533 2023-07-03 06:07:16.000000 control-lab-ly-1.1.1a2/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     8498 2023-07-03 06:52:23.000000 control-lab-ly-1.1.1a2/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    23175 2023-07-05 07:05:03.000000 control-lab-ly-1.1.1a2/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4543 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a2/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.446344 control-lab-ly-1.1.1a2/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.461248 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.477926 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.497052 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-07-12 02:31:34.507041 control-lab-ly-1.1.1a2/tests/
--rw-rw-rw-   0        0        0      398 2023-07-03 06:53:18.000000 control-lab-ly-1.1.1a2/tests/test_init.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.217659 control-lab-ly-1.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    22729 2023-07-12 08:31:31.217659 control-lab-ly-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.642497 control-lab-ly-1.1.2/docs/
+-rw-rw-rw-   0        0        0     8501 2023-07-12 08:29:11.000000 control-lab-ly-1.1.2/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.2/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.2/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13112 2023-07-03 05:57:22.000000 control-lab-ly-1.1.2/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.648497 control-lab-ly-1.1.2/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.1.2/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1497 2023-07-12 08:31:31.219658 control-lab-ly-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.520622 control-lab-ly-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.667083 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    22729 2023-07-12 08:31:30.000000 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7085 2023-07-12 08:31:30.000000 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:31:30.000000 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-07-12 08:31:30.000000 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 08:31:30.000000 control-lab-ly-1.1.2/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.670154 control-lab-ly-1.1.2/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.677960 control-lab-ly-1.1.2/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.686151 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.697587 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17940 2023-07-10 07:55:52.000000 control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.1.2/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.700582 control-lab-ly-1.1.2/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.720042 control-lab-ly-1.1.2/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.741042 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16416 2023-06-23 06:16:42.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     3780 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.757044 control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14530 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.2/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.767634 control-lab-ly-1.1.2/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.776633 control-lab-ly-1.1.2/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11192 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.786633 control-lab-ly-1.1.2/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9890 2023-06-21 10:05:07.000000 control-lab-ly-1.1.2/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.790634 control-lab-ly-1.1.2/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.799623 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.810315 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.820868 control-lab-ly-1.1.2/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    11489 2023-07-12 03:09:07.000000 control-lab-ly-1.1.2/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.835979 control-lab-ly-1.1.2/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.842263 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.856977 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      359 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18010 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     1993 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.870122 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      287 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10637 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.878032 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.898785 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10508 2023-07-04 08:31:36.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.911572 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3549 2023-07-03 07:23:35.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.933412 control-lab-ly-1.1.2/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-06-26 05:50:00.000000 control-lab-ly-1.1.2/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8358 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8199 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14473 2023-06-27 03:07:03.000000 control-lab-ly-1.1.2/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.942979 control-lab-ly-1.1.2/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.967787 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9737 2023-07-12 07:32:55.000000 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     6191 2023-07-12 02:48:47.000000 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     6355 2023-06-22 05:19:20.000000 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/grbl_lib.py
+-rw-rw-rw-   0        0        0     4789 2023-07-12 07:34:06.000000 control-lab-ly-1.1.2/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.975602 control-lab-ly-1.1.2/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:30.987391 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.002449 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15969 2023-07-03 02:34:15.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7266 2023-07-06 09:52:37.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4324 2023-07-03 05:56:38.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10566 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32435 2023-07-06 09:48:51.000000 control-lab-ly-1.1.2/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.011049 control-lab-ly-1.1.2/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.020687 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.032676 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.042685 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.056296 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    32163 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.063292 control-lab-ly-1.1.2/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.072354 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.083942 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.2/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.095302 control-lab-ly-1.1.2/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.101304 control-lab-ly-1.1.2/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.105311 control-lab-ly-1.1.2/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.117112 control-lab-ly-1.1.2/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.2/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.124358 control-lab-ly-1.1.2/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.132358 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.150186 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-06-22 09:26:34.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0     1836 2023-06-27 03:00:08.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.158734 control-lab-ly-1.1.2/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2988 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    15898 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.180364 control-lab-ly-1.1.2/src/controllably/misc/
+-rw-rw-rw-   0        0        0      627 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9533 2023-07-03 06:07:16.000000 control-lab-ly-1.1.2/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     8498 2023-07-03 06:52:23.000000 control-lab-ly-1.1.2/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    23175 2023-07-05 07:05:03.000000 control-lab-ly-1.1.2/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4543 2023-06-15 06:52:39.000000 control-lab-ly-1.1.2/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.184363 control-lab-ly-1.1.2/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.189488 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.199487 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.211469 control-lab-ly-1.1.2/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.2/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-07-12 08:31:31.215469 control-lab-ly-1.1.2/tests/
+-rw-rw-rw-   0        0        0      398 2023-07-03 06:53:18.000000 control-lab-ly-1.1.2/tests/test_init.py
```

### Comparing `control-lab-ly-1.1.1a2/LICENSE.md` & `control-lab-ly-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/PKG-INFO` & `control-lab-ly-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.1a2
+Version: 1.1.2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -358,15 +358,20 @@
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
 ## Version 1.1.1
-Bug fixes and patches. First released 30 Jun 2023.
+### Changed
+- fix bug with `Cartesian` changing speeds
+
+
+## Version 1.1.1
+Bug fixes and patches. First released 12 Jul 2023.
 ### Added
 - import `Device` classes in init files to view documentation
 - added library for GRBL status and error codes
 - add `update_root_direcctory()` function to Helper
 ### Changed
 - fix bug with adding new rows into Dataframes
 - initialise `PiezoRoboticsDevice` upon connection
```

### Comparing `control-lab-ly-1.1.1a2/docs/CHANGELOG.md` & `control-lab-ly-1.1.2/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
 ## Version 1.1.1
-Bug fixes and patches. First released 30 Jun 2023.
+### Changed
+- fix bug with `Cartesian` changing speeds
+
+
+## Version 1.1.1
+Bug fixes and patches. First released 12 Jul 2023.
 ### Added
 - import `Device` classes in init files to view documentation
 - added library for GRBL status and error codes
 - add `update_root_direcctory()` function to Helper
 ### Changed
 - fix bug with adding new rows into Dataframes
 - initialise `PiezoRoboticsDevice` upon connection
```

### Comparing `control-lab-ly-1.1.1a2/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/docs/LICENSE.md` & `control-lab-ly-1.1.2/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/docs/README.md` & `control-lab-ly-1.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/docs/assets/Documentation guide.png` & `control-lab-ly-1.1.2/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/setup.cfg` & `control-lab-ly-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
-00000030: 2e31 2d61 320d 0a64 6573 6372 6970 7469  .1-a2..descripti
-00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
-00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
-00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
-00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
-00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
-000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000d0: 0d0a 6175 7468 6f72 203d 2043 6861 6e67  ..author = Chang
-000000e0: 204a 6965 204c 656f 6e67 0d0a 6175 7468   Jie Leong..auth
-000000f0: 6f72 5f65 6d61 696c 203d 2063 6861 6e67  or_email = chang
-00000100: 6a69 652e 6c65 6f6e 6740 6f75 746c 6f6f  jie.leong@outloo
-00000110: 6b2e 636f 6d0d 0a75 726c 203d 2068 7474  k.com..url = htt
-00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000130: 6b79 6c65 6a65 616e 6c65 7769 732f 636f  kylejeanlewis/co
-00000140: 6e74 726f 6c2d 6c61 622d 6c65 0d0a 7072  ntrol-lab-le..pr
-00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000160: 4769 7448 7562 203d 2068 7474 7073 3a2f  GitHub = https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
-00000180: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
-00000190: 6c2d 6c61 622d 6c65 0d0a 0944 6f63 756d  l-lab-le...Docum
-000001a0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
-000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
-000001c0: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
-000001d0: 726f 6c2d 6c61 622d 6c65 2f62 6c6f 622f  rol-lab-le/blob/
-000001e0: 6d61 696e 2f64 6f63 732f 5245 4144 4d45  main/docs/README
-000001f0: 2e6d 640d 0a09 4368 616e 6765 6c6f 6720  .md...Changelog 
-00000200: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000210: 2e63 6f6d 2f6b 796c 656a 6561 6e6c 6577  .com/kylejeanlew
-00000220: 6973 2f63 6f6e 7472 6f6c 2d6c 6162 2d6c  is/control-lab-l
-00000230: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
-00000240: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a09  /CHANGELOG.md...
-00000250: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
-00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-00000270: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-00000280: 6f6c 2d6c 6162 2d6c 652f 6973 7375 6573  ol-lab-le/issues
-00000290: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
-000002a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
-000002b0: 7974 686f 6e0d 0a09 6c61 6220 6175 746f  ython...lab auto
-000002c0: 6d61 7469 6f6e 0d0a 636c 6173 7369 6669  mation..classifi
-000002d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000002e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000002f0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
-00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000340: 6368 0d0a 094c 6963 656e 7365 203a 3a20  ch...License :: 
-00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000360: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-00000370: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000380: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
-00000390: 696e 646f 7773 0d0a 0950 726f 6772 616d  indows...Program
-000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003e0: 2033 2e38 0d0a 0954 6f70 6963 203a 3a20   3.8...Topic :: 
-000003f0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
-00000400: 6565 7269 6e67 0d0a 0d0a 5b6f 7074 696f  eering....[optio
-00000410: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-00000420: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-00000440: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000450: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
-00000460: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000470: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
-00000480: 7569 7265 7320 3d20 0d0a 0969 6d75 7469  uires = ...imuti
-00000490: 6c73 3e3d 302e 350d 0a09 4d61 726b 646f  ls>=0.5...Markdo
-000004a0: 776e 3e3d 332e 330d 0a09 6e75 6d70 793e  wn>=3.3...numpy>
-000004b0: 3d31 2e31 390d 0a09 6f70 656e 6376 5f70  =1.19...opencv_p
-000004c0: 7974 686f 6e3e 3d34 2e35 2e30 0d0a 0970  ython>=4.5.0...p
-000004d0: 616e 6461 733e 3d31 2e32 0d0a 0970 794d  andas>=1.2...pyM
-000004e0: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
-000004f0: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
-00000500: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
-00000510: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
-00000520: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
-00000530: 0974 6b68 746d 6c76 6965 773e 3d30 2e32  .tkhtmlview>=0.2
-00000540: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000550: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000560: 7265 203d 2073 7263 0d0a 6578 636c 7564  re = src..exclud
-00000570: 6520 3d20 7465 7374 730d 0a0d 0a5b 6f70  e = tests....[op
-00000580: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-00000590: 7461 5d0d 0a2a 203d 202a 2e6a 736f 6e2c  ta]..* = *.json,
-000005a0: 202a 2e79 616d 6c2c 202a 2e70 6e67 0d0a   *.yaml, *.png..
-000005b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000005c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000005d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 2e32 0d0a 6465 7363 7269 7074 696f 6e20  .2..description 
+00000040: 3d20 4c61 6220 4571 7569 706d 656e 7420  = Lab Equipment 
+00000050: 4175 746f 6d61 7469 6f6e 2050 6163 6b61  Automation Packa
+00000060: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
+00000070: 7469 6f6e 203d 2066 696c 653a 2064 6f63  tion = file: doc
+00000080: 732f 5245 4144 4d45 2e6d 642c 2064 6f63  s/README.md, doc
+00000090: 732f 4348 414e 4745 4c4f 472e 6d64 0d0a  s/CHANGELOG.md..
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000c0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
+000000d0: 7574 686f 7220 3d20 4368 616e 6720 4a69  uthor = Chang Ji
+000000e0: 6520 4c65 6f6e 670d 0a61 7574 686f 725f  e Leong..author_
+000000f0: 656d 6169 6c20 3d20 6368 616e 676a 6965  email = changjie
+00000100: 2e6c 656f 6e67 406f 7574 6c6f 6f6b 2e63  .leong@outlook.c
+00000110: 6f6d 0d0a 7572 6c20 3d20 6874 7470 733a  om..url = https:
+00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+00000130: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+00000140: 6f6c 2d6c 6162 2d6c 650d 0a70 726f 6a65  ol-lab-le..proje
+00000150: 6374 5f75 726c 7320 3d20 0d0a 0947 6974  ct_urls = ...Git
+00000160: 4875 6220 3d20 6874 7470 733a 2f2f 6769  Hub = https://gi
+00000170: 7468 7562 2e63 6f6d 2f6b 796c 656a 6561  thub.com/kylejea
+00000180: 6e6c 6577 6973 2f63 6f6e 7472 6f6c 2d6c  nlewis/control-l
+00000190: 6162 2d6c 650d 0a09 446f 6375 6d65 6e74  ab-le...Document
+000001a0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+000001b0: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
+000001c0: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
+000001d0: 2d6c 6162 2d6c 652f 626c 6f62 2f6d 6169  -lab-le/blob/mai
+000001e0: 6e2f 646f 6373 2f52 4541 444d 452e 6d64  n/docs/README.md
+000001f0: 0d0a 0943 6861 6e67 656c 6f67 203d 2068  ...Changelog = h
+00000200: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000210: 6d2f 6b79 6c65 6a65 616e 6c65 7769 732f  m/kylejeanlewis/
+00000220: 636f 6e74 726f 6c2d 6c61 622d 6c65 2f62  control-lab-le/b
+00000230: 6c6f 622f 6d61 696e 2f64 6f63 732f 4348  lob/main/docs/CH
+00000240: 414e 4745 4c4f 472e 6d64 0d0a 0954 7261  ANGELOG.md...Tra
+00000250: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000260: 6974 6875 622e 636f 6d2f 6b79 6c65 6a65  ithub.com/kyleje
+00000270: 616e 6c65 7769 732f 636f 6e74 726f 6c2d  anlewis/control-
+00000280: 6c61 622d 6c65 2f69 7373 7565 730d 0a6c  lab-le/issues..l
+00000290: 6963 656e 7365 203d 204d 4954 0d0a 6b65  icense = MIT..ke
+000002a0: 7977 6f72 6473 203d 200d 0a09 7079 7468  ywords = ...pyth
+000002b0: 6f6e 0d0a 096c 6162 2061 7574 6f6d 6174  on...lab automat
+000002c0: 696f 6e0d 0a63 6c61 7373 6966 6965 7273  ion..classifiers
+000002d0: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
+000002e0: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+000002f0: 416c 7068 610d 0a09 496e 7465 6e64 6564  Alpha...Intended
+00000300: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000310: 656c 6f70 6572 730d 0a09 496e 7465 6e64  elopers...Intend
+00000320: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000330: 6369 656e 6365 2f52 6573 6561 7263 680d  cience/Research.
+00000340: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000350: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+00000360: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+00000370: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+00000380: 6963 726f 736f 6674 203a 3a20 5769 6e64  icrosoft :: Wind
+00000390: 6f77 730d 0a09 5072 6f67 7261 6d6d 696e  ows...Programmin
+000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003b0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+000003c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000003e0: 380d 0a09 546f 7069 6320 3a3a 2053 6369  8...Topic :: Sci
+000003f0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000400: 696e 670d 0a0d 0a5b 6f70 7469 6f6e 735d  ing....[options]
+00000410: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000420: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+00000430: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
+00000440: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00000450: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
+00000460: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000470: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000480: 6573 203d 200d 0a09 696d 7574 696c 733e  es = ...imutils>
+00000490: 3d30 2e35 0d0a 094d 6172 6b64 6f77 6e3e  =0.5...Markdown>
+000004a0: 3d33 2e33 0d0a 096e 756d 7079 3e3d 312e  =3.3...numpy>=1.
+000004b0: 3139 0d0a 096f 7065 6e63 765f 7079 7468  19...opencv_pyth
+000004c0: 6f6e 3e3d 342e 352e 300d 0a09 7061 6e64  on>=4.5.0...pand
+000004d0: 6173 3e3d 312e 320d 0a09 7079 4d6f 6462  as>=1.2...pyModb
+000004e0: 7573 5443 503e 3d30 2e32 0d0a 0970 7973  usTCP>=0.2...pys
+000004f0: 6572 6961 6c3e 3d33 2e35 0d0a 0950 7953  erial>=3.5...PyS
+00000500: 696d 706c 6547 5549 3e3d 342e 3630 0d0a  impleGUI>=4.60..
+00000510: 0950 7956 4953 413e 3d31 2e31 320d 0a09  .PyVISA>=1.12...
+00000520: 5079 5941 4d4c 3e3d 362e 300d 0a09 746b  PyYAML>=6.0...tk
+00000530: 6874 6d6c 7669 6577 3e3d 302e 320d 0a0d  htmlview>=0.2...
+00000540: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000550: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+00000560: 3d20 7372 630d 0a65 7863 6c75 6465 203d  = src..exclude =
+00000570: 2074 6573 7473 0d0a 0d0a 5b6f 7074 696f   tests....[optio
+00000580: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000590: 0d0a 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e  ..* = *.json, *.
+000005a0: 7961 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b  yaml, *.png....[
+000005b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000005c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000005d0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.2/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.1a2
+Version: 1.1.2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -358,15 +358,20 @@
 
 ## Unreleased
 *Items under development*
 ### 1.2.0
 - Integration for mass balance from Sartorius
 
 ## Version 1.1.1
-Bug fixes and patches. First released 30 Jun 2023.
+### Changed
+- fix bug with `Cartesian` changing speeds
+
+
+## Version 1.1.1
+Bug fixes and patches. First released 12 Jul 2023.
 ### Added
 - import `Device` classes in init files to view documentation
 - added library for GRBL status and error codes
 - add `update_root_direcctory()` function to Helper
 ### Changed
 - fix bug with adding new rows into Dataframes
 - initialise `PiezoRoboticsDevice` upon connection
```

### Comparing `control-lab-ly-1.1.1a2/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.2/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.2/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.2/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/__init__.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/maker_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/mover_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/loader_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/pop_ups.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/Elements/templates.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/guide_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Control/GUI/multichannel_panel.py` & `control-lab-ly-1.1.2/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.2/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.2/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.1.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.2/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
         Returns:
             list[str]: list of response string(s) from device
         """
         responses = [b'']
         self._write(command)
         try:
-            responses = self.device.readlines()
+            responses = self.device.readline()
         except Exception as e:
             if self.verbose:
                 print(e)
         else:
             if self.verbose:
                 print(responses)
         return
```

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.2/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/Physical/force_sensor_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.2/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.2/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.limits = limits
         self._speed_max = max_speed
         if safe_height is not None:
             self.setHeight(safe=safe_height)
         
         self._connect(port)
         self.home()
+        self.setSpeed(self._speed_max)
         return
     
     @abstractmethod
     def getSettings(self) -> list[str]:
         """
         Get hardware settings
 
@@ -172,15 +173,15 @@
         z_first = True if (self.coordinates[2] < coordinates[2]) else False
         positionXY = f'X{coordinates[0]}Y{coordinates[1]}'
         position_Z = f'Z{coordinates[2]}'
         moves = [position_Z, positionXY] if z_first else [positionXY, position_Z]
         
         self._query("G90\n")
         for move in moves:
-            self._query(f"G0 {move}\n")
+            self._query(f"G01 {move}\n")
         self._query("G90\n")
         
         distances = abs(self.coordinates - coordinates)
         times = distances / self.speed
         move_time = max(times[:2]) + times[2]
         time.sleep(move_time)
         self.updatePosition(coordinates=coordinates)
@@ -199,18 +200,18 @@
         Args:
             speed (int): speed in mm/s
         
         Returns:
             tuple[bool, float]: whether speed has changed; speed
         """
         print(f'Speed: {speed} mm/s')
-        # self._speed_fraction = (speed/self._speed_max)
-        # speed = int(self._speed_max*self._speed_fraction * 60)   # get speed in mm/min
-        # self._query(f"G01 F{speed}\n")  # feed rate (i.e. speed) in mm/min
-        return False, self.speed
+        self._speed_fraction = (speed/self._speed_max)
+        speed = int(self._speed_max*self._speed_fraction * 60)   # get speed in mm/min
+        self._query(f"G01 F{speed}\n")  # feed rate (i.e. speed) in mm/min
+        return True, self.speed
     
     def shutdown(self):
         """Shutdown procedure for tool"""
         # self.home()
         return super().shutdown()
     
     # Protected method(s)
```

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             print(f'Please select a temperature between {self.temperature_range[0]} and {self.temperature_range[1]}°C.')
             return False
         set_temperature = round( min(max(set_temperature,0), 110) )
         command = f'M190 R{set_temperature}\n' if blocking else f'M140 S{set_temperature}\n'
         
         print(f"New set temperature at {set_temperature}°C")
         if blocking:
-            print(f"Waiting for temperature to reach {self.set_temperature}°C")
+            print(f"Waiting for temperature to reach {set_temperature}°C")
         try:
             self._query(command)
         except Exception as e:
             print('Unable to heat stage!')
             if self.verbose:
                 print(e)
             return
```

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/grbl_lib.py` & `control-lab-ly-1.1.2/src/controllably/Move/Cartesian/grbl_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,18 +82,14 @@
     def home(self) -> bool:
         """Make the robot go home"""
         self._query("$H\n")
         self.coordinates = self.home_coordinates
         print("Homed")
         return True
     
-    def setSpeed(self, speed: int):
-        print("`setSpeed` method not available in `Primitiv` class")
-        return super().setSpeed(speed)
-    
     def stop(self):
         """Stop movement immediately"""
         self._query("!\n")
         return
 
     # Protected method(s)
     def _connect(self, port:str, baudrate:int = 115200, timeout:Optional[int] = 0.1):
```

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.2/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.2/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.2/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/Flir/ax8_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/Flir/ax8_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/image.py` & `control-lab-ly-1.1.2/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.2/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.2/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.2/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/factory.py` & `control-lab-ly-1.1.2/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/helper.py` & `control-lab-ly-1.1.2/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/layout.py` & `control-lab-ly-1.1.2/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/logger.py` & `control-lab-ly-1.1.2/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.2/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.2/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.2/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.2/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.1a2/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.2/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

