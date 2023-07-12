# Comparing `tmp/storage_device_managers-0.13.0.tar.gz` & `tmp/storage_device_managers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage_device_managers-0.13.0.tar", max compression
+gzip compressed data, was "storage_device_managers-0.9.0.tar", max compression
```

## Comparing `storage_device_managers-0.13.0.tar` & `storage_device_managers-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35106 2023-07-12 21:34:04.584259 storage_device_managers-0.13.0/LICENSE
--rw-r--r--   0        0        0      566 2023-07-12 21:34:04.584259 storage_device_managers-0.13.0/README.md
--rw-r--r--   0        0        0     1364 2023-07-12 21:34:04.588259 storage_device_managers-0.13.0/pyproject.toml
--rw-r--r--   0        0        0    13347 2023-07-12 21:34:04.588259 storage_device_managers-0.13.0/src/storage_device_managers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:34:04.588259 storage_device_managers-0.13.0/src/storage_device_managers/py.typed
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 storage_device_managers-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0    35106 2023-06-15 19:36:56.857826 storage_device_managers-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1249 2023-06-15 21:36:15.761780 storage_device_managers-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-06-15 20:47:57.614397 storage_device_managers-0.9.0/src/storage_device_managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:47:57.614397 storage_device_managers-0.9.0/src/storage_device_managers/py.typed
+-rw-r--r--   0        0        0     8726 2023-06-15 21:31:36.242303 storage_device_managers-0.9.0/src/storage_device_managers/storage_device_managers.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 storage_device_managers-0.9.0/PKG-INFO
```

### Comparing `storage_device_managers-0.13.0/LICENSE` & `storage_device_managers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `storage_device_managers-0.13.0/pyproject.toml` & `storage_device_managers-0.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 [tool.poetry]
 name = "storage-device-managers"
-version = "0.13.0"
+version = "0.9.0"
 description = "Helpful context managers for managing decryption and mounts of storage devices"
-authors = ["Max Görner <5477952+MaxG87@users.noreply.github.com>"]
-repository = "https://github.com/MaxG87/storage-device-managers"
-readme = "README.md"
+authors = ["Max Görner <max@familie-goerner.eu>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-loguru = {version = "^0.7.0", optional = true}
-shell-interface = "^0.12.0"
-
-[tool.poetry.extras]
-logging = ["loguru"]
+loguru = "^0.7.0"
+shell-interface = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
-hypothesis = "^6.81.1"
-pytest = "^7.4.0"
+hypothesis = "^6.78.2"
+pytest = "^7.3.2"
 pynvim = "^0.4.3"
 jedi = "^0.18.2"
 pdbpp = "^0.10.3"
-pytest-cov = "^4.1.0"
-mypy = "^1.4.1"
-black = "^23.7.0"
-ruff = "^0.0.278"
+pytest-cov = "^3.0.0"
+mypy = "^1.3.0"
+black = "^23.3.0"
+ruff = "^0.0.272"
 
 [tool.mypy]
 allow_any_unimported = false
 warn_unreachable = true
 enable_error_code = [
     "possibly-undefined"
 ]
 strict = true
+allow_incomplete_defs = true
+allow_untyped_defs = true
 
 
 [[tool.mypy.overrides]]
 module = "tests.*"
-allow_incomplete_defs = true
-allow_untyped_defs = true
+disable_error_code = [
+    "possibly-undefined"
+]
 
 [tool.pytest.ini_options]
 addopts = [
     "--cov", "src",
     "--cov-branch",
     "--cov-fail-under", "85"
 ]
 testpaths = ["tests"]
 
 [tool.ruff]
 src = [".", "src/"]
 select = ["A", "B", "C", "F", "I", "ISC", "PIE", "PL", "Q", "RUF", "SIM", "TID", "W", "YTT"]
-ignore = ["E", "SIM117"]
+ignore = ["E", "PLC1901", "SIM117"]
 
 [tool.ruff.mccabe]
 max-complexity = 6
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `storage_device_managers-0.13.0/src/storage_device_managers/__init__.py` & `storage_device_managers-0.9.0/src/storage_device_managers/storage_device_managers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,27 @@
 from __future__ import annotations
 
 import contextlib
 import enum
 import secrets
 import string
 from collections import defaultdict
-from importlib import metadata
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from types import SimpleNamespace
-from typing import Iterator, Optional, Union
+from typing import Iterator, Optional
 from uuid import UUID, uuid4
 
 import shell_interface as sh
-
-try:
-    from loguru import logger  # type: ignore[import, unused-ignore]
-
-    logger.disable("storage_device_managers")
-except ModuleNotFoundError:
-    logger = SimpleNamespace()  # type: ignore[assignment, unused-ignore]
-    logger.success = lambda msg: None  # type: ignore[assignment, unused-ignore]
-    logger.info = lambda msg: None  # type: ignore[assignment, unused-ignore]
-
-__version__ = metadata.version(__name__)
-
-
-class DeviceDecryptionError(RuntimeError):
-    pass
+from loguru import logger
 
 
 class InvalidDecryptedDevice(ValueError):
     pass
 
 
