# Comparing `tmp/hello_robot_stretch_body-0.4.9.tar.gz` & `tmp/hello_robot_stretch_body-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body-0.4.9.tar", last modified: Fri Sep 23 17:39:06 2022, max compression
+gzip compressed data, was "hello_robot_stretch_body-0.5.0.dev0.tar", last modified: Tue Jul 11 23:50:57 2023, max compression
```

## Comparing `hello_robot_stretch_body-0.4.9.tar` & `hello_robot_stretch_body-0.5.0.dev0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      916 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2449 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1937 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.552698 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2449 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1637 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      553 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2035 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.556697 hello_robot_stretch_body-0.4.9/stretch_body/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      948 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    33711 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3996 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/cobbs_framing.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5518 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    36111 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    10775 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_X_chain.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    39292 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3528 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      571 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2929 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21149 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1000 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27808 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26762 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/prismatic_joint.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14301 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8433 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_collision.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6479 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_collision_models.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6869 2022-09-23 16:03:21.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_monitor.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6929 2022-09-23 17:19:29.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    25176 2022-09-23 17:09:48.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE1V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    18715 2022-09-23 17:06:19.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE2V0.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11660 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/scope.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    49692 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/stepper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3814 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    28383 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    13897 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/transport.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      213 2022-09-23 17:38:49.000000 hello_robot_stretch_body-0.4.9/stretch_body/version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12090 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/wacc.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1919 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/wrist_yaw.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9733 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/xbox_controller.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6818 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_collisions.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dxl_comms.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21963 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9004 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_steppers.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_sync.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_timing_stats.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_wrist_yaw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 23:50:57.234567 hello_robot_stretch_body-0.5.0.dev0/
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-11 23:50:57.234567 hello_robot_stretch_body-0.5.0.dev0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2262 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 23:50:57.226567 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-11 23:50:57.000000 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-11 23:50:57.000000 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 23:50:57.000000 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      578 2023-07-11 23:50:57.000000 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 23:50:57.000000 hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 23:50:57.234567 hello_robot_stretch_body-0.5.0.dev0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2084 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 23:50:57.230567 hello_robot_stretch_body-0.5.0.dev0/stretch_body/
+-rw-rw-r--   0 root         (0) root         (0)       34 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      970 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/arm.py
+-rw-rw-r--   0 root         (0) root         (0)    34473 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3304 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/cobbs_framing.py
+-rw-rw-r--   0 root         (0) root         (0)     6086 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/device.py
+-rw-rw-r--   0 root         (0) root         (0)    36111 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_XL430.py
+-rw-rw-r--   0 root         (0) root         (0)    11462 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_X_chain.py
+-rw-rw-r--   0 root         (0) root         (0)    42687 2023-06-29 23:55:29.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_hello_XL430.py
+-rw-rw-r--   0 root         (0) root         (0)     3659 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/end_of_arm.py
+-rw-rw-r--   0 root         (0) root         (0)      571 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/end_of_arm_tools.py
+-rw-rw-r--   0 root         (0) root         (0)     3055 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/head.py
+-rw-rw-r--   0 root         (0) root         (0)    21912 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/hello_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1022 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/lift.py
+-rw-rw-r--   0 root         (0) root         (0)    39704 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/pimu.py
+-rw-rw-r--   0 root         (0) root         (0)    27354 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/prismatic_joint.py
+-rw-rw-r--   0 root         (0) root         (0)    21754 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot.py
+-rw-rw-r--   0 root         (0) root         (0)     8415 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_collision.py
+-rw-rw-r--   0 root         (0) root         (0)     6479 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_collision_models.py
+-rw-rw-r--   0 root         (0) root         (0)     6859 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_monitor.py
+-rw-rw-r--   0 root         (0) root         (0)     6949 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params.py
+-rw-rw-r--   0 root         (0) root         (0)    26094 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params_RE1V0.py
+-rw-rw-r--   0 root         (0) root         (0)    19672 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params_RE2V0.py
+-rw-rw-r--   0 root         (0) root         (0)     4504 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_trace.py
+-rwxrwxr-x   0 root         (0) root         (0)    12072 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/scope.py
+-rw-rw-r--   0 root         (0) root         (0)    61278 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/stepper.py
+-rw-rw-r--   0 root         (0) root         (0)     3829 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/stretch_gripper.py
+-rw-rw-r--   0 root         (0) root         (0)    29097 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/trajectories.py
+-rw-rw-r--   0 root         (0) root         (0)    45367 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/transport.py
+-rw-rw-r--   0 root         (0) root         (0)      218 2023-07-11 23:46:12.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/version.py
+-rw-rw-r--   0 root         (0) root         (0)    20335 2023-07-11 23:38:34.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/wacc.py
+-rw-rw-r--   0 root         (0) root         (0)     1934 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/wrist_yaw.py
+-rwxrwxr-x   0 root         (0) root         (0)     9733 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/stretch_body/xbox_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 23:50:57.234567 hello_robot_stretch_body-0.5.0.dev0/test/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_arm.py
+-rw-rw-r--   0 root         (0) root         (0)     6818 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_base.py
+-rw-rw-r--   0 root         (0) root         (0)     9977 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_collisions.py
+-rw-rw-r--   0 root         (0) root         (0)     3198 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_device.py
+-rw-rw-r--   0 root         (0) root         (0)     1111 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_dxl_comms.py
+-rw-rw-r--   0 root         (0) root         (0)     7882 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_dynamixel_XL430.py
+-rw-rw-r--   0 root         (0) root         (0)    14520 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_dynamixel_hello_XL430.py
+-rw-rw-r--   0 root         (0) root         (0)     1435 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_end_of_arm.py
+-rw-rw-r--   0 root         (0) root         (0)     1914 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_end_of_arm_tools.py
+-rw-rw-r--   0 root         (0) root         (0)     3833 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_head.py
+-rw-rw-r--   0 root         (0) root         (0)    23286 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_hello_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4761 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_lift.py
+-rw-rw-r--   0 root         (0) root         (0)     2069 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_pimu.py
+-rw-rw-r--   0 root         (0) root         (0)     9004 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_robot.py
+-rw-rw-r--   0 root         (0) root         (0)     2391 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_robot_params.py
+-rw-rw-r--   0 root         (0) root         (0)    26117 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_steppers.py
+-rw-rw-r--   0 root         (0) root         (0)     1657 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_stretch_gripper.py
+-rw-rw-r--   0 root         (0) root         (0)     6263 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_sync.py
+-rw-rw-r--   0 root         (0) root         (0)     4381 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_timing_stats.py
+-rw-rw-r--   0 root         (0) root         (0)    29747 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_trajectories.py
+-rw-rw-r--   0 root         (0) root         (0)     3918 2023-05-22 20:49:30.000000 hello_robot_stretch_body-0.5.0.dev0/test/test_wrist_yaw.py
```

### Comparing `hello_robot_stretch_body-0.4.9/PKG-INFO` & `hello_robot_stretch_body-0.5.0.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,73 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_body
-Version: 0.4.9
+Version: 0.5.0.dev0
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
+Description: Stretch Body
+        ============
+        
+        The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
+        
+        Installing
+        ----------
+        
+        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade hello-robot-stretch-body
+        ```
+        
+        To install or upgrade to a pre-release of Stretch Body for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body
+        ```
+        
+        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+        
+        Running tests
+        -------------
+        
+        There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
+        
+        In Python3, run `python3 -m unittest test.test_<suite-name>`.
+        
+        For example, to run the `stretch_body.robot.Robot` functional tests, run:
+        
+        ```bash
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/body
+        $ python3 -m unittest test.test_robot
+        ```
+        
+        Developing
+        ----------
+        
+        The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
+        
+        In Python3, run `python3 -m pip install -e .`
+        
+        For example, to test changes to `stretch_body.robot.Robot`, run:
+        
+        ```bash
+        $ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/body
+        $ python3 -m pip install -e .
+        ```
+        
+        Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
+        
+        Deploying
+        ---------
+        
+        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-Stretch Body
-============
-
-The stretch_body package provides a low level Python API to the Hello Robot Stretch RE1 hardware.
-
-Installing
-----------
-
-To install stable Stretch Body for Python2, run:
-
-```bash
-$ python -m pip install --upgrade hello-robot-stretch-body
-```
-
-To install a pre-release of Stretch Body for Python2, run:
-
-```bash
-$ python -m pip install --upgrade --pre hello-robot-stretch-body
-```
-
-Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-
-For Python3, substitute `python` with `python3`.
-
-Running tests
--------------
-
-There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
-
-In Python2, run `python -m unittest test.test_<suite-name>`. For Python3, substitute `python` with `python3`.
-
-For example, to run the `stretch_body.robot.Robot` functional tests, run
-
-```bash
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/body
-$ python -m unittest test.test_robot
-```
-
-Developing
-----------
-
-The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
-
-In Python2, run `python -m pip install -e .` For Python3, substitute `python` with `python3`.
-
-For example, to test changes to `stretch_body.robot.Robot`, run
-
-```bash
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/body
-$ python -m pip install -e .
-```
-
-Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
-
-Deploying
----------
-
-Increment the version number and run the `deploy.sh` script.
-
-
```

### Comparing `hello_robot_stretch_body-0.4.9/README.md` & `hello_robot_stretch_body-0.5.0.dev0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 Stretch Body
 ============
 
-The stretch_body package provides a low level Python API to the Hello Robot Stretch RE1 hardware.
+The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
 
 Installing
 ----------
 
-To install stable Stretch Body for Python2, run:
+This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
 
 ```bash
-$ python -m pip install --upgrade hello-robot-stretch-body
+$ python3 -m pip install --upgrade hello-robot-stretch-body
 ```
 
-To install a pre-release of Stretch Body for Python2, run:
+To install or upgrade to a pre-release of Stretch Body for Python3, run:
 
 ```bash
-$ python -m pip install --upgrade --pre hello-robot-stretch-body
+$ python3 -m pip install --upgrade --pre hello-robot-stretch-body
 ```
 
 Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
 
-For Python3, substitute `python` with `python3`.
-
 Running tests
 -------------
 
 There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
 
-In Python2, run `python -m unittest test.test_<suite-name>`. For Python3, substitute `python` with `python3`.
+In Python3, run `python3 -m unittest test.test_<suite-name>`.
 
-For example, to run the `stretch_body.robot.Robot` functional tests, run
+For example, to run the `stretch_body.robot.Robot` functional tests, run:
 
 ```bash
 $ git clone https://github.com/hello-robot/stretch_body.git
 $ cd stretch_body/body
-$ python -m unittest test.test_robot
+$ python3 -m unittest test.test_robot
 ```
 
 Developing
 ----------
 
 The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
 
-In Python2, run `python -m pip install -e .` For Python3, substitute `python` with `python3`.
+In Python3, run `python3 -m pip install -e .`
 
-For example, to test changes to `stretch_body.robot.Robot`, run
+For example, to test changes to `stretch_body.robot.Robot`, run:
 
 ```bash
+$ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
 $ git clone https://github.com/hello-robot/stretch_body.git
 $ cd stretch_body/body
-$ python -m pip install -e .
+$ python3 -m pip install -e .
 ```
 
 Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
 
 Deploying
 ---------
 
-Increment the version number and run the `deploy.sh` script.
+Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
```

### Comparing `hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/PKG-INFO` & `hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,73 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-body
-Version: 0.4.9
+Version: 0.5.0.dev0
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
+Description: Stretch Body
+        ============
+        
+        The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
+        
+        Installing
+        ----------
+        
+        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade hello-robot-stretch-body
+        ```
+        
+        To install or upgrade to a pre-release of Stretch Body for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body
+        ```
+        
+        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+        
+        Running tests
+        -------------
+        
+        There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
+        
+        In Python3, run `python3 -m unittest test.test_<suite-name>`.
+        
+        For example, to run the `stretch_body.robot.Robot` functional tests, run:
+        
+        ```bash
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/body
+        $ python3 -m unittest test.test_robot
+        ```
+        
+        Developing
+        ----------
+        
+        The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
+        
+        In Python3, run `python3 -m pip install -e .`
+        
+        For example, to test changes to `stretch_body.robot.Robot`, run:
+        
+        ```bash
+        $ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/body
+        $ python3 -m pip install -e .
+        ```
+        
+        Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
+        
+        Deploying
+        ---------
+        
+        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-Stretch Body
-============
-
-The stretch_body package provides a low level Python API to the Hello Robot Stretch RE1 hardware.
-
-Installing
-----------
-
-To install stable Stretch Body for Python2, run:
-
-```bash
-$ python -m pip install --upgrade hello-robot-stretch-body
-```
-
-To install a pre-release of Stretch Body for Python2, run:
-
-```bash
-$ python -m pip install --upgrade --pre hello-robot-stretch-body
-```
-
-Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-
-For Python3, substitute `python` with `python3`.
-
-Running tests
--------------
-
-There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
-
-In Python2, run `python -m unittest test.test_<suite-name>`. For Python3, substitute `python` with `python3`.
-
-For example, to run the `stretch_body.robot.Robot` functional tests, run
-
-```bash
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/body
-$ python -m unittest test.test_robot
-```
-
-Developing
-----------
-
-The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
-
-In Python2, run `python -m pip install -e .` For Python3, substitute `python` with `python3`.
-
-For example, to test changes to `stretch_body.robot.Robot`, run
-
-```bash
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/body
-$ python -m pip install -e .
-```
-
-Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
-
-Deploying
----------
-
-Increment the version number and run the `deploy.sh` script.
-
-
```

### Comparing `hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/SOURCES.txt` & `hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 README.md
 setup.py
 hello_robot_stretch_body.egg-info/PKG-INFO
 hello_robot_stretch_body.egg-info/SOURCES.txt
 hello_robot_stretch_body.egg-info/dependency_links.txt
 hello_robot_stretch_body.egg-info/requires.txt
 hello_robot_stretch_body.egg-info/top_level.txt
@@ -24,14 +23,15 @@
 stretch_body/robot.py
 stretch_body/robot_collision.py
 stretch_body/robot_collision_models.py
 stretch_body/robot_monitor.py
 stretch_body/robot_params.py
 stretch_body/robot_params_RE1V0.py
 stretch_body/robot_params_RE2V0.py
+stretch_body/robot_trace.py
 stretch_body/scope.py
 stretch_body/stepper.py
 stretch_body/stretch_gripper.py
 stretch_body/trajectories.py
 stretch_body/transport.py
 stretch_body/version.py
 stretch_body/wacc.py
```

### Comparing `hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/requires.txt` & `hello_robot_stretch_body-0.5.0.dev0/hello_robot_stretch_body.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-numpy
-scipy
-matplotlib
-ipython
-pandas
-sympy
-nose
-inputs
-drawnow
-rplidar-roboticia
-snakeviz
-pyusb
 SpeechRecognition
-pixel-ring
+aioserial
 click
 cma
 colorama
-scikit-image
-open3d
-pyrealsense2
-pathlib
-psutil
+drawnow
 gitpython
-urdfpy
-opencv-contrib-python
+hello-robot-stretch-body-tools>=0.4.2
+hello-robot-stretch-factory>=0.3.5
+hello-robot-stretch-tool-share>=0.2.6
+inputs
+ipython
 jupyter
+matplotlib==3.5.0
+nose
 numba
+numpy==1.23.2
+open3d
+opencv-contrib-python
+pandas
+pathlib
+pixel-ring
+psutil
+pyrealsense2
+pyusb
 pyyaml>=5.1
-hello-robot-stretch-tool-share>=0.2.5
-hello-robot-stretch-factory>=0.3.5
-hello-robot-stretch-body-tools>=0.4.2
+rplidar-roboticia
+scikit-image
+scipy
+snakeviz
+sympy
+urdfpy
 
 [:python_version < "3.0"]
 jsonschema==2.6.0
-qtconsole==4.7.7
 llvmlite==0.31.0
+qtconsole==4.7.7
 terminado==0.8.3
 
 [:python_version >= "3.0.0"]
-renamed-opencv-python-inference-engine
 dynamixel-sdk>=3.1
+renamed-opencv-python-inference-engine
```

### Comparing `hello_robot_stretch_body-0.4.9/setup.py` & `hello_robot_stretch_body-0.5.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     url="https://github.com/hello-robot/stretch_body",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 2",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
     ],
-    install_requires=['numpy', 'scipy', 'matplotlib', 'ipython', 'pandas', 'sympy', 'nose',
+    install_requires=['numpy==1.23.2', 'scipy', 'matplotlib==3.5.0', 'ipython', 'pandas', 'sympy', 'nose',
                       'inputs', 'drawnow', 'rplidar-roboticia', 'snakeviz', 'pyusb', 'SpeechRecognition', 'pixel-ring',
                       'click', 'cma', 'colorama',
                       'scikit-image', 'open3d', 'pyrealsense2', 'pathlib', 'psutil', 'gitpython', 'urdfpy',
                       'opencv-contrib-python', 'renamed-opencv-python-inference-engine; python_version >= "3.0.0"', # resolve cv2 conflict for py3
                       'jsonschema==2.6.0; python_version < "3.0"', 'qtconsole==4.7.7; python_version < "3.0"', 'jupyter', # required by juypter
                       'llvmlite==0.31.0; python_version < "3.0"', 'numba', # numba required by stretch_funmap, depends on old llvmlite for py2
                       'terminado==0.8.3; python_version < "3.0"', # depend on old terminado for py2
                       'dynamixel-sdk>=3.1; python_version >= "3.0.0"', # py2 gets dynamixel-sdk through ROS
                       'pyyaml>=5.1', # required for yaml.FullLoader
-                      'hello-robot-stretch-tool-share>=0.2.5', # defines other Stretch end effectors
-                      'hello-robot-stretch-factory>=0.3.5','hello-robot-stretch-body-tools>=0.4.2'
-
+                      'hello-robot-stretch-tool-share>=0.2.6', # defines other Stretch end effectors
+                      'hello-robot-stretch-factory>=0.3.5','hello-robot-stretch-body-tools>=0.4.2',
+                      'aioserial'
                       ]
 )
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/arm.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/arm.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import math
 
 
 class Arm(PrismaticJoint):
     """
     API to the Stretch Arm
     """
-    def __init__(self):
-        PrismaticJoint.__init__(self, 'arm')
+    def __init__(self,usb=None):
+        PrismaticJoint.__init__(self, name='arm',usb=usb)
 
     # ######### Utilties ##############################
 
     def motor_rad_to_translate_m(self,ang): #input in rad, output m
         return (self.params['chain_pitch']*self.params['chain_sprocket_teeth']/self.params['gr_spur']/(math.pi*2))*ang
 
     def translate_m_to_motor_rad(self, x):
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/base.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 import logging
 import numpy
 
 class Base(Device):
     """
     API to the Stretch Mobile Base
     """
-    def __init__(self):
+    def __init__(self, usb_left=None, usb_right=None):
         Device.__init__(self, 'base')
-        self.left_wheel = Stepper(usb='/dev/hello-motor-left-wheel')
-        self.right_wheel = Stepper(usb='/dev/hello-motor-right-wheel')
+        if usb_left is None:
+            usb_left = self.params['usb_name_left_wheel']
+        if usb_right is None:
+            usb_right = self.params['usb_name_right_wheel']
+        self.left_wheel = Stepper(usb=usb_left, name='hello-motor-left-wheel')
+        self.right_wheel = Stepper(usb=usb_right, name='hello-motor-right-wheel')
         self.status = {'timestamp_pc':0,'x':0,'y':0,'theta':0,'x_vel':0,'y_vel':0,'theta_vel':0, 'pose_time_s':0,'effort': [0, 0], 'left_wheel': self.left_wheel.status, 'right_wheel': self.right_wheel.status, 'translation_force': 0, 'rotation_torque': 0}
         self.trajectory = DiffDriveTrajectory()
         self._waypoint_lwpos = None
         self._waypoint_rwpos = None
         self.thread_rate_hz = 5.0
         self.first_step=True
         wheel_circumference_m = self.params['wheel_diameter_m'] * pi
@@ -30,17 +34,19 @@
         self.stiffness=1.0
         self.vel_mr=self.translate_to_motor_rad(self.params['motion']['default']['vel_m'])
         self.accel_mr=self.translate_to_motor_rad(self.params['motion']['default']['accel_m'])
         self.fast_motion_allowed = True
     # ###########  Device Methods #############
 
     def startup(self, threaded=True):
-        Device.startup(self, threaded=threaded)
-        success=self.left_wheel.startup(threaded=False) and self.right_wheel.startup(threaded=False)
-        self.__update_status()
+        #Startup steppers first so that status is populated before this Device thread begins (if threaded==true)
+        success = self.left_wheel.startup(threaded=False) and self.right_wheel.startup(threaded=False)
+        if success:
+            Device.startup(self, threaded=threaded)
+            self.__update_status()
         return success
 
     def _thread_loop(self):
         self.pull_status()
         self.update_trajectory()
 
     def stop(self):
@@ -413,14 +419,20 @@
         self._waypoint_lwpos = self.left_wheel.status['pos']
         self._waypoint_rwpos = self.right_wheel.status['pos']
         ls0, rs0 = self.trajectory.get_wheel_segments(0, self.translate_to_motor_rad, self.rotate_to_motor_rad,
             self._waypoint_lwpos, self._waypoint_rwpos)
         return self.left_wheel.start_waypoint_trajectory(ls0.to_array()) and \
             self.right_wheel.start_waypoint_trajectory(rs0.to_array())
 
+    def reset_odometry(self):
+        """
+        Reset X/Y/Theta to report 0
+        """
+        self.first_step = True
+
     def is_trajectory_active(self):
         return (self.left_wheel.status['waypoint_traj']['state'] == 'active' or self.right_wheel.status['waypoint_traj']['state'] == 'active')
 
     def get_trajectory_ts(self):
         # Return trajectory execution time
         if self.is_trajectory_active() and self.left_wheel._waypoint_ts is not None and self.right_wheel._waypoint_ts:
             return max(time.time()-self.left_wheel._waypoint_ts,time.time()-self.right_wheel._waypoint_ts)
@@ -514,17 +526,25 @@
         """
         Computes base odometery based on stepper positions / velocities
         """
         self.left_wheel.pull_status()
         self.right_wheel.pull_status()
         self.__update_status()
 
+    async def pull_status_async(self):
+        """
+        Computes base odometery based on stepper positions / velocities
+        """
+        await self.left_wheel.pull_status_async()
+        await self.right_wheel.pull_status_async()
+        self.__update_status()
+
     def __update_status(self):
-        self.status['timestamp_pc'] = time.time()
 
+        self.status['timestamp_pc'] = time.time()
         p0 = self.status['left_wheel']['pos']
         p1 = self.status['right_wheel']['pos']
         t0 = self.status['left_wheel']['timestamp']
         t1 = self.status['right_wheel']['timestamp']
         self.status['translation_force'] = 0 #Deprecated
         self.status['rotation_torque'] = 0 #Deprecated
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/device.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from __future__ import print_function
 from stretch_body.robot_params import RobotParams
 import stretch_body.hello_utils as hello_utils
 import time
 import logging, logging.config
 import threading
 import sys
+import os
 
 class DeviceTimestamp:
     def __init__(self):
+        self.reset()
+
+    def reset(self):
         self.timestamp_last = None
         self.timestamp_base = 0
-        self.timestamp_first= None
-        self.ts_start=time.time()
+        self.timestamp_first = None
+        self.ts_start = time.time()
 
     def set(self, ts): #take a timestamp from a uC in uS and put in terms of system clock
         if self.timestamp_last is None:  # First time
             self.timestamp_last = ts
             self.timestamp_first=ts
         if ts - self.timestamp_last < 0:  # rollover
             self.timestamp_base = self.timestamp_base + 0xFFFFFFFF
         self.timestamp_last = ts
         s=(self.timestamp_base + ts - self.timestamp_first) / 1000000.0
         return self.ts_start+s
 
 
 class Device:
     logging_params = RobotParams.get_params()[1]['logging']
+    os.system('mkdir -p '+hello_utils.get_stretch_directory("/log/stretch_body_logger")) #Some robots may not have this directory yet
     logging.config.dictConfig(logging_params)
     """
     Generic base class for all custom Stretch hardware
     """
     def __init__(self, name='',req_params=True):
         self.name = name
         self.user_params, self.robot_params = RobotParams.get_params()
         self.params = self.robot_params.get(self.name, {})
         self.logger = logging.getLogger(self.name)
 
         if self.params == {} and req_params:
-                self.logger.warning('Parameters for device %s not found. Check parameter YAML and device name. Exiting...' % self.name)
-                sys.exit(1)
+            self.logger.error('Parameters for device %s not found. Check parameter YAML and device name. Exiting...' % self.name)
+            sys.exit(1)
 
         self.timestamp = DeviceTimestamp()
         self.thread_active = False
         self.thread_rate_hz = 25.0
         self.thread_stats = None
         self.thread = None
         self.thread_shutdown_flag = threading.Event()
@@ -96,27 +101,27 @@
     def pretty_print(self):
         print('----- {0} ------ '.format(self.name))
         hello_utils.pretty_print_dict("params", self.params)
 
     def write_device_params(self,device_name, params,fleet_dir=None):
         raise DeprecationWarning('This method has been deprecated since v0.3.0')
 
-    def write_configuration_param_to_YAML(self,param_name,value,fleet_dir=None):
+    def write_configuration_param_to_YAML(self,param_name,value,fleet_dir=None,force_creation=False):
         """
         Update the robot configuration YAML with a new value
         """
-        self._write_param_to_YAML(param_name,value,filename='stretch_configuration_params.yaml',fleet_dir=fleet_dir)
+        self._write_param_to_YAML(param_name,value,filename='stretch_configuration_params.yaml',fleet_dir=fleet_dir,force_creation=force_creation)
 
-    def write_user_param_to_YAML(self, param_name, value, fleet_dir=None):
+    def write_user_param_to_YAML(self, param_name, value, fleet_dir=None,force_creation=False):
         """
         Update the robot configuration YAML with a new value
         """
-        self._write_param_to_YAML(param_name, value, filename='stretch_user_params.yaml', fleet_dir=fleet_dir)
+        self._write_param_to_YAML(param_name, value, filename='stretch_user_params.yaml', fleet_dir=fleet_dir,force_creation=force_creation)
 
-    def _write_param_to_YAML(self,param_name,value,filename,fleet_dir=None):
+    def _write_param_to_YAML(self,param_name,value,filename,fleet_dir=None,force_creation=False):
         """
         Update the YAML with a new value
         The param_name has the form device.key, or for a nested dictionary, device.key1.key2...
         For example, write_configuration_param_to_YAML('pimu.config.cliff_zero',100) will set this value to 100 in the YAML
         """
         cp = hello_utils.read_fleet_yaml(filename, fleet_dir=fleet_dir)
         param_keys=param_name.split('.')
@@ -124,15 +129,22 @@
         for param_key in param_keys:
             if param_key in d:
                 if param_key==param_keys[-1]:
                     d[param_key] = value
                 else:
                     d = d[param_key]
             else:
-                print('Improper param_name in _write_param_to_YAML. Not able to update %s' % param_name)
+                if force_creation:
+                    if param_key == param_keys[-1]:
+                        d[param_key] = value
+                    else:
+                        d[param_key] = {}
+                        d=d[param_key]
+                else:
+                    print('Improper param_name in _write_param_to_YAML. Not able to update %s' % param_name)
         hello_utils.write_fleet_yaml(filename, cp, fleet_dir=fleet_dir)
 
     # ########### Thread interface #############
 
     def _thread_loop(self):
         # self.step_sentry(robot=None) TODO: Support step_sentry here
         self.pull_status()
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_XL430.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_X_chain.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_X_chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     def get_motor(self,motor_name):
         try:
             return self.motors[motor_name]
         except (AttributeError, KeyError):
             return None
 
     def startup(self, threaded=False):
-        Device.startup(self, threaded=threaded)
         for mk in self.motors.keys():  # Provide nop data in case comm failures
             self.status[mk] = self.motors[mk].status
         if not self.hw_valid:
             return False
         if len(self.motors.keys()):
             try:
                 if self.params['use_group_sync_read']:
@@ -82,14 +81,15 @@
                         raise DynamixelCommError
                     self.status[mk] = self.motors[mk].status
                 self.pull_status()
             except DynamixelCommError:
                 self.comm_errors.add_error(rx=True,gsr=True)
                 self.hw_valid = False
                 return False
+        Device.startup(self, threaded=threaded)
         return True
 
     def _thread_loop(self):
         self.pull_status()
         self.update_trajectory()
 
     def stop(self):
@@ -124,46 +124,58 @@
             self.motors[motor].stop_trajectory()
 
     def pull_status(self):
         if not self.hw_valid:
             return
         try:
             ts = time.time()
+            error=False
             if self.params['use_group_sync_read']:
                 pos = self.sync_read(self.readers['pos'])
                 if pos==None and self.params['retry_on_comm_failure']:
                     pos = self.sync_read(self.readers['pos'])
