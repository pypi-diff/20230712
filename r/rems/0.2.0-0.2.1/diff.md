# Comparing `tmp/rems-0.2.0.tar.gz` & `tmp/rems-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rems-0.2.0.tar", last modified: Tue Jul  4 20:10:04 2023, max compression
+gzip compressed data, was "rems-0.2.1.tar", last modified: Wed Jul 12 19:54:27 2023, max compression
```

## Comparing `rems-0.2.0.tar` & `rems-0.2.1.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.364946 rems-0.2.0/
--rw-rw-rw-   0        0        0      498 2023-07-04 20:10:04.364946 rems-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4874 2023-07-04 19:17:53.000000 rems-0.2.0/ReadMe.md
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.364946 rems-0.2.0/rems/
--rw-rw-rw-   0        0        0      462 2023-07-03 02:24:52.000000 rems-0.2.0/rems/Config.py
--rw-rw-rw-   0        0        0     8193 2023-07-04 19:15:40.000000 rems-0.2.0/rems/Operator.py
--rw-rw-rw-   0        0        0      639 2023-07-03 02:24:52.000000 rems-0.2.0/rems/__init__.py
--rw-rw-rw-   0        0        0       79 2023-07-04 20:10:04.364946 rems-0.2.0/rems/_static_version.py
--rw-rw-rw-   0        0        0     6047 2023-07-03 02:24:52.000000 rems-0.2.0/rems/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.323945 rems-0.2.0/rems/device/
--rw-rw-rw-   0        0        0      595 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/BasicDeviceBase.py
--rw-rw-rw-   0        0        0     1056 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/DeviceBase.py
--rw-rw-rw-   0        0        0      585 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/DriveBase.py
--rw-rw-rw-   0        0        0      292 2023-07-03 02:24:52.000000 rems-0.2.0/rems/device/ObserveStateBase.py
--rw-rw-rw-   0        0        0      601 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/SenseBase.py
--rw-rw-rw-   0        0        0      302 2023-07-03 22:34:09.000000 rems-0.2.0/rems/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.324945 rems-0.2.0/rems/device/imu/
--rw-rw-rw-   0        0        0     1159 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/imu/ImuDevice.py
--rw-rw-rw-   0        0        0     4812 2023-07-03 02:24:52.000000 rems-0.2.0/rems/device/imu/Imu_interface.py
--rw-rw-rw-   0        0        0       59 2023-07-03 02:24:52.000000 rems-0.2.0/rems/device/imu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.326945 rems-0.2.0/rems/device/webots/
--rw-rw-rw-   0        0        0     4116 2023-07-04 19:15:41.000000 rems-0.2.0/rems/device/webots/WebotsBinder.py
--rw-rw-rw-   0        0        0     1477 2023-07-04 19:15:41.000000 rems-0.2.0/rems/device/webots/WebotsDrive.py
--rw-rw-rw-   0        0        0     2299 2023-07-04 19:15:40.000000 rems-0.2.0/rems/device/webots/WebotsSense.py
--rw-rw-rw-   0        0        0      116 2023-07-03 02:24:52.000000 rems-0.2.0/rems/device/webots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.330946 rems-0.2.0/rems/inputs/
--rw-rw-rw-   0        0        0      376 2023-07-03 02:24:52.000000 rems-0.2.0/rems/inputs/FileCsvInput.py
--rw-rw-rw-   0        0        0     3159 2023-07-04 19:15:41.000000 rems-0.2.0/rems/inputs/FileInput.py
--rw-rw-rw-   0        0        0      634 2023-07-04 19:15:41.000000 rems-0.2.0/rems/inputs/HockInput.py
--rw-rw-rw-   0        0        0     1403 2023-07-04 19:15:40.000000 rems-0.2.0/rems/inputs/InputBase.py
--rw-rw-rw-   0        0        0     2237 2023-07-04 19:15:40.000000 rems-0.2.0/rems/inputs/JoyManipulator.py
--rw-rw-rw-   0        0        0     3594 2023-07-04 19:15:41.000000 rems-0.2.0/rems/inputs/JoystickInput.py
--rw-rw-rw-   0        0        0     2442 2023-07-04 19:15:40.000000 rems-0.2.0/rems/inputs/KeyboardInput.py
--rw-rw-rw-   0        0        0      270 2023-07-03 02:24:52.000000 rems-0.2.0/rems/inputs/__init__.py
--rw-rw-rw-   0        0        0       43 2023-07-03 02:24:52.000000 rems-0.2.0/rems/inputs/estop_callback.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.332945 rems-0.2.0/rems/inputs/map/
--rw-rw-rw-   0        0        0     2386 2023-07-03 02:24:52.000000 rems-0.2.0/rems/inputs/map/JOYSTICK_KEYMAP.py
--rw-rw-rw-   0        0        0      209 2023-07-04 19:15:41.000000 rems-0.2.0/rems/inputs/map/KEYBOARD_KEYMAP.py
--rw-rw-rw-   0        0        0       65 2023-07-03 02:24:52.000000 rems-0.2.0/rems/inputs/map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.335945 rems-0.2.0/rems/outputs/
--rw-rw-rw-   0        0        0     7515 2023-07-03 02:24:52.000000 rems-0.2.0/rems/outputs/AnimationOutput.py
--rw-rw-rw-   0        0        0     1693 2023-07-04 19:15:40.000000 rems-0.2.0/rems/outputs/FileCsvOutput.py
--rw-rw-rw-   0        0        0     1623 2023-07-03 02:24:52.000000 rems-0.2.0/rems/outputs/FileOutput.py
--rw-rw-rw-   0        0        0      491 2023-07-04 19:15:41.000000 rems-0.2.0/rems/outputs/GraphOutput.py
--rw-rw-rw-   0        0        0     2011 2023-07-04 19:15:40.000000 rems-0.2.0/rems/outputs/OutputBase.py
--rw-rw-rw-   0        0        0     4491 2023-07-03 02:24:52.000000 rems-0.2.0/rems/outputs/PlotlyHelper.py
--rw-rw-rw-   0        0        0     3652 2023-07-03 02:24:52.000000 rems-0.2.0/rems/outputs/RealTimeFigOutputBase.py
--rw-rw-rw-   0        0        0      200 2023-07-03 02:24:52.000000 rems-0.2.0/rems/outputs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.336945 rems-0.2.0/rems/process/
--rw-rw-rw-   0        0        0      916 2023-07-03 02:24:52.000000 rems-0.2.0/rems/process/ProcessSystem.py
--rw-rw-rw-   0        0        0      961 2023-07-03 02:24:52.000000 rems-0.2.0/rems/process/TestProcess.py
--rw-rw-rw-   0        0        0       80 2023-07-03 02:24:52.000000 rems-0.2.0/rems/process/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.338945 rems-0.2.0/rems/robot_def/
--rw-rw-rw-   0        0        0     3712 2023-07-04 19:15:41.000000 rems-0.2.0/rems/robot_def/Manipulator5DoF.py
--rw-rw-rw-   0        0        0     3733 2023-07-04 19:15:41.000000 rems-0.2.0/rems/robot_def/MecanumDriveType.py
--rw-rw-rw-   0        0        0     2203 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robot_def/WoodbotDef.py
--rw-rw-rw-   0        0        0      129 2023-07-03 02:24:52.000000 rems-0.2.0/rems/robot_def/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.340946 rems-0.2.0/rems/robot_def/webots/
--rw-rw-rw-   0        0        0     2372 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robot_def/webots/YoubotArmDef.py
--rw-rw-rw-   0        0        0     1820 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robot_def/webots/YoubotBaseDef.py
--rw-rw-rw-   0        0        0      670 2023-07-04 19:15:41.000000 rems-0.2.0/rems/robot_def/webots/YoubotDef.py
--rw-rw-rw-   0        0        0      116 2023-07-03 22:34:08.000000 rems-0.2.0/rems/robot_def/webots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.344945 rems-0.2.0/rems/robots/
--rw-rw-rw-   0        0        0      630 2023-07-03 22:34:08.000000 rems-0.2.0/rems/robots/JacobianModel.py
--rw-rw-rw-   0        0        0      398 2023-07-03 02:24:52.000000 rems-0.2.0/rems/robots/NopRobot.py
--rw-rw-rw-   0        0        0     4645 2023-07-04 19:15:41.000000 rems-0.2.0/rems/robots/RobotBase.py
--rw-rw-rw-   0        0        0     4178 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robots/RobotBaseAsync.py
--rw-rw-rw-   0        0        0     2515 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robots/RobotDefBase.py
--rw-rw-rw-   0        0        0     3788 2023-07-03 02:24:52.000000 rems-0.2.0/rems/robots/RobotThread.py
--rw-rw-rw-   0        0        0      271 2023-07-03 02:24:52.000000 rems-0.2.0/rems/robots/RunConfig.py
--rw-rw-rw-   0        0        0      300 2023-07-03 22:58:13.000000 rems-0.2.0/rems/robots/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-07-04 19:15:40.000000 rems-0.2.0/rems/robots/bind_robot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.345945 rems-0.2.0/rems/sim_handler/
--rw-rw-rw-   0        0        0      107 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/SystemDefault.py
--rw-rw-rw-   0        0        0       51 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.348945 rems-0.2.0/rems/sim_handler/job_background/
--rw-rw-rw-   0        0        0      917 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/JobHandler.py
--rw-rw-rw-   0        0        0      380 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/JobHandlerBase.py
--rw-rw-rw-   0        0        0      839 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/JobHandlerMP.py
--rw-rw-rw-   0        0        0      731 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/RayJobHandler.py
--rw-rw-rw-   0        0        0      271 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/__init__.py
--rw-rw-rw-   0        0        0      133 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/job_return_type.py
--rw-rw-rw-   0        0        0      111 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/job_background/job_type.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.352946 rems-0.2.0/rems/sim_handler/ray/
--rw-rw-rw-   0        0        0      567 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/ActorWrapper.py
--rw-rw-rw-   0        0        0      725 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/ProcessActor.py
--rw-rw-rw-   0        0        0      459 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/RayWrapTest.py
--rw-rw-rw-   0        0        0     4206 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/RayWrapper.py
--rw-rw-rw-   0        0        0     5569 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/RobotRayWrapper.py
--rw-rw-rw-   0        0        0     2746 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/SimActor.py
--rw-rw-rw-   0        0        0      231 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/__init__.py
--rw-rw-rw-   0        0        0     1040 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/autocounter.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.353946 rems-0.2.0/rems/sim_handler/ray/examples/
--rw-rw-rw-   0        0        0     7756 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/examples/cluster.yml
--rw-rw-rw-   0        0        0     1852 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/ray/examples/ray_host.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.355945 rems-0.2.0/rems/sim_handler/thread/
--rw-rw-rw-   0        0        0     4960 2023-07-04 19:15:40.000000 rems-0.2.0/rems/sim_handler/thread/DeviceExecutor.py
--rw-rw-rw-   0        0        0     1813 2023-07-04 19:15:40.000000 rems-0.2.0/rems/sim_handler/thread/ProcessExecutor.py
--rw-rw-rw-   0        0        0       76 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/thread/TheadFunction.py
--rw-rw-rw-   0        0        0       90 2023-07-03 02:24:52.000000 rems-0.2.0/rems/sim_handler/thread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.360945 rems-0.2.0/rems/utils/
--rw-rw-rw-   0        0        0      239 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/AutoUpdatePip.py
--rw-rw-rw-   0        0        0      203 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/Rotations.py
--rw-rw-rw-   0        0        0      127 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/__init__.py
--rw-rw-rw-   0        0        0     1675 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/autotune_plots.py
--rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/calibration.yml
--rw-rw-rw-   0        0        0    11488 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/interpolate_limb_trajectory.py
--rw-rw-rw-   0        0        0     5954 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/neural_network.py
--rw-rw-rw-   0        0        0      306 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/tictoc.py
--rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/timestamp.py
--rw-rw-rw-   0        0        0      605 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/urdf_relative_path.py
--rw-rw-rw-   0        0        0   524288 2023-07-03 02:24:52.000000 rems-0.2.0/rems/utils/video.avi
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.321945 rems-0.2.0/rems.egg-info/
--rw-rw-rw-   0        0        0      498 2023-07-04 20:10:04.000000 rems-0.2.0/rems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3269 2023-07-04 20:10:04.000000 rems-0.2.0/rems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 20:10:04.000000 rems-0.2.0/rems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-07-04 20:10:04.000000 rems-0.2.0/rems.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-04 20:10:04.000000 rems-0.2.0/rems.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      176 2023-07-04 19:15:41.000000 rems-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 20:10:04.364946 rems-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1782 2023-07-04 20:09:42.000000 rems-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.362945 rems-0.2.0/trajectory/
-drwxrwxrwx   0        0        0        0 2023-07-04 20:10:04.363946 rems-0.2.0/trajectory/r2k/
--rw-rw-rw-   0        0        0   299700 2023-07-03 02:24:52.000000 rems-0.2.0/trajectory/r2k/target_robot_video.csv
--rw-rw-rw-   0        0        0   161657 2023-07-03 02:24:52.000000 rems-0.2.0/trajectory/target_robot_circle.csv
--rw-rw-rw-   0        0        0   196194 2023-07-03 02:24:52.000000 rems-0.2.0/trajectory/target_robot_circle_line.csv
--rw-rw-rw-   0        0        0    34694 2023-07-03 02:24:52.000000 rems-0.2.0/trajectory/target_robot_line.csv
--rw-rw-rw-   0        0        0     7297 2023-07-03 02:24:52.000000 rems-0.2.0/trajectory/trajectory_Generator.py
--rw-rw-rw-   0        0        0     4572 2023-07-04 18:48:25.000000 rems-0.2.0/webots_example_run.py
--rw-rw-rw-   0        0        0     1497 2023-07-03 02:24:52.000000 rems-0.2.0/woodbot_run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.790231 rems-0.2.1/
+-rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 rems-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2023-07-12 19:54:27.790231 rems-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4874 2023-07-04 19:17:53.000000 rems-0.2.1/ReadMe.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.790231 rems-0.2.1/rems/
+-rw-rw-rw-   0        0        0      462 2023-07-03 02:24:52.000000 rems-0.2.1/rems/Config.py
+-rw-rw-rw-   0        0        0     8193 2023-07-04 19:15:40.000000 rems-0.2.1/rems/Operator.py
+-rw-rw-rw-   0        0        0      511 2023-07-05 02:28:02.000000 rems-0.2.1/rems/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-07-12 19:54:27.790231 rems-0.2.1/rems/_static_version.py
+-rw-rw-rw-   0        0        0     6047 2023-07-03 02:24:52.000000 rems-0.2.1/rems/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.749232 rems-0.2.1/rems/device/
+-rw-rw-rw-   0        0        0      595 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/BasicDeviceBase.py
+-rw-rw-rw-   0        0        0     1056 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/DeviceBase.py
+-rw-rw-rw-   0        0        0      585 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/DriveBase.py
+-rw-rw-rw-   0        0        0      292 2023-07-03 02:24:52.000000 rems-0.2.1/rems/device/ObserveStateBase.py
+-rw-rw-rw-   0        0        0      601 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/SenseBase.py
+-rw-rw-rw-   0        0        0      152 2023-07-05 02:34:50.000000 rems-0.2.1/rems/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.750232 rems-0.2.1/rems/device/imu/
+-rw-rw-rw-   0        0        0     1159 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/imu/ImuDevice.py
+-rw-rw-rw-   0        0        0     4812 2023-07-03 02:24:52.000000 rems-0.2.1/rems/device/imu/Imu_interface.py
+-rw-rw-rw-   0        0        0       59 2023-07-03 02:24:52.000000 rems-0.2.1/rems/device/imu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.752232 rems-0.2.1/rems/device/webots/
+-rw-rw-rw-   0        0        0     4116 2023-07-04 19:15:41.000000 rems-0.2.1/rems/device/webots/WebotsBinder.py
+-rw-rw-rw-   0        0        0     1477 2023-07-04 19:15:41.000000 rems-0.2.1/rems/device/webots/WebotsDrive.py
+-rw-rw-rw-   0        0        0     2299 2023-07-04 19:15:40.000000 rems-0.2.1/rems/device/webots/WebotsSense.py
+-rw-rw-rw-   0        0        0      116 2023-07-03 02:24:52.000000 rems-0.2.1/rems/device/webots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.756230 rems-0.2.1/rems/inputs/
+-rw-rw-rw-   0        0        0      376 2023-07-03 02:24:52.000000 rems-0.2.1/rems/inputs/FileCsvInput.py
+-rw-rw-rw-   0        0        0     3159 2023-07-04 19:15:41.000000 rems-0.2.1/rems/inputs/FileInput.py
+-rw-rw-rw-   0        0        0      634 2023-07-04 19:15:41.000000 rems-0.2.1/rems/inputs/HockInput.py
+-rw-rw-rw-   0        0        0     1403 2023-07-04 19:15:40.000000 rems-0.2.1/rems/inputs/InputBase.py
+-rw-rw-rw-   0        0        0     2237 2023-07-04 19:15:40.000000 rems-0.2.1/rems/inputs/JoyManipulator.py
+-rw-rw-rw-   0        0        0     3594 2023-07-04 19:15:41.000000 rems-0.2.1/rems/inputs/JoystickInput.py
+-rw-rw-rw-   0        0        0     2442 2023-07-04 19:15:40.000000 rems-0.2.1/rems/inputs/KeyboardInput.py
+-rw-rw-rw-   0        0        0      270 2023-07-03 02:24:52.000000 rems-0.2.1/rems/inputs/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-07-03 02:24:52.000000 rems-0.2.1/rems/inputs/estop_callback.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.758228 rems-0.2.1/rems/inputs/map/
+-rw-rw-rw-   0        0        0     2386 2023-07-03 02:24:52.000000 rems-0.2.1/rems/inputs/map/JOYSTICK_KEYMAP.py
+-rw-rw-rw-   0        0        0      209 2023-07-04 19:15:41.000000 rems-0.2.1/rems/inputs/map/KEYBOARD_KEYMAP.py
+-rw-rw-rw-   0        0        0       65 2023-07-03 02:24:52.000000 rems-0.2.1/rems/inputs/map/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.761228 rems-0.2.1/rems/outputs/
+-rw-rw-rw-   0        0        0     7814 2023-07-12 01:59:37.000000 rems-0.2.1/rems/outputs/AnimationOutput.py
+-rw-rw-rw-   0        0        0     1693 2023-07-04 19:15:40.000000 rems-0.2.1/rems/outputs/FileCsvOutput.py
+-rw-rw-rw-   0        0        0     1623 2023-07-03 02:24:52.000000 rems-0.2.1/rems/outputs/FileOutput.py
+-rw-rw-rw-   0        0        0      491 2023-07-04 19:15:41.000000 rems-0.2.1/rems/outputs/GraphOutput.py
+-rw-rw-rw-   0        0        0     2011 2023-07-04 19:15:40.000000 rems-0.2.1/rems/outputs/OutputBase.py
+-rw-rw-rw-   0        0        0     4670 2023-07-12 01:56:10.000000 rems-0.2.1/rems/outputs/PlotlyHelper.py
+-rw-rw-rw-   0        0        0     3652 2023-07-03 02:24:52.000000 rems-0.2.1/rems/outputs/RealTimeFigOutputBase.py
+-rw-rw-rw-   0        0        0      200 2023-07-03 02:24:52.000000 rems-0.2.1/rems/outputs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.762228 rems-0.2.1/rems/process/
+-rw-rw-rw-   0        0        0      916 2023-07-03 02:24:52.000000 rems-0.2.1/rems/process/ProcessSystem.py
+-rw-rw-rw-   0        0        0      961 2023-07-03 02:24:52.000000 rems-0.2.1/rems/process/TestProcess.py
+-rw-rw-rw-   0        0        0       80 2023-07-03 02:24:52.000000 rems-0.2.1/rems/process/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.764229 rems-0.2.1/rems/robot_def/
+-rw-rw-rw-   0        0        0     3712 2023-07-04 19:15:41.000000 rems-0.2.1/rems/robot_def/Manipulator5DoF.py
+-rw-rw-rw-   0        0        0     3733 2023-07-04 19:15:41.000000 rems-0.2.1/rems/robot_def/MecanumDriveType.py
+-rw-rw-rw-   0        0        0     2203 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robot_def/WoodbotDef.py
+-rw-rw-rw-   0        0        0      129 2023-07-03 02:24:52.000000 rems-0.2.1/rems/robot_def/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.766229 rems-0.2.1/rems/robot_def/webots/
+-rw-rw-rw-   0        0        0     2372 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robot_def/webots/YoubotArmDef.py
+-rw-rw-rw-   0        0        0     1820 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robot_def/webots/YoubotBaseDef.py
+-rw-rw-rw-   0        0        0      670 2023-07-04 19:15:41.000000 rems-0.2.1/rems/robot_def/webots/YoubotDef.py
+-rw-rw-rw-   0        0        0      116 2023-07-03 22:34:08.000000 rems-0.2.1/rems/robot_def/webots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.770228 rems-0.2.1/rems/robots/
+-rw-rw-rw-   0        0        0      630 2023-07-03 22:34:08.000000 rems-0.2.1/rems/robots/JacobianModel.py
+-rw-rw-rw-   0        0        0      398 2023-07-03 02:24:52.000000 rems-0.2.1/rems/robots/NopRobot.py
+-rw-rw-rw-   0        0        0     4645 2023-07-04 19:15:41.000000 rems-0.2.1/rems/robots/RobotBase.py
+-rw-rw-rw-   0        0        0     4178 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robots/RobotBaseAsync.py
+-rw-rw-rw-   0        0        0     2515 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robots/RobotDefBase.py
+-rw-rw-rw-   0        0        0     3788 2023-07-03 02:24:52.000000 rems-0.2.1/rems/robots/RobotThread.py
+-rw-rw-rw-   0        0        0      271 2023-07-03 02:24:52.000000 rems-0.2.1/rems/robots/RunConfig.py
+-rw-rw-rw-   0        0        0      300 2023-07-03 22:58:13.000000 rems-0.2.1/rems/robots/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-07-04 19:15:40.000000 rems-0.2.1/rems/robots/bind_robot.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.771228 rems-0.2.1/rems/sim_handler/
+-rw-rw-rw-   0        0        0      107 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/SystemDefault.py
+-rw-rw-rw-   0        0        0       51 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.774228 rems-0.2.1/rems/sim_handler/job_background/
+-rw-rw-rw-   0        0        0      917 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/JobHandler.py
+-rw-rw-rw-   0        0        0      380 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/JobHandlerBase.py
+-rw-rw-rw-   0        0        0      839 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/JobHandlerMP.py
+-rw-rw-rw-   0        0        0      731 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/RayJobHandler.py
+-rw-rw-rw-   0        0        0      271 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/job_return_type.py
+-rw-rw-rw-   0        0        0      111 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/job_background/job_type.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.778228 rems-0.2.1/rems/sim_handler/ray/
+-rw-rw-rw-   0        0        0      567 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/ActorWrapper.py
+-rw-rw-rw-   0        0        0      725 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/ProcessActor.py
+-rw-rw-rw-   0        0        0      459 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/RayWrapTest.py
+-rw-rw-rw-   0        0        0     4206 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/RayWrapper.py
+-rw-rw-rw-   0        0        0     5569 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/RobotRayWrapper.py
+-rw-rw-rw-   0        0        0     2746 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/SimActor.py
+-rw-rw-rw-   0        0        0      231 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/__init__.py
+-rw-rw-rw-   0        0        0     1040 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/autocounter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.779228 rems-0.2.1/rems/sim_handler/ray/examples/
+-rw-rw-rw-   0        0        0     7756 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/examples/cluster.yml
+-rw-rw-rw-   0        0        0     1852 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/ray/examples/ray_host.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.781228 rems-0.2.1/rems/sim_handler/thread/
+-rw-rw-rw-   0        0        0     4960 2023-07-04 19:15:40.000000 rems-0.2.1/rems/sim_handler/thread/DeviceExecutor.py
+-rw-rw-rw-   0        0        0     1813 2023-07-04 19:15:40.000000 rems-0.2.1/rems/sim_handler/thread/ProcessExecutor.py
+-rw-rw-rw-   0        0        0       76 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/thread/TheadFunction.py
+-rw-rw-rw-   0        0        0       90 2023-07-03 02:24:52.000000 rems-0.2.1/rems/sim_handler/thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.786231 rems-0.2.1/rems/utils/
+-rw-rw-rw-   0        0        0      239 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/AutoUpdatePip.py
+-rw-rw-rw-   0        0        0      203 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/Rotations.py
+-rw-rw-rw-   0        0        0      127 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/__init__.py
+-rw-rw-rw-   0        0        0     1675 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/autotune_plots.py
+-rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/calibration.yml
+-rw-rw-rw-   0        0        0    11488 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/interpolate_limb_trajectory.py
+-rw-rw-rw-   0        0        0     5956 2023-07-05 01:54:20.000000 rems-0.2.1/rems/utils/neural_network.py
+-rw-rw-rw-   0        0        0      306 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/tictoc.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/timestamp.py
+-rw-rw-rw-   0        0        0      605 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/urdf_relative_path.py
+-rw-rw-rw-   0        0        0   524288 2023-07-03 02:24:52.000000 rems-0.2.1/rems/utils/video.avi
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.746229 rems-0.2.1/rems.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-07-12 19:54:27.000000 rems-0.2.1/rems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3281 2023-07-12 19:54:27.000000 rems-0.2.1/rems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:54:27.000000 rems-0.2.1/rems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-07-12 19:54:27.000000 rems-0.2.1/rems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 19:54:27.000000 rems-0.2.1/rems.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      193 2023-07-05 03:09:31.000000 rems-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:54:27.790231 rems-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1848 2023-07-12 19:53:49.000000 rems-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.788231 rems-0.2.1/trajectory/
+drwxrwxrwx   0        0        0        0 2023-07-12 19:54:27.789231 rems-0.2.1/trajectory/r2k/
+-rw-rw-rw-   0        0        0   299700 2023-07-03 02:24:52.000000 rems-0.2.1/trajectory/r2k/target_robot_video.csv
+-rw-rw-rw-   0        0        0   161657 2023-07-03 02:24:52.000000 rems-0.2.1/trajectory/target_robot_circle.csv
+-rw-rw-rw-   0        0        0   196194 2023-07-03 02:24:52.000000 rems-0.2.1/trajectory/target_robot_circle_line.csv
+-rw-rw-rw-   0        0        0    34694 2023-07-03 02:24:52.000000 rems-0.2.1/trajectory/target_robot_line.csv
+-rw-rw-rw-   0        0        0     7297 2023-07-03 02:24:52.000000 rems-0.2.1/trajectory/trajectory_Generator.py
+-rw-rw-rw-   0        0        0     4572 2023-07-04 18:48:25.000000 rems-0.2.1/webots_example_run.py
+-rw-rw-rw-   0        0        0     1497 2023-07-03 02:24:52.000000 rems-0.2.1/woodbot_run.py
```

### Comparing `rems-0.2.0/ReadMe.md` & `rems-0.2.1/ReadMe.md`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/Operator.py` & `rems-0.2.1/rems/Operator.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/_version.py` & `rems-0.2.1/rems/_version.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/BasicDeviceBase.py` & `rems-0.2.1/rems/device/BasicDeviceBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/DeviceBase.py` & `rems-0.2.1/rems/device/DeviceBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/DriveBase.py` & `rems-0.2.1/rems/device/DriveBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/SenseBase.py` & `rems-0.2.1/rems/device/SenseBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/imu/ImuDevice.py` & `rems-0.2.1/rems/device/imu/ImuDevice.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/imu/Imu_interface.py` & `rems-0.2.1/rems/device/imu/Imu_interface.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/webots/WebotsBinder.py` & `rems-0.2.1/rems/device/webots/WebotsBinder.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/webots/WebotsDrive.py` & `rems-0.2.1/rems/device/webots/WebotsDrive.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/device/webots/WebotsSense.py` & `rems-0.2.1/rems/device/webots/WebotsSense.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/FileInput.py` & `rems-0.2.1/rems/inputs/FileInput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/HockInput.py` & `rems-0.2.1/rems/inputs/HockInput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/InputBase.py` & `rems-0.2.1/rems/inputs/InputBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/JoyManipulator.py` & `rems-0.2.1/rems/inputs/JoyManipulator.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/JoystickInput.py` & `rems-0.2.1/rems/inputs/JoystickInput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/KeyboardInput.py` & `rems-0.2.1/rems/inputs/KeyboardInput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/inputs/map/JOYSTICK_KEYMAP.py` & `rems-0.2.1/rems/inputs/map/JOYSTICK_KEYMAP.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/outputs/AnimationOutput.py` & `rems-0.2.1/rems/outputs/AnimationOutput.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 FORMAT_XY = dict(x=float, y=float)
 FORMAT_XYTh = dict(x=float, y=float, th_z=float)
 DEFAULT_AXIS_SIZE = 0.1
 SCALE = 0.04
 MARGIN = 0.1
 
 class AnimationOutput(OutputBase):
-    def __init__(self, filepath, tail_length=float('inf'), fps_limit=15):
+    def __init__(self, filepath, tail_length=float('inf'), fps_limit=15, save_html_path=None):
         super().__init__()
         self.filepath = filepath
+        self.save_html_path = save_html_path
         self.tail_length = tail_length
         self.fps_limit = fps_limit
         self.last_update = 0.0
         self.use_cache = False
         self.fig = None
 
     def process(self, state, inpt, outpt, timestamp, info):
@@ -34,32 +35,35 @@
             last_state = round(self._states[-1], 2)
             self._update_canvas(plot_data, f"state: {last_state.__str__()}")
 
     def make_output(self):
         """make proper output from the data"""
         if len(self._timestamps) <= 2:
             return
-        p = PlotlyHelper()
+        p = PlotlyHelper(save_html_path=self.save_html_path)
         p.anim_path_dot(*self.get_plot_list(self._states, FORMAT_XYTh), fps=self.calc_fps())
         self.generate_video()
 
     def _under_fps_limit(self, timestamp):
         return bool((1/(timestamp - self.last_update)) <= self.fps_limit)
 
     def _create_canvas(self):
         #marker = (3, 0, i * 90), markersize = 20, linestyle = 'None')
         self.fig, self.ax = plt.subplots()
         self.line, = self.ax.plot([], lw=3)
         self.ann = self.ax.annotate('', xy=(0, 0),
                                     arrowprops=dict(arrowstyle="<-", color='red', lw=3))
         self.text = self.ax.text(0.0, 0.0, "")
+        self.ax.set_xlabel(f'x, [m]')
+        self.ax.set_ylabel(f'y, [m]')
         self.fig.canvas.draw()
         self.ax_cache = self.fig.canvas.copy_from_bbox(self.ax.bbox)
         plt.autoscale(True)
         plt.rcParams["keymap.quit"] = "esc"
+        plt.grid(True)
         plt.show(block=False)
 
     def _update_canvas(self, line=None, text=None):
         x_l, y_l = self.ax.get_xlim(), self.ax.get_ylim()
         x_l, y_l = (x_l[1]-x_l[0]), (y_l[1]-y_l[0])
         if line is not None:
             x,y,th = line
@@ -120,14 +124,16 @@
             ret_list.append([d[i] for d in list_data])
         return tuple(ret_list)
 
     def generate_video(self):
         # initializing a figure
         fig = plt.figure()
         axis = plt.axes()
+        axis.set_xlabel(f'x, [m]')
+        axis.set_ylabel(f'y, [m]')
         ann = axis.annotate('', xy=(0,0), arrowprops=dict(arrowstyle="<-",
                          color='red',
                          lw=3,
                          ls='--'))
         ann_list =[ann]
         # labeling the x-axis and y-axis
         #axis = plt.axes(xlim=(0, 1000), ylim=(0, 1000))
@@ -138,14 +144,15 @@
         states_x, states_y, state_th = self.get_plot_list(self._states, FORMAT_XYTh)
 
         axis.set_xlim([min(states_x), max(states_x)])
         axis.set_ylim([min(states_y), max(states_y)])
         x_l, y_l = self._get_axis_size(states_x, states_y)
         line, = axis.plot(0, 0)
         text = axis.text(0.0,0.0,'')
+        plt.grid(True)
 
         def animate(frame_number):
             x.append(states_x[frame_number])
             y.append(states_y[frame_number])
             th.append(state_th[frame_number])
             line.set_xdata(x)
             line.set_ydata(y)
```