-class UnmountError(RuntimeError):
-    pass
-
-
 class ValidCompressions(enum.Enum):
     LZO = "lzo"
     ZLIB = "zlib"
     ZLIB1 = "zlib:1"
     ZLIB2 = "zlib:2"
     ZLIB3 = "zlib:3"
     ZLIB4 = "zlib:4"
@@ -72,49 +52,43 @@
 def decrypted_device(device: Path, pass_cmd: str) -> Iterator[Path]:
     """Decrypt a given device using pass_cmd
 
     Given a device and a shell command that outputs a password on STDOUT, this
     context manager will open the device using `cryptsetup`. Upon exit, the
     device is closed again.
 
-
     Note that pass_cmd will directly be executed in a subshell. Therefore, DO NOT
     USE UNTRUSTED `pass_cmd`!
 
     Parameters:
     -----------
     device
         file-like object to be opened with `cryptsetup`
     pass_cmd
         command that prints the device's password on STDOUT
 
     Returns:
     --------
     Path
         destination of opened device
-
-    Raises:
-    -------
-    DeviceDecryptionError
-        if cryptsetup returns a non-zero exit code
     """
     decrypted = open_encrypted_device(device, pass_cmd)
     logger.success(f"Speichermedium {device} erfolgreich entschlüsselt.")
     try:
         yield decrypted
     finally:
         close_decrypted_device(decrypted)
         logger.success(
             f"Verschlüsselung des Speichermediums {device} erfolgreich geschlossen."
         )
 
 
 @contextlib.contextmanager
 def mounted_device(
-    device: Path, compression: Optional[ValidCompressions] = None
+    device: Path, compression: Optional[ValidCompressions]
 ) -> Iterator[Path]:
     """Mount a given BtrFS device
 
     Given a path pointing to a file-like object, this context manager will
     mount it to some temporary directory and return its path. Upon exit, the
     file-like object is unmounted again.
 
@@ -150,15 +124,15 @@
         finally:
             unmount_device(device)
             logger.success(f"Speichermedium {device} erfolgreich ausgehangen.")
 
 
 @contextlib.contextmanager
 def symbolic_link(src: Path, dest: Path) -> Iterator[Path]:
-    """Create a symbolic link from `src` to `dest`
+    """Create an symbolic link from `src` to `dest`
 
     This context manager will create a symbolic link from src to dest. It
     differentiates itself from `Path.link_to()` by …:
 
         * … creating the link with root privileges. This allows to limit root
           permissions to only the necessary parts of the program.
 
@@ -190,149 +164,58 @@
         # all, the aimed for state has been reached.
         rm_cmd: sh.StrPathList = ["sudo", "rm", "-f", absolute_dest]
         sh.run_cmd(cmd=rm_cmd)
         logger.success(f"Symlink von {src} nach {dest} erfolgreich entfernt.")
 
 
 def mount_btrfs_device(
-    device: Path, mount_dir: Path, compression: Optional[ValidCompressions] = None
+    device: Path, mount_dir: Path, compression: Optional[ValidCompressions]
 ) -> None:
-    """
-    Mount a given BtrFS device
-
-    Given a path pointing to a file-like object and a target directory, this function
-    will mount the device to the target directory.
-
-    The filesystem of `device` must be BtrFS. While technically other file systems
-    might work too, this behaviour is not guaranteed and might be broken without
-    further notice!
-
-    If `compression` is provided, a mount option specifying the transparent file
-    system compression is set.
-
-    Parameters:
-    -----------
-    device
-        file-like object to be mounted
-    mount_dir
-        directory to which `device` is mounted
-    compression
-        compression level to be used by BtrFS
-    """
     cmd: sh.StrPathList = [
         "sudo",
         "mount",
         device,
         mount_dir,
     ]
     if compression is not None:
         cmd.extend(["-o", f"compress={compression.value}"])
     sh.run_cmd(cmd=cmd)
 
 
-def is_mounted(device: Path) -> bool:
-    """Check whether a given device is mounted
-
-    Parameters:
-    -----------
-    device
-        file-like object to be checked
-
-    Returns:
-    --------
-    bool
-        True if `device` is mounted, False otherwise
-    """
-    device_as_str = str(device)
+def is_mounted(dest: Path) -> bool:
+    dest_as_str = str(dest)
     try:
-        mount_dest = get_mounted_devices()[device_as_str]
-        logger.info(f"Mount des Speichermediums {device} in {mount_dest} gefunden.")
+        mount_dest = get_mounted_devices()[dest_as_str]
+        logger.info(f"Mount des Speichermediums {dest} in {mount_dest} gefunden.")
     except KeyError:
-        logger.info(f"Kein Mountpunkt für Speichermedium {device} gefunden.")
+        logger.info(f"Kein Mountpunkt für Speichermedium {dest} gefunden.")
         return False
     return True
 
 
 def get_mounted_devices() -> dict[str, set[Path]]:
-    """Get all mounted devices
-
-    This function will parse the output of `mount` and return everything that
-    is mounted to somewhere. Since a source can be mounted to multiple
-    destinations, the return value is a dictionary mapping device names to sets
-    of mount points.
-
-    Returns:
-    --------
-    dict
-        A dictionary mapping device names to the set of mount points.
-    """
     raw_mounts = sh.run_cmd(cmd=["mount"], capture_output=True)
     mount_lines = raw_mounts.stdout.decode().splitlines()
     mount_points = defaultdict(set)
     for line in mount_lines:
         device = line.split()[0]
         dest = Path(line.split()[2])
         mount_points[device].add(dest)
     return dict(mount_points)
 
 
 def unmount_device(device: Path) -> None:
-    """Unmount a given device
-
-    This function will unmount a given device. It relies on the system's
-    `umount` programm to do so.
-
-    Parameters:
-    -----------
-    device
-        The device to be unmounted.
-
-    Raises:
-    -------
-    UnmountError
-        if `umount` returns a non-zero exit code
-    """
     cmd: sh.StrPathList = ["sudo", "umount", device]
-    try:
-        sh.run_cmd(cmd=cmd)
-    except sh.ShellInterfaceError as e:
-        raise UnmountError from e
+    sh.run_cmd(cmd=cmd)
 
 
 def open_encrypted_device(device: Path, pass_cmd: str) -> Path:
-    """Open an encrypted device
-
-    This function will open an encrypted device. The given path must point to a
-    device that can be opened by `cryptsetup`.
-
-    In order to encrypt the device, `pass_cmd` is executed and its output is
-    piped into `cryptsetup`. This allows to use any program that can output
-    the password to decrypt the device.
-
-    Note that pass_cmd will directly be executed in a subshell. Therefore, DO NOT
-    USE UNTRUSTED `pass_cmd`!
-
-    Parameters:
-    -----------
-    device
-        The device to be opened.
-    pass_cmd
-        The command that outputs the password to decrypt the device.
-
-    Raises:
-    -------
-    DeviceDecryptionError
-        if cryptsetup returns a non-zero exit code
-    """
     map_name = device.name
     decrypt_cmd: sh.StrPathList = ["sudo", "cryptsetup", "open", device, map_name]
-    try:
-        sh.pipe_pass_cmd_to_real_cmd(pass_cmd, decrypt_cmd)
-    except sh.ShellInterfaceError as e:
-        raise DeviceDecryptionError from e
+    sh.pipe_pass_cmd_to_real_cmd(pass_cmd, decrypt_cmd)
     return Path("/dev/mapper/") / map_name
 
 
 def close_decrypted_device(device: Path) -> None:
     """Close a decrypted device
 
     This function will try to close a device that was previously opened by
