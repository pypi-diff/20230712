# Comparing `tmp/key_switcheroo-0.0.6.tar.gz` & `tmp/key_switcheroo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.6.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.7.tar", max compression
```

## Comparing `key_switcheroo-0.0.6.tar` & `key_switcheroo-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0     5060 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/README.md
--rw-r--r--   0        0        0      678 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/__init__.py
--rw-r--r--   0        0        0     3164 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/custom_keygen.py
--rw-r--r--   0        0        0       77 2023-07-07 03:40:51.516287 key_switcheroo-0.0.6/switcheroo/data_store/__init__.py
--rw-r--r--   0        0        0     3307 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/data_store/data_stores.py
--rw-r--r--   0        0        0     3024 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/data_store/s3.py
--rw-r--r--   0        0        0      632 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/exceptions.py
--rw-r--r--   0        0        0     1410 2023-07-07 03:40:51.516287 key_switcheroo-0.0.6/switcheroo/paths.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     1617 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/server/__init__.py
--rwxr-xr-x   0        0        0     1915 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/server/__main__.py
--rw-r--r--   0        0        0     5045 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/server/server.py
--rw-r--r--   0        0        0     2658 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/util.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5060 2023-07-09 19:13:51.612702 key_switcheroo-0.0.7/README.md
+-rw-r--r--   0        0        0      788 2023-07-12 16:58:29.038276 key_switcheroo-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.7/switcheroo/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/__init__.py
+-rw-r--r--   0        0        0     3654 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/__init__.py
+-rw-r--r--   0        0        0     1909 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/s3.py
+-rw-r--r--   0        0        0       92 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/util.py
+-rw-r--r--   0        0        0      356 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/exceptions/s3.py
+-rw-r--r--   0        0        0      287 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/serializer.py
+-rw-r--r--   0        0        0     1774 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/paths.py
+-rw-r--r--   0        0        0      205 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/__init__.py
+-rw-r--r--   0        0        0     1296 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/s3.py
+-rw-r--r--   0        0        0     2957 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/__init__.py
+-rw-r--r--   0        0        0     1809 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/s3.py
+-rw-r--r--   0        0        0      931 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_stores/__init__.py
+-rw-r--r--   0        0        0      834 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/exceptions.py
+-rw-r--r--   0        0        0      183 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/objects/__init__.py
+-rw-r--r--   0        0        0     4638 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/objects/key.py
+-rw-r--r--   0        0        0        0 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/scripts/__init__.py
+-rw-r--r--   0        0        0     1966 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/scripts/publish.py
+-rwxr-xr-x   0        0        0     2002 2023-07-11 21:36:01.857025 key_switcheroo-0.0.7/switcheroo/ssh/scripts/retrieve.py
+-rw-r--r--   0        0        0     2997 2023-07-12 16:58:29.038276 key_switcheroo-0.0.7/switcheroo/util.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.7/PKG-INFO
```

### Comparing `key_switcheroo-0.0.6/README.md` & `key_switcheroo-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.6/pyproject.toml` & `key_switcheroo-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 boto3 = "^1.27.0"
 
 [tool.poetry.group.dev.dependencies]
 PyHamcrest = "^2.0.4"
 pyright = "^1.1.316"
 pylint = "^2.17.4"
 black = "^23.3.0"
+boto3-stubs = {version = "1.27.0", extras = ["s3", "sts"]}
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.scripts]
 
-switcheroo_publish = "switcheroo.publisher.__main__:main"
-switcheroo_retrieve = "switcheroo.server.__main__:main"
+switcheroo_publish = "switcheroo.ssh.scripts.publish:main"
+switcheroo_retrieve = "switcheroo.ssh.scripts.retrieve:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `key_switcheroo-0.0.6/switcheroo/data_store/data_stores.py` & `key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,94 @@
-"Data stores that specifies where a Server stores its keys"
-from abc import ABC, abstractmethod
+from abc import abstractmethod
+from typing import TypeVar
 from pathlib import Path
-from tempfile import TemporaryDirectory
+from switcheroo.base.data_store import DataStore
+from switcheroo.ssh.data_stores import ssh_home_file_ds
+from switcheroo.ssh.objects import Key, KeyMetadata
+from switcheroo.ssh.exceptions import SSHItem, SSHItemNotFoundException
+from switcheroo.ssh import AuthorizedKeysCmndProvider
 from switcheroo import paths