+                error= error or (pos==None)
 
                 vel = self.sync_read(self.readers['vel'])
                 if vel == None and self.params['retry_on_comm_failure']:
                     vel = self.sync_read(self.readers['vel'])
+                error = error or (vel == None)
 
                 if self.status_mux_id == 0:
                     effort = self.sync_read(self.readers['effort'])
                     if effort == None and self.params['retry_on_comm_failure']:
                         effort = self.sync_read(self.readers['effort'])
+                    error = error or (effort == None)
                 else:
                     effort = None
 
                 if self.status_mux_id == 1:
                     temp = self.sync_read(self.readers['temp'])
                     if temp == None and self.params['retry_on_comm_failure']:
                         temp = self.sync_read(self.readers['temp'])
+                    error = error or (temp == None)
                 else:
                     temp = None
 
                 if self.status_mux_id == 2:
                     hardware_error = self.sync_read(self.readers['hardware_error'])
                     if hardware_error == None and self.params['retry_on_comm_failure']:
                         hardware_error = self.sync_read(self.readers['hardware_error'])
+                    error = error or (hardware_error == None)
                 else:
                     hardware_error = None
 
                 self.status_mux_id = (self.status_mux_id + 1) % 3
 
+                if error:
+                    self.comm_errors.add_error(rx=True, gsr=True)
+                    self.logger.warning('Dynamixel communication error during pull_status on %s: ' % self.name)
+                    #self.port_handler.ser.reset_output_buffer()
+                    #self.port_handler.ser.reset_input_buffer()
+
                 idx = 0
                 # Build dictionary of status data and push to each motor status
                 # None may indicate comm error or the field wasn't read on this mux cycle
                 for mk in self.motors.keys():
                     data = {'ts': time.time()}
                     if pos is not None:
                         data['x'] = pos[idx]
@@ -189,38 +201,39 @@
                     idx = idx + 1
             else:
                 for m in self.motors:
                     with self.pt_lock:
                         self.motors[m].pull_status()
         except(DynamixelCommError, IOError):
             self.comm_errors.add_error(rx=True, gsr=True)
-            self.port_handler.ser.reset_output_buffer()
-            self.port_handler.ser.reset_input_buffer()
+            self.logger.warning('Dynamixel communication error during pull_status on %s: ' % self.name)
 
     def pretty_print(self):
         print('--- Dynamixel X Chain ---')
         print('USB', self.usb)
         for mk in self.motors.keys():
             self.motors[mk].pretty_print()
 
     def sync_read(self, reader):
         if not self.hw_valid:
             return None
         with self.pt_lock:
             result = reader.txRxPacket()
         if result != COMM_SUCCESS:
             self.logger.debug('Dynamixel X sync read txRxPacket failed with error code = ' + str(result))
-            raise DynamixelCommError
+            return None
+            #raise DynamixelCommError
 
         def get_val(id_num):
             try:
-                b = reader.getData(id_num, reader.start_address, reader.data_length)
+                with self.pt_lock:
+                    b = reader.getData(id_num, reader.start_address, reader.data_length)
             except IndexError:
                 #Bad data struct size possible to raise Index Error
-                raise DynamixelCommError
+                return None #raise DynamixelCommError
             # The error code seems to be 0, yet there are also
             # circumstances where b will be 0 without an error, such
             # as being at position = 0. For now, I am commenting out
             # this error reporting code. One possibility is to edit
             # the SDK module. Another possibility is to use the
             # Available command separately.
             #
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/dynamixel_hello_XL430.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,31 +49,34 @@
 
 
 
 class DynamixelHelloXL430(Device):
     """
     Abstract the Dynamixel X-Series to handle calibration, radians, etc
     """
-    def __init__(self, name, chain=None):
+    def __init__(self, name, chain=None, usb=None):
         Device.__init__(self, name)
         try:
             self.chain = chain
             self.hw_valid = False
             self.status={'timestamp_pc':0,'comm_errors':0,'pos':0,'vel':0,'effort':0,'temp':0,'shutdown':0, 'hardware_error':0,
                          'input_voltage_error':0,'overheating_error':0,'motor_encoder_error':0,'electrical_shock_error':0,'overload_error':0,
                          'stalled':0,'stall_overload':0,'pos_ticks':0,'vel_ticks':0,'effort_ticks':0,'watchdog_errors':0}
             self.thread_rate_hz = 15.0
             self.trajectory = RevoluteTrajectory()
             self._waypoint_ts = None
             self._waypoint_vel = self.params['motion']['trajectory_max']['vel_r']
             self._waypoint_accel = self.params['motion']['trajectory_max']['accel_r']
+            self.usb = usb
+            if self.usb is None:
+                self.usb = self.params['usb_name']
 
             #Share bus resource amongst many XL430s
             self.motor = DynamixelXL430(dxl_id=self.params['id'],
-                                        usb=self.params['usb_name'],
+                                        usb=self.usb,
                                         port_handler=None if chain is None else chain.port_handler,
                                         pt_lock=None if chain is None else chain.pt_lock,
                                         baud=self.params['baud'],
                                         logger=self.logger)
             self.polarity = -1.0 if self.params['flip_encoder_polarity'] else 1.0
             self.ts_over_eff_start=None
             self.is_calibrated=False
@@ -88,14 +91,16 @@
 
             self.is_homing=False
             self.status_mux_id = 0
             self.was_runstopped = False
             self.comm_errors = DynamixelCommErrorStats(name,logger=self.logger)
             self.v_des = None #Track the motion profile settings on servo
             self.a_des = None #Track the motion profile settings on servo
+            self.warn_error=False
+            self.bubble_up_comm_exception=False
         except KeyError:
             self.motor=None
 
     # ###########  Device Methods #############
 
     def check_homing_offset(self):
         """
@@ -152,14 +157,28 @@
         self.soft_motion_limits['current'][1]=min(filter(lambda x: x is not None, [self.soft_motion_limits['collision'][1],self.soft_motion_limits['hard'][1],self.soft_motion_limits['user'][1]]))
 
     # ###################################################
 
     def do_ping(self, verbose=False):
         return self.motor.do_ping(verbose)
 
+    def check_servo_errors(self):
+        if self.status['overload_error']:
+            msg = 'WARNING: Servo %s in error state: overload_error. Reboot servo with stretch_robot_dynamixel_reboot.py' % self.name
+            self.logger.warning(msg)
+            self.warn_error = True
+            return False
+
+        if self.status['overheating_error']:
+            msg = 'WARNING: Servo %s in error state: overheating_error. Reboot servo with stretch_robot_dynamixel_reboot.py' % self.name
+            self.logger.warning(msg)
+            self.warn_error=True
+            return False
+        return True
+
     def startup(self, threaded=False):
         if self.motor is None:
             return False
         Device.startup(self, threaded=threaded)
         try:
             if self.motor.do_ping(verbose=False):
                 self.hw_valid = True
@@ -181,22 +200,32 @@
                 self.set_motion_params() #Initialize servo motion profile with default values
                 self.pre_traj_vel = None
                 self.pre_traj_acc = None
 
                 self.is_calibrated=self.motor.is_calibrated()
                 self.check_homing_offset()
                 self.enable_torque()
+                #Pull 3 times given mux / init the status dict
+                self.pull_status()
                 self.pull_status()
+                self.pull_status()
+
+                if not self.check_servo_errors():
+
+                    self.hw_valid = False
+                    return False
+
                 return True
             else:
                 self.logger.warning('DynamixelHelloXL430 Ping failed... %s' % self.name)
                 print('DynamixelHelloXL430 Ping failed...', self.name)
                 return False
         except DynamixelCommError:
             self.logger.warning('DynamixelHelloXL430 Ping failed... %s' % self.name)
+            self.comm_errors.add_error(rx=False, gsr=False)
             print('DynamixelHelloXL430 Ping failed...', self.name)
             return False
 
     def _thread_loop(self):
         self.pull_status()
         self.update_trajectory()
 
@@ -254,23 +283,28 @@
                         err = self.motor.get_hardware_error()
                     err_valid = self.motor.last_comm_success
                 else:
                     err = self.status['hardware_error']
 
                 self.status_mux_id = (self.status_mux_id + 1) % 3
 
+                self.check_servo_errors()
 
                 if not pos_valid or not vel_valid or not eff_valid or not temp_valid or not err_valid:
-                    raise DynamixelCommError
+                    self.logger.warning('Dynamixel communication error during pull_status on %s: ' % self.name)
+                    self.comm_errors.add_error(rx=True, gsr=False)
+                    return
                 ts = time.time()
             except(termios.error, DynamixelCommError, IndexError):
-                self.logger.warning('Dynamixel communication error on %s: '%self.name)
-                self.motor.port_handler.ser.reset_output_buffer()
-                self.motor.port_handler.ser.reset_input_buffer()
+                self.logger.warning('Dynamixel communication error during pull_status  on %s: '%self.name)
+                # self.motor.port_handler.ser.reset_output_buffer()
+                # self.motor.port_handler.ser.reset_input_buffer()
                 self.comm_errors.add_error(rx=True,gsr=False)
+                if self.bubble_up_comm_exception:
+                    raise DynamixelCommError
                 return
         else:
             x = data['x']
             v = data['v']
             eff = data['eff']
             temp = data['temp']
             ts = data['ts']
@@ -331,15 +365,15 @@
         Returns
         -------
         bool
             True if success, False if timeout
         """
         ts = time.time()
         while time.time() - ts < timeout:
-            if self.motor.get_moving_status() & 1 == 1:
+            if  self.motor.get_moving_status()& 1 == 1:
                 return True
             time.sleep(0.1)
         return False
 
     def pretty_print(self):
         if not self.hw_valid:
             print('----- HelloXL430 ------ ')
@@ -396,47 +430,62 @@
 
     def disable_torque(self):
         if not self.hw_valid:
             return
         self.motor.disable_torque()
 
     def move_to_vel(self,v_des,a_des=None):
+        nretry = 2
         if not self.hw_valid:
             return
         if self.params['req_calibration'] and not self.is_calibrated:
             self.logger.warning('Dynamixel not calibrated: %s' % self.name)
             print('Dynamixel not calibrated:', self.name)
             return
-        try:
-            self.motor.set_vel(v_des)
-        except(termios.error, DynamixelCommError, IndexError):
-            self.logger.warning('Dynamixel communication error on %s: ' % self.name)
-            self.comm_errors.add_error(rx=True, gsr=False)
+        success = False
+        for i in range(nretry):
+            try:
+                self.motor.set_vel(v_des)
+                success = True
+                break
+            except(termios.error, DynamixelCommError, IndexError):
+                self.logger.warning('Dynamixel communication error during move_to_vel on %s: ' % self.name)
+                self.comm_errors.add_error(rx=True, gsr=False)
+                if self.bubble_up_comm_exception:
+                    raise DynamixelCommError
+
 
     def move_to(self,x_des, v_des=None, a_des=None):
+        nretry = 2
         if not self.hw_valid:
             return
         if self.params['req_calibration'] and not self.is_calibrated:
             self.logger.warning('Dynamixel not calibrated: %s' % self.name)
             print('Dynamixel not calibrated:', self.name)
             return
-        try:
-            #print('Motion Params',v_des,a_des)
-            self.set_motion_params(v_des,a_des)
-            old_x_des = x_des
-            x_des = min(max(self.get_soft_motion_limits()[0], x_des), self.get_soft_motion_limits()[1])
-            if x_des != old_x_des:
-                self.logger.debug('Clipping move_to({0}) with soft limits {1}'.format(old_x_des, self.soft_motion_limits['current']))
-            t_des = self.world_rad_to_ticks(x_des)
-            t_des = max(self.params['range_t'][0], min(self.params['range_t'][1], t_des))
-            self.motor.go_to_pos(t_des)
-        except (termios.error, DynamixelCommError, IndexError):
-            self.logger.warning('Dynamixel communication error on: %s' % self.name)
-            self.comm_errors.add_error(rx=False, gsr=False)
 
+        #print('Motion Params',v_des,a_des)
+        self.set_motion_params(v_des,a_des)
+        old_x_des = x_des
+        x_des = min(max(self.get_soft_motion_limits()[0], x_des), self.get_soft_motion_limits()[1])
+        if x_des != old_x_des:
+            self.logger.debug('Clipping move_to({0}) with soft limits {1}'.format(old_x_des, self.soft_motion_limits['current']))
+        t_des = self.world_rad_to_ticks(x_des)
+        t_des = max(self.params['range_t'][0], min(self.params['range_t'][1], t_des))
+        success=False
+        for i in range(nretry):
+            try:
+                self.motor.go_to_pos(t_des)
+                success=True
+                break
+            except (termios.error, DynamixelCommError, IndexError):
+                self.logger.warning('Dynamixel communication error during move_to on %s: ' % self.name)
+                self.comm_errors.add_error(rx=False, gsr=False)
+                if self.bubble_up_comm_exception:
+                    raise DynamixelCommError
 
     def set_motion_params(self,v_des=None,a_des=None, force=False):
         try:
             if not self.hw_valid:
                 return
             v_des = abs(v_des) if v_des is not None else self.params['motion']['default']['vel']
             v_des = min(self.params['motion']['max']['vel'], v_des)
@@ -446,16 +495,18 @@
 
             a_des = abs(a_des) if a_des is not None else self.params['motion']['default']['accel']
             a_des = min(self.params['motion']['max']['accel'], a_des)
             if a_des != self.a_des or force:
                 self.motor.set_profile_acceleration(abs(self.world_rad_to_ticks_per_sec_sec(a_des)))
                 self.a_des = a_des
         except (termios.error, DynamixelCommError):
