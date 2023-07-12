# Comparing `tmp/mecademicpy-1.3.0.tar.gz` & `tmp/mecademicpy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecademicpy-1.3.0.tar", last modified: Wed Nov 23 16:50:02 2022, max compression
+gzip compressed data, was "mecademicpy-1.4.0.tar", last modified: Wed Jul 12 13:43:04 2023, max compression
```

## Comparing `mecademicpy-1.3.0.tar` & `mecademicpy-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 16:50:02.318842 mecademicpy-1.3.0/
--rw-rw-rw-   0        0        0     1087 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/LICENSE
--rw-rw-rw-   0        0        0    17439 2022-11-23 16:50:02.318842 mecademicpy-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    16952 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-23 16:50:02.287611 mecademicpy-1.3.0/mecademicpy/
--rw-rw-rw-   0        0        0        0 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/__init__.py
--rw-rw-rw-   0        0        0   121307 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/_robot_base.py
--rw-rw-rw-   0        0        0    13127 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/_robot_trajectory_logger.py
--rw-rw-rw-   0        0        0    63661 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/mx_robot_def.py
--rw-rw-rw-   0        0        0    54292 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/mx_robot_def_legacy.py
--rw-rw-rw-   0        0        0    92409 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/robot.py
--rw-rw-rw-   0        0        0    41709 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/robot_classes.py
--rw-rw-rw-   0        0        0    15931 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/robot_trajectory_files.py
--rw-rw-rw-   0        0        0     3336 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/mecademicpy/tools.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:50:02.308843 mecademicpy-1.3.0/mecademicpy.egg-info/
--rw-rw-rw-   0        0        0    17439 2022-11-23 16:50:02.000000 mecademicpy-1.3.0/mecademicpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2022-11-23 16:50:02.000000 mecademicpy-1.3.0/mecademicpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 16:50:02.000000 mecademicpy-1.3.0/mecademicpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-11-23 16:50:02.000000 mecademicpy-1.3.0/mecademicpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-23 16:50:02.000000 mecademicpy-1.3.0/mecademicpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-23 16:50:02.318842 mecademicpy-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1146 2022-11-23 16:49:46.000000 mecademicpy-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:43:04.398704 mecademicpy-1.4.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    17404 2023-07-12 13:43:04.398704 mecademicpy-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16917 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 13:43:04.378709 mecademicpy-1.4.0/mecademicpy/
+-rw-rw-rw-   0        0        0        0 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/__init__.py
+-rw-rw-rw-   0        0        0   147994 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/_robot_base.py
+-rw-rw-rw-   0        0        0    15831 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/_robot_trajectory_logger.py
+-rw-rw-rw-   0        0        0    73109 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/mx_robot_def.py
+-rw-rw-rw-   0        0        0    62614 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/mx_robot_def_legacy.py
+-rw-rw-rw-   0        0        0   108711 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/robot.py
+-rw-rw-rw-   0        0        0    49948 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/robot_classes.py
+-rw-rw-rw-   0        0        0    15931 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/robot_trajectory_files.py
+-rw-rw-rw-   0        0        0     5544 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/mecademicpy/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:43:04.398704 mecademicpy-1.4.0/mecademicpy.egg-info/
+-rw-rw-rw-   0        0        0    17404 2023-07-12 13:43:04.000000 mecademicpy-1.4.0/mecademicpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-12 13:43:04.000000 mecademicpy-1.4.0/mecademicpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:43:04.000000 mecademicpy-1.4.0/mecademicpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-12 13:43:04.000000 mecademicpy-1.4.0/mecademicpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 13:43:04.000000 mecademicpy-1.4.0/mecademicpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:43:04.398704 mecademicpy-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-07-12 13:42:39.000000 mecademicpy-1.4.0/setup.py
```

### Comparing `mecademicpy-1.3.0/LICENSE` & `mecademicpy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecademicpy-1.3.0/PKG-INFO` & `mecademicpy-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: mecademicpy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A package to control the Mecademic robots through python
 Home-page: https://github.com/Mecademic/mecademicpy
 Author: Mecademic
 Author-email: support@mecademic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.jpg?raw=true  "Mecademic")
+![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.png?raw=true  "Mecademic")
 # Mecademic Python API
 
-A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products. 
+A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products.
 
 #### Supported Robots
 
- * Meca500 R2, R3
+ * Meca500, Mcs500
 
 #### Supported Firmware Versions
 
  * 8.3 and up
 
 ## Prerequisites
 