-from switcheroo.custom_keygen import KeyMetadata
-from switcheroo import util
-from switcheroo.exceptions import KeyNotFoundException
 
+T = TypeVar("T")
 
-class DataStore(ABC):
-    "A server uses a DataStore to get public keys from somewhere."
-
-    def __init__(self, ssh_home: Path | None = None, temp: bool = False):
-        # If temp is true, will reset the home_dir to a temp file upon usage as a context manager
-        self._temp = temp
-        # ssh_home is only relevant if not being used as a context manager
-        self._dir: Path = paths.local_ssh_home() if ssh_home is None else ssh_home
-        # To be used later if we decide to use this as a context manager, and temp is selected
-        self._temp_dir: TemporaryDirectory[str] | None = None
 
-    @property
-    def home_dir(self) -> Path:
-        """The folder where local files are stored"""
-        if self._temp and self._temp_dir is not None:
-            return Path(self._temp_dir.name)
-        return self._dir
+def retrieve_or_throw(  # pylint: disable=too-many-arguments
+    data_store: DataStore,
+    location: Path,
+    clas: type[T],
+    ssh_item: SSHItem,
+    user: str,
+    host: str,
+) -> T:
+    result = data_store.retrieve(location, clas)
+    if result is None:
+        raise SSHItemNotFoundException(
+            SSHItemNotFoundException.Data(
+                requested_user=user, requested_host=host, requested_item=ssh_item
+            )
+        )
+    return result
 
+
+class KeyRetriever(AuthorizedKeysCmndProvider):
     @abstractmethod
-    def get_sshd_config_line(self):
-        "Return the config line that the server will add to the sshd_config"
+    def retrieve_private_key(self, host: str, user: str) -> Key.PrivateComponent:
+        pass
 
     @abstractmethod
-    def publish(
-        self, host: str, user: str, metadata: KeyMetadata | None
-    ) -> tuple[str, KeyMetadata]:
-        """Publish a new public key for the given host and user with metadata"""
+    def retrieve_public_key(self, host: str, user: str) -> Key.PublicComponent:
+        pass
 
     @abstractmethod
-    def retrieve(self, host: str, user: str) -> str:
-        """Retrieve the public key for the given host and user"""
+    def retrieve_key_metadata(self, host: str, user: str) -> KeyMetadata:
+        pass
 