-            #self.logger.warning('Dynamixel communication error on: %s' % self.name)
+            self.logger.warning('Dynamixel communication error during set_motion_params on: %s' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
 
     def move_by(self,x_des, v_des=None, a_des=None):
         if not self.hw_valid:
             return
         try:
             if abs(x_des) > 0.00002: #Avoid drift
@@ -465,58 +516,72 @@
 
                 if self.motor.last_comm_success:
                     cx=self.ticks_to_world_rad(x)
                     self.move_to(cx + x_des, v_des, a_des)
                 else:
                     self.logger.debug('Move_By comm failure on %s' % self.name)
         except (termios.error, DynamixelCommError):
-            #self.logger.warning('Dynamixel communication error on: %s' % self.name)
+            self.logger.warning('Dynamixel communication error during move_by on %s: ' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
     def quick_stop(self):
         if not self.hw_valid:
             return
         try:
             self.motor.disable_torque()
             self.motor.enable_torque()
         except (termios.error, DynamixelCommError):
+            self.logger.warning('Dynamixel communication error during quick_stop on %s: ' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
     def enable_pos(self):
         if not self.hw_valid:
             return
         try:
             self.motor.disable_torque()
             if self.params['use_multiturn']:
                 self.motor.enable_multiturn()
             else:
                 self.motor.enable_pos()
             self.motor.enable_torque()
             self.set_motion_params(force=True)
         except (termios.error, DynamixelCommError):
+            self.logger.warning('Dynamixel communication error during enable_pos on %s: ' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
     def enable_pwm(self):
         if not self.hw_valid:
             return
         try:
             self.motor.disable_torque()
             self.motor.enable_pwm()
             self.motor.enable_torque()
         except (termios.error, DynamixelCommError):
+            self.logger.warning('Dynamixel communication error during enable_pwm on %s: ' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
 
     def set_pwm(self,x):
         if not self.hw_valid:
             return
         try:
             self.motor.set_pwm(x)
         except (termios.error, DynamixelCommError):
+            self.logger.warning('Dynamixel communication error during set_pwm on %s: ' % self.name)
             self.comm_errors.add_error(rx=False, gsr=False)
+            if self.bubble_up_comm_exception:
+                raise DynamixelCommError
 
     # ######### Waypoint Trajectory Interface ##############################
 
     def is_trajectory_active(self):
         return self._waypoint_ts !=None
 
     def get_trajectory_ts(self):
@@ -717,118 +782,126 @@
 
     def home(self, single_stop=False, move_to_zero=True,delay_at_stop=0.0,save_calibration=False,set_homing_offset=True):
         # Requires at least one hardstop in the pwm_homing[0] direction
         # Can be in multiturn or single turn mode
         # Mark the first hardstop as zero ticks on the Dynammixel
         # Second hardstop is optional
         # Return success, measured range
+        self.bubble_up_comm_exception=True
+        try:
+            if not self.hw_valid:
+                self.logger.warning('Not able to home %s. Hardware not present'%self.name)
+                return False, None
+            if not self.params['req_calibration']:
+                print('Homing not required for: '+self.name)
+                return False, None
 
-        if not self.hw_valid:
-            self.logger.warning('Not able to home %s. Hardware not present'%self.name)
-            return False, None
-        if not self.params['req_calibration']:
-            print('Homing not required for: '+self.name)
-            return False, None
-
-        self.pull_status()
-        if self.status['overload_error'] or self.status['overheating_error']:
-            self.logger.warning('Hardware error, unable to home. Exiting')
-            return False, None
-
-        self.is_homing=True
-        self.enable_pwm()
-        print('Moving to first hardstop...')
-        self.set_pwm(self.params['pwm_homing'][0])
-        ts=time.time()
-        time.sleep(1.0)
-        timeout=False
-        while self.motor.is_moving() and not timeout:
-            timeout=time.time()-ts>15.0
-            time.sleep(0.5)
-        time.sleep(delay_at_stop)
-        self.set_pwm(0)
-
-        if timeout:
-            self.logger.warning('Timed out moving to first hardstop. Exiting.')
-            return False, None
-        if self.status['overload_error'] or self.status['overheating_error']:
-            self.logger.warning('Hardware error, unable to home. Exiting')
-            return False, None
-
-        #Need to move back to pos mode to get the position (ticks) w/o the homing offset (single turn mode)
-        if not self.params['use_multiturn']:
-            self.enable_pos()
-        contact_0 = self.motor.get_pos()
-        print('First hardstop contact at position (ticks): %d' % contact_0)
-
-        if set_homing_offset:
-            print('-----')
-            self.motor.disable_torque()
-            print('Homing offset was %d'%self.motor.get_homing_offset())
-            print('Marking current position to zero ticks')
-            self.motor.zero_position()
-            print("Homing offset is now  %d (ticks)"%self.motor.get_homing_offset())
-            print('-----')
-            contact_0=0
-
-        self.motor.disable_torque()
-        self.motor.set_calibrated(1)
-        self.is_calibrated=1
-        self.motor.enable_torque()
-
-        self.enable_pwm()
+            self.pull_status()
 
-        print('Current position (ticks):',self.motor.get_pos())
+            if not self.check_servo_errors():
+                self.logger.warning('Hardware error, unable to home. Exiting')
+                return False, None
 
-        if not single_stop:
-            #Measure the range and write to YAML
-            print('Moving to second hardstop...')
-            self.set_pwm(self.params['pwm_homing'][1])
-            ts = time.time()
+            self.is_homing=True
+            self.enable_pwm()
+            print('Moving to first hardstop...')
+            self.set_pwm(self.params['pwm_homing'][0])
+            ts=time.time()
             time.sleep(1.0)
-            timeout = False
+            timeout=False
             while self.motor.is_moving() and not timeout:
-                timeout = time.time() - ts > 15.0
+                timeout=time.time()-ts>15.0
                 time.sleep(0.5)
             time.sleep(delay_at_stop)
             self.set_pwm(0)
 
             if timeout:
-                self.logger.warning('Timed out moving to second hardstop. Exiting.')
+                self.logger.warning('Timed out moving to first hardstop. Exiting.')
                 return False, None
-            if self.status['overload_error'] or self.status['overheating_error']:
+
+            if not self.check_servo_errors():
                 self.logger.warning('Hardware error, unable to home. Exiting')
                 return False, None
 
-            # Need to move back to pos mode to get the position (ticks) w/o the homing offset (single turn mode)
+            #Need to move back to pos mode to get the position (ticks) w/o the homing offset (single turn mode)
             if not self.params['use_multiturn']:
                 self.enable_pos()
-            contact_1 = self.motor.get_pos()
-            print('Hit second hardstop at: (ticks)', contact_1)
+            contact_0 = self.motor.get_pos()
+            print('First hardstop contact at position (ticks): %d' % contact_0)
+
+            if set_homing_offset:
+                print('-----')
+                self.motor.disable_torque()
+                print('Homing offset was %d'%self.motor.get_homing_offset())
+                print('Marking current position to zero ticks')
+                self.motor.zero_position()
+                print("Homing offset is now  %d (ticks)"%self.motor.get_homing_offset())
+                print('-----')
+                contact_0=0
 
-            print('Homed to range of motion to (ticks):',[contact_0,contact_1])
-            self.params['range_t'] = [contact_0 + self.params['range_pad_t'][0], contact_1 + self.params['range_pad_t'][1]]
-            print('Padded range of motion is (ticks):',self.params['range_t'])
-            r1=self.ticks_to_world_rad(self.params['range_t'][0])
-            r2=self.ticks_to_world_rad(self.params['range_t'][1])
-            print('   Radians:',[r1,r2])
-            print('   Degrees:',[rad_to_deg(r1),rad_to_deg(r2)])
+            self.motor.disable_torque()
+            self.motor.set_calibrated(1)
+            self.is_calibrated=1
+            self.motor.enable_torque()
 
-            if save_calibration:
-                self.write_configuration_param_to_YAML(self.name+'.range_t', self.params['range_t'])
+            self.enable_pwm()
 
-        self.enable_pos()
-        if move_to_zero:
-            print('Moving to calibrated zero: (rad)')
-            self.move_to(0)
-            self.wait_until_at_setpoint(timeout=6.0)
-        self.is_homing=False
-        if not single_stop:
-            return  True, self.params['range_t']
-        return True, None
+            print('Current position (ticks):',self.motor.get_pos())
+
+            if not single_stop:
+                #Measure the range and write to YAML
+                print('Moving to second hardstop...')
+                self.set_pwm(self.params['pwm_homing'][1])
+                ts = time.time()
+                time.sleep(1.0)
+                timeout = False
+                while self.motor.is_moving() and not timeout:
+                    timeout = time.time() - ts > 15.0
+                    time.sleep(0.5)
+                time.sleep(delay_at_stop)
+                self.set_pwm(0)
+
+                if timeout:
+                    self.logger.warning('Timed out moving to second hardstop. Exiting.')
+                    return False, None
+
+                if not self.check_servo_errors():
+                    self.logger.warning('Hardware error, unable to home. Exiting')
+                    return False, None
+
+                # Need to move back to pos mode to get the position (ticks) w/o the homing offset (single turn mode)
+                if not self.params['use_multiturn']:
+                    self.enable_pos()
+                contact_1 = self.motor.get_pos()
+                print('Hit second hardstop at: (ticks)', contact_1)
+
+                print('Homed to range of motion to (ticks):',[contact_0,contact_1])
+                self.params['range_t'] = [contact_0 + self.params['range_pad_t'][0], contact_1 + self.params['range_pad_t'][1]]
+                print('Padded range of motion is (ticks):',self.params['range_t'])
+                r1=self.ticks_to_world_rad(self.params['range_t'][0])
+                r2=self.ticks_to_world_rad(self.params['range_t'][1])
+                print('   Radians:',[r1,r2])
+                print('   Degrees:',[rad_to_deg(r1),rad_to_deg(r2)])
+
+                if save_calibration:
+                    self.write_configuration_param_to_YAML(self.name+'.range_t', self.params['range_t'])
+
+            self.enable_pos()
+            if move_to_zero:
+                print('Moving to calibrated zero: (rad)')
+                self.move_to(0)
+                self.wait_until_at_setpoint(timeout=6.0)
+            self.is_homing=False
+            self.bubble_up_comm_exception = False
+            if not single_stop:
+                return  True, self.params['range_t']
+            return True, None
+        except DynamixelCommError:
+            self.logger.warning('Communication error, unable to home. Exiting')
+            return False, None
 
 # ##########################################
 
     def ticks_to_world_rad_per_sec_sec(self,t):
         rps_servo=self.ticks_to_rad_per_sec_sec(t)
         return self.polarity*rps_servo/self.params['gr']
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/end_of_arm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import print_function
 from stretch_body.dynamixel_X_chain import DynamixelXChain
 import importlib
+from stretch_body.robot_params import RobotParams
 
 class EndOfArm(DynamixelXChain):
     """
     The EndOfArm class allows for an extensible serial chain of Dynamixel X series devices
     It allows the specific type of device to be declared at runtime via the Yaml parameters
     In this way, a user can add their own custom Dynamixel based tools to the robot end-of-arm by
     simply deriving it from DynamixelHelloXL430 and declaring the class name / Python module name
     in the User YAML file
     """
-    def __init__(self, name='end_of_arm'):
-        DynamixelXChain.__init__(self, usb='/dev/hello-dynamixel-wrist', name=name)
+    def __init__(self, name='end_of_arm', usb=None):
+        if usb is None:
+            usb = RobotParams.get_params()[1]['end_of_arm']['usb_name']
+        DynamixelXChain.__init__(self, usb=usb, name=name)
         self.joints = self.params.get('devices', {}).keys()
         for j in self.joints:
             module_name = self.params['devices'][j]['py_module_name']
             class_name = self.params['devices'][j]['py_class_name']
             dynamixel_device = getattr(importlib.import_module(module_name), class_name)(chain=self)
             self.add_motor(dynamixel_device)
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm_tools.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/head.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/head.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import print_function
 from stretch_body.dynamixel_hello_XL430 import DynamixelHelloXL430
 from stretch_body.hello_utils import *
 from stretch_body.dynamixel_X_chain import DynamixelXChain
+from stretch_body.robot_params import RobotParams
 
 class Head(DynamixelXChain):
     """
     API to the Stretch RE1 Head
     """
-    def __init__(self):
-        DynamixelXChain.__init__(self, usb='/dev/hello-dynamixel-head', name='head')
+    def __init__(self, usb=None):
+        if usb is None:
+            usb = RobotParams.get_params()[1]['head']['usb_name']
+        DynamixelXChain.__init__(self, usb=usb, name='head')
         self.joints = ['head_pan', 'head_tilt']
         for j in self.joints:
             self.add_motor(DynamixelHelloXL430(name=j, chain=self))
         self.poses = {'ahead': [0, 0], 'back': [deg_to_rad(-180), deg_to_rad(0)],
                       'tool': [deg_to_rad(-90), deg_to_rad(-45)],
                       'wheels': [deg_to_rad(0), deg_to_rad(-90)], 'left': [deg_to_rad(90), deg_to_rad(0)],
                       'up': [deg_to_rad(0), deg_to_rad(30)]}
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/hello_utils.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/hello_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import yaml
 import math
 import os
 import time
 import logging
 import numpy as np
 import sys
+import numbers
+
 
 def print_stretch_re_use():
     print("For use with S T R E T C H (R) RESEARCH EDITION from Hello Robot Inc.")
     print("---------------------------------------------------------------------\n")
 
 def create_time_string(time_format='%Y%m%d%H%M%S'):
     """Returns current time formatted as `time_format`
@@ -47,18 +49,20 @@
 
 def set_fleet_id(id):
     os.environ['HELLO_FLEET_ID']=id
 
 def get_fleet_directory():
     return os.environ['HELLO_FLEET_PATH']+'/'+get_fleet_id()+'/'
 
+
 def set_fleet_directory(fleet_path,fleet_id):
     os.environ['HELLO_FLEET_ID'] = fleet_id
     os.environ['HELLO_FLEET_PATH'] = fleet_path
 
+
 def get_stretch_directory(sub_directory=''):
     """Returns path to stretch_user dir if HELLO_FLEET_PATH env var exists
 
     Parameters
     ----------
     sub_directory : str
         valid sub_directory within stretch_user/
@@ -105,27 +109,45 @@
     with open(fleet_dir+fn, 'w') as yaml_file:
         if header is not None:
             yaml_file.write(header)
         yaml.dump(rp, yaml_file, default_flow_style=False)
 
 
 def overwrite_dict(overwritee_dict, overwriter_dict):
+    """Merge two dictionaries while overwriting common keys and
+    report errors when values of the same key differ in Python
+    type. The result gets stored in `overwritee_dict`.
+
+    Parameters
+    ----------
+    overwritee_dict : dict
+        The dictionary which will be overwritten. Use this as the merged result.
+    overwriter_dict : dict
+        The dictionary which will overwrite.
+
+    Returns
+    -------
+    bool
+        True if no mismatches were found during the overwrite, False otherwise.
+    """
+    no_mismatches = True
     for k in overwriter_dict.keys():
         if k in overwritee_dict:
-            if (type(overwritee_dict[k])==type(overwriter_dict[k])) or (type(overwritee_dict[k])==int and type(overwriter_dict[k])==float) or (type(overwritee_dict[k])==float and type(overwriter_dict[k])==int):
-                if type(overwritee_dict[k])==dict:
-                    overwrite_dict(overwritee_dict[k],overwriter_dict[k])
-                else:
-                    overwritee_dict[k]=overwriter_dict[k]
+            if (isinstance(overwritee_dict[k], dict) and isinstance(overwriter_dict[k], dict)):
+                sub_no_mismatches = overwrite_dict(overwritee_dict[k], overwriter_dict[k])
+                no_mismatches = no_mismatches and sub_no_mismatches
             else:
-                print('Overwritting Robot Params. Type mismatch for key:',k)
-                print('Overwriter',overwriter_dict[k])
-                print('Overwritee', overwritee_dict[k])
-        else: #If key not present, add anyhow (useful for adding new params)
+                if (type(overwritee_dict[k]) == type(overwriter_dict[k])) or (isinstance(overwritee_dict[k], numbers.Real) and isinstance(overwriter_dict[k], numbers.Real)):
+                    overwritee_dict[k] = overwriter_dict[k]
+                else:
+                    no_mismatches = False
+                    print('stretch_body.hello_utils.overwrite_dict ERROR: Type mismatch for key={0}, between overwritee={1} and overwriter={2}'.format(k, overwritee_dict[k], overwriter_dict[k]), file=sys.stderr)
+        else: #If key not present, add anyhow (useful for overlaying params)
             overwritee_dict[k] = overwriter_dict[k]
+    return no_mismatches
 
 def pretty_print_dict(title, d):
     """Print human readable representation of dictionary to terminal
 
     Parameters
     ----------
     title : str
@@ -148,15 +170,15 @@
     """
 
     def __init__(self, loop_name, target_loop_rate):
         self.loop_name = loop_name
         self.target_loop_rate = target_loop_rate
         self.ts_loop_start = None
         self.ts_loop_end = None
-        self.last_ts_loop_end = None
+        self.last_ts_loop_start = None
         self.status = {'execution_time_s': 0,
                        'curr_rate_hz': 0,
                        'avg_rate_hz': 0,
                        'supportable_rate_hz': 0,
                        'min_rate_hz': float('inf'),
                        'max_rate_hz': 0,
                        'std_rate_hz': 0,
@@ -164,44 +186,40 @@
                        'num_loops': 0}
         self.logger = logging.getLogger(self.loop_name)
         self.curr_rate_history = []
         self.supportable_rate_history = []
         self.n_history = 100
         self.debug_freq = 50
         self.sleep_time_s = 0.0
+        self.ts_0=time.time()
 
     def pretty_print(self):
         print('--------- TimingStats %s -----------' % self.loop_name)
         print('Target rate (Hz): %.2f' % self.target_loop_rate)
         print('Current rate (Hz): %.2f' % self.status['curr_rate_hz'])
         print('Average rate (Hz): %.2f' % self.status['avg_rate_hz'])
         print('Standard deviation of rate history (Hz): %.2f' % self.status['std_rate_hz'])
         print('Min rate (Hz): %.2f' % self.status['min_rate_hz'])
         print('Max rate (Hz): %.2f' % self.status['max_rate_hz'])
         print('Supportable rate (Hz): %.2f' % self.status['supportable_rate_hz'])
         print('Warnings: %d out of %d' % (self.status['missed_loops'], self.status['num_loops']))
 
     def mark_loop_start(self):
+        self.status['num_loops'] += 1
         self.ts_loop_start=time.time()
 
-    def mark_loop_end(self):
-        self.status['num_loops'] += 1
-        # First two cycles initialize vars / log
-        if not self.ts_loop_start:
-            return
-        if self.ts_loop_end is None:
-            self.ts_loop_end = time.time()
-            return
-        if self.last_ts_loop_end is None:
-            self.last_ts_loop_end = self.ts_loop_end
-            self.ts_loop_end = time.time()
-            self.status['execution_time_s'] = self.ts_loop_end - self.ts_loop_start
-            self.status['curr_rate_hz'] = 1.0 / (self.ts_loop_end - self.last_ts_loop_end)
+        if self.last_ts_loop_start is None: #Wait until have sufficient data
+            self.last_ts_loop_start=self.ts_loop_start
             return
 
+        self.status['curr_rate_hz'] = 1.0 / (self.ts_loop_start - self.last_ts_loop_start)
+        self.status['min_rate_hz'] = min(self.status['curr_rate_hz'], self.status['min_rate_hz'])
+        self.status['max_rate_hz'] = max(self.status['curr_rate_hz'], self.status['max_rate_hz'])
+
+
         # Calculate average and supportable loop rate **must be done before marking loop end**
         if len(self.curr_rate_history) >= self.n_history:
             self.curr_rate_history.pop(0)
         self.curr_rate_history.append(self.status['curr_rate_hz'])
         self.status['avg_rate_hz'] = np.mean(self.curr_rate_history)
         self.status['std_rate_hz'] = np.std(self.curr_rate_history)
         if len(self.supportable_rate_history) >= self.n_history:
@@ -219,29 +237,31 @@
             self.logger.debug('Min rate (Hz): %f' % self.status['min_rate_hz'])
             self.logger.debug('Max rate (Hz): %f' % self.status['max_rate_hz'])
             self.logger.debug('Supportable rate (Hz): %f' % self.status['supportable_rate_hz'])
             self.logger.debug('Standard deviation of supportable rate history (Hz): %f' % np.std(self.supportable_rate_history))
             self.logger.debug('Warnings: %d out of %d' % (self.status['missed_loops'], self.status['num_loops']))
             self.logger.debug('Sleep time (s): %f' % self.sleep_time_s)
 
-        # Calculate current loop rate & execution time
-        self.last_ts_loop_end = self.ts_loop_end
-        self.ts_loop_end = time.time()
-        self.status['execution_time_s'] = self.ts_loop_end - self.ts_loop_start
-        self.status['curr_rate_hz'] = 1.0 / (self.ts_loop_end - self.last_ts_loop_end)
-        self.status['min_rate_hz'] = min(self.status['curr_rate_hz'], self.status['min_rate_hz'])
-        self.status['max_rate_hz'] = max(self.status['curr_rate_hz'], self.status['max_rate_hz'])
+        self.last_ts_loop_start = self.ts_loop_start
 
         # Calculate sleep time to achieve desired loop rate
         self.sleep_time_s = (1 / self.target_loop_rate) - self.status['execution_time_s']
-        if self.sleep_time_s < 0.0:
+        if self.sleep_time_s < 0.0 and time.time()-self.ts_0>5.0: #Allow 5s for timing to stabilize on startup
             self.status['missed_loops'] += 1
             if self.status['missed_loops'] == 1:
                 self.logger.debug('Missed target loop rate of %.2f Hz for %s. Currently %.2f Hz' % (self.target_loop_rate, self.loop_name, self.status['curr_rate_hz']))
 
+    def mark_loop_end(self):
+        # First two cycles initialize vars / log
+        if self.ts_loop_start is None:
+            return
+        self.ts_loop_end = time.time()
+        self.status['execution_time_s'] = self.ts_loop_end - self.ts_loop_start
+
+
     def generate_rate_histogram(self, save=None):
         import matplotlib.pyplot as plt
         fig, axs = plt.subplots(1, 1, sharey=True, tight_layout=True)
         fig.suptitle('Distribution of loop rate (Hz). Target of %.2f ' % self.target_loop_rate)
         axs.hist(x=self.curr_rate_history, bins='auto', color='#0504aa', alpha=0.7, rwidth=0.85)
         plt.show() if save is None else plt.savefig(save)
 
@@ -249,15 +269,22 @@
         """
         Returns
         -------
         float : Time to sleep for to hit target loop rate
         """
         return max(0.0, self.sleep_time_s)
 
-    
+    def wait_until_ready_to_run(self,sleep=.0005):
+        if self.ts_loop_start is None:
+            time.sleep(.01)
+            return True
+        while time.time()-self.ts_loop_start<(1/self.target_loop_rate):
+            time.sleep(sleep)
+
+
 class ThreadServiceExit(Exception):
     """
     Custom exception which is used to trigger the clean exit
     of all running threads and the main program.
     """
     pass
 
@@ -466,25 +493,25 @@
     #Check if old parameters still found in YAML
     if ('contact_thresh_max_N' in joint.params) or ('contact_thresh_N' in joint.params):
         msg="Robot is using out-of-date contact parameters"
         msg=msg+'Please run tool RE1_migrate_contacts.py before continuing.\n'
         msg=msg+'For more details, see https://forum.hello-robot.com/t/476 \n'
         msg = msg + 'In method %s.%s' % (joint.name, method_name)
         print(msg)
-        joint.logger.warning(msg)
+        joint.logger.error(msg)
         sys.exit(1)
 
     #Check if code is passing in old values
     if contact_thresh_N is not None:
         msg='Use of parameter contact_thresh_N is no longer supported\n'
         msg= msg + 'Update your code to use (contact_thresh)\n'
         msg = msg +  'For more details, see https://forum.hello-robot.com/t/476\n'
         msg=msg+'In method %s.%s'%(joint.name,method_name)
         print(msg)
-        joint.logger.warning(msg)
+        joint.logger.error(msg)
         sys.exit(1)
 
 def check_deprecated_contact_model_prismatic_joint(joint,method_name, contact_thresh_pos_N,contact_thresh_neg_N,contact_thresh_pos,contact_thresh_neg ):
     """
     With RE2 we are transitioning entire stretch fleet to use new API (and effort_pct for the contact model)
     Catch older code that is using the older API and require updating of code
     For code that was, for example:
@@ -497,33 +524,33 @@
     #Check if old parameters still found in YAML
     if ('contact_thresh_max_N' in joint.params) or ('contact_thresh_N' in joint.params) or ('homing_force_N' in joint.params):
         msg="Robot is using out-of-date contact parameters\n"
         msg=msg+'Please run tool RE1_migrate_contacts.py before continuing.\n'
         msg=msg+'For more details, see https://forum.hello-robot.com/t/476 \n'
         msg = msg + 'In method %s.%s' % (joint.name, method_name)
         print(msg)
-        joint.logger.warning(msg)
+        joint.logger.error(msg)
         sys.exit(1)
 
     #Check if code is passing in old values
     if contact_thresh_pos_N is not None or contact_thresh_neg_N is not None:
         msg='Use of parameters contact_thresh_pos_N and contact_thresh_neg_N is no longer supported\n'
         msg= msg + 'Update your code to use (contact_thresh_pos, contact_thresh_neg)\n'
         msg = msg +  'For more details, see https://forum.hello-robot.com/t/476\n'
         msg=msg+'In method %s.%s'%(joint.name,method_name)
         print(msg)
-        joint.logger.warning(msg)
+        joint.logger.error(msg)
         sys.exit(1)
 
     #Check if code is passing in new values but not yet migrated
     if contact_thresh_pos is not None or contact_thresh_neg is not None \
             or (contact_thresh_pos is None and contact_thresh_neg is None):
         if ('contact_models' not in joint.params) or ('effort_pct' not in joint.params['contact_models']) or\
                 ('contact_thresh_default' not in joint.params['contact_models']['effort_pct']) or\
                 ('contact_thresh_homing' not in joint.params['contact_models']['effort_pct']) :
             msg='Effort_Pct contact parameters not available\n'
             msg = msg + 'Please run tool RE1_migrate_contacts.py before continuing.\n'
             msg = msg + 'For more details, see https://forum.hello-robot.com/t/476 \n'
             msg=msg+'In method %s.%s'%(joint.name,method_name)
             print(msg)
-            joint.logger.warning(msg)
+            joint.logger.error(msg)
             sys.exit(1)
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/lift.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/lift.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import math
 
 
 class Lift(PrismaticJoint):
     """
     API to the Stretch Lift
     """
-    def __init__(self):
-        PrismaticJoint.__init__(self, 'lift')
+    def __init__(self,usb=None):
+        PrismaticJoint.__init__(self, name='lift',usb=usb)
 
     # ######### Utilties ##############################
 
     def motor_rad_to_translate_m(self,ang): #input in rad
         d=self.params['pinion_t']*self.params['belt_pitch_m']/math.pi
         lift_m = (math.degrees(ang)/180.0)*math.pi*(d/2)
         return lift_m
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/pimu.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/pimu.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from stretch_body.transport import *
 from stretch_body.device import Device
 from stretch_body.hello_utils import *
 import textwrap
 import threading
 import psutil
 import time
-
+import array as arr
 
 # ######################## PIMU #################################
 
 """
 The PIMU is the power and IMU Arduino board in the base
 """
 
@@ -53,16 +53,15 @@
         print('Pitch (deg)', rad_to_deg(self.status['pitch']))
         print('Heading (deg)', rad_to_deg(self.status['heading']))
         print('Bump', self.status['bump'])
         print('Timestamp (s)', self.status['timestamp'])
         print('-----------------------')
 
     def unpack_status(self, s):
-        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
-            .format(self.board_info['protocol_version']))
+        raise NotImplementedError('This method not supported by IMU for firmware.')
 
 # ######################## IMU PROTOCOL P0 #################################
 class IMU_Protocol_P0(IMUBase):
     def unpack_status(self, s):
         # take in an array of bytes
         # this needs to exactly match the C struct format
         sidx=0
@@ -112,15 +111,16 @@
         return sidx
 
 # ######################## IMU #################################
 class IMU(IMUBase):
     def __init__(self):
         IMUBase.__init__(self)
         # Order in descending order so more recent protocols/methods override less recent
-        self.supported_protocols = {'p0': (IMU_Protocol_P0,), 'p1': (IMU_Protocol_P1,IMU_Protocol_P0,)}
+        self.supported_protocols = {'p0': (IMU_Protocol_P0,), 'p1': (IMU_Protocol_P1,IMU_Protocol_P0,),
+                                    'p2': (IMU_Protocol_P1,IMU_Protocol_P0,),'p3': (IMU_Protocol_P1,IMU_Protocol_P0,)}
 
 # ##################################################################################
 class PimuBase(Device):
     """
     API to the Stretch Power and IMU board (Pimu)
     """
     RPC_SET_PIMU_CONFIG = 1
@@ -129,132 +129,170 @@
     RPC_REPLY_PIMU_STATUS = 4
     RPC_SET_PIMU_TRIGGER = 5
     RPC_REPLY_PIMU_TRIGGER = 6
     RPC_GET_PIMU_BOARD_INFO = 7
     RPC_REPLY_PIMU_BOARD_INFO = 8
     RPC_SET_MOTOR_SYNC = 9
     RPC_REPLY_MOTOR_SYNC = 10
+    RPC_READ_TRACE =11
+    RPC_REPLY_READ_TRACE =12
+    RPC_GET_PIMU_STATUS_AUX = 13
+    RPC_REPLY_PIMU_STATUS_AUX = 14
+    RPC_LOAD_TEST_PULL = 15
+    RPC_REPLY_LOAD_TEST_PULL = 16
+    RPC_LOAD_TEST_PUSH = 17
+    RPC_REPLY_LOAD_TEST_PUSH = 18
 
     STATE_AT_CLIFF_0 = 1
     STATE_AT_CLIFF_1 = 2
     STATE_AT_CLIFF_2 = 4
     STATE_AT_CLIFF_3 = 8
     STATE_RUNSTOP_EVENT = 16
     STATE_CLIFF_EVENT = 32
     STATE_FAN_ON = 64
     STATE_BUZZER_ON = 128
     STATE_LOW_VOLTAGE_ALERT = 256
     STATE_OVER_TILT_ALERT = 512
     STATE_HIGH_CURRENT_ALERT = 1024
     STATE_CHARGER_CONNECTED = 2048
     STATE_BOOT_DETECTED = 4096
+    STATE_IS_TRACE_ON = 8192
 
     TRIGGER_BOARD_RESET = 1
     TRIGGER_RUNSTOP_RESET = 2
     TRIGGER_CLIFF_EVENT_RESET = 4
     TRIGGER_BUZZER_ON = 8
     TRIGGER_BUZZER_OFF = 16
     TRIGGER_FAN_ON = 32
     TRIGGER_FAN_OFF = 64
     TRIGGER_IMU_RESET = 128
     TRIGGER_RUNSTOP_ON = 256
     TRIGGER_BEEP = 512
     TRIGGER_LIGHTBAR_TEST = 1024
+    TRIGGER_ENABLE_TRACE= 2048
+    TRIGGER_DISABLE_TRACE=4096
+
 
+    TRACE_TYPE_STATUS = 0
+    TRACE_TYPE_DEBUG = 1
+    TRACE_TYPE_PRINT = 2
 
-    def __init__(self, event_reset=False):
+
+    def __init__(self, event_reset=False, usb=None):
         Device.__init__(self, 'pimu')
         self.config = self.params['config']
-        self.lock = threading.RLock()
         self.imu = IMU()
         self._dirty_config = True
         self._dirty_trigger = False
         self.frame_id_last = None
         self.frame_id_base = 0
-        self.transport = Transport(usb='/dev/hello-pimu', logger=self.logger)
+        if usb is None:
+            usb = self.params['usb_name']
+        self.transport = Transport(usb=usb, logger=self.logger)
         self.status = {'voltage': 0, 'current': 0, 'temp': 0,'cpu_temp': 0, 'cliff_range':[0,0,0,0], 'frame_id': 0,
                        'timestamp': 0,'at_cliff':[False,False,False,False], 'runstop_event': False, 'bump_event_cnt': 0,
                        'cliff_event': False, 'fan_on': False, 'buzzer_on': False, 'low_voltage_alert':False,'high_current_alert':False,'over_tilt_alert':False,
-                       'charger_connected':False, 'boot_detected':False,'imu': self.imu.status,'debug':0,'state':0,'motor_sync_drop':0,
+                       'charger_connected':False, 'boot_detected':False,'imu': self.imu.status,'debug':0,'state':0,'trace_on':0,
+                       'motor_sync_rate': 0, 'motor_sync_cnt': 0, 'motor_sync_queues': 0,
                        'transport': self.transport.status}
+
+        self.status_zero=self.status.copy()
+        self.status_aux = {'foo': 0}
+
         self._trigger=0
         self.ts_last_fan_on=None
         self.fan_on_last=False
         #Reset PIMU state so that Ctrl-C and re-instantiate Pimu class is efficient way to get out of an event
         if event_reset:
             self.runstop_event_reset()
             self.cliff_event_reset()
 
         self.board_info = {'board_variant': None, 'firmware_version': None, 'protocol_version': None,'hardware_id':0}
         self.hw_valid = False
         self.ts_last_motor_sync=None
         self.ts_last_motor_sync_warn=None
-
+        self.load_test_payload = arr.array('B', range(256)) * 4
+        self.ts_get_cpu_temp=0
+        self.get_cpu_temp()
 
     # ###########  Device Methods #############
 
     def startup(self, threaded=False):
         try:
             Device.startup(self, threaded=threaded)
-            with self.lock:
-                self.hw_valid = self.transport.startup()
-                if self.hw_valid:
-                    # Pull board info
-                    self.transport.payload_out[0] = self.RPC_GET_PIMU_BOARD_INFO
-                    self.transport.queue_rpc(1, self.rpc_board_info_reply)
-                    self.transport.step(exiting=False)
-                    return True
-                return False
+            self.hw_valid = self.transport.startup()
+            if self.hw_valid:
+                payload = arr.array('B', [self.RPC_GET_PIMU_BOARD_INFO])
+                self.transport.do_pull_rpc_sync(payload, self.rpc_board_info_reply)
+                self.transport.configure_version(self.board_info['firmware_version'])
+                return True
+            return False
         except KeyError:
             self.hw_valid =False
             return False
 
 
-
     def stop(self):
         Device.stop(self)
         if not self.hw_valid:
             return
-        with self.lock:
-            self.set_fan_off()
-            self.push_command(exiting=True)
-            self.transport.stop()
-            self.hw_valid = False
+        self.set_fan_off()
+        self.push_command(exiting=True)
+        self.transport.stop()
+        self.hw_valid = False
 
     def set_config(self,c):
-        with self.lock:
-            self.config=c.copy()
-            self._dirty_config = True
+        self.config=c.copy()
+        self._dirty_config = True
+
+    def pull_status(self, exiting=False):
+        if not self.hw_valid:
+            return
+        payload = arr.array('B', [self.RPC_GET_PIMU_STATUS])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_status_reply)
 
-    def pull_status(self,exiting=False):
+    async def pull_status_async(self, exiting=False):
         if not self.hw_valid:
             return
-        with self.lock:
-            # Queue Body Status RPC
-            self.transport.payload_out[0] = self.RPC_GET_PIMU_STATUS
-            self.transport.queue_rpc(1, self.rpc_status_reply)
-            self.transport.step(exiting=exiting)
+        payload = arr.array('B', [self.RPC_GET_PIMU_STATUS])
+        await self.transport.do_pull_rpc_async(payload, self.rpc_status_reply, exiting=exiting)
 
-    def push_command(self,exiting=False):
+    async def push_command_async(self, exiting=False):
         if not self.hw_valid:
             return
-        with self.lock:
-            if self._dirty_config:
-                self.transport.payload_out[0] = self.RPC_SET_PIMU_CONFIG
-                sidx = self.pack_config(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_config_reply)
-                self._dirty_config=False
-
-            if self._dirty_trigger:
-                self.transport.payload_out[0] = self.RPC_SET_PIMU_TRIGGER
-                sidx = self.pack_trigger(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_trigger_reply)
-                self._trigger=0
-                self._dirty_trigger=False
-            self.transport.step2(exiting=exiting)
+        payload = self.transport.get_empty_payload()
+        if self._dirty_config:
+            payload[0] = self.RPC_SET_PIMU_CONFIG
+            sidx = self.pack_config(payload, 1)
+            await self.transport.do_push_rpc_async(payload[:sidx], self.rpc_config_reply)
+            self._dirty_config = False
+
+        if self._dirty_trigger:
+            payload[0] = self.RPC_SET_PIMU_TRIGGER
+            sidx = self.pack_trigger(payload, 1)
+            await self.transport.do_push_rpc_async(payload[:sidx], self.rpc_trigger_reply)
+            self._trigger = 0
+            self._dirty_trigger = False
+
+    def push_command(self, exiting=False):
+        if not self.hw_valid:
+            return
+        payload = self.transport.get_empty_payload()
+        if self._dirty_config:
+            payload[0] = self.RPC_SET_PIMU_CONFIG
+            sidx = self.pack_config(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_config_reply)
+            self._dirty_config = False
+
+        if self._dirty_trigger:
+            payload[0] = self.RPC_SET_PIMU_TRIGGER
+            sidx = self.pack_trigger(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_trigger_reply)
+            self._trigger = 0
+            self._dirty_trigger = False
 
     def pretty_print(self):
         print('------ Pimu -----')
         print('Voltage',self.status['voltage'])
         print('Current', self.status['current'])
         print('CPU Temp',self.status['cpu_temp'])
         print('Board Temp', self.status['temp'])
@@ -265,114 +303,115 @@
         print('Runstop Event', self.status['runstop_event'])
         print('Bump Event Cnt', self.status['bump_event_cnt'])
         print('Fan On', self.status['fan_on'])
         print('Buzzer On', self.status['buzzer_on'])
         print('Low Voltage Alert', self.status['low_voltage_alert'])
         print('High Current Alert', self.status['high_current_alert'])
         print('Over Tilt Alert',self.status['over_tilt_alert'])
+        print('Trace on:', self.status['trace_on'])
         if self.board_info['hardware_id']>0:
             print('Charger Connected', self.status['charger_connected'])
             print('Boot Detected', self.status['boot_detected'])
         print('Debug', self.status['debug'])
         print('Timestamp (s)', self.status['timestamp'])
-        print('Read error', self.transport.status['read_error'])
-        print('Dropped motor sync',self.status['motor_sync_drop'])
+        #print('Read error', self.transport.status['read_error'])
+        print('Queued motor sync', self.status['motor_sync_queues'])
+        print('Motor sync rate', self.status['motor_sync_rate'])
+        print('Motor sync cnt', self.status['motor_sync_cnt'])
         print('Board variant:',self.board_info['board_variant'])
         print('Firmware version:', self.board_info['firmware_version'])
+        print('Transport version:', self.transport.version)
         self.imu.pretty_print()
 
     # ####################### User Functions #######################################################
 
+
     def runstop_event_reset(self):
         """
         Reset the robot runstop, allowing motion to continue
         """
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_RUNSTOP_RESET
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_RUNSTOP_RESET
+        self._dirty_trigger=True
 
     def runstop_event_trigger(self):
         """
         Trigger the robot runstop, stopping motion
         """
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_RUNSTOP_ON
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_RUNSTOP_ON
+        self._dirty_trigger=True
 
     def trigger_beep(self):
         """
         Generate a single short beep
         """
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_BEEP
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_BEEP
+        self._dirty_trigger=True
 
     def trigger_lightbar_test(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_LIGHTBAR_TEST
-            self._dirty_trigger = True
+        self._trigger = self._trigger | self.TRIGGER_LIGHTBAR_TEST
+        self._dirty_trigger = True
 
     # ####################### Utility functions ####################################################
     def imu_reset(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_IMU_RESET
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_IMU_RESET
+        self._dirty_trigger=True
 
-    def trigger_motor_sync(self):
-        #Push out immediately
-        if not self.hw_valid:
-            return
+
+    def is_ready_for_sync(self):
+        # For RE1.0 robots (hardware_id==0) the runstop and sync line are shared
+        # This limits the maximum rate that the motor sync can be triggered
+        # For RE2.0 robots the sync rate is limited by the min pulse width (~10ms)
+        #Track the rate that the sync is triggered
+        # This is called once prior to issuing stepper push_commands
+        # If it is True then trigger_motor_sync is safe to call after the push_commands
+        # By calling it first, it ensures that the sync rate is accurate (eg, not measuring timing of RPC, etc)
         t = time.time()
-        #For RE1.0 robots (hardware_id==0) the runstop and sync line are shared
-        #This limits the maximum rate that the motor sync can be triggered
-        #For RE2.0 robots the sync rate is limited by the min pulse width (~10ms)
         if self.ts_last_motor_sync is not None:
-            sync_rate = 1 / (t - self.ts_last_motor_sync)
-            if sync_rate>self.params['max_sync_rate_hz']:
+            rate=1 / (t - self.ts_last_motor_sync)
+            if rate>self.params['max_sync_rate_hz']:
                 self.status['motor_sync_drop'] += 1
                 if self.ts_last_motor_sync_warn is None or t-self.ts_last_motor_sync_warn>5.0:
-                    print('Warning: Rate of calls to Pimu:trigger_motor_sync rate of %f above maximum frequency of %.2f Hz. Motor commands dropped: %d'%(sync_rate,self.params['max_sync_rate_hz'],self.status['motor_sync_drop']))
+                    print('Warning: Rate of calls to Pimu:trigger_motor_sync rate of %f above maximum frequency of %.2f Hz. Motor commands dropped: %d'%(rate,self.params['max_sync_rate_hz'],self.status['motor_sync_drop']))
                     self.ts_last_motor_sync_warn=t
-                return
+                return False
+            self.status['motor_sync_rate'] = rate #Only update rate if it is ready
+        return True
+
+    def trigger_motor_sync(self):
+        #Push out immediately
+        if not self.hw_valid:
+            return
+        payload = arr.array('B', [self.RPC_SET_MOTOR_SYNC])
+        self.transport.do_push_rpc_sync(payload, self.rpc_motor_sync_reply)
+        self.ts_last_motor_sync = time.time()
 
-        with self.lock:
-            self.transport.payload_out[0] = self.RPC_SET_MOTOR_SYNC
-            self.transport.queue_rpc(1, self.rpc_motor_sync_reply)
-            self.transport.step()
-            self.ts_last_motor_sync = t
 
     def set_fan_on(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_FAN_ON
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_FAN_ON
+        self._dirty_trigger=True
 
     def set_fan_off(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_FAN_OFF
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_FAN_OFF
+        self._dirty_trigger=True
 
     def set_buzzer_on(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_BUZZER_ON
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_BUZZER_ON
+        self._dirty_trigger=True
 
     def set_buzzer_off(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_BUZZER_OFF
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_BUZZER_OFF
+        self._dirty_trigger=True
 
     def board_reset(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_BOARD_RESET
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_BOARD_RESET
+        self._dirty_trigger=True
 
     def cliff_event_reset(self):
-        with self.lock:
-            self._trigger=self._trigger | self.TRIGGER_CLIFF_EVENT_RESET
-            self._dirty_trigger=True
+        self._trigger=self._trigger | self.TRIGGER_CLIFF_EVENT_RESET
+        self._dirty_trigger=True
 
     # ########### Sensor Calibration #################
     def get_voltage(self,raw):
         raw_to_V = 20.0/1024 #10bit adc, 0-20V per 0-3.3V reading
         return raw*raw_to_V
 
 
@@ -386,69 +425,96 @@
         raw_to_mV = 3300 / 1024.0
         mV = raw * raw_to_mV
         mA = mV/.408 # conversion per circuit
         return mA/1000.0
     # ################Data Packing #####################
 
     def unpack_board_info(self,s):
-        with self.lock:
-            sidx=0
-            self.board_info['board_variant'] = unpack_string_t(s[sidx:], 20)
-            self.board_info['hardware_id'] = 0
-            if len(self.board_info['board_variant'])==6: #New format of Pimu.x Older format of Pimu.BoardName.Vx' If older format,default to 0
-                self.board_info['hardware_id']=int(self.board_info['board_variant'][-1])
-            sidx += 20
-            self.board_info['firmware_version'] = unpack_string_t(s[sidx:], 20)
-            self.board_info['protocol_version'] = self.board_info['firmware_version'][self.board_info['firmware_version'].rfind('p'):]
-            sidx += 20
-            return sidx
+        sidx=0
+        self.board_info['board_variant'] = unpack_string_t(s[sidx:], 20)
+        self.board_info['hardware_id'] = 0
+        if len(self.board_info['board_variant'])==6: #New format of Pimu.x Older format of Pimu.BoardName.Vx' If older format,default to 0
+            self.board_info['hardware_id']=int(self.board_info['board_variant'][-1])
+        sidx += 20
+        self.board_info['firmware_version'] = unpack_string_t(s[sidx:], 20)
+        self.board_info['protocol_version'] = self.board_info['firmware_version'][self.board_info['firmware_version'].rfind('p'):]
+        sidx += 20
+        return sidx
 
     def pack_config(self,s,sidx):
-        with self.lock:
-            for i in range(4):
-                pack_float_t(s, sidx, self.config['cliff_zero'][i])
-                sidx += 4
-            pack_float_t(s, sidx, self.config['cliff_thresh']);sidx += 4
-            pack_float_t(s, sidx, self.config['cliff_LPF']);sidx += 4
-            pack_float_t(s, sidx, self.config['voltage_LPF']);sidx += 4
-            pack_float_t(s, sidx, self.config['current_LPF']);sidx += 4
-            pack_float_t(s, sidx, self.config['temp_LPF']);sidx += 4
-            pack_uint8_t(s, sidx, self.config['stop_at_cliff']); sidx += 1
-            pack_uint8_t(s, sidx, self.config['stop_at_runstop']);sidx += 1
-            pack_uint8_t(s, sidx, self.config['stop_at_tilt']);sidx += 1
-            pack_uint8_t(s, sidx, self.config['stop_at_low_voltage']);sidx += 1
-            pack_uint8_t(s, sidx, self.config['stop_at_high_current']); sidx += 1
-            for i in range(3):
-                pack_float_t(s, sidx, self.config['mag_offsets'][i])
-                sidx += 4
-            for i in range(9):
-                pack_float_t(s, sidx, self.config['mag_softiron_matrix'][i])
-                sidx += 4
-            for i in range(3):
-                pack_float_t(s, sidx, self.config['gyro_zero_offsets'][i])
-                sidx += 4
-            pack_float_t(s, sidx, self.config['rate_gyro_vector_scale']); sidx += 4
-            pack_float_t(s, sidx, self.config['gravity_vector_scale']); sidx += 4
-            pack_float_t(s, sidx, self.config['accel_LPF']); sidx += 4
-            pack_float_t(s, sidx, self.config['bump_thresh']); sidx += 4
-            pack_float_t(s, sidx, self.config['low_voltage_alert']);sidx += 4
-            pack_float_t(s, sidx, self.config['high_current_alert']);sidx += 4
-            pack_float_t(s, sidx, self.config['over_tilt_alert']); sidx += 4
-            return sidx
+        for i in range(4):
+            pack_float_t(s, sidx, self.config['cliff_zero'][i])
+            sidx += 4
+        pack_float_t(s, sidx, self.config['cliff_thresh']);sidx += 4
+        pack_float_t(s, sidx, self.config['cliff_LPF']);sidx += 4
+        pack_float_t(s, sidx, self.config['voltage_LPF']);sidx += 4
+        pack_float_t(s, sidx, self.config['current_LPF']);sidx += 4
+        pack_float_t(s, sidx, self.config['temp_LPF']);sidx += 4
+        pack_uint8_t(s, sidx, self.config['stop_at_cliff']); sidx += 1
+        pack_uint8_t(s, sidx, self.config['stop_at_runstop']);sidx += 1
+        pack_uint8_t(s, sidx, self.config['stop_at_tilt']);sidx += 1
+        pack_uint8_t(s, sidx, self.config['stop_at_low_voltage']);sidx += 1
+        pack_uint8_t(s, sidx, self.config['stop_at_high_current']); sidx += 1
+        for i in range(3):
+            pack_float_t(s, sidx, self.config['mag_offsets'][i])
+            sidx += 4
+        for i in range(9):
+            pack_float_t(s, sidx, self.config['mag_softiron_matrix'][i])
+            sidx += 4
+        for i in range(3):
+            pack_float_t(s, sidx, self.config['gyro_zero_offsets'][i])
+            sidx += 4
+        pack_float_t(s, sidx, self.config['rate_gyro_vector_scale']); sidx += 4
+        pack_float_t(s, sidx, self.config['gravity_vector_scale']); sidx += 4
+        pack_float_t(s, sidx, self.config['accel_LPF']); sidx += 4
+        pack_float_t(s, sidx, self.config['bump_thresh']); sidx += 4
+        pack_float_t(s, sidx, self.config['low_voltage_alert']);sidx += 4
+        pack_float_t(s, sidx, self.config['high_current_alert']);sidx += 4
+        pack_float_t(s, sidx, self.config['over_tilt_alert']); sidx += 4
+        return sidx
 
     def pack_trigger(self,s,sidx):
-        with self.lock:
-            pack_uint32_t(s,sidx,self._trigger); sidx+=4
-            return sidx
+        pack_uint32_t(s,sidx,self._trigger); sidx+=4
+        return sidx
 
     def unpack_status(self,s):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
-    # ################Transport Callbacks #####################
+    def read_firmware_trace(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def rpc_read_firmware_trace_reply(self, reply):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def enable_firmware_trace(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def disable_firmware_trace(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+
+    def pull_status_aux(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+            .format(self.board_info['protocol_version']))
+
+
+    def push_load_test(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def pull_load_test(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+        # ################Transport Callbacks #####################
 
     def rpc_motor_sync_reply(self,reply):
         if reply[0] != self.RPC_REPLY_MOTOR_SYNC:
             self.logger.warning('Error RPC_REPLY_MOTOR_SYNC', reply[0])
 
     def rpc_config_reply(self,reply):
         if reply[0] != self.RPC_REPLY_PIMU_CONFIG:
@@ -471,152 +537,357 @@
             self.unpack_status(reply[1:])
         else:
             self.logger.warning('Error RPC_REPLY_PIMU_STATUS', reply[0])
 
 
     # ################ Sentry #####################
     def get_cpu_temp(self):
+        #Note, this call can be slow
         cpu_temp = 0
         try:
             t = psutil.sensors_temperatures()['coretemp']
             for c in t:
                 cpu_temp = max(cpu_temp, c.current)
         except(KeyError, IOError): #May not be available on virtual machines
             cpu_temp=25.0
         return cpu_temp
 
     def step_sentry(self,robot=None):
         if self.hw_valid and self.robot_params['robot_sentry']['base_fan_control']:
             #Manage CPU temp using the mobile base fan
             #See https://www.intel.com/content/www/us/en/support/articles/000005946/intel-nuc.html
-            cpu_temp=self.get_cpu_temp()
-            if cpu_temp>self.params['base_fan_on']:
+
+            if time.time()-self.ts_get_cpu_temp>10.0: #Once every 10s as is slow changing and is a slow sys call
+                self.status['cpu_temp']=self.get_cpu_temp()
+                self.ts_get_cpu_temp=time.time()
+            if self.status['cpu_temp']>self.params['base_fan_on']:
                 if self.ts_last_fan_on is None or time.time()-self.ts_last_fan_on>3.0: #Will turn itself off if don't refresh command
                     self.set_fan_on()
                     self.push_command()
                     self.ts_last_fan_on = time.time()
                 if  not self.status['fan_on']:
                     self.logger.debug('Base fan turned on')
 
             if self.fan_on_last and not self.status['fan_on']:
                 self.logger.debug('Base fan turned off')
 
-            if cpu_temp<self.params['base_fan_off']and self.status['fan_on']:
+            if self.status['cpu_temp']<self.params['base_fan_off']and self.status['fan_on']:
                 self.set_fan_off()
                 self.push_command()
             self.fan_on_last = self.status['fan_on']
 
 
+
 # ######################## PIMU PROTOCOL PO #################################
 
 class Pimu_Protocol_P0(PimuBase):
     def unpack_status(self,s):
-        with self.lock:
-            sidx=0
-            sidx +=self.imu.unpack_status((s[sidx:]))
-            self.status['voltage']=self.get_voltage(unpack_float_t(s[sidx:]));sidx+=4
-            self.status['current'] = self.get_current(unpack_float_t(s[sidx:]));sidx+=4
-            self.status['temp'] = self.get_temp(unpack_float_t(s[sidx:]));sidx+=4
-
-            for i in range(4):
-                self.status['cliff_range'][i]=unpack_float_t(s[sidx:])
-                sidx+=4
-
-            self.status['state'] = unpack_uint32_t(s[sidx:])
-            sidx += 4
-
-            self.status['at_cliff']=[]
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_0) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_1) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_2) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_3) != 0)
-            self.status['runstop_event'] = (self.status['state'] & self.STATE_RUNSTOP_EVENT) != 0
-            self.status['cliff_event'] = (self.status['state'] & self.STATE_CLIFF_EVENT) != 0
-            self.status['fan_on'] = (self.status['state'] & self.STATE_FAN_ON) != 0
-            self.status['buzzer_on'] = (self.status['state'] & self.STATE_BUZZER_ON) != 0
-            self.status['low_voltage_alert'] = (self.status['state'] & self.STATE_LOW_VOLTAGE_ALERT) != 0
-            self.status['high_current_alert'] = (self.status['state'] & self.STATE_HIGH_CURRENT_ALERT) != 0
-            self.status['over_tilt_alert'] = (self.status['state'] & self.STATE_OVER_TILT_ALERT) != 0
-            self.status['charger_connected'] = (self.status['state'] & self.STATE_CHARGER_CONNECTED) != 0
-            self.status['boot_detected'] = (self.status['state'] & self.STATE_BOOT_DETECTED) != 0
-            self.status['timestamp'] = self.timestamp.set(unpack_uint32_t(s[sidx:])); sidx += 4
-            self.status['bump_event_cnt'] = unpack_uint16_t(s[sidx:]);sidx += 2
-            self.status['debug'] = unpack_float_t(s[sidx:]); sidx += 4
-            self.status['cpu_temp']=self.get_cpu_temp()
-            return sidx
+        sidx=0
+        sidx +=self.imu.unpack_status((s[sidx:]))
+        self.status['voltage']=self.get_voltage(unpack_float_t(s[sidx:]));sidx+=4
+        self.status['current'] = self.get_current(unpack_float_t(s[sidx:]));sidx+=4
+        self.status['temp'] = self.get_temp(unpack_float_t(s[sidx:]));sidx+=4
+
+        for i in range(4):
+            self.status['cliff_range'][i]=unpack_float_t(s[sidx:])
+            sidx+=4
+
+        self.status['state'] = unpack_uint32_t(s[sidx:])
+        sidx += 4
+
+        self.status['at_cliff']=[]
+        self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_0) != 0)
+        self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_1) != 0)
+        self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_2) != 0)
+        self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_3) != 0)
+        self.status['runstop_event'] = (self.status['state'] & self.STATE_RUNSTOP_EVENT) != 0
+        self.status['cliff_event'] = (self.status['state'] & self.STATE_CLIFF_EVENT) != 0
+        self.status['fan_on'] = (self.status['state'] & self.STATE_FAN_ON) != 0
+        self.status['buzzer_on'] = (self.status['state'] & self.STATE_BUZZER_ON) != 0
+        self.status['low_voltage_alert'] = (self.status['state'] & self.STATE_LOW_VOLTAGE_ALERT) != 0
+        self.status['high_current_alert'] = (self.status['state'] & self.STATE_HIGH_CURRENT_ALERT) != 0
+        self.status['over_tilt_alert'] = (self.status['state'] & self.STATE_OVER_TILT_ALERT) != 0
+        self.status['charger_connected'] = (self.status['state'] & self.STATE_CHARGER_CONNECTED) != 0
+        self.status['boot_detected'] = (self.status['state'] & self.STATE_BOOT_DETECTED) != 0
+        self.status['timestamp'] = self.timestamp.set(unpack_uint32_t(s[sidx:])); sidx += 4
+        self.status['bump_event_cnt'] = unpack_uint16_t(s[sidx:]);sidx += 2
+        self.status['debug'] = unpack_float_t(s[sidx:]); sidx += 4
+        return sidx
 
 # ######################## PIMU PROTOCOL P1 #################################
 class Pimu_Protocol_P1(PimuBase):
-    def unpack_status(self,s):
-        with self.lock:
-            sidx=0
-            sidx +=self.imu.unpack_status((s[sidx:]))
-            self.status['voltage']=self.get_voltage(unpack_float_t(s[sidx:]));sidx+=4
-            self.status['current'] = self.get_current(unpack_float_t(s[sidx:]));sidx+=4
-            self.status['temp'] = self.get_temp(unpack_float_t(s[sidx:]));sidx+=4
-
-            for i in range(4):
-                self.status['cliff_range'][i]=unpack_float_t(s[sidx:])
-                sidx+=4
+    def unpack_status(self, s, unpack_to=None):
+        if unpack_to is None:
+            unpack_to = self.status
 
-            self.status['state'] = unpack_uint32_t(s[sidx:])
-            sidx += 4
+        sidx=0
+        sidx +=self.imu.unpack_status((s[sidx:]))
+        unpack_to['voltage']=self.get_voltage(unpack_float_t(s[sidx:]));sidx+=4
+        unpack_to['current'] = self.get_current(unpack_float_t(s[sidx:]));sidx+=4
+        unpack_to['temp'] = self.get_temp(unpack_float_t(s[sidx:]));sidx+=4
+
+        for i in range(4):
+            unpack_to['cliff_range'][i]=unpack_float_t(s[sidx:])
+            sidx+=4
+
+        unpack_to['state'] = unpack_uint32_t(s[sidx:])
+        sidx += 4
+        unpack_to['at_cliff']=[]
+        unpack_to['at_cliff'].append((unpack_to['state'] & PimuBase.STATE_AT_CLIFF_0) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_1) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_2) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_3) != 0)
+        unpack_to['runstop_event'] = (unpack_to['state'] & self.STATE_RUNSTOP_EVENT) != 0
+        unpack_to['cliff_event'] = (unpack_to['state'] & self.STATE_CLIFF_EVENT) != 0
+        unpack_to['fan_on'] = (unpack_to['state'] & self.STATE_FAN_ON) != 0
+        unpack_to['buzzer_on'] = (unpack_to['state'] & self.STATE_BUZZER_ON) != 0
+        unpack_to['low_voltage_alert'] = (unpack_to['state'] & self.STATE_LOW_VOLTAGE_ALERT) != 0
+        unpack_to['high_current_alert'] = (unpack_to['state'] & self.STATE_HIGH_CURRENT_ALERT) != 0
+        unpack_to['over_tilt_alert'] = (unpack_to['state'] & self.STATE_OVER_TILT_ALERT) != 0
+        if self.board_info['hardware_id']>0:
+            unpack_to['charger_connected'] = (unpack_to['state'] & self.STATE_CHARGER_CONNECTED) != 0
+            unpack_to['boot_detected'] = (unpack_to['state'] & self.STATE_BOOT_DETECTED) != 0
+        unpack_to['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:])); sidx += 8
+        self.imu.status['timestamp'] = unpack_to['timestamp']
+        unpack_to['bump_event_cnt'] = unpack_uint16_t(s[sidx:]);sidx += 2
+        unpack_to['debug'] = unpack_float_t(s[sidx:]); sidx += 4
+        return sidx
+
+
+
+
+
+
+# ######################## PIMU PROTOCOL P2 #################################
+class Pimu_Protocol_P2(PimuBase):
+
+    def read_firmware_trace(self):
+        self.trace_buf = []
+        self.timestamp.reset() #Timestamp holds state, reset within lock to avoid threading issues
+        self.n_trace_read=1
+        ts=time.time()
+        while ( self.n_trace_read) and time.time()-ts<60.0:
+            payload = arr.array('B', [self.RPC_READ_TRACE])
+            self.transport.do_pull_rpc_sync(payload, self.rpc_read_firmware_trace_reply)
+            time.sleep(.001)
+        return self.trace_buf
+
+    def unpack_debug_trace(self,s,unpack_to):
+        sidx=0
+        unpack_to['u8_1']=unpack_uint8_t(s[sidx:]);sidx+=1
+        unpack_to['u8_2'] = unpack_uint8_t(s[sidx:]);sidx += 1
+        unpack_to['f_1'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['f_2'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['f_3'] = unpack_float_t(s[sidx:]);sidx += 4
+        return sidx
+
+    def unpack_print_trace(self,s,unpack_to):
+        sidx=0
+        line_len=32
+        unpack_to['timestamp']=self.timestamp.set(unpack_uint64_t(s[sidx:]));sidx += 8
+        unpack_to['line'] = unpack_string_t(s[sidx:], line_len); sidx += line_len
+        unpack_to['x'] = unpack_float_t(s[sidx:]);sidx += 4
+        return sidx
+
+    def rpc_read_firmware_trace_reply(self, reply):
+        if len(reply)>0 and reply[0] == self.RPC_REPLY_READ_TRACE:
+            self.n_trace_read=reply[1]
+            self.trace_buf.append({'id': len(self.trace_buf), 'status': {},'debug':{},'print':{}})
+            if reply[2]==self.TRACE_TYPE_STATUS:
+                self.trace_buf[-1]['status']= self.status_zero.copy()
+                self.unpack_status(reply[3:],unpack_to=self.trace_buf[-1]['status'])
+            elif reply[2]==self.TRACE_TYPE_DEBUG:
+                self.unpack_debug_trace(reply[3:],unpack_to=self.trace_buf[-1]['debug'])
+            elif reply[2]==self.TRACE_TYPE_PRINT:
+                self.unpack_print_trace(reply[3:],unpack_to=self.trace_buf[-1]['print'])
+            else:
+                print('Unrecognized trace type %d'%reply[2])
+        else:
+            print('Error RPC_REPLY_READ_TRACE')
+            self.n_trace_read=0
+            self.trace_buf = []
+    def enable_firmware_trace(self):
+        self._trigger = self._trigger | self.TRIGGER_ENABLE_TRACE
+        self._dirty_trigger = True
+
+    def disable_firmware_trace(self):
+        self._trigger = self._trigger | self.TRIGGER_DISABLE_TRACE
+        self._dirty_trigger = True
+
+    def unpack_status(self, s, unpack_to=None):
+        if unpack_to is None:
+            unpack_to = self.status
+
+        sidx=0
+        sidx +=self.imu.unpack_status((s[sidx:]))
+        unpack_to['voltage']=self.get_voltage(unpack_float_t(s[sidx:]));sidx+=4
+        unpack_to['current'] = self.get_current(unpack_float_t(s[sidx:]));sidx+=4
+        unpack_to['temp'] = self.get_temp(unpack_float_t(s[sidx:]));sidx+=4
+
+        for i in range(4):
+            unpack_to['cliff_range'][i]=unpack_float_t(s[sidx:])
+            sidx+=4
+
+        unpack_to['state'] = unpack_uint32_t(s[sidx:])
+        sidx += 4
+
+        unpack_to['at_cliff']=[]
+        unpack_to['at_cliff'].append((unpack_to['state'] & PimuBase.STATE_AT_CLIFF_0) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_1) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_2) != 0)
+        unpack_to['at_cliff'].append((unpack_to['state'] & self.STATE_AT_CLIFF_3) != 0)
+        unpack_to['runstop_event'] = (unpack_to['state'] & self.STATE_RUNSTOP_EVENT) != 0
+        unpack_to['cliff_event'] = (unpack_to['state'] & self.STATE_CLIFF_EVENT) != 0
+        unpack_to['fan_on'] = (unpack_to['state'] & self.STATE_FAN_ON) != 0
+        unpack_to['buzzer_on'] = (unpack_to['state'] & self.STATE_BUZZER_ON) != 0
+        unpack_to['low_voltage_alert'] = (unpack_to['state'] & self.STATE_LOW_VOLTAGE_ALERT) != 0
+        unpack_to['high_current_alert'] = (unpack_to['state'] & self.STATE_HIGH_CURRENT_ALERT) != 0
+        unpack_to['over_tilt_alert'] = (unpack_to['state'] & self.STATE_OVER_TILT_ALERT) != 0
+        if self.board_info['hardware_id']>0:
+            unpack_to['charger_connected'] = (unpack_to['state'] & self.STATE_CHARGER_CONNECTED) != 0
+            unpack_to['boot_detected'] = (unpack_to['state'] & self.STATE_BOOT_DETECTED) != 0
+        unpack_to['trace_on'] = (unpack_to['state'] & self.STATE_IS_TRACE_ON) != 0
+        unpack_to['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:])); sidx += 8
+        self.imu.status['timestamp'] = unpack_to['timestamp']
+        unpack_to['bump_event_cnt'] = unpack_uint16_t(s[sidx:]);sidx += 2
+        unpack_to['debug'] = unpack_float_t(s[sidx:]); sidx += 4
+        return sidx
 
-            self.status['at_cliff']=[]
-            self.status['at_cliff'].append((self.status['state'] & PimuBase.STATE_AT_CLIFF_0) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_1) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_2) != 0)
-            self.status['at_cliff'].append((self.status['state'] & self.STATE_AT_CLIFF_3) != 0)
-            self.status['runstop_event'] = (self.status['state'] & self.STATE_RUNSTOP_EVENT) != 0
-            self.status['cliff_event'] = (self.status['state'] & self.STATE_CLIFF_EVENT) != 0
-            self.status['fan_on'] = (self.status['state'] & self.STATE_FAN_ON) != 0
-            self.status['buzzer_on'] = (self.status['state'] & self.STATE_BUZZER_ON) != 0
-            self.status['low_voltage_alert'] = (self.status['state'] & self.STATE_LOW_VOLTAGE_ALERT) != 0
-            self.status['high_current_alert'] = (self.status['state'] & self.STATE_HIGH_CURRENT_ALERT) != 0
-            self.status['over_tilt_alert'] = (self.status['state'] & self.STATE_OVER_TILT_ALERT) != 0
-            if self.board_info['hardware_id']>0:
-                self.status['charger_connected'] = (self.status['state'] & self.STATE_CHARGER_CONNECTED) != 0
-                self.status['boot_detected'] = (self.status['state'] & self.STATE_BOOT_DETECTED) != 0
-            self.status['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:])); sidx += 8
-            self.imu.status['timestamp'] = self.status['timestamp']
-            self.status['bump_event_cnt'] = unpack_uint16_t(s[sidx:]);sidx += 2
-            self.status['debug'] = unpack_float_t(s[sidx:]); sidx += 4
-            self.status['cpu_temp']=self.get_cpu_temp()
-            return sidx
+# ######################## PIMU PROTOCOL P2 #################################
+class Pimu_Protocol_P3(PimuBase):
 
+
+    def is_ready_for_sync(self):
+        """
+        With P3 this function is no longer meaningful as sync overruns are handled on the fw level
+        """
+        return True
+    def trigger_motor_sync(self):
+        # Push out immediately
+        if not self.hw_valid:
+            return
+        payload = arr.array('B', [self.RPC_SET_MOTOR_SYNC])
+        old_sync_cnt = self.status['motor_sync_cnt']
+        self.transport.do_push_rpc_sync(payload, self.rpc_motor_sync_reply)
+
+        t=time.time()
+        # Should motor_sync_cnt should increment with each call to trigger_motor_sync, if not it is an overrun
+        if self.status['motor_sync_cnt'] == old_sync_cnt:
+            self.status['motor_sync_queues']=self.status['motor_sync_queues']+1
+            print('Warning: Queued motor_sync as trigger_motor_sync calls above maximum rate. Overruns: %d' % (self.status['motor_sync_queues']))
+            self.ts_last_motor_sync_warn = t
+
+        if self.ts_last_motor_sync is not None:
+            self.status['motor_sync_rate']=1 / (t - self.ts_last_motor_sync)
+        self.ts_last_motor_sync = t
+
+    def rpc_motor_sync_reply(self,reply):
+        if reply[0] != self.RPC_REPLY_MOTOR_SYNC:
+            self.logger.warning('Error RPC_REPLY_MOTOR_SYNC', reply[0])
+        else:
+            self.unpack_motor_sync_reply(reply[1:])
+
+
+    def unpack_motor_sync_reply(self, s):
+        # take in an array of bytes
+        # this needs to exactly match the C struct format
+        sidx=0
+        self.status['motor_sync_cnt']=  unpack_int16_t(s[sidx:])
+        sidx += 2
+        return sidx
+
+    def pull_status_aux(self):
+        if not self.hw_valid:
+            return
+        payload = arr.array('B', [self.RPC_GET_PIMU_STATUS_AUX])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_status_aux_reply)
+
+
+    def rpc_status_aux_reply(self,reply):
+        if reply[0] == self.RPC_REPLY_PIMU_STATUS_AUX:
+            self.unpack_status_aux(reply[1:])
+        else:
+            self.logger.warning('Error RPC_REPLY_PIMU_AUX_STATUS', reply[0])
+
+    def unpack_status_aux(self, s):
+        # take in an array of bytes
+        # this needs to exactly match the C struct format
+        sidx=0
+        self.status_aux['foo']=  unpack_int16_t(s[sidx:]);sidx += 2
+        return sidx
+
+    def push_load_test(self):
+        if not self.hw_valid:
+            return
+        payload=self.transport.get_empty_payload()
+        payload[0] = self.RPC_LOAD_TEST_PUSH
+        payload[1:] = self.load_test_payload
+        self.transport.do_push_rpc_sync(payload, self.rpc_load_test_push_reply)
+
+    def pull_load_test(self):
+        if not self.hw_valid:
+            return
+        payload = arr.array('B',[self.RPC_LOAD_TEST_PULL])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_load_test_pull_reply)
+
+
+    def rpc_load_test_push_reply(self, reply):
+        if reply[0] != self.RPC_REPLY_LOAD_TEST_PUSH:
+            print('Error RPC_REPLY_LOAD_TEST_PUSH', reply[0])
+
+    def rpc_load_test_pull_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_LOAD_TEST_PULL:
+            d = reply[1:]
+            for i in range(1024):
+                if d[i] != self.load_test_payload[(i + 1) % 1024]:
+                    print('Load test pull bad data', d[i], self.load_test_payload[(i + 1) % 1024])
+            self.load_test_payload = d
+            print('Successful load test pull')
+        else:
+            print('Error RPC_REPLY_LOAD_TEST_PULL', reply[0])
 # ######################## PIMU #################################
 class Pimu(PimuBase):
     """
     API to the Stretch Power and IMU board (Pimu)
     """
-    def __init__(self, event_reset=False):
-        PimuBase.__init__(self, event_reset)
+    def __init__(self, event_reset=False, usb=None):
+        PimuBase.__init__(self, event_reset,usb)
         # Order in descending order so more recent protocols/methods override less recent
-        self.supported_protocols = {'p0': (Pimu_Protocol_P0,), 'p1': (Pimu_Protocol_P1,Pimu_Protocol_P0,)}
+        self.supported_protocols = {'p0': (Pimu_Protocol_P0,), 'p1': (Pimu_Protocol_P1, Pimu_Protocol_P0,),
+                                    'p2': (Pimu_Protocol_P2, Pimu_Protocol_P1, Pimu_Protocol_P0,),
+                                    'p3': (Pimu_Protocol_P3, Pimu_Protocol_P2, Pimu_Protocol_P1, Pimu_Protocol_P0,)}
 
     def startup(self, threaded=False):
         """
         First determine which protocol version the uC firmware is running.
         Based on that version, replaces PimuBase class inheritance with a inheritance to a child class of PimuBase that supports that protocol
         """
         PimuBase.startup(self, threaded=threaded)
         if self.hw_valid:
             if self.board_info['protocol_version'] in self.supported_protocols:
                 Pimu.__bases__ = self.supported_protocols[self.board_info['protocol_version']]
                 IMU.__bases__= self.imu.supported_protocols[self.board_info['protocol_version']]
             else:
-                protocol_msg = """
-                ----------------
-                Firmware protocol mismatch on {0}.
-                Protocol on board is {1}.
-                Valid protocols are: {2}.
-                Disabling device.
-                Please upgrade the firmware and/or version of Stretch Body.
-                ----------------
-                """.format(self.name, self.board_info['protocol_version'], self.supported_protocols.keys())
+                if self.board_info['protocol_version'] is None:
+                    protocol_msg = """
+                                    ----------------
+                                    Failure in communications for {0} on startup.
+                                    Please power cycle the robot and try again.
+                                    ----------------
+                                    """.format(self.name)
+                else:
+                    protocol_msg = """
+                    ----------------
+                    Firmware protocol mismatch on {0}.
+                    Protocol on board is {1}.
+                    Valid protocols are: {2}.
+                    Disabling device.
+                    Please upgrade the firmware and/or version of Stretch Body.
+                    ----------------
+                    """.format(self.name, self.board_info['protocol_version'], self.supported_protocols.keys())
                 self.logger.warning(textwrap.dedent(protocol_msg))
                 self.hw_valid = False
                 self.transport.stop()
         if self.hw_valid:
             self.push_command()
             self.pull_status()
         return self.hw_valid
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/prismatic_joint.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/prismatic_joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,58 +7,76 @@
 import sys
 
 
 class PrismaticJoint(Device):
     """
     API to the Stretch Prismatic Joints
     """
-    def __init__(self,name):
+    def __init__(self,name,usb=None):
         Device.__init__(self,name )
-        self.motor = Stepper(usb='/dev/hello-motor-'+name)
+        if usb is None:
+            usb=self.params['usb_name']
+        motor_name = None
+        if name == 'lift':
+            motor_name = 'hello-motor-lift'
+        elif name == 'arm':
+            motor_name = 'hello-motor-arm'
+        self.motor = Stepper(usb=usb, name=motor_name)
         self.status = {'timestamp_pc':0,'pos': 0.0, 'vel': 0.0, 'force':0.0,'motor': self.motor.status}
         self.trajectory = PrismaticTrajectory()
         self.thread_rate_hz = 5.0
 
         # Default controller params
         self.stiffness = 1.0
         self.i_feedforward=self.params['i_feedforward']
         self.vel_r = self.translate_m_to_motor_rad(self.params['motion']['default']['vel_m'])
         self.accel_r = self.translate_m_to_motor_rad(self.params['motion']['default']['accel_m'])
         self.soft_motion_limits = {'collision': [None, None], 'user': [None, None],
                                    'hard': [self.params['range_m'][0], self.params['range_m'][1]],
                                    'current': [self.params['range_m'][0], self.params['range_m'][1]]}
-        self.motor.set_motion_limits(self.translate_m_to_motor_rad(self.soft_motion_limits['current'][0]),
-                                     self.translate_m_to_motor_rad(self.soft_motion_limits['current'][1]))
+
 
     # ###########  Device Methods #############
     def startup(self, threaded=True):
-        Device.startup(self, threaded=threaded)
-        success= self.motor.startup(threaded=False)
-        self.__update_status()
+        # Startup stepper first so that status is populated before this Device thread begins (if threaded==true)
+        success = self.motor.startup(threaded=False)
+        if success:
+            Device.startup(self, threaded=threaded)
+            self.__update_status()
+            self.motor.set_motion_limits(self.translate_m_to_motor_rad(self.soft_motion_limits['current'][0]),
+                                         self.translate_m_to_motor_rad(self.soft_motion_limits['current'][1]))
         return success
 
     def stop(self):
         Device.stop(self)
         if self.motor.hw_valid and int(str(self.motor.board_info['protocol_version'])[1:]) >= 1:
             self.motor.stop_waypoint_trajectory()
         self.motor.stop()
 
     def pull_status(self):
         self.motor.pull_status()
         self.__update_status()
 
+    async def pull_status_async(self):
+        await self.motor.pull_status_async()
+        self.__update_status()
+
     def __update_status(self):
         self.status['timestamp_pc'] = time.time()
         self.status['pos'] = self.motor_rad_to_translate_m(self.status['motor']['pos'])
         self.status['vel'] = self.motor_rad_to_translate_m(self.status['motor']['vel'])
         self.status['force'] =  0 #Deprecated
 
     def push_command(self):
         self.motor.push_command()
 
+
+    async def push_command_async(self):
+        await self.motor.push_command_async()
+
     def _thread_loop(self):
         self.pull_status()
         self.update_trajectory()
 
     def pretty_print(self):
         print('----- %s ------ '%self.name.capitalize())
         print('Pos (m): ', self.status['pos'])
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_collision.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_collision.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         self.robot.arm.set_soft_motion_limit_min(x=target_limits['arm'][0], limit_type='collision')
         self.robot.arm.set_soft_motion_limit_max(x=target_limits['arm'][1], limit_type='collision')
         self.robot.head.motors['head_tilt'].set_soft_motion_limit_min(x=target_limits['head_tilt'][0], limit_type='collision')
         self.robot.head.motors['head_tilt'].set_soft_motion_limit_max(x=target_limits['head_tilt'][1], limit_type='collision')
         self.robot.head.motors['head_pan'].set_soft_motion_limit_min(x=target_limits['head_pan'][0],limit_type='collision')
         self.robot.head.motors['head_pan'].set_soft_motion_limit_max(x=target_limits['head_pan'][1],limit_type='collision')
         for j in self.robot.end_of_arm.joints:
-            self.robot.end_of_arm.motors[j].set_soft_motion_limit_min(x=target_limits['head_pan'][0],limit_type='collision')
-            self.robot.end_of_arm.motors[j].set_soft_motion_limit_max(x=target_limits['head_pan'][1],limit_type='collision')
+            self.robot.end_of_arm.motors[j].set_soft_motion_limit_min(x=target_limits[j][0],limit_type='collision')
+            self.robot.end_of_arm.motors[j].set_soft_motion_limit_max(x=target_limits[j][1],limit_type='collision')
 
 
 # #######################################################################
 """
 Helper Classes: Example for EndOfArmForwardKinematics
             cfg = {
                 'joint_lift': status['lift']['pos'],
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_collision_models.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_collision_models.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_monitor.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,49 +56,49 @@
             self.monitor_over_tilt_alert()
 
 
     # ##################################
     def monitor_base_cliff_event(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['cliff_event'] and  self.monitor_history['monitor_base_cliff_event']==0:
-                self.logger.debug("Base cliff event")
+                self.logger.info("Base cliff event")
             self.monitor_history['monitor_base_cliff_event'] = self.robot.pimu.status['cliff_event']
 
     # ##################################
     def monitor_base_bump_event(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['bump_event_cnt'] != self.monitor_history['monitor_base_bump_event']:
-                self.logger.debug("Base bump event")
+                self.logger.info("Base bump event")
             self.monitor_history['monitor_base_bump_event'] = self.robot.pimu.status['bump_event_cnt']
 
     # ##################################
     def monitor_over_tilt_alert(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['over_tilt_alert'] and self.monitor_history['monitor_over_tilt_alert'] == 0:
-                self.logger.debug("Over Tilt Alert")
+                self.logger.info("Over Tilt Alert")
             self.monitor_history['monitor_over_tilt_alert'] = self.robot.pimu.status['over_tilt_alert']
 
     # ##################################
     def monitor_wrist_single_tap(self):
         if self.robot.wacc is not None:
             if self.robot.wacc.status['single_tap_count']!=self.monitor_history['monitor_wrist_single_tap']:
-                self.logger.debug("Wrist single tap: %d" % self.robot.wacc.status['single_tap_count'])
+                self.logger.info("Wrist single tap: %d" % self.robot.wacc.status['single_tap_count'])
             self.monitor_history['monitor_wrist_single_tap']=self.robot.wacc.status['single_tap_count']
 
     # ##################################
     def monitor_guarded_contact(self):
         joints=[self.robot.lift, self.robot.arm]
         mn='monitor_guarded_contact'
         for j in joints:
             if j is not None:
                 if j.name not in self.monitor_history[mn]:# Init history
                     self.monitor_history[mn][j.name] = 0
                 if j is not None:
                     if self.monitor_history[mn][j.name]==0 and j.motor.status['in_guarded_event']:
-                        self.logger.debug("Guarded contact %s"%j.name)
+                        self.logger.info("Guarded contact %s"%j.name)
                 self.monitor_history[mn][j.name] =j.motor.status['in_guarded_event']
 
     # ##################################
     def monitor_dynamixel_flags(self):
         chains=[self.robot.head,self.robot.end_of_arm]
         mn='monitor_dynamixel_flags'
         errs = ['overheating_error', 'overload_error']
@@ -111,38 +111,38 @@
                         self.monitor_history[mn][c.name][k] = {}
                         for e in errs:
                             self.monitor_history[mn][c.name][k][e]=0
                 #Flag changes from 0 to 1 on error
                 for k in c.motors.keys():
                     for e in errs:
                         if c.motors[k].status[e] and not self.monitor_history[mn][c.name][k][e]:
-                            self.logger.debug("Dynamixel %s on %s:%s"%(e,c.name,k))
+                            self.logger.warn("Dynamixel %s on %s:%s"%(e,c.name,k))
                         self.monitor_history[mn][c.name][k][e] = c.motors[k].status[e]
 
     # ##################################
     def monitor_runstop(self):
         if self.robot.status['pimu']['runstop_event'] != self.monitor_history['monitor_runstop']:
             if self.robot.status['pimu']['runstop_event']:
-                self.logger.debug("Runstop activated")
+                self.logger.info("Runstop activated")
             else:
-                self.logger.debug("Runstop deactivated")
+                self.logger.info("Runstop deactivated")
         self.monitor_history['monitor_runstop']=self.robot.status['pimu']['runstop_event']
 
     # ##################################
     def monitor_voltage(self):
         v=self.robot.pimu.status['voltage']
         if v < self.robot.pimu.config['low_voltage_alert']:
             if v-self.monitor_history['monitor_voltage']<-0.5:#every 0.5V of drop allow to report
-                self.logger.debug('Low voltage of: %.2f'%v)
+                self.logger.info('Low voltage of: %.2f'%v)
                 self.monitor_history['monitor_voltage']=v
         else:
             self.monitor_history['monitor_voltage'] =v
 
     # ##################################
     def monitor_current(self):
         i=self.robot.pimu.status['current']
         if i > self.robot.pimu.config['high_current_alert']:
             if i-self.monitor_history['monitor_current']>0.25:#every 0.25A of rise allow to report
-                self.logger.debug('High current of: %.2f'%i)
+                self.logger.info('High current of: %.2f'%i)
                 self.monitor_history['monitor_current']=i
         else:
             self.monitor_history['monitor_current'] =i
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_params.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     "level": "INFO",
                     "formatter": "default_console_formatter",
                 },
                 "file_handler": {
                     "class": "logging.FileHandler",
                     "level": "DEBUG",
                     "formatter": "default_file_formatter",
-                    "filename": hello_utils.get_stretch_directory('log/') + 'stretchbody_{0}.log'.format(
+                    "filename": hello_utils.get_stretch_directory('log/stretch_body_logger/') + 'stretchbody_{0}.log'.format(
                         hello_utils.create_time_string())
                 }
             },
             "formatters": {
                 "default_console_formatter": {
                     "format": "[%(levelname)s] [%(name)s]: %(message)s"
                 },
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE1V0.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params_RE1V0.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,21 @@
         'zero_t': 7175,
         'baud':115200}}
 
 # ###################### NOMINAL PARAMS #####################################################
 #Parameters that are common across the RE1.0 fleet
 nominal_params={
     'arm':{
+        'usb_name': '/dev/hello-motor-arm',
         'chain_pitch': 0.0167,
         'chain_sprocket_teeth': 10,
         'gr_spur': 3.875,
         'i_feedforward': 0,
         'force_N_per_A': 55.9, #Legacy
-        'calibration_range_bounds': [0.515, 0.525],
+        'calibration_range_bounds': [0.514, 0.525],
         'contact_models':{
             'effort_pct': {'contact_thresh_calibration_margin':10.0,'contact_thresh_max': [-90.0, 90.0]}},
         'motion':{
             'default':{
                 'accel_m': 0.14,
                 'vel_m': 0.14},
             'fast':{
@@ -96,14 +97,16 @@
             'slow':{
                 'accel_m': 0.07,
                 'vel_m': 0.06},
             'trajectory_max': {
                 'vel_m': 0.3,
                 'accel_m': 0.5}}},
     'base':{
+        'usb_name_left_wheel': '/dev/hello-motor-left-wheel',
+        'usb_name_right_wheel': '/dev/hello-motor-right-wheel',
         'force_N_per_A': 21.18, #Legacy
         'gr': 3.4,
         'motion':{
             'default':{
                 'accel_m': 0.2,
                 'vel_m': 0.15},
             'fast':{
@@ -140,23 +143,25 @@
         'py_class_name': 'CollisionStretchGripper',
         'py_module_name': 'stretch_body.robot_collision_models'},
     'dxl_comm_errors': {
         'warn_every_s': 1.0,
         'warn_above_rate': 0.1,
         'verbose': 0},
     'end_of_arm':{
+        'usb_name': '/dev/hello-dynamixel-wrist',
         'devices':{
             'wrist_yaw':{
               'py_class_name': 'WristYaw',
               'py_module_name': 'stretch_body.wrist_yaw'}},
         'use_group_sync_read': 1,
         'retry_on_comm_failure': 1,
         'dxl_latency_timer': 64,
         'stow': {'wrist_yaw': 3.4}},
     'head':{
+        'usb_name': '/dev/hello-dynamixel-head',
         'use_group_sync_read': 1,
         'retry_on_comm_failure': 1,
         'dxl_latency_timer':64},
     'head_pan':{
         'range_pad_t': [50.0, -50.0],
         'flip_encoder_polarity': 1,
         'gr': 1.0,
@@ -239,14 +244,15 @@
         'stall_min_vel': 0.1},
     'hello-motor-arm':{
         'gains':{
             'effort_LPF': 10.0,
             'enable_guarded_mode': 1,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':0,
             'flip_effort_polarity': 0,
             'flip_encoder_polarity': 0,
             'iMax_neg': -3.2,
             'iMax_pos': 3.2,
             'i_contact_neg': -3.2,
             'i_contact_pos': 3.2,
             'i_safety_feedforward': 0.0,
@@ -274,14 +280,15 @@
         'rated_current': 2.8},
     'hello-motor-left-wheel':{
         'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 0,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':1,
             'flip_effort_polarity': 1,
             'flip_encoder_polarity': 1,
             'iMax_neg': -2.8,
             'iMax_pos': 2.8,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
@@ -309,14 +316,15 @@
         'rated_current': 2.8},
     'hello-motor-lift':{
             'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 1,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':0,
             'flip_effort_polarity': 1,
             'flip_encoder_polarity': 1,
             'iMax_neg': -3.2,
             'iMax_pos': 3.2,
             'i_contact_neg': -1.5,
             'i_contact_pos': 2.0,
             'i_safety_feedforward': 0.4,
@@ -344,14 +352,15 @@
         'rated_current': 2.8},
     'hello-motor-right-wheel':{
         'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 0,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':1,
             'flip_effort_polarity': 0,
             'flip_encoder_polarity': 0,
             'iMax_neg': -2.8,
             'iMax_pos': 2.8,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
@@ -374,14 +383,15 @@
             'vel_status_LPF': 10.0},
         'holding_torque': 1.26,
         'motion':{
             'accel': 15,
             'vel': 25},
         'rated_current': 2.8},
     'lift':{
+        'usb_name': '/dev/hello-motor-lift',
         'belt_pitch_m': 0.005,
         'contact_models': {
             'effort_pct': {
                 'contact_thresh_calibration_margin': 10.0,
                 'contact_thresh_max': [-100, 100]}},
         'calibration_range_bounds': [1.094, 1.106],
         'force_N_per_A': 75.0, #Legacy
@@ -399,17 +409,18 @@
                 'accel_m': 0.05,
                 'vel_m': 0.05},
             'trajectory_max': {
                 'vel_m': 0.2,
                 'accel_m': 0.3}},
         'pinion_t': 12},
     'pimu':{
+      'usb_name': '/dev/hello-pimu',
       'base_fan_off': 70,
       'base_fan_on': 82,
-      'max_sync_rate_hz':20.0,
+      'max_sync_rate_hz':20.0, #deprecated with P3
       'config':{
         'accel_LPF': 20.0,
         'bump_thresh': 20.0,
         'cliff_LPF': 10.0,
         'cliff_thresh': -50,
         'current_LPF': 10.0,
         'high_current_alert': 7.0,
@@ -422,42 +433,50 @@
         'stop_at_tilt': 0,
         'temp_LPF': 1.0,
         'voltage_LPF': 1.0}},
     'robot':{
         'rates':{
             'DXLStatusThread_Hz': 15.0,
             'NonDXLStatusThread_Hz': 25.0,
-            'NonDXLStatusThread_monitor_downrate_int': 5,
-            'NonDXLStatusThread_collision_downrate_int': 5,
-            'NonDXLStatusThread_sentry_downrate_int': 2,
-            'NonDXLStatusThread_trajectory_downrate_int': 2},
+            'SystemMonitorThread_Hz': 15.0,
+            'SystemMonitorThread_monitor_downrate_int': 2,
+            'SystemMonitorThread_trace_downrate_int': 1,
+            'SystemMonitorThread_collision_downrate_int': 5,
+            'SystemMonitorThread_sentry_downrate_int': 1,
+            'SystemMonitorThread_nondxl_trajectory_downrate_int': 2},
         'tool': 'tool_stretch_gripper',
-        'use_collision_manager': 1,
+        'use_collision_manager': 0,
         'stow':{
         'arm': 0.0,
         'head_pan': 0.0,
         'head_tilt': 0.0,
         'lift': 0.2,
         'stretch_gripper': 0,
         'wrist_yaw': 3.4},
         'use_monitor': 1,
-        'use_sentry': 1},
+        'use_trace': 0,
+        'use_sentry': 1,
+        'use_asyncio':1},
     'robot_collision': {
         'models': ['collision_arm_camera']
     },
     'robot_monitor':{
         'monitor_base_bump_event': 1,
         'monitor_base_cliff_event': 1,
         'monitor_current': 1,
         'monitor_dynamixel_flags': 1,
         'monitor_guarded_contact': 1,
         'monitor_over_tilt_alert': 1,
         'monitor_runstop': 1,
         'monitor_voltage': 1,
         'monitor_wrist_single_tap': 1},
+    'robot_trace':{
+        'n_samples_per_file':100,
+        'duration_limit_minutes':10.0
+    },
     'robot_sentry':{
         'base_fan_control': 1,
         'base_max_velocity': 1,
         'dynamixel_stop_on_runstop': 1,
         'stretch_gripper_overload': 1,
         'wrist_yaw_overload': 1,
         'stepper_is_moving_filter': 1},
@@ -528,14 +547,15 @@
             'wrist_yaw': {
                 'py_class_name': 'WristYaw',
                 'py_module_name': 'stretch_body.wrist_yaw'
             }
         },
         'collision_models': ['collision_stretch_gripper']},
     'wacc':{
+        'usb_name': '/dev/hello-wacc',
         'config': {
         'accel_LPF': 10.0,
         'accel_range_g': 4,
         'accel_single_tap_dur': 70,
         'accel_single_tap_thresh': 50,
         'ana_LPF': 10.0}},
     'wrist_yaw':{
@@ -573,15 +593,17 @@
         'stall_max_time': 1.0,
         'stall_min_vel': 0.1,
         'temperature_limit': 72,
         'usb_name': '/dev/hello-dynamixel-wrist',
         'use_multiturn': 1,
         'retry_on_comm_failure': 1,
         'enable_runstop': 1,
-        'disable_torque_on_stop': 1}
+        'disable_torque_on_stop': 1},
+    'respeaker': {'usb_name': '/dev/hello-respeaker'},
+    'lidar': {'usb_name': '/dev/hello-lrf'}
 }
 # ###################### OLDER: FACTORY PARAMS #####################################################
 #The deprecated factory params dictionary for RE1.0 (5.1.2022)
 # Kept here for migration / records
 
 factory_params_deprecated = {
     "dxl_comm_errors":{
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE2V0.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/robot_params_RE2V0.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # ######################### USER PARAMS ##################################################
 #Template for the generated file: stretch_user_params.yaml
 user_params_header='#User parameters\n' \
                    '#You can override nominal settings here\n' \
                    '#USE WITH CAUTION. IT IS POSSIBLE TO CAUSE UNSAFE BEHAVIOR OF THE ROBOT \n'
 
 user_params_template={
-    'robot': {'use_collision_manager': 1}} #Include this just as an example
+    'robot': {'use_collision_manager': 0}} #Include this just as an example
 
 # ###################### CONFIGURATION PARAMS #####################################################
 #Template for the generated file: stretch_configuration_params.yaml
 #Configuration parameters may have variation across the fleet of RE2 robots
 configuration_params_header='#Parameters that are specific to this robot\n' \
                             '#Do not edit, instead edit stretch_user_params.yaml\n'
 
@@ -34,15 +34,15 @@
     'head_pan':{
         'range_t': [0, 3827],
         'zero_t': 1250},
     'head_tilt':{
         'range_t': [1775,3150],
         'zero_t': 2048},
     'hello-motor-arm':{'serial_no': 'NA'},
-    'hello-motor-lift':{'serial_no': 'NA'},
+    'hello-motor-lift':{'serial_no': 'NA','gains':{'i_safety_feedforward':1.2}},
     'hello-motor-left-wheel':{'serial_no': 'NA'},
     'hello-motor-right-wheel':{'serial_no': 'NA'},
     'pimu':{
         'config':{
             'cliff_zero': [0.0, 0.0, 0.0, 0.0],
             'gyro_zero_offsets': [0.0, 0.0, 0.0],
             'gravity_vector_scale': 1.0,
@@ -57,26 +57,27 @@
     'stretch_gripper':{
         'range_t': [0, 8022],
         'zero_t': 5212},
     'wacc':{'config':{
         'accel_gravity_scale': 1.0}},
     'wrist_yaw':{
         'range_t': [0,9340],
-        'zero_t': 7175}}
+        'zero_t': 7005}}
 
 # ###################### NOMINAL PARAMS #####################################################
 #Parameters that are common across the RE2 fleet
 nominal_params={
     'arm':{
+        'usb_name': '/dev/hello-motor-arm',
         'force_N_per_A': 55.9,  # Legacy
         'chain_pitch': 0.0167,
         'chain_sprocket_teeth': 10,
         'gr_spur': 3.875,
         'i_feedforward': 0,
-        'calibration_range_bounds':[0.515, 0.525],
+        'calibration_range_bounds':[0.514, 0.525],
         'contact_models':{
             'effort_pct': {'contact_thresh_calibration_margin':10.0,'contact_thresh_max': [-90.0, 90.0]}},
         'motion':{
             'default':{
                 'accel_m': 0.14,
                 'vel_m': 0.14},
             'fast':{
@@ -88,14 +89,16 @@
             'slow':{
                 'accel_m': 0.05,
                 'vel_m': 0.05},
             'trajectory_max': {
                 'vel_m': 0.4,
                 'accel_m': 0.4}}},
     'base':{
+        'usb_name_left_wheel': '/dev/hello-motor-left-wheel',
+        'usb_name_right_wheel': '/dev/hello-motor-right-wheel',
         'force_N_per_A': 21.18,  # Legacy
         'gr': 3.8,
         'motion':{
             'default':{
                 'accel_m': 0.12,
                 'vel_m': 0.12},
             'fast':{
@@ -132,24 +135,26 @@
         'py_class_name': 'CollisionStretchGripper',
         'py_module_name': 'stretch_body.robot_collision_models'},
     'dxl_comm_errors': {
         'warn_every_s': 1.0,
         'warn_above_rate': 0.1,
         'verbose': 0},
     'end_of_arm':{
+        'usb_name': '/dev/hello-dynamixel-wrist',
         'devices':{
             'wrist_yaw':{
               'py_class_name': 'WristYaw',
               'py_module_name': 'stretch_body.wrist_yaw'}},
         'use_group_sync_read': 1,
         'retry_on_comm_failure': 1,
         'baud': 115200,
         'dxl_latency_timer': 64,
         'stow': {'wrist_yaw': 3.4}},
     'head':{
+        'usb_name': '/dev/hello-dynamixel-head',
         'use_group_sync_read': 1,
         'retry_on_comm_failure': 1,
         'dxl_latency_timer':64,
         'baud': 115200},
     'head_pan':{
         'flip_encoder_polarity': 1,
         'gr': 1.0,
@@ -236,14 +241,15 @@
         'range_pad_t': [50.0, -50.0]},
     'hello-motor-arm':{
         'gains':{
             'effort_LPF': 10.0,
             'enable_guarded_mode': 1,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':0,
             'flip_effort_polarity': 0,
             'flip_encoder_polarity': 0,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -2.0,
             'i_contact_pos': 2.0,
             'i_safety_feedforward': 0.0,
@@ -271,14 +277,15 @@
         'rated_current': 2.8},
     'hello-motor-left-wheel':{
         'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 0,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':1,
             'flip_effort_polarity': 1,
             'flip_encoder_polarity': 1,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
@@ -306,14 +313,15 @@
         'rated_current': 2.8},
     'hello-motor-lift':{
             'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 1,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':0,
             'flip_effort_polarity': 1,
             'flip_encoder_polarity': 1,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 1.2,
@@ -341,14 +349,15 @@
         'rated_current': 2.8},
     'hello-motor-right-wheel':{
         'gains':{
             'effort_LPF': 2.0,
             'enable_guarded_mode': 0,
             'enable_runstop': 1,
             'enable_sync_mode': 1,
+            'enable_vel_watchdog':1,
             'flip_effort_polarity': 0,
             'flip_encoder_polarity': 0,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
@@ -371,14 +380,15 @@
             'vel_status_LPF': 10.0},
         'holding_torque': 1.26,
         'motion':{
             'accel': 15,
             'vel': 25},
         'rated_current': 2.8},
     'lift':{
+        'usb_name': '/dev/hello-motor-lift',
         'force_N_per_A': 75.0,  # Legacy
         'calibration_range_bounds': [1.094, 1.106],
         'contact_models': {
             'effort_pct':{
                 'contact_thresh_calibration_margin': 10.0,
                 'contact_thresh_max': [-100, 100]}},
         'belt_pitch_m': 0.005,
@@ -396,17 +406,18 @@
               'accel_m': 0.05,
               'vel_m': 0.05},
             'trajectory_max': {
               'accel_m': 0.3,
               'vel_m': 0.15}},
           'pinion_t': 12},
     'pimu':{
+      'usb_name': '/dev/hello-pimu',
       'base_fan_off': 70,
       'base_fan_on': 82,
-      'max_sync_rate_hz': 80.0,
+      'max_sync_rate_hz': 80.0, #deprecated with P3
       'config':{
         'accel_LPF': 20.0,
         'bump_thresh': 20.0,
         'cliff_LPF': 10.0,
         'cliff_thresh': -50,
         'current_LPF': 10.0,
         'high_current_alert': 7.0,
@@ -419,29 +430,33 @@
         'stop_at_tilt': 0,
         'temp_LPF': 1.0,
         'voltage_LPF': 1.0}},
     'robot':{
         'rates':{
             'DXLStatusThread_Hz': 15.0,
             'NonDXLStatusThread_Hz': 25.0,
-            'NonDXLStatusThread_monitor_downrate_int': 5,
-            'NonDXLStatusThread_collision_downrate_int': 5,
-            'NonDXLStatusThread_sentry_downrate_int': 2,
-            'NonDXLStatusThread_trajectory_downrate_int': 2},
+            'SystemMonitorThread_Hz': 15.0,
+            'SystemMonitorThread_monitor_downrate_int': 2,
+            'SystemMonitorThread_trace_downrate_int': 1,
+            'SystemMonitorThread_collision_downrate_int': 5,
+            'SystemMonitorThread_sentry_downrate_int': 1,
+            'SystemMonitorThread_nondxl_trajectory_downrate_int': 2},
         'tool': 'tool_stretch_gripper',
-        'use_collision_manager': 1,
+        'use_collision_manager': 0,
         'stow':{
         'arm': 0.0,
         'head_pan': 0.0,
         'head_tilt': 0.0,
         'lift': 0.23,
         'stretch_gripper': 0,
         'wrist_yaw': 3.4},
         'use_monitor': 1,
-        'use_sentry': 1},
+        'use_trace': 0,
+        'use_sentry': 1,
+        'use_asyncio':1},
     'robot_collision': {
         'models': ['collision_arm_camera']
     },
     'robot_monitor':{
         'monitor_base_bump_event': 1,
         'monitor_base_cliff_event': 1,
         'monitor_current': 1,
@@ -454,14 +469,18 @@
     'robot_sentry':{
         'base_fan_control': 1,
         'base_max_velocity': 1,
         'dynamixel_stop_on_runstop': 1,
         'stretch_gripper_overload': 1,
         'wrist_yaw_overload': 1,
         'stepper_is_moving_filter': 1},
+    'robot_trace':{
+        'n_samples_per_file':100,
+        'duration_limit_minutes':10.0
+    },
     'stretch_gripper':{
         'range_pad_t': [100.0, -100.0],
         'flip_encoder_polarity': 0,
         'gr': 1.0,
         'id': 14,
         'max_voltage_limit': 15,
         'min_grip_strength': -125,
@@ -528,14 +547,15 @@
             'wrist_yaw': {
                 'py_class_name': 'WristYaw',
                 'py_module_name': 'stretch_body.wrist_yaw'
             }
         },
         'collision_models': ['collision_stretch_gripper']},
     'wacc':{
+        'usb_name': '/dev/hello-wacc',
         'config': {
         'accel_LPF': 10.0,
         'accel_range_g': 4,
         'accel_single_tap_dur': 70,
         'accel_single_tap_thresh': 50,
         'ana_LPF': 10.0}},
     'wrist_yaw':{
@@ -574,9 +594,11 @@
         'temperature_limit': 72,
         'usb_name': '/dev/hello-dynamixel-wrist',
         'use_multiturn': 1,
         'retry_on_comm_failure': 1,
         'baud': 115200,
         'enable_runstop': 1,
         'disable_torque_on_stop': 1,
-        'range_pad_t': [50.0, -50.0]}
+        'range_pad_t': [100.0, -100.0]},
+    'respeaker': {'usb_name': '/dev/hello-respeaker'},
+    'lidar': {'usb_name': '/dev/hello-lrf'}
 }
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/scope.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/scope.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     Simple oscilloscope visualization of a data stream
     """
     def __init__(self,num_points=100,yrange=None,title='Scope'):
         plt.ion()  # enable interactivity
         self.y = None
         self.num_points=num_points
         self.fig = plt.figure()
-        self.fig.canvas.set_window_title(title)
+        # set window title
+        if self.fig.canvas.manager is not None:
+            self.fig.canvas.manager.set_window_title(title)
+        # self.fig.canvas.set_window_title(title)
         self.yrange=yrange
     def step_display(self,new_val):
         if self.y is None:
             self.y=[new_val] * self.num_points
         self.y.append(new_val)
         self.y=self.y[1:]
         drawnow(self.make_fig)
@@ -94,15 +97,20 @@
         self.epsilon = 15
         self.pind = None
 
         # Setup plot and widgets
         widget_loc = lambda x: plt.axes([0.84, 0.8-((x)*0.05), 0.12, 0.02])
         self.fig, self.axes = plt.subplots(1, 1, figsize=(9.0, 8.0), sharex=True)
         self.fig.subplots_adjust(right=0.8)
-        self.fig.canvas.set_window_title(title)
+
+        # set window title
+        if self.fig.canvas.manager is not None:
+            self.fig.canvas.manager.set_window_title(title)
+        #self.fig.canvas.set_window_title(title)
+
         self.axes.set_yscale('linear')
         self.axes.set_ylim(min(self.yrange) - 0.75, max(self.yrange) + 0.75)
         self.axes.axhspan(min(self.yrange) - 2 ** 32, min(self.yrange), facecolor='0.2', alpha=0.5)
         self.axes.axhspan(max(self.yrange), max(self.yrange) + 2 ** 32, facecolor='0.2', alpha=0.5)
         self.axes.set_xlabel(xlabel)
         self.axes.set_ylabel(ylabel)
         self.axes.grid(True)
@@ -257,15 +265,18 @@
         plt.ion()  # enable interactivity
         self.y1 = None
         self.y2 = None
         self.y3 = None
         self.y4 = None
         self.num_points=num_points
         self.fig = plt.figure()
-        self.fig.canvas.set_window_title(title)
+        # set window title
+        if self.fig.canvas.manager is not None:
+            self.fig.canvas.manager.set_window_title(title)
+        # self.fig.canvas.set_window_title(title)
         self.yrange=yrange
     def savefig(self,filename):
         plt.savefig(filename)
     def step_display(self,y1,y2,y3,y4):
         if self.y1 is None:
             self.y1=[y1] * self.num_points
         if self.y2 is None:
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/stepper.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/stepper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from stretch_body.transport import *
 from stretch_body.device import Device
 from stretch_body.hello_utils import *
 import textwrap
 import threading
 import sys
 import time
+import array as arr
 
 
 
 # ######################## STEPPER #################################
 
 class StepperBase(Device):
     """
@@ -17,16 +18,16 @@
     """
     RPC_SET_COMMAND = 1
     RPC_REPLY_COMMAND = 2
     RPC_GET_STATUS = 3
     RPC_REPLY_STATUS = 4
     RPC_SET_GAINS = 5
     RPC_REPLY_GAINS = 6
-    RPC_LOAD_TEST = 7
-    RPC_REPLY_LOAD_TEST = 8
+    RPC_LOAD_TEST_PUSH = 7
+    RPC_REPLY_LOAD_TEST_PUSH = 8
     RPC_SET_TRIGGER = 9
     RPC_REPLY_SET_TRIGGER = 10
     RPC_SET_ENC_CALIB = 11
     RPC_REPLY_ENC_CALIB = 12
     RPC_READ_GAINS_FROM_FLASH = 13
     RPC_REPLY_READ_GAINS_FROM_FLASH = 14
     RPC_SET_MENU_ON = 15
@@ -37,14 +38,20 @@
     RPC_REPLY_MOTION_LIMITS = 20
     RPC_SET_NEXT_TRAJECTORY_SEG =21
     RPC_REPLY_SET_NEXT_TRAJECTORY_SEG =22
     RPC_START_NEW_TRAJECTORY =23
     RPC_REPLY_START_NEW_TRAJECTORY =24
     RPC_RESET_TRAJECTORY =25
     RPC_REPLY_RESET_TRAJECTORY =26
+    RPC_READ_TRACE =27
+    RPC_REPLY_READ_TRACE =28
+    RPC_GET_STATUS_AUX = 29
+    RPC_REPLY_STATUS_AUX = 30
+    RPC_LOAD_TEST_PULL = 31
+    RPC_REPLY_LOAD_TEST_PULL = 32
 
     MODE_SAFETY = 0
     MODE_FREEWHEEL = 1
     MODE_HOLD = 2
     MODE_POS_PID = 3
     MODE_VEL_PID = 4
     MODE_POS_TRAJ = 5
@@ -77,217 +84,267 @@
     DIAG_CALIBRATION_RCVD = 256  # Is calibration table in flash
     DIAG_IN_GUARDED_EVENT = 512  # Guarded event occurred during motion
     DIAG_IN_SAFETY_EVENT = 1024  # Is it forced into safety mode
     DIAG_WAITING_ON_SYNC = 2048  # Command received but no sync yet
     DIAG_TRAJ_ACTIVE     = 4096     # Whether a waypoint trajectory is actively executing
     DIAG_TRAJ_WAITING_ON_SYNC = 8192 # Currently waiting on a sync signal before starting trajectory
     DIAG_IN_SYNC_MODE = 16384        # Currently running in sync mode
+    DIAG_IS_TRACE_ON = 32768   #Is trace recording
 
     CONFIG_SAFETY_HOLD = 1  # Hold position in safety mode? Otherwise freewheel
     CONFIG_ENABLE_RUNSTOP = 2  # Recognize runstop signal?
     CONFIG_ENABLE_SYNC_MODE = 4  # Commands are synchronized from digital trigger
     CONFIG_ENABLE_GUARDED_MODE = 8  # Stops on current threshold
     CONFIG_FLIP_ENCODER_POLARITY = 16
     CONFIG_FLIP_EFFORT_POLARITY = 32
-
+    CONFIG_ENABLE_VEL_WATCHDOG = 64 #Timeout velocity commands
 
     TRIGGER_MARK_POS = 1
     TRIGGER_RESET_MOTION_GEN = 2
     TRIGGER_BOARD_RESET = 4
     TRIGGER_WRITE_GAINS_TO_FLASH = 8
     TRIGGER_RESET_POS_CALIBRATED = 16
     TRIGGER_POS_CALIBRATED = 32
     TRIGGER_MARK_POS_ON_CONTACT=64
+    TRIGGER_ENABLE_TRACE=128
+    TRIGGER_DISABLE_TRACE=256
+
+    TRACE_TYPE_STATUS = 0
+    TRACE_TYPE_DEBUG = 1
+    TRACE_TYPE_PRINT = 2
+
 
-    def __init__(self, usb):
-        Device.__init__(self, name=usb[5:])
+    def __init__(self, usb,name=None):
+        if name is None:
+            name=usb[5:] #Pull from usb device name
+        Device.__init__(self, name=name)
         self.usb=usb
-        self.lock=threading.RLock()
         self.transport = Transport(usb=self.usb, logger=self.logger)
 
         self._command = {'mode':0, 'x_des':0,'v_des':0,'a_des':0,'stiffness':1.0,'i_feedforward':0.0,'i_contact_pos':0,'i_contact_neg':0,'incr_trigger':0}
         self.status = {'mode': 0, 'effort_ticks': 0, 'effort_pct':0,'current':0,'pos': 0, 'vel': 0, 'err':0,'diag': 0,'timestamp': 0, 'debug':0,'guarded_event':0,
                        'transport': self.transport.status,'pos_calibrated':0,'runstop_on':0,'near_pos_setpoint':0,'near_vel_setpoint':0,
                        'is_moving':0,'is_moving_filtered':0,'at_current_limit':0,'is_mg_accelerating':0,'is_mg_moving':0,'calibration_rcvd': 0,'in_guarded_event':0,
-                       'in_safety_event':0,'waiting_on_sync':0,
+                       'in_safety_event':0,'waiting_on_sync':0,'in_sync_mode':0,'trace_on':0,'ctrl_cycle_cnt':0,
                        'waypoint_traj':{'state':'idle','setpoint':None, 'segment_id':0,}}
+
+        self.status_aux={'cmd_cnt_rpc':0,'cmd_cnt_exec':0,'cmd_rpc_overflow':0,'sync_irq_cnt':0,'sync_irq_overflow':0}
+
+        self.status_zero=self.status.copy()
+
         self.board_info={'board_variant':None, 'firmware_version':None,'protocol_version':None,'hardware_id':0}
         self.motion_limits=[0,0]
         self.is_moving_history = [False] * 10
 
         self._waypoint_traj_segment = [0] * 8
         self._waypoint_traj_start_success = False
         self._waypoint_traj_set_next_traj_success = False
         self._waypoint_traj_start_error_msg = ""
         self._waypoint_traj_set_next_error_msg = ""
         self._waypoint_ts = None
 
+        self.ts_last_syncd_motion=0
+
         self._dirty_command = False
         self._dirty_gains = False
         self._dirty_trigger = False
         self._dirty_read_gains_from_flash=False
-        self._dirty_load_test=False
         self._trigger=0
         self._trigger_data=0
         self.load_test_payload = arr.array('B', range(256)) * 4
         self.hw_valid=False
         self.gains = self.params['gains'].copy()
         self.gains_flash = {}
 
+
     # ###########  Device Methods #############
     def startup(self, threaded=False):
         try:
             Device.startup(self, threaded=threaded)
-            with self.lock:
-                self.hw_valid = self.transport.startup()
-                if self.hw_valid:
-                    # Pull board info
-                    self.transport.payload_out[0] = self.RPC_GET_STEPPER_BOARD_INFO
-                    self.transport.queue_rpc(1, self.rpc_board_info_reply)
-                    self.transport.step(exiting=False)
-                    return True
-                return False
+            self.hw_valid = self.transport.startup()
+            if self.hw_valid:
+                # Pull board info
+                payload = arr.array('B', [self.RPC_GET_STEPPER_BOARD_INFO])
+                self.transport.do_pull_rpc_sync(payload, self.rpc_board_info_reply)
+                self.transport.configure_version(self.board_info['firmware_version'])
+                return True
+            return False
         except KeyError:
             self.hw_valid =False
             return False
 
     #Configure control mode prior to calling this on process shutdown (or default to freewheel)
     def stop(self):
         Device.stop(self)
         if not self.hw_valid:
             return
-        with self.lock:
-            self.logger.debug('Shutting down Stepper on: ' + self.usb)
-            self.enable_safety()
-            self.push_command(exiting=True)
-            self.transport.stop()
-            self.hw_valid = False
+        self.logger.debug('Shutting down Stepper on: ' + self.usb)
+        self.enable_safety()
+        self.push_command(exiting=True)
+        self.transport.stop()
+        self.hw_valid = False
+
+    def is_sync_required(self, ts_last_sync):
+        return self.status['in_sync_mode'] and self.ts_last_syncd_motion > ts_last_sync
 
-    def push_command(self,exiting=False):
+    def push_command(self, exiting=False):
         if not self.hw_valid:
             return
-        with self.lock:
-            if self._dirty_load_test:
-                self.transport.payload_out[0] = self.RPC_LOAD_TEST
-                self.transport.payload_out[1:] = self.load_test_payload
-                self.transport.queue_rpc2(1024 + 1, self.rpc_load_test_reply)
-                self._dirty_load_test=False
-
-            if self._dirty_trigger:
-                self.transport.payload_out[0] = self.RPC_SET_TRIGGER
-                sidx = self.pack_trigger(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_trigger_reply)
-                self._trigger=0
-                self._dirty_trigger = False
-
-            if self._dirty_gains:
-                self.transport.payload_out[0] = self.RPC_SET_GAINS
-                sidx = self.pack_gains(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_gains_reply)
-                self._dirty_gains=False
-
-            if self._dirty_command:
-                self.transport.payload_out[0] = self.RPC_SET_COMMAND
-                sidx = self.pack_command(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_command_reply)
-                self._dirty_command=False
-            self.transport.step2(exiting=exiting)
+        payload = self.transport.get_empty_payload()
+
+        if self._dirty_trigger:
+            payload[0] = self.RPC_SET_TRIGGER
+            sidx = self.pack_trigger(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_trigger_reply, exiting=exiting)
+            self._trigger=0
+            self._dirty_trigger = False
+
+        if self._dirty_gains:
+            payload[0] = self.RPC_SET_GAINS
+            sidx = self.pack_gains(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_gains_reply, exiting=exiting)
+            self._dirty_gains = False
+
+        if self._dirty_command:
+            if self.status['in_sync_mode']:  # Mark the time of latest new motion command sent
+                self.ts_last_syncd_motion = time.time()
+            else:
+                self.ts_last_syncd_motion = 0
+
+            payload[0] = self.RPC_SET_COMMAND
+            sidx = self.pack_command(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_command_reply, exiting=exiting)
+            self._dirty_command = False
+
+    async def push_command_async(self,exiting=False):
+        if not self.hw_valid:
+            return
+        payload = self.transport.get_empty_payload()
+
+        if self._dirty_trigger:
+            payload[0] = self.RPC_SET_TRIGGER
+            sidx = self.pack_trigger(payload, 1)
+            await self.transport.do_push_rpc_async(payload[:sidx], self.rpc_trigger_reply, exiting=exiting)
+            self._trigger=0
+            self._dirty_trigger = False
+
+        if self._dirty_gains:
+            payload[0] = self.RPC_SET_GAINS
+            sidx = self.pack_gains(payload, 1)
+            await self.transport.do_push_rpc_async(payload[:sidx], self.rpc_gains_reply, exiting=exiting)
+            self._dirty_gains = False
+
+        if self._dirty_command:
+            if self.status['in_sync_mode']: #Mark the time of latest new motion command sent
+                self.ts_last_syncd_motion=time.time()
+            else:
+                self.ts_last_syncd_motion = 0
 
+            payload[0] = self.RPC_SET_COMMAND
+            sidx = self.pack_command(payload, 1)
+            await self.transport.do_push_rpc_async(payload[:sidx], self.rpc_command_reply, exiting=exiting)
+            self._dirty_command = False
 
     def pull_status(self, exiting=False):
         if not self.hw_valid:
             return
-        with self.lock:
-            if self._dirty_read_gains_from_flash:
-                self.transport.payload_out[0] = self.RPC_READ_GAINS_FROM_FLASH
-                self.transport.queue_rpc(1, self.rpc_read_gains_from_flash_reply)
-                self._dirty_read_gains_from_flash = False
+        if self._dirty_read_gains_from_flash:
+            payload = arr.array('B', [self.RPC_READ_GAINS_FROM_FLASH])
+            self.transport.do_pull_rpc_sync(payload, self.rpc_read_gains_from_flash_reply)
+            self._dirty_read_gains_from_flash = False
+        payload = arr.array('B', [self.RPC_GET_STATUS])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_status_reply, exiting=exiting)
 
-            # Queue Status RPC
-            self.transport.payload_out[0] = self.RPC_GET_STATUS
-            sidx = 1
-            self.transport.queue_rpc(sidx, self.rpc_status_reply)
-            self.transport.step(exiting=exiting)
+    async def pull_status_async(self, exiting=False):
+        if not self.hw_valid:
+            return
+
+        if self._dirty_read_gains_from_flash:
+            payload = arr.array('B', [self.RPC_READ_GAINS_FROM_FLASH])
+            await self.transport.do_pull_rpc_async(payload, self.rpc_read_gains_from_flash_reply, exiting=exiting)
+            self._dirty_read_gains_from_flash = False
+
+        payload = arr.array('B', [self.RPC_GET_STATUS])
+        await self.transport.do_pull_rpc_async(payload, self.rpc_status_reply, exiting=exiting)
+
+    def push_load_test(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def pull_load_test(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
 
     def pretty_print(self):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
-            .format(self.board_info['protocol_version']))
+                                  .format(self.board_info['protocol_version']))
 
     def step_sentry(self, robot):
         if self.hw_valid and self.robot_params['robot_sentry']['stepper_is_moving_filter']:
             self.is_moving_history.pop(0)
             self.is_moving_history.append(self.status['is_moving'])
             self.status['is_moving_filtered'] = max(set(self.is_moving_history), key=self.is_moving_history.count)
+
     # ###########################################################################
     # ###########################################################################
 
-    def set_load_test(self):
-        self._dirty_load_test=True
 
     def set_motion_limits(self,limit_neg, limit_pos):
-        with self.lock:
-            if limit_neg!=self.motion_limits[0] or limit_pos!=self.motion_limits[1]:
-                #Push out immediately
-                self.motion_limits=[limit_neg, limit_pos]
-                self.transport.payload_out[0] = self.RPC_SET_MOTION_LIMITS
-                sidx = self.pack_motion_limits(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_motion_limits_reply)
-                self.transport.step2()
+        if limit_neg!=self.motion_limits[0] or limit_pos!=self.motion_limits[1]:
+            #Push out immediately
+            self.motion_limits=[limit_neg, limit_pos]
+            payload=self.transport.get_empty_payload()
+            payload[0] = self.RPC_SET_MOTION_LIMITS
+            sidx = self.pack_motion_limits(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_motion_limits_reply)
 
     def set_gains(self,g):
-        with self.lock:
-            self.gains=g.copy()
-            self._dirty_gains = True
+        self.gains=g.copy()
+        self._dirty_gains = True
 
     def write_gains_to_YAML(self):
         raise DeprecationWarning('This method has been deprecated since v0.3.0')
 
     def write_gains_to_flash(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_WRITE_GAINS_TO_FLASH
-            self._dirty_trigger = True
+        self._trigger = self._trigger | self.TRIGGER_WRITE_GAINS_TO_FLASH
+        self._dirty_trigger = True
 
     def read_gains_from_flash(self):
         self._dirty_read_gains_from_flash=True
 
     def board_reset(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_BOARD_RESET
-            self._dirty_trigger=True
+        self._trigger = self._trigger | self.TRIGGER_BOARD_RESET
+        self._dirty_trigger=True
 
     def mark_position_on_contact(self,x):
-        with self.lock:
-            self._trigger_data = x
-            self._trigger = self._trigger | self.TRIGGER_MARK_POS_ON_CONTACT
-            self._dirty_trigger=True
+        self._trigger_data = x
+        self._trigger = self._trigger | self.TRIGGER_MARK_POS_ON_CONTACT
+        self._dirty_trigger=True
 
     def mark_position(self,x):
         if self.status['mode']!=self.MODE_SAFETY:
             self.logger.warning('Can not mark position. Must be in MODE_SAFETY for %s'%self.usb)
             return
-
-        with self.lock:
-            self._trigger_data=x
-            self._trigger = self._trigger | self.TRIGGER_MARK_POS
-            self._dirty_trigger=True
+        self._trigger_data=x
+        self._trigger = self._trigger | self.TRIGGER_MARK_POS
+        self._dirty_trigger=True
 
     def reset_motion_gen(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_RESET_MOTION_GEN
-            self._dirty_trigger = True
+        self._trigger = self._trigger | self.TRIGGER_RESET_MOTION_GEN
+        self._dirty_trigger = True
 
     def reset_pos_calibrated(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_RESET_POS_CALIBRATED
-            self._dirty_trigger = True
+        self._trigger = self._trigger | self.TRIGGER_RESET_POS_CALIBRATED
+        self._dirty_trigger = True
 
     def set_pos_calibrated(self):
-        with self.lock:
-            self._trigger = self._trigger | self.TRIGGER_POS_CALIBRATED
-            self._dirty_trigger = True
+        self._trigger = self._trigger | self.TRIGGER_POS_CALIBRATED
+        self._dirty_trigger = True
+
+
 
     # ###########################################################################
     def enable_safety(self):
             self.set_command(mode=self.MODE_SAFETY)
 
     def enable_freewheel(self):
             self.set_command(mode=self.MODE_FREEWHEEL)
@@ -337,66 +394,68 @@
         self.gains['enable_guarded_mode'] = 1
         self._dirty_gains = 1
 
     def disable_guarded_mode(self):
         self.gains['enable_guarded_mode'] = 0
         self._dirty_gains = 1
 
+
+
+    # ######################################################################
     #Primary interface to controlling the stepper
     #YAML defaults are used if values not provided
     #This allows user to override defaults every control cycle and then easily revert to defaults
     def set_command(self,mode=None, x_des=None, v_des=None, a_des=None,i_des=None, stiffness=None,i_feedforward=None, i_contact_pos=None, i_contact_neg=None  ):
-        with self.lock:
-            if mode is not None:
-                self._command['mode'] = mode
-
-            if x_des is not None:
-                self._command['x_des'] = x_des
-                if self._command['mode'] == self.MODE_POS_TRAJ_INCR:
-                    self._command['incr_trigger'] = (self._command['incr_trigger']+1)%255
+        if mode is not None:
+            self._command['mode'] = mode
 
-            if v_des is not None:
-                self._command['v_des'] = v_des
-            else:
-                if mode == self.MODE_VEL_PID or mode == self.MODE_VEL_TRAJ:
-                    self._command['v_des'] = 0
-                else:
-                    self._command['v_des'] = self.params['motion']['vel']
+        if x_des is not None:
+            self._command['x_des'] = x_des
+            if self._command['mode'] == self.MODE_POS_TRAJ_INCR:
+                self._command['incr_trigger'] = (self._command['incr_trigger']+1)%255
 
-            if a_des is not None:
-                self._command['a_des'] = a_des
+        if v_des is not None:
+            self._command['v_des'] = v_des
+        else:
+            if mode == self.MODE_VEL_PID or mode == self.MODE_VEL_TRAJ:
+                self._command['v_des'] = 0
             else:
-                self._command['a_des'] = self.params['motion']['accel']
+                self._command['v_des'] = self.params['motion']['vel']
 
-            if stiffness is not None:
-                self._command['stiffness'] = max(0.0, min(1.0, stiffness))
-            else:
-                self._command['stiffness'] =1
+        if a_des is not None:
+            self._command['a_des'] = a_des
+        else:
+            self._command['a_des'] = self.params['motion']['accel']
 
-            if i_feedforward is not None:
-                self._command['i_feedforward'] = i_feedforward
-            else:
-                self._command['i_feedforward'] = 0
+        if stiffness is not None:
+            self._command['stiffness'] = max(0.0, min(1.0, stiffness))
+        else:
+            self._command['stiffness'] =1
 
-            if i_des is not None and mode == self.MODE_CURRENT:
-                self._command['i_feedforward'] =i_des
+        if i_feedforward is not None:
+            self._command['i_feedforward'] = i_feedforward
+        else:
+            self._command['i_feedforward'] = 0
 
+        if i_des is not None and mode == self.MODE_CURRENT:
+            self._command['i_feedforward'] =i_des
 
-            if i_contact_pos is not None:
-                self._command['i_contact_pos'] = i_contact_pos
-            else:
-                self._command['i_contact_pos']=self.params['gains']['i_contact_pos']
 
-            if i_contact_neg is not None:
-                self._command['i_contact_neg'] = i_contact_neg
-            else:
-                self._command['i_contact_neg'] = self.params['gains']['i_contact_neg']
-            #print(time.time(), i_des, self._command['i_feedforward'],mode == self.MODE_CURRENT)
-            #print(time.time(),self._command['x_des'],self._command['incr_trigger'],self._command['v_des'],self._command['a_des'])
-            self._dirty_command=True
+        if i_contact_pos is not None:
+            self._command['i_contact_pos'] = i_contact_pos
+        else:
+            self._command['i_contact_pos']=self.params['gains']['i_contact_pos']
+
+        if i_contact_neg is not None:
+            self._command['i_contact_neg'] = i_contact_neg
+        else:
+            self._command['i_contact_neg'] = self.params['gains']['i_contact_neg']
+        #print(time.time(), i_des, self._command['i_feedforward'],mode == self.MODE_CURRENT)
+        #print(time.time(),self._command['x_des'],self._command['incr_trigger'],self._command['v_des'],self._command['a_des'])
+        self._dirty_command=True
 
 
     def wait_while_is_moving(self,timeout=15.0):
         """
         Poll until is moving flag is false
         Return True if success
         Return False if timeout
@@ -424,23 +483,23 @@
     ########### Handle current and effort conversions  ###########
 
     #Effort_ticks are in the units of the uC current controller (0-255 8 bit)
     #Conversion to A is based on the sense resistor and motor driver (see firmware)
     def current_to_effort_ticks(self,i_A):
         if self.board_info['hardware_id']==0: # I = Vref / (10 * R), Rs = 0.10 Ohm, Vref = 3.3V -->3.3A
             mA_per_tick = (3300 / 255) / (10 * 0.1)
-        if self.board_info['hardware_id']==1: # I = Vref / (5 * R), Rs = 0.150 Ohm, Vref = 3.3V -->4.4A
+        if self.board_info['hardware_id']>=1: # I = Vref / (5 * R), Rs = 0.150 Ohm, Vref = 3.3V -->4.4A
             mA_per_tick = (3300 / 255) / (5 * 0.15)
         effort_ticks = (i_A * 1000.0) / mA_per_tick
         return min(255,max(-255,int(effort_ticks)))
 
     def effort_ticks_to_current(self,e):
         if self.board_info['hardware_id'] == 0:  # I = Vref / (10 * R), Rs = 0.10 Ohm, Vref = 3.3V -->3.3A
             mA_per_tick = (3300 / 255) / (10 * 0.1)
-        if self.board_info['hardware_id'] == 1:  # I = Vref / (5 * R), Rs = 0.150 Ohm, Vref = 3.3V -->4.4A
+        if self.board_info['hardware_id'] >= 1:  # I = Vref / (5 * R), Rs = 0.150 Ohm, Vref = 3.3V -->4.4A
             mA_per_tick = (3300 / 255) / (5 * 0.15)
         return e * mA_per_tick / 1000.0
 
     # Effort_pct is defined as a percentage of the maximum allowable motor winding current
     # Range is -100.0 to 100.0
     def current_to_effort_pct(self,i_A):
         if i_A>0:
@@ -474,24 +533,26 @@
     def read_encoder_calibration_from_YAML(self):
         device_name=self.usb[5:]
         sn=self.robot_params[device_name]['serial_no']
         fn='calibration_steppers/'+device_name+'_'+sn+'.yaml'
         enc_data=read_fleet_yaml(fn)
         return enc_data
 
-    def write_encoder_calibration_to_YAML(self,data):
+    def write_encoder_calibration_to_YAML(self,data,filename=None, fleet_dir=None):
         device_name = self.usb[5:]
-        sn = self.robot_params[device_name]['serial_no']
-        fn = 'calibration_steppers/'+device_name + '_' + sn + '.yaml'
-        print('Writing encoder calibration: %s'%fn)
-        write_fleet_yaml(fn,data)
+        if filename is None:
+            sn = self.robot_params[device_name]['serial_no']
+            filename = 'calibration_steppers/'+device_name + '_' + sn + '.yaml'
+        print('Writing encoder calibration: %s'%filename)
+        write_fleet_yaml(filename,data,fleet_dir=fleet_dir)
 
     def read_encoder_calibration_from_flash(self):
         self.turn_menu_interface_on()
         time.sleep(0.5)
+        time.sleep(0.5)
         self.logger.debug('Reading encoder calibration...')
         e = self.menu_transaction(b'q',do_print=False)[19]
         self.turn_rpc_interface_on()
         self.push_command()
         self.logger.debug('Reseting board')
         self.board_reset()
         self.push_command()
@@ -515,66 +576,64 @@
         if not self.hw_valid:
             return
         #This will take a few seconds. Blocks until complete.
         if len(data)!=16384:
             self.logger.warning('Bad encoder data')
         else:
             self.logger.debug('Writing encoder calibration...')
+            payload=self.transport.get_empty_payload()
             for p in range(256):
                 if p%10==0:
                     sys.stdout.write('.')
                     sys.stdout.flush()
-                self.transport.payload_out[0] = self.RPC_SET_ENC_CALIB
-                self.transport.payload_out[1] = p
+                payload[0] = self.RPC_SET_ENC_CALIB
+                payload[1] = p
                 sidx=2
                 for i in range(64):
-                    pack_float_t(self.transport.payload_out, sidx, data[p*64+i])
+                    pack_float_t(payload, sidx, data[p*64+i])
                     sidx += 4
                 # self.logger.debug('Sending encoder calibration rpc of size',sidx)
-                self.transport.queue_rpc(sidx, self.rpc_enc_calib_reply)
-                self.transport.step()
+                self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_enc_calib_reply)
 
     def rpc_enc_calib_reply(self,reply):
         if reply[0] != self.RPC_REPLY_ENC_CALIB:
             self.logger.debug('Error RPC_REPLY_ENC_CALIB', reply[0])
 
     # ######################Menu Interface ################################3
 
 
     def turn_rpc_interface_on(self):
-        with self.lock:
-            self.menu_transaction(b'zyx')
+        self.menu_transaction(b'zyx')
 
 
     def turn_menu_interface_on(self):
         if not self.hw_valid:
             return
-        with self.lock:
-            # Run immediately rather than queue
-            self.transport.payload_out[0] = self.RPC_SET_MENU_ON
-            self.transport.queue_rpc(1, self.rpc_menu_on_reply)
-            self.transport.step()
+        payload = arr.array('B',[self.RPC_SET_MENU_ON])
+        self.transport.do_push_rpc_sync(payload, self.rpc_menu_on_reply)
+
 
     def print_menu(self):
-        with self.lock:
-            self.menu_transaction(b'm')
+        self.menu_transaction(b'm')
 
     def menu_transaction(self,x,do_print=True):
         if not self.hw_valid:
             return
-        with self.lock:
-            self.transport.ser.write(x)
-            time.sleep(0.1)
-            reply=[]
-            while self.transport.ser.inWaiting():
-                r=self.transport.ser.readline()
-                if do_print:
+        self.transport.ser.write(x)
+        time.sleep(0.1)
+        reply=[]
+        while self.transport.ser.inWaiting():
+            r=self.transport.ser.readline()
+            if do_print:
+                if type(r)==bytes:
+                    print(r.decode('UTF-8'), end=' ')
+                else:
                     print(r, end=' ')
-                reply.append(r)
-            return reply
+            reply.append(r)
+        return reply
 
     # ################Waypoint Trajectory Interface #####################
     def start_waypoint_trajectory(self, first_segment):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
     def set_next_trajectory_segment(self, next_segment):
@@ -583,152 +642,138 @@
 
     def stop_waypoint_trajectory(self):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
     # ################Transport Callbacks #####################
     def unpack_board_info(self,s):
-        with self.lock:
-            sidx=0
-            self.board_info['board_variant'] = unpack_string_t(s[sidx:], 20).strip('\x00')
-            self.board_info['hardware_id'] = 0
-            if len(self.board_info['board_variant'])==9: #New format of Stepper.x  Older format of Stepper.BoardName.Vx' If older format,default to 0
-                self.board_info['hardware_id']=int(self.board_info['board_variant'][-1])
-            sidx += 20
-            self.board_info['firmware_version'] = unpack_string_t(s[sidx:], 20).strip('\x00')
-            self.board_info['protocol_version'] = self.board_info['firmware_version'][self.board_info['firmware_version'].rfind('p'):]
-            sidx += 20
-            return sidx
+        sidx=0
+        self.board_info['board_variant'] = unpack_string_t(s[sidx:], 20).strip('\x00')
+        self.board_info['hardware_id'] = 0
+        if len(self.board_info['board_variant'])==9: #New format of Stepper.x  Older format of Stepper.BoardName.Vx' If older format,default to 0
+            self.board_info['hardware_id']=int(self.board_info['board_variant'][-1])
+        sidx += 20
+        self.board_info['firmware_version'] = unpack_string_t(s[sidx:], 20).strip('\x00')
+        self.board_info['protocol_version'] = self.board_info['firmware_version'][self.board_info['firmware_version'].rfind('p'):]
+        sidx += 20
+        return sidx
 
     def unpack_status(self,s):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
     def unpack_gains(self,s):
-        with self.lock:
-            sidx=0
-            self.gains_flash['pKp_d'] = unpack_float_t(s[sidx:]);sidx+=4
-            self.gains_flash['pKi_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['pKd_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['pLPF'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['pKi_limit'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vKp_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vKi_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vKd_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vLPF'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vKi_limit'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vTe_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['iMax_pos'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['iMax_neg'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['phase_advance_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['pos_near_setpoint_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vel_near_setpoint_d'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['vel_status_LPF'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['effort_LPF'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['safety_stiffness'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.gains_flash['i_safety_feedforward'] = unpack_float_t(s[sidx:]);sidx += 4
-            config = unpack_uint8_t(s[sidx:]);sidx += 1
-            self.gains_flash['safety_hold']= int(config & self.CONFIG_SAFETY_HOLD>0)
-            self.gains_flash['enable_runstop'] = int(config & self.CONFIG_ENABLE_RUNSTOP>0)
-            self.gains_flash['enable_sync_mode'] = int(config & self.CONFIG_ENABLE_SYNC_MODE>0)
-            self.gains_flash['enable_guarded_mode'] = int(config & self.CONFIG_ENABLE_GUARDED_MODE > 0)
-            self.gains_flash['flip_encoder_polarity'] = int(config & self.CONFIG_FLIP_ENCODER_POLARITY > 0)
-            self.gains_flash['flip_effort_polarity'] = int(config & self.CONFIG_FLIP_EFFORT_POLARITY > 0)
-            return sidx
-
-    def pack_motion_limits(self,s,sidx):
-        with self.lock:
-            pack_float_t(s, sidx, self.motion_limits[0])
-            sidx += 4
-            pack_float_t(s, sidx, self.motion_limits[1])
-            sidx += 4
-            return sidx
-
-    def pack_command(self,s,sidx):
-        with self.lock:
-            pack_uint8_t(s, sidx, self._command['mode'])
-            sidx += 1
-            pack_float_t(s, sidx, self._command['x_des'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['v_des'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['a_des'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['stiffness'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['i_feedforward'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['i_contact_pos'])
-            sidx += 4
-            pack_float_t(s, sidx, self._command['i_contact_neg'])
-            sidx += 4
-            pack_uint8_t(s, sidx, self._command['incr_trigger'])
-            sidx += 1
-            return sidx
+        sidx=0
+        self.gains_flash['pKp_d'] = unpack_float_t(s[sidx:]);sidx+=4
+        self.gains_flash['pKi_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['pKd_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['pLPF'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['pKi_limit'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vKp_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vKi_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vKd_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vLPF'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vKi_limit'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vTe_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['iMax_pos'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['iMax_neg'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['phase_advance_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['pos_near_setpoint_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vel_near_setpoint_d'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['vel_status_LPF'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['effort_LPF'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['safety_stiffness'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.gains_flash['i_safety_feedforward'] = unpack_float_t(s[sidx:]);sidx += 4
+        config = unpack_uint8_t(s[sidx:]);sidx += 1
+        self.gains_flash['safety_hold']= int(config & self.CONFIG_SAFETY_HOLD>0)
+        self.gains_flash['enable_runstop'] = int(config & self.CONFIG_ENABLE_RUNSTOP>0)
+        self.gains_flash['enable_sync_mode'] = int(config & self.CONFIG_ENABLE_SYNC_MODE>0)
+        self.gains_flash['enable_guarded_mode'] = int(config & self.CONFIG_ENABLE_GUARDED_MODE > 0)
+        self.gains_flash['flip_encoder_polarity'] = int(config & self.CONFIG_FLIP_ENCODER_POLARITY > 0)
+        self.gains_flash['flip_effort_polarity'] = int(config & self.CONFIG_FLIP_EFFORT_POLARITY > 0)
+        self.gains_flash['enable_vel_watchdog'] = int(config & self.CONFIG_ENABLE_VEL_WATCHDOG > 0)
+        return sidx
+
+    def pack_motion_limits(self, s, sidx):
+        pack_float_t(s, sidx, self.motion_limits[0])
+        sidx += 4
+        pack_float_t(s, sidx, self.motion_limits[1])
+        sidx += 4
+        return sidx
+
+    def pack_command(self, s, sidx):
+        pack_uint8_t(s, sidx, self._command['mode'])
+        sidx += 1
+        pack_float_t(s, sidx, self._command['x_des'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['v_des'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['a_des'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['stiffness'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['i_feedforward'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['i_contact_pos'])
+        sidx += 4
+        pack_float_t(s, sidx, self._command['i_contact_neg'])
+        sidx += 4
+        pack_uint8_t(s, sidx, self._command['incr_trigger'])
+        sidx += 1
+        return sidx
 
     def pack_gains(self,s,sidx):
-        with self.lock:
-            pack_float_t(s, sidx, self.gains['pKp_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['pKi_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['pKd_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['pLPF']);sidx += 4
-            pack_float_t(s, sidx, self.gains['pKi_limit']);sidx += 4
-            pack_float_t(s, sidx, self.gains['vKp_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['vKi_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['vKd_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['vLPF']);sidx += 4
-            pack_float_t(s, sidx, self.gains['vKi_limit']); sidx += 4
-            pack_float_t(s, sidx, self.gains['vTe_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['iMax_pos']);sidx += 4
-            pack_float_t(s, sidx, self.gains['iMax_neg']);sidx += 4
-            pack_float_t(s, sidx, self.gains['phase_advance_d']);sidx += 4
-            pack_float_t(s, sidx, self.gains['pos_near_setpoint_d']); sidx += 4
-            pack_float_t(s, sidx, self.gains['vel_near_setpoint_d']); sidx += 4
-            pack_float_t(s, sidx, self.gains['vel_status_LPF']);sidx += 4
-            pack_float_t(s, sidx, self.gains['effort_LPF']);sidx += 4
-            pack_float_t(s, sidx, self.gains['safety_stiffness']);sidx += 4
-            pack_float_t(s, sidx, self.gains['i_safety_feedforward']);sidx += 4
-            config=0
-            if self.gains['safety_hold']:
-                config=config | self.CONFIG_SAFETY_HOLD
-            if self.gains['enable_runstop']:
-                config=config | self.CONFIG_ENABLE_RUNSTOP
-            if self.gains['enable_sync_mode']:
-                config=config | self.CONFIG_ENABLE_SYNC_MODE
-            if self.gains['enable_guarded_mode']:
-                config=config | self.CONFIG_ENABLE_GUARDED_MODE
-            if self.gains['flip_encoder_polarity']:
-                config = config | self.CONFIG_FLIP_ENCODER_POLARITY
-            if self.gains['flip_effort_polarity']:
-                config = config | self.CONFIG_FLIP_EFFORT_POLARITY
-            pack_uint8_t(s, sidx, config); sidx += 1
-            return sidx
+        pack_float_t(s, sidx, self.gains['pKp_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['pKi_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['pKd_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['pLPF']);sidx += 4
+        pack_float_t(s, sidx, self.gains['pKi_limit']);sidx += 4
+        pack_float_t(s, sidx, self.gains['vKp_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['vKi_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['vKd_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['vLPF']);sidx += 4
+        pack_float_t(s, sidx, self.gains['vKi_limit']); sidx += 4
+        pack_float_t(s, sidx, self.gains['vTe_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['iMax_pos']);sidx += 4
+        pack_float_t(s, sidx, self.gains['iMax_neg']);sidx += 4
+        pack_float_t(s, sidx, self.gains['phase_advance_d']);sidx += 4
+        pack_float_t(s, sidx, self.gains['pos_near_setpoint_d']); sidx += 4
+        pack_float_t(s, sidx, self.gains['vel_near_setpoint_d']); sidx += 4
+        pack_float_t(s, sidx, self.gains['vel_status_LPF']);sidx += 4
+        pack_float_t(s, sidx, self.gains['effort_LPF']);sidx += 4
+        pack_float_t(s, sidx, self.gains['safety_stiffness']);sidx += 4
+        pack_float_t(s, sidx, self.gains['i_safety_feedforward']);sidx += 4
+        config=0
+        if self.gains['safety_hold']:
+            config=config | self.CONFIG_SAFETY_HOLD
+        if self.gains['enable_runstop']:
+            config=config | self.CONFIG_ENABLE_RUNSTOP
+        if self.gains['enable_sync_mode']:
+            config=config | self.CONFIG_ENABLE_SYNC_MODE
+        if self.gains['enable_guarded_mode']:
+            config=config | self.CONFIG_ENABLE_GUARDED_MODE
+        if self.gains['flip_encoder_polarity']:
+            config = config | self.CONFIG_FLIP_ENCODER_POLARITY
+        if self.gains['flip_effort_polarity']:
+            config = config | self.CONFIG_FLIP_EFFORT_POLARITY
+        if self.gains['enable_vel_watchdog']:
+            config=config | self.CONFIG_ENABLE_VEL_WATCHDOG
+        pack_uint8_t(s, sidx, config); sidx += 1
+        return sidx
 
     def pack_trigger(self, s, sidx):
-        with self.lock:
-            pack_uint32_t(s, sidx, self._trigger);
-            sidx += 4
-            pack_float_t(s, sidx, self._trigger_data);
-            sidx += 4
-            return sidx
-
+        pack_uint32_t(s, sidx, self._trigger)
+        sidx += 4
+        pack_float_t(s, sidx, self._trigger_data)
+        sidx += 4
+        return sidx
     def pack_trajectory_segment(self, s, sidx):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
-    def rpc_load_test_reply(self, reply):
-        if reply[0] == self.RPC_REPLY_LOAD_TEST:
-            d = reply[1:]
-            for i in range(1024):
-                if d[i] != self.load_test_payload[(i + 1) % 1024]:
-                    print('Load test bad data', d[i], self.load_test_payload[(i + 1) % 1024])
-            self.load_test_payload = d
-        else:
-            print('Error RPC_REPLY_LOAD_TEST', reply[0])
-
     def rpc_board_info_reply(self, reply):
         if reply[0] == self.RPC_REPLY_STEPPER_BOARD_INFO:
             self.unpack_board_info(reply[1:])
         else:
             print('Error RPC_REPLY_STEPPER_BOARD_INFO', reply[0])
 
     def rpc_gains_reply(self, reply):
@@ -759,57 +804,75 @@
 
     def rpc_read_gains_from_flash_reply(self, reply):
         if reply[0] == self.RPC_REPLY_READ_GAINS_FROM_FLASH:
             nr = self.unpack_gains(reply[1:])
         else:
             print('Error RPC_REPLY_READ_GAINS_FROM_FLASH', reply[0])
 
+
     def rpc_start_new_traj_reply(self, reply):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
     def rpc_set_next_traj_seg_reply(self, reply):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
     def rpc_reset_traj_reply(self, reply):
         raise NotImplementedError('This method not supported for firmware on protocol {0}.'
             .format(self.board_info['protocol_version']))
 
+
+    def rpc_read_firmware_trace_reply(self, reply):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def enable_firmware_trace(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+    def disable_firmware_trace(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
+
+    def pull_status_aux(self):
+        raise NotImplementedError('This method not supported for firmware on protocol {0}.'
+                                  .format(self.board_info['protocol_version']))
+
 # ######################## STEPPER PROTOCOL PO #################################
 
 class Stepper_Protocol_P0(StepperBase):
     def unpack_status(self,s):
-        with self.lock:
-            sidx=0
-            self.status['mode']=unpack_uint8_t(s[sidx:]);sidx+=1
-            self.status['effort_ticks'] = unpack_float_t(s[sidx:]);sidx+=4
-            self.status['current']=self.effort_ticks_to_current(self.status['effort_ticks'])
-            self.status['effort_pct']=self.current_to_effort_pct(self.status['current'])
-            self.status['pos'] = unpack_double_t(s[sidx:]);sidx+=8
-            self.status['vel'] = unpack_float_t(s[sidx:]);sidx+=4
-            self.status['err'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.status['diag'] = unpack_uint32_t(s[sidx:]);sidx += 4
-            self.status['timestamp'] = self.timestamp.set(unpack_uint32_t(s[sidx:]));sidx += 4
-            self.status['debug'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.status['guarded_event'] = unpack_uint32_t(s[sidx:]);sidx += 4
-
-            self.status['pos_calibrated'] =self.status['diag'] & self.DIAG_POS_CALIBRATED > 0
-            self.status['runstop_on'] =self.status['diag'] & self.DIAG_RUNSTOP_ON > 0
-            self.status['near_pos_setpoint'] =self.status['diag'] & self.DIAG_NEAR_POS_SETPOINT > 0
-            self.status['near_vel_setpoint'] = self.status['diag'] & self.DIAG_NEAR_VEL_SETPOINT > 0
-            self.status['is_moving'] =self.status['diag'] & self.DIAG_IS_MOVING > 0
-            self.status['at_current_limit'] =self.status['diag'] & self.DIAG_AT_CURRENT_LIMIT > 0
-            self.status['is_mg_accelerating'] = self.status['diag'] & self.DIAG_IS_MG_ACCELERATING > 0
-            self.status['is_mg_moving'] =self.status['diag'] & self.DIAG_IS_MG_MOVING > 0
-            self.status['calibration_rcvd'] = self.status['diag'] & self.DIAG_CALIBRATION_RCVD > 0
-            self.status['in_guarded_event'] = self.status['diag'] & self.DIAG_IN_GUARDED_EVENT > 0
-            self.status['in_safety_event'] = self.status['diag'] & self.DIAG_IN_SAFETY_EVENT > 0
-            self.status['waiting_on_sync'] = self.status['diag'] & self.DIAG_WAITING_ON_SYNC > 0
-            return sidx
+        sidx=0
+        self.status['mode']=unpack_uint8_t(s[sidx:]);sidx+=1
+        self.status['effort_ticks'] = unpack_float_t(s[sidx:]);sidx+=4
+        self.status['current']=self.effort_ticks_to_current(self.status['effort_ticks'])
+        self.status['effort_pct']=self.current_to_effort_pct(self.status['current'])
+        self.status['pos'] = unpack_double_t(s[sidx:]);sidx+=8
+        self.status['vel'] = unpack_float_t(s[sidx:]);sidx+=4
+        self.status['err'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.status['diag'] = unpack_uint32_t(s[sidx:]);sidx += 4
+        self.status['timestamp'] = self.timestamp.set(unpack_uint32_t(s[sidx:]));sidx += 4
+        self.status['debug'] = unpack_float_t(s[sidx:]);sidx += 4
+        self.status['guarded_event'] = unpack_uint32_t(s[sidx:]);sidx += 4
+
+        self.status['pos_calibrated'] =self.status['diag'] & self.DIAG_POS_CALIBRATED > 0
+        self.status['runstop_on'] =self.status['diag'] & self.DIAG_RUNSTOP_ON > 0
+        self.status['near_pos_setpoint'] =self.status['diag'] & self.DIAG_NEAR_POS_SETPOINT > 0
+        self.status['near_vel_setpoint'] = self.status['diag'] & self.DIAG_NEAR_VEL_SETPOINT > 0
+        self.status['is_moving'] =self.status['diag'] & self.DIAG_IS_MOVING > 0
+        self.status['at_current_limit'] =self.status['diag'] & self.DIAG_AT_CURRENT_LIMIT > 0
+        self.status['is_mg_accelerating'] = self.status['diag'] & self.DIAG_IS_MG_ACCELERATING > 0
+        self.status['is_mg_moving'] =self.status['diag'] & self.DIAG_IS_MG_MOVING > 0
+        self.status['calibration_rcvd'] = self.status['diag'] & self.DIAG_CALIBRATION_RCVD > 0
+        self.status['in_guarded_event'] = self.status['diag'] & self.DIAG_IN_GUARDED_EVENT > 0
+        self.status['in_safety_event'] = self.status['diag'] & self.DIAG_IN_SAFETY_EVENT > 0
+        self.status['waiting_on_sync'] = self.status['diag'] & self.DIAG_WAITING_ON_SYNC > 0
+        return sidx
 
     def pretty_print(self):
         print('-----------')
         print('Mode', self.MODE_NAMES[self.status['mode']])
         print('x_des (rad)', self._command['x_des'], '(deg)',rad_to_deg(self._command['x_des']))
         print('v_des (rad)', self._command['v_des'], '(deg)',rad_to_deg(self._command['v_des']))
         print('a_des (rad)', self._command['a_des'], '(deg)',rad_to_deg(self._command['a_des']))
@@ -834,58 +897,60 @@
         print('       Is MG Accelerating:', self.status['is_mg_accelerating'])
         print('       Is MG Moving:', self.status['is_mg_moving'])
         print('       Encoder Calibration in Flash:', self.status['calibration_rcvd'])
         print('       In Guarded Event:', self.status['in_guarded_event'])
         print('       In Safety Event:', self.status['in_safety_event'])
         print('       Waiting on Sync:', self.status['waiting_on_sync'])
         print('Timestamp (s)', self.status['timestamp'])
-        print('Read error', self.transport.status['read_error'])
+        #print('Read error', self.transport.status['read_error'])
         print('Board variant:', self.board_info['board_variant'])
         print('Firmware version:', self.board_info['firmware_version'])
 
 # ######################## STEPPER PROTOCOL P1 #################################
 class Stepper_Protocol_P1(StepperBase):
-    def unpack_status(self,s):
-        with self.lock:
-            sidx=0
-            self.status['mode']=unpack_uint8_t(s[sidx:]);sidx+=1
-            self.status['effort_ticks'] = unpack_float_t(s[sidx:]);sidx+=4
-            self.status['current']=self.effort_ticks_to_current(self.status['effort_ticks'])
-            self.status['effort_pct'] = self.current_to_effort_pct(self.status['current'])
-            self.status['pos'] = unpack_double_t(s[sidx:]);sidx+=8
-            self.status['vel'] = unpack_float_t(s[sidx:]);sidx+=4
-            self.status['err'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.status['diag'] = unpack_uint32_t(s[sidx:]);sidx += 4
-            self.status['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:]));sidx += 8
-            self.status['debug'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.status['guarded_event'] = unpack_uint32_t(s[sidx:]);sidx += 4
-            self.status['waypoint_traj']['setpoint'] = unpack_float_t(s[sidx:]);sidx += 4
-            self.status['waypoint_traj']['segment_id'] = unpack_uint16_t(s[sidx:]);sidx += 2
-
-            self.status['pos_calibrated'] =self.status['diag'] & self.DIAG_POS_CALIBRATED > 0
-            self.status['runstop_on'] =self.status['diag'] & self.DIAG_RUNSTOP_ON > 0
-            self.status['near_pos_setpoint'] =self.status['diag'] & self.DIAG_NEAR_POS_SETPOINT > 0
-            self.status['near_vel_setpoint'] = self.status['diag'] & self.DIAG_NEAR_VEL_SETPOINT > 0
-            self.status['is_moving'] =self.status['diag'] & self.DIAG_IS_MOVING > 0
-            self.status['at_current_limit'] =self.status['diag'] & self.DIAG_AT_CURRENT_LIMIT > 0
-            self.status['is_mg_accelerating'] = self.status['diag'] & self.DIAG_IS_MG_ACCELERATING > 0
-            self.status['is_mg_moving'] =self.status['diag'] & self.DIAG_IS_MG_MOVING > 0
-            self.status['calibration_rcvd'] = self.status['diag'] & self.DIAG_CALIBRATION_RCVD > 0
-            self.status['in_guarded_event'] = self.status['diag'] & self.DIAG_IN_GUARDED_EVENT > 0
-            self.status['in_safety_event'] = self.status['diag'] & self.DIAG_IN_SAFETY_EVENT > 0
-            self.status['waiting_on_sync'] = self.status['diag'] & self.DIAG_WAITING_ON_SYNC > 0
-            self.status['in_sync_mode'] = self.status['diag'] & self.DIAG_IN_SYNC_MODE > 0
-
-            if self.status['diag'] & self.DIAG_TRAJ_WAITING_ON_SYNC > 0:
-                self.status['waypoint_traj']['state']='waiting_on_sync'
-            elif self.status['diag'] & self.DIAG_TRAJ_ACTIVE > 0:
-                self.status['waypoint_traj']['state']='active'
-            else:
-                self.status['waypoint_traj']['state']='idle'
-            return sidx
+
+    def unpack_status(self,s,unpack_to=None):
+        if unpack_to is None:
+            unpack_to=self.status
+        sidx=0
+        unpack_to['mode']=unpack_uint8_t(s[sidx:]);sidx+=1
+        unpack_to['effort_ticks'] = unpack_float_t(s[sidx:]);sidx+=4
+        unpack_to['current']=self.effort_ticks_to_current(unpack_to['effort_ticks'])
+        unpack_to['effort_pct'] = self.current_to_effort_pct(unpack_to['current'])
+        unpack_to['pos'] = unpack_double_t(s[sidx:]);sidx+=8
+        unpack_to['vel'] = unpack_float_t(s[sidx:]);sidx+=4
+        unpack_to['err'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['diag'] = unpack_uint32_t(s[sidx:]);sidx += 4
+        unpack_to['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:]));sidx += 8
+        unpack_to['debug'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['guarded_event'] = unpack_uint32_t(s[sidx:]);sidx += 4
+        unpack_to['waypoint_traj']['setpoint'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['waypoint_traj']['segment_id'] = unpack_uint16_t(s[sidx:]);sidx += 2
+
+        unpack_to['pos_calibrated'] =unpack_to['diag'] & self.DIAG_POS_CALIBRATED > 0
+        unpack_to['runstop_on'] =unpack_to['diag'] & self.DIAG_RUNSTOP_ON > 0
+        unpack_to['near_pos_setpoint'] =unpack_to['diag'] & self.DIAG_NEAR_POS_SETPOINT > 0
+        unpack_to['near_vel_setpoint'] = unpack_to['diag'] & self.DIAG_NEAR_VEL_SETPOINT > 0
+        unpack_to['is_moving'] =unpack_to['diag'] & self.DIAG_IS_MOVING > 0
+        unpack_to['at_current_limit'] =unpack_to['diag'] & self.DIAG_AT_CURRENT_LIMIT > 0
+        unpack_to['is_mg_accelerating'] = unpack_to['diag'] & self.DIAG_IS_MG_ACCELERATING > 0
+        unpack_to['is_mg_moving'] =unpack_to['diag'] & self.DIAG_IS_MG_MOVING > 0
+        unpack_to['calibration_rcvd'] = unpack_to['diag'] & self.DIAG_CALIBRATION_RCVD > 0
+        unpack_to['in_guarded_event'] = unpack_to['diag'] & self.DIAG_IN_GUARDED_EVENT > 0
+        unpack_to['in_safety_event'] = unpack_to['diag'] & self.DIAG_IN_SAFETY_EVENT > 0
+        unpack_to['waiting_on_sync'] = unpack_to['diag'] & self.DIAG_WAITING_ON_SYNC > 0
+        unpack_to['in_sync_mode'] = unpack_to['diag'] & self.DIAG_IN_SYNC_MODE > 0
+        if unpack_to['diag'] & self.DIAG_TRAJ_WAITING_ON_SYNC > 0:
+            unpack_to['waypoint_traj']['state']='waiting_on_sync'
+        elif unpack_to['diag'] & self.DIAG_TRAJ_ACTIVE > 0:
+            unpack_to['waypoint_traj']['state']='active'
+        else:
+            unpack_to['waypoint_traj']['state']='idle'
+
+        return sidx
 
     def pretty_print(self):
         print('-----------')
         print('Mode', self.MODE_NAMES[self.status['mode']])
         print('x_des (rad)', self._command['x_des'], '(deg)',rad_to_deg(self._command['x_des']))
         print('v_des (rad)', self._command['v_des'], '(deg)',rad_to_deg(self._command['v_des']))
         print('a_des (rad)', self._command['a_des'], '(deg)',rad_to_deg(self._command['a_des']))
@@ -909,20 +974,21 @@
         print('       At Current Limit:', self.status['at_current_limit'])
         print('       Is MG Accelerating:', self.status['is_mg_accelerating'])
         print('       Is MG Moving:', self.status['is_mg_moving'])
         print('       Encoder Calibration in Flash:', self.status['calibration_rcvd'])
         print('       In Guarded Event:', self.status['in_guarded_event'])
         print('       In Safety Event:', self.status['in_safety_event'])
         print('       Waiting on Sync:', self.status['waiting_on_sync'])
+        print('       Trace recording:', self.status['trace_on'])
         print('Waypoint Trajectory')
         print('       State:', self.status['waypoint_traj']['state'])
         print('       Setpoint: (rad) %s | (deg) %s'%(self.status['waypoint_traj']['setpoint'],  rad_to_deg(self.status['waypoint_traj']['setpoint'])))
         print('       Segment ID:', self.status['waypoint_traj']['segment_id'])
         print('Timestamp (s)', self.status['timestamp'])
-        print('Read error', self.transport.status['read_error'])
+        #print('Read error', self.transport.status['read_error'])
         print('Board variant:', self.board_info['board_variant'])
         print('Firmware version:', self.board_info['firmware_version'])
 
     def enable_pos_traj_waypoint(self):
         self.set_command(mode=self.MODE_POS_TRAJ_WAYPOINT)
 
     def start_waypoint_trajectory(self, first_segment):
@@ -942,24 +1008,24 @@
             True if uC successfully initiated a new trajectory
         """
         if len(first_segment) != 8:
             self.logger.warning('start_waypoint_trajectory: Invalid segment arr length (must be 8)')
             return False
         self._waypoint_traj_segment = first_segment
         self._waypoint_ts = time.time()
-        with self.lock:
-            if self._waypoint_traj_segment is not None:
-                self.transport.payload_out[0] = self.RPC_START_NEW_TRAJECTORY
-                sidx = self.pack_trajectory_segment(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_start_new_traj_reply)
-            self.transport.step2()
-            if not self._waypoint_traj_start_success:
-                self.logger.warning('start_waypoint_trajectory: %s' % self._waypoint_traj_start_error_msg.capitalize())
-            #return self._waypoint_traj_start_success
+        if self._waypoint_traj_segment is not None:
+            payload = self.transport.get_empty_payload()
+            payload[0] = self.RPC_START_NEW_TRAJECTORY
+            sidx = self.pack_trajectory_segment(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_start_new_traj_reply)
+        if not self._waypoint_traj_start_success:
+            self.logger.warning('start_waypoint_trajectory: %s' % self._waypoint_traj_start_error_msg.capitalize())
+        # return self._waypoint_traj_start_success
         return self._waypoint_traj_start_success
+
     def set_next_trajectory_segment(self, next_segment):
         """Sets the next segment for the hardware to execute
 
         This method is generally called multiple times while the prior segment is executing. This
         provides the hardware with the next segment to gracefully transition across the entire spline,
         while allowing users to preempt or modify the future trajectory in real time.
 
@@ -978,92 +1044,293 @@
         bool
             True if uC successfully queued next trajectory
         """
         if len(next_segment) != 8:
             self.logger.warning('set_next_trajectory_segment: Invalid segment arr length (must be 8)')
             return False
         self._waypoint_traj_segment = next_segment
-        with self.lock:
-            if self._waypoint_traj_segment is not None:
-                self.transport.payload_out[0] = self.RPC_SET_NEXT_TRAJECTORY_SEG
-                sidx = self.pack_trajectory_segment(self.transport.payload_out, 1)
-                self.transport.queue_rpc2(sidx, self.rpc_set_next_traj_seg_reply)
-            self.transport.step2()
-            if not self._waypoint_traj_set_next_traj_success:
-                self.logger.warning('set_next_trajectory_segment: %s' % self._waypoint_traj_set_next_error_msg.capitalize())
-            return self._waypoint_traj_set_next_traj_success
+        if self._waypoint_traj_segment is not None:
+            payload = self.transport.get_empty_payload()
+            payload[0] = self.RPC_SET_NEXT_TRAJECTORY_SEG
+            sidx = self.pack_trajectory_segment(payload, 1)
+            self.transport.do_push_rpc_sync(payload[:sidx], self.rpc_set_next_traj_seg_reply)
+        if not self._waypoint_traj_set_next_traj_success:
+            self.logger.warning('set_next_trajectory_segment: %s' % self._waypoint_traj_set_next_error_msg.capitalize())
+        return self._waypoint_traj_set_next_traj_success
 
     def stop_waypoint_trajectory(self):
         """Stops execution of the waypoint trajectory running in hardware
         """
         self._waypoint_ts = None
-        with self.lock:
-            self.transport.payload_out[0] = self.RPC_RESET_TRAJECTORY
-            self.transport.queue_rpc2(1, self.rpc_reset_traj_reply)
-            self.transport.step2()
+        payload = arr.array('B', [self.RPC_RESET_TRAJECTORY])
+        self.transport.do_push_rpc_sync(payload, self.rpc_reset_traj_reply)
 
     def pack_trajectory_segment(self, s, sidx):
-        with self.lock:
-            for i in range(7):
-                pack_float_t(s, sidx, self._waypoint_traj_segment[i]); sidx += 4
-            pack_uint8_t(s, sidx, self._waypoint_traj_segment[7]); sidx += 1
-            return sidx
+        for i in range(7):
+            pack_float_t(s, sidx, self._waypoint_traj_segment[i]);
+            sidx += 4
+        pack_uint8_t(s, sidx, self._waypoint_traj_segment[7]);
+        sidx += 1
+        return sidx
 
     def rpc_start_new_traj_reply(self, reply):
         if reply[0] == self.RPC_REPLY_START_NEW_TRAJECTORY:
-            with self.lock:
-                sidx=1
-                self._waypoint_traj_start_success = unpack_uint8_t(reply[sidx:]); sidx += 1
-                self._waypoint_traj_start_error_msg = unpack_string_t(reply[sidx:], 100).strip('\x00'); sidx += 100
+            sidx = 1
+            self._waypoint_traj_start_success = unpack_uint8_t(reply[sidx:]);
+            sidx += 1
+            self._waypoint_traj_start_error_msg = unpack_string_t(reply[sidx:], 100).strip('\x00')
+            sidx += 100
         else:
             self.logger.error('RPC_REPLY_START_NEW_TRAJECTORY replied {0}'.format(reply[0]))
 
     def rpc_set_next_traj_seg_reply(self, reply):
         if reply[0] == self.RPC_REPLY_SET_NEXT_TRAJECTORY_SEG:
-            with self.lock:
-                sidx=1
-                self._waypoint_traj_set_next_traj_success = unpack_uint8_t(reply[sidx:]); sidx += 1
-                self._waypoint_traj_set_next_error_msg = unpack_string_t(reply[sidx:], 100).strip('\x00'); sidx += 100
+            sidx = 1
+            self._waypoint_traj_set_next_traj_success = unpack_uint8_t(reply[sidx:]);
+            sidx += 1
+            self._waypoint_traj_set_next_error_msg = unpack_string_t(reply[sidx:], 100).strip('\x00')
+            sidx += 100
         else:
             self.logger.error('RPC_REPLY_SET_NEXT_TRAJECTORY_SEG replied {0}'.format(reply[0]))
 
     def rpc_reset_traj_reply(self, reply):
         if reply[0] != self.RPC_REPLY_RESET_TRAJECTORY:
             self.logger.error('RPC_REPLY_RESET_TRAJECTORY replied {0}'.format(reply[0]))
 
 
+# ######################## STEPPER PROTOCOL P2 #################################
+class Stepper_Protocol_P2(StepperBase):
+
+    def read_firmware_trace(self):
+        self.trace_buf = []
+        self.timestamp.reset() #Timestamp holds state, reset within lock to avoid threading issues
+        self.n_trace_read=1
+        ts=time.time()
+        while ( self.n_trace_read) and time.time()-ts<60.0:
+            payload = arr.array('B', [self.RPC_READ_TRACE])
+            self.transport.do_pull_rpc_sync(payload, self.rpc_read_firmware_trace_reply)
+            time.sleep(.001)
+        return self.trace_buf
+    def unpack_debug_trace(self,s,unpack_to):
+        sidx=0
+        unpack_to['u8_1']=unpack_uint8_t(s[sidx:]);sidx+=1
+        unpack_to['u8_2'] = unpack_uint8_t(s[sidx:]);sidx += 1
+        unpack_to['f_1'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['f_2'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['f_3'] = unpack_float_t(s[sidx:]);sidx += 4
+        return sidx
+
+    def unpack_print_trace(self,s,unpack_to):
+        sidx=0
+        line_len=32
+        unpack_to['timestamp']=self.timestamp.set(unpack_uint64_t(s[sidx:]));sidx += 8
+        unpack_to['line'] = unpack_string_t(s[sidx:], line_len); sidx += line_len
+        unpack_to['x'] = unpack_float_t(s[sidx:]);sidx += 4
+        return sidx
+    def rpc_read_firmware_trace_reply(self, reply):
+        if len(reply)>0 and reply[0] == self.RPC_REPLY_READ_TRACE:
+            self.n_trace_read=reply[1]
+            self.trace_buf.append({'id': len(self.trace_buf), 'status': {},'debug':{},'print':{}})
+            if reply[2]==self.TRACE_TYPE_STATUS:
+                self.trace_buf[-1]['status']= self.status_zero.copy()
+                self.unpack_status(reply[3:],unpack_to=self.trace_buf[-1]['status'])
+            elif reply[2]==self.TRACE_TYPE_DEBUG:
+                self.unpack_debug_trace(reply[3:],unpack_to=self.trace_buf[-1]['debug'])
+            elif reply[2]==self.TRACE_TYPE_PRINT:
+                self.unpack_print_trace(reply[3:],unpack_to=self.trace_buf[-1]['print'])
+            else:
+                print('Unrecognized trace type %d'%reply[2])
+        else:
+            print('Error RPC_REPLY_READ_TRACE')
+            self.n_trace_read=0
+            self.trace_buf = []
+    def enable_firmware_trace(self):
+        self._trigger = self._trigger | self.TRIGGER_ENABLE_TRACE
+        self._dirty_trigger = True
+
+    def disable_firmware_trace(self):
+        self._trigger = self._trigger | self.TRIGGER_DISABLE_TRACE
+        self._dirty_trigger = True
+
+
+    def unpack_status(self,s,unpack_to=None):
+        if unpack_to is None:
+            unpack_to=self.status
+        sidx=0
+        unpack_to['mode']=unpack_uint8_t(s[sidx:]);sidx+=1
+        unpack_to['effort_ticks'] = unpack_float_t(s[sidx:]);sidx+=4
+        unpack_to['current']=self.effort_ticks_to_current(unpack_to['effort_ticks'])
+        unpack_to['effort_pct'] = self.current_to_effort_pct(unpack_to['current'])
+        unpack_to['pos'] = unpack_double_t(s[sidx:]);sidx+=8
+        unpack_to['vel'] = unpack_float_t(s[sidx:]);sidx+=4
+        unpack_to['err'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['diag'] = unpack_uint32_t(s[sidx:]);sidx += 4
+        unpack_to['timestamp'] = self.timestamp.set(unpack_uint64_t(s[sidx:]));sidx += 8
+        unpack_to['debug'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['guarded_event'] = unpack_uint32_t(s[sidx:]);sidx += 4
+        unpack_to['waypoint_traj']['setpoint'] = unpack_float_t(s[sidx:]);sidx += 4
+        unpack_to['waypoint_traj']['segment_id'] = unpack_uint16_t(s[sidx:]);sidx += 2
+
+        unpack_to['pos_calibrated'] =unpack_to['diag'] & self.DIAG_POS_CALIBRATED > 0
+        unpack_to['runstop_on'] =unpack_to['diag'] & self.DIAG_RUNSTOP_ON > 0
+        unpack_to['near_pos_setpoint'] =unpack_to['diag'] & self.DIAG_NEAR_POS_SETPOINT > 0
+        unpack_to['near_vel_setpoint'] = unpack_to['diag'] & self.DIAG_NEAR_VEL_SETPOINT > 0
+        unpack_to['is_moving'] =unpack_to['diag'] & self.DIAG_IS_MOVING > 0
+        unpack_to['at_current_limit'] =unpack_to['diag'] & self.DIAG_AT_CURRENT_LIMIT > 0
+        unpack_to['is_mg_accelerating'] = unpack_to['diag'] & self.DIAG_IS_MG_ACCELERATING > 0
+        unpack_to['is_mg_moving'] =unpack_to['diag'] & self.DIAG_IS_MG_MOVING > 0
+        unpack_to['calibration_rcvd'] = unpack_to['diag'] & self.DIAG_CALIBRATION_RCVD > 0
+        unpack_to['in_guarded_event'] = unpack_to['diag'] & self.DIAG_IN_GUARDED_EVENT > 0
+        unpack_to['in_safety_event'] = unpack_to['diag'] & self.DIAG_IN_SAFETY_EVENT > 0
+        unpack_to['waiting_on_sync'] = unpack_to['diag'] & self.DIAG_WAITING_ON_SYNC > 0
+        unpack_to['in_sync_mode'] = unpack_to['diag'] & self.DIAG_IN_SYNC_MODE > 0
+        unpack_to['trace_on'] = unpack_to['diag'] & self.DIAG_IS_TRACE_ON > 0
+
+        if unpack_to['diag'] & self.DIAG_TRAJ_WAITING_ON_SYNC > 0:
+            unpack_to['waypoint_traj']['state']='waiting_on_sync'
+        elif unpack_to['diag'] & self.DIAG_TRAJ_ACTIVE > 0:
+            unpack_to['waypoint_traj']['state']='active'
+        else:
+            unpack_to['waypoint_traj']['state']='idle'
+
+        return sidx
+
+# ######################## STEPPER PROTOCOL P3 #################################
+
+class Stepper_Protocol_P3(StepperBase):
+
+    def rpc_start_new_traj_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_START_NEW_TRAJECTORY:
+            self._waypoint_traj_start_success = unpack_uint8_t(reply[1:])
+            self._waypoint_traj_start_error_msg = 'SUCCESS' if self._waypoint_traj_start_success else 'FAIL'
+        else:
+            self.logger.error('RPC_REPLY_START_NEW_TRAJECTORY replied {0}'.format(reply[0]))
+
+    def rpc_set_next_traj_seg_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_SET_NEXT_TRAJECTORY_SEG:
+            self._waypoint_traj_set_next_traj_success = unpack_uint8_t(reply[1:])
+            self._waypoint_traj_set_next_traj_success = 'SUCCESS' if self._waypoint_traj_start_success else 'FAIL'
+        else:
+            self.logger.error('RPC_REPLY_SET_NEXT_TRAJECTORY_SEG replied {0}'.format(reply[0]))
+
+    def push_load_test(self):
+        if not self.hw_valid:
+            return
+        payload = self.transport.get_empty_payload()
+        payload[0] = self.RPC_LOAD_TEST_PUSH
+        payload[1:] = self.load_test_payload
+        self.transport.do_push_rpc_sync(payload, self.rpc_load_test_push_reply)
+
+    def pull_load_test(self):
+        if not self.hw_valid:
+            return
+        payload = arr.array('B',[self.RPC_LOAD_TEST_PULL])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_load_test_pull_reply)
+
+    def rpc_load_test_push_reply(self, reply):
+        if reply[0] != self.RPC_REPLY_LOAD_TEST_PUSH:
+            print('Error RPC_REPLY_LOAD_TEST_PUSH', reply[0])
+
+    def rpc_load_test_pull_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_LOAD_TEST_PULL:
+            d = reply[1:]
+            for i in range(1024):
+                if d[i] != self.load_test_payload[(i + 1) % 1024]:
+                    print('Load test pull bad data', d[i], self.load_test_payload[(i + 1) % 1024])
+            self.load_test_payload = d
+            print('Successful load test pull')
+        else:
+            print('Error RPC_REPLY_LOAD_TEST_PULL', reply[0])
+
+    def pull_status_aux(self):
+        if not self.hw_valid:
+            return
+        payload = arr.array('B',[self.RPC_GET_STATUS_AUX])
+        self.transport.do_pull_rpc_sync(payload, self.rpc_status_aux_reply)
+
+    def unpack_status_aux(self,s):
+        sidx = 0
+        self.status_aux['cmd_cnt_rpc'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        self.status_aux['cmd_cnt_exec'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        self.status_aux['cmd_rpc_overflow'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        self.status_aux['sync_irq_cnt'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        self.status_aux['sync_irq_overflow'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        return sidx
+
+    def rpc_status_aux_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_STATUS_AUX:
+            nr = self.unpack_status_aux(reply[1:])
+        else:
+            print('Error RPC_REPLY_STATUS', reply[0])
+
+
+    def unpack_command_reply(self,s):
+        sidx = 0
+        self.status['ctrl_cycle_cnt'] = unpack_uint16_t(s[sidx:])
+        sidx += 2
+        return sidx
+
+    def rpc_command_reply(self, reply):
+        if reply[0] == self.RPC_REPLY_COMMAND:
+            nr = self.unpack_command_reply(reply[1:])
+        else:
+            print('Error RPC_REPLY_COMMAND', reply[0])
+
 # ######################## STEPPER #################################
 class Stepper(StepperBase):
     """
     API to the Stretch Stepper Board
     """
-    def __init__(self,usb):
-        StepperBase.__init__(self,usb)
+    def __init__(self,usb, name=None):
+        StepperBase.__init__(self,usb,name)
         # Order in descending order so more recent protocols/methods override less recent
-        self.supported_protocols = {'p0': (Stepper_Protocol_P0,), 'p1': (Stepper_Protocol_P1,Stepper_Protocol_P0,)}
-
+        self.supported_protocols = {'p0': (Stepper_Protocol_P0,),
+                                    'p1': (Stepper_Protocol_P1,Stepper_Protocol_P0,),
+                                    'p2': (Stepper_Protocol_P2,Stepper_Protocol_P1,Stepper_Protocol_P0,),
+                                    'p3': (Stepper_Protocol_P3,Stepper_Protocol_P2,Stepper_Protocol_P1,Stepper_Protocol_P0,)}
+    
+    def expand_protocol_methods(self, protocol_class):
+        for attr_name, attr_value in protocol_class.__dict__.items():
+            if callable(attr_value) and not attr_name.startswith("__"):
+                setattr(self, attr_name, attr_value.__get__(self, Stepper))
+                
     def startup(self, threaded=False):
         """
         First determine which protocol version the uC firmware is running.
-        Based on that version, replaces PimuBase class inheritance with a inheritance to a child class of PimuBase that supports that protocol
+        Based on that version, populates Stepper class with the supported specific Stepper_protocol_P* class methods.
         """
         StepperBase.startup(self, threaded=threaded)
         if self.hw_valid:
             if self.board_info['protocol_version'] in self.supported_protocols:
-                Stepper.__bases__ = self.supported_protocols[self.board_info['protocol_version']]
+                protocol_classes = self.supported_protocols[self.board_info['protocol_version']]
+                for p in protocol_classes[::-1]:
+                    self.expand_protocol_methods(p)
             else:
-                protocol_msg = """
-                ----------------
-                Firmware protocol mismatch on {0}.
-                Protocol on board is {1}.
-                Valid protocols are: {2}.
-                Disabling device.
-                Please upgrade the firmware and/or version of Stretch Body.
-                ----------------
-                """.format(self.name, self.board_info['protocol_version'], self.supported_protocols.keys())
+                if self.board_info['protocol_version'] is None:
+                    protocol_msg = """
+                                    ----------------
+                                    Failure in communications for {0} on startup.
+                                    Please power cycle the robot and try again.
+                                    ----------------
+                                    """.format(self.name)
+                else:
+                    protocol_msg = """
+                    ----------------
+                    Firmware protocol mismatch on {0}.
+                    Protocol on board is {1}.
+                    Valid protocols are: {2}.
+                    Disabling device.
+                    Please upgrade the firmware and/or version of Stretch Body.
+                    ----------------
+                    """.format(self.name, self.board_info['protocol_version'], self.supported_protocols.keys())
                 self.logger.warning(textwrap.dedent(protocol_msg))
                 self.hw_valid = False
                 self.transport.stop()
 
         if self.hw_valid:
             self.enable_safety()
             self._dirty_gains = True
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/stretch_gripper.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/stretch_gripper.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     """
     API to the Stretch Gripper
     The StretchGripper motion is non-linear w.r.t to motor motion due to its design
     As such, the position of the gripper is represented at as unit-less value, 'pct'
     The Pct ranges from approximately -100 (fully closed) to approximately +50 (fully open)
     A Pct of zero is the fingertips just touching
     """
-    def __init__(self, chain=None):
-        DynamixelHelloXL430.__init__(self, 'stretch_gripper', chain)
+    def __init__(self, chain=None, usb=None):
+        DynamixelHelloXL430.__init__(self, 'stretch_gripper', chain, usb)
         self.status['pos_pct']= 0.0
         self.pct_max_open=self.world_rad_to_pct(self.ticks_to_world_rad(self.params['range_t'][1])) #May be a bit greater than 50 given non-linear calibration
         self.poses = {'zero': 0,
                       'open': self.pct_max_open,
                       'close': -100}
 
     def startup(self, threaded=True):
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/trajectories.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/trajectories.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,14 +670,15 @@
 
         Returns
         -------
         Tuple(bool, str)
             whether the segment is valid, and error message if not
         """
         # only check if valid if there are enough waypoints
+
         if len(self.waypoints) < 2:
             return True, "must have at least two waypoints"
 
         # verify that spline starts at time zero
         if not np.isclose(self.waypoints[0].time, 0.0, atol=WAYPOINT_ISCLOSE_ATOL):
             return False, "first waypoint must be planned for time zero"
 
@@ -706,8 +707,18 @@
             success, v_max, a_max =hu.is_segment_feasible(ls.to_array(), v_des, a_des)
             if not success:
                 return False, "left wheel segment %d exceeds dynamic bounds of (%f vel | %f acc ) with max of (%f vel | %f acc )"%(i,v_des,a_des,v_max,a_max)
             success, v_max, a_max =hu.is_segment_feasible(rs.to_array(), v_des, a_des)
             if not success:
                 return False, "right wheel segment %d exceeds dynamic bounds of (%f vel | %f acc ) with max of (%f vel | %f acc )"%(i,v_des,a_des,v_max,a_max)
 
+        # verify that either translate or rotate only at a time
+        for i in range(1,len(self.waypoints)):
+            dx=self.waypoints[i].pose[0]-self.waypoints[i-1].pose[0]
+            dy = self.waypoints[i].pose[1] - self.waypoints[i-1].pose[1]
+            dtheta = self.waypoints[i].pose[2] - self.waypoints[i-1].pose[2]
+            translating = (not np.isclose(dx, 0.0, atol=WAYPOINT_ISCLOSE_ATOL)) or (not np.isclose(dy, 0.0, atol=WAYPOINT_ISCLOSE_ATOL))
+            rotating = (not np.isclose(dtheta, 0.0, atol=WAYPOINT_ISCLOSE_ATOL))
+            if translating and rotating:
+                return False, 'DiffDriveTrajectory waypoint cannot both translate and rotate: \n%s'%str(self.waypoints[i])
+
         return True, ""
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/wrist_yaw.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/wrist_yaw.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import time
 
 
 class WristYaw(DynamixelHelloXL430):
     """
     API to the Stretch wrist yaw joint
     """
-    def __init__(self, chain=None):
-        DynamixelHelloXL430.__init__(self, 'wrist_yaw', chain)
+    def __init__(self, chain=None, usb=None):
+        DynamixelHelloXL430.__init__(self, 'wrist_yaw', chain, usb)
         self.poses = {'side': deg_to_rad(90.0),
                       'forward': deg_to_rad(0.0),
                       'stow': deg_to_rad(180.0)}
 
     def startup(self, threaded=True):
         return DynamixelHelloXL430.startup(self, threaded=threaded)
```

### Comparing `hello_robot_stretch_body-0.4.9/stretch_body/xbox_controller.py` & `hello_robot_stretch_body-0.5.0.dev0/stretch_body/xbox_controller.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_arm.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_base.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_collisions.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_collisions.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_device.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_dxl_comms.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_dxl_comms.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_dynamixel_XL430.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_end_of_arm.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_end_of_arm_tools.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_head.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_hello_utils.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_hello_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 import stretch_body.hello_utils
 
 import time
 import math
 import random
 import warnings
+from collections import defaultdict
 
 
 class TestHelloUtils(unittest.TestCase):
 
     def test_yaml_file_released(self):
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter("always")
@@ -25,49 +26,76 @@
         self.assertEqual(read_params1, {})
 
     def test_overwriting_params(self):
         """Test the behavior of the overwrite_dict method.
         """
         dee1 = {'param1': 1}
         der1 = {'param2': 2}
-        stretch_body.hello_utils.overwrite_dict(dee1, der1)
+        no_mismatches1 = stretch_body.hello_utils.overwrite_dict(dee1, der1)
         self.assertEqual(dee1, {'param1': 1, 'param2': 2})
+        self.assertTrue(no_mismatches1)
 
         dee2 = {'param1': 'to_override'}
         der2 = {'param1': 'over'}
-        stretch_body.hello_utils.overwrite_dict(dee2, der2)
+        no_mismatches2 = stretch_body.hello_utils.overwrite_dict(dee2, der2)
         self.assertEqual(dee2, {'param1': 'over'})
+        self.assertTrue(no_mismatches2)
 
         dee3 = {'param1': {'motion': 'to_override', 'no_change': 1}}
         der3 = {'param1': {'motion': 'over'}}
-        stretch_body.hello_utils.overwrite_dict(dee3, der3)
+        no_mismatches3 = stretch_body.hello_utils.overwrite_dict(dee3, der3)
         self.assertEqual(dee3, {'param1': {'motion': 'over', 'no_change': 1}})
+        self.assertTrue(no_mismatches3)
 
         dee4 = {'param1': {'motion': 'same', 'no_change': 1}}
         der4 = {'param1': {'motion': {}}}
-        stretch_body.hello_utils.overwrite_dict(dee4, der4)
+        no_mismatches4 = stretch_body.hello_utils.overwrite_dict(dee4, der4)
         self.assertEqual(dee4, {'param1': {'motion': 'same', 'no_change': 1}})
+        self.assertFalse(no_mismatches4)
 
         dee5 = {'param1': {'motion': {}, 'no_change': 1}}
         der5 = {'param1': {'motion': 2}}
-        stretch_body.hello_utils.overwrite_dict(dee5, der5)
+        no_mismatches5 = stretch_body.hello_utils.overwrite_dict(dee5, der5)
         self.assertEqual(dee5, {'param1': {'motion': {}, 'no_change': 1}})
+        self.assertFalse(no_mismatches5)
+
+        dee6 = {'param1': {'motion': 1}}
+        der6 = {'param1': {'motion': 'stringtype'}}
+        no_mismatches6 = stretch_body.hello_utils.overwrite_dict(dee6, der6)
+        self.assertEqual(dee6, {'param1': {'motion': 1}})
+        self.assertFalse(no_mismatches6)
+
+        # int and float and overwrite each other
+        dee7 = {'param1': {'motion': 1}}
+        der7 = {'param1': {'motion': 2.0}}
+        no_mismatches7 = stretch_body.hello_utils.overwrite_dict(dee7, der7)
+        self.assertEqual(dee7, {'param1': {'motion': 2.0}})
+        self.assertTrue(no_mismatches7)
+
+        dee8 = {'param1': {'param2': 0}}
+        param2dict = defaultdict()
+        param2dict['param2'] = 2
+        der8 = {'param1': param2dict}
+        no_mismatches8 = stretch_body.hello_utils.overwrite_dict(dee8, der8)
+        self.assertEqual(dee8, {'param1': {'param2': 2}})
+        self.assertTrue(no_mismatches8)
 
     def test_overwriting_vs_updating_params(self):
         """Verify the difference between overwrite_dict and updating a dict.
         """
-        overider1 = {"robot": {"motion": {"max": 100}}}
         overidee1 = {"robot": {"motion": {"min": -100}}}
-        stretch_body.hello_utils.overwrite_dict(overidee1, overider1)
+        overider1 = {"robot": {"motion": {"max": 100}}}
+        no_mismatches1 = stretch_body.hello_utils.overwrite_dict(overidee1, overider1)
         self.assertEqual(overidee1, {"robot": {"motion": {"max": 100, "min": -100}}})
+        self.assertTrue(no_mismatches1)
 
-        overider2 = {"robot": {"motion": {"max": 100}}}
         overidee2 = {"robot": {"motion": {"min": -100}}}
+        overider2 = {"robot": {"motion": {"max": 100}}}
         overidee2.update(overider2)
-        self.assertNotEqual(overidee1, overidee2)
+        self.assertNotEqual(overidee2, {"robot": {"motion": {"max": 100, "min": -100}}})
 
     def test_pretty_print_dict(self):
         dict1 = {"param1": 1, "param2": 2}
         stretch_body.hello_utils.pretty_print_dict("params", dict1)
 
         dict2 = {"robot": {"motion": {"max": 100, "min": -100}, "retry": True}}
         stretch_body.hello_utils.pretty_print_dict("Stretch", dict2)
```

### Comparing `hello_robot_stretch_body-0.4.9/test/test_lift.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_pimu.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_robot.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_robot_params.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_steppers.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_steppers.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_stretch_gripper.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_sync.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_timing_stats.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_timing_stats.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_trajectories.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.9/test/test_wrist_yaw.py` & `hello_robot_stretch_body-0.5.0.dev0/test/test_wrist_yaw.py`

 * *Files identical despite different names*