-Please read the [user programming manual](https://mecademic.com/resources/documentation) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
+Please read the [user programming manual](https://www.mecademic.com/support/) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
 
 To be able to use the module without unexpected errors, the user must have a copy of python installed on their machine and it is required to use python version 3.7 or higher. We recommend using Python 3.9 since this is the version on which this module is actively tested. [Python](https://www.python.org/) can be installed from its main website (a reboot will be require after the installation to complete the setup).
 
 The user can validate their python installation by running `python --version` in a terminal.
 
 This library is compatible with Windows, Linux, and Mac.
 
 ## Downloading the package
 
 To download and install the package, the user can easily do so through pip. Pip will download and install the package on your machine and place it in the python local packages directory. This is done by running the following command:
 
 ```
 pip install mecademicpy
-``` 
+```
 
 ## Quick Start
 
 **Ensure the robot is properly connected to the computer, powered on, and in a nominal state.**
 
 In a python shell or script, import the library. Then initialize an instance of the `Robot` class. Finally, use the `Connect` function by passing the IP Address of the robot as an argument to establish a connection:
 
 ```python
 import mecademicpy.robot as mdr
 robot = mdr.Robot()
 robot.Connect(address='192.168.0.100')
 ```
 
 The `Connect` function will raise if connection with robot fails.
-This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode). 
+This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode).
 
 Before using the robot, it must be activated and homed. To do so, run the following functions:
 
 ```python
 robot.ActivateRobot()
 robot.Home()
 ```
 
-The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done. 
+The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done.
 
-Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://mecademic.com/resources/documentation) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot. 
+Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://www.mecademic.com/support/) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot.
 
 Here is an example of a simple motion to perform:
 
 ```python
 robot.MoveJoints(0, 0, 0, 0, 0, 0)
 robot.MoveJoints(0, -60, 60, 0, 0, 0)
 ```
@@ -239,27 +239,27 @@
 robot.ResetError()
 ```
 
 It is recommended to use `GetStatusRobot()` to learn about the current robot status and reset the relevant flags to an appropriate state before resuming operation. For example, an error may require to call `ResumeMotion()`. In this case, verify that `GetStatusRobot().pause_motion_status` is set to `True` before calling `ResumeMotion()`.
 
 The `on_error` callback can also be used to manage robot errors.
 
-Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception. 
+Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception.
 
 If the user is waiting on an event or checkpoint that the `Robot` class later determines will never occur, the event will unblock and raise an exception. For example, if the user is waiting on a checkpoint (`WaitCheckpoint`), but calls `Disconnect()` or `ClearMotion()` before the checkpoint is received, the checkpoint will unblock and raise an exception. Events and checkpoints will also unblock with exception on robot error state.
 
 The user should use python's built-in `try...except` blocks to handle appropriate exceptions.
 
 ### Preserved State on Disconnection
 
-Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot. 
+Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot.
 
 ### Logging Data to File
 
-It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context. 
+It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context.
 
 An example usage of `StartLogging` and `EngLogging`:
 
 ```python
 robot.WaitIdle()
 robot.WaitEndOfCycle()
 robot.StartLogging(0.001)
@@ -288,27 +288,27 @@
     robot.WaitIdle()
 ```
 
 The `FileLogger` context will automatically end logging after either completing the `with` block or encountering an exception.
 
 The user can select which fields to log using the `fields` parameter in `StartLogging` or `FileLogger`. By default, all available fields are logged. The available fields are currently:
 
-- `"TargetJointPos"` 
+- `"TargetJointPos"`
 - `"TargetCartPos"`
 - `"TargetJointVel"`
 - `"TargetCartVel"`
 - `"TargetConf"`
 - `"TargetConfTurn"`
 
 - `"JointPos"`
 - `"CartPos"`
-- `"JointVel"` 
-- `"JointTorq"` 
-- `"CartVel"` 
-- `"Conf"` 
+- `"JointVel"`
+- `"JointTorq"`
+- `"CartVel"`
+- `"Conf"`
 - `"ConfTurn"`
 
 - `"Accel"`
 
 
 These strings should be placed into the list given to the `fields` parameter.
 
@@ -359,11 +359,11 @@
 
 To get support, you can start an issue on the Mecademic github page, issues section or send an email to support@mecademic.com.
 
 ## License
 
 All packages in this repository are licensed under the MIT license.
 
-## Authors 
+## Authors
 
 * **Mecademic** - *Continuous work*
```

### Comparing `mecademicpy-1.3.0/README.md` & `mecademicpy-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.jpg?raw=true  "Mecademic")
+![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.png?raw=true  "Mecademic")
 # Mecademic Python API
 
-A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products. 
+A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products.
 
 #### Supported Robots
 
- * Meca500 R2, R3
+ * Meca500, Mcs500
 
 #### Supported Firmware Versions
 
  * 8.3 and up
 
 ## Prerequisites
 
-Please read the [user programming manual](https://mecademic.com/resources/documentation) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
+Please read the [user programming manual](https://www.mecademic.com/support/) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
 
 To be able to use the module without unexpected errors, the user must have a copy of python installed on their machine and it is required to use python version 3.7 or higher. We recommend using Python 3.9 since this is the version on which this module is actively tested. [Python](https://www.python.org/) can be installed from its main website (a reboot will be require after the installation to complete the setup).
 
 The user can validate their python installation by running `python --version` in a terminal.
 
 This library is compatible with Windows, Linux, and Mac.
 
 ## Downloading the package
 
 To download and install the package, the user can easily do so through pip. Pip will download and install the package on your machine and place it in the python local packages directory. This is done by running the following command:
 
 ```
 pip install mecademicpy
-``` 
+```
 
 ## Quick Start
 
 **Ensure the robot is properly connected to the computer, powered on, and in a nominal state.**
 
 In a python shell or script, import the library. Then initialize an instance of the `Robot` class. Finally, use the `Connect` function by passing the IP Address of the robot as an argument to establish a connection:
 
 ```python
 import mecademicpy.robot as mdr
 robot = mdr.Robot()
 robot.Connect(address='192.168.0.100')
 ```
 
 The `Connect` function will raise if connection with robot fails.
-This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode). 
+This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode).
 
 Before using the robot, it must be activated and homed. To do so, run the following functions:
 
 ```python
 robot.ActivateRobot()
 robot.Home()
 ```
 
-The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done. 
+The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done.
 
-Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://mecademic.com/resources/documentation) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot. 
+Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://www.mecademic.com/support/) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot.
 
 Here is an example of a simple motion to perform:
 
 ```python
 robot.MoveJoints(0, 0, 0, 0, 0, 0)
 robot.MoveJoints(0, -60, 60, 0, 0, 0)
 ```
@@ -224,27 +224,27 @@
 robot.ResetError()
 ```
 
 It is recommended to use `GetStatusRobot()` to learn about the current robot status and reset the relevant flags to an appropriate state before resuming operation. For example, an error may require to call `ResumeMotion()`. In this case, verify that `GetStatusRobot().pause_motion_status` is set to `True` before calling `ResumeMotion()`.
 
 The `on_error` callback can also be used to manage robot errors.
 
-Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception. 
+Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception.
 
 If the user is waiting on an event or checkpoint that the `Robot` class later determines will never occur, the event will unblock and raise an exception. For example, if the user is waiting on a checkpoint (`WaitCheckpoint`), but calls `Disconnect()` or `ClearMotion()` before the checkpoint is received, the checkpoint will unblock and raise an exception. Events and checkpoints will also unblock with exception on robot error state.
 
 The user should use python's built-in `try...except` blocks to handle appropriate exceptions.
 
 ### Preserved State on Disconnection
 
-Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot. 
+Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot.
 
 ### Logging Data to File
 
-It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context. 
+It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context.
 
 An example usage of `StartLogging` and `EngLogging`:
 
 ```python
 robot.WaitIdle()
 robot.WaitEndOfCycle()
 robot.StartLogging(0.001)
@@ -273,27 +273,27 @@
     robot.WaitIdle()
 ```
 
 The `FileLogger` context will automatically end logging after either completing the `with` block or encountering an exception.
 
 The user can select which fields to log using the `fields` parameter in `StartLogging` or `FileLogger`. By default, all available fields are logged. The available fields are currently:
 
-- `"TargetJointPos"` 
+- `"TargetJointPos"`
 - `"TargetCartPos"`
 - `"TargetJointVel"`
 - `"TargetCartVel"`
 - `"TargetConf"`
 - `"TargetConfTurn"`
 
 - `"JointPos"`
 - `"CartPos"`
-- `"JointVel"` 
-- `"JointTorq"` 
-- `"CartVel"` 
-- `"Conf"` 
+- `"JointVel"`
+- `"JointTorq"`
+- `"CartVel"`
+- `"Conf"`
 - `"ConfTurn"`
 
 - `"Accel"`
 
 
 These strings should be placed into the list given to the `fields` parameter.
 
@@ -344,11 +344,11 @@
 
 To get support, you can start an issue on the Mecademic github page, issues section or send an email to support@mecademic.com.
 
 ## License
 
 All packages in this repository are licensed under the MIT license.
 
-## Authors 
+## Authors
 
 * **Mecademic** - *Continuous work*
```

### Comparing `mecademicpy-1.3.0/mecademicpy/_robot_base.py` & `mecademicpy-1.4.0/mecademicpy/_robot_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 import pathlib
 import queue
 import socket
 import threading
 import time
 import weakref
 from argparse import ArgumentError
-from typing import Optional
+from typing import Optional, Union
 
 import requests
 
 from .mx_robot_def import MxRobotStatusCode as mx_st
 from .mx_robot_def import *
 from .robot_classes import *
 from .tools import *
 
 _CHECKPOINT_ID_MAX_PRIVATE = 8191  # Max allowable checkpoint id, inclusive
 
 _TERMINATE = '--terminate--'
 
+_MONITORING_TIMEOUT_MS = 10000  # Max time without receiving any monitoring message from the robot
+
 
 def disconnect_on_exception(func):
     """Decorator to call disconnect if an exception is raised. Needs to be declared outside of class.
 
     Attributes
     ----------
     func : function object
@@ -67,14 +69,18 @@
         Set if gripper status is updated.
     on_external_tool_status_updated: event
         Set if external tool status has been updated.
     on_gripper_state_updated: event
         Set if gripper state has been updated.
     on_valve_state_updated: event
         Set if pneumatic module valve state has been updated.
+    on_output_state_updated: event
+        Set if digital outputs state has been updated.
+    on_input_state_updated: event
+        Set if digital inputs state has been updated.
     on_activated : event
         Set if robot is activated.
     on_deactivated : event
         Set if robot is deactivated.
     on_homed : event
         Set if robot is homed.
     on_error : event
@@ -101,14 +107,22 @@
         Set if robot is in sim mode.
     on_deactivate_sim : event
         Set if robot is not in sim mode.
     on_activate_ext_tool_sim : event
         Set if robot is in gripper sim mode.
     on_deactivate_ext_tool_sim : event
         Set if robot is not in gripper sim mode.
+    on_psu_io_sim_enabled : event
+        Set if robot psu is not in IO sim mode.
+    on_psu_io_sim_disabled : event
+        Set if robot psu is in IO sim mode.
+    on_io_sim_enabled : event
+        Set if robot IO module is not in sim mode.
+    on_io_sim_disabled : event
+        Set if robot IO module is in sim mode.
     on_activate_recovery_mode : event
         Set if robot is in recovery mode.
     on_deactivate_recovery_mode : event
         Set if robot is not in recovery mode.
     on_joints_updated : event
         Set if joint angles has been updated.
     on_pose_updated : event
@@ -134,14 +148,16 @@
 
         self.on_status_updated = InterruptableEvent()
         self.on_status_gripper_updated = InterruptableEvent()
 
         self.on_external_tool_status_updated = InterruptableEvent()
         self.on_gripper_state_updated = InterruptableEvent()
         self.on_valve_state_updated = InterruptableEvent()
+        self.on_output_state_updated = InterruptableEvent()
+        self.on_input_state_updated = InterruptableEvent()
 
         self.on_activated = InterruptableEvent()
         self.on_deactivated = InterruptableEvent()
 
         self.on_homed = InterruptableEvent()
 
         self.on_error = InterruptableEvent()
@@ -158,14 +174,19 @@
 
         self.on_activate_sim = InterruptableEvent()
         self.on_deactivate_sim = InterruptableEvent()
 
         self.on_activate_ext_tool_sim = InterruptableEvent()
         self.on_deactivate_ext_tool_sim = InterruptableEvent()
 
+        self.on_psu_io_sim_enabled = InterruptableEvent()
+        self.on_psu_io_sim_disabled = InterruptableEvent()
+        self.on_io_sim_enabled = InterruptableEvent()
+        self.on_io_sim_disabled = InterruptableEvent()
+
         self.on_activate_recovery_mode = InterruptableEvent()
         self.on_deactivate_recovery_mode = InterruptableEvent()
 
         self.on_joints_updated = InterruptableEvent()
         self.on_pose_updated = InterruptableEvent()
 
         self.on_brakes_activated = InterruptableEvent()
@@ -187,14 +208,16 @@
         self.on_deactivate_sim.set()
 
         self.on_status_updated.set()
         self.on_status_gripper_updated.set()
         self.on_external_tool_status_updated.set()
         self.on_gripper_state_updated.set()
         self.on_valve_state_updated.set()
+        self.on_output_state_updated.set()
+        self.on_input_state_updated.set()
 
         self.on_joints_updated.set()
         self.on_pose_updated.set()
         self.on_brakes_activated.set()
 
     def clear_all(self):
         """Clear all events.
@@ -315,14 +338,16 @@
         Thread used to transmit messages to the command port.
     _command_tx_queue : queue
         Queue used to temporarily store commands to be sent to the command port.
     _monitor_rx_thread : thread handle
         Thread used to receive messages from the monitor port.
     _monitor_rx_queue : queue
         Queue used to temporarily store messages from the monitor port.
+    _rx_timestamp : float
+        Last time a message was received from the robot
 
     _command_response_handler_thread : thread handle
         Thread used to read messages from the command response queue.
     _monitor_handler_thread : thread handle
         Thread used to read messages from the monitor queue.
 
     _main_lock : recursive lock object
@@ -346,14 +371,20 @@
         Stores most current gripper state
     _gripper_state_before_last_move : GripperState object
         Stores gripper state at the time a Open/Close/Move gripper command is sent
         (then used to accelerate WaitGripperMoveCompletion in case target_pos_reached is already True when its called
          because otherwise it's not possible to know if the move has completed, or not yet started)
     _valve_state: ValveState object
         Stores most current pneumatic valve state
+    _rt_psu_io_status: IoStatus object
+        Stores most current PSU IO module status
+    _rt_io_module_status: IoStatus object
+        Stores most current IO module status
+    _fw_update_status: Firmware update status
+        Stores most current firmware update status reported by the robot
     _robot_events : RobotEvents object
         Stores events related to the robot state.
 
     _file_logger : RobotDataLogger object
         Collects RobotInformation, all RobotRtData and SentCommands during determined period
     _monitoring_interval : float
         Initial monitoring interval to restore after logging session
@@ -395,14 +426,15 @@
         Most recent response to "SyncCmdQueue" (mx_st.MX_ST_SYNC_CMD_QUEUE) received from the robot
 """
 
     def __init__(self):
         """Constructor for an instance of the Robot class.
         """
         # Initialize member variables that are NOT reset by "with" block (i.e. by __enter__ and __exit__)
+        self.logger = logging.getLogger(__name__)
         self._is_initialized = False
         # (callbacks remain registered after "with" block
         self._robot_callbacks = RobotCallbacks()
         self._run_callbacks_in_separate_thread = False
         self._reset()
 
     def __del__(self):
@@ -467,35 +499,37 @@
         self._callback_thread = None
 
         self._robot_info = RobotInfo()
         self._robot_rt_data = None
         self._robot_rt_data_stable = None
         self._robot_status = RobotStatus()
         self._first_robot_status_received = False
-        self._using_json_api = False
+        self._using_legacy_json_api = False
         self._gripper_status = GripperStatus()
         self._external_tool_status = ExtToolStatus()
         self._gripper_state = GripperState()
         self._gripper_state_before_last_move = GripperState()
         self._valve_state = ValveState()
+        self._rt_psu_io_status = IoStatus()
+        self._rt_io_module_status = IoStatus()
         self._robot_events = _RobotEvents()
+        self._reset_fw_update_status()
 
         self._file_logger = None
         self._monitoring_interval = None
         self._monitoring_interval_to_restore = None
 
         self._reset_disconnect_attributes()
 
         self._enable_synchronous_mode = None
         self._disconnect_on_exception = None
 
         self._offline_mode = None
         self._monitor_mode = None
 
-        self.logger = logging.getLogger(__name__)
         self.default_timeout = DEFAULT_WAIT_TIMEOUT
 
         # Variables to hold joint positions and poses while waiting for timestamp.
         self._tmp_rt_joint_pos = None
         self._tmp_rt_cart_pos = None
 
         self._tx_sync = 0
@@ -505,22 +539,29 @@
 
         self._is_initialized = True
 
     def _reset_disconnect_attributes(self):
         self._command_rx_queue = queue.Queue()
         self._command_tx_queue = queue.Queue()
         self._monitor_rx_queue = queue.Queue()
+        self._rx_timestamp = 0
+        self._monitor_timeout_used = False
         self._custom_response_events = list()
 
         self._user_checkpoints = dict()
         self._internal_checkpoints = dict()
         self._internal_checkpoint_counter = MX_CHECKPOINT_ID_MAX + 1
 
         self._clear_motion_requests = 0
 
+    def _reset_fw_update_status(self):
+        self._fw_update_status = UpdateProgress()
+        self._fw_update_reboot_timestamp = 0.0  # Timestamp, non-zero while rebooting
+        self._fw_update_started: bool = False
+
     #####################################################################################
     # Static methods.
     #####################################################################################
 
     @staticmethod
     def _deactivate_on_exception(func, command_socket: socket.socket, *args, **kwargs):
         """Wrap input function to send deactivate signal to command_socket on exception.
@@ -609,15 +650,15 @@
             if command == _TERMINATE:
                 return
             else:
                 logger.debug(f'Socket Tx - Command: {command}')
                 robot_socket.sendall((command + '\0').encode('ascii'))
 
     @staticmethod
-    def _connect_socket(logger: logging.Logger, address: str, port: int, socket_timeout=0.1) -> socket.socket:
+    def _connect_socket(logger: logging.Logger, address: str, port: int, socket_timeout=1.0) -> socket.socket:
         """Connects to an arbitrary socket.
 
         Parameters
         ----------
         logger : logger instance
             Logger to use.
         address : string
@@ -631,66 +672,70 @@
         -------
         new_socket : socket object
             Successfully-connected socket object.
 
         """
         logger.debug(f'Attempting to connect to {address}:{port}')
 
-        connect_loops = math.ceil(socket_timeout / 0.1)
-        for _ in range(connect_loops):
+        loop_timeout_ms = 100
+        start_time = time.monotonic()
+        while True:
             # Create socket and attempt connection.
             new_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            new_socket.settimeout(100)
+            new_socket.settimeout(loop_timeout_ms / 1000)
             try:
                 new_socket.connect((address, port))
                 break
-            except (socket.timeout, TimeoutError) as e:
-                logger.debug(f'Timeout connecting to {address}:{port}, retrying in 100ms.')
-                continue
-            except ConnectionRefusedError:
-                logger.debug(f'Connection refused to {address}:{port}, retrying in 100ms.')
-                time.sleep(0.1)
-                continue
-            except Exception as exception:
-                raise TimeoutError(f'Unable to connect to {address}:{port}, exception: {exception}')
-
-        if new_socket is None:
-            raise TimeoutError(f'Timeout while connecting to {address}:{port}.')
+            except (socket.timeout, TimeoutError) as exception:
+                if (time.monotonic() - start_time) < socket_timeout:
+                    logger.debug(f'Timeout connecting to {address}:{port}, retrying now.')
+                else:
+                    raise TimeoutError(f'Unable to connect to {address}:{port}, exception: {exception}')
+            except ConnectionRefusedError as exception:
+                if (time.monotonic() - start_time) < socket_timeout:
+                    logger.debug(f'Connection refused to {address}:{port}, retrying in {loop_timeout_ms}ms.')
+                    time.sleep(loop_timeout_ms / 1000.0)
+                else:
+                    raise ConnectionRefusedError(f'Unable to connect to {address}:{port}, exception: {exception}')
 
-        logger.info(f'Connected to {address}:{port}.')
         return new_socket
 
-    @staticmethod
-    def _handle_callbacks(logger, callback_queue: _CallbackQueue, callbacks: RobotCallbacks, timeout: float = None):
-        """Runs callbacks found in callback_queue.
-
-        Parameters
-        ----------
-        logger : logger instance
-            Logger to use.
-        callback_queue : queue
-            Stores triggered callbacks.
-        callbacks : RobotCallbacks instance
-            Stores user-defined callback functions.
-        timeout : float or None
-            If none, block forever on empty queue, if 0, don't block, else block with timeout.
-        """
-        block_on_empty = (timeout != 0)
+    def _handle_callbacks(self, polling=False):
+        """Runs callbacks found in callback_queue."""
 
+        is_connected = True
         while True:
+
             # If we are not blocking on empty, return if empty.
-            if not block_on_empty and callback_queue.qsize() == 0:
+            if polling and self._callback_queue.qsize() == 0:
                 return
 
-            callback_name, data = callback_queue.get(block=block_on_empty, timeout=timeout)
+            try:
+                # Call blocking with timeout of 0.1.
+                # If polling:
+                #   we know this won't block since there is something in the queue (validated above).
+                # If not polling (i.e. we're the callback thread)
+                #   then check with short timeout and ignore the error. We do this to periodically check if the
+                #   connection was dropped, so we detect a disconnection and trigger "on_disconnected" callback
+                #   even in the case the app is never calling IsConnected
+                callback_name, data = self._callback_queue.get(block=True, timeout=0.1)
+            except Exception as e:
+                # Check if still connected
+                if is_connected:
+                    is_connected = self.IsConnected()
+                    # Continue even if no more connected so we run one last loop and get the chance to call
+                    # the "on_disconnected" callback that we may just have pushed to the queue
+                    continue
+                else:
+                    break
 
             if callback_name == _TERMINATE:
                 return
 
-            callback_function = callbacks.__dict__[callback_name]
+            callback_function = self._robot_callbacks.__dict__[callback_name]
             if callback_function is not None:
                 if data is not None:
                     callback_function(data)
                 else:
                     callback_function()
 
     #####################################################################################
@@ -721,76 +766,77 @@
         self._robot_callbacks = RobotCallbacks()
         self._run_callbacks_in_separate_thread = False
         self._callback_queue = _CallbackQueue(self._robot_callbacks)
         self._callback_thread = None
 
     def _start_callback_thread(self):
         if self._run_callbacks_in_separate_thread and self._callback_thread is None:
-            self._callback_thread = threading.Thread(target=self._handle_callbacks,
-                                                     args=(
-                                                         self.logger,
-                                                         self._callback_queue,
-                                                         self._robot_callbacks,
-                                                     ))
+            self._callback_thread = threading.Thread(target=self._handle_callbacks)
             self._callback_thread.setDaemon(True)  # Make sure thread does not prevent application from quitting
             self._callback_thread.start()
 
     def _stop_callback_thread(self):
         if self._callback_thread:
             self._callback_queue.put(_TERMINATE)
-            self._callback_thread.join(timeout=self.default_timeout)
-            self._callback_thread = None
+            if self._callback_thread != threading.current_thread():
+                self._callback_thread.join(timeout=self.default_timeout)
+                self._callback_thread = None
 
     # Robot control functions.
 
     def Connect(self,
                 address: str = MX_DEFAULT_ROBOT_IP,
                 enable_synchronous_mode: bool = False,
                 disconnect_on_exception: bool = True,
                 monitor_mode: bool = False,
                 offline_mode: bool = False,
-                timeout: float = 0.1):
+                timeout: float = 1.0):
         """See documentation in equivalent function in robot.py"""
         try:
             with self._main_lock:
 
                 if self.IsConnected():
-                    try:
-                        self._check_internal_states(refresh_monitoring_mode=True)
-                        return  # Still connected -> Do nothing
-                    except Exception:
-                        self.logger.info('Connection to robot was lost, attempting re-connection.')
+                    return  # Still connected -> Do nothing
+
+                self._custom_port = None
 
                 # Check that the ip address is valid and set address.
                 if not isinstance(address, str):
                     raise TypeError(f'Invalid IP address ({address}).')
 
                 # Check if user has specified a custom port to connect to
                 addr_port = address.split(':')
+                mode_str = "monitoring mode" if monitor_mode else "control mode"
                 if len(addr_port) > 1:
                     self._custom_port = int(addr_port[1])
                     address = addr_port[0]
-                    self.logger.info(f"Connecting to robot {address}:{self._custom_port}")
+                    if self._fw_update_reboot_timestamp == 0:  # Don't print this trace when reconnecting during firmware update
+                        self.logger.info(f"Connecting to robot {address}:{self._custom_port} ({mode_str})")
                 else:
-                    self.logger.info(f"Connecting to robot: {address}")
+                    if self._fw_update_reboot_timestamp == 0:  # Don't print this trace when reconnecting during firmware update
+                        self.logger.info(f"Connecting to robot: {address} ({mode_str})")
+
                 ipaddress.ip_address(address)
                 self._address = address
 
                 self._enable_synchronous_mode = enable_synchronous_mode
                 self._disconnect_on_exception = disconnect_on_exception
 
                 self._offline_mode = offline_mode
                 self._monitor_mode = monitor_mode
 
                 self._first_robot_status_received = False
-                self._using_json_api = False
+                self._using_legacy_json_api = False
 
                 if not self._monitor_mode:
                     self._initialize_command_socket(timeout)
                     self._initialize_command_connection()
+                else:
+                    # Activate the monitoring timeout to detect if we're no more receiving anything from the robot
+                    self._monitor_timeout_used = True
 
                 self._robot_events.clear_all()
 
                 self._robot_events.on_deactivated.set()
                 self._robot_events.on_error_reset.set()
                 self._robot_events.on_pstop2_reset.set()
                 self._robot_events.on_pstop2_resettable.set()
@@ -799,21 +845,20 @@
                 self._set_brakes_engaged(True)
 
                 self._robot_events.on_status_updated.set()
                 self._robot_events.on_status_gripper_updated.set()
                 self._robot_events.on_external_tool_status_updated.set()
                 self._robot_events.on_gripper_state_updated.set()
                 self._robot_events.on_valve_state_updated.set()
+                self._robot_events.on_output_state_updated.set()
+                self._robot_events.on_input_state_updated.set()
 
                 self._robot_events.on_joints_updated.set()
                 self._robot_events.on_pose_updated.set()
 
-                # Start callback thread if necessary
-                self._start_callback_thread()
-
             connect_to_monitoring_port = True
             if not self._monitor_mode and self._robot_info.version.major >= 8:
                 can_query_robot_info = True
 
                 if not self._robot_info.rt_message_capable:
                     # For these versions (8.3-), it is not possible to get robot information if in error.
                     self._send_custom_command('GetStatusRobot',
@@ -847,26 +892,31 @@
 
                         # Get initial monitoring interval
                         monitoring_interval_response = self._send_custom_command(
                             'GetMonitoringInterval',
                             expected_responses=[mx_st.MX_ST_GET_MONITORING_INTERVAL],
                             timeout=self.default_timeout,
                             skip_internal_check=True)
-                        self._monitoring_interval = float(monitoring_interval_response.data)
-                        self._monitoring_interval_to_restore = self._monitoring_interval
+                        if isinstance(monitoring_interval_response, Message):
+                            self._monitoring_interval = float(f'{monitoring_interval_response.data}')
+                            self._monitoring_interval_to_restore = self._monitoring_interval
 
                     # Check if this robot supports sending monitoring data on ctrl port (which we want to do to avoid
                     # race conditions between the two sockets causing potential problems with this API)
                     # Also make sure we have received a robot status event before continuing
                     if self._robot_info.rt_on_ctrl_port_capable:
                         connect_to_monitoring_port = False  # We won't need to connect to monitoring port
                         self._send_custom_command('SetCtrlPortMonitoring(1)',
                                                   expected_responses=[mx_st.MX_ST_GET_STATUS_ROBOT],
                                                   timeout=self.default_timeout,
                                                   skip_internal_check=True)
+                        # Since we're going to receive monitoring messages on the control port, we'll periodically
+                        # receive events from the robot and can thus enable the "monitor timeout" to detect that
+                        # we're disconnected from the robot if ever we no more receive any message from it
+                        self._monitor_timeout_used = True
                     else:
                         self._send_custom_command('GetStatusRobot',
                                                   expected_responses=[mx_st.MX_ST_GET_STATUS_ROBOT],
                                                   timeout=self.default_timeout,
                                                   skip_internal_check=True)
 
             if connect_to_monitoring_port:
@@ -878,22 +928,28 @@
             self._robot_info.ip_address = address
 
             if self._robot_info.version.major < 8:
                 self.logger.warning('Python API not supported for firmware under version 8')
 
             self._robot_events.on_connected.set()
             self._callback_queue.put('on_connected')
-        except Exception:
+
+            # Start callback thread if necessary
+            self._start_callback_thread()
+        except Exception as e:
+            if self._fw_update_reboot_timestamp == 0:  # Don't print this trace when reconnecting during firmware update
+                self.logger.info(f'Failed to connect: {e}')
             self._disconnect()
             raise
 
     def Disconnect(self):
         """See documentation in equivalent function in robot.py"""
         if self.IsConnected():
-            self.logger.info('Disconnecting from the robot.')
+            if self._fw_update_reboot_timestamp == 0:  # Don't print this trace when reconnecting during firmware update
+                self.logger.info('Disconnecting from the robot.')
             self._disconnect()
         else:
             self.logger.debug('Ignoring Disconnect() called on a non-connected robot.')
 
     def _disconnect(self):
         """
         Internal function to disconnect Mecademic Robot object from the Mecademic robot and cleanup internal states.
@@ -953,25 +1009,34 @@
             Object containing the current robot status
 
         """
         # Use appropriate default timeout of not specified
         if timeout is None:
             timeout = self.default_timeout
         if synchronous_update:
-            if self._using_json_api:
+            if self._using_legacy_json_api:
                 with self._main_lock:
                     self._send_command('GetMotionStatus')
             self._send_sync_command('GetStatusRobot', self._robot_events.on_status_updated, timeout)
 
         with self._main_lock:
             return copy.deepcopy(self._robot_status)
 
     def IsConnected(self) -> bool:
         """See documentation in equivalent function in robot.py"""
-        return self._robot_events.on_connected.is_set()
+        if self._robot_events.on_connected.is_set():
+            try:
+                self._check_internal_states(refresh_monitoring_mode=True)
+                return True
+            except Exception:
+                if not self._fw_update_status.in_progress:
+                    self.logger.info('Connection to robot was lost.')
+                return False
+        else:
+            return False
 
     @disconnect_on_exception
     def DeactivateRobot(self):
         """See documentation in equivalent function in robot.py"""
         with self._main_lock:
             self._check_internal_states()
             self._send_command('DeactivateRobot')
@@ -1134,14 +1199,26 @@
     UPDATE_TIMEOUT = 15 * 60  # 15 minutes timeout
 
     def UpdateRobot(self,
                     firmware: Union[str, pathlib.Path],
                     address: Optional[str] = None,
                     timeout: float = UPDATE_TIMEOUT):
         """See documentation in equivalent function in robot.py"""
+        try:
+            self._update_robot(firmware, address, timeout)
+        except Exception as e:
+            raise
+        finally:
+            self._reset_fw_update_status()
+
+    def _update_robot(self,
+                      firmware: Union[str, pathlib.Path],
+                      address: Optional[str] = None,
+                      timeout: float = UPDATE_TIMEOUT):
+        """See documentation of UpdateRobot in robot.py"""
 
         if isinstance(firmware, pathlib.Path):
             firmware_file: pathlib.Path = firmware
         elif isinstance(firmware, str):
             firmware_file = pathlib.Path(firmware)
         else:
             raise ArgumentError(None,
@@ -1162,94 +1239,126 @@
         if not self.IsConnected():
             self.Connect(address=address)
         elif self._monitor_mode:
             self.logger.info(f'Connected to robot in monitoring mode only, attempting connection in command mode'
                              'to deactivate robot')
             self.Connect(address=address)
 
-        if self.GetStatusRobot(synchronous_update=True).activation_state:
+        # Make sure that the robot is not in EStop
+        if robot_model_is_meca500(
+                self.GetRobotInfo().robot_model) and self.GetStatusRobot(synchronous_update=True).estopState:
+            raise MecademicException(
+                f'Firmware update failed: Robot is in ESTOP. Please clear the ESTOP condition before updating.')
+
+        # Check if we must use legacy mode
+        use_legacy_update = not self.GetRobotInfo().version.is_at_least(9, 3, 0)
+
+        # Make sure that the robot is deactivated
+        if self.GetStatusRobot().activation_state:
             self.logger.info(f'Robot is activated, will attempt to deactivate before updating firmware')
             self.DeactivateRobot()
             self.WaitDeactivated()
         if self._enable_synchronous_mode is None:
             current_synchronous_mode = False
         else:
             current_synchronous_mode = self._enable_synchronous_mode
         self.Disconnect()
 
-        tested_port_8080 = False
-        robot_url = f"http://{address}/"
-        while (True):
-
-            self.logger.info(f"Installing firmware: {firmware_file.resolve()}")
-
-            with open(str(firmware_file), 'rb') as firmware_stream:
-                firmware_data = firmware_stream.read()
-                firmware_data_size = str(len(firmware_data))
-
-            headers = {
-                'Connection': 'keep-alive',
-                'Content-type': 'application/x-gzip',
-                'Content-Length': firmware_data_size
-            }
+        if not use_legacy_update:
+            # Reconnect to the robot using the JSON API
+            self.Connect(address=f'{address}:{MX_ROBOT_TCP_PORT_CONTROL_JSON}')
+
+        self.logger.info(f"Installing firmware: {firmware_file.resolve()}")
+
+        with open(str(firmware_file), 'rb') as firmware_stream:
+            firmware_data = firmware_stream.read()
+            firmware_data_size = str(len(firmware_data))
+
+        headers = {
+            'Connection': 'keep-alive',
+            'Content-type': 'application/x-gzip',
+            'Content-Length': firmware_data_size
+        }
+
+        if use_legacy_update:
+            self.logger.info(f"Uploading firmware (legacy mode)...")
+            robot_url = f"http://{address}/"
+        else:
+            self.logger.info(f"Uploading firmware...")
+            robot_url = f"http://{address}/fw-update/{firmware_file.name}"
 
-            self.logger.info(f"Uploading firmware")
-            request_post = requests.post(robot_url, data=firmware_data, headers=headers)
-            try:
-                request_post.raise_for_status()
-                break
-            except Exception as e:
-                if not tested_port_8080:
-                    # Failed -> Probably a robot v9.2+ with the new Web Portal. Let's use the 'legacy' Web
-                    # portal (for now at least, until we update this Python code to support the new "Json" API)
-                    tested_port_8080 = True
-                    robot_url = f"http://{address}:8080/"
-                    continue
-                self.logger.error(f"Upgrade post request error: {e}")
-                raise
+        request_post = requests.post(robot_url, data=firmware_data, headers=headers)
+        try:
+            request_post.raise_for_status()
+        except Exception as e:
+            self.logger.error(f"Upgrade post request error: {e}")
+            raise
 
         if not request_post.ok:
             error_message = f"Firmware upload request failed"
             raise RuntimeError(error_message)
 
-        self.logger.info(f"Upgrading the robot")
-        update_progress = UpdateProgress()
+        self.logger.info(f"Starting the firmware update...")
 
+        if not use_legacy_update:
+            # Send the 'StartFwUpdate' command
+            self._fw_update_status.in_progress = True  # Set once here, but the will be updated from robot update status
+            self._send_custom_command(f'StartFwUpdate({firmware_file.name})')
+
+        # Follow update status
         start_time = time.monotonic()
         while True:
+            if use_legacy_update:
+                self._check_update_progress_legacy(robot_url)
+            else:
+                self._check_update_progress(address)
 
-            # Give time to the web server restart, the function doesn't handle well errors.
-            time.sleep(2)
-
-            self._check_update_progress(robot_url, update_progress)
-            if update_progress.complete:
-                self.logger.info(f"Firmware update complete")
+            # Check if complete, failed or timeout
+            if self._fw_update_status.error:
+                raise MecademicException(f'Firmware update failed: {self._fw_update_status.error_msg}')
+            if self._fw_update_status.complete:
+                self.logger.info(f"Firmware update done")
                 break
             if time.monotonic() > start_time + timeout:
                 error_message = f"Timeout while waiting for update done response, after {timeout} seconds"
                 raise TimeoutError(error_message)
 
-        self.logger.info(f"Waiting for robot to reboot")
-
-        # need to wait to make sure the robot shutdown before attempting to ping it.
-        time.sleep(15)
-        # Try to ping the robot until it's responding (or until default timeout)
-        ping_robot(address)
-        # Now that robot responds to ping, wait until it accepts new connections
-        self.Connect(address, timeout=60, enable_synchronous_mode=current_synchronous_mode)
-
-        current_version = self.GetRobotInfo().version
-        if current_version.major < 8.0:
-            expected_version = firmware_file_version.short_version
+        if use_legacy_update:
+            # need to wait to make sure the robot shutdown before attempting to ping it.
+            time.sleep(15)
+            # Try to ping the robot until it's responding (or until default timeout)
+            ping_robot(address)
+            # Now that robot responds to ping, wait until it accepts new connections
+            self.Connect(address, timeout=60, enable_synchronous_mode=current_synchronous_mode)
         else:
-            expected_version = firmware_file_version.full_version
+            end_time = time.monotonic() + 30
+            while True:
+                if time.monotonic() > end_time:
+                    raise TimeoutError('Timeout while attempting to reconnect in control mode')
+                try:
+                    # Reconnect in control mode
+                    # (shorter timeout here, we know we're already connected so it should not be long)
+                    self.Disconnect()
+                    self.Connect(address, timeout=10, enable_synchronous_mode=current_synchronous_mode)
+                    break
+                except Exception as e:
+                    error_message = str(e)
+                    if 'id=3002,' in error_message:
+                        time.sleep(1)
+                        continue
+                    raise
 
-        if str(current_version) in expected_version:
-            self.logger.info(f"robot is now running version {current_version}")
+        if self.GetRobotInfo().version.is_at_least(8.0):
+            current_version = self.GetRobotInfo().version.get_str(build=True, extra=False)
+            expected_version = firmware_file_version.full_version
         else:
+            current_version = self.GetRobotInfo().version
+            expected_version = firmware_file_version.short_version
+
+        if not str(current_version) in expected_version:
             error_msg = f"Fail to install robot properly. current version {current_version}, " \
                         f"expecting: {expected_version}"
             self.logger.error(error_msg)
             raise AssertionError(error_msg)
 
         robot_status = self.GetStatusRobot(synchronous_update=True)
         if robot_status.error_status:
@@ -1259,34 +1368,139 @@
 
         self.logger.info(f"Installation of {current_version} successfully completed")
 
     #####################################################################################
     # Private methods.
     #####################################################################################
 
-    def _check_update_progress(self, robot_url: str, update_progress: UpdateProgress):
+    def _normalize_cart_cmd_args(self, alpha: float = None, beta: float = None, gamma: float = None) -> list[float]:
+        """Normalize alpha, beta and gamma arguments for Cartesian commands which accept alpha/beta
+        arguments to be omitted"""
+        if self.GetRobotInfo().num_joints == 6:
+            if alpha is None or beta is None or gamma is None:
+                raise ValueError('Missing argument (on this robot Cartesian positions require 6 values)')
+            else:
+                return [alpha, beta, gamma]
+        else:
+            # Only 2 valid ways of passing Cartesian arguments on 4 axes robots: Pass all, or pass only gamma
+            if alpha is not None and beta is not None and gamma is not None:
+                # Fine, all were passed
+                return [alpha, beta, gamma]
+            elif alpha is not None and beta is None and gamma is None:
+                # Only alpha was passed, probably by positional argument, assume it's the "gamma" value
+                return [0, 0, alpha]
+            elif alpha is None and beta is None and gamma is not None:
+                # Only gamma was passed, assume 0 for the others
+                return [0, 0, gamma]
+
+            raise ValueError('Wrong number of argument (on this robot Cartesian positions require 4 values)')
+
+    def _normalize_conf_cmd_args(self, shoulder: int = None, elbow: int = None, wrist: int = None) -> list[int]:
+        """Normalize shoulder, elbow and wrist "conf" arguments for commands which accept to omit shoulder and
+           wrist (for 4 axes robots which only have elbow conf)"""
+        if self.GetRobotInfo().num_joints == 6:
+            if shoulder is None or elbow is None or wrist is None:
+                raise ValueError('Missing argument (on this robot configuration requires 3 values)')
+            else:
+                return [shoulder, elbow, wrist]
+        else:
+            # Only 2 valid ways of passing Cartesian arguments on 4 axes robots: Pass all, or pass only elbow
+            if shoulder is not None and elbow is not None and wrist is not None:
+                # Fine, all were passed
+                return [shoulder, elbow, wrist]
+            elif shoulder is not None and elbow is None and wrist is None:
+                # Only shoulder was passed, probably by positional argument, assume it's the "elbow" value
+                return [0, shoulder, 0]
+            elif shoulder is None and elbow is not None and wrist is None:
+                # Only elbow was passed, assume 0 for the others
+                return [0, elbow, 0]
+
+            raise ValueError('Wrong number of arguments (on this robot configuration require 1 value)')
+
+    def _get_reboot_duration(self):
+        """ Get the average expected reboot duration for current robot model """
+        if self.GetRobotInfo().robot_model == MxRobotModel.MX_ROBOT_MODEL_MCS500_R1:
+            return MX_FW_UPDATE_REBOOT_DURATION_SEC_MCS500
+        else:
+            return MX_FW_UPDATE_REBOOT_DURATION_SEC_MECA500
+
+    def _get_fw_update_duration(self):
+        """ Get the average expected firmware update duration for current robot model """
+        if self.GetRobotInfo().robot_model == MxRobotModel.MX_ROBOT_MODEL_MCS500_R1:
+            return MX_FW_UPDATE_AVG_DURATION_SEC_MCS500
+        else:
+            return MX_FW_UPDATE_AVG_DURATION_SEC_MECA500
+
+    def _check_update_progress(self, address: str):
         """
-        Check progress of firmware update.
+        Check progress of firmware update (new implementation using JSON API).
+
+        Parameters
+        ----------
+        address: string
+            Robot IP address/port
+        """
+        time.sleep(0.1)
+        # Update status is updated in background by _handle_fw_update_progress until robot reboots at the end of the
+        # update, at which time the code below will periodically print progress for convenience
+        if not self.IsConnected():
+            # During update, we'll get disconnected. Try reconnecting in monitoring mode to follow update progress
+            try:
+                if self._monitor_mode and self._fw_update_status.in_progress and self._fw_update_reboot_timestamp == 0:
+                    # Got disconnected -> Consider we're awaiting for the robot to reboot
+                    self._fw_update_reboot_timestamp = time.monotonic()
+                self.Connect(address=f'{address}:{MX_ROBOT_TCP_PORT_FEED_JSON}', monitor_mode=True, timeout=1.0)
+                # Reconnected in monitoring mode, therefore update is started
+                self._fw_update_started = True
+            except Exception as e:
+                # In case we're updating to an older package (<9.3) we won't be able to connect to JSON port.
+                # So let's try to connect to standard port.
+                try:
+                    self.Connect(address=f'{address}', monitor_mode=True, timeout=0.1)
+                    # Successfully connected to legacy port. Validate that we're connected to older version
+                    if self.GetRobotInfo().version.is_at_least(9, 3):
+                        # Recent version, we should be able to connect to JSON port,
+                        # so let's close here and retry JSON above (next loop)
+                        self.Disconnect()
+                    else:
+                        # Older version. No JSON port exists so let's assume that the update is complete
+                        self._fw_update_status.complete = True
+                except:
+                    # Robot is probably still rebooting
+                    # Update the update percentage based on estimated reboot time
+                    if self._fw_update_reboot_timestamp == 0:
+                        reboot_pct = 0
+                    else:
+                        reboot_elapsed_ms = 1000 * (time.monotonic() - self._fw_update_reboot_timestamp)
+                        reboot_pct = 100 * (reboot_elapsed_ms / (1000 * self._get_reboot_duration()))
+                        if reboot_pct > 100:
+                            reboot_pct = 100
+
+                    # Print status while awaiting for robot to reboot
+                    if time.monotonic() - self._fw_update_status._last_print_timestamp > 5.0:
+                        self._print_fw_update_status(int(reboot_pct))
+
+    def _check_update_progress_legacy(self, robot_url: str):
+        """
+        Check progress of firmware update (legacy version with old web portal).
 
         Parameters
         ----------
         robot_url: string
             Robot URL
 
-        update_progress: UpdateProgress
-            Update progress information object
-
         """
-        update_progress.complete = False
+        time.sleep(2)
+        self._fw_update_status.complete = False
         request_get = requests.get(robot_url, 'update', timeout=10)
         try:
             request_get.raise_for_status()
         except Exception as e:
             self.logger.error(f'Upgrade get request error: {e}')
-            raise
+            raise e
 
         # get only correct answer (http code 200)
         if request_get.status_code == 200:
             request_response = request_get.text
         else:
             request_response = None
         # while the json file is note created, get function will return 0
@@ -1306,26 +1520,26 @@
         if request_answer['STATUS']:
             status_code = int(request_answer['STATUS']['Code'])
             status_msg = request_answer['STATUS']['MSG']
 
         if status_code in [0, 1]:
             keys = sorted(request_answer['LOG'].keys())
             if keys:
-                previous_progress = update_progress.progress
-                update_progress.progress = request_answer['LOG'][keys[-1]]
-                new_progress = update_progress.progress.replace(previous_progress, '')
+                previous_progress = self._fw_update_status.progress_str
+                self._fw_update_status.progress_str = request_answer['LOG'][keys[-1]]
+                new_progress = self._fw_update_status.progress_str.replace(previous_progress, '')
                 if ':' in new_progress:
                     self.logger.info(new_progress)
                 elif '100%' in new_progress:
                     self.logger.info(new_progress)
                 else:
                     self.logger.debug(new_progress)
             if status_code == 0:
                 self.logger.info(f'status_msg {status_msg}')
-                update_progress.complete = True
+                self._fw_update_status.complete = True
                 return
         else:
             error_message = f'error while updating: {status_msg}'
             self.logger.error(error_message)
             raise RuntimeError(error_message)
 
     def _check_monitor_threads(self):
@@ -1382,22 +1596,28 @@
             if self._monitor_mode:
                 if not refresh_monitoring_mode:
                     raise InvalidStateError('Cannot send command while in monitoring mode.')
             else:
                 self._check_command_threads()
 
             self._check_monitor_threads()
+
+            # Consider we're disconnected if we've not recently received a message from the robot
+            if self._monitor_timeout_used and self._rx_timestamp != 0:
+                elapsedMs = 1000 * (time.monotonic() - self._rx_timestamp)
+                if elapsedMs > _MONITORING_TIMEOUT_MS:
+                    raise TimeoutError(
+                        f'Timeout: No message received from the robot in the last {elapsedMs}ms. Assuming we are disconnected from the robot.'
+                    )
         except Exception:
             # An error was detected while validating internal states. Disconnect from robot.
             self._disconnect()
             raise
 
-    def _split_command_args(self,
-                            command: str,
-                            args: Union[str, list, tuple] = None) -> list[str, Union[str, list, tuple]]:
+    def _split_command_args(self, command: str, args: Union[str, list, tuple] = None) -> list:
         """In the case the arguments are passed in the command argument, this function will split the command name
            and arguments.
 
         Parameters
         ----------
         command : str
             String that contains the command name and possibly the arguments too
@@ -1439,15 +1659,17 @@
             # Clearing the motion queue also requires clearing checkpoints, as the robot will not send them anymore.
             message = "ClearMotion"
             self._invalidate_checkpoints(message)
             self._invalidate_interruptable_events_on_clear_motion(message)
 
         # Assemble arguments into a string and concatenate to end of command.
         if args:
-            if isinstance(args, list) or isinstance(args, tuple):
+            if isinstance(args, tuple):
+                command += f'({args_to_string(list(args))})'
+            elif isinstance(args, list):
                 command += f'({args_to_string(args)})'
             else:
                 command += f'({args})'
 
         # Put command into tx queue.
         self._command_tx_queue.put(command)
 
@@ -1553,29 +1775,30 @@
             self._command_socket,
             *args,
         ))
         thread.setDaemon(True)  # Make sure thread does not prevent application from quitting
         thread.start()
         return thread
 
-    def _initialize_command_socket(self, timeout=0.1):
+    def _initialize_command_socket(self, timeout=1.0):
         """Establish the command socket and the associated thread.
 
         """
         if self._offline_mode:
             return
 
         if self._command_socket is not None:
             raise InvalidStateError('Cannot connect since existing command socket exists.')
 
         if self._custom_port:
             port = self._custom_port
         else:
             port = MX_ROBOT_TCP_PORT_CONTROL
         self._command_socket = self._connect_socket(self.logger, self._address, port, timeout)
+        self.logger.info(f'Connected to {self._address}:{port} (control mode)')
 
         if self._command_socket is None:
             raise CommunicationError('Command socket could not be created. Is the IP address correct?')
 
         # Create rx thread for command socket communication.
         self._command_rx_thread = self._launch_thread(target=self._handle_socket_rx,
                                                       args=(
@@ -1603,14 +1826,15 @@
             raise InvalidStateError('Cannot connect since existing monitor socket exists.')
 
         if self._custom_port:
             port = self._custom_port
         else:
             port = MX_ROBOT_TCP_PORT_FEED
         self._monitor_socket = self._connect_socket(self.logger, self._address, port, timeout)
+        self.logger.info(f'Connected to {self._address}:{port} (monitoring mode)')
 
         if self._monitor_socket is None:
             raise CommunicationError('Monitor socket could not be created. Is the IP address correct?')
 
         # Create rx thread for monitor socket communication.
         self._monitor_rx_thread = self._launch_thread(target=self._handle_socket_rx,
                                                       args=(
@@ -2030,14 +2254,16 @@
 
         Parameters
         ----------
         response : Message object
             Robot status response to parse and handle.
 
         """
+        # Remember the last time we've received a message from the robot
+        self._rx_timestamp = time.monotonic()
 
         # Print error trace if this is an error code
         if response.id in robot_status_code_info:
             code_info = robot_status_code_info[response.id]
             if code_info.is_error:
                 self.logger.error(f'Received robot error {code_info.code} ({code_info.name}): {response.data}')
         else:
@@ -2097,15 +2323,15 @@
 
         #
         # Handle various responses/events that we're interested into
         #
         if response.id == mx_st.MX_ST_GET_STATUS_ROBOT:
             self._handle_robot_status_response(response)
 
-        if response.id == mx_st.MX_ST_GET_MOTION_STATUS:
+        if response.id == 2011:  # Legacy motion status (now included in MX_ST_GET_STATUS_ROBOT)
             self._handle_motion_status_response(response)
 
         elif response.id == mx_st.MX_ST_GET_ROBOT_SERIAL:
             self._handle_robot_get_robot_serial_response(response)
 
         elif response.id == mx_st.MX_ST_GET_STATUS_GRIPPER:
             self._handle_gripper_status_response(response)
@@ -2124,14 +2350,23 @@
 
         elif response.id == mx_st.MX_ST_RT_GRIPPER_FORCE:
             self._robot_rt_data.rt_gripper_force.update_from_csv(response.data)
 
         elif response.id == mx_st.MX_ST_RT_GRIPPER_POS:
             self._robot_rt_data.rt_gripper_pos.update_from_csv(response.data)
 
+        elif response.id == mx_st.MX_ST_RT_IO_STATUS:
+            self._handle_io_status(response)
+
+        elif response.id == mx_st.MX_ST_RT_OUTPUT_STATE:
+            self._handle_output_state(response)
+
+        elif response.id == mx_st.MX_ST_RT_INPUT_STATE:
+            self._handle_input_state(response)
+
         elif response.id == mx_st.MX_ST_EXTTOOL_SIM:
             if not str(response.data).isdigit():
                 # Legacy response without the tool type argument
                 self._handle_ext_tool_sim_status(MxExtToolType.MX_EXT_TOOL_MEGP25_SHORT)
             else:
                 self._handle_ext_tool_sim_status(int(response.data))
 
@@ -2162,15 +2397,15 @@
             else:
                 self._robot_events.on_pstop2.clear()
                 self._robot_events.on_pstop2_reset.set()
                 self._callback_queue.put('on_pstop2_reset')
 
         elif response.id == mx_st.MX_ST_ESTOP:
             self._robot_status.estopState = self._parse_response_int(response)[0]
-            if self._robot_status.estopState == MxStopState.MX_STOP_STATE_ACTIVE:
+            if self._robot_status.estopState != MxStopState.MX_STOP_STATE_RESET:
                 self._robot_events.on_estop_reset.clear()
                 self._robot_events.on_estop.set()
                 self._callback_queue.put('on_estop')
             else:
                 self._robot_events.on_estop.clear()
                 self._robot_events.on_estop_reset.set()
                 self._callback_queue.put('on_estop_reset')
@@ -2243,14 +2478,20 @@
             # Don't abort the event otherwise we can't try later to reset the error because WaitErrorReset
             # remains "aborted" for ever
             # self._robot_events.on_error_reset.abort(message)
 
         elif response.id == mx_st.MX_ST_GET_REAL_TIME_MONITORING:
             self._handle_get_realtime_monitoring_response(response)
 
+        elif response.id == mx_st.MX_ST_PSU_DONGLE_STATUS:
+            self._handle_psu_dongle_status(response)
+
+        elif response.id == mx_st.MX_ST_FW_UPDATE_PROGRESS:
+            self._handle_fw_update_progress(response)
+
         elif response.id == mx_st.MX_ST_SYNC_CMD_QUEUE:
             self._handle_sync_response(response)
 
     def _parse_response_bool(self, response: Message) -> list[bool]:
         """ Parse standard robot response, returns array of boolean values
         """
         if response.data.strip() == '':
@@ -2272,21 +2513,23 @@
         Parameters
         ----------
         activated : bool
             Robot is activated or not
         """
         if not self._first_robot_status_received or self._robot_status.activation_state != activated:
             if activated:
-                self.logger.info(f'Robot is activated.')
+                if self._robot_status.activation_state != activated:
+                    self.logger.info(f'Robot is activated.')
                 self._robot_events.on_deactivated.clear()
                 self._robot_events.on_activated.set()
                 self._set_brakes_engaged(False)
                 self._callback_queue.put('on_activated')
             else:
-                self.logger.info(f'Robot is deactivated.')
+                if self._robot_status.activation_state != activated:
+                    self.logger.info(f'Robot is deactivated.')
                 self._robot_events.on_activated.clear()
                 self._robot_events.on_deactivated.set()
                 self._set_brakes_engaged(True)
                 self._callback_queue.put('on_deactivated')
                 # Invalidate checkpoints and appropriate interruptable events
                 message = 'Robot was deactivated'
                 self._invalidate_checkpoints(message)
@@ -2363,14 +2606,16 @@
                 message = "robot is in error"
                 self._invalidate_checkpoints(message)
                 self._invalidate_interruptable_events_on_error(message)
                 self._robot_events.on_error.set()
                 self._robot_events.abort_all_on_error(message)
                 self._robot_events.on_error_reset.clear()
                 self._callback_queue.put('on_error')
+                # Always consider the robot paused when entering error state
+                self._robot_status.pause_motion_status = True
             else:
                 self._robot_events.clear_abort_all()
                 self._robot_events.on_error.clear()
                 self._robot_events.on_error_reset.set()
                 self._callback_queue.put('on_error_reset')
             self._robot_status.error_status = error_status
 
@@ -2431,18 +2676,17 @@
 
         Parameters
         ----------
         response : Message object
             Motion status response to parse and handle.
 
         """
-        assert response.id == mx_st.MX_ST_GET_MOTION_STATUS
         if response.jsonData:
             # JSON format.
-            self._using_json_api = True
+            self._using_legacy_json_api = True
             jsonData = response.jsonData[MX_JSON_KEY_DATA]
             self._set_paused(jsonData[MX_JSON_KEY_MOTION_ROBOT_HOLD])
             self._set_eob(jsonData[MX_JSON_KEY_MOTION_ROBOT_EOB])
 
         # Note: Let's not yet update _first_robot_status_received or on_status_updated.
         #       We'll do that in _handle_robot_status_response since we're expecting to receive robot status
         #       immediately after motion status.
@@ -2455,22 +2699,37 @@
         response : Message object
             Robot status response to parse and handle.
 
         """
         assert response.id == mx_st.MX_ST_GET_STATUS_ROBOT
         if response.jsonData:
             # JSON format.
-            self._using_json_api = True
             jsonData = response.jsonData[MX_JSON_KEY_DATA]
-            self._set_activated(jsonData[MX_JSON_KEY_STATUS_ROBOT_STATE] >= MxRobotState.MX_ROBOT_STATE_ACTIVATED)
-            self._set_homed(jsonData[MX_JSON_KEY_STATUS_ROBOT_STATE] == MxRobotState.MX_ROBOT_STATE_RUN)
-            self._set_sim_mode(jsonData[MX_JSON_KEY_STATUS_ROBOT_SIM])
-            self._set_recovery_mode(jsonData[MX_JSON_KEY_STATUS_ROBOT_RECOVERY])
-            self._set_error_status(jsonData[MX_JSON_KEY_STATUS_ROBOT_ERR] != 0)
-            self._set_brakes_engaged(jsonData[MX_JSON_KEY_STATUS_ROBOT_BRAKES] != 0)
+            jsonRobotStatus = None
+            jsonMotionStatus = None
+            if MX_JSON_KEY_ROBOT_STATUS in jsonData:
+                jsonRobotStatus = jsonData[MX_JSON_KEY_ROBOT_STATUS]
+            if MX_JSON_KEY_MOTION_STATUS in jsonData:
+                jsonMotionStatus = jsonData[MX_JSON_KEY_MOTION_STATUS]
+
+            if jsonRobotStatus is None:
+                # Legacy JSON format
+                jsonRobotStatus = jsonData
+
+            if jsonRobotStatus is not None:
+                self._set_activated(
+                    jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_STATE] >= MxRobotState.MX_ROBOT_STATE_ACTIVATED)
+                self._set_homed(jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_STATE] == MxRobotState.MX_ROBOT_STATE_RUN)
+                self._set_sim_mode(jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_SIM])
+                self._set_recovery_mode(jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_RECOVERY])
+                self._set_error_status(jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_ERR] != 0)
+                self._set_brakes_engaged(jsonRobotStatus[MX_JSON_KEY_STATUS_ROBOT_BRAKES] != 0)
+            if jsonMotionStatus is not None:
+                self._set_paused(jsonMotionStatus[MX_JSON_KEY_MOTION_ROBOT_HOLD])
+                self._set_eob(jsonMotionStatus[MX_JSON_KEY_MOTION_ROBOT_EOB])
         else:
             # Legacy format.
             status_flags = self._parse_response_bool(response)
 
             self._set_activated(status_flags[0])
             self._set_homed(status_flags[1])
             self._set_sim_mode(status_flags[2])
@@ -2559,23 +2818,36 @@
 
         Parameters
         ----------
         response : Message object
             External tool status response to parse and handle.
 
         """
+
         assert response.id == mx_st.MX_ST_RT_EXTTOOL_STATUS
-        self._robot_rt_data.rt_external_tool_status.update_from_csv(response.data)
-        status_flags = self._robot_rt_data.rt_external_tool_status.data
+        if response.jsonData:
+            # JSON format.
+            jsonData = response.jsonData[MX_JSON_KEY_DATA]
+            self._robot_rt_data.rt_external_tool_status.timestamp = response.jsonData[MX_JSON_KEY_TIMESTAMP_US]
+            status_flags = self._robot_rt_data.rt_external_tool_status.data
+            status_flags[0] = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_SIM_TYPE]
+            status_flags[1] = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_PHYSICAL_TYPE]
+            status_flags[2] = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_HOMED]
+            status_flags[3] = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_ERROR]
+            status_flags[4] = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_OVERHEAT]
+            self._external_tool_status.comm_err_warning = jsonData[MX_JSON_KEY_EXTTOOL_STATUS_COMM_ERR]
+        else:
+            self._robot_rt_data.rt_external_tool_status.update_from_csv(response.data)
+            status_flags = self._robot_rt_data.rt_external_tool_status.data
 
         self._external_tool_status.sim_tool_type = status_flags[0]
         self._external_tool_status.physical_tool_type = status_flags[1]
-        self._external_tool_status.homing_state = status_flags[2]
-        self._external_tool_status.error_status = status_flags[3]
-        self._external_tool_status.overload_error = status_flags[4]
+        self._external_tool_status.homing_state = status_flags[2] != 0
+        self._external_tool_status.error_status = status_flags[3] != 0
+        self._external_tool_status.overload_error = status_flags[4] != 0
 
         if self._is_in_sync():
             self._robot_events.on_external_tool_status_updated.set()
             self._callback_queue.put('on_external_tool_status_updated')
 
     def _handle_gripper_state_response(self, response: Message):
         """Parse gripper state response and update status fields and events.
@@ -2614,14 +2886,162 @@
 
         self._valve_state.valve_opened = self._robot_rt_data.rt_valve_state.data
 
         if self._is_in_sync():
             self._robot_events.on_valve_state_updated.set()
             self._callback_queue.put('on_valve_state_updated')
 
+    def _handle_io_status(self, response: Message):
+        """Parse IO status and update status fields and events.
+
+        Parameters
+        ----------
+        response : Message object
+            Io state to parse and handle.
+
+        """
+        assert response.id == mx_st.MX_ST_RT_IO_STATUS
+
+        # Extract the Bank id
+        bank_id = MxIoBankId.MX_IO_BANK_ID_UNDEFINED
+        values = []
+        if response.jsonData:
+            bank_id = response.jsonData[MX_JSON_KEY_DATA][MX_JSON_KEY_IO_STATUS_BANK_ID]
+        else:
+            values = tools.string_to_numbers(response.data)
+            bank_id = values[1]
+
+        new_io_status = IoStatus()
+        new_io_status_ts = TimestampedData.zeros(4)
+        if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+            new_io_status = self._rt_psu_io_status
+        elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+            new_io_status = self._rt_io_module_status
+        else:
+            return
+        new_io_status.bank_id = bank_id
+        prev_sim_mode = new_io_status.sim_mode
+
+        if response.jsonData:
+            # JSON format. Convert into timestamped data
+            jsonData = response.jsonData[MX_JSON_KEY_DATA]
+
+            # Extract JSON data
+            if MX_JSON_KEY_IO_STATUS_PRESENT in jsonData:
+                new_io_status.present = jsonData[MX_JSON_KEY_IO_STATUS_PRESENT]
+            if MX_JSON_KEY_IO_STATUS_NB_INPUTS in jsonData:
+                new_io_status.nb_inputs = jsonData[MX_JSON_KEY_IO_STATUS_NB_INPUTS]
+            if MX_JSON_KEY_IO_STATUS_NB_OUTPUTS in jsonData:
+                new_io_status.nb_outputs = jsonData[MX_JSON_KEY_IO_STATUS_NB_OUTPUTS]
+            if MX_JSON_KEY_IO_STATUS_SIM_MODE in jsonData:
+                new_io_status.sim_mode = jsonData[MX_JSON_KEY_IO_STATUS_SIM_MODE]
+            if MX_JSON_KEY_IO_STATUS_ERROR in jsonData:
+                new_io_status.error = jsonData[MX_JSON_KEY_IO_STATUS_ERROR]
+            if MX_JSON_KEY_TIMESTAMP_US in response.jsonData:
+                new_io_status.timestamp = response.jsonData[MX_JSON_KEY_TIMESTAMP_US]
+            # Convert into timestamped data (equivalent to text API)
+            new_io_status_ts.timestamp = new_io_status.timestamp
+            new_io_status_ts.data[0] = new_io_status.bank_id
+            new_io_status_ts.data[1] = 1 if new_io_status.present else 0
+            new_io_status_ts.data[2] = 1 if new_io_status.sim_mode else 0
+            new_io_status_ts.data[3] = new_io_status.error
+        else:
+            # Extract API values
+            new_io_status_ts.update_from_csv(response.data)
+            new_io_status.timestamp = values[0]
+            new_io_status.present = True if values[2] != 0 else False
+            new_io_status.sim_mode = True if values[3] != 0 else False
+            new_io_status.error = values[4]
+            # Note: nb_inputs and nb_outputs is updated by _handle_input_state / _handle_output_state
+
+        # Store back into our context
+        if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+            self._rt_psu_io_status = new_io_status
+            self._robot_rt_data.rt_psu_io_status = new_io_status_ts
+        elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+            self._rt_io_module_status = new_io_status
+            self._robot_rt_data.rt_io_module_status = new_io_status_ts
+
+        # Update events/callbacks
+        if not self._first_robot_status_received or prev_sim_mode != new_io_status.sim_mode:
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                if new_io_status.sim_mode:
+                    self._robot_events.on_psu_io_sim_enabled.set()
+                    self._robot_events.on_psu_io_sim_disabled.clear()
+                    self._callback_queue.put('on_psu_io_sim_enabled')
+                else:
+                    self._robot_events.on_psu_io_sim_enabled.clear()
+                    self._robot_events.on_psu_io_sim_disabled.set()
+                    self._callback_queue.put('on_psu_io_sim_disabled')
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                if new_io_status.sim_mode:
+                    self._robot_events.on_io_sim_enabled.set()
+                    self._robot_events.on_io_sim_disabled.clear()
+                    self._callback_queue.put('on_io_sim_enabled')
+                else:
+                    self._robot_events.on_io_sim_enabled.clear()
+                    self._robot_events.on_io_sim_disabled.set()
+                    self._callback_queue.put('on_io_sim_disabled')
+
+    def _handle_output_state(self, response: Message):
+        """Parse digital output state and update status fields and events.
+
+        Parameters
+        ----------
+        response : Message object
+            Digital output state to parse and handle.
+
+        """
+        assert response.id == mx_st.MX_ST_RT_OUTPUT_STATE
+        values = tools.string_to_numbers(response.data)
+        changed = False
+        if len(values) > 1:
+            timestamp = values[0]
+            bank_id = values[1]
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                changed = True
+                self._robot_rt_data.rt_psu_outputs.update_from_data(timestamp, values[2:])
+                self._rt_psu_io_status.nb_outputs = len(self._robot_rt_data.rt_psu_outputs.data)
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                changed = True
+                self._robot_rt_data.rt_io_module_outputs.update_from_data(timestamp, values[2:])
+                self._rt_io_module_status.nb_outputs = len(self._robot_rt_data.rt_io_module_outputs.data)
+
+        if changed and self._is_in_sync():
+            self._robot_events.on_output_state_updated.set()
+            self._callback_queue.put('on_output_state_updated')
+
+    def _handle_input_state(self, response: Message):
+        """Parse digital input state and update status fields and events.
+
+        Parameters
+        ----------
+        response : Message object
+            Digital input state to parse and handle.
+
+        """
+        assert response.id == mx_st.MX_ST_RT_INPUT_STATE
+        values = tools.string_to_numbers(response.data)
+        changed = False
+        if len(values) > 1:
+            timestamp = values[0]
+            bank_id = values[1]
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                changed = True
+                self._robot_rt_data.rt_psu_inputs.update_from_data(timestamp, values[2:])
+                self._rt_psu_io_status.nb_inputs = len(self._robot_rt_data.rt_psu_inputs.data)
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                changed = True
+                self._robot_rt_data.rt_io_module_inputs.update_from_data(timestamp, values[2:])
+                self._rt_io_module_status.nb_inputs = len(self._robot_rt_data.rt_io_module_inputs.data)
+
+        if changed and self._is_in_sync():
+            self._robot_events.on_input_state_updated.set()
+            self._callback_queue.put('on_input_state_updated')
+
     def _handle_checkpoint_response(self, response: Message):
         """Handle the checkpoint message from the robot, set the appropriate events, etc.
 
         Parameters
         ----------
         response : Message object
             Response message which includes the received checkpoint id.
@@ -2724,18 +3144,101 @@
                 self._robot_rt_data.rt_external_tool_status.enabled = True
             if event_id == mx_st.MX_ST_RT_VALVE_STATE:
                 self._robot_rt_data.rt_valve_state.enabled = True
             if event_id == mx_st.MX_ST_RT_GRIPPER_FORCE:
                 self._robot_rt_data.rt_gripper_force.enabled = True
             if event_id == mx_st.MX_ST_RT_GRIPPER_POS:
                 self._robot_rt_data.rt_gripper_pos.enabled = True
+            if event_id == mx_st.MX_ST_RT_IO_STATUS:
+                self._robot_rt_data.rt_io_module_status.enabled = True
+            if event_id == mx_st.MX_ST_RT_OUTPUT_STATE:
+                self._robot_rt_data.rt_io_module_outputs.enabled = True
+            if event_id == mx_st.MX_ST_RT_INPUT_STATE:
+                self._robot_rt_data.rt_io_module_inputs.enabled = True
 
         # Make sure to clear values that we should no more received
         self._robot_rt_data._clear_if_disabled()
 
+    def _print_fw_update_status(self, reboot_pct: float = 0):
+        """ Print a trace that summarize current firmware update status (progression) """
+        reboot_ratio = self._get_reboot_duration() / self._get_fw_update_duration()
+
+        total_pct = ((1 - reboot_ratio) * self._fw_update_status.progress) + (reboot_ratio * reboot_pct)
+
+        if self._fw_update_status.error:
+            # Print as 'debug' trace (error trace will be printed by UpdateRobot function anyways)
+            self.logger.debug(f'Firmware update failed: {self._fw_update_status.error_msg}')
+        elif self._fw_update_status.complete:
+            # Print as 'debug' trace (info trace will be printed by UpdateRobot function anyways)
+            self.logger.debug(f'Firmware update complete')
+        else:
+            self.logger.info(f'Firmware update progress: {int(total_pct)}% ({self._fw_update_status.step})')
+        self._fw_update_status._last_print_timestamp = time.monotonic()
+
+    def _handle_fw_update_progress(self, event: Message):
+        """Parse robot firmware update progress message
+
+        Parameters
+        ----------
+        event : Message object
+            The event message to parse.
+
+        """
+        assert event.id == mx_st.MX_ST_FW_UPDATE_PROGRESS
+        if event.jsonData:
+            jsonData = event.jsonData[MX_JSON_KEY_DATA]
+
+            # Parse JSON message
+            new_updating = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_UPDATING]
+            new_version = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_VERSION]
+            new_error = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR]
+            new_error_msg = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR_MSG]
+            new_progress_pct = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_PCT]
+            new_step = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_STEP]
+            reboot_done = False
+            if MX_JSON_KEY_FW_UPDATE_PROGRESS_REBOOT_DONE in jsonData:
+                reboot_done = jsonData[MX_JSON_KEY_FW_UPDATE_PROGRESS_REBOOT_DONE]
+
+            # Check if it's time to print update progress
+            print_now = False
+            if self._fw_update_reboot_timestamp != 0:
+                print_now = False  # In this case progress is printed by _check_update_progress
+            if new_step != self._fw_update_status.step:
+                print_now = True
+            elif time.monotonic() - self._fw_update_status._last_print_timestamp > 5.0:
+                print_now = True
+
+            self._fw_update_status.in_progress = new_updating
+            self._fw_update_status.complete = self._fw_update_started and not new_updating
+            self._fw_update_status.version = new_version
+            self._fw_update_status.error = new_error
+            self._fw_update_status.error_msg = new_error_msg
+            self._fw_update_status.progress = new_progress_pct
+            self._fw_update_status.step = new_step
+
+            if print_now:
+                reboot_pct = 100 if reboot_done else 0
+                self._print_fw_update_status(reboot_pct)
+
+    def _handle_psu_dongle_status(self, event: Message):
+        """Parse power-supply dongle status
+
+        Parameters
+        ----------
+        event : Message object
+            The event message to parse.
+
+        """
+        assert event.id == mx_st.MX_ST_PSU_DONGLE_STATUS
+        if event.jsonData:
+            jsonData = event.jsonData[MX_JSON_KEY_DATA]
+
+            # Parse JSON message
+            self._robot_info.psu_dongle_detected = jsonData[MX_JSON_KEY_PSU_DONGLE_DETECTED]
+
     def _handle_sync_response(self, response: Message):
         """Parse robot response to "SyncCmdQueue" request
            This class uses the "SyncCmdQueue" request/response to ensure synchronous "Get" operations have received the
            expected response from the robot (and not a response/event sent by the robot prior to our "Get" request).
 
         Parameters
         ----------
```

### Comparing `mecademicpy-1.3.0/mecademicpy/_robot_trajectory_logger.py` & `mecademicpy-1.4.0/mecademicpy/_robot_trajectory_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import queue
 import time
 from pathlib import PurePath
 
 import pandas as pd
 
 from .mx_robot_def import MxRobotStatusCode as mx_st
+from .robot_classes import *
 from .robot_trajectory_files import RobotTrajectories
 
 # 2nd values of this dict are taken from controller.cpp HandleSetRealTimeMonitoring() -> ParseStatusCodeString()
 # dict and put in UpperCamelCase for convenience (all column names in logged dataframe will be in the format of these
 # values)
 robot_rt_data_to_real_time_monit = {
     'rt_target_joint_pos': (mx_st.MX_ST_RT_TARGET_JOINT_POS, 'TargetJointPos'),
@@ -34,14 +35,20 @@
     'rt_trf': (mx_st.MX_ST_RT_TRF, 'Trf'),
     'rt_checkpoint': (mx_st.MX_ST_RT_CHECKPOINT, 'Checkpoint'),
     'rt_external_tool_status': (mx_st.MX_ST_RT_EXTTOOL_STATUS, 'ExtToolStatus'),
     'rt_valve_state': (mx_st.MX_ST_RT_VALVE_STATE, 'ValveState'),
     'rt_gripper_state': (mx_st.MX_ST_RT_GRIPPER_STATE, 'GripperState'),
     'rt_gripper_force': (mx_st.MX_ST_RT_GRIPPER_FORCE, 'GripperForce'),
     'rt_gripper_pos': (mx_st.MX_ST_RT_GRIPPER_POS, 'GripperPos'),
+    'rt_psu_io_status': (mx_st.MX_ST_RT_IO_STATUS, 'PsuIoModuleStatus'),
+    'rt_psu_outputs': (mx_st.MX_ST_RT_OUTPUT_STATE, 'PsuOutputState'),
+    'rt_psu_inputs': (mx_st.MX_ST_RT_INPUT_STATE, 'PsuInputState'),
+    'rt_io_module_status': (mx_st.MX_ST_RT_IO_STATUS, 'IoModuleStatus'),
+    'rt_io_module_outputs': (mx_st.MX_ST_RT_OUTPUT_STATE, 'IoModuleOutputState'),
+    'rt_io_module_inputs': (mx_st.MX_ST_RT_INPUT_STATE, 'IoModuleInputState'),
     '': (mx_st.MX_ST_RT_CYCLE_END, 'CycleEnd')  # Should not be used, handled by Robot class when it uses the logger
 }
 
 
 class _RobotTrajectoryLogger:
     """Class to handle logging robot state to file.
 