@@ -345,15 +228,15 @@
     device
         The device do be closed.
 
     Raises:
     -------
     InvalidDecryptedDevice
         if `device` does not point into `/dev/mapper`
-    shell_interface.ShellInterfaceError
+    CalledProcessError
         if the exit code of the close command is non-zero
     """
     if device.parent != Path("/dev/mapper"):
         raise InvalidDecryptedDevice
     map_name = device.name
     close_cmd = ["sudo", "cryptsetup", "close", map_name]
     sh.run_cmd(cmd=close_cmd)
@@ -418,54 +301,7 @@
     str
         password command producing the password
     """
     n_chars = 16
     alphabet = string.ascii_letters + string.digits
     passphrase = "".join(secrets.choice(alphabet) for _ in range(n_chars))
     return f"echo {passphrase}"
-
-
-def chown(
-    file_or_folder: Path,
-    /,
-    user: Union[int, str],
-    group: Optional[Union[int, str]] = None,
-    *,
-    recursive: bool,
-) -> None:
-    """Change user and group of a device or folder
-
-    This function will change the ownership as specified. It requires root
-    privileges and will ask for them if not available. If no group is given,
-    only the owner is changed.
-
-    If recursive is true, ownership information of all files and folders
-    contained by `file_or_folder` will be adapted.
-
-    If `file_or_folder` points to a file, `recursive` must be `False`.
-    Otherwise a ValueError will be raised.
-
-
-    Parameters:
-    -----------
-    user
-        user ID, either as name or as UID
-    group
-        group ID, either as name or as GID
-    recursive
-        whether or not to change ownership for content
-
-    Raises:
-    --------
-    ValueError
-        if `file_or_folder` is a file but `recursive` is `True`
-    """
-    if file_or_folder.is_file() and recursive:
-        raise ValueError(
-            "First argument must point to a directory if `recursive` is `True`!"
-        )
-
-    user_spec = str(user) if group is None else f"{user}:{group}"
-    chown_cmd: sh.StrPathList = ["sudo", "chown", user_spec, file_or_folder]
-    if recursive is not None:
-        chown_cmd.append("--recursive")
-    sh.run_cmd(cmd=chown_cmd)
```

