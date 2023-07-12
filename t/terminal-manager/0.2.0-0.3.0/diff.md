# Comparing `tmp/terminal_manager-0.2.0.tar.gz` & `tmp/terminal_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.2.0.tar", last modified: Fri Jul  7 07:58:48 2023, max compression
+gzip compressed data, was "terminal_manager-0.3.0.tar", last modified: Wed Jul 12 07:26:08 2023, max compression
```

## Comparing `terminal_manager-0.2.0.tar` & `terminal_manager-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.112207 terminal_manager-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 terminal_manager-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      703 2023-07-07 07:58:48.111214 terminal_manager-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-01 07:31:05.000000 terminal_manager-0.2.0/README.md
--rw-rw-rw-   0        0        0      732 2023-07-07 07:55:18.000000 terminal_manager-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 07:58:48.113207 terminal_manager-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.014633 terminal_manager-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.056408 terminal_manager-0.2.0/src/terminal_manager/
--rw-rw-rw-   0        0        0     4314 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/collection.py
--rw-rw-rw-   0        0        0     5232 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/command.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.106224 terminal_manager-0.2.0/src/terminal_manager/default_collections/
--rw-rw-rw-   0        0        0      161 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/const.py
--rw-rw-rw-   0        0        0     3846 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/linux.py
--rw-rw-rw-   0        0        0     4072 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3980 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0       56 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/errors.py
--rw-rw-rw-   0        0        0      645 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/event.py
--rw-rw-rw-   0        0        0      222 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/locker.py
--rw-rw-rw-   0        0        0     8561 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/sensor.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.096214 terminal_manager-0.2.0/src/terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      703 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-07-07 07:58:48.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.3.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.3.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      704 2023-07-12 07:19:59.000000 terminal_manager-0.3.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.242628 terminal_manager-0.3.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.246628 terminal_manager-0.3.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5762 2023-07-12 06:44:51.000000 terminal_manager-0.3.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-12 03:52:34.000000 terminal_manager-0.3.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5085 2023-07-12 03:55:26.000000 terminal_manager-0.3.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-11 09:02:39.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1052 2023-07-12 06:44:13.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4115 2023-07-12 06:45:08.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4390 2023-07-12 06:45:18.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4272 2023-07-12 06:45:28.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-12 03:59:37.000000 terminal_manager-0.3.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-12 04:01:05.000000 terminal_manager-0.3.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-11 09:02:39.000000 terminal_manager-0.3.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8339 2023-07-12 04:08:12.000000 terminal_manager-0.3.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-12 04:05:10.000000 terminal_manager-0.3.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.2.0/LICENSE` & `terminal_manager-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 zhbjsh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 zhbjsh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `terminal_manager-0.2.0/PKG-INFO` & `terminal_manager-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: terminal_manager
-Version: 0.2.0
-Summary: Control and monitor devices with terminal commands
-Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
-Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
-Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Terminal Manager
-
-## Initialize
-
-```python
-from terminal_manager import Manager
-
-manager = Manager()
-```
+Metadata-Version: 2.1
+Name: terminal_manager
+Version: 0.3.0
+Summary: Control and monitor devices with terminal commands
+Author-email: zhbjsh <zhbjsh@outlook.com>
+Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
+Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
+Keywords: terminal,command line
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Terminal Manager
+
+## Initialize
+
+```python
+from terminal_manager import Manager
+
+manager = Manager()
+```
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/__init__.py` & `terminal_manager-0.3.0/src/terminal_manager/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,169 @@
-"""Terminal manager."""
 from __future__ import annotations
 
-from collections.abc import Sequence
-from dataclasses import dataclass
-import logging
-from typing import Any
-
-from .collection import Collection
-from .command import ActionCommand, Command, SensorCommand
-from .default_collections import ActionKey, SensorKey
-from .errors import CommandError
-from .event import Event
-from .locker import Locker
-from .sensor import BinarySensor, NumberSensor, Sensor, TextSensor
-
-_LOGGER = logging.getLogger(__name__)
-
-DEFAULT_NAME = "Manager"
-DEFAULT_COMMAND_TIMEOUT = 15
-
-
-@dataclass(frozen=True)
-class CommandOutput:
-    """The CommandOutput class."""
-
-    timestamp: float
-    stdout: list[str]
-    stderr: list[str]
-    code: int
-
-
-class Manager(Collection, Locker):
-    """The Manager class."""
-
-    def __init__(
-        self,
-        *,
-        name: str = DEFAULT_NAME,
-        command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
-        collection: Collection | None = None,
-        logger: logging.Logger = _LOGGER,
-    ) -> None:
-        Locker.__init__(self)
-        Collection.__init__(self, name)
-        self.command_timeout = command_timeout
-        self.logger = logger
-
-        if collection:
-            self.set_action_commands(collection.action_commands)
-            self.set_sensor_commands(collection.sensor_commands)
+from collections.abc import Callable
+from dataclasses import KW_ONLY, dataclass, field
+from string import Formatter
+from typing import TYPE_CHECKING
 
-    async def async_execute_command_string(
-        self, string: str, command_timeout: int | None = None
-    ) -> CommandOutput:
-        """Execute a command string.
+from .errors import CommandError
+from .helpers import name_to_key
+from .sensor import Sensor
 
-        Raises:
-            CommandError
-        """
-        raise CommandError("Not implemented")
+if TYPE_CHECKING:
+    from . import CommandOutput, Manager
 
-    async def async_execute_command(
-        self, command: Command, variables: dict | None = None
-    ) -> CommandOutput:
-        """Execute a command.
+SENSOR_PLACEHOLDER_KEY = "_"
 
-        Raises:
-            CommandError
-        """
-        await command.async_execute(self, variables)
 
-    async def async_run_action(
-        self, key: str, variables: dict | None = None
-    ) -> CommandOutput:
-        """Run an action.
+@dataclass
+class Command:
+    string: str
+    _: KW_ONLY
+    timeout: float | None = None
+    renderer: Callable[[str], str] | None = None
+
+    @property
+    def field_keys(self) -> list[str]:
+        return {key for _, key, _, _ in Formatter().parse(self.string) if key}
+
+    def _render(self, string: str) -> str:
+        if self.renderer:
+            return self.renderer(string)
+        return string
+
+    def get_variable_keys(self, manager: Manager) -> set[str]:
+        """Get the variable keys."""
+        return {key for key in self.field_keys if key not in manager.sensors_by_key}
+
+    def get_sensor_keys(self, manager: Manager) -> set[str]:
+        """Get the sensor keys."""
+        return {key for key in self.field_keys if key in manager.sensors_by_key}
+
+    async def async_format(
+        self, manager: Manager, variables: dict | None = None
+    ) -> str:
+        """Format the string.
 
         Raises:
             CommandError
         """
-        command = self.get_action_command(key)
-        return await self.async_execute_command(command, variables)
+        variables = {**variables} if variables else {}
+        missing_sensor_keys = set()
 
-    async def async_poll_sensor(
-        self, key: str, *, raise_errors: bool = False
-    ) -> Sensor:
-        """Poll a sensor.
+        for key in self.get_variable_keys(manager):
+            if key not in variables:
+                raise CommandError(f"Variable {key} is missing")
+
+        for key in self.get_sensor_keys(manager):
+            if key not in variables:
+                sensor = manager.get_sensor(key)
+                if sensor.value is not None:
+                    variables[sensor.key] = sensor.value
+                else:
+                    missing_sensor_keys.add(sensor.key)
+
+        for sensor in await manager.async_poll_sensors(missing_sensor_keys):
+            if sensor.value is not None:
+                variables[sensor.key] = sensor.value
+            else:
+                raise CommandError(f"Value of sensor {sensor.key} is None")
+
+        try:
+            return self._render(self.string.format(**variables))
+        except Exception as exc:
+            raise CommandError("Failed to generate string ({exc})") from exc
 
-        Raises:
-            CommandError (`raise_errors`)
-        """
-        sensors = await self.async_poll_sensors([key], raise_errors=raise_errors)
-        return sensors[0]
-
-    async def async_poll_sensors(
-        self, keys: Sequence[str], *, raise_errors: bool = False
-    ) -> list[Sensor]:
-        """Poll multiple sensors.
+    async def async_execute(
+        self, manager: Manager, variables: dict | None = None
+    ) -> CommandOutput:
+        """Execute.
 
         Raises:
-            CommandError (`raise_errors`)
+            CommandError
         """
-        sensors = [self.get_sensor(key) for key in keys]
-        commands = [self.get_sensor_command(key) for key in set(keys)]
+        try:
+            string = await self.async_format(manager, variables)
+        except CommandError as exc:
+            manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
+            raise
+
+        try:
+            output = await manager.async_execute_command_string(string, self.timeout)
+        except CommandError as exc:
+            manager.logger.debug("%s: %s => %s", manager.name, string, exc)
+            raise
+
+        manager.logger.debug(
+            "%s: %s => %s, %s, %s",
+            manager.name,
+            string,
+            output.stdout,
+            output.stderr,
+            output.code,
+        )
 
-        for command in commands:
-            try:
-                await self.async_execute_command(command)
-            except CommandError:
-                if raise_errors:
-                    raise
-
-        return sensors
-
-    async def async_set_sensor_value(
-        self, key: str, value: Any, *, raise_errors: bool = False
-    ) -> Sensor:
-        """Set the value of a sensor.
+        return output
 
-        Raises:
-            TypeError (`raise_errors`)
-            ValueError (`raise_errors`)
-            CommandError (`raise_errors`)
-        """
-        sensors = await self.async_set_sensor_values(
-            [key], [value], raise_errors=raise_errors
-        )
-        return sensors[0]
 
-    async def async_set_sensor_values(
-        self, keys: Sequence[str], values: Sequence[Any], *, raise_errors: bool = False
-    ) -> list[Sensor]:
-        """Set the value of multiple sensors.
+@dataclass
+class ActionCommand(Command):
+    name: str | None = None
+    key: str | None = None
+    _: KW_ONLY
+    attributes: dict = field(default_factory=dict)
+
+    def __post_init__(self):
+        self.key = self.key or name_to_key(self.name)
+
+
+@dataclass
+class SensorCommand(Command):
+    _: KW_ONLY
+    interval: int | None = None
+    sensors: list[Sensor] = field(default_factory=list)
+
+    def __post_init__(self):
+        self.last_update: float | None = None
+
+    @property
+    def sensors_by_key(self) -> dict[str, Sensor]:
+        return {
+            sensor.key: sensor
+            for command_sensor in self.sensors
+            for sensor in (command_sensor, *command_sensor.child_sensors)
+            if command_sensor.key != SENSOR_PLACEHOLDER_KEY
+        }
+
+    def remove_sensor(self, key: str) -> None:
+        """Remove a sensor."""
+        self.sensors = [
+            Sensor(key=SENSOR_PLACEHOLDER_KEY) if sensor.key == key else sensor
+            for sensor in self.sensors
+        ]
+
+    def update_sensors(self, manager: Manager, output: CommandOutput | None) -> None:
+        """Update the sensors."""
+        if output and output.code == 0:
+            self.last_update = output.timestamp
+            data = output.stdout
+        else:
+            data = []
+
+        for i, sensor in enumerate(self.sensors):
+            if sensor.dynamic:
+                sensor.update(manager, data[i:] or None)
+                return
+            sensor.update(manager, data[i] if len(data) > i else None)
 
-        Raises:
-            TypeError (`raise_errors`)
-            ValueError (`raise_errors`)
-            CommandError (`raise_errors`)
-        """
-        sensors = await self.async_poll_sensors(keys, raise_errors=raise_errors)
+    async def async_execute(
+        self, manager: Manager, variables: dict | None = None
+    ) -> CommandOutput:
+        try:
+            output = await super().async_execute(manager, variables)
+        except CommandError:
+            self.update_sensors(manager, None)
+            raise
 
-        for i, sensor in enumerate(sensors):
-            if sensor.value is None:
-                continue
-            try:
-                await sensor.async_set(self, values[i])
-            except (TypeError, ValueError, CommandError):
-                if raise_errors:
-                    raise
+        self.update_sensors(manager, output)
 
-        return await self.async_poll_sensors(keys, raise_errors=raise_errors)
+        return output
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/collection.py` & `terminal_manager-0.3.0/src/terminal_manager/collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from copy import deepcopy
 
 from .command import ActionCommand, SensorCommand
 from .sensor import Sensor
 
 
 class Collection:
-    """The Collection class."""
-
     action_commands: list[ActionCommand]
     sensor_commands: list[SensorCommand]
 
     def __init__(
         self,
         name: str,
         action_commands: list[ActionCommand] | None = None,
@@ -18,43 +16,40 @@
     ) -> None:
         self.name = name
         self.set_action_commands(action_commands or [])
         self.set_sensor_commands(sensor_commands or [])
 
     @property
     def action_commands_by_key(self) -> dict[str, ActionCommand]:
-        """Action commands by key."""
         return {command.key: command for command in self.action_commands}
 
     @property
     def sensor_commands_by_sensor_key(self) -> dict[str, SensorCommand]:
-        """Sensor commands by sensor key."""
         return {
             key: command
             for command in self.sensor_commands
             for key in command.sensors_by_key
         }
 
     @property
     def sensors_by_key(self) -> dict[str, Sensor]:
-        """Sensors by key."""
         return {
             key: sensor
             for command in self.sensor_commands
             for key, sensor in command.sensors_by_key.items()
         }
 
     def set_action_commands(self, action_commands: list[ActionCommand]) -> None:
-        """Set action commands."""
+        """Set the action commands."""
         self.action_commands = []
         for command in action_commands:
             self.add_action_command(command)
 
     def set_sensor_commands(self, sensor_commands: list[SensorCommand]) -> None:
-        """Set sensor commands."""
+        """Set the sensor commands."""
         self.sensor_commands = []
         for command in sensor_commands:
             self.add_sensor_command(command)
 
     def add_action_command(self, command: ActionCommand) -> None:
         """Add an action command.
 
@@ -92,14 +87,14 @@
         """Remove an action command."""
         command = self.get_action_command(key)
         self.action_commands.remove(command)
 
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor.
 
-        Remove the sensor command as well if it doesnt have any other sensors.
+        Remove the sensor command if it doesnt have any other sensors.
         """
         command = self.get_sensor_command(key)
         command.remove_sensor(key)
 
         if not command.sensors_by_key:
             self.sensor_commands.remove(command)
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/command.py` & `terminal_manager-0.3.0/src/terminal_manager/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,188 @@
+"""Terminal manager."""
 from __future__ import annotations
 
-from collections.abc import Callable
-from dataclasses import KW_ONLY, dataclass, field
-from string import Formatter
-from typing import TYPE_CHECKING
-
+import logging
+from collections.abc import Sequence
+from dataclasses import dataclass
+from typing import Any
+
+from .collection import Collection
+from .command import ActionCommand, Command, SensorCommand
+from .default_collections import ActionKey, SensorKey
 from .errors import CommandError
-from .helpers import name_to_key
-from .sensor import Sensor
+from .event import Event
+from .sensor import BinarySensor, NumberSensor, Sensor, TextSensor
+from .synchronizer import Synchronizer
+
+_LOGGER = logging.getLogger(__name__)
+
+DEFAULT_NAME = "Manager"
+DEFAULT_COMMAND_TIMEOUT = 15
+
+
+@dataclass(frozen=True)
+class CommandOutput:
+    timestamp: float
+    stdout: list[str]
+    stderr: list[str]
+    code: int
+
+
+class Manager(Collection, Synchronizer):
+    def __init__(
+        self,
+        *,
+        name: str = DEFAULT_NAME,
+        command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
+        collection: Collection | None = None,
+        logger: logging.Logger = _LOGGER,
+    ) -> None:
+        Synchronizer.__init__(self)
+        Collection.__init__(
+            self,
+            name,
+            collection.action_commands if collection else None,
+            collection.sensor_commands if collection else None,
+        )
+        self.command_timeout = command_timeout
+        self.logger = logger
 
-if TYPE_CHECKING:
-    from . import CommandOutput, Manager
+    @property
+    def hostname(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.HOSTNAME):
+            return sensor.last_known_value
 
-SENSOR_PLACEHOLDER_KEY = "_"
+    @property
+    def os_name(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.OS_NAME):
+            return sensor.last_known_value
 
+    @property
+    def os_version(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.OS_VERSION):
+            return sensor.last_known_value
 
-@dataclass
-class Command:
-    """The Command class."""
+    @property
+    def os_architecture(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.OS_ARCHITECTURE):
+            return sensor.last_known_value
 
-    string: str
-    _: KW_ONLY
-    timeout: float | None = None
-    renderer: Callable[[str], str] | None = None
+    @property
+    def machine_type(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.MACHINE_TYPE):
+            return sensor.last_known_value
 
     @property
-    def field_keys(self) -> list[str]:
-        """Field keys."""
-        return {key for _, key, _, _ in Formatter().parse(self.string) if key}
+    def interface(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.INTERFACE):
+            return sensor.last_known_value
 
-    def _render(self, string: str) -> str:
-        if self.renderer:
-            return self.renderer(string)
+    @property
+    def mac_address(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.MAC_ADDRESS):
+            return sensor.last_known_value
 
-        return string
+    @property
+    def wake_on_lan(self) -> bool | None:
+        if sensor := self.sensors_by_key.get(SensorKey.WAKE_ON_LAN):
+            return sensor.last_known_value
 
-    def get_variable_keys(self, manager: Manager) -> set[str]:
-        """Get variable keys."""
-        return {key for key in self.field_keys if key not in manager.sensors_by_key}
+    async def async_execute_command_string(
+        self, string: str, command_timeout: int | None = None
+    ) -> CommandOutput:
+        """Execute a command string.
 
-    def get_sensor_keys(self, manager: Manager) -> set[str]:
-        """Get sensor keys."""
-        return {key for key in self.field_keys if key in manager.sensors_by_key}
+        Raises:
+            CommandError
+        """
+        raise CommandError("Not implemented")
 
-    async def async_format(
-        self, manager: Manager, variables: dict | None = None
-    ) -> str:
-        """Format the string.
+    async def async_execute_command(
+        self, command: Command, variables: dict | None = None
+    ) -> CommandOutput:
+        """Execute a command.
 
         Raises:
             CommandError
         """
-        variables = {**variables} if variables else {}
-        missing_sensor_keys = set()
-
-        for key in self.get_variable_keys(manager):
-            if key not in variables:
-                raise CommandError(f"Variable {key} is missing")
-
-        for key in self.get_sensor_keys(manager):
-            if key not in variables:
-                sensor = manager.get_sensor(key)
-                if sensor.value is not None:
-                    variables[sensor.key] = sensor.value
-                else:
-                    missing_sensor_keys.add(sensor.key)
-
-        for sensor in await manager.async_poll_sensors(missing_sensor_keys):
-            if sensor.value is not None:
-                variables[sensor.key] = sensor.value
-            else:
-                raise CommandError(f"Value of sensor {sensor.key} is None")
-
-        try:
-            return self._render(self.string.format(**variables))
-        except Exception as exc:
-            raise CommandError("Failed to generate string ({exc})") from exc
+        await command.async_execute(self, variables)
 
-    async def async_execute(
-        self, manager: Manager, variables: dict | None = None
+    async def async_run_action(
+        self, key: str, variables: dict | None = None
     ) -> CommandOutput:
-        """Execute.
+        """Run an action.
 
         Raises:
             CommandError
         """
-        try:
-            string = await self.async_format(manager, variables)
-        except CommandError as exc:
-            manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
-            raise
-
-        try:
-            output = await manager.async_execute_command_string(string, self.timeout)
-        except CommandError as exc:
-            manager.logger.debug("%s: %s => %s", manager.name, string, exc)
-            raise
-
-        manager.logger.debug(
-            "%s: %s => %s, %s, %s",
-            manager.name,
-            string,
-            output.stdout,
-            output.stderr,
-            output.code,
-        )
+        command = self.get_action_command(key)
+        return await self.async_execute_command(command, variables)
 
-        return output
+    async def async_poll_sensor(
+        self, key: str, *, raise_errors: bool = False
+    ) -> Sensor:
+        """Poll a sensor.
 
+        Raises:
+            CommandError (only with `raise_errors=True`)
+        """
+        sensors = await self.async_poll_sensors([key], raise_errors=raise_errors)
+        return sensors[0]
 
-@dataclass
-class ActionCommand(Command):
-    """The ActionCommand class."""
-
-    name: str | None = None
-    key: str | None = None
-    _: KW_ONLY
-    attributes: dict = field(default_factory=dict)
-
-    def __post_init__(self):
-        self.key = self.key or name_to_key(self.name)
-
-
-@dataclass
-class SensorCommand(Command):
-    """The SensorCommand class."""
-
-    _: KW_ONLY
-    interval: int | None = None
-    sensors: list[Sensor] = field(default_factory=list)
-
-    def __post_init__(self):
-        self.last_update: float | None = None
-
-    @property
-    def sensors_by_key(self) -> dict[str, Sensor]:
-        """Sensors by key."""
-        return {
-            sensor.key: sensor
-            for command_sensor in self.sensors
-            for sensor in (command_sensor, *command_sensor.child_sensors)
-            if command_sensor.key != SENSOR_PLACEHOLDER_KEY
-        }
-
-    def remove_sensor(self, key: str) -> None:
-        """Remove a sensor."""
-        self.sensors = [
-            Sensor(key=SENSOR_PLACEHOLDER_KEY) if sensor.key == key else sensor
-            for sensor in self.sensors
-        ]
-
-    def update_sensors(self, manager: Manager, output: CommandOutput | None) -> None:
-        """Update sensors."""
-        if output and output.code == 0:
-            self.last_update = output.timestamp
-            data = output.stdout
-        else:
-            data = []
-
-        for i, sensor in enumerate(self.sensors):
-            if sensor.dynamic:
-                sensor.update(manager, data[i:] or None)
-                return
-            sensor.update(manager, data[i] if len(data) > i else None)
+    async def async_poll_sensors(
+        self, keys: Sequence[str], *, raise_errors: bool = False
+    ) -> list[Sensor]:
+        """Poll multiple sensors.
 
-    async def async_execute(
-        self, manager: Manager, variables: dict | None = None
-    ) -> CommandOutput:
-        try:
-            output = await super().async_execute(manager, variables)
-        except CommandError:
-            self.update_sensors(manager, None)
-            raise
+        Raises:
+            CommandError (only with `raise_errors=True`)
+        """
+        sensors = [self.get_sensor(key) for key in keys]
+        commands = [self.get_sensor_command(key) for key in set(keys)]
+
+        for command in commands:
+            try:
+                await self.async_execute_command(command)
+            except CommandError:
+                if raise_errors:
+                    raise
+
+        return sensors
+
+    async def async_set_sensor_value(
+        self, key: str, value: Any, *, raise_errors: bool = False
+    ) -> Sensor:
+        """Set the value of a controllable sensor.
+
+        Raises:
+            TypeError (only with `raise_errors=True`)
+            ValueError (only with `raise_errors=True`)
+            CommandError (only with `raise_errors=True`)
+        """
+        sensors = await self.async_set_sensor_values(
+            [key], [value], raise_errors=raise_errors
+        )
+        return sensors[0]
+
+    async def async_set_sensor_values(
+        self, keys: Sequence[str], values: Sequence[Any], *, raise_errors: bool = False
+    ) -> list[Sensor]:
+        """Set the value of multiple controllable sensors.
+
+        Raises:
+            TypeError (only with `raise_errors=True`)
+            ValueError (only with `raise_errors=True`)
+            CommandError (only with `raise_errors=True`)
+        """
+        sensors = await self.async_poll_sensors(keys, raise_errors=raise_errors)
 
-        self.update_sensors(manager, output)
+        for i, sensor in enumerate(sensors):
+            if sensor.value is None:
+                continue
+            try:
+                await sensor.async_set(self, values[i])
+            except (TypeError, ValueError, CommandError):
+                if raise_errors:
+                    raise
 
-        return output
+        return await self.async_poll_sensors(keys, raise_errors=raise_errors)
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.3.0/src/terminal_manager/default_collections/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,34 +7,36 @@
     TURN_OFF = "Turn off"
     RESTART = "Restart"
 
 
 class SensorKey:
     INTERFACE = "interface"
     MAC_ADDRESS = "mac_address"
-    WOL_SUPPORT = "wol_support"
+    WAKE_ON_LAN = "wake_on_lan"
     MACHINE_TYPE = "machine_type"
     HOSTNAME = "hostname"
     OS_NAME = "os_name"
     OS_VERSION = "os_version"
     OS_ARCHITECTURE = "os_architecture"
     TOTAL_MEMORY = "total_memory"
     FREE_MEMORY = "free_memory"
     CPU_LOAD = "cpu_load"
     FREE_DISK_SPACE = "free_disk_space"
     TEMPERATURE = "temperature"
+    PROCESSES = "processes"
 
 
 class SensorName:
     INTERFACE = "Interface"
     MAC_ADDRESS = "MAC Address"
-    WOL_SUPPORT = "Wake on LAN Support"
+    WAKE_ON_LAN = "Wake on LAN"
     MACHINE_TYPE = "Machine Type"
     HOSTNAME = "Hostname"
     OS_NAME = "OS Name"
     OS_VERSION = "OS Version"
     OS_ARCHITECTURE = "OS Architecture"
     TOTAL_MEMORY = "Total Memory"
     FREE_MEMORY = "Free Memory"
     CPU_LOAD = "CPU Load"
     FREE_DISK_SPACE = "Free Disk Space"
     TEMPERATURE = "Temperature"
+    PROCESSES = "Processes"
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.3.0/src/terminal_manager/default_collections/linux.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             ],
         ),
         SensorCommand(
             "file=/sys/class/net/{interface}/device/power/wakeup; "
             + "[[ ! -f $file ]] || cat $file",
             sensors=[
                 BinarySensor(
-                    SensorName.WOL_SUPPORT,
-                    SensorKey.WOL_SUPPORT,
+                    SensorName.WAKE_ON_LAN,
+                    SensorKey.WAKE_ON_LAN,
                     payload_on="enabled",
                 )
             ],
         ),
         SensorCommand(
             "/sbin/route -n | awk '/^0.0.0.0/ {{print $NF}}'",
             sensors=[
@@ -122,9 +122,19 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                     float=True,
                 )
             ],
         ),
+        SensorCommand(
+            "ps -e --no-headers | wc -l",
+            interval=60,
+            sensors=[
+                NumberSensor(
+                    SensorName.PROCESSES,
+                    SensorKey.PROCESSES,
+                )
+            ],
+        ),
     ],
 )
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "shutdown -r -t 0",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         # TODO: MAC_ADDRESS
-        # TODO: WOL_SUPPORT
+        # TODO: WAKE_ON_LAN
         # TODO: INTERFACE
         SensorCommand(
             "for /f \"skip=1 tokens=*\" %i in ('wmic ComputerSystem get SystemType') "
             + "do @echo %i",
             sensors=[
                 TextSensor(
                     SensorName.MACHINE_TYPE,
@@ -126,9 +126,19 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                     float=True,
                 )
             ],
         ),
+        SensorCommand(
+            'wmic process get processId | findstr /r "\\<[0-9][0-9]*\\>" | find /c /v ""',
+            interval=60,
+            sensors=[
+                NumberSensor(
+                    SensorName.PROCESSES,
+                    SensorKey.PROCESSES,
+                )
+            ],
+        ),
     ],
 )
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "Restart-Computer -Force",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         # TODO: MAC_ADDRESS
-        # TODO: WOL_SUPPORT
+        # TODO: WAKE_ON_LAN
         # TODO: INTERFACE
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
             + "Select Name, SystemType;"
             + "$x.Name;"
             + "$x.SystemType;",
             sensors=[
@@ -122,9 +122,19 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                     float=True,
                 )
             ],
         ),
+        SensorCommand(
+            "Get-Process | Measure | ForEach-Object {$_.Count}",
+            interval=60,
+            sensors=[
+                NumberSensor(
+                    SensorName.PROCESSES,
+                    SensorKey.PROCESSES,
+                )
+            ],
+        ),
     ],
 )
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/event.py` & `terminal_manager-0.3.0/src/terminal_manager/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from collections.abc import Callable
 
 
 class Event:
-    """The Event class."""
-
     def __init__(self) -> None:
         self._subscribers: list[Callable] = []
 
     def subscribe(self, subscriber) -> Callable:
         """Subscribe."""
         self._subscribers.append(subscriber)
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/locker.py` & `terminal_manager-0.3.0/src/terminal_manager/synchronizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from __future__ import annotations
 
 import asyncio
+import inspect
 from collections.abc import Coroutine
 from functools import wraps
-import inspect
 
 
 def locked(coro: Coroutine):
-    """The locked decorator."""
-
     @wraps(coro)
-    async def wrapper(instance: Locker, *args, **kwargs):
-        async with instance.lock:
-            return await coro(instance, *args, **kwargs)
+    async def wrapper(obj: Synchronizer, *args, **kwargs):
+        async with obj.lock:
+            return await coro(obj, *args, **kwargs)
 
     return wrapper
 
 
 class AsyncRLock(asyncio.Lock):
-    """The AsyncRLock class."""
-
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._task = None
         self._depth = 0
 
     async def acquire(self) -> None:
         if self._task is None or self._task != asyncio.current_task():
@@ -36,17 +32,15 @@
         if self._depth > 0:
             self._depth -= 1
         if self._depth == 0:
             super().release()
             self._task = None
 
 
-class Locker:
-    """The Locker class."""
-
+class Synchronizer:
     def __init__(self) -> None:
         self.lock = AsyncRLock()
 
     def __init_subclass__(cls, **kwargs):
         for name in cls.__dict__:
             attr = getattr(cls, name)
             if inspect.iscoroutinefunction(attr):
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager/sensor.py` & `terminal_manager-0.3.0/src/terminal_manager/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
+import re
 from collections.abc import Callable
 from copy import deepcopy
 from dataclasses import KW_ONLY, dataclass, field
-import re
 from typing import TYPE_CHECKING, Any
 
 from .event import Event
 from .helpers import name_to_key
 
 if TYPE_CHECKING:
     from . import Manager
@@ -15,16 +15,14 @@
 
 TRUE_STRINGS = ["true", "enabled", "on", "active", "1"]
 FALSE_STRINGS = ["false", "disabled", "off", "inactive", "0"]
 
 
 @dataclass
 class Sensor:
-    """The Sensor class."""
-
     name: str | None = None
     key: str | None = None
     _: KW_ONLY
     dynamic: bool = False
     separator: str | None = None
     unit: str | None = None
     renderer: Callable[[str], str] | None = None
@@ -39,20 +37,18 @@
         self.child_sensors: list[Sensor] = []
         self.on_update = Event()
         self.on_child_added = Event()
         self.on_child_removed = Event()
 
     @property
     def controllable(self) -> bool:
-        """Controllable."""
         return self.command_set is not None
 
     @property
     def child_sensors_by_key(self) -> dict[str, Sensor]:
-        """Child sensors by key."""
         return {child.key: child for child in self.child_sensors}
 
     def _get_control_command(self, _: Any) -> Command | None:
         return self.command_set
 
     def _add_child(self, child: Sensor) -> None:
         self.child_sensors.append(child)
@@ -132,15 +128,15 @@
         else:
             self.child_sensors = []
             self._update_value(manager, data)
 
         self.on_update.notify(self)
 
     async def async_set(self, manager: Manager, value: Any) -> None:
-        """Set.
+        """Set a value.
 
         Raises:
             TypeError
             ValueError
             CommandError
         """
         self._validate(value)
@@ -152,16 +148,14 @@
         await manager.async_execute_command(
             command, variables={"id": self.id, "value": value}
         )
 
 
 @dataclass
 class TextSensor(Sensor):
-    """The TextSensor class."""
-
     _: KW_ONLY
     minimum: int | None = None
     maximum: int | None = None
     pattern: str | None = None
     options: list[Any] | None = None
 
     def _validate(self, value: Any) -> None:
@@ -179,16 +173,14 @@
 
         if self.options and value not in self.options:
             raise ValueError(f"{value} is not in {self.options}")
 
 
 @dataclass
 class NumberSensor(Sensor):
-    """The NumberSensor class."""
-
     _: KW_ONLY
     float: bool = False
     minimum: int | float | None = None
     maximum: int | float | None = None
 
     def _convert(self, value_string: str) -> int | float:
         if self.float:
@@ -208,16 +200,14 @@
 
         if self.maximum and value > self.maximum:
             raise ValueError(f"{value} is bigger then {self.maximum}")
 
 
 @dataclass
 class BinarySensor(Sensor):
-    """The BinarySensor class."""
-
     _: KW_ONLY
     command_on: Command | None = None
     command_off: Command | None = None
     payload_on: str | None = None
     payload_off: str | None = None
 
     @property
@@ -259,16 +249,14 @@
 
     def _validate(self, value: Any) -> None:
         if not isinstance(value, bool):
             raise TypeError(f"{value} is {type(value)} and not {bool}")
 
 
 class DynamicData:
-    """The DynamicData class."""
-
     def __init__(
         self,
         parent_name: str | None,
         parent_key: str,
         id_field: str,
         data_field: str,
         name_field: str | None = None,
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.3.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: terminal-manager
-Version: 0.2.0
-Summary: Control and monitor devices with terminal commands
-Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
-Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
-Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Terminal Manager
-
-## Initialize
-
-```python
-from terminal_manager import Manager
-
-manager = Manager()
-```
+Metadata-Version: 2.1
+Name: terminal-manager
+Version: 0.3.0
+Summary: Control and monitor devices with terminal commands
+Author-email: zhbjsh <zhbjsh@outlook.com>
+Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
+Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
+Keywords: terminal,command line
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Terminal Manager
+
+## Initialize
+
+```python
+from terminal_manager import Manager
+
+manager = Manager()
+```
```

### Comparing `terminal_manager-0.2.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.3.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pyproject.toml
 src/terminal_manager/__init__.py
 src/terminal_manager/collection.py
 src/terminal_manager/command.py
 src/terminal_manager/errors.py
 src/terminal_manager/event.py
 src/terminal_manager/helpers.py
-src/terminal_manager/locker.py
 src/terminal_manager/sensor.py
+src/terminal_manager/synchronizer.py
 src/terminal_manager.egg-info/PKG-INFO
 src/terminal_manager.egg-info/SOURCES.txt
 src/terminal_manager.egg-info/dependency_links.txt
 src/terminal_manager.egg-info/requires.txt
 src/terminal_manager.egg-info/top_level.txt
 src/terminal_manager/default_collections/__init__.py
 src/terminal_manager/default_collections/const.py
```