@@ -67,31 +74,31 @@
     data_dict:
         Keys: timestamps. Values: robot state stored at moment corresponding to timestamp
     robot_trajectories: RobotTrajectories object
         Contains robot states logged data and information about the robot used during logging
     """
 
     def __init__(self,
-                 robot_info,
-                 robot_rt_data,
+                 robot_info: RobotInfo,
+                 robot_rt_data: RobotRtData,
                  fields: list[str] = None,
                  file_name: str = None,
                  file_path: str = None,
                  record_time: bool = True,
                  monitoring_interval: float = None):
         """Initialize class.
 
         Parameters
         ----------
         robot_info : RobotInfo
             Contains robot information.
-        fields : list of strings
-            List of fields to be logged.
         robot_rt_data : RobotRtData object
             Contains state of robot.
+        fields : list of strings
+            List of fields to be logged.
         file_name: string or None
             Log file name
             If None, file name will be built with date/time and robot information (robot type, serial, version).
         file_path : string or None
             Path to save the zipped file that contains logged data + robot info in, respectively, csv and json file.
             If not provided, file will be saved in working directory.
         record_time : bool
@@ -153,17 +160,17 @@
             self.robot_trajectories.robot_context.robot_information[0]['serial_number'] = f'{robot_info.serial}'
         if record_time:
             self.robot_trajectories.robot_context.robot_information[0]['time_recorded'] = f'{current_date_time}'
         if monitoring_interval:
             self.robot_trajectories.robot_context.robot_information[0]['monitoring_interval'] = f'{monitoring_interval}'
 
         # Write headers for logged data
-        self.write_field_and_element_headers(robot_info)
+        self.write_field_and_element_headers(robot_info, robot_rt_data)
 
-    def get_timestamp_data(self, robot_rt_data, field):
+    def get_timestamp_data(self, robot_rt_data: RobotRtData, field):
         """ Return timestamp data object associated with the specific field (or None).
 
         Parameters
         ----------
         robot_rt_data : RobotRtData object
             Current state of robot to get timestamp_data from
         field : String
@@ -176,22 +183,45 @@
             if index not in accel_dict:
                 return None
             field_attr = accel_dict[index]
         else:
             field_attr = getattr(robot_rt_data, field)
         return field_attr
 
-    def write_field_and_element_headers(self, robot_info):
+    def _build_io_fields(self, prefix: str, type: str, count: int) -> list[str]:
+        """Build a list of digital IO field names
+
+        Parameters
+        ----------
+        prefix : str
+            IO bank prefix (ex: 'psu' or 'ioModule')
+        type : str
+            IO type ('Input' or 'Output')
+        count : int
+            Number of IOs of this type in this bank
+
+        Returns
+        -------
+        list[str]
+            _description_
+        """
+        fields = []
+        for idx in range(count):
+            fields.append(f'{prefix}{type}_{idx + 1}')
+        return fields
+
+    def write_field_and_element_headers(self, robot_info: RobotInfo, robot_rt_data: RobotRtData):
         """Write the full field name and element name in each column.
 
         Parameters
         ----------
         robot_info : RobotInfo
             Information about the robot, such as model name and number of joints.
-
+        robot_rt_data : RobotRtData object
+            Contains state of robot.
         """
 
         def assemble_with_prefix(field, names):
             return [field + '_' + str(x) for x in names]
 
         # Write full name for each field.
         for key, value in self.fields.items():
@@ -209,27 +239,48 @@
                 self.expanded_fields.append(value)
             elif key.endswith('conf'):
                 self.expanded_fields.extend(assemble_with_prefix(value, ['Shoulder', 'Elbow', 'Wrist']))
             elif key.endswith('checkpoint'):
                 self.expanded_fields.append(value)
             elif key.endswith('rt_external_tool_status'):
                 self.expanded_fields.extend(
-                    assemble_with_prefix(value, ['sim_model', 'physical_model', 'present', 'homed', 'error']))
+                    assemble_with_prefix(value, ['SimModel', 'PhysicalModel', 'Present', 'Homed', 'Error']))
             elif key.endswith('rt_valve_state'):
                 self.expanded_fields.extend(assemble_with_prefix(value, ['valve1', 'valve2']))
             elif key.endswith('rt_gripper_state'):
-                self.expanded_fields.extend(assemble_with_prefix(value, ['holding', 'atpos', 'closed', 'opened']))
+                self.expanded_fields.extend(
+                    assemble_with_prefix(value, ['Holding', 'TargetReached', 'Closed', 'Opened']))
             elif key.endswith('rt_gripper_force'):
                 self.expanded_fields.extend(assemble_with_prefix(value, ['%']))
             elif key.endswith('rt_gripper_pos'):
                 self.expanded_fields.extend(assemble_with_prefix(value, ['mm']))
+            elif key.endswith('rt_psu_io_status'):
+                self.expanded_fields.extend(assemble_with_prefix(value, ['BankId', 'Present', 'SimMode', 'Error']))
+            elif key.endswith('rt_io_module_status'):
+                self.expanded_fields.extend(assemble_with_prefix(value, ['BankId', 'Present', 'SimMode', 'Error']))
+            elif key.endswith('rt_psu_outputs'):
+                nb_outputs = len(robot_rt_data.rt_psu_outputs.data)
+                if nb_outputs != 0:
+                    self.expanded_fields.extend(self._build_io_fields('Psu', 'Output', nb_outputs))
+            elif key.endswith('rt_psu_inputs'):
+                nb_inputs = len(robot_rt_data.rt_psu_inputs.data)
+                if nb_inputs != 0:
+                    self.expanded_fields.extend(self._build_io_fields('Psu', 'Input', nb_inputs))
+            elif key.endswith('rt_io_module_outputs'):
+                nb_outputs = len(robot_rt_data.rt_io_module_outputs.data)
+                if nb_outputs != 0:
+                    self.expanded_fields.extend(self._build_io_fields('IoModule', 'Output', nb_outputs))
+            elif key.endswith('rt_io_module_inputs'):
+                nb_inputs = len(robot_rt_data.rt_io_module_inputs.data)
+                if nb_inputs != 0:
+                    self.expanded_fields.extend(self._build_io_fields('IoModule', 'Input', nb_inputs))
             else:
                 raise ValueError(f'Missing formatting for field: {key}')
 
-    def write_fields(self, timestamp, robot_rt_data):
+    def write_fields(self, timestamp, robot_rt_data: RobotRtData):
         """Write fields to file.
 
         Parameters
         ----------
         timestamp : numeric
             The timestamp of the current data.
         robot_rt_data : RobotRtData object
```

### Comparing `mecademicpy-1.3.0/mecademicpy/mx_robot_def.py` & `mecademicpy-1.4.0/mecademicpy/mx_robot_def.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 MX_JOINT_LIMIT_MIN_RANGE_DEG = 25  # Last joint requires ~12 deg during homing in either direction
 MX_RECOVERY_MODE_MAX_JOINT_VEL_PCT = 5.0
 MX_RECOVERY_MODE_MAX_JOINT_ACC_PCT = 40.0
 MX_RECOVERY_MODE_MAX_CART_LIN_VEL_MM_PER_SEC = 20.0
 MX_RECOVERY_MODE_MAX_CART_ANG_VEL_DEG_PER_SEC = 30.0
 MX_RECOVERY_MODE_MAX_CART_ACC_PCT = 40.0
 MX_EIP_MAJOR_VERSION = 2
-MX_EIP_MINOR_VERSION = 1
+MX_EIP_MINOR_VERSION = 3
 MX_PNET_MAJOR_VERSION = 1
 MX_PNET_MINOR_VERSION = 1
 MX_PNET_PATCH_VERSION = 0
 MX_NB_DYNAMIC_PDOS = 4
 
 
 class MxRobotMsgType(IntEnum):
@@ -54,15 +54,15 @@
 class MxRobotModel(IntEnum):
     MX_ROBOT_MODEL_UNKNOWN = 0,  # Unknown robot model
     MX_ROBOT_MODEL_M500_R1 = 1,  # M500 R1 Robot
     MX_ROBOT_MODEL_M500_R2 = 2,  # M500 R2 Robot
     MX_ROBOT_MODEL_M500_R3 = 3,  # M500 R3 Robot
     MX_ROBOT_MODEL_M500_R4 = 4,  # M500 R4 Robot
     MX_ROBOT_MODEL_M1000_R1 = 10,  # Meca-1000 robot, R1
-    MX_ROBOT_MODEL_SCARA_R1 = 20,  # Scara robot, R1
+    MX_ROBOT_MODEL_MCS500_R1 = 20,  # Scara robot, R1
 
 
 class MxEventSeverity(IntEnum):
     MX_EVENT_SEVERITY_SILENT = 0,  # Trace event in robot log
     MX_EVENT_SEVERITY_WARNING = 1,  # Send status code on event
     MX_EVENT_SEVERITY_PAUSE_MOTION = 2,  # Send status code and pause motion on event
     MX_EVENT_SEVERITY_CLEAR_MOTION = 3,  # Send status code, pause and clear motion on event
@@ -72,14 +72,28 @@
 
 class MxTorqueLimitsMode(IntEnum):
     MX_TORQUE_LIMITS_DETECT_ALL = 0,  # Always check if torque is within limits
     MX_TORQUE_LIMITS_DETECT_SKIP_ACCEL = 1,  # Do not check if torque is within limits during acceleration or
     MX_TORQUE_LIMITS_INVALID = 0xFFFFFFFF,  # Set consistent sizeof(MxTorqueLimitsMode)
 
 
+class MxIoBankId(IntEnum):
+    MX_IO_BANK_ID_UNDEFINED = 0,
+    MX_IO_BANK_ID_PSU = 1,  # IO pins from Power supply.
+    MX_IO_BANK_ID_IO_MODULE = 2,  # IOs from the IO expansion module.
+MX_IO_BANK_NAME_PSU = "PSU"  # \ref MX_IO_BANK_ID_PSU
+MX_IO_BANK_NAME_IO_MODULE = "IoModule"  # \ref MX_IO_BANK_ID_IO_MODULE
+
+
+class MxDigitalIoState(IntEnum):
+    MX_DIGITAL_IO_STATE_STAY = -1,  # Leave previous state
+    MX_DIGITAL_IO_STATE_0 = 0,  # Set digital output value to 0
+    MX_DIGITAL_IO_STATE_1 = 1,  # Set digital output value to 1
+
+
 class MxCollisionAvoidanceMode(IntEnum):
     MX_COLLISION_MODE_SELF_COLLISION_DETECTION = 0,
     MX_COLLISION_MODE_TCP_IN_WORKSPACE = 1,
     MX_COLLISION_MODE_ROBOT_IN_WORKSPACE = 2,
     MX_COLLISION_MODE_FULL_COLLISION_DETECTION = 3,
 
 
@@ -114,27 +128,32 @@
     MX_MOTION_CMD_TYPE_SETCONF = 15,  # Set the desired inverse kinematic config for MovePose.
     MX_MOTION_CMD_TYPE_SETAUTOCONF = 16,  # Enable or disable automatic configuration for inverse kinematic
     MX_MOTION_CMD_TYPE_SETCHECKPOINT = 17,  # Inserts a "set checkpoint" command between two moves, so robot status
     MX_MOTION_CMD_TYPE_GRIPPEROPENCLOSE = 18,  # Open or close the gripper
     MX_MOTION_CMD_TYPE_GRIPPERVEL = 19,  # Limit the velocity of the gripper fingers in percent
     MX_MOTION_CMD_TYPE_GRIPPERFORCE = 20,  # Limit the grip force of the gripper in percent
     MX_MOTION_CMD_TYPE_MOVEJOINTSVEL = 21,  # Set current mode to "join velocity mode"
-    MX_MOTION_CMD_TYPE_MOVELINVELWRF = 22,  # Set current mode to "cartesian WRF velocity mode"
-    MX_MOTION_CMD_TYPE_MOVELINVELTRF = 23,  # Set current mode to "cartesian TRF velocity mode"
+    MX_MOTION_CMD_TYPE_MOVELINVELWRF = 22,  # Set current mode to "Cartesian WRF velocity mode"
+    MX_MOTION_CMD_TYPE_MOVELINVELTRF = 23,  # Set current mode to "Cartesian TRF velocity mode"
     MX_MOTION_CMD_TYPE_SETVELTIMEOUT = 24,  # Timeout for current velocity mode
     MX_MOTION_CMD_TYPE_SETCONFTURN = 25,  # Set the last joint turn conf (i.e. which turn should be used
     MX_MOTION_CMD_TYPE_SETAUTOCONFTURN = 26,  # Enable or disable automatic last joint turn selection
     MX_MOTION_CMD_TYPE_SETTORQUELIMITS = 27,  # Set torque limits for current motion
     MX_MOTION_CMD_TYPE_SETTORQUELIMITSCFG = 28,  # Set torque limits configuration for current motion
     MX_MOTION_CMD_TYPE_MOVEJOINTSREL = 29,  # Move each joint relative to current joint position
     MX_MOTION_CMD_TYPE_SETVALVESTATE = 30,  # Set valve box valves states
     MX_MOTION_CMD_TYPE_GRIPPERRANGE = 31,  # Set the Close and Open position that will be used when calling
     MX_MOTION_CMD_TYPE_GRIPPERPOS = 32,  # Move gripper to a specific position, in mm from the most closed
+    MX_MOTION_CMD_TYPE_SETJOINTVELLIMIT = 33,  # Max allowed joint vel (max for SetJointVel and linear moves).
+    MX_MOTION_CMD_TYPE_SETOUTPUTSTATE = 34,  # Set digital output states (through motion queue)
+    MX_MOTION_CMD_TYPE_SETOUTPUTSTATE_IMMEDIATE = 35,  # Set digital output states (immediate, bypass motion queue)
+    MX_MOTION_CMD_TYPE_SETIOSIM = 36,  # Set (or clear) IO simulation mode
     MX_MOTION_CMD_TYPE_START_OFFLINE_PROGRAM = 100,  # Start an offline program with specified id
     MX_MOTION_CMD_TYPE_SETDBG = 1000,  # Enable debug options on the robot. For Mecademic use only.
+    MX_MOTION_CMD_TYPE_MG2BUSDBG = 1001,  # Send custom command on Mg2 bus. For Mecademic use only.
 
 
 class MxEip_DynamicType(IntEnum):
     MX_EIP_DYNAMIC_AUTO = 0,
     MX_EIP_DYNAMIC_CFG_FW_VERSION = 1,
     MX_EIP_DYNAMIC_CFG_PRODUCT_TYPE = 2,
     MX_EIP_DYNAMIC_CFG_ROBOT_SERIAL = 3,
@@ -150,14 +169,17 @@
     MX_EIP_DYNAMIC_CFG_MODEL_JOINT_LIMITS_4_5_6 = 13,
     MX_EIP_DYNAMIC_CFG_JOINT_LIMITS_1_2_3 = 14,
     MX_EIP_DYNAMIC_CFG_JOINT_LIMITS_4_5_6 = 15,
     MX_EIP_DYNAMIC_CFG_EXT_TOOL_FW_VERSION = 16,
     MX_EIP_DYNAMIC_CFG_WORKSPACE_LIMITS_CFG = 17,
     MX_EIP_DYNAMIC_CFG_WORKSPACE_LIMITS = 18,
     MX_EIP_DYNAMIC_CFG_TOOL_SPHERE = 19,
+    MX_EIP_DYNAMIC_CFG_CALIBRATION = 30,
+    MX_EIP_DYNAMIC_CFG_BRF_OFFSET = 31,
+    MX_EIP_DYNAMIC_CFG_FRF_OFFSET = 35,
     MX_EIP_DYNAMIC_MQ_CONF = 20,
     MX_EIP_DYNAMIC_MQ_PARAMS = 21,
     MX_EIP_DYNAMIC_MQ_VEL_ACCEL = 22,
     MX_EIP_DYNAMIC_MQ_GRIPPER_CFG = 23,
     MX_EIP_DYNAMIC_MQ_TORQUE_LIMITS_CFG = 24,
     MX_EIP_DYNAMIC_MQ_TORQUE_LIMITS = 25,
     MX_EIP_DYNAMIC_RT_TARGET_JOINT_POS = 30,  # Present in basic PDOs already