### Comparing `rems-0.2.0/rems/outputs/FileCsvOutput.py` & `rems-0.2.1/rems/outputs/FileCsvOutput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/outputs/FileOutput.py` & `rems-0.2.1/rems/outputs/FileOutput.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/outputs/OutputBase.py` & `rems-0.2.1/rems/outputs/OutputBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/outputs/PlotlyHelper.py` & `rems-0.2.1/rems/outputs/PlotlyHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 
 DEFAULT_MARGIN = 0.1
 FPS_LIMIT = 10
 SCALE = 100
 
 class PlotlyHelper:
-    def __init__(self):
-        pass
+    def __init__(self, save_html_path=None):
+        self.save_html_path = save_html_path
 
     def anim_path_dot(self, x, y, th=None, fps=1, title="Animation"):
 
         if th is None:
             th = np.zeros(len(x))
 
         x_range, y_range = self.axis_limit(x, y, DEFAULT_MARGIN)
@@ -27,16 +27,16 @@
                              mode="lines",
                              line=dict(width=2, color="blue")),
                   go.Scatter(x=x, y=y,
                              mode="lines",
                              line=dict(width=2, color="blue"))
                   ],
             layout=go.Layout(
-                xaxis=dict(range=x_range, autorange=False, zeroline=False),
-                yaxis=dict(range=y_range, autorange=False, zeroline=False),
+                xaxis=dict(range=x_range, autorange=False, zeroline=False, title='x, [m]'),
+                yaxis=dict(range=y_range, autorange=False, zeroline=False, title='y, [m]'),
                 title_text=title, hovermode="closest",
                 updatemenus=[dict(type="buttons",
                                   buttons=[dict(label="Play", method="animate",
                                                 args=[None, {"frame": {"duration": duration, "redraw": False},
                                                              "mode": "immediate",
                                                              "fromcurrent": True, "transition": {"duration": duration,
                                                                                                  "easing": "quadratic-in-out"}}]),
@@ -74,14 +74,16 @@
                             startarrowsize=2,
                             startarrowhead=4,
 
 
                         )], )
             ) for k in N],)
         fig.update_yaxes(scaleanchor="x", scaleratio=1)