-    def __enter__(self):
-        if self._temp:
-            self._temp_dir: TemporaryDirectory[str] | None = TemporaryDirectory[
-                str
-            ](  # pylint: disable=consider-using-with
-                prefix="ssh-keys-", dir=self._dir
+    def retrieve_key(self, host: str, user: str) -> tuple[Key, KeyMetadata]:
+        key = Key(
+            (
+                self.retrieve_private_key(host, user).byte_data,
+                self.retrieve_public_key(host, user).byte_data,
             )
+        )
+        metadata = self.retrieve_key_metadata(host, user)
+        return (key, metadata)
+
 
-    def __exit__(self, exc_t, exc_v, exc_tb):
-        if self._temp:
-            assert self._temp_dir is not None
-            self._temp_dir.__exit__(None, None, None)
-
-
-class FileSystemDataStore(DataStore):
-    "Stores keys in a file system"
-
-    def get_sshd_config_line(self) -> str:
-        return f'-ds local --sshdir "{str(self.home_dir)}"'
-
-    def publish(
-        self, host: str, user: str, metadata: KeyMetadata | None = None
-    ) -> tuple[str, KeyMetadata]:
-        if metadata is None:
-            metadata = KeyMetadata.now_by_executing_user()
-        _, public_key = util.generate_private_public_key_in_file(
-            paths.local_key_dir(host, user, home_dir=self.home_dir)
+class FileKeyRetriever(KeyRetriever):
+    def __init__(self, key_dir: Path) -> None:
+        super().__init__()
+        self._key_dir = key_dir
+        self._key_datastore = ssh_home_file_ds(key_dir)
+
+    def retrieve_public_key(self, host: str, user: str) -> Key.PublicComponent:
+        return retrieve_or_throw(
+            self._key_datastore,
+            location=paths.local_relative_public_key_loc(host, user),
+            clas=Key.PublicComponent,
+            ssh_item="public key",
+            host=host,
+            user=user,
         )
-        metadata_file = paths.local_metadata_loc(host, user, home_dir=self.home_dir)
-        with open(metadata_file, encoding="utf-8", mode="wt") as metadata_file:
-            metadata.serialize(metadata_file)
-        return public_key.decode(), metadata
-
-    def retrieve(self, host: str, user: str) -> str:
-        key_path = paths.local_public_key_loc(host, user, home_dir=self.home_dir)
-        try:
-            with open(key_path, mode="rt", encoding="utf-8") as key_file:
-                return key_file.read()
-        except FileNotFoundError as exc:
-            exception_data = KeyNotFoundException.Data(user, host)
-            raise KeyNotFoundException(exception_data) from exc
+
+    def retrieve_private_key(self, host: str, user: str) -> Key.PrivateComponent:
+        return retrieve_or_throw(
+            self._key_datastore,
+            location=paths.local_relative_private_key_loc(host, user),
+            clas=Key.PrivateComponent,
+            ssh_item="private key",
+            host=host,
+            user=user,
+        )
+
+    def retrieve_key_metadata(self, host: str, user: str) -> KeyMetadata:
+        return retrieve_or_throw(
+            self._key_datastore,
+            location=paths.local_relative_metadata_loc(host, user),
+            clas=KeyMetadata,
+            ssh_item="metadata",
+            host=host,
+            user=user,
+        )
+
+    @property
+    def command(self) -> str:
+        return f'-ds local --sshdir "{str(self._key_dir)}"'
```

### Comparing `key_switcheroo-0.0.6/switcheroo/exceptions.py` & `key_switcheroo-0.0.7/switcheroo/ssh/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import dataclasses
+from typing import TypeAlias, Literal
 
+SSHItem: TypeAlias = Literal["public key", "private key", "metadata"]
 
-class KeyNotFoundException(Exception):
+
+class SSHItemNotFoundException(Exception):
     """Raised when a public key cannot be found for the user.
 
     Attributes:
         message -- explanation of the error
     """
 
     @dataclasses.dataclass(frozen=True)
     class Data:
         requested_user: str
         requested_host: str
+        requested_item: SSHItem
 
     def __init__(self, data: Data | None = None):
         if data is None:
-            self.message = "Public key could not be found!"
+            self.message = "Some SSH-related item could not be found!"
         else:
-            self.message = f"Public key could not be found for user {data.requested_user}\
-                and host {data.requested_host}"
+            self.message = (
+                f"{data.requested_item} could not be found for user "
+                f"{data.requested_user} and host {data.requested_host}"
+            )
         super().__init__(self.message)
```

### Comparing `key_switcheroo-0.0.6/switcheroo/paths.py` & `key_switcheroo-0.0.7/switcheroo/paths.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from switcheroo.custom_keygen import KeyGen, KeyMetadata
+from switcheroo.ssh.objects.key import KeyMetadata, KeyGen
 
 
 def local_ssh_home() -> Path:
     """Path to the .ssh dir"""
     return Path.home() / ".ssh"
 
 
@@ -15,23 +15,35 @@
 
 
 def local_public_key_loc(host: str, user: str, home_dir: Path | None) -> Path:
     """Path to the public key (if stored locally) for a host/user"""
     return local_key_dir(host, user, home_dir=home_dir) / KeyGen.PUBLIC_KEY_NAME
 
 
+def local_relative_public_key_loc(host: str, user: str) -> Path:
+    return Path(host) / user / KeyGen.PUBLIC_KEY_NAME
+
+
+def local_relative_private_key_loc(host: str, user: str) -> Path:
+    return Path(host) / user / KeyGen.PRIVATE_KEY_NAME
+
+
 def local_private_key_loc(host: str, user: str, home_dir: Path | None) -> Path:
     """Path to the private key for a host/user"""
     return local_key_dir(host, user, home_dir=home_dir) / KeyGen.PRIVATE_KEY_NAME
 
 
 def local_metadata_loc(host: str, user: str, home_dir: Path | None) -> Path:
     return local_key_dir(host, user, home_dir=home_dir) / KeyMetadata.FILE_NAME
 
 
+def local_relative_metadata_loc(host: str, user: str) -> Path:
+    return Path(host) / user / KeyMetadata.FILE_NAME
+
+
 def cloud_key_dir(host: str, user: str) -> Path:
     return Path(host) / user
 
 
 def cloud_public_key_loc(host: str, user: str) -> Path:
     """Path to the public key (if stored in the cloud) for a host/user"""
     return cloud_key_dir(host, user) / KeyGen.PUBLIC_KEY_NAME
```

### Comparing `key_switcheroo-0.0.6/switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.7/switcheroo/ssh/scripts/publish.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from pathlib import Path
 from argparse import ArgumentParser
-from switcheroo.publisher.key_publisher import Publisher, LocalPublisher, S3Publisher
+from switcheroo.ssh.data_org.publisher import KeyPublisher, FileKeyPublisher
+from switcheroo.ssh.data_org.publisher.s3 import S3KeyPublisher
+from switcheroo import paths
 
 
 def create_argument_parser() -> ArgumentParser:
+    # pylint: disable=R0801
     argument_parser = ArgumentParser(
         prog="key_publisher",
         description="Creates public/private SSH keys and publishes "
         + "the public key either locally or to S3 (default is S3)",
         epilog="Thanks for using key_publisher! :)",
     )
 
@@ -16,32 +20,40 @@
     argument_parser.add_argument(
         "-ds",
         "--datastore",
         choices=["s3", "local"],
         default="s3",
         help="choose where to store the public key, on S3 or on the local system (default is S3)",
     )
+
     argument_parser.add_argument(
         "--bucket",
         required=False,
         help="If s3 is selected, the bucket name to store the key in",
     )
+    argument_parser.add_argument(
+        "--sshdir",
+        required=False,
+        help="The absolute path to\
+            the directory that stores local keys (ie /home/you/.ssh)",
+        default=paths.local_ssh_home(),
+    )
 
     return argument_parser
 
 
 def main():
     parser = create_argument_parser()
     args = parser.parse_args()
-    publisher: Publisher | None = None
+    publisher: KeyPublisher | None = None
     if args.datastore == "local":  # If the user chose to store the public key locally
-        publisher = LocalPublisher(args.hostname, args.user)
+        publisher = FileKeyPublisher(Path(args.sshdir))
     else:  # If the user chose to store the public key on S3 or chose to default to S3
         if args.bucket is None:
             parser.error("The s3 option requires a bucket name!")
-        publisher = S3Publisher(args.bucket, args.hostname, args.user)
+        publisher = S3KeyPublisher(args.bucket, root_ssh_dir=Path(args.sshdir))
     assert publisher is not None
-    publisher.publish_new_key()
+    publisher.publish_key(args.hostname, args.user)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `key_switcheroo-0.0.6/switcheroo/server/__main__.py` & `key_switcheroo-0.0.7/switcheroo/ssh/scripts/retrieve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from argparse import ArgumentParser
 from pathlib import Path
 import socket
 import traceback
-from switcheroo.data_store import DataStore, FileSystemDataStore
-from switcheroo.data_store.s3 import S3DataStore
+from switcheroo.ssh.data_org.retriever import KeyRetriever, FileKeyRetriever
+from switcheroo.ssh.data_org.retriever.s3 import S3KeyRetriever
 from switcheroo import paths
 
 
 def create_argument_parser() -> ArgumentParser:
+    # pylint: disable=R0801
     argument_parser = ArgumentParser(
         prog="key_retriever",
         description="Fetches the public SSH keys from S3 or the local machine",
         epilog="Thanks for using key_retriever! :)",
     )
     argument_parser.add_argument("user")
     argument_parser.add_argument(
@@ -25,36 +26,36 @@
         "--bucket",
         required=False,
         help="If s3 is selected, the bucket name to look for the key",
     )
     argument_parser.add_argument(
         "--sshdir",
         required=False,
-        help="If local is selected, the absolute path to\
-            the directory that stores the keys (ie /home/you/.ssh)",
+        help="The absolute path to\
+            the directory that stores local keys (ie /home/you/.ssh)",
         default=paths.local_ssh_home(),
     )
     return argument_parser
 
 
 def main():
     parser = create_argument_parser()
     args = parser.parse_args()
-    data_store: DataStore | None = None
+    retriever: KeyRetriever | None = None
 
     if args.datastore == "local":
-        data_store = FileSystemDataStore(Path(args.sshdir))
+        retriever = FileKeyRetriever(Path(args.sshdir))
     elif args.datastore == "s3":
         if args.bucket is None:
             parser.error("The s3 option requires a specified bucket name!")
-        data_store = S3DataStore(args.bucket)
+        retriever = S3KeyRetriever(paths.local_ssh_home(), args.bucket)
     try:
-        assert data_store is not None
-        public_key = data_store.retrieve(socket.getfqdn(), args.user)
-        print(public_key)
+        assert retriever is not None
+        public_key = retriever.retrieve_public_key(socket.getfqdn(), args.user)
+        print(public_key.byte_data.decode())
     except Exception as exc:  # pylint: disable = broad-exception-caught
         print(exc)
         print(traceback.format_exc())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `key_switcheroo-0.0.6/switcheroo/util.py` & `key_switcheroo-0.0.7/switcheroo/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Utility functions"""
 from socket import getservbyport
 from random import randint
 import os
 from pathlib import Path
-from switcheroo.custom_keygen import KeyGen
+from switcheroo.ssh.objects.key import KeyMetadata, KeyGen
 
 
 def get_open_port() -> int:
     "Returns a random open port, starting at 1024"
     start_port = 1024
     all_primary_ports = list(range(start_port, start_port + 100))
     last_selectable_port = all_primary_ports[len(all_primary_ports) - 1]
 
     def select_new_port() -> int:
         nonlocal all_primary_ports
         if len(all_primary_ports) == 0:  # Out of ports
             nonlocal last_selectable_port
             # Create a new port range to choose from
             all_primary_ports = list(
-                range(last_selectable_port + 1, last_selectable_port + 1001)
+                range(last_selectable_port + 1, last_selectable_port + 101)
             )
-            last_selectable_port += 100
+            last_selectable_port += 101
         # Choose a new port
         new_port_index = randint(0, len(all_primary_ports) - 1)
         # Remove it from our options, so we dont choose it again
+        port = all_primary_ports[new_port_index]
         del all_primary_ports[new_port_index]
-        return all_primary_ports[new_port_index]
+        return port
 
     # Select a new port until we find an open one
     while True:
         selected_port = select_new_port()
         try:
             getservbyport(selected_port)
         except OSError:
@@ -42,32 +43,40 @@
     os.umask(0)
 
     # Opener to restrict permissions
     def open_restricted_permissions(path: str, flags: int):
         return os.open(path=str(path), flags=flags, mode=0o600)
 
     with open(
-        str(private_key_path), mode="wb", opener=open_restricted_permissions
+        str(private_key_path),
+        mode="wt",
+        encoding="utf-8",
+        opener=open_restricted_permissions,
     ) as private_out:
-        private_out.write(private_key)
+        private_out.write(private_key.decode())
 
 
 def store_public_key(public_key: bytes, public_key_dir: Path):
     public_key_dir.mkdir(parents=True, exist_ok=True)
     public_key_path = public_key_dir / KeyGen.PUBLIC_KEY_NAME
-    with open(public_key_path, mode="wb") as public_out:
-        public_out.write(public_key)
+    with open(public_key_path, mode="wt", encoding="utf-8") as public_out:
+        public_out.write(public_key.decode())
 
 
 def generate_private_public_key_in_file(
     public_key_dir: Path, private_key_dir: Path | None = None
 ) -> tuple[bytes, bytes]:
     "Creates a private key and public key at the given paths"
     # If private key was not given a separate dir, use the same one as for public key
     if private_key_dir is None:
         private_key_dir = public_key_dir
     # Generate the keys
     private_key, public_key = KeyGen.generate_private_public_key()
     # Store them
     store_private_key(private_key, private_key_dir)
     store_public_key(public_key, public_key_dir)
+    metadata = KeyMetadata.now_by_executing_user()
+    with open(
+        public_key_dir / KeyMetadata.FILE_NAME, mode="wt", encoding="utf-8"
+    ) as metadata_file:
+        metadata_file.write(metadata.serialize_to_string())
     return private_key, public_key
```

### Comparing `key_switcheroo-0.0.6/PKG-INFO` & `key_switcheroo-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