@@ -173,14 +195,16 @@
     MX_EIP_DYNAMIC_RT_CART_VEL = 44,
     MX_EIP_DYNAMIC_RT_CONF = 45,
     MX_EIP_DYNAMIC_RT_ACCELEROMETER_5 = 46,
     MX_EIP_DYNAMIC_RT_WRF = 50,  # Present in basic PDOs already
     MX_EIP_DYNAMIC_RT_TRF = 51,  # Present in basic PDOs already
     MX_EIP_DYNAMIC_RT_EXTTOOL_STATUS = 52,
     MX_EIP_DYNAMIC_RT_GRIPPER_VALVE_STATE = 53,
+    MX_EIP_DYNAMIC_RT_PSU_IO_STATE = 71,  # Digital outputs and inputs from the Mcs500 PSU
+    MX_EIP_DYNAMIC_RT_IO_MODULE_IO_STATE = 72,  # Digital outputs and inputs from the Mcs500 IO module
     MX_EIP_DYNAMIC_INTERNAL_SET_DBG = 0x08000000,
     MX_EIP_DYNAMIC_FORCE_32_BITS = 0xFFFFFFFF,
 MX_EIP_DYNAMIC_INTERNAL_MASK = 0x0FFFFFFF
 MX_EIP_DYNAMIC_INTERNAL_SHIFT = 28  # Bit shift that corresponds to MX_EIP_DYNAMIC_INTERNAL_MASK
 MX_ST_EXCESSIVE_TRQ = 3028  # replaced by MX_ST_TORQUE_LIMIT_STATUS
 
 
@@ -211,30 +235,31 @@
     MX_ST_ILLEGAL_WHILE_SAVING = 1031,  # This command is illegal while saving an offline program.
     MX_ST_HOMING_JOINTS_OUT_OF_RANGE = 1032,  # DEPRECATED. Was used only on release 8.X
     MX_ST_START_CONF_MISMATCH = 1033,  # Requested move blocked because start pos is not in requested conf
     MX_ST_NO_GRIPPER = 1038,  # No gripper is connected, command can't be executed.
     MX_ST_CMD_FAILED = 1040,  # Command failed (generic response for various simple commands)
     MX_ST_NO_VBOX = 1041,  # No pneumatic module is connected.
     MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED = 1042,  # Switching external tool type is only possible when the robot
+    MX_ST_INVALID_BANK_ID = 1043,  # The specified IO bank is not present on this robot.
     MX_ST_OFFLINE_PROGRAM_LIST_ERR = 1500,  # Failed "ListPrograms" API command
     MX_ST_OFFLINE_PROGRAM_LOAD_ERR = 1501,  # Failed "LoadProgram" API command
     MX_ST_OFFLINE_PROGRAM_SAVE_ERR = 1502,  # Failed "SaveProgram" API command
     MX_ST_OFFLINE_PROGRAM_DELETE_ERR = 1503,  # Failed "DeleteProgram" API command
     MX_ST_ACTIVATED = 2000,  # Motors were successfully activated
     MX_ST_HOME_DONE = 2002,  # Homing done.
     MX_ST_DEACTIVATED = 2004,  # Motors deactivated.
     MX_ST_ERROR_RESET = 2005,  # The error was reset. Commands can now be sent again.
     MX_ST_NO_ERROR_RESET = 2006,  # There was no error to reset.
     MX_ST_GET_STATUS_ROBOT = 2007,  # This event reports the status of the robot.
     MX_ST_BRAKES_OFF = 2008,  # All brakes are now released.
     MX_ST_MASTER_DONE = 2009,  # Mastering now done.
     MX_ST_BRAKES_ON = 2010,  # All brakes are now set.
-    MX_ST_GET_MOTION_STATUS = 2011,  # This event reports the motion status of the robot (JSON format).
-    MX_ST_GET_WRF = 2013,  # Response to GetTrf
-    MX_ST_GET_TRF = 2014,  # Response to GetWrf
+    MX_ST_GET_WRF = 2013,  # Response to GetWrf
+    MX_ST_GET_TRF = 2014,  # Response to GetTrf
+    MX_ST_GET_TIME_SCALING = 2015,  # Response to GetTimeScaling
     MX_ST_GET_JOINTS = 2026,  # "GetJoints" response (current joint angles in degrees).
     MX_ST_GET_POSE = 2027,  # "GetPose" response (current position in mm, Euler angles in degrees).
     MX_ST_GET_AUTO_CONF = 2028,
     MX_ST_GET_CONF = 2029,  # "GetConf" response (current shoulder, elbow, wrist conf)
     MX_ST_GET_AUTO_CONF_TURN = 2031,
     MX_ST_GET_CONF_TURN = 2036,  # "GetConfTurn" response
     MX_ST_PAUSE_MOTION = 2042,  # Motion paused.
@@ -246,27 +271,30 @@
     MX_ST_RECOVERY_MODE_ON = 2049,  # Robot is now in recovery mode.
     MX_ST_RECOVERY_MODE_OFF = 2050,  # Robot is no more in recovery mode.
     MX_ST_RECOVERY_VEL_CAP = 2051,  # Recovery mode has capped velocity.
     MX_ST_EOM_ON = 2052,  # End of movement events are enabled.
     MX_ST_EOM_OFF = 2053,  # End of movement events are disabled.
     MX_ST_EOB_ON = 2054,  # End of block events are enabled.
     MX_ST_EOB_OFF = 2055,  # End of block events are enabled.
+    MX_ST_IO_SIM = 2056,  # Response to GetIoSim.
     MX_ST_START_SAVING = 2060,  # Offline program saving now started.
     MX_ST_N_CMD_SAVED = 2061,  # Offline program saving done (reports number of saved commands)
     MX_ST_OFFLINE_START = 2063,  # Offline program started to run.
     MX_ST_OFFLINE_LOOP_ON = 2064,  # Offline program loop is enabled.
     MX_ST_OFFLINE_LOOP_OFF = 2065,  # Offline program loop is disabled.
     MX_ST_GET_STATUS_GRIPPER = 2079,  # "GetStatusGripper" response (see pdf doc for response fields meaning).
     MX_ST_GET_CMD_PENDING_COUNT = 2080,  # Number of pending commands in the queue.
     MX_ST_GET_FW_VERSION = 2081,  # The firmware version running on the robot.
     MX_ST_GET_FW_VERSION_FULL = 2082,  # More detailed info about the firmware version running on the robot.
     MX_ST_GET_ROBOT_SERIAL = 2083,  # Current robot serial number (response to GetRobotSerial and SetRobotSerial)
     MX_ST_GET_PRODUCT_TYPE = 2084,  # Current product type (Meca500...)
     MX_ST_CMD_SUCCESSFUL = 2085,  # Command successful (generic response for various simple commands)
     MX_ST_GET_EXT_TOOL_FW_VERSION = 2086,  # "GetExtToolFwVersion" response with current gripper firmware version.
+    MX_ST_GET_EXT_PORT_COMM_ERRORS = 2087,  # "GetExtPortCommErrors" response.
+    MX_ST_GET_EXT_TOOL_COMM_ERRORS = 2088,  # "GetExtToolCommErrors" response.
     MX_ST_GET_NETWORK_CONFIG = 2089,  # "GetNetworkConfig" response (JSON format)
     MX_ST_GET_JOINT_LIMITS = 2090,  # "GetJointLimits" response (joint nb, min, max)
     MX_ST_SET_JOINT_LIMITS = 2092,  # "SetJointLimits" success response
     MX_ST_SET_JOINT_LIMITS_CFG = 2093,  # "SetJointLimitsCfg" success response (joint limits enabled)
     MX_ST_GET_JOINT_LIMITS_CFG = 2094,  # "GetJointLimitsCfg" response
     MX_ST_GET_ROBOT_NAME = 2095,  # "GetRobotName" response
     MX_ST_SET_CTRL_PORT_MONIT = 2096,  # "SetCtrlPortMonitoring" response
@@ -280,14 +308,17 @@
     MX_ST_GET_JOINT_OFFSET = 2112,  # "GetJointOffset" response
     MX_ST_GET_MODEL_JOINT_LIMITS = 2113,  # "GetModelJointLimits" response
     MX_ST_GET_TEST_BENCH_MODE = 2114,  # "GetTestBenchMode" response
     MX_ST_GET_MOTION_OPTIONS = 2115,  # "GetMotionOptions" response
     MX_ST_GET_MONITORING_INTERVAL = 2116,  # "GetMonitoringInterval" response
     MX_ST_GET_REAL_TIME_MONITORING = 2117,  # "GetRealTimeMonitoring" response
     MX_ST_GET_NETWORK_OPTIONS = 2119,  # "GetNetworkOptions" response
+    MX_ST_GET_BRF_OFFSET = 2120,  # "GetBrfOffset" response
+    MX_ST_GET_FRF_OFFSET = 2121,  # "GetFrfOffset" response
+    MX_ST_GET_ROBOT_CALIBRATED = 2122,  # "GetRobotCalibrated" response
     MX_ST_GET_RTC = 2140,  # "GetRtc" response
     MX_ST_GET_BLENDING = 2150,  # "GetBlending" response
     MX_ST_GET_VEL_TIMEOUT = 2151,  # "GetVelTimeout" response
     MX_ST_GET_JOINT_VEL = 2152,  # "GetJointVel" response
     MX_ST_GET_JOINT_ACC = 2153,  # "GetJointAcc" response
     MX_ST_GET_CART_LIN_VEL = 2154,  # "GetCartLinVel" response
     MX_ST_GET_CART_ANG_VEL = 2155,  # "GetCartAngVel" response
@@ -300,14 +331,17 @@
     MX_ST_GET_GRIPPER_RANGE = 2162,  # "GetGipperRange" response
     MX_ST_GET_WORKSPACE_LIMITS_CFG = 2163,  # "GetWorkspaceLimitsCfg" response
     MX_ST_SET_WORKSPACE_LIMITS_CFG = 2164,  # "SetWorkspaceLimitsCfg" response
     MX_ST_GET_WORKSPACE_LIMITS = 2165,  # "GetWorkspaceLimits" response
     MX_ST_SET_WORKSPACE_LIMITS = 2166,  # "SetWorkspaceLimits" response
     MX_ST_GET_TOOL_SPHERE = 2167,  # "GetToolSphere" response
     MX_ST_SET_TOOL_SPHERE = 2168,  # "SetToolSphere" response
+    MX_ST_GET_JOINT_VEL_LIMIT = 2169,  # "GetJointVelLimit" response
+    MX_ST_SET_CALIBRATION_CFG = 2170,  # "SetCalibrationCfg" response
+    MX_ST_GET_CALIBRATION_CFG = 2171,  # "GetCalibrationCfg" response
     MX_ST_RT_TARGET_JOINT_POS = 2200,  # Timestamp + joint positions in degrees
     MX_ST_RT_TARGET_CART_POS = 2201,  # Timestamp + Cartesian position (in mm, Euler angles in degrees).
     MX_ST_RT_TARGET_JOINT_VEL = 2202,  # Timestamp + joint velocity in degrees per second
     MX_ST_RT_TARGET_JOINT_TORQ = 2203,  # Timestamp + joint torque ratio in percent
     MX_ST_RT_TARGET_CART_VEL = 2204,  # Timestamp + Cartesian velocity (in mm, Euler angles in degrees per sec).
     MX_ST_RT_TARGET_CONF = 2208,  # Timestamp + conf that corresponds to MX_ST_RT_TARGET_JOINT_POS
     MX_ST_RT_TARGET_CONF_TURN = 2209,  # Timestamp + last joint turn that corresponds to MX_ST_RT_TARGET_JOINT_POS
@@ -326,18 +360,25 @@
     MX_ST_RT_CYCLE_END = 2230,  # Timestamp of the real-time cycle which has just ended.
     MX_ST_RT_EXTTOOL_STATUS = 2300,  # Timestamp + external tool status
     MX_ST_RT_VALVE_STATE = 2310,  # Timestamp + valve state
     MX_ST_RT_GRIPPER_STATE = 2320,  # Timestamp + gripper state
     MX_ST_RT_GRIPPER_FORCE = 2321,  # Timestamp + gripper force in percent
     MX_ST_RT_GRIPPER_POS = 2322,  # Timestamp + gripper position in percent
     MX_ST_RT_GRIPPER_VEL = 2323,  # Timestamp + gripper speed in percent
+    MX_ST_RT_IO_STATUS = 2330,  # Timestamp + IO module status
+    MX_ST_RT_OUTPUT_STATE = 2340,  # Timestamp + bankId + output states
+    MX_ST_RT_INPUT_STATE = 2341,  # Timestamp + bankId + input states
+    MX_ST_RT_DEBUG_MG2_SAFE_MCU = 2400,  # Safe MCU debug status.
+    MX_ST_RT_DEBUG_MG2_DRIVES = 2401,  # Drives debug status.
+    MX_ST_RT_DEBUG_MG2_PSU = 2402,  # PSU debug status.
     MX_ST_OFFLINE_PROGRAM_LIST = 2500,  # Response to "ListPrograms" API command
     MX_ST_OFFLINE_PROGRAM_LOAD = 2501,  # Response to "LoadProgram" API command
     MX_ST_OFFLINE_PROGRAM_SAVE = 2502,  # Response to "SaveProgram" API command
     MX_ST_OFFLINE_PROGRAM_DELETE = 2503,  # Response to "DeleteProgram" API command
+    MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE = 2504,  # Response to "StartDemoProgram" API command.
     MX_ST_CONNECTED = 3000,  # Confirms connection to robot.
     MX_ST_USER_ALREADY = 3001,  # Another user is already connected to the robot (current connection refused).
     MX_ST_UPGRADE_IN_PROGRESS = 3002,  # A firmware upgrade is in progress (current connection refused).
     MX_ST_CMD_TOO_LONG = 3003,  # Command string is too long (or missing NUL character).
     MX_ST_EOM = 3004,  # The robot has stopped moving.
     MX_ST_ERROR_MOTION = 3005,  # Motion error (probably collision or overload). This error can be reset.
     MX_ST_ERROR_DRIVE_COMM = 3006,  # Comm error with drives. This error cannot be reset.
@@ -345,14 +386,16 @@
     MX_ST_EOB = 3012,  # No more motion command are in queue and robot is no more moving.
     MX_ST_END_OFFLINE = 3013,  # The offline program has finished.
     MX_ST_CANT_SAVE_OFFLINE = 3014,  # There was a problem saving the offline program.
     MX_ST_IGNORING_CMD = 3016,  # Non-motion command ignored during execution of an offline program.
     MX_ST_NO_OFFLINE_SAVED = 3017,  # There is no program in memory.
     MX_ST_OFFLINE_LOOP = 3018,  # The offline program is being restarted (looped).
     MX_ST_OFFLINE_INVALID = 3020,  # The offline program is invalid and can't be played
+    MX_ST_DEV_MODE = 3021,  # The robot is running in developer mode (non official binary)
+    MX_ST_PSU_DONGLE_STATUS = 3022,  # Power-supply USB debug dongle status (sent only when detected)
     MX_ST_ERROR_GRIPPER = 3025,  # The gripper reported an error.
     MX_ST_MAINTENANCE_CHECK = 3026,  # A hardware problem was detected. Contact Mecademic support.
     MX_ST_INTERNAL_ERROR = 3027,  # Unknown internal error occurred.
     MX_ST_TORQUE_LIMIT_STATUS = 3028,  # "GetTorqueLimitsStatus" response and torque limit status update.
     MX_ST_TORQUE_LIMIT_ERROR = 3029,  # Excessive torque error occurred.
     MX_ST_CHECKPOINT_REACHED = 3030,  # A previously set checkpoint (with given id) was just reached.
     MX_ST_TEXT_API_ERROR = 3031,  # A previously received text API command was incorrect.
@@ -363,14 +406,18 @@
     MX_ST_TCP_DUMP_DONE = 3036,  # TCPDump has ended
     MX_ST_ERROR_VBOX = 3037,  # The pneumatic module reported an error
     MX_ST_FW_UPDATE_PROGRESS = 3038,  # Firmware update progress (JSON format)
     MX_ST_EXT_TOOL_NEED_UPDATE = 3039,  # The external tool need a firmware update.
     MX_ST_COLLISION_STATUS = 3040,  # Collision status update
     MX_ST_COLLISION_ERROR = 3041,  # Collision error occurred.
     MX_ST_FW_NEED_REINSTALL = 3042,  # Firmware must be reinstalled again.
+    MX_ST_EXT_TOOL_COMM_ERR = 3043,  # Excessive communication errors with external tool.
+    MX_ST_EXT_PORT_COMM_ERR = 3044,  # Abnormal communication error with external port.
+    MX_ST_COLLISION_STOP = 3045,  # Robot has decelerated due to imminent collision.
+    MX_ST_PSU_ERROR = 3046,  # Robot power supply has non-resettable error.
     MX_ST_ESTOP = 3070,  # The EStop condition raised
     MX_ST_INVALID = 0xFFFFFFFF,
 MX_ST_EXTTOOL_SIM_OFF = 2048
 
 
 class MxRobotState(IntEnum):
     MX_ROBOT_STATE_UNKNOWN = 0,
@@ -380,60 +427,92 @@
     MX_ROBOT_STATE_ACTIVATED = 4,
     MX_ROBOT_STATE_HOMING = 5,
     MX_ROBOT_STATE_MASTERING = 6,
     MX_ROBOT_STATE_RUN = 7,
     MX_ROBOT_STATE_DEACTIVATING = 9,
 MX_JSON_KEY_CODE = "code"  # Key for the status/command code in JSON message
 MX_JSON_KEY_DATA = "data"  # Key for the status/command data in JSON message
+MX_JSON_KEY_TIMESTAMP_US = "timestampUs"  # Robot timestamp in microseconds
 MX_JSON_KEY_META_DATA = "metaData"  # Key for the status/command meta data in JSON message
 MX_JSON_KEY_MSG_TYPE = "msgType"  # Key for message type inside metaData. Values from MxRobotMsgType
 MX_JSON_KEY_FW_UPDATE_PROGRESS_UPDATING = "updating"  # bool: Firmware update has started
 MX_JSON_KEY_FW_UPDATE_PROGRESS_VERSION = "version"  # string: Firmware version we're updating to
 MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR = "error"  # bool: Firmware update has failed
 MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR_MSG = "errorMsg"  # string: User message if failed
 MX_JSON_KEY_FW_UPDATE_PROGRESS_PCT = "progressPct"  # float: Update percentage (0 to 100)
 MX_JSON_KEY_FW_UPDATE_PROGRESS_STEP = "step"  # string: Current update step (human readable)
+MX_JSON_KEY_FW_UPDATE_PROGRESS_REBOOT_DONE = "rebootDone"  # bool: Tells if robot reboot was done
 MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG = "log"  # array of {time, msg}: Update history
 MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG_TIME = "time"  # int: Absolute time of this log (seconds since Epoch)
+MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG_FAILED = "failed"  # bool: Indicate if this step has failed
+MX_JSON_KEY_ROBOT_STATUS = "robotStatus"  # Parent key for following child keys:
 MX_JSON_KEY_STATUS_ROBOT_STATE = "state"  # integer: Value (as integer) from enum MxRobotState
 MX_JSON_KEY_STATUS_ROBOT_SIM = "simMode"  # bool: Sim mode
 MX_JSON_KEY_STATUS_ROBOT_RECOVERY = "recovery"  # bool: Recovery enabled
 MX_JSON_KEY_STATUS_ROBOT_BRAKES = "brakesEngaged"  # bool: Brakes engaged
 MX_JSON_KEY_STATUS_ROBOT_ERR = "errorCode"  # integer: Error code (0 if no error)
 MX_JSON_KEY_STATUS_ROBOT_ERR_MSG = "errorMsg"  # string: User message related to error code
 MX_JSON_KEY_STATUS_ROBOT_ESTOP = "eStop"  # bool: ESTOP condition is active
+MX_JSON_KEY_STATUS_ROBOT_ESTOP_RESETTABLE = "eStopResettable"  # bool: ESTOP cleared but awaiting Reset
+MX_JSON_KEY_MOTION_STATUS = "motionStatus"  # Parent key for following child keys:
 MX_JSON_KEY_MOTION_ROBOT_CHECKPOINT = "checkpoint"  # integer: Most recently reached checkpoint id
 MX_JSON_KEY_MOTION_ROBOT_OFFLINE_PRGRM = "offlineProgramId"  # integer: Running offline-program Id
 MX_JSON_KEY_MOTION_ROBOT_HOLD = "paused"  # bool: Hold motion
 MX_JSON_KEY_MOTION_ROBOT_EOM = "eom"  # bool: End of motion
 MX_JSON_KEY_MOTION_ROBOT_EOB = "eob"  # bool: End of block
 MX_JSON_KEY_MOTION_ROBOT_PSTOP2 = "pStop2"  # bool: PSTOP2 condition is active
 MX_JSON_KEY_MOTION_ROBOT_PSTOP2_RESETTABLE = "pStop2Resettable"  # bool: PSTOP2 condition can be reset
 MX_JSON_KEY_MOTION_ROBOT_EXCESSIVE_TORQ = "excessiveTorque"  # bool: Excessive torque ratio
+MX_JSON_KEY_EXTTOOL_STATUS_SIM_TYPE = "simType"  # Values from enum MxExtToolType
+MX_JSON_KEY_EXTTOOL_STATUS_PHYSICAL_TYPE = "physicalType"  # Values from enum MxExtToolType
+MX_JSON_KEY_EXTTOOL_STATUS_HOMED = "homed"  # bool: Tool homing was done
+MX_JSON_KEY_EXTTOOL_STATUS_ERROR = "error"  # bool: True when in error state
+MX_JSON_KEY_EXTTOOL_STATUS_OVERHEAT = "overheat"  # bool: True when in overheat state
+MX_JSON_KEY_EXTTOOL_STATUS_COMM_ERR = "commErrWarning"  # bool: True when some comm errors (not yet in err)
+MX_JSON_KEY_IO_STATUS_BANK_ID = "bankId"  # integer: BankId we're returning status for
+MX_JSON_KEY_IO_STATUS_BANK_NAME = "bankName"  # integer: Bank name we're returning status for
+MX_JSON_KEY_IO_STATUS_PRESENT = "present"  # bool: Indicate if this IO module is present
+MX_JSON_KEY_IO_STATUS_NB_INPUTS = "nbDigitalInputs"  # integer: Number of digital inputs present
+MX_JSON_KEY_IO_STATUS_NB_OUTPUTS = "nbDigitalOutputs"  # integer: Number of digital outputs present
+MX_JSON_KEY_IO_STATUS_SIM_MODE = "simMode"  # bool: Tells if currently in simulation mode
+MX_JSON_KEY_IO_STATUS_ERROR = "error"  # integer: True when in error state
 MX_JSON_KEY_NETWORK_CONFIG_ROBOT_NAME = "name"  # string: The robot name (hostname on the network)
 MX_JSON_KEY_NETWORK_CONFIG_DHCP = "dhcp"  # bool: Indicate if IP is obtained using DHCP
 MX_JSON_KEY_NETWORK_CONFIG_IP = "ip"  # string: The IPv4 address of the robot
 MX_JSON_KEY_NETWORK_CONFIG_MASK = "mask"  # string: The netmask
 MX_JSON_KEY_NETWORK_CONFIG_GATEWAY = "gateway"  # string: The gateway address
 MX_JSON_KEY_NETWORK_CONFIG_MAC = "mac"  # string: The robot's MAC address
+MX_JSON_KEY_PSU_DONGLE_DETECTED = "detected"  # bool: True if dongle was detected and updated successfully
 MX_FW_UPDATE_UPLOAD_URL = "/fw-update"
 MX_GET_LOGS_URL = "/get-logs"
 MX_FW_UPDATE_STATUS_EXTRACTING = "Extracting files from firmware package..."
 MX_FW_UPDATE_STATUS_CLOSING_CONNECTIONS = "Closing connections and stacks..."
 MX_FW_UPDATE_STATUS_LAUNCH_SCRIPT = "Launching firmware update script..."
 MX_FW_UPDATE_STATUS_ANALYZING = "Analyzing files..."
 MX_FW_UPDATE_STATUS_DRIVE = "Updating drive #"  # Plus drive number
 MX_FW_UPDATE_STATUS_EXT_PORT = "Updating external port"
 MX_FW_UPDATE_STATUS_EXT_TOOL = "Updating external tool"
 MX_FW_UPDATE_STATUS_NO_FW_IMAGE = "(No firmware image in this package)"
 MX_FW_UPDATE_STATUS_FW_IMAGE = "Updating firmware image"
 MX_FW_UPDATE_STATUS_CLEANUP = "Cleanup after update"
 MX_FW_UPDATE_STATUS_REBOOTING = "Awaiting for robot to reboot"
+MX_FW_UPDATE_STATUS_BOOT_BIN = "Updating boot binary"
+MX_FW_UPDATE_STATUS_SAFE_BOOT = "Updating safe boot"
+MX_FW_UPDATE_STATUS_SAFE_MCU_MASTER = "Updating master SafeMCU"
+MX_FW_UPDATE_STATUS_SAFE_MCU_SLAVE = "Updating slave SafeMCU"
+MX_FW_UPDATE_STATUS_PSU_MASTER = "Updating master power supply"
+MX_FW_UPDATE_STATUS_PSU_SLAVE = "Updating slave power supply"
+MX_FW_UPDATE_STATUS_IO_MODULE = "Updating IO module"
+MX_FW_UPDATE_AVG_DURATION_SEC_MECA500 = 350
+MX_FW_UPDATE_REBOOT_DURATION_SEC_MECA500 = 60
+MX_FW_UPDATE_AVG_DURATION_SEC_MCS500 = 250
+MX_FW_UPDATE_REBOOT_DURATION_SEC_MCS500 = 120  # Note: rootfs update done during this reboot
 MX_CMD_TAG_ROBOT_CONTROL = "RobotControl"
 MX_CMD_TAG_EXT_TOOL = "ExternalTool"
+MX_CMD_TAG_IO_BANK = "IoBank"
 MX_CMD_TAG_MOTION = "Motion"
 MX_CMD_TAG_UTILITIES = "Utilities"
 MX_CMD_TAG_SYS_CFG = "SystemConfig"
 MX_CMD_TAG_PGM = "Program"
 MX_CMD_TAG_GET = "Get"
 MX_CMD_TAG_PERMANENT = "Permanent"
 MX_CMD_TAG_TEMPORARY = "Temporary"