+        if self.save_html_path is not None:
+            fig.write_html(self.save_html_path)
         fig.show()
 
     def _get_axis_size(self, x, y):
         l = []
         for v in (x, y):
             l.append(max(v) - min(v))
         return tuple(l)
```

### Comparing `rems-0.2.0/rems/outputs/RealTimeFigOutputBase.py` & `rems-0.2.1/rems/outputs/RealTimeFigOutputBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/process/ProcessSystem.py` & `rems-0.2.1/rems/process/ProcessSystem.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/process/TestProcess.py` & `rems-0.2.1/rems/process/TestProcess.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/Manipulator5DoF.py` & `rems-0.2.1/rems/robot_def/Manipulator5DoF.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/MecanumDriveType.py` & `rems-0.2.1/rems/robot_def/MecanumDriveType.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/WoodbotDef.py` & `rems-0.2.1/rems/robot_def/WoodbotDef.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/webots/YoubotArmDef.py` & `rems-0.2.1/rems/robot_def/webots/YoubotArmDef.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/webots/YoubotBaseDef.py` & `rems-0.2.1/rems/robot_def/webots/YoubotBaseDef.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robot_def/webots/YoubotDef.py` & `rems-0.2.1/rems/robot_def/webots/YoubotDef.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/JacobianModel.py` & `rems-0.2.1/rems/robots/JacobianModel.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/RobotBase.py` & `rems-0.2.1/rems/robots/RobotBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/RobotBaseAsync.py` & `rems-0.2.1/rems/robots/RobotBaseAsync.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/RobotDefBase.py` & `rems-0.2.1/rems/robots/RobotDefBase.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/RobotThread.py` & `rems-0.2.1/rems/robots/RobotThread.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/robots/bind_robot.py` & `rems-0.2.1/rems/robots/bind_robot.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/job_background/JobHandler.py` & `rems-0.2.1/rems/sim_handler/job_background/JobHandler.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/job_background/JobHandlerMP.py` & `rems-0.2.1/rems/sim_handler/job_background/JobHandlerMP.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/job_background/RayJobHandler.py` & `rems-0.2.1/rems/sim_handler/job_background/RayJobHandler.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/ActorWrapper.py` & `rems-0.2.1/rems/sim_handler/ray/ActorWrapper.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/ProcessActor.py` & `rems-0.2.1/rems/sim_handler/ray/ProcessActor.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/RayWrapper.py` & `rems-0.2.1/rems/sim_handler/ray/RayWrapper.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/RobotRayWrapper.py` & `rems-0.2.1/rems/sim_handler/ray/RobotRayWrapper.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/SimActor.py` & `rems-0.2.1/rems/sim_handler/ray/SimActor.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/autocounter.py` & `rems-0.2.1/rems/sim_handler/ray/autocounter.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/examples/cluster.yml` & `rems-0.2.1/rems/sim_handler/ray/examples/cluster.yml`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/ray/examples/ray_host.py` & `rems-0.2.1/rems/sim_handler/ray/examples/ray_host.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/thread/DeviceExecutor.py` & `rems-0.2.1/rems/sim_handler/thread/DeviceExecutor.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/sim_handler/thread/ProcessExecutor.py` & `rems-0.2.1/rems/sim_handler/thread/ProcessExecutor.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/utils/autotune_plots.py` & `rems-0.2.1/rems/utils/autotune_plots.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/utils/interpolate_limb_trajectory.py` & `rems-0.2.1/rems/utils/interpolate_limb_trajectory.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/utils/neural_network.py` & `rems-0.2.1/rems/utils/neural_network.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -136,8 +136,8 @@
     TEST_SIZE = 0.1
     NN = NeuralNetwork(NN_ARCHITECTURE, [])
     X, y = make_moons(n_samples=N_SAMPLES, noise=0.2, random_state=100)
     #X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=TEST_SIZE, random_state=42)
     Y_hat, _ = NN.full_forward_propagation(np.transpose(X))
     print(Y_hat)
     param_auto_tune = NN.Neural_to_Auto_Format(NN.params_values)
-    params_value = NN.Auto_to_Neural_Format(param_auto_tune)
+    params_value = NN.Auto_to_Neural_Format(param_auto_tune)
```

