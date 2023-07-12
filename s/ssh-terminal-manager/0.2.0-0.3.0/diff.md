# Comparing `tmp/ssh_terminal_manager-0.2.0.tar.gz` & `tmp/ssh_terminal_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.2.0.tar", last modified: Fri Jul  7 08:15:04 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.3.0.tar", last modified: Wed Jul 12 07:53:03 2023, max compression
```

## Comparing `ssh_terminal_manager-0.2.0.tar` & `ssh_terminal_manager-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.632968 ssh_terminal_manager-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      841 2023-07-07 08:15:04.631968 ssh_terminal_manager-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.2.0/README.md
--rw-rw-rw-   0        0        0      859 2023-07-07 08:02:41.000000 ssh_terminal_manager-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 08:15:04.632968 ssh_terminal_manager-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.565963 ssh_terminal_manager-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.590971 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/
--rw-rw-rw-   0        0        0     9844 2023-07-07 07:51:11.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/__init__.py
--rw-rw-rw-   0        0        0      347 2023-07-07 07:51:11.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.629967 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      841 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.3.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.3.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      797 2023-07-12 07:27:33.000000 ssh_terminal_manager-0.3.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9137 2023-07-12 06:56:45.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-12 03:59:09.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.2.0/LICENSE` & `ssh_terminal_manager-0.3.0/LICENSE`

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

### Comparing `ssh_terminal_manager-0.2.0/PKG-INFO` & `ssh_terminal_manager-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: ssh_terminal_manager
-Version: 0.2.0
-Summary: Control and monitor devices with SSH terminal commands
-Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
-Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
-Keywords: ssh,terminal,command line
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# SSH Terminal Manager
-
-## Initialize
-
-```python
-from ssh_terminal_manager import SSHManager
-
-manager = SSHManager("192.168.0.123", username="user", password="1234")
-
-await manager.async_update_state(raise_errors=True)
-```
+Metadata-Version: 2.1
+Name: ssh_terminal_manager
+Version: 0.3.0
+Summary: Control and monitor devices with SSH terminal commands
+Author-email: zhbjsh <zhbjsh@outlook.com>
+Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
+Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
+Keywords: ssh,terminal,command line
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SSH Terminal Manager
+
+## Initialize
+
+```python
+from ssh_terminal_manager import SSHManager
+
+manager = SSHManager("192.168.0.123", username="user", password="1234")
+
+await manager.async_update_state(raise_errors=True)
+```
```

### Comparing `ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import asyncio
 import logging
 from time import time
 
 import icmplib
 import paramiko
+import wakeonlan
 from terminal_manager import (
     DEFAULT_COMMAND_TIMEOUT,
     ActionCommand,
     BinarySensor,
     Collection,
     Command,
     CommandError,
@@ -20,15 +21,14 @@
     NumberSensor,
     Sensor,
     SensorCommand,
     TextSensor,
     default_collections,
 )
 from terminal_manager.default_collections import ActionKey, SensorKey
-import wakeonlan
 
 from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("echo ''")
 
 DEFAULT_PORT = 22
@@ -38,135 +38,96 @@
 DEFAULT_ALLOW_TURN_OFF = False
 
 ONLINE = "online"
 CONNECTED = "connected"
 
 
 class CustomRejectPolicy(paramiko.MissingHostKeyPolicy):
-    """Custom reject policy for ssh client."""
-
     def missing_host_key(
         self, client: paramiko.SSHClient, hostname: str, key: paramiko.PKey
     ) -> None:
         raise SSHHostKeyUnknownError("Host key is unknown")
 
 
 class State:
-    """The State class."""
-
     online: bool = False
     connected: bool = False
 
     def __init__(self, manager: SSHManager) -> None:
         self._manager = manager
         self.on_change = Event()
 
     def update(self, name, value) -> None:
-        """Update."""
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
         self._manager.logger.debug("%s: %s is %s", self._manager.name, name, value)
         self.on_change.notify(self)
 
 
 class SSHManager(Manager):