@@ -534,14 +613,16 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_NO_GRIPPER, "MX_ST_NO_GRIPPER", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_CMD_FAILED):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CMD_FAILED, "MX_ST_CMD_FAILED", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_NO_VBOX):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_NO_VBOX, "MX_ST_NO_VBOX", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED, "MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED", is_error=True, is_resettable=True),
+    int(MxRobotStatusCode.MX_ST_INVALID_BANK_ID):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_INVALID_BANK_ID, "MX_ST_INVALID_BANK_ID", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LIST_ERR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LIST_ERR, "MX_ST_OFFLINE_PROGRAM_LIST_ERR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LOAD_ERR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LOAD_ERR, "MX_ST_OFFLINE_PROGRAM_LOAD_ERR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_SAVE_ERR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_SAVE_ERR, "MX_ST_OFFLINE_PROGRAM_SAVE_ERR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_DELETE_ERR):
@@ -554,16 +635,16 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_DEACTIVATED, "MX_ST_DEACTIVATED", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_ERROR_RESET):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_ERROR_RESET, "MX_ST_ERROR_RESET", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_NO_ERROR_RESET):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_NO_ERROR_RESET, "MX_ST_NO_ERROR_RESET", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_STATUS_ROBOT):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_STATUS_ROBOT, "MX_ST_GET_STATUS_ROBOT", is_error=False, is_resettable=False),
-    int(MxRobotStatusCode.MX_ST_GET_MOTION_STATUS):
-    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_MOTION_STATUS, "MX_ST_GET_MOTION_STATUS", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_TIME_SCALING):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_TIME_SCALING, "MX_ST_GET_TIME_SCALING", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_BRAKES_OFF):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_BRAKES_OFF, "MX_ST_BRAKES_OFF", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_MASTER_DONE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_MASTER_DONE, "MX_ST_MASTER_DONE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_BRAKES_ON):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_BRAKES_ON, "MX_ST_BRAKES_ON", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_WRF):
@@ -590,14 +671,16 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CLEAR_MOTION, "MX_ST_CLEAR_MOTION", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_SIM_ON):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_SIM_ON, "MX_ST_SIM_ON", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_SIM_OFF):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_SIM_OFF, "MX_ST_SIM_OFF", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_EXTTOOL_SIM):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EXTTOOL_SIM, "MX_ST_EXTTOOL_SIM", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_IO_SIM):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_IO_SIM, "MX_ST_IO_SIM", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_EOM_ON):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EOM_ON, "MX_ST_EOM_ON", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_EOM_OFF):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EOM_OFF, "MX_ST_EOM_OFF", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_EOB_ON):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EOB_ON, "MX_ST_EOB_ON", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_EOB_OFF):
@@ -618,14 +701,18 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_CMD_PENDING_COUNT, "MX_ST_GET_CMD_PENDING_COUNT", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_FW_VERSION):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_FW_VERSION, "MX_ST_GET_FW_VERSION", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_FW_VERSION_FULL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_FW_VERSION_FULL, "MX_ST_GET_FW_VERSION_FULL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_EXT_TOOL_FW_VERSION):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_EXT_TOOL_FW_VERSION, "MX_ST_GET_EXT_TOOL_FW_VERSION", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_EXT_PORT_COMM_ERRORS):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_EXT_PORT_COMM_ERRORS, "MX_ST_GET_EXT_PORT_COMM_ERRORS", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_EXT_TOOL_COMM_ERRORS):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_EXT_TOOL_COMM_ERRORS, "MX_ST_GET_EXT_TOOL_COMM_ERRORS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_ROBOT_SERIAL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_ROBOT_SERIAL, "MX_ST_GET_ROBOT_SERIAL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_PRODUCT_TYPE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_PRODUCT_TYPE, "MX_ST_GET_PRODUCT_TYPE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_CMD_SUCCESSFUL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CMD_SUCCESSFUL, "MX_ST_CMD_SUCCESSFUL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_SET_CTRL_PORT_MONIT):
@@ -646,14 +733,16 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_SET_JOINT_LIMITS_CFG, "MX_ST_SET_JOINT_LIMITS_CFG", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_WORKSPACE_LIMITS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_WORKSPACE_LIMITS, "MX_ST_GET_WORKSPACE_LIMITS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_WORKSPACE_LIMITS_CFG):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_WORKSPACE_LIMITS_CFG, "MX_ST_GET_WORKSPACE_LIMITS_CFG", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_TOOL_SPHERE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_TOOL_SPHERE, "MX_ST_GET_TOOL_SPHERE", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_CALIBRATION_CFG):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_CALIBRATION_CFG, "MX_ST_GET_CALIBRATION_CFG", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_JOINT_LIMITS_CFG):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_JOINT_LIMITS_CFG, "MX_ST_GET_JOINT_LIMITS_CFG", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_ROBOT_NAME):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_ROBOT_NAME, "MX_ST_GET_ROBOT_NAME", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_MODEL_VEL_LIMITS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_MODEL_VEL_LIMITS, "MX_ST_GET_MODEL_VEL_LIMITS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_CMD_DEF):
@@ -672,22 +761,30 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_MOTION_OPTIONS, "MX_ST_GET_MOTION_OPTIONS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_MONITORING_INTERVAL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_MONITORING_INTERVAL, "MX_ST_GET_MONITORING_INTERVAL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_REAL_TIME_MONITORING):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_REAL_TIME_MONITORING, "MX_ST_GET_REAL_TIME_MONITORING", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_NETWORK_OPTIONS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_NETWORK_OPTIONS, "MX_ST_GET_NETWORK_OPTIONS", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_BRF_OFFSET):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_BRF_OFFSET, "MX_ST_GET_BRF_OFFSET", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_FRF_OFFSET):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_FRF_OFFSET, "MX_ST_GET_FRF_OFFSET", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_ROBOT_CALIBRATED):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_ROBOT_CALIBRATED, "MX_ST_GET_ROBOT_CALIBRATED", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_RTC):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_RTC, "MX_ST_GET_RTC", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_BLENDING):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_BLENDING, "MX_ST_GET_BLENDING", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_VEL_TIMEOUT):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_VEL_TIMEOUT, "MX_ST_GET_VEL_TIMEOUT", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_JOINT_VEL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_JOINT_VEL, "MX_ST_GET_JOINT_VEL", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_GET_JOINT_VEL_LIMIT):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_JOINT_VEL_LIMIT, "MX_ST_GET_JOINT_VEL_LIMIT", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_JOINT_ACC):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_JOINT_ACC, "MX_ST_GET_JOINT_ACC", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_CART_LIN_VEL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_CART_LIN_VEL, "MX_ST_GET_CART_LIN_VEL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_CART_ANG_VEL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_GET_CART_ANG_VEL, "MX_ST_GET_CART_ANG_VEL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_GET_CART_ACC):
@@ -744,30 +841,42 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_GRIPPER_VEL, "MX_ST_RT_GRIPPER_VEL", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_EXTTOOL_STATUS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_EXTTOOL_STATUS, "MX_ST_RT_EXTTOOL_STATUS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_GRIPPER_STATE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_GRIPPER_STATE, "MX_ST_RT_GRIPPER_STATE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_VALVE_STATE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_VALVE_STATE, "MX_ST_RT_VALVE_STATE", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_RT_IO_STATUS):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_IO_STATUS, "MX_ST_RT_IO_STATUS", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_RT_OUTPUT_STATE):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_OUTPUT_STATE, "MX_ST_RT_OUTPUT_STATE", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_RT_INPUT_STATE):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_INPUT_STATE, "MX_ST_RT_INPUT_STATE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_CHECKPOINT):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_CHECKPOINT, "MX_ST_RT_CHECKPOINT", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_WRF):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_WRF, "MX_ST_RT_WRF", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_TRF):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_TRF, "MX_ST_RT_TRF", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_RT_CYCLE_END):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_CYCLE_END, "MX_ST_RT_CYCLE_END", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_RT_DEBUG_MG2_SAFE_MCU):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_DEBUG_MG2_SAFE_MCU, "MX_ST_RT_DEBUG_MG2_SAFE_MCU", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_RT_DEBUG_MG2_DRIVES):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_RT_DEBUG_MG2_DRIVES, "MX_ST_RT_DEBUG_MG2_DRIVES", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LIST):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LIST, "MX_ST_OFFLINE_PROGRAM_LIST", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LOAD):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_LOAD, "MX_ST_OFFLINE_PROGRAM_LOAD", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_SAVE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_SAVE, "MX_ST_OFFLINE_PROGRAM_SAVE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_DELETE):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_DELETE, "MX_ST_OFFLINE_PROGRAM_DELETE", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE, "MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_CONNECTED):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CONNECTED, "MX_ST_CONNECTED", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_USER_ALREADY):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_USER_ALREADY, "MX_ST_USER_ALREADY", is_error=True, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_UPGRADE_IN_PROGRESS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_UPGRADE_IN_PROGRESS, "MX_ST_UPGRADE_IN_PROGRESS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_CMD_TOO_LONG):
@@ -788,14 +897,18 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CANT_SAVE_OFFLINE, "MX_ST_CANT_SAVE_OFFLINE", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_IGNORING_CMD):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_IGNORING_CMD, "MX_ST_IGNORING_CMD", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_NO_OFFLINE_SAVED):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_NO_OFFLINE_SAVED, "MX_ST_NO_OFFLINE_SAVED", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_OFFLINE_LOOP):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_LOOP, "MX_ST_OFFLINE_LOOP", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_DEV_MODE):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_DEV_MODE, "MX_ST_DEV_MODE", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_PSU_DONGLE_STATUS):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_PSU_DONGLE_STATUS, "MX_ST_PSU_DONGLE_STATUS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_OFFLINE_INVALID):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_OFFLINE_INVALID, "MX_ST_OFFLINE_INVALID", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_ERROR_GRIPPER):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_ERROR_GRIPPER, "MX_ST_ERROR_GRIPPER", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_ERROR_VBOX):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_ERROR_VBOX, "MX_ST_ERROR_VBOX", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_MAINTENANCE_CHECK):
@@ -804,14 +917,16 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_INTERNAL_ERROR, "MX_ST_INTERNAL_ERROR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_TORQUE_LIMIT_STATUS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_TORQUE_LIMIT_STATUS, "MX_ST_TORQUE_LIMIT_STATUS", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_TORQUE_LIMIT_ERROR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_TORQUE_LIMIT_ERROR, "MX_ST_TORQUE_LIMIT_ERROR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_COLLISION_STATUS):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_COLLISION_STATUS, "MX_ST_COLLISION_STATUS", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_COLLISION_STOP):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_COLLISION_STOP, "MX_ST_COLLISION_STOP", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_COLLISION_ERROR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_COLLISION_ERROR, "MX_ST_COLLISION_ERROR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_CHECKPOINT_REACHED):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_CHECKPOINT_REACHED, "MX_ST_CHECKPOINT_REACHED", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_TEXT_API_ERROR):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_TEXT_API_ERROR, "MX_ST_TEXT_API_ERROR", is_error=True, is_resettable=True),
     int(MxRobotStatusCode.MX_ST_NO_VALID_CFG):
@@ -828,14 +943,20 @@
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EXT_TOOL_NEED_UPDATE, "MX_ST_EXT_TOOL_NEED_UPDATE", is_error=True, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_FW_NEED_REINSTALL):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_FW_NEED_REINSTALL, "MX_ST_FW_NEED_REINSTALL", is_error=True, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_PSTOP2):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_PSTOP2, "MX_ST_PSTOP2", is_error=False, is_resettable=False),
     int(MxRobotStatusCode.MX_ST_ESTOP):
     RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_ESTOP, "MX_ST_ESTOP", is_error=False, is_resettable=False),
+    int(MxRobotStatusCode.MX_ST_EXT_PORT_COMM_ERR):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EXT_PORT_COMM_ERR, "MX_ST_EXT_PORT_COMM_ERR", is_error=True, is_resettable=True),
+    int(MxRobotStatusCode.MX_ST_EXT_TOOL_COMM_ERR):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_EXT_TOOL_COMM_ERR, "MX_ST_EXT_TOOL_COMM_ERR", is_error=True, is_resettable=True),
+    int(MxRobotStatusCode.MX_ST_PSU_ERROR):
+    RobotStatusCodeInfo(MxRobotStatusCode.MX_ST_PSU_ERROR, "MX_ST_PSU_ERROR", is_error=True, is_resettable=False),
 }
 #
 # C constants from file mx_exttool_def.h
 #
 MX_EXT_TOOL_MPM500_NB_VALVES = 2  # MPM500 valve quantity
 MX_EXT_TOOL_VBOX_MAX_VALVES = 6  # Maximum valve quantity for comm protocol
```

### Comparing `mecademicpy-1.3.0/mecademicpy/mx_robot_def_legacy.py` & `mecademicpy-1.4.0/mecademicpy/mx_robot_def_legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 MX_JOINT_LIMIT_MIN_RANGE_DEG = 25  # Last joint requires ~12 deg during homing in either direction
 MX_RECOVERY_MODE_MAX_JOINT_VEL_PCT = 5.0
 MX_RECOVERY_MODE_MAX_JOINT_ACC_PCT = 40.0
 MX_RECOVERY_MODE_MAX_CART_LIN_VEL_MM_PER_SEC = 20.0
 MX_RECOVERY_MODE_MAX_CART_ANG_VEL_DEG_PER_SEC = 30.0
 MX_RECOVERY_MODE_MAX_CART_ACC_PCT = 40.0
 MX_EIP_MAJOR_VERSION = 2
-MX_EIP_MINOR_VERSION = 1
+MX_EIP_MINOR_VERSION = 3
 MX_PNET_MAJOR_VERSION = 1
 MX_PNET_MINOR_VERSION = 1
 MX_PNET_PATCH_VERSION = 0
 MX_NB_DYNAMIC_PDOS = 4
 MX_ROBOT_MSG_TYPE_REQUEST = 0  # Request from the user
 MX_ROBOT_MSG_TYPE_REQUEST_INTERNAL = 1  # Internal request from the user
 MX_ROBOT_MSG_TYPE_RESPONSE = 10  # Response to user request
@@ -48,24 +48,32 @@
 MX_ROBOT_MSG_TYPE_MON_EVENT_PERIODIC_PREFIX = "!"  # Prefix for MX_ROBOT_MSG_TYPE_MON_EVENT_PERIODIC
 MX_ROBOT_MODEL_UNKNOWN = 0  # Unknown robot model
 MX_ROBOT_MODEL_M500_R1 = 1  # M500 R1 Robot
 MX_ROBOT_MODEL_M500_R2 = 2  # M500 R2 Robot
 MX_ROBOT_MODEL_M500_R3 = 3  # M500 R3 Robot
 MX_ROBOT_MODEL_M500_R4 = 4  # M500 R4 Robot
 MX_ROBOT_MODEL_M1000_R1 = 10  # Meca-1000 robot, R1
-MX_ROBOT_MODEL_SCARA_R1 = 20  # Scara robot, R1
+MX_ROBOT_MODEL_MCS500_R1 = 20  # Scara robot, R1
 MX_EVENT_SEVERITY_SILENT = 0  # Trace event in robot log
 MX_EVENT_SEVERITY_WARNING = 1  # Send status code on event
 MX_EVENT_SEVERITY_PAUSE_MOTION = 2  # Send status code and pause motion on event
 MX_EVENT_SEVERITY_CLEAR_MOTION = 3  # Send status code, pause and clear motion on event
 MX_EVENT_SEVERITY_ERROR = 4  # Send status code, pause, clear motion and go in error mode on event
 MX_EVENT_SEVERITY_INVALID = 0xFFFFFFFF  # Set consistent sizeof(MxEventSeverity)
 MX_TORQUE_LIMITS_DETECT_ALL = 0  # Always check if torque is within limits
 MX_TORQUE_LIMITS_DETECT_SKIP_ACCEL = 1  # Do not check if torque is within limits during acceleration or
 MX_TORQUE_LIMITS_INVALID = 0xFFFFFFFF  # Set consistent sizeof(MxTorqueLimitsMode)
+MX_IO_BANK_ID_UNDEFINED = 0
+MX_IO_BANK_ID_PSU = 1  # IO pins from Power supply.
+MX_IO_BANK_ID_IO_MODULE = 2  # IOs from the IO expansion module.
+MX_IO_BANK_NAME_PSU = "PSU"  # \ref MX_IO_BANK_ID_PSU
+MX_IO_BANK_NAME_IO_MODULE = "IoModule"  # \ref MX_IO_BANK_ID_IO_MODULE
+MX_DIGITAL_IO_STATE_STAY = -1  # Leave previous state
+MX_DIGITAL_IO_STATE_0 = 0  # Set digital output value to 0
+MX_DIGITAL_IO_STATE_1 = 1  # Set digital output value to 1
 MX_COLLISION_MODE_SELF_COLLISION_DETECTION = 0
 MX_COLLISION_MODE_TCP_IN_WORKSPACE = 1
 MX_COLLISION_MODE_ROBOT_IN_WORKSPACE = 2
 MX_COLLISION_MODE_FULL_COLLISION_DETECTION = 3
 MX_STOP_STATE_RESET = 0  # PStop2 or EStop condition is not active
 MX_STOP_STATE_ACTIVE = 1  # PStop2 or EStop condition is active (robot is stopped/deactivated)
 MX_STOP_STATE_RESETTABLE = 2  # PStop2 or EStop condition is cleared but awaiting ack (ResetPStop)
@@ -90,27 +98,32 @@
 MX_MOTION_CMD_TYPE_SETCONF = 15  # Set the desired inverse kinematic config for MovePose.
 MX_MOTION_CMD_TYPE_SETAUTOCONF = 16  # Enable or disable automatic configuration for inverse kinematic
 MX_MOTION_CMD_TYPE_SETCHECKPOINT = 17  # Inserts a "set checkpoint" command between two moves, so robot status
 MX_MOTION_CMD_TYPE_GRIPPEROPENCLOSE = 18  # Open or close the gripper
 MX_MOTION_CMD_TYPE_GRIPPERVEL = 19  # Limit the velocity of the gripper fingers in percent
 MX_MOTION_CMD_TYPE_GRIPPERFORCE = 20  # Limit the grip force of the gripper in percent
 MX_MOTION_CMD_TYPE_MOVEJOINTSVEL = 21  # Set current mode to "join velocity mode"
-MX_MOTION_CMD_TYPE_MOVELINVELWRF = 22  # Set current mode to "cartesian WRF velocity mode"
-MX_MOTION_CMD_TYPE_MOVELINVELTRF = 23  # Set current mode to "cartesian TRF velocity mode"
+MX_MOTION_CMD_TYPE_MOVELINVELWRF = 22  # Set current mode to "Cartesian WRF velocity mode"
+MX_MOTION_CMD_TYPE_MOVELINVELTRF = 23  # Set current mode to "Cartesian TRF velocity mode"
 MX_MOTION_CMD_TYPE_SETVELTIMEOUT = 24  # Timeout for current velocity mode
 MX_MOTION_CMD_TYPE_SETCONFTURN = 25  # Set the last joint turn conf (i.e. which turn should be used
 MX_MOTION_CMD_TYPE_SETAUTOCONFTURN = 26  # Enable or disable automatic last joint turn selection
 MX_MOTION_CMD_TYPE_SETTORQUELIMITS = 27  # Set torque limits for current motion
 MX_MOTION_CMD_TYPE_SETTORQUELIMITSCFG = 28  # Set torque limits configuration for current motion
 MX_MOTION_CMD_TYPE_MOVEJOINTSREL = 29  # Move each joint relative to current joint position
 MX_MOTION_CMD_TYPE_SETVALVESTATE = 30  # Set valve box valves states
 MX_MOTION_CMD_TYPE_GRIPPERRANGE = 31  # Set the Close and Open position that will be used when calling
 MX_MOTION_CMD_TYPE_GRIPPERPOS = 32  # Move gripper to a specific position, in mm from the most closed
+MX_MOTION_CMD_TYPE_SETJOINTVELLIMIT = 33  # Max allowed joint vel (max for SetJointVel and linear moves).
+MX_MOTION_CMD_TYPE_SETOUTPUTSTATE = 34  # Set digital output states (through motion queue)
+MX_MOTION_CMD_TYPE_SETOUTPUTSTATE_IMMEDIATE = 35  # Set digital output states (immediate, bypass motion queue)
+MX_MOTION_CMD_TYPE_SETIOSIM = 36  # Set (or clear) IO simulation mode
 MX_MOTION_CMD_TYPE_START_OFFLINE_PROGRAM = 100  # Start an offline program with specified id
 MX_MOTION_CMD_TYPE_SETDBG = 1000  # Enable debug options on the robot. For Mecademic use only.
+MX_MOTION_CMD_TYPE_MG2BUSDBG = 1001  # Send custom command on Mg2 bus. For Mecademic use only.
 MX_EIP_DYNAMIC_AUTO = 0
 MX_EIP_DYNAMIC_CFG_FW_VERSION = 1
 MX_EIP_DYNAMIC_CFG_PRODUCT_TYPE = 2
 MX_EIP_DYNAMIC_CFG_ROBOT_SERIAL = 3
 MX_EIP_DYNAMIC_CFG_JOINT_OFFSET = 4
 MX_EIP_DYNAMIC_CFG_ROBOT_DH_MODEL_1 = 5
 MX_EIP_DYNAMIC_CFG_ROBOT_DH_MODEL_2 = 6
@@ -123,14 +136,17 @@
 MX_EIP_DYNAMIC_CFG_MODEL_JOINT_LIMITS_4_5_6 = 13
 MX_EIP_DYNAMIC_CFG_JOINT_LIMITS_1_2_3 = 14
 MX_EIP_DYNAMIC_CFG_JOINT_LIMITS_4_5_6 = 15
 MX_EIP_DYNAMIC_CFG_EXT_TOOL_FW_VERSION = 16
 MX_EIP_DYNAMIC_CFG_WORKSPACE_LIMITS_CFG = 17
 MX_EIP_DYNAMIC_CFG_WORKSPACE_LIMITS = 18
 MX_EIP_DYNAMIC_CFG_TOOL_SPHERE = 19
+MX_EIP_DYNAMIC_CFG_CALIBRATION = 30
+MX_EIP_DYNAMIC_CFG_BRF_OFFSET = 31
+MX_EIP_DYNAMIC_CFG_FRF_OFFSET = 35
 MX_EIP_DYNAMIC_MQ_CONF = 20
 MX_EIP_DYNAMIC_MQ_PARAMS = 21
 MX_EIP_DYNAMIC_MQ_VEL_ACCEL = 22
 MX_EIP_DYNAMIC_MQ_GRIPPER_CFG = 23
 MX_EIP_DYNAMIC_MQ_TORQUE_LIMITS_CFG = 24
 MX_EIP_DYNAMIC_MQ_TORQUE_LIMITS = 25
 MX_EIP_DYNAMIC_RT_TARGET_JOINT_POS = 30  # Present in basic PDOs already
@@ -146,14 +162,16 @@
 MX_EIP_DYNAMIC_RT_CART_VEL = 44
 MX_EIP_DYNAMIC_RT_CONF = 45
 MX_EIP_DYNAMIC_RT_ACCELEROMETER_5 = 46
 MX_EIP_DYNAMIC_RT_WRF = 50  # Present in basic PDOs already
 MX_EIP_DYNAMIC_RT_TRF = 51  # Present in basic PDOs already
 MX_EIP_DYNAMIC_RT_EXTTOOL_STATUS = 52
 MX_EIP_DYNAMIC_RT_GRIPPER_VALVE_STATE = 53
+MX_EIP_DYNAMIC_RT_PSU_IO_STATE = 71  # Digital outputs and inputs from the Mcs500 PSU
+MX_EIP_DYNAMIC_RT_IO_MODULE_IO_STATE = 72  # Digital outputs and inputs from the Mcs500 IO module
 MX_EIP_DYNAMIC_INTERNAL_SET_DBG = 0x08000000
 MX_EIP_DYNAMIC_FORCE_32_BITS = 0xFFFFFFFF
 MX_EIP_DYNAMIC_INTERNAL_MASK = 0x0FFFFFFF
 MX_EIP_DYNAMIC_INTERNAL_SHIFT = 28  # Bit shift that corresponds to MX_EIP_DYNAMIC_INTERNAL_MASK
 MX_ST_EXCESSIVE_TRQ = 3028  # replaced by MX_ST_TORQUE_LIMIT_STATUS
 MX_ST_NONE = 0
 MX_ST_BUFFER_FULL = 1000  # Maximum number of queued commands reached. Try sending fewer at a time.
@@ -181,30 +199,31 @@
 MX_ST_ILLEGAL_WHILE_SAVING = 1031  # This command is illegal while saving an offline program.
 MX_ST_HOMING_JOINTS_OUT_OF_RANGE = 1032  # DEPRECATED. Was used only on release 8.X
 MX_ST_START_CONF_MISMATCH = 1033  # Requested move blocked because start pos is not in requested conf
 MX_ST_NO_GRIPPER = 1038  # No gripper is connected, command can't be executed.
 MX_ST_CMD_FAILED = 1040  # Command failed (generic response for various simple commands)
 MX_ST_NO_VBOX = 1041  # No pneumatic module is connected.
 MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED = 1042  # Switching external tool type is only possible when the robot
+MX_ST_INVALID_BANK_ID = 1043  # The specified IO bank is not present on this robot.
 MX_ST_OFFLINE_PROGRAM_LIST_ERR = 1500  # Failed "ListPrograms" API command
 MX_ST_OFFLINE_PROGRAM_LOAD_ERR = 1501  # Failed "LoadProgram" API command
 MX_ST_OFFLINE_PROGRAM_SAVE_ERR = 1502  # Failed "SaveProgram" API command
 MX_ST_OFFLINE_PROGRAM_DELETE_ERR = 1503  # Failed "DeleteProgram" API command
 MX_ST_ACTIVATED = 2000  # Motors were successfully activated
 MX_ST_HOME_DONE = 2002  # Homing done.
 MX_ST_DEACTIVATED = 2004  # Motors deactivated.
 MX_ST_ERROR_RESET = 2005  # The error was reset. Commands can now be sent again.
 MX_ST_NO_ERROR_RESET = 2006  # There was no error to reset.
 MX_ST_GET_STATUS_ROBOT = 2007  # This event reports the status of the robot.
 MX_ST_BRAKES_OFF = 2008  # All brakes are now released.
 MX_ST_MASTER_DONE = 2009  # Mastering now done.
 MX_ST_BRAKES_ON = 2010  # All brakes are now set.
-MX_ST_GET_MOTION_STATUS = 2011  # This event reports the motion status of the robot (JSON format).
-MX_ST_GET_WRF = 2013  # Response to GetTrf
-MX_ST_GET_TRF = 2014  # Response to GetWrf
+MX_ST_GET_WRF = 2013  # Response to GetWrf
+MX_ST_GET_TRF = 2014  # Response to GetTrf
+MX_ST_GET_TIME_SCALING = 2015  # Response to GetTimeScaling
 MX_ST_GET_JOINTS = 2026  # "GetJoints" response (current joint angles in degrees).
 MX_ST_GET_POSE = 2027  # "GetPose" response (current position in mm, Euler angles in degrees).
 MX_ST_GET_AUTO_CONF = 2028
 MX_ST_GET_CONF = 2029  # "GetConf" response (current shoulder, elbow, wrist conf)
 MX_ST_GET_AUTO_CONF_TURN = 2031
 MX_ST_GET_CONF_TURN = 2036  # "GetConfTurn" response
 MX_ST_PAUSE_MOTION = 2042  # Motion paused.
@@ -216,27 +235,30 @@
 MX_ST_RECOVERY_MODE_ON = 2049  # Robot is now in recovery mode.
 MX_ST_RECOVERY_MODE_OFF = 2050  # Robot is no more in recovery mode.
 MX_ST_RECOVERY_VEL_CAP = 2051  # Recovery mode has capped velocity.
 MX_ST_EOM_ON = 2052  # End of movement events are enabled.
 MX_ST_EOM_OFF = 2053  # End of movement events are disabled.
 MX_ST_EOB_ON = 2054  # End of block events are enabled.
 MX_ST_EOB_OFF = 2055  # End of block events are enabled.
+MX_ST_IO_SIM = 2056  # Response to GetIoSim.
 MX_ST_START_SAVING = 2060  # Offline program saving now started.
 MX_ST_N_CMD_SAVED = 2061  # Offline program saving done (reports number of saved commands)
 MX_ST_OFFLINE_START = 2063  # Offline program started to run.
 MX_ST_OFFLINE_LOOP_ON = 2064  # Offline program loop is enabled.
 MX_ST_OFFLINE_LOOP_OFF = 2065  # Offline program loop is disabled.
 MX_ST_GET_STATUS_GRIPPER = 2079  # "GetStatusGripper" response (see pdf doc for response fields meaning).
 MX_ST_GET_CMD_PENDING_COUNT = 2080  # Number of pending commands in the queue.
 MX_ST_GET_FW_VERSION = 2081  # The firmware version running on the robot.
 MX_ST_GET_FW_VERSION_FULL = 2082  # More detailed info about the firmware version running on the robot.
 MX_ST_GET_ROBOT_SERIAL = 2083  # Current robot serial number (response to GetRobotSerial and SetRobotSerial)
 MX_ST_GET_PRODUCT_TYPE = 2084  # Current product type (Meca500...)
 MX_ST_CMD_SUCCESSFUL = 2085  # Command successful (generic response for various simple commands)
 MX_ST_GET_EXT_TOOL_FW_VERSION = 2086  # "GetExtToolFwVersion" response with current gripper firmware version.
+MX_ST_GET_EXT_PORT_COMM_ERRORS = 2087  # "GetExtPortCommErrors" response.
+MX_ST_GET_EXT_TOOL_COMM_ERRORS = 2088  # "GetExtToolCommErrors" response.
 MX_ST_GET_NETWORK_CONFIG = 2089  # "GetNetworkConfig" response (JSON format)
 MX_ST_GET_JOINT_LIMITS = 2090  # "GetJointLimits" response (joint nb, min, max)
 MX_ST_SET_JOINT_LIMITS = 2092  # "SetJointLimits" success response
 MX_ST_SET_JOINT_LIMITS_CFG = 2093  # "SetJointLimitsCfg" success response (joint limits enabled)
 MX_ST_GET_JOINT_LIMITS_CFG = 2094  # "GetJointLimitsCfg" response
 MX_ST_GET_ROBOT_NAME = 2095  # "GetRobotName" response
 MX_ST_SET_CTRL_PORT_MONIT = 2096  # "SetCtrlPortMonitoring" response
@@ -250,14 +272,17 @@
 MX_ST_GET_JOINT_OFFSET = 2112  # "GetJointOffset" response
 MX_ST_GET_MODEL_JOINT_LIMITS = 2113  # "GetModelJointLimits" response
 MX_ST_GET_TEST_BENCH_MODE = 2114  # "GetTestBenchMode" response
 MX_ST_GET_MOTION_OPTIONS = 2115  # "GetMotionOptions" response
 MX_ST_GET_MONITORING_INTERVAL = 2116  # "GetMonitoringInterval" response
 MX_ST_GET_REAL_TIME_MONITORING = 2117  # "GetRealTimeMonitoring" response
 MX_ST_GET_NETWORK_OPTIONS = 2119  # "GetNetworkOptions" response
+MX_ST_GET_BRF_OFFSET = 2120  # "GetBrfOffset" response
+MX_ST_GET_FRF_OFFSET = 2121  # "GetFrfOffset" response
+MX_ST_GET_ROBOT_CALIBRATED = 2122  # "GetRobotCalibrated" response
 MX_ST_GET_RTC = 2140  # "GetRtc" response
 MX_ST_GET_BLENDING = 2150  # "GetBlending" response
 MX_ST_GET_VEL_TIMEOUT = 2151  # "GetVelTimeout" response
 MX_ST_GET_JOINT_VEL = 2152  # "GetJointVel" response
 MX_ST_GET_JOINT_ACC = 2153  # "GetJointAcc" response
 MX_ST_GET_CART_LIN_VEL = 2154  # "GetCartLinVel" response
 MX_ST_GET_CART_ANG_VEL = 2155  # "GetCartAngVel" response
@@ -270,14 +295,17 @@
 MX_ST_GET_GRIPPER_RANGE = 2162  # "GetGipperRange" response
 MX_ST_GET_WORKSPACE_LIMITS_CFG = 2163  # "GetWorkspaceLimitsCfg" response
 MX_ST_SET_WORKSPACE_LIMITS_CFG = 2164  # "SetWorkspaceLimitsCfg" response
 MX_ST_GET_WORKSPACE_LIMITS = 2165  # "GetWorkspaceLimits" response
 MX_ST_SET_WORKSPACE_LIMITS = 2166  # "SetWorkspaceLimits" response
 MX_ST_GET_TOOL_SPHERE = 2167  # "GetToolSphere" response
 MX_ST_SET_TOOL_SPHERE = 2168  # "SetToolSphere" response
+MX_ST_GET_JOINT_VEL_LIMIT = 2169  # "GetJointVelLimit" response
+MX_ST_SET_CALIBRATION_CFG = 2170  # "SetCalibrationCfg" response
+MX_ST_GET_CALIBRATION_CFG = 2171  # "GetCalibrationCfg" response
 MX_ST_RT_TARGET_JOINT_POS = 2200  # Timestamp + joint positions in degrees
 MX_ST_RT_TARGET_CART_POS = 2201  # Timestamp + Cartesian position (in mm, Euler angles in degrees).
 MX_ST_RT_TARGET_JOINT_VEL = 2202  # Timestamp + joint velocity in degrees per second
 MX_ST_RT_TARGET_JOINT_TORQ = 2203  # Timestamp + joint torque ratio in percent
 MX_ST_RT_TARGET_CART_VEL = 2204  # Timestamp + Cartesian velocity (in mm, Euler angles in degrees per sec).
 MX_ST_RT_TARGET_CONF = 2208  # Timestamp + conf that corresponds to MX_ST_RT_TARGET_JOINT_POS
 MX_ST_RT_TARGET_CONF_TURN = 2209  # Timestamp + last joint turn that corresponds to MX_ST_RT_TARGET_JOINT_POS
@@ -296,18 +324,25 @@
 MX_ST_RT_CYCLE_END = 2230  # Timestamp of the real-time cycle which has just ended.
 MX_ST_RT_EXTTOOL_STATUS = 2300  # Timestamp + external tool status
 MX_ST_RT_VALVE_STATE = 2310  # Timestamp + valve state
 MX_ST_RT_GRIPPER_STATE = 2320  # Timestamp + gripper state
 MX_ST_RT_GRIPPER_FORCE = 2321  # Timestamp + gripper force in percent
 MX_ST_RT_GRIPPER_POS = 2322  # Timestamp + gripper position in percent
 MX_ST_RT_GRIPPER_VEL = 2323  # Timestamp + gripper speed in percent
+MX_ST_RT_IO_STATUS = 2330  # Timestamp + IO module status
+MX_ST_RT_OUTPUT_STATE = 2340  # Timestamp + bankId + output states
+MX_ST_RT_INPUT_STATE = 2341  # Timestamp + bankId + input states
+MX_ST_RT_DEBUG_MG2_SAFE_MCU = 2400  # Safe MCU debug status.
+MX_ST_RT_DEBUG_MG2_DRIVES = 2401  # Drives debug status.
+MX_ST_RT_DEBUG_MG2_PSU = 2402  # PSU debug status.
 MX_ST_OFFLINE_PROGRAM_LIST = 2500  # Response to "ListPrograms" API command
 MX_ST_OFFLINE_PROGRAM_LOAD = 2501  # Response to "LoadProgram" API command
 MX_ST_OFFLINE_PROGRAM_SAVE = 2502  # Response to "SaveProgram" API command
 MX_ST_OFFLINE_PROGRAM_DELETE = 2503  # Response to "DeleteProgram" API command
+MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE = 2504  # Response to "StartDemoProgram" API command.
 MX_ST_CONNECTED = 3000  # Confirms connection to robot.
 MX_ST_USER_ALREADY = 3001  # Another user is already connected to the robot (current connection refused).
 MX_ST_UPGRADE_IN_PROGRESS = 3002  # A firmware upgrade is in progress (current connection refused).
 MX_ST_CMD_TOO_LONG = 3003  # Command string is too long (or missing NUL character).
 MX_ST_EOM = 3004  # The robot has stopped moving.
 MX_ST_ERROR_MOTION = 3005  # Motion error (probably collision or overload). This error can be reset.
 MX_ST_ERROR_DRIVE_COMM = 3006  # Comm error with drives. This error cannot be reset.
@@ -315,14 +350,16 @@
 MX_ST_EOB = 3012  # No more motion command are in queue and robot is no more moving.
 MX_ST_END_OFFLINE = 3013  # The offline program has finished.
 MX_ST_CANT_SAVE_OFFLINE = 3014  # There was a problem saving the offline program.
 MX_ST_IGNORING_CMD = 3016  # Non-motion command ignored during execution of an offline program.
 MX_ST_NO_OFFLINE_SAVED = 3017  # There is no program in memory.
 MX_ST_OFFLINE_LOOP = 3018  # The offline program is being restarted (looped).
 MX_ST_OFFLINE_INVALID = 3020  # The offline program is invalid and can't be played