### Comparing `rems-0.2.0/rems/utils/urdf_relative_path.py` & `rems-0.2.1/rems/utils/urdf_relative_path.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems/utils/video.avi` & `rems-0.2.1/rems/utils/video.avi`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/rems.egg-info/SOURCES.txt` & `rems-0.2.1/rems.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 ReadMe.md
 requirements.txt
 setup.py
 webots_example_run.py
 woodbot_run.py
 rems/Config.py
 rems/Operator.py
```

### Comparing `rems-0.2.0/setup.py` & `rems-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='rems',
-    version='0.2.0',
+    version='0.2.1',
     cmdclass=cmdclass,
     description=get_metadata('description'),
     author=get_metadata('author'),
+    project_urls={'GitHub': 'https://github.com/Suke0811/REMS'},
     license='LGPLv3',
     packages=find_packages(include=['rems', 'rems.*']),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Robot Framework',
         'Intended Audience :: Developers',
```

### Comparing `rems-0.2.0/trajectory/r2k/target_robot_video.csv` & `rems-0.2.1/trajectory/r2k/target_robot_video.csv`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/trajectory/target_robot_circle.csv` & `rems-0.2.1/trajectory/target_robot_circle.csv`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/trajectory/target_robot_circle_line.csv` & `rems-0.2.1/trajectory/target_robot_circle_line.csv`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/trajectory/target_robot_line.csv` & `rems-0.2.1/trajectory/target_robot_line.csv`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/trajectory/trajectory_Generator.py` & `rems-0.2.1/trajectory/trajectory_Generator.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/webots_example_run.py` & `rems-0.2.1/webots_example_run.py`

 * *Files identical despite different names*

### Comparing `rems-0.2.0/woodbot_run.py` & `rems-0.2.1/woodbot_run.py`

 * *Files identical despite different names*