-    """The SSHManager class."""
-
     def __init__(
         self,
         host: str,
         *,
         name: str | None = None,
         mac_address: str | None = None,
-        add_host_keys: bool = DEFAULT_ADD_HOST_KEYS,
         port: int = DEFAULT_PORT,
         username: str | None = None,
         password: str | None = None,
         key_filename: str | None = None,
         host_keys_filename: str | None = None,
+        add_host_keys: bool = DEFAULT_ADD_HOST_KEYS,
+        allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
         ssh_timeout: int = DEFAULT_SSH_TIMEOUT,
         ping_timeout: int = DEFAULT_PING_TIMEOUT,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
         collection: Collection | None = None,
-        allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         super().__init__(
             name=name or host,
             command_timeout=command_timeout,
             collection=collection,
             logger=logger,
         )
         self.host = host
-        self._mac_address = mac_address
         self.port = port
         self.username = username
         self.password = password
         self.key_filename = key_filename
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
         self.allow_turn_off = allow_turn_off
+        self._mac_address = mac_address
         self.state = State(self)
-        self._client = paramiko.SSHClient()
-        self._client.load_system_host_keys()
-        self._client.set_missing_host_key_policy(
+        self.client = paramiko.SSHClient()
+        self.client.load_system_host_keys()
+        self.client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
 
         if host_keys_filename:
             with open(host_keys_filename, "a", encoding="utf-8"):
                 pass
-            self._client.load_host_keys(host_keys_filename)
-
-    @property
-    def hostname(self) -> str | None:
-        """Hostname."""
-        if sensor := self.sensors_by_key.get(SensorKey.HOSTNAME):
-            return sensor.last_known_value
+            self.client.load_host_keys(host_keys_filename)
 
     @property
     def mac_address(self) -> str | None:
-        """MAC address."""
         if self._mac_address:
             return self._mac_address
-        if sensor := self.sensors_by_key.get(SensorKey.MAC_ADDRESS):
-            return sensor.last_known_value
-
-    @property
-    def wol_support(self) -> bool | None:
-        """Wake on LAN support."""
-        if sensor := self.sensors_by_key.get(SensorKey.WOL_SUPPORT):
-            return sensor.last_known_value
-
-    @property
-    def os_name(self) -> str | None:
-        """OS name."""
-        if sensor := self.sensors_by_key.get(SensorKey.OS_NAME):
-            return sensor.last_known_value
-
-    @property
-    def os_version(self) -> str | None:
-        """OS version."""
-        if sensor := self.sensors_by_key.get(SensorKey.OS_VERSION):
-            return sensor.last_known_value
-
-    @property
-    def machine_type(self) -> str | None:
-        """Machine type."""
-        if sensor := self.sensors_by_key.get(SensorKey.MACHINE_TYPE):
-            return sensor.last_known_value
+        return super().mac_address
 
     def _execute_command_string(self, string: str, timeout: int) -> CommandOutput:
         if not self.state.connected:
             raise CommandError("Not connected")
 
         try:
-            stdin, stdout, stderr = self._client.exec_command(
+            stdin, stdout, stderr = self.client.exec_command(
                 string,
                 timeout=float(timeout),
             )
         except Exception as exc:
             self._disconnect()
             raise CommandError("Disconnected before execution") from exc
 
@@ -185,21 +146,21 @@
             raise CommandError("Disconnected during execution") from exc
 
     def _connect(self) -> None:
         if self.state.connected:
             return
 
         try:
-            self._client.connect(
+            self.client.connect(
                 self.host,
                 self.port,
                 self.username,
                 self.password,
                 key_filename=self.key_filename,
-                timeout=self.ssh_timeout,  # timeout for the TCP connect
+                timeout=self.ssh_timeout,  # TCP connect timeout
                 allow_agent=False,
             )
         except SSHHostKeyUnknownError:
             self._disconnect()
             raise
         except paramiko.AuthenticationException as exc:
             self._disconnect()
@@ -210,15 +171,15 @@
 
         self.state.update(CONNECTED, True)
 
     def _disconnect(self) -> None:
         if not self.state.connected:
             return
 
-        self._client.close()
+        self.client.close()
         self.state.update(CONNECTED, False)
 
         for command in self.sensor_commands:
             command.update_sensors(self, None)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
@@ -226,19 +187,18 @@
         loop = asyncio.get_running_loop()
         timeout = command_timeout or self.command_timeout
         return await loop.run_in_executor(
             None, self._execute_command_string, string, timeout
         )
 
     async def async_connect(self) -> None:
-        """Connect the SSH client.
+        """Connect to the SSH server.
 
-        Set `state.connected` to `True` and update all
-        sensor commands if successful, otherwise disconnect
-        and raise an error.
+        Set `state.connected` to `True` and update all sensor
+        commands if successful, otherwise raise an error.
 
         Raises:
             SSHHostKeyUnknownError
             SSHAuthError
             SSHConnectError
         """
         loop = asyncio.get_running_loop()
@@ -249,28 +209,28 @@
                 await self.async_execute_command(command)
             except CommandError:
                 pass
 
     async def async_disconnect(self) -> None:
         """Disconnect the SSH client.
 
-        Set `state.connected` to `False` and
-        update all sensor commands with `None`.
+        Set `state.connected` to `False` and update all sensor
+        commands with `None`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
     async def async_update_state(self, *, raise_errors: bool = False) -> None:
         """Update state.
 
         Raises:
-            OfflineError (`raise_errors`)
+            OfflineError (only with `raise_errors=True`)
             SSHHostKeyUnknownError
             SSHAuthError
-            SSHConnectError (`raise_errors`)
+            SSHConnectError (only with `raise_errors=True`)
         """
         if self.state.connected:
             try:
                 await self.async_execute_command(_TEST_COMMAND)
                 return
             except CommandError:
                 pass
@@ -296,23 +256,40 @@
         try:
             await self.async_connect()
         except SSHConnectError:
             if raise_errors:
                 raise
 
     async def async_turn_on(self) -> None:
-        """Turn the host on."""
-        if self.state.online:
+        """Turn on by Wake on LAN."""
+        if self.state.online or self.mac_address is None:
             return
 
         wakeonlan.send_magic_packet(self.mac_address)
 
     async def async_turn_off(self) -> None:
-        """Turn the host off.
+        """Turn off by running the `TURN_OFF` action.
 
         Raises:
             CommandError
         """
-        if self.allow_turn_off is False:
+        if not (
+            self.state.connected
+            and self.allow_turn_off
+            and ActionKey.TURN_OFF in self.action_commands_by_key
+        ):
             return
 
         await self.async_run_action(ActionKey.TURN_OFF)
+
+    async def async_restart(self) -> None:
+        """Restart by running the `RESTART` action.
+
+        Raises:
+            CommandError
+        """
+        if not (
+            self.state.connected and ActionKey.RESTART in self.action_commands_by_key
+        ):
+            return
+
+        await self.async_run_action(ActionKey.RESTART)
```

### Comparing `ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: ssh-terminal-manager
-Version: 0.2.0
-Summary: Control and monitor devices with SSH terminal commands
-Author-email: zhbjsh <zhbjsh@outlook.com>
-Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
-Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
-Keywords: ssh,terminal,command line
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# SSH Terminal Manager
-
-## Initialize
-
-```python
-from ssh_terminal_manager import SSHManager
-
-manager = SSHManager("192.168.0.123", username="user", password="1234")
-
-await manager.async_update_state(raise_errors=True)
-```
+Metadata-Version: 2.1
+Name: ssh-terminal-manager
+Version: 0.3.0
+Summary: Control and monitor devices with SSH terminal commands
+Author-email: zhbjsh <zhbjsh@outlook.com>
+Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
+Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
+Keywords: ssh,terminal,command line
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SSH Terminal Manager
+
+## Initialize
+
+```python
+from ssh_terminal_manager import SSHManager
+
+manager = SSHManager("192.168.0.123", username="user", password="1234")
+
+await manager.async_update_state(raise_errors=True)
+```
```