+MX_ST_DEV_MODE = 3021  # The robot is running in developer mode (non official binary)
+MX_ST_PSU_DONGLE_STATUS = 3022  # Power-supply USB debug dongle status (sent only when detected)
 MX_ST_ERROR_GRIPPER = 3025  # The gripper reported an error.
 MX_ST_MAINTENANCE_CHECK = 3026  # A hardware problem was detected. Contact Mecademic support.
 MX_ST_INTERNAL_ERROR = 3027  # Unknown internal error occurred.
 MX_ST_TORQUE_LIMIT_STATUS = 3028  # "GetTorqueLimitsStatus" response and torque limit status update.
 MX_ST_TORQUE_LIMIT_ERROR = 3029  # Excessive torque error occurred.
 MX_ST_CHECKPOINT_REACHED = 3030  # A previously set checkpoint (with given id) was just reached.
 MX_ST_TEXT_API_ERROR = 3031  # A previously received text API command was incorrect.
@@ -333,74 +370,110 @@
 MX_ST_TCP_DUMP_DONE = 3036  # TCPDump has ended
 MX_ST_ERROR_VBOX = 3037  # The pneumatic module reported an error
 MX_ST_FW_UPDATE_PROGRESS = 3038  # Firmware update progress (JSON format)
 MX_ST_EXT_TOOL_NEED_UPDATE = 3039  # The external tool need a firmware update.
 MX_ST_COLLISION_STATUS = 3040  # Collision status update
 MX_ST_COLLISION_ERROR = 3041  # Collision error occurred.
 MX_ST_FW_NEED_REINSTALL = 3042  # Firmware must be reinstalled again.
+MX_ST_EXT_TOOL_COMM_ERR = 3043  # Excessive communication errors with external tool.
+MX_ST_EXT_PORT_COMM_ERR = 3044  # Abnormal communication error with external port.
+MX_ST_COLLISION_STOP = 3045  # Robot has decelerated due to imminent collision.
+MX_ST_PSU_ERROR = 3046  # Robot power supply has non-resettable error.
 MX_ST_ESTOP = 3070  # The EStop condition raised
 MX_ST_INVALID = 0xFFFFFFFF
 MX_ST_EXTTOOL_SIM_OFF = 2048
 MX_ROBOT_STATE_UNKNOWN = 0
 MX_ROBOT_STATE_INIT = 1
 MX_ROBOT_STATE_POWERED = 2
 MX_ROBOT_STATE_ACTIVATING = 3
 MX_ROBOT_STATE_ACTIVATED = 4
 MX_ROBOT_STATE_HOMING = 5
 MX_ROBOT_STATE_MASTERING = 6
 MX_ROBOT_STATE_RUN = 7
 MX_ROBOT_STATE_DEACTIVATING = 9
 MX_JSON_KEY_CODE = "code"  # Key for the status/command code in JSON message
 MX_JSON_KEY_DATA = "data"  # Key for the status/command data in JSON message
+MX_JSON_KEY_TIMESTAMP_US = "timestampUs"  # Robot timestamp in microseconds
 MX_JSON_KEY_META_DATA = "metaData"  # Key for the status/command meta data in JSON message
 MX_JSON_KEY_MSG_TYPE = "msgType"  # Key for message type inside metaData. Values from MxRobotMsgType
 MX_JSON_KEY_FW_UPDATE_PROGRESS_UPDATING = "updating"  # bool: Firmware update has started
 MX_JSON_KEY_FW_UPDATE_PROGRESS_VERSION = "version"  # string: Firmware version we're updating to
 MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR = "error"  # bool: Firmware update has failed
 MX_JSON_KEY_FW_UPDATE_PROGRESS_ERROR_MSG = "errorMsg"  # string: User message if failed
 MX_JSON_KEY_FW_UPDATE_PROGRESS_PCT = "progressPct"  # float: Update percentage (0 to 100)
 MX_JSON_KEY_FW_UPDATE_PROGRESS_STEP = "step"  # string: Current update step (human readable)
+MX_JSON_KEY_FW_UPDATE_PROGRESS_REBOOT_DONE = "rebootDone"  # bool: Tells if robot reboot was done
 MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG = "log"  # array of {time, msg}: Update history
 MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG_TIME = "time"  # int: Absolute time of this log (seconds since Epoch)
+MX_JSON_KEY_FW_UPDATE_PROGRESS_LOG_FAILED = "failed"  # bool: Indicate if this step has failed
+MX_JSON_KEY_ROBOT_STATUS = "robotStatus"  # Parent key for following child keys:
 MX_JSON_KEY_STATUS_ROBOT_STATE = "state"  # integer: Value (as integer) from enum MxRobotState
 MX_JSON_KEY_STATUS_ROBOT_SIM = "simMode"  # bool: Sim mode
 MX_JSON_KEY_STATUS_ROBOT_RECOVERY = "recovery"  # bool: Recovery enabled
 MX_JSON_KEY_STATUS_ROBOT_BRAKES = "brakesEngaged"  # bool: Brakes engaged
 MX_JSON_KEY_STATUS_ROBOT_ERR = "errorCode"  # integer: Error code (0 if no error)
 MX_JSON_KEY_STATUS_ROBOT_ERR_MSG = "errorMsg"  # string: User message related to error code
 MX_JSON_KEY_STATUS_ROBOT_ESTOP = "eStop"  # bool: ESTOP condition is active
+MX_JSON_KEY_STATUS_ROBOT_ESTOP_RESETTABLE = "eStopResettable"  # bool: ESTOP cleared but awaiting Reset
+MX_JSON_KEY_MOTION_STATUS = "motionStatus"  # Parent key for following child keys:
 MX_JSON_KEY_MOTION_ROBOT_CHECKPOINT = "checkpoint"  # integer: Most recently reached checkpoint id
 MX_JSON_KEY_MOTION_ROBOT_OFFLINE_PRGRM = "offlineProgramId"  # integer: Running offline-program Id
 MX_JSON_KEY_MOTION_ROBOT_HOLD = "paused"  # bool: Hold motion
 MX_JSON_KEY_MOTION_ROBOT_EOM = "eom"  # bool: End of motion
 MX_JSON_KEY_MOTION_ROBOT_EOB = "eob"  # bool: End of block
 MX_JSON_KEY_MOTION_ROBOT_PSTOP2 = "pStop2"  # bool: PSTOP2 condition is active
 MX_JSON_KEY_MOTION_ROBOT_PSTOP2_RESETTABLE = "pStop2Resettable"  # bool: PSTOP2 condition can be reset
 MX_JSON_KEY_MOTION_ROBOT_EXCESSIVE_TORQ = "excessiveTorque"  # bool: Excessive torque ratio
+MX_JSON_KEY_EXTTOOL_STATUS_SIM_TYPE = "simType"  # Values from enum MxExtToolType
+MX_JSON_KEY_EXTTOOL_STATUS_PHYSICAL_TYPE = "physicalType"  # Values from enum MxExtToolType
+MX_JSON_KEY_EXTTOOL_STATUS_HOMED = "homed"  # bool: Tool homing was done
+MX_JSON_KEY_EXTTOOL_STATUS_ERROR = "error"  # bool: True when in error state
+MX_JSON_KEY_EXTTOOL_STATUS_OVERHEAT = "overheat"  # bool: True when in overheat state
+MX_JSON_KEY_EXTTOOL_STATUS_COMM_ERR = "commErrWarning"  # bool: True when some comm errors (not yet in err)
+MX_JSON_KEY_IO_STATUS_BANK_ID = "bankId"  # integer: BankId we're returning status for
+MX_JSON_KEY_IO_STATUS_BANK_NAME = "bankName"  # integer: Bank name we're returning status for
+MX_JSON_KEY_IO_STATUS_PRESENT = "present"  # bool: Indicate if this IO module is present
+MX_JSON_KEY_IO_STATUS_NB_INPUTS = "nbDigitalInputs"  # integer: Number of digital inputs present
+MX_JSON_KEY_IO_STATUS_NB_OUTPUTS = "nbDigitalOutputs"  # integer: Number of digital outputs present
+MX_JSON_KEY_IO_STATUS_SIM_MODE = "simMode"  # bool: Tells if currently in simulation mode
+MX_JSON_KEY_IO_STATUS_ERROR = "error"  # integer: True when in error state
 MX_JSON_KEY_NETWORK_CONFIG_ROBOT_NAME = "name"  # string: The robot name (hostname on the network)
 MX_JSON_KEY_NETWORK_CONFIG_DHCP = "dhcp"  # bool: Indicate if IP is obtained using DHCP
 MX_JSON_KEY_NETWORK_CONFIG_IP = "ip"  # string: The IPv4 address of the robot
 MX_JSON_KEY_NETWORK_CONFIG_MASK = "mask"  # string: The netmask
 MX_JSON_KEY_NETWORK_CONFIG_GATEWAY = "gateway"  # string: The gateway address
 MX_JSON_KEY_NETWORK_CONFIG_MAC = "mac"  # string: The robot's MAC address
+MX_JSON_KEY_PSU_DONGLE_DETECTED = "detected"  # bool: True if dongle was detected and updated successfully
 MX_FW_UPDATE_UPLOAD_URL = "/fw-update"
 MX_GET_LOGS_URL = "/get-logs"
 MX_FW_UPDATE_STATUS_EXTRACTING = "Extracting files from firmware package..."
 MX_FW_UPDATE_STATUS_CLOSING_CONNECTIONS = "Closing connections and stacks..."
 MX_FW_UPDATE_STATUS_LAUNCH_SCRIPT = "Launching firmware update script..."
 MX_FW_UPDATE_STATUS_ANALYZING = "Analyzing files..."
 MX_FW_UPDATE_STATUS_DRIVE = "Updating drive #"  # Plus drive number
 MX_FW_UPDATE_STATUS_EXT_PORT = "Updating external port"
 MX_FW_UPDATE_STATUS_EXT_TOOL = "Updating external tool"
 MX_FW_UPDATE_STATUS_NO_FW_IMAGE = "(No firmware image in this package)"
 MX_FW_UPDATE_STATUS_FW_IMAGE = "Updating firmware image"
 MX_FW_UPDATE_STATUS_CLEANUP = "Cleanup after update"
 MX_FW_UPDATE_STATUS_REBOOTING = "Awaiting for robot to reboot"
+MX_FW_UPDATE_STATUS_BOOT_BIN = "Updating boot binary"
+MX_FW_UPDATE_STATUS_SAFE_BOOT = "Updating safe boot"
+MX_FW_UPDATE_STATUS_SAFE_MCU_MASTER = "Updating master SafeMCU"
+MX_FW_UPDATE_STATUS_SAFE_MCU_SLAVE = "Updating slave SafeMCU"
+MX_FW_UPDATE_STATUS_PSU_MASTER = "Updating master power supply"
+MX_FW_UPDATE_STATUS_PSU_SLAVE = "Updating slave power supply"
+MX_FW_UPDATE_STATUS_IO_MODULE = "Updating IO module"
+MX_FW_UPDATE_AVG_DURATION_SEC_MECA500 = 350
+MX_FW_UPDATE_REBOOT_DURATION_SEC_MECA500 = 60
+MX_FW_UPDATE_AVG_DURATION_SEC_MCS500 = 250
+MX_FW_UPDATE_REBOOT_DURATION_SEC_MCS500 = 120  # Note: rootfs update done during this reboot
 MX_CMD_TAG_ROBOT_CONTROL = "RobotControl"
 MX_CMD_TAG_EXT_TOOL = "ExternalTool"
+MX_CMD_TAG_IO_BANK = "IoBank"
 MX_CMD_TAG_MOTION = "Motion"
 MX_CMD_TAG_UTILITIES = "Utilities"
 MX_CMD_TAG_SYS_CFG = "SystemConfig"
 MX_CMD_TAG_PGM = "Program"
 MX_CMD_TAG_GET = "Get"
 MX_CMD_TAG_PERMANENT = "Permanent"
 MX_CMD_TAG_TEMPORARY = "Temporary"
@@ -501,14 +574,16 @@
     RobotStatusCodeInfo(MX_ST_NO_GRIPPER, "MX_ST_NO_GRIPPER", is_error=True, is_resettable=True),
     MX_ST_CMD_FAILED:
     RobotStatusCodeInfo(MX_ST_CMD_FAILED, "MX_ST_CMD_FAILED", is_error=True, is_resettable=True),
     MX_ST_NO_VBOX:
     RobotStatusCodeInfo(MX_ST_NO_VBOX, "MX_ST_NO_VBOX", is_error=True, is_resettable=True),
     MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED:
     RobotStatusCodeInfo(MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED, "MX_ST_EXT_TOOL_SIM_MUST_DEACTIVATED", is_error=True, is_resettable=True),
+    MX_ST_INVALID_BANK_ID:
+    RobotStatusCodeInfo(MX_ST_INVALID_BANK_ID, "MX_ST_INVALID_BANK_ID", is_error=True, is_resettable=True),
     MX_ST_OFFLINE_PROGRAM_LIST_ERR:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_LIST_ERR, "MX_ST_OFFLINE_PROGRAM_LIST_ERR", is_error=True, is_resettable=True),
     MX_ST_OFFLINE_PROGRAM_LOAD_ERR:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_LOAD_ERR, "MX_ST_OFFLINE_PROGRAM_LOAD_ERR", is_error=True, is_resettable=True),
     MX_ST_OFFLINE_PROGRAM_SAVE_ERR:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_SAVE_ERR, "MX_ST_OFFLINE_PROGRAM_SAVE_ERR", is_error=True, is_resettable=True),
     MX_ST_OFFLINE_PROGRAM_DELETE_ERR:
@@ -521,16 +596,16 @@
     RobotStatusCodeInfo(MX_ST_DEACTIVATED, "MX_ST_DEACTIVATED", is_error=False, is_resettable=False),
     MX_ST_ERROR_RESET:
     RobotStatusCodeInfo(MX_ST_ERROR_RESET, "MX_ST_ERROR_RESET", is_error=False, is_resettable=False),
     MX_ST_NO_ERROR_RESET:
     RobotStatusCodeInfo(MX_ST_NO_ERROR_RESET, "MX_ST_NO_ERROR_RESET", is_error=False, is_resettable=False),
     MX_ST_GET_STATUS_ROBOT:
     RobotStatusCodeInfo(MX_ST_GET_STATUS_ROBOT, "MX_ST_GET_STATUS_ROBOT", is_error=False, is_resettable=False),
-    MX_ST_GET_MOTION_STATUS:
-    RobotStatusCodeInfo(MX_ST_GET_MOTION_STATUS, "MX_ST_GET_MOTION_STATUS", is_error=False, is_resettable=False),
+    MX_ST_GET_TIME_SCALING:
+    RobotStatusCodeInfo(MX_ST_GET_TIME_SCALING, "MX_ST_GET_TIME_SCALING", is_error=False, is_resettable=False),
     MX_ST_BRAKES_OFF:
     RobotStatusCodeInfo(MX_ST_BRAKES_OFF, "MX_ST_BRAKES_OFF", is_error=False, is_resettable=False),
     MX_ST_MASTER_DONE:
     RobotStatusCodeInfo(MX_ST_MASTER_DONE, "MX_ST_MASTER_DONE", is_error=False, is_resettable=False),
     MX_ST_BRAKES_ON:
     RobotStatusCodeInfo(MX_ST_BRAKES_ON, "MX_ST_BRAKES_ON", is_error=False, is_resettable=False),
     MX_ST_GET_WRF:
@@ -557,14 +632,16 @@
     RobotStatusCodeInfo(MX_ST_CLEAR_MOTION, "MX_ST_CLEAR_MOTION", is_error=False, is_resettable=False),
     MX_ST_SIM_ON:
     RobotStatusCodeInfo(MX_ST_SIM_ON, "MX_ST_SIM_ON", is_error=False, is_resettable=False),
     MX_ST_SIM_OFF:
     RobotStatusCodeInfo(MX_ST_SIM_OFF, "MX_ST_SIM_OFF", is_error=False, is_resettable=False),
     MX_ST_EXTTOOL_SIM:
     RobotStatusCodeInfo(MX_ST_EXTTOOL_SIM, "MX_ST_EXTTOOL_SIM", is_error=False, is_resettable=False),
+    MX_ST_IO_SIM:
+    RobotStatusCodeInfo(MX_ST_IO_SIM, "MX_ST_IO_SIM", is_error=False, is_resettable=False),
     MX_ST_EOM_ON:
     RobotStatusCodeInfo(MX_ST_EOM_ON, "MX_ST_EOM_ON", is_error=False, is_resettable=False),
     MX_ST_EOM_OFF:
     RobotStatusCodeInfo(MX_ST_EOM_OFF, "MX_ST_EOM_OFF", is_error=False, is_resettable=False),
     MX_ST_EOB_ON:
     RobotStatusCodeInfo(MX_ST_EOB_ON, "MX_ST_EOB_ON", is_error=False, is_resettable=False),
     MX_ST_EOB_OFF:
@@ -585,14 +662,18 @@
     RobotStatusCodeInfo(MX_ST_GET_CMD_PENDING_COUNT, "MX_ST_GET_CMD_PENDING_COUNT", is_error=False, is_resettable=False),
     MX_ST_GET_FW_VERSION:
     RobotStatusCodeInfo(MX_ST_GET_FW_VERSION, "MX_ST_GET_FW_VERSION", is_error=False, is_resettable=False),
     MX_ST_GET_FW_VERSION_FULL:
     RobotStatusCodeInfo(MX_ST_GET_FW_VERSION_FULL, "MX_ST_GET_FW_VERSION_FULL", is_error=False, is_resettable=False),
     MX_ST_GET_EXT_TOOL_FW_VERSION:
     RobotStatusCodeInfo(MX_ST_GET_EXT_TOOL_FW_VERSION, "MX_ST_GET_EXT_TOOL_FW_VERSION", is_error=False, is_resettable=False),
+    MX_ST_GET_EXT_PORT_COMM_ERRORS:
+    RobotStatusCodeInfo(MX_ST_GET_EXT_PORT_COMM_ERRORS, "MX_ST_GET_EXT_PORT_COMM_ERRORS", is_error=False, is_resettable=False),
+    MX_ST_GET_EXT_TOOL_COMM_ERRORS:
+    RobotStatusCodeInfo(MX_ST_GET_EXT_TOOL_COMM_ERRORS, "MX_ST_GET_EXT_TOOL_COMM_ERRORS", is_error=False, is_resettable=False),
     MX_ST_GET_ROBOT_SERIAL:
     RobotStatusCodeInfo(MX_ST_GET_ROBOT_SERIAL, "MX_ST_GET_ROBOT_SERIAL", is_error=False, is_resettable=False),
     MX_ST_GET_PRODUCT_TYPE:
     RobotStatusCodeInfo(MX_ST_GET_PRODUCT_TYPE, "MX_ST_GET_PRODUCT_TYPE", is_error=False, is_resettable=False),
     MX_ST_CMD_SUCCESSFUL:
     RobotStatusCodeInfo(MX_ST_CMD_SUCCESSFUL, "MX_ST_CMD_SUCCESSFUL", is_error=False, is_resettable=False),
     MX_ST_SET_CTRL_PORT_MONIT:
@@ -613,14 +694,16 @@
     RobotStatusCodeInfo(MX_ST_SET_JOINT_LIMITS_CFG, "MX_ST_SET_JOINT_LIMITS_CFG", is_error=False, is_resettable=False),
     MX_ST_GET_WORKSPACE_LIMITS:
     RobotStatusCodeInfo(MX_ST_GET_WORKSPACE_LIMITS, "MX_ST_GET_WORKSPACE_LIMITS", is_error=False, is_resettable=False),
     MX_ST_GET_WORKSPACE_LIMITS_CFG:
     RobotStatusCodeInfo(MX_ST_GET_WORKSPACE_LIMITS_CFG, "MX_ST_GET_WORKSPACE_LIMITS_CFG", is_error=False, is_resettable=False),
     MX_ST_GET_TOOL_SPHERE:
     RobotStatusCodeInfo(MX_ST_GET_TOOL_SPHERE, "MX_ST_GET_TOOL_SPHERE", is_error=False, is_resettable=False),
+    MX_ST_GET_CALIBRATION_CFG:
+    RobotStatusCodeInfo(MX_ST_GET_CALIBRATION_CFG, "MX_ST_GET_CALIBRATION_CFG", is_error=False, is_resettable=False),
     MX_ST_GET_JOINT_LIMITS_CFG:
     RobotStatusCodeInfo(MX_ST_GET_JOINT_LIMITS_CFG, "MX_ST_GET_JOINT_LIMITS_CFG", is_error=False, is_resettable=False),
     MX_ST_GET_ROBOT_NAME:
     RobotStatusCodeInfo(MX_ST_GET_ROBOT_NAME, "MX_ST_GET_ROBOT_NAME", is_error=False, is_resettable=False),
     MX_ST_GET_MODEL_VEL_LIMITS:
     RobotStatusCodeInfo(MX_ST_GET_MODEL_VEL_LIMITS, "MX_ST_GET_MODEL_VEL_LIMITS", is_error=False, is_resettable=False),
     MX_ST_GET_CMD_DEF:
@@ -639,22 +722,30 @@
     RobotStatusCodeInfo(MX_ST_GET_MOTION_OPTIONS, "MX_ST_GET_MOTION_OPTIONS", is_error=False, is_resettable=False),
     MX_ST_GET_MONITORING_INTERVAL:
     RobotStatusCodeInfo(MX_ST_GET_MONITORING_INTERVAL, "MX_ST_GET_MONITORING_INTERVAL", is_error=False, is_resettable=False),
     MX_ST_GET_REAL_TIME_MONITORING:
     RobotStatusCodeInfo(MX_ST_GET_REAL_TIME_MONITORING, "MX_ST_GET_REAL_TIME_MONITORING", is_error=False, is_resettable=False),
     MX_ST_GET_NETWORK_OPTIONS:
     RobotStatusCodeInfo(MX_ST_GET_NETWORK_OPTIONS, "MX_ST_GET_NETWORK_OPTIONS", is_error=False, is_resettable=False),
+    MX_ST_GET_BRF_OFFSET:
+    RobotStatusCodeInfo(MX_ST_GET_BRF_OFFSET, "MX_ST_GET_BRF_OFFSET", is_error=False, is_resettable=False),
+    MX_ST_GET_FRF_OFFSET:
+    RobotStatusCodeInfo(MX_ST_GET_FRF_OFFSET, "MX_ST_GET_FRF_OFFSET", is_error=False, is_resettable=False),
+    MX_ST_GET_ROBOT_CALIBRATED:
+    RobotStatusCodeInfo(MX_ST_GET_ROBOT_CALIBRATED, "MX_ST_GET_ROBOT_CALIBRATED", is_error=False, is_resettable=False),
     MX_ST_GET_RTC:
     RobotStatusCodeInfo(MX_ST_GET_RTC, "MX_ST_GET_RTC", is_error=False, is_resettable=False),
     MX_ST_GET_BLENDING:
     RobotStatusCodeInfo(MX_ST_GET_BLENDING, "MX_ST_GET_BLENDING", is_error=False, is_resettable=False),
     MX_ST_GET_VEL_TIMEOUT:
     RobotStatusCodeInfo(MX_ST_GET_VEL_TIMEOUT, "MX_ST_GET_VEL_TIMEOUT", is_error=False, is_resettable=False),
     MX_ST_GET_JOINT_VEL:
     RobotStatusCodeInfo(MX_ST_GET_JOINT_VEL, "MX_ST_GET_JOINT_VEL", is_error=False, is_resettable=False),
+    MX_ST_GET_JOINT_VEL_LIMIT:
+    RobotStatusCodeInfo(MX_ST_GET_JOINT_VEL_LIMIT, "MX_ST_GET_JOINT_VEL_LIMIT", is_error=False, is_resettable=False),
     MX_ST_GET_JOINT_ACC:
     RobotStatusCodeInfo(MX_ST_GET_JOINT_ACC, "MX_ST_GET_JOINT_ACC", is_error=False, is_resettable=False),
     MX_ST_GET_CART_LIN_VEL:
     RobotStatusCodeInfo(MX_ST_GET_CART_LIN_VEL, "MX_ST_GET_CART_LIN_VEL", is_error=False, is_resettable=False),
     MX_ST_GET_CART_ANG_VEL:
     RobotStatusCodeInfo(MX_ST_GET_CART_ANG_VEL, "MX_ST_GET_CART_ANG_VEL", is_error=False, is_resettable=False),
     MX_ST_GET_CART_ACC:
@@ -711,30 +802,42 @@
     RobotStatusCodeInfo(MX_ST_RT_GRIPPER_VEL, "MX_ST_RT_GRIPPER_VEL", is_error=False, is_resettable=False),
     MX_ST_RT_EXTTOOL_STATUS:
     RobotStatusCodeInfo(MX_ST_RT_EXTTOOL_STATUS, "MX_ST_RT_EXTTOOL_STATUS", is_error=False, is_resettable=False),
     MX_ST_RT_GRIPPER_STATE:
     RobotStatusCodeInfo(MX_ST_RT_GRIPPER_STATE, "MX_ST_RT_GRIPPER_STATE", is_error=False, is_resettable=False),
     MX_ST_RT_VALVE_STATE:
     RobotStatusCodeInfo(MX_ST_RT_VALVE_STATE, "MX_ST_RT_VALVE_STATE", is_error=False, is_resettable=False),
+    MX_ST_RT_IO_STATUS:
+    RobotStatusCodeInfo(MX_ST_RT_IO_STATUS, "MX_ST_RT_IO_STATUS", is_error=False, is_resettable=False),
+    MX_ST_RT_OUTPUT_STATE:
+    RobotStatusCodeInfo(MX_ST_RT_OUTPUT_STATE, "MX_ST_RT_OUTPUT_STATE", is_error=False, is_resettable=False),
+    MX_ST_RT_INPUT_STATE:
+    RobotStatusCodeInfo(MX_ST_RT_INPUT_STATE, "MX_ST_RT_INPUT_STATE", is_error=False, is_resettable=False),
     MX_ST_RT_CHECKPOINT:
     RobotStatusCodeInfo(MX_ST_RT_CHECKPOINT, "MX_ST_RT_CHECKPOINT", is_error=False, is_resettable=False),
     MX_ST_RT_WRF:
     RobotStatusCodeInfo(MX_ST_RT_WRF, "MX_ST_RT_WRF", is_error=False, is_resettable=False),
     MX_ST_RT_TRF:
     RobotStatusCodeInfo(MX_ST_RT_TRF, "MX_ST_RT_TRF", is_error=False, is_resettable=False),
     MX_ST_RT_CYCLE_END:
     RobotStatusCodeInfo(MX_ST_RT_CYCLE_END, "MX_ST_RT_CYCLE_END", is_error=False, is_resettable=False),
+    MX_ST_RT_DEBUG_MG2_SAFE_MCU:
+    RobotStatusCodeInfo(MX_ST_RT_DEBUG_MG2_SAFE_MCU, "MX_ST_RT_DEBUG_MG2_SAFE_MCU", is_error=False, is_resettable=False),
+    MX_ST_RT_DEBUG_MG2_DRIVES:
+    RobotStatusCodeInfo(MX_ST_RT_DEBUG_MG2_DRIVES, "MX_ST_RT_DEBUG_MG2_DRIVES", is_error=False, is_resettable=False),
     MX_ST_OFFLINE_PROGRAM_LIST:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_LIST, "MX_ST_OFFLINE_PROGRAM_LIST", is_error=False, is_resettable=False),
     MX_ST_OFFLINE_PROGRAM_LOAD:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_LOAD, "MX_ST_OFFLINE_PROGRAM_LOAD", is_error=False, is_resettable=False),
     MX_ST_OFFLINE_PROGRAM_SAVE:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_SAVE, "MX_ST_OFFLINE_PROGRAM_SAVE", is_error=False, is_resettable=False),
     MX_ST_OFFLINE_PROGRAM_DELETE:
     RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_DELETE, "MX_ST_OFFLINE_PROGRAM_DELETE", is_error=False, is_resettable=False),
+    MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE:
+    RobotStatusCodeInfo(MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE, "MX_ST_OFFLINE_PROGRAM_RUNNING_DEMO_MODE", is_error=False, is_resettable=False),
     MX_ST_CONNECTED:
     RobotStatusCodeInfo(MX_ST_CONNECTED, "MX_ST_CONNECTED", is_error=False, is_resettable=False),
     MX_ST_USER_ALREADY:
     RobotStatusCodeInfo(MX_ST_USER_ALREADY, "MX_ST_USER_ALREADY", is_error=True, is_resettable=False),
     MX_ST_UPGRADE_IN_PROGRESS:
     RobotStatusCodeInfo(MX_ST_UPGRADE_IN_PROGRESS, "MX_ST_UPGRADE_IN_PROGRESS", is_error=False, is_resettable=False),
     MX_ST_CMD_TOO_LONG:
@@ -755,14 +858,18 @@
     RobotStatusCodeInfo(MX_ST_CANT_SAVE_OFFLINE, "MX_ST_CANT_SAVE_OFFLINE", is_error=True, is_resettable=True),
     MX_ST_IGNORING_CMD:
     RobotStatusCodeInfo(MX_ST_IGNORING_CMD, "MX_ST_IGNORING_CMD", is_error=True, is_resettable=True),
     MX_ST_NO_OFFLINE_SAVED:
     RobotStatusCodeInfo(MX_ST_NO_OFFLINE_SAVED, "MX_ST_NO_OFFLINE_SAVED", is_error=True, is_resettable=True),
     MX_ST_OFFLINE_LOOP:
     RobotStatusCodeInfo(MX_ST_OFFLINE_LOOP, "MX_ST_OFFLINE_LOOP", is_error=False, is_resettable=False),
+    MX_ST_DEV_MODE:
+    RobotStatusCodeInfo(MX_ST_DEV_MODE, "MX_ST_DEV_MODE", is_error=False, is_resettable=False),
+    MX_ST_PSU_DONGLE_STATUS:
+    RobotStatusCodeInfo(MX_ST_PSU_DONGLE_STATUS, "MX_ST_PSU_DONGLE_STATUS", is_error=False, is_resettable=False),
     MX_ST_OFFLINE_INVALID:
     RobotStatusCodeInfo(MX_ST_OFFLINE_INVALID, "MX_ST_OFFLINE_INVALID", is_error=True, is_resettable=True),
     MX_ST_ERROR_GRIPPER:
     RobotStatusCodeInfo(MX_ST_ERROR_GRIPPER, "MX_ST_ERROR_GRIPPER", is_error=True, is_resettable=True),
     MX_ST_ERROR_VBOX:
     RobotStatusCodeInfo(MX_ST_ERROR_VBOX, "MX_ST_ERROR_VBOX", is_error=True, is_resettable=True),
     MX_ST_MAINTENANCE_CHECK:
@@ -771,14 +878,16 @@
     RobotStatusCodeInfo(MX_ST_INTERNAL_ERROR, "MX_ST_INTERNAL_ERROR", is_error=True, is_resettable=True),
     MX_ST_TORQUE_LIMIT_STATUS:
     RobotStatusCodeInfo(MX_ST_TORQUE_LIMIT_STATUS, "MX_ST_TORQUE_LIMIT_STATUS", is_error=False, is_resettable=False),
     MX_ST_TORQUE_LIMIT_ERROR:
     RobotStatusCodeInfo(MX_ST_TORQUE_LIMIT_ERROR, "MX_ST_TORQUE_LIMIT_ERROR", is_error=True, is_resettable=True),
     MX_ST_COLLISION_STATUS:
     RobotStatusCodeInfo(MX_ST_COLLISION_STATUS, "MX_ST_COLLISION_STATUS", is_error=False, is_resettable=False),
+    MX_ST_COLLISION_STOP:
+    RobotStatusCodeInfo(MX_ST_COLLISION_STOP, "MX_ST_COLLISION_STOP", is_error=False, is_resettable=False),
     MX_ST_COLLISION_ERROR:
     RobotStatusCodeInfo(MX_ST_COLLISION_ERROR, "MX_ST_COLLISION_ERROR", is_error=True, is_resettable=True),
     MX_ST_CHECKPOINT_REACHED:
     RobotStatusCodeInfo(MX_ST_CHECKPOINT_REACHED, "MX_ST_CHECKPOINT_REACHED", is_error=False, is_resettable=False),
     MX_ST_TEXT_API_ERROR:
     RobotStatusCodeInfo(MX_ST_TEXT_API_ERROR, "MX_ST_TEXT_API_ERROR", is_error=True, is_resettable=True),
     MX_ST_NO_VALID_CFG:
@@ -795,14 +904,20 @@
     RobotStatusCodeInfo(MX_ST_EXT_TOOL_NEED_UPDATE, "MX_ST_EXT_TOOL_NEED_UPDATE", is_error=True, is_resettable=False),
     MX_ST_FW_NEED_REINSTALL:
     RobotStatusCodeInfo(MX_ST_FW_NEED_REINSTALL, "MX_ST_FW_NEED_REINSTALL", is_error=True, is_resettable=False),
     MX_ST_PSTOP2:
     RobotStatusCodeInfo(MX_ST_PSTOP2, "MX_ST_PSTOP2", is_error=False, is_resettable=False),
     MX_ST_ESTOP:
     RobotStatusCodeInfo(MX_ST_ESTOP, "MX_ST_ESTOP", is_error=False, is_resettable=False),
+    MX_ST_EXT_PORT_COMM_ERR:
+    RobotStatusCodeInfo(MX_ST_EXT_PORT_COMM_ERR, "MX_ST_EXT_PORT_COMM_ERR", is_error=True, is_resettable=True),
+    MX_ST_EXT_TOOL_COMM_ERR:
+    RobotStatusCodeInfo(MX_ST_EXT_TOOL_COMM_ERR, "MX_ST_EXT_TOOL_COMM_ERR", is_error=True, is_resettable=True),
+    MX_ST_PSU_ERROR:
+    RobotStatusCodeInfo(MX_ST_PSU_ERROR, "MX_ST_PSU_ERROR", is_error=True, is_resettable=False),
 }
 #
 # C constants from file mx_exttool_def.h
 #
 MX_EXT_TOOL_MPM500_NB_VALVES = 2  # MPM500 valve quantity
 MX_EXT_TOOL_VBOX_MAX_VALVES = 6  # Maximum valve quantity for comm protocol
 MX_EXT_TOOL_NONE = 0  # No external tool connected
```

### Comparing `mecademicpy-1.3.0/mecademicpy/robot.py` & `mecademicpy-1.4.0/mecademicpy/robot.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
         """
         if self._callback_thread:
             raise InvalidStateError(
                 'Cannot call RunCallbacks since callback handler is already running in separate thread.')
 
         # Setting timeout=0 means we don't block on an empty queue.
-        self._handle_callbacks(self.logger, self._callback_queue, self._robot_callbacks, timeout=0)
+        self._handle_callbacks(polling=True)
 
     def Connect(self,
                 address: str = MX_DEFAULT_ROBOT_IP,
                 enable_synchronous_mode: bool = False,
                 disconnect_on_exception: bool = True,
                 monitor_mode: bool = False,
                 offline_mode: bool = False,
-                timeout=0.1):
+                timeout=1.0):
         """Attempt to connect to a Mecademic Robot.
            This function is synchronous (awaits for success or timeout) even when using this class in asynchronous mode
            (see enable_synchronous_mode below).
 
         Parameters
         ----------
         address : string
@@ -233,139 +233,169 @@
         """
         if len(args) != self._robot_info.num_joints:
             raise ValueError('Incorrect number of joints sent to command.')
 
         self._send_motion_command('MoveJointsVel', args)
 
     @disconnect_on_exception
-    def MovePose(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MovePose(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Move robot's tool to an absolute Cartesian position (non-linear move, but all joints arrive simultaneously).
 
         Parameters
         ----------
         x, y, z : float
             Desired end effector coordinates in mm.
         alpha, beta, gamma
             Desired end effector orientation in degrees.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MovePose(200, 10, 100, 45)
+                - MovePose(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MovePose', [x, y, z, alpha, beta, gamma])
 
     @disconnect_on_exception
-    def MoveLin(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLin(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Linearly move robot's tool to an absolute Cartesian position.
 
         Parameters
         ----------
         x, y, z : float
             Desired end effector coordinates in mm.
         alpha, beta, gamma
             Desired end effector orientation in degrees.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MoveLin(200, 10, 100, 45)
+                - MoveLin(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MoveLin', [x, y, z, alpha, beta, gamma])
 
     @disconnect_on_exception
-    def MoveLinRelTrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinRelTrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Linearly move robot's tool to a Cartesian position relative to current TRF position.
 
         Parameters
         ----------
         x, y, z : float
             Desired displacement in mm.
         alpha, beta, gamma
             Desired orientation change in deg.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MoveLinRelTrf(200, 10, 100, 45)
+                - MoveLinRelTrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MoveLinRelTrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'MoveLinRelTrf' function instead")
     @disconnect_on_exception
-    def MoveLinRelTRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinRelTRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use MoveLinRelTrf instead.
         """
         self.MoveLinRelTrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
-    def MoveLinRelWrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinRelWrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Linearly move robot's tool to a Cartesian position relative to a reference frame that has the same
         orientation.
 
         Parameters
         ----------
         x, y, z : float
             Desired displacement in mm.
         alpha, beta, gamma
             Desired orientation change in deg.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MoveLinRelWrf(200, 10, 100, 45)
+                - MoveLinRelWrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MoveLinRelWrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'MoveLinRelWrf' function instead")
     @disconnect_on_exception
-    def MoveLinRelWRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinRelWRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use MoveLinRelWrf instead.
         """
         self.MoveLinRelWrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
-    def MoveLinVelTrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinVelTrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Move robot's by Cartesian velocity relative to the TRF.
 
            Joints will move for a time controlled by velocity timeout (SetVelTimeout).
 
         Parameters
         ----------
         x, y, z : float
             Desired velocity in mm/s.
         alpha, beta, gamma
             Desired angular velocity in degrees/s.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MoveLinVelTrf(200, 10, 100, 45)
+                - MoveLinVelTrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MoveLinVelTrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'MoveLinVelTrf' function instead")
     @disconnect_on_exception
-    def MoveLinVelTRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinVelTRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use MoveLinVelTrf instead
 
         """
         self.MoveLinVelTrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
-    def MoveLinVelWrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinVelWrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Move robot's by Cartesian velocity relative to the WRF.
 
            Joints will move for a time controlled by velocity timeout (SetVelTimeout).
 
         Parameters
         ----------
         x, y, z : float
             Desired velocity in mm/s.
         alpha, beta, gamma
             Desired angular velocity in degrees/s.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - MoveLinVelWrf(200, 10, 100, 45)
+                - MoveLinVelWrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('MoveLinVelWrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'MoveLinVelWrf' function instead")
     @disconnect_on_exception
-    def MoveLinVelWRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def MoveLinVelWRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use MoveLinVelWrf instead
 
         """
         self.MoveLinVelWrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
     def SetVelTimeout(self, t: float):
@@ -378,36 +408,41 @@
         t : float
             Desired duration for velocity-mode motion commands.
 
         """
         self._send_motion_command('SetVelTimeout', [t])
 
     @disconnect_on_exception
-    def SetConf(self, shoulder: int, elbow: int, wrist: int):
+    def SetConf(self, shoulder: int = None, elbow: int = None, wrist: int = None):
         """Manually set inverse kinematics options (and disable auto-conf).
+            On 4-axes robots (like Mcs500), shoulder and wrist values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - SetConf(1)
+                - SetConf(elbow=1)
 
         Parameters
         ----------
         shoulder : +1 or -1
             Shoulder inverse kinematics parameter.
         elbow : +1 or -1
             Elbow inverse kinematics parameter.
         wrist : +1 or -1
             Wrist inverse kinematics parameter.
 
         """
+        [shoulder, elbow, wrist] = self._normalize_conf_cmd_args(shoulder, elbow, wrist)
         self._send_motion_command('SetConf', [shoulder, elbow, wrist])
 
     @disconnect_on_exception
     def SetAutoConf(self, e: int):
         """Enable or disable auto-conf (automatic selection of inverse kinematics options).
 
         Parameters
         ----------
-        e : boolean
+        e : bool
             If true, robot will automatically choose the best configuration for the desired pose.
 
         """
         self._send_motion_command('SetAutoConf', [int(e)])
 
     @disconnect_on_exception
     def SetConfTurn(self, n: int):
@@ -423,15 +458,15 @@
 
     @disconnect_on_exception
     def SetAutoConfTurn(self, e: int):
         """Enable or disable auto-conf (automatic selection of inverse kinematics options) for joint 6.
 
         Parameters
         ----------
-        e : boolean
+        e : bool
             If true, robot will automatically choose the best configuration for the desired pose.
 
         """
         self._send_motion_command('SetAutoConfTurn', [int(e)])
 
     @disconnect_on_exception
     def SetBlending(self, p: float):
@@ -508,58 +543,84 @@
         p : float
             Target joint velocity, in percent.
 
         """
         self._send_motion_command('SetJointVel', [p])
 
     @disconnect_on_exception
-    def SetTrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def SetJointVelLimit(self, p: float):
+        """Change the safety joint velocity limit that is applied to all type of moves.
+        In joint space:     The joints velocity will be capped to this limit
+                            even if SetJointVel or MoveJointsVel request higher speed.
+        With linear moves:  The joints velocity will be capped to this limit regardless of the requested
+                            linear or angular velocity.
+
+        Parameters
+        ----------
+        p : float
+            Joint velocity limit in percent.
+
+        """
+        self._send_motion_command('SetJointVelLimit', [p])
+
+    @disconnect_on_exception
+    def SetTrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Set the TRF (tool reference frame) Cartesian position.
 
         Parameters
         ----------
         x, y, z : float
             Desired reference coordinates in mm.
         alpha, beta, gamma
             Desired reference orientation in degrees.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - SetTrf(200, 10, 100, 45)
+                - SetTrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('SetTrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'SetTrf' function instead")
     @disconnect_on_exception
-    def SetTRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def SetTRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use SetTrf instead
 
         """
         self.SetTrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
-    def SetWrf(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def SetWrf(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Set the WRF (world reference frame) Cartesian position.
 
         Parameters
         ----------
         x, y, z : float
             Desired reference coordinates in mm.
         alpha, beta, gamma
             Desired reference orientation in degrees.
+            On 4-axes robots (like Mcs500), alpha and beta values are not used and can be omitted.
+            Examples for 4-axes robots:
+                - SetWrf(200, 10, 100, 45)
+                - SetWrf(200, 10, 100, gamma=45)
 
         """
+        [alpha, beta, gamma] = self._normalize_cart_cmd_args(alpha, beta, gamma)
         self._send_motion_command('SetWrf', [x, y, z, alpha, beta, gamma])
 
     @deprecation.deprecated(deprecated_in="1.2.0",
                             removed_in="1.3.0",
                             current_version=__version__,
                             details="Use the 'SetWrf' function instead")
     @disconnect_on_exception
-    def SetWRF(self, x: float, y: float, z: float, alpha: float, beta: float, gamma: float):
+    def SetWRF(self, x: float, y: float, z: float, alpha: float = None, beta: float = None, gamma: float = None):
         """Deprecated use SetWrf instead
 
         """
         self.SetWrf(x, y, z, alpha, beta, gamma)
 
     @disconnect_on_exception
     def SetCheckpoint(self, n: int) -> InterruptableEvent:
@@ -620,16 +681,26 @@
             Maximum time to spend waiting for the move to complete (in seconds).
         """
         return super().WaitGripperMoveCompletion(timeout)
 
     @disconnect_on_exception
     def GripperOpen(self):
         """Open the gripper.
-           Note that the robot may move while the gripper is opening.
-           See method WaitGripperMoveCompletion for more information.
+           Note 1:  This command will not cause the robot to stop moving.
+
+           Note 2:  This command will be executed at the beginning of the blending (or deceleration) period of
+                    the previous command in the motion queue.
+                    You can insert a Delay before moving the gripper to make sure that gripper move starts only
+                    once the robot has stopped moving.
+
+           Note 3:  The robot will not wait for gripper move to be completed before continuing with the next command
+                    in the motion queue.
+                    If you need to wait for the gripper move to be completed before continuing your program, do not
+                    post any request in the motion queue after MoveGripper, then call method WaitGripperMoveCompletion
+                    in your application to know when your application can continue sending other move commands.
 
         """
         self._gripper_state_before_last_move = copy.deepcopy(self._gripper_state)
         self._send_motion_command('GripperOpen')
 
         if self._enable_synchronous_mode and self._robot_info.gripper_pos_ctrl_capable and self.GetRtExtToolStatus(
         ).is_gripper():
@@ -637,16 +708,26 @@
             if gripper_state.opened and gripper_state.target_pos_reached:
                 return
             self.WaitGripperMoveCompletion()
 
     @disconnect_on_exception
     def GripperClose(self):
         """Close the gripper.
-           Note that the robot may move while the gripper is closing.
-           See method WaitGripperMoveCompletion for more information.
+           Note 1:  This command will not cause the robot to stop moving.
+
+           Note 2:  This command will be executed at the beginning of the blending (or deceleration) period of
+                    the previous command in the motion queue.
+                    You can insert a Delay before moving the gripper to make sure that gripper move starts only
+                    once the robot has stopped moving.
+
+           Note 3:  The robot will not wait for gripper move to be completed before continuing with the next command
+                    in the motion queue.
+                    If you need to wait for the gripper move to be completed before continuing your program, do not
+                    post any request in the motion queue after MoveGripper, then call method WaitGripperMoveCompletion
+                    in your application to know when your application can continue sending other move commands.
 
         """
         self._gripper_state_before_last_move = copy.deepcopy(self._gripper_state)
         self._send_motion_command('GripperClose')
 
         if self._enable_synchronous_mode and self._robot_info.gripper_pos_ctrl_capable and self.GetRtExtToolStatus(
         ).is_gripper():
@@ -654,28 +735,38 @@
             if gripper_state.closed and gripper_state.target_pos_reached:
                 return
             self.WaitGripperMoveCompletion()
 
     @disconnect_on_exception
     def MoveGripper(self, target: Union[bool, float]):
         """Move the gripper to a target position.
-           Note that the robot may move while the gripper is moving.
-           See method WaitGripperMoveCompletion for more information.
+           Note 1:  This command will not cause the robot to stop moving.
 
-           If the target specified is a boolean, it indicates if the target position is the opened (True, GRIPPER_OPEN)
+           Note 2:  This command will be executed at the beginning of the blending (or deceleration) period of
+                    the previous command in the motion queue.
+                    You can insert a Delay before moving the gripper to make sure that gripper move starts only
+                    once the robot has stopped moving.
+
+           Note 3:  The robot will not wait for gripper move to be completed before continuing with the next command
+                    in the motion queue.
+                    If you need to wait for the gripper move to be completed before continuing your program, do not
+                    post any request in the motion queue after MoveGripper, then call method WaitGripperMoveCompletion
+                    in your application to know when your application can continue sending other move commands.
+
+           If the target specified is a bool, it indicates if the target position is the opened (True, GRIPPER_OPEN)
            or closed (False, GRIPPER_CLOSE) position.
            Otherwise the target position indicates the opening of the gripper, in mm from the most closed position.
 
         Corresponds to text API calls "GripperOpen" / "GripperClose" / "MoveGripper".
 
 
         Parameters
         ----------
-        target : boolean or float
-            boolean type: Open or close the gripper (GRIPPER_OPEN or GRIPPER_CLOSE)
+        target : bool or float
+            bool type: Open or close the gripper (GRIPPER_OPEN or GRIPPER_CLOSE)
             float type: The gripper's target position, in mm from the most closed position.
 
         """
         if isinstance(target, bool):
             if target:
                 self.GripperOpen()
             else:
@@ -730,33 +821,68 @@
             The position relative to the completely closed position that the gripper will move to when calling
             GripperOpen. In mm.
 
         """
         self._send_motion_command('SetGripperRange', [closePos, openPos])
 
     @disconnect_on_exception
-    def SetValveState(self, *args: list[int]):
+    def SetValveState(self, *args: Union[MxCmdValveState, int, str]):
         """Set the pneumatic module valve states.
-           Note that the robot may move while the valves are being opened/closed.
-           Using the Delay method may be appropriate to postpone subsequent move commands in the motion queue
-           if necessary.
+           Note 1:  This command will not cause the robot to stop moving.
+
+           Note 2:  This command will be executed at the beginning of the blending (or deceleration) period of
+                    the previous command in the motion queue.
+                    You can insert a Delay before changing the valves states to make sure that valves are changed
+                    once the robot has stopped moving.
 
         Parameters
         ----------
-        valve_1...valve_n : int
+        valve_1...valve_n :
             The desired state for valve:
-                - MxCmdValveState.MX_VALVE_STATE_STAY
-                - MxCmdValveState.MX_VALVE_STATE_CLOSE
-                - MxCmdValveState.MX_VALVE_STATE_OPEN
+                - MxCmdValveState.MX_VALVE_STATE_STAY (alternatively: -1, '*' or 'stay')
+                - MxCmdValveState.MX_VALVE_STATE_CLOSE (alternatively: 0 or 'close')
+                - MxCmdValveState.MX_VALVE_STATE_OPEN (alternatively: 1 or 'open')
             MPM500 pneumatic module has 2 valves.
 
         """
         self._send_motion_command('SetValveState', args)
 
     @disconnect_on_exception
+    def SetOutputState(self, bank_id: MxIoBankId, *args: Union[MxDigitalIoState, int, str]):
+        """Set the digital output states for the specified IO bank.
+           Note 1:  This command will not cause the robot to stop moving.
+
+           Note 2:  This command will be executed at the beginning of the blending (or deceleration) period of
+                    the previous command in the motion queue.
+                    You can insert a Delay before changing the IO states to make sure that they change
+                    once the robot has stopped moving.
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId
+            The IO bank Id to set output states for.
+        io_1...io_n : int
+            The desired IO state (the number of available outputs depends on the chosen bank id):
+                - MxDigitalIoState.MX_DIGITAL_IO_STATE_STAY (alternatively: -1, '*' or 'stay')
+                - MxDigitalIoState.MX_DIGITAL_IO_STATE_0 (alternatively: 0 or 'off')
+                - MxDigitalIoState.MX_DIGITAL_IO_STATE_1 (alternatively: 1 or 'on')
+
+        """
+        final_args = list(args)
+        final_args.insert(0, bank_id)
+        self._send_motion_command('SetOutputState', final_args)
+
+    @disconnect_on_exception
+    def SetOutputStateImmediate(self, bank_id: MxIoBankId, *args: Union[MxDigitalIoState, int, str]):
+        """Same as SetOutputState but without going through robot's motion queue (immediately applied)"""
+        final_args = list(args)
+        final_args.insert(0, bank_id)
+        self._send_motion_command('SetOutputStateImmediate', final_args)
+
+    @disconnect_on_exception
     def WaitForAnyCheckpoint(self, timeout: float = None):
         """Pause program execution until any checkpoint has been received from the robot.
 
         Parameters
         ----------
         timeout : float
             Maximum time to spend waiting for the checkpoint (in seconds).
@@ -803,20 +929,23 @@
 
     @disconnect_on_exception
     def WaitActivated(self, timeout: float = None):
         """Pause program execution until the robot is activated.
 
         Parameters
         ----------
-        timeout : float, by default 15
+        timeout : float, by default 30
             Maximum time to spend waiting for the event (in seconds).
         """
         # Use appropriate default timeout of not specified
         if timeout is None:
-            timeout = 15.0
+            if robot_model_is_mg2(self.GetRobotInfo().robot_model):
+                timeout = 5.0
+            else:
+                timeout = 30.0
         self._robot_events.on_activated.wait(timeout=timeout)
 
     @disconnect_on_exception
     def WaitDeactivated(self, timeout: float = None):
         """Pause program execution until the robot is deactivated.
 
         Parameters
@@ -833,15 +962,18 @@
         Parameters
         ----------
         timeout : float, by default 40
             Maximum time to spend waiting for the event (in seconds).
         """
         # Use appropriate default timeout of not specified
         if timeout is None:
-            timeout = 40.0
+            if robot_model_is_mg2(self.GetRobotInfo().robot_model):
+                timeout = 5.0
+            else:
+                timeout = 40.0
         self._robot_events.on_homed.wait(timeout=timeout)
 
     @disconnect_on_exception
     def WaitSimActivated(self, timeout: float = None):
         """Pause program execution until the robot simulation mode is activated.
 
         Parameters
@@ -895,14 +1027,52 @@
         """
         # Use appropriate default timeout of not specified
         if timeout is None:
             timeout = self.default_timeout
         self._robot_events.on_deactivate_ext_tool_sim.wait(timeout=timeout)
 
     @disconnect_on_exception
+    def WaitIoSimEnabled(self, bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE, timeout: float = None):
+        """Pause program execution until the robot PSU IO simulation mode is enabled.
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId, MxIoBankId.MX_IO_BANK_ID_IO_MODULE
+            Id of the IO module to wait for.
+        timeout : float, defaults to DEFAULT_WAIT_TIMEOUT
+            Maximum time to spend waiting for the event (in seconds).
+        """
+        # Use appropriate default timeout of not specified
+        if timeout is None:
+            timeout = self.default_timeout
+        if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+            self._robot_events.on_psu_io_sim_enabled.wait(timeout=timeout)
+        else:
+            self._robot_events.on_io_sim_enabled.wait(timeout=timeout)
+
+    @disconnect_on_exception
+    def WaitIoSimDisabled(self, bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE, timeout: float = None):
+        """Pause program execution until the robot IO simulation mode is disabled.
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId, MxIoBankId.MX_IO_BANK_ID_IO_MODULE
+            Id of the IO module to wait for.
+        timeout : float, defaults to DEFAULT_WAIT_TIMEOUT
+            Maximum time to spend waiting for the event (in seconds).
+        """
+        # Use appropriate default timeout of not specified
+        if timeout is None:
+            timeout = self.default_timeout
+        if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+            self._robot_events.on_psu_io_sim_disabled.wait(timeout=timeout)
+        else:
+            self._robot_events.on_io_sim_disabled.wait(timeout=timeout)
+
+    @disconnect_on_exception
     def WaitRecoveryMode(self, activated: bool, timeout: float = None):
         """Pause program execution until the robot recovery mode is in the requested state.
 
         Parameters
         ----------
         activated : bool
             Recovery mode to wait for (activated or deactivated
@@ -1123,15 +1293,15 @@
         if self._enable_synchronous_mode:
             checkpoint.wait()
 
     @disconnect_on_exception
     def SendCustomCommand(self,
                           command: str,
                           expected_responses: list[int] = None,
-                          timeout: float = None) -> InterruptableEvent:
+                          timeout: float = None) -> InterruptableEvent | Message:
         """Send custom command to robot (a command that the robot may support but that this Python API does not
            provide an explicit function for).
 
         Parameters
         ----------
         command : str
             Desired custom command.
@@ -1430,15 +1600,15 @@
                            timeout: float = None) -> ExtToolStatus:
         """Return a copy of the current external tool status
 
         Parameters
         ----------
         include_timestamp : bool
             If true, return a TimestampedData object, otherwise just return states.
-        synchronous_update: boolean
+        synchronous_update: bool
             True -> Synchronously get updated external tool status. False -> Get latest known status.
         timeout: float
             Timeout (in seconds) waiting for synchronous response from the robot.
 
         Returns
         -------
         TimestampedData or ExtToolStatus
@@ -1454,25 +1624,68 @@
         with self._main_lock:
             if include_timestamp:
                 return copy.deepcopy(self._robot_rt_data.rt_external_tool_status)
             else:
                 return copy.deepcopy(self._external_tool_status)
 
     @disconnect_on_exception
+    def GetRtIoStatus(self,
+                      bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE,
+                      include_timestamp: bool = False,
+                      synchronous_update: bool = False,
+                      timeout: float = None) -> IoStatus:
+        """Return a copy of the current IO module status
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId
+            The IO bank Id to get output states for.
+        synchronous_update: bool
+            True -> Synchronously get updated IO module status. False -> Get latest known status.
+        timeout: float
+            Timeout (in seconds) waiting for synchronous response from the robot.
+
+        Returns
+        -------
+        TimestampedData or IoStatus
+            Object containing the current IO module status
+
+        """
+        # Use appropriate default timeout of not specified
+        if timeout is None:
+            timeout = self.default_timeout
+        if synchronous_update:
+            self._send_sync_command(f'GetRtIoStatus({bank_id})', self._robot_events.on_output_state_updated, timeout)
+
+        with self._main_lock:
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                if include_timestamp:
+                    return copy.deepcopy(self._robot_rt_data.rt_psu_io_status)
+                else:
+                    return copy.deepcopy(self._rt_psu_io_status)
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                if include_timestamp:
+                    return copy.deepcopy(self._robot_rt_data.rt_io_module_status)
+                else:
+                    return copy.deepcopy(self._rt_io_module_status)
+            else:
+                raise MecademicException("Argument Error in Command : GetRtIoStatus")
+
+    @disconnect_on_exception
     def GetRtGripperState(self,
                           include_timestamp: bool = False,
                           synchronous_update: bool = False,
                           timeout: float = None) -> GripperState:
         """Return a copy of the current gripper state
 
         Parameters
         ----------
         include_timestamp : bool
             If true, return a TimestampedData object, otherwise just return states.
-        synchronous_update: boolean
+        synchronous_update: bool
             True -> Synchronously get updated gripper state. False -> Get latest known status.
         timeout: float
             Timeout (in seconds) waiting for synchronous response from the robot.
 
         Returns
         -------
         TimestampedData or GripperState
@@ -1498,15 +1711,15 @@
                         timeout: float = None) -> ValveState:
         """Return a copy of the current valve state
 
         Parameters
         ----------
         include_timestamp : bool
             If true, return a TimestampedData object, otherwise just return states.
-        synchronous_update: boolean
+        synchronous_update: bool
             True -> Synchronously get updated valve states. False -> Get latest known status.
         timeout: float
             Timeout (in seconds) waiting for synchronous response from the robot.
 
         Returns
         -------
         TimestampedData or ValveState
@@ -1522,14 +1735,87 @@
         with self._main_lock:
             if include_timestamp:
                 return copy.deepcopy(self._robot_rt_data.rt_valve_state)
             else:
                 return copy.deepcopy(self._valve_state)
 
     @disconnect_on_exception
+    def GetRtOutputState(self,
+                         bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE,
+                         synchronous_update: bool = False,
+                         timeout: float = None) -> TimestampedData:
+        """Return a copy of the current digital outputs state
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId
+            The IO bank Id to get output states for.
+        synchronous_update: bool
+            True -> Synchronously get updated states. False -> Get latest known status.
+        timeout: float
+            Timeout (in seconds) waiting for synchronous response from the robot.
+
+        Returns
+        -------
+        TimestampedData
+            Object containing the current digital output states for requested bank id.
+
+        """
+        # Use appropriate default timeout of not specified
+        if timeout is None:
+            timeout = self.default_timeout
+        if synchronous_update:
+            self._send_sync_command(f'GetRtOutputState({bank_id})', self._robot_events.on_output_state_updated, timeout)
+
+        with self._main_lock:
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                return copy.deepcopy(self._robot_rt_data.rt_psu_outputs)
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                return copy.deepcopy(self._robot_rt_data.rt_io_module_outputs)
+            else:
+                return TimestampedData.zeros(0)
+
+    @disconnect_on_exception
+    def GetRtInputState(self,
+                        bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE,
+                        synchronous_update: bool = False,
+                        timeout: float = None) -> TimestampedData:
+        """Return a copy of the current digital inputs state
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId
+            The IO bank Id to get input states for.
+        synchronous_update: bool
+            True -> Synchronously get updated states. False -> Get latest known status.
+        timeout: float
+            Timeout (in seconds) waiting for synchronous response from the robot.
+
+        Returns
+        -------
+        TimestampedData
+            Object containing the current digital input states for requested bank id.
+
+        """
+
+        # Use appropriate default timeout of not specified
+        if timeout is None:
+            timeout = self.default_timeout
+        if synchronous_update:
+            self._send_sync_command(f'GetRtInputState({bank_id})', self._robot_events.on_input_state_updated, timeout)
+
+        with self._main_lock:
+            if bank_id == MxIoBankId.MX_IO_BANK_ID_PSU:
+                return copy.deepcopy(self._robot_rt_data.rt_psu_inputs)
+            elif bank_id == MxIoBankId.MX_IO_BANK_ID_IO_MODULE:
+                return copy.deepcopy(self._robot_rt_data.rt_io_module_inputs)
+            else:
+                return TimestampedData.zeros(0)
+
+    @disconnect_on_exception
     def GetRtTargetJointPos(self,
                             include_timestamp: bool = False,
                             synchronous_update: bool = False,
                             timeout: float = None) -> TimestampedData:
         """Returns the real-time target joint positions of the robot.
 
         Parameters
@@ -1643,15 +1929,16 @@
     def SetRealTimeMonitoring(self, *events: tuple):
         """Configure which real-time monitoring events to enable.
 
         Parameters
         ----------
         events : list of event IDs
             List of event IDs to enable.
-            Example: events=[MxRobotStatusCode.MX_ST_RT_TARGET_JOINT_POS, MxRobotStatusCode.MX_ST_RT_TARGET_CART_POS]
+            Example:
+          SetRealTimeMonitoring(MxRobotStatusCode.MX_ST_RT_TARGET_JOINT_POS, MxRobotStatusCode.MX_ST_RT_TARGET_CART_POS)
             enables the target joint positions and target end effector pose messages.
             Can also use events='all' to enable all.
 
         """
         with self._main_lock:
             self._check_internal_states()
             if isinstance(events, tuple):
@@ -1727,14 +2014,38 @@
         if self._enable_synchronous_mode:
             if sim_ext_tool_type == MxExtToolType.MX_EXT_TOOL_NONE:
                 self.WaitExtToolSimDeactivated()
             else:
                 self.WaitExtToolSimActivated()
 
     @disconnect_on_exception
+    def SetIoSim(self, bank_id: MxIoBankId = MxIoBankId.MX_IO_BANK_ID_IO_MODULE, enable: bool = True):
+        """Enable or disable IO simulation. This allows emulating the presence of an IO module and use the
+           corresponding APIs (ex: SetOutputState) without the module to be physically present.
+           This can also be used even if the physical module is present to test the APIs without actually applying the
+           changes on the physical module (to test the APIs without the robot moving)
+
+        Parameters
+        ----------
+        bank_id : MxIoBankId
+            The IO bank Id to enable or disable simulation mode for.
+        enable : bool
+            Enable or disable simulation mode.
+        """
+        with self._main_lock:
+            self._check_internal_states()
+            self._send_command('SetIoSim', [bank_id, 1 if enable else 0])
+
+        if self._enable_synchronous_mode:
+            if enable:
+                self.WaitIoSimEnabled(bank_id)
+            else:
+                self.WaitIoSimDisabled(bank_id)
+
+    @disconnect_on_exception
     def SetRecoveryMode(self, activated: bool = True):
         """Enable/disable recovery mode, allowing robot to move (slowly) without homing and without joint limits."""
         with self._main_lock:
             self._check_internal_states()
             self._send_command('SetRecoveryMode', f'{1 if activated else 0}')
 
         if self._enable_synchronous_mode:
@@ -1906,15 +2217,18 @@
         skip_acceleration : MxTorqueLimitsMode
             Whether torque limits are ignored during acceleration periods (allowing fast accelerations without
             triggering torque limits exceeded condition)
             Available modes (see MxTorqueLimitsMode):
                 - MX_TORQUE_LIMITS_DETECT_ALL or 0 or False : Always check if torque is within limits
                 - MX_TORQUE_LIMITS_DETECT_SKIP_ACCEL or 1 or True : Do not check if torque is within limits during acceleration
         """
-        severity_int = TORQUE_LIMIT_SEVERITIES[severity] if type(severity) == str else severity
+        if isinstance(severity, str):
+            severity_int = TORQUE_LIMIT_SEVERITIES[severity]
+        else:
+            severity_int = severity
         skip_acceleration_int = 1 if skip_acceleration else 0
         self._send_motion_command('SetTorqueLimitsCfg', [severity_int, skip_acceleration_int])
 
     @disconnect_on_exception
     def SetTorqueLimits(self, *args: float):
         """Set the torque limit (in percent) for each joint.
         Note that torque limits will be applied only if severity mode is set to other than 'disabled' by
@@ -1989,15 +2303,15 @@
 
     @disconnect_on_exception
     def GetRobotRtData(self, synchronous_update: bool = False, timeout: float = None) -> RobotRtData:
         """Return a copy of the current robot real-time data, with all values associated with the same timestamp
 
         Parameters
         ----------
-        synchronous_update: boolean
+        synchronous_update: bool
             True -> Synchronously wait for the next data cycle to get updated data. False -> Get latest known data.
         timeout: float
             Timeout (in seconds) waiting for updated cyclic data from the robot. Only used for synchronous requests.
 
         Return
         ------
         RobotRtData
@@ -2012,15 +2326,15 @@
 
     @disconnect_on_exception
     def GetStatusRobot(self, synchronous_update: bool = False, timeout: float = None) -> RobotStatus:
         """Return a copy of the current robot status
 
         Parameters
         ----------
-        synchronous_update: boolean
+        synchronous_update: bool
             True -> Synchronously get updated robot status. False -> Get latest known status.
         timeout: float, defaults to DEFAULT_WAIT_TIMEOUT
             Timeout (in seconds) waiting for synchronous response from the robot.
 
         Returns
         -------
         RobotStatus
@@ -2049,15 +2363,16 @@
         # Use appropriate default timeout of not specified
         if timeout is None:
             timeout = self.default_timeout
 
         response = self._send_custom_command('GetGripperRange',
                                              expected_responses=[MxRobotStatusCode.MX_ST_GET_GRIPPER_RANGE],
                                              timeout=self.default_timeout)
-        positions = string_to_numbers(response.data)
+        if isinstance(response, Message):
+            positions = string_to_numbers(response.data)
         assert len(positions) == 2
         return positions[0], positions[1]
 
     def LogTrace(self, trace: str):
         """Send a text trace that is printed in the robot's log internal file (which can be retrieved from robot's Web
            portal under menu "Options -> Get Log").
            (useful for clearly identifying steps of a program within robot's log when reporting problems to
```

### Comparing `mecademicpy-1.3.0/mecademicpy/robot_classes.py` & `mecademicpy-1.4.0/mecademicpy/robot_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,14 +140,18 @@
             Function to be called once gripper status is updated (legacy, use following external tools callbacks).
         on_external_tool_status_updated: function object
             Function to be called once external tool status is updated.
         on_gripper_state_updated: function object
             Function to be called once gripper state is updated.
         on_valve_state_updated: function object
             Function to be called once valve state is updated.
+        on_output_state_updated: function object
+            Function to be called when digital outputs changed.
+        on_input_state_updated: function object
+            Function to be called when digital inputs changed.
         on_activated : function object
             Function to be called once activated.
         on_deactivated : function object
             Function to be called once deactivated.
         on_homed : function object
             Function to be called once homing is complete.
         on_error : function object
@@ -177,37 +181,53 @@
             Function to be called once sim mode is activated.
         on_deactivate_sim : function object
             Function to be called once sim mode is deactivated.
         on_activate_ext_tool_sim : function object
             Function to be called once gripper sim mode is activated.
         on_deactivate_ext_tool_sim : function object
             Function to be called once gripper sim mode is deactivated.
+        on_psu_io_sim_enabled : function object
+            Function to be called once power supply Io simulation mode is enabled.
+        on_psu_io_sim_disabled : function object
+            Function to be called once power supply Io simulation mode is disabled.
+        on_io_sim_enabled : function object
+            Function to be called once IO simulation mode is enabled.
+        on_io_sim_disabled : function object
+            Function to be called once IO simulation mode is disabled.
         on_activate_recovery_mode : function object
             Function to be called once recovery mode is activated.
         on_deactivate_recovery_mode : function object
             Function to be called once recovery mode is deactivated.
         on_command_message : function object
             Function to be called each time a command response is received.
         on_monitor_message : function object
-            Function to be called each time a monitor response is received.
+            Function to be called each time an event is received on the monitoring port.
+            Only available when connected to the robot in monitoring mode.
+            Note that on_monitor_message may not be very useful. We suggest to use on_end_of_cycle instead
+            (which works for both monitoring or control mode connections).
         on_offline_program_state : function object
             Function to be called each time an offline program starts or fails to start.
         on_end_of_cycle : function object
-            Function to be called each time end of cycle is reached."""
+            Function to be called each time end of cycle is reached.
+            It's called once all real-time data for current monitoring interval has been received.
+            At this moment, all robot real-time data is coherent (belongs to the same cycle).
+            """
 
     def __init__(self):
         self.on_connected = None
         self.on_disconnected = None
 
         self.on_status_updated = None
         self.on_status_gripper_updated = None
 
         self.on_external_tool_status_updated = None
         self.on_gripper_state_updated = None
         self.on_valve_state_updated = None
+        self.on_output_state_updated = None
+        self.on_input_state_updated = None
 
         self.on_activated = None
         self.on_deactivated = None
 
         self.on_homed = None
 
         self.on_error = None
@@ -225,14 +245,18 @@
         self.on_checkpoint_reached = None
 
         self.on_activate_sim = None
         self.on_deactivate_sim = None
 
         self.on_activate_ext_tool_sim = None
         self.on_deactivate_ext_tool_sim = None
+        self.on_psu_io_sim_enabled = None
+        self.on_psu_io_sim_disabled = None
+        self.on_io_sim_enabled = None
+        self.on_io_sim_disabled = None
 
         self.on_activate_recovery_mode = None
         self.on_deactivate_recovery_mode = None
 
         self.on_command_message = None
         self.on_monitor_message = None
 
@@ -411,14 +435,36 @@
         """
         self.full_version = version
         self.update_version(self.full_version)
 
     def __str__(self) -> str:
         return self.full_version
 
+    def get_str(self, build=False, extra=False) -> str:
+        """Get version string
+
+        Parameters
+        ----------
+        build : bool, optional
+            Include the build number in the version (ex:9.3.0.4739), by default False
+        extra : bool, optional
+            Include the build 'extra in the version (ex:9.3.0.4739-master), by default False
+
+        Returns
+        -------
+        str
+            Formatted version string
+        """
+        version_to_return = self.short_version
+        if build and self.build:
+            version_to_return += f'.{self.build}'
+        if extra and self.extra:
+            version_to_return += f'-{self.extra}'
+        return version_to_return
+
     def update_version(self, version: str):
         """Update object firmware version values by parsing a version string.
 
         :param version: string
             New version of firmware. Supports multiple version formats
             ie. 8.1.9, 8.4.3.1805-official
         """
@@ -437,20 +483,15 @@
         self.build = None
         self.extra = None
         if regex_version.group("build"):
             self.build = int(regex_version.group("build"))
         if regex_version.group("extra"):
             self.extra = regex_version.group("extra")
 
-        self.full_version = self.short_version
-        if self.build:
-            self.full_version += f".{self.build}"
-
-        if self.extra:
-            self.full_version += f"-{self.extra}"
+        self.full_version = self.get_str(build=True, extra=True)
 
     def is_at_least(self, major, minor=0, patch=0) -> bool:
         """Tells if this RobotInfo instance's version is at least the specified version
 
         Parameters
         ----------
         major : integer
@@ -485,20 +526,24 @@
 
 
 class RobotInfo:
     """Class for storing metadata about a robot.
 
     Attributes
     ----------
+    robot_model: MxRobotModel
+        Model of robot
     model : string
-        Model of robot.
+        Model of robot (legacy, use robot_model instead since it's an enum with well-known values)
     revision : int
         Robot revision.
     is_virtual : bool
         True if is a virtual robot.
+    is_safe_boot : bool
+        True if is booted in safe-boot mode.
     version : str
         robot firmware revision number as received from the connection string.
     serial : string
         Serial identifier of robot.
     ip_address : string
         IP address of this robot.
     rt_message_capable : bool
@@ -507,55 +552,75 @@
         True if robot is capable of sending real-time monitoring messages on control port (SetCtrlPortMonitoring).
     num_joints : int
         Number of joints on the robot.
     requires_homing : bool
         Tells if this robot requires homing.
     supports_ext_tool : bool
         Tells if this robot supports connecting external tools (gripper or valve box).
+    supports_io_module : bool
+        Tells if this robot supports IO expansion module.
     gripper_pos_ctrl_capable : bool
         Tells if this robot supports gripper position control.
     ext_tool_version_capable : bool
         Tells if this robot supports external tool fw version fetch.
     ext_tool_version : str
         External tool firmware revision number as received from the connection string.
         Version 0.0.0.0 if device isn't connected or ext_tool_version_capable == False.
 """
 
     def __init__(self,
                  model: str = 'Unknown',
                  revision: int = 0,
                  is_virtual: bool = False,
+                 is_safe_boot: bool = False,
                  version: str = '0.0.0',
                  serial: str = '',
                  ext_tool_version: str = '0.0.0.0'):
+        self.robot_model = MxRobotModel.MX_ROBOT_MODEL_M500_R3
         self.model = model
         self.revision = revision
         self.is_virtual = is_virtual
+        self.is_safe_boot = is_safe_boot
         self.version = RobotVersion(version)
         self.serial = serial
         self.ip_address = None  # Set later
         self.rt_message_capable = False
         self.rt_on_ctrl_port_capable = False
         self.gripper_pos_ctrl_capable = False
         self.ext_tool_version_capable = False
         self.ext_tool_version = RobotVersion(ext_tool_version)
+        self.psu_dongle_detected = False
 
         if self.model == 'Meca500':
+            if self.revision == 1:
+                self.robot_model = MxRobotModel.MX_ROBOT_MODEL_M500_R1
+            elif self.revision == 2:
+                self.robot_model = MxRobotModel.MX_ROBOT_MODEL_M500_R2
+            elif self.revision == 3:
+                self.robot_model = MxRobotModel.MX_ROBOT_MODEL_M500_R3
+            elif self.revision == 4:
+                self.robot_model = MxRobotModel.MX_ROBOT_MODEL_M500_R4
             self.num_joints = 6
             self.requires_homing = True
             self.supports_ext_tool = True
-        elif self.model == 'Scara':
+            self.supports_io_module = False
+        elif self.model == 'Mcs500':
+            self.robot_model = MxRobotModel.MX_ROBOT_MODEL_MCS500_R1
             self.num_joints = 4
             self.requires_homing = False
             self.supports_ext_tool = False
+            self.supports_io_module = True
         elif self.model == 'Unknown':
+            self.robot_model = MxRobotModel.MX_ROBOT_MODEL_UNKNOWN
             self.num_joints = 1
             self.requires_homing = False
             self.supports_ext_tool = False
+            self.supports_ext_tool = False
         else:
+            self.robot_model = MxRobotModel.MX_ROBOT_MODEL_UNKNOWN
             raise ValueError(f'Invalid robot model: {self.model}')
 
         # Check if this robot supports real-time monitoring events
         if self.version.is_at_least(8, 4):
             self.rt_message_capable = True
         # Check if this robot supports real-time monitoring on control port
         if self.version.is_at_least(9, 0):
@@ -582,29 +647,36 @@
         Parameters
         ----------
         input_string : string
             Input string to be parsed.
 
         """
         ROBOT_CONNECTION_STRING = r"Connected to (?P<model>[\w|-]+) ?R?(?P<revision>\d)?"
-        ROBOT_CONNECTION_STRING += r"(?P<virtual>-virtual)?( v|_)?(?P<version>\d+\.\d+\.\d+)"
+        ROBOT_CONNECTION_STRING += r"(?P<virtual>-virtual)?(?P<safe_boot>-safe-boot)?( v|_)?(?P<version>\d+\.\d+\.\d+)"
 
         virtual = False
+        safe_boot = False
 
         try:
             robot_info_regex = re.search(ROBOT_CONNECTION_STRING, input_string)
             if robot_info_regex is None:
                 raise ValueError(f'Could not parse robot info string "{input_string}"')
             if robot_info_regex.group('model'):
                 model = robot_info_regex.group('model')
             if robot_info_regex.group('revision'):
                 revision = int(robot_info_regex.group('revision'))
             if robot_info_regex.group('virtual'):
                 virtual = True
-            return cls(model=model, revision=revision, is_virtual=virtual, version=robot_info_regex.group('version'))
+            if robot_info_regex.group('safe_boot'):
+                safe_boot = True
+            return cls(model=model,
+                       revision=revision,
+                       is_virtual=virtual,
+                       is_safe_boot=safe_boot,
+                       version=robot_info_regex.group('version'))
         except Exception as exception:
             raise ValueError(f'Could not parse robot info string "{input_string}", error: {exception}')
 
     def get_serial_digit(self) -> int:
         """Returns robot serial digits.
            ie. M500-0123 -> 123
 
@@ -619,27 +691,49 @@
             raise ValueError(f'Invalid serial number string received: {self.serial}, expecting "M500-1234"')
 
         serial_digit = int(serial_split[1])
         return serial_digit
 
 
 class UpdateProgress:
-    """ Class containing firmware update progress information
+    """Class for storing the robot's firmware update status.
 
     Attributes
     ----------
+    in_progress : bool
+        Firmware update is in progress
     complete : bool
-        Firmware update process state
-    progress : string
+        Firmware update has completed
+    version : str
+        The firmware version being installed
+    error : boolean
+        Tells if the update failed
+    error_msg : str
+        Message that explains why the update failed
+    progress : str
         Update progress message received from robot
+    step : str
+        String that describes the current firmware update step being performed
+
+    _last_print_timestamp : float
+        Last time we have printed the firmware update status
 """
 
-    def __init__(self) -> None:
-        self.complete: bool = False
-        self.progress: str = ''
+    def __init__(self):
+        # The following are status fields.
+        self.in_progress = False
+        self.complete = False
+        self.version = ""
+        self.error = False
+        self.error_msg = ""
+        self.progress = 0.0
+        self.progress_str = ""  # For legacy update
+        self.step = ""
+
+        self._last_print_timestamp = 0.0
 
 
 class TimestampedData:
     """ Class for storing timestamped data (real-time data received from the robot)
 
     Attributes
     ----------
@@ -675,16 +769,18 @@
         ----------
         input_string : string
             Comma-separated string. First value is timestamp, rest is data.
 
         """
         numbs = tools.string_to_numbers(input_string)
 
-        if (len(numbs) - 1) != len(self.data):
+        if (len(numbs) - 1) < len(self.data):
             raise ValueError('Cannot update TimestampedData with incompatible data.')
+        elif (len(numbs) - 1) > len(self.data):
+            numbs = numbs[0:len(self.data) + 1]
 
         if numbs[0] >= self.timestamp:
             self.timestamp = numbs[0]
             self.data = numbs[1:]
 
     def update_from_data(self, timestamp: int, data: list[float]):
         """Update with data unless timestamp is older
@@ -805,39 +901,61 @@
     rt_gripper_state : TimestampedData
         Gripper state [holding_part, target_pos_reached, opened, closed]. (GetRtGripperState)
     rt_gripper_force : TimestampedData
         Gripper force in % of maximum force. (GetRtGripperForce)
     rt_gripper_pos : TimestampedData. (GetRtValveState)
         Gripper position in mm. (GetRtGripperPos)
 
+    rt_psu_io_status : TimestampedData
+        Power supply's IO module status
+    rt_psu_outputs : TimestampedData
+        Power supply's digital outputs state [output[0], output[1], ...]. (GetRtOutputState)
+    rt_psu_inputs : TimestampedData
+        Power supply's digital inputs state [input[0], input[1], ...]. (GetRtInputState)
+
+    rt_io_module_status : TimestampedData
+        IO module status
+    rt_io_module_outputs : TimestampedData
+        IO module's digital outputs state [output[0], output[1], ...]. (GetRtOutputState)
+    rt_io_module_inputs : TimestampedData
+        IO module's digital inputs state [input[0], input[1], ...]. (GetRtInputState)
+
     rt_wrf : TimestampedData
         Current definition of the WRF w.r.t. the BRF with timestamp. Cartesian data are in mm, Euler angles in degrees.
         [cartesian coordinates x, y, z, Euler angles omega-x, omega-y, omega-z] (GetRtWrf)
     rt_trf : TimestampedData
         Current definition of the TRF w.r.t. the FRF with timestamp. cartesian data are in mm, Euler angles in degrees.
         [cartesian coordinates x, y, z, Euler angles omega-x, omega-y, omega-z] (GetRtTrf)
     rt_checkpoint : TimestampedData
         Last executed checkpoint with timestamp. (GetCheckpoint)
 """
 
     def __init__(self, num_joints: int):
+        self._init_timestamped_data(num_joints)
+        self.max_queue_size = 0
+
+    def _init_timestamped_data(self, num_joints: int):
+        """Initialize timestamped data class members according to detected robot model (number of joints)"""
+        nb_cart_val = num_joints  # 4 degrees of liberty for 4 joints robots, 6 for 6 joint robots
+        nb_conf_val = 3 if num_joints == 6 else 1  # 4 degrees of liberty for 4 joints robots, 6 for 6 joint robots
+
         self.rt_target_joint_pos = TimestampedData.zeros(num_joints)  # microseconds timestamp, degrees
-        self.rt_target_cart_pos = TimestampedData.zeros(6)  # microseconds timestamp, mm and degrees
+        self.rt_target_cart_pos = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm and degrees
         self.rt_target_joint_vel = TimestampedData.zeros(num_joints)  # microseconds timestamp, degrees/second
-        self.rt_target_cart_vel = TimestampedData.zeros(6)  # microseconds timestamp, mm/s and deg/s
+        self.rt_target_cart_vel = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm/s and deg/s
         self.rt_target_joint_torq = TimestampedData.zeros(num_joints)  # microseconds timestamp, percent of maximum
-        self.rt_target_conf = TimestampedData.zeros(3)
+        self.rt_target_conf = TimestampedData.zeros(nb_conf_val)
         self.rt_target_conf_turn = TimestampedData.zeros(1)
 
         self.rt_joint_pos = TimestampedData.zeros(num_joints)  # microseconds timestamp, degrees
-        self.rt_cart_pos = TimestampedData.zeros(6)  # microseconds timestamp, mm and degrees
+        self.rt_cart_pos = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm and degrees
         self.rt_joint_vel = TimestampedData.zeros(num_joints)  # microseconds timestamp, degrees/second
         self.rt_joint_torq = TimestampedData.zeros(num_joints)  # microseconds timestamp, percent of maximum
-        self.rt_cart_vel = TimestampedData.zeros(6)  # microseconds timestamp, mm/s and deg/s
-        self.rt_conf = TimestampedData.zeros(3)
+        self.rt_cart_vel = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm/s and deg/s
+        self.rt_conf = TimestampedData.zeros(nb_conf_val)
         self.rt_conf_turn = TimestampedData.zeros(1)
 
         # Another way of getting robot joint position using less-precise encoders.
         # For robot production testing (otherwise use rt_joint_pos which is much more precise)
         self.rt_abs_joint_pos = TimestampedData.zeros(num_joints)  # microseconds timestamp, degrees
 
         # Contains dictionary of accelerometers stored in the robot indexed by joint number.
@@ -849,19 +967,25 @@
         self.rt_valve_state = TimestampedData.zeros(
             MX_EXT_TOOL_MPM500_NB_VALVES)  # microseconds timestamp, valve1 opened, valve2 opened
         self.rt_gripper_state = TimestampedData.zeros(
             4)  # microseconds timestamp, holding part, target pos reached, closed, opened
         self.rt_gripper_force = TimestampedData.zeros(1)  # microseconds timestamp, gripper force [%]
         self.rt_gripper_pos = TimestampedData.zeros(1)  # microseconds timestamp, gripper position [mm]
 
-        self.rt_wrf = TimestampedData.zeros(6)  # microseconds timestamp, mm and degrees
-        self.rt_trf = TimestampedData.zeros(6)  # microseconds timestamp, mm and degrees
-        self.rt_checkpoint = TimestampedData.zeros(1)  # microseconds timestamp, checkpointId
+        self.rt_psu_io_status = TimestampedData.zeros(4)
+        self.rt_psu_outputs = TimestampedData.zeros(0)
+        self.rt_psu_inputs = TimestampedData.zeros(0)
+
+        self.rt_io_module_status = TimestampedData.zeros(4)
+        self.rt_io_module_outputs = TimestampedData.zeros(0)
+        self.rt_io_module_inputs = TimestampedData.zeros(0)
 
-        self.max_queue_size = 0
+        self.rt_wrf = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm and degrees
+        self.rt_trf = TimestampedData.zeros(nb_cart_val)  # microseconds timestamp, mm and degrees
+        self.rt_checkpoint = TimestampedData.zeros(1)  # microseconds timestamp, checkpointId
 
     def _for_each_rt_data(self):
         """Iterates for each TimestampedData type member of this class (rt_joint_pos, rt_cart_pos, etc.)
         """
         # Collect class member names
         member_names = vars(self)
         # Iterate though all "rt_" members
@@ -933,14 +1057,20 @@
         self.error_status = False
         self.pstop2State = MxStopState.MX_STOP_STATE_RESET
         self.estopState = MxStopState.MX_STOP_STATE_RESET
         self.pause_motion_status = False
         self.end_of_block_status = False
         self.brakes_engaged = False
 
+    def __str__(self) -> str:
+        return f"Activated: {self.activation_state}, homed: {self.homing_state}, sim: {self.simulation_mode}, " \
+               f"recovery mode: {self.recovery_mode}, error: {self.error_status}, pstop2 state: {self.pstop2State}, " \
+               f"estop state: {str(self.estopState)}, pause motion: {str(self.pause_motion_status)}, " \
+               f"EOB: {self.end_of_block_status}, brakes engaged: {self.brakes_engaged}"
+
 
 class GripperStatus:
     """Class for storing the Mecademic robot's gripper status.
        LEGACY, use ExtToolStatus and GripperState instead.
 
     Attributes
     ----------
@@ -984,24 +1114,29 @@
         Physical external tool type (same values as mentioned above).
     homing_state : bool
         True if the gripper is homed.
     error_status : bool
         True if the gripper is in error state.
     overload_error : bool
         True if the gripper is in overload error state.
+    comm_err_warning : bool
+        True if some communication errors were detected with the external tool.
+        This could mean that the cable may be damaged and must be replaced,
+        or that the cable may simply not be screwed tight enough on either side.
 """
 
     def __init__(self):
 
         # The following are status fields.
         self.sim_tool_type = MxExtToolType.MX_EXT_TOOL_NONE
         self.physical_tool_type = MxExtToolType.MX_EXT_TOOL_NONE
         self.homing_state = False
         self.error_status = False
         self.overload_error = False
+        self.comm_err_warning = False
 
     def __str__(self) -> str:
         return f"Sim tool type: {self.sim_tool_type}, Physical tool type: {self.physical_tool_type}, " \
                f"homed: {self.homing_state}, error: {self.error_status}, overload: {self.overload_error}"
 
     def __repr__(self) -> str:
         return str(self)
@@ -1065,14 +1200,58 @@
         bool
             True if tool is a pneumatic module, False otherwise
         """
         tool_type = self.physical_tool_type if physical else self.current_tool_type()
         return tool_type in [MxExtToolType.MX_EXT_TOOL_VBOX_2VALVES]
 
 
+class IoStatus:
+    """Class for storing the Mecademic robot's IO modules status.
+
+    Attributes
+    ----------
+    bank_id : int
+        Type of this IO module.
+        1: MxIoBankId.MX_IO_BANK_ID_PSU
+        2: MxIoBankId.MX_IO_BANK_ID_IO_MODULE
+    present : bool
+        True if an IO module of this type is present on the robot.
+    nb_inputs : int
+        Number of digital inputs supported by this IO module.
+    nb_outputs : int
+        Number of digital outputs supported by this IO module.
+    sim_mode : bool
+        True if the IO module is in simulation mode.
+    error : int
+        Error code of the IO module (0 if no error).
+    timestamp : int
+        Monotonic timestamp associated with data (in microseconds since robot last reboot)
+        This timestamp is stamped by the robot so it is not affected by host/network jitter
+"""
+
+    def __init__(self):
+
+        # The following are status fields.
+        self.bank_id = MxIoBankId.MX_IO_BANK_ID_UNDEFINED
+        self.present = False
+        self.nb_inputs = 0
+        self.nb_outputs = 0
+        self.sim_mode = False
+        self.error = 0
+        self.timestamp = 0
+
+    def __str__(self) -> str:
+        return f"BankId: {self.bank_id}, Physically present: {self.present}, " \
+               f"Digital inputs: {self.nb_inputs}, Digital outputs: {self.nb_outputs}, " \
+               f"Simulation mode: {self.sim_mode}, error: {self.error}"
+
+    def __repr__(self) -> str:
+        return str(self)
+
+
 class ValveState:
     """Class for storing the Mecademic robot's pneumatic module valve states.
 
     Attributes
     ----------
     valve_opened : list[int]
         List of valve state: MX_VALVE_STATE_CLOSE or MX_VALVE_STATE_OPENED
```

### Comparing `mecademicpy-1.3.0/mecademicpy/robot_trajectory_files.py` & `mecademicpy-1.4.0/mecademicpy/robot_trajectory_files.py`

 * *Files identical despite different names*

### Comparing `mecademicpy-1.3.0/mecademicpy.egg-info/PKG-INFO` & `mecademicpy-1.4.0/mecademicpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: mecademicpy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A package to control the Mecademic robots through python
 Home-page: https://github.com/Mecademic/mecademicpy
 Author: Mecademic
 Author-email: support@mecademic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.jpg?raw=true  "Mecademic")
+![Mecademic](https://github.com/Mecademic/mecademicpy/blob/main/docs/logo/mecademic_logo.png?raw=true  "Mecademic")
 # Mecademic Python API
 
-A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products. 
+A python module designed for robot products from Mecademic. The module offers tools that give access to the features of the Mecademic Robots such as MoveLin and MoveJoints available through the TCP/IP text interface. The module can be started from a terminal or a python application and controls the Mecademic products.
 
 #### Supported Robots
 
- * Meca500 R2, R3
+ * Meca500, Mcs500
 
 #### Supported Firmware Versions
 
  * 8.3 and up
 
 ## Prerequisites
 
-Please read the [user programming manual](https://mecademic.com/resources/documentation) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
+Please read the [user programming manual](https://www.mecademic.com/support/) to understand concepts necessary for proper usage of the API. This API implements a subset of the commands in the `Communicating over TCP/IP` section. For the exact list of available commands, use the `help()` command as explained in [API Reference](#api-reference).
 
 To be able to use the module without unexpected errors, the user must have a copy of python installed on their machine and it is required to use python version 3.7 or higher. We recommend using Python 3.9 since this is the version on which this module is actively tested. [Python](https://www.python.org/) can be installed from its main website (a reboot will be require after the installation to complete the setup).
 
 The user can validate their python installation by running `python --version` in a terminal.
 
 This library is compatible with Windows, Linux, and Mac.
 
 ## Downloading the package
 
 To download and install the package, the user can easily do so through pip. Pip will download and install the package on your machine and place it in the python local packages directory. This is done by running the following command:
 
 ```
 pip install mecademicpy
-``` 
+```
 
 ## Quick Start
 
 **Ensure the robot is properly connected to the computer, powered on, and in a nominal state.**
 
 In a python shell or script, import the library. Then initialize an instance of the `Robot` class. Finally, use the `Connect` function by passing the IP Address of the robot as an argument to establish a connection:
 
 ```python
 import mecademicpy.robot as mdr
 robot = mdr.Robot()
 robot.Connect(address='192.168.0.100')
 ```
 
 The `Connect` function will raise if connection with robot fails.
-This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode). 
+This function is synchronous (awaits for success or timeout) even when using the `Robot` class in [asynchronous mode](#synchronous-vs.-asynchronous-mode).
 
 Before using the robot, it must be activated and homed. To do so, run the following functions:
 
 ```python
 robot.ActivateRobot()
 robot.Home()
 ```
 
-The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done. 
+The robot should move slightly to perform its homing routine. We can also use `robot.WaitHomed()` or [synchronous mode](#synchronous-vs.-asynchronous-mode) to block execution until homing is done.
 
-Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://mecademic.com/resources/documentation) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot. 
+Once homing is complete, the robot is now ready to perform operations. [The user programming manual](https://www.mecademic.com/support/) or the documentation in the module is sufficient to be able to make the Robot perform actions and control the robot.
 
 Here is an example of a simple motion to perform:
 
 ```python
 robot.MoveJoints(0, 0, 0, 0, 0, 0)
 robot.MoveJoints(0, -60, 60, 0, 0, 0)
 ```
@@ -239,27 +239,27 @@
 robot.ResetError()
 ```
 
 It is recommended to use `GetStatusRobot()` to learn about the current robot status and reset the relevant flags to an appropriate state before resuming operation. For example, an error may require to call `ResumeMotion()`. In this case, verify that `GetStatusRobot().pause_motion_status` is set to `True` before calling `ResumeMotion()`.
 
 The `on_error` callback can also be used to manage robot errors.
 
-Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception. 
+Improper use of the class can also cause exceptions to be raised. For example, calling `MoveJoints()` without any arguments will raise an exception.
 
 If the user is waiting on an event or checkpoint that the `Robot` class later determines will never occur, the event will unblock and raise an exception. For example, if the user is waiting on a checkpoint (`WaitCheckpoint`), but calls `Disconnect()` or `ClearMotion()` before the checkpoint is received, the checkpoint will unblock and raise an exception. Events and checkpoints will also unblock with exception on robot error state.
 
 The user should use python's built-in `try...except` blocks to handle appropriate exceptions.
 
 ### Preserved State on Disconnection
 
-Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot. 
+Once the robot is disconnected, not all states are immediately cleared. Therefore, it is possible to still get the last-known state of the robot.
 
 ### Logging Data to File
 
-It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context. 
+It is possible to continuously log the robot state to a file using the API either using the `StartLogging` and `EndLogging` functions or using the `FileLogger` context.
 
 An example usage of `StartLogging` and `EngLogging`:
 
 ```python
 robot.WaitIdle()
 robot.WaitEndOfCycle()
 robot.StartLogging(0.001)
@@ -288,27 +288,27 @@
     robot.WaitIdle()
 ```
 
 The `FileLogger` context will automatically end logging after either completing the `with` block or encountering an exception.
 
 The user can select which fields to log using the `fields` parameter in `StartLogging` or `FileLogger`. By default, all available fields are logged. The available fields are currently:
 
-- `"TargetJointPos"` 
+- `"TargetJointPos"`
 - `"TargetCartPos"`
 - `"TargetJointVel"`
 - `"TargetCartVel"`
 - `"TargetConf"`
 - `"TargetConfTurn"`
 
 - `"JointPos"`
 - `"CartPos"`
-- `"JointVel"` 
-- `"JointTorq"` 
-- `"CartVel"` 
-- `"Conf"` 
+- `"JointVel"`
+- `"JointTorq"`
+- `"CartVel"`
+- `"Conf"`
 - `"ConfTurn"`
 
 - `"Accel"`
 
 
 These strings should be placed into the list given to the `fields` parameter.
 
@@ -359,11 +359,11 @@
 
 To get support, you can start an issue on the Mecademic github page, issues section or send an email to support@mecademic.com.
 
 ## License
 
 All packages in this repository are licensed under the MIT license.
 
-## Authors 
+## Authors
 
 * **Mecademic** - *Continuous work*
```

### Comparing `mecademicpy-1.3.0/setup.py` & `mecademicpy-1.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='mecademicpy',
-                 version='1.3.0',
+                 version='1.4.0',
                  author='Mecademic',
                  author_email='support@mecademic.com',
                  license='MIT',
                  description='A package to control the Mecademic robots through python',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/Mecademic/mecademicpy',
```

