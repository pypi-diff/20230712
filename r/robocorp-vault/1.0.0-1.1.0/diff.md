# Comparing `tmp/robocorp_vault-1.0.0.tar.gz` & `tmp/robocorp_vault-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_vault-1.0.0.tar", max compression
+gzip compressed data, was "robocorp_vault-1.1.0.tar", max compression
```

## Comparing `robocorp_vault-1.0.0.tar` & `robocorp_vault-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1194 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/README.md
--rw-r--r--   0        0        0      782 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5351 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/__init__.py
--rw-r--r--   0        0        0      112 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_errors.py
--rw-r--r--   0        0        0     1587 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_secrets.py
--rw-r--r--   0        0        0     1858 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_utils.py
--rw-r--r--   0        0        0    18022 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_vault.py
--rw-r--r--   0        0        0        0 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/py.typed
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 robocorp_vault-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1193 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/README.md
+-rw-r--r--   0        0        0      802 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5350 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/__init__.py
+-rw-r--r--   0        0        0    12926 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_adapters.py
+-rw-r--r--   0        0        0      112 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_errors.py
+-rw-r--r--   0        0        0     6335 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_requests.py
+-rw-r--r--   0        0        0     1587 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_secrets.py
+-rw-r--r--   0        0        0     1858 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_utils.py
+-rw-r--r--   0        0        0     3080 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_vault.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/py.typed
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 robocorp_vault-1.1.0/PKG-INFO
```

### Comparing `robocorp_vault-1.0.0/README.md` & `robocorp_vault-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Robocorp Control Room Vault API library
 
 `robocorp-vault` is a library which provides read and write access to the
 `Vault` at `Robocorp Control Room`.
 
-
 ## Usage
 
-
 ```python    
 from robocorp import vault
 from robocorp import log 
 
 def reading_secrets():
     secrets_container = vault.get_secret('secret_name')
     # Shows secret keys available:
@@ -29,8 +27,8 @@
 Note that values set or gotten from the vault will be automatically
 hidden from `robocorp.log` logs (if `robocorp.log` is available
 in the environment), but care needs to be taken when setting it
 so that secrets don't become exposed before being set into the vault.
 
 i.e.: When setting values into the vault, if such values are sensitive,
 use `with robocorp.log.suppress_variables()` so that such value doesn't
-become logged before it's received by the vault.
+become logged before it's received by the vault.
```

### Comparing `robocorp_vault-1.0.0/pyproject.toml` & `robocorp_vault-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-vault"
-version = "1.0.0"
+version = "1.1.0"
 description = "Robocorp Control Room Vault API integration library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
@@ -12,14 +12,15 @@
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cryptography = "^41.0.1"
 requests = "^2.31"
 pyyaml = "^6.0"
+tenacity = "^8.0.1"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 mock = "^5.0"
 types-requests = "^2.31"
 types-mock = "^5.0"
 types-PyYAML = "^6.0"
```

### Comparing `robocorp_vault-1.0.0/src/robocorp/vault/__init__.py` & `robocorp_vault-1.1.0/src/robocorp/vault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     "swaglabs": {
         "username": "standard_user",
         "password": "secret_sauce"
     }
 }
 ```
 
-
 OR
 
 ```yaml
 
 swaglabs:
     username: standard_user
     password: secret_sauce
@@ -65,15 +64,15 @@
 
 
 from contextlib import nullcontext
 from functools import lru_cache
 
 from ._secrets import SecretContainer
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @lru_cache
 def _get_vault():
     from ._vault import Vault
```

### Comparing `robocorp_vault-1.0.0/src/robocorp/vault/_secrets.py` & `robocorp_vault-1.1.0/src/robocorp/vault/_secrets.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.0.0/src/robocorp/vault/_utils.py` & `robocorp_vault-1.1.0/src/robocorp/vault/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.0.0/src/robocorp/vault/_vault.py` & `robocorp_vault-1.1.0/src/robocorp/vault/_adapters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import base64
 import binascii
 import copy
 import json
 import logging
 import os
-import traceback
 from abc import ABCMeta, abstractmethod
 from typing import Callable, Tuple
 
-import requests
 from cryptography.exceptions import InvalidTag
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 
 from ._errors import RobocorpVaultError
+from ._requests import HTTPError, Requests
 from ._secrets import SecretContainer
-from ._utils import import_by_name, required_env, resolve_path, url_join
+from ._utils import required_env, resolve_path, url_join
 
 
 class BaseSecretManager(metaclass=ABCMeta):
     """Abstract class for secrets management.
 
     Should be used as a base-class for any adapter implementation.
     """
 
     @abstractmethod
-    def get_secret(self, secret_name):
+    def get_secret(self, secret_name) -> SecretContainer:
         """Return ``SecretContainer`` object with given name."""
 
     @abstractmethod
     def set_secret(self, secret: SecretContainer):
         """Set a secret with a new value."""
 
 
@@ -102,23 +101,24 @@
 
     def _load(self):
         """Load secrets file."""
         with open(self.path, encoding="utf-8") as fd:
             data = self._loader(fd)
 
         if not isinstance(data, dict):
-            raise ValueError("Invalid content format")
+            raise ValueError(f"Expected dictionary, was '{type(data)}'")
 
         return data
 
     def _save(self, data):
         """Save the secrets content to disk."""
+        if not isinstance(data, dict):
+            raise ValueError(f"Expected dictionary, was '{type(data)}'")
+
         with open(self.path, "w", encoding="utf-8") as f:
-            if not isinstance(data, dict):
-                raise ValueError("Invalid content format")
             self._dumper(data, f, indent=4)
 
     def get_secret(self, secret_name: str) -> SecretContainer:
         """Get secret defined with given name from file.
 
         Args:
             secret_name: Name of secret to fetch
@@ -168,35 +168,32 @@
 
     ENCRYPTION_SCHEME = "robocloud-vault-transit-v2"
 
     def __init__(self, *args, **kwargs):
         # pylint: disable=unused-argument
         self.logger = logging.getLogger(__name__)
         # Environment variables set by runner
-        self._host = required_env("RC_API_SECRET_HOST")
-        self._token = required_env("RC_API_SECRET_TOKEN")
-        self._workspace = required_env("RC_WORKSPACE_ID")
+        host = required_env("RC_API_SECRET_HOST")
+        token = required_env("RC_API_SECRET_TOKEN")
+        workspace = required_env("RC_WORKSPACE_ID")
+        headers = {"Authorization": f"Bearer {token}"}
+        endpoint = url_join(
+            host,
+            "secrets-v1",
+            "workspaces",
+            workspace,
+            "secrets",
+            "",  # Ensure endpoint has trailing slash
+        )
+        self._client = Requests(route_prefix=endpoint, default_headers=headers)
         # Generated lazily on request
         self.__private_key = None
         self.__public_bytes = None
 
     @property
-    def headers(self):
-        """Default request headers."""
-        return {"Authorization": f"Bearer {self._token}"}
-
-    @property
-    def params(self):
-        """Default request parameters."""
-        return {
-            "encryptionScheme": self.ENCRYPTION_SCHEME,
-            "publicKey": self._public_bytes,
-        }
-
-    @property
     def _private_key(self):
         """Cryptography private key object."""
         if self.__private_key is None:
             self.__private_key = rsa.generate_private_key(
                 public_exponent=65537, key_size=4096, backend=default_backend()
             )
 
@@ -211,60 +208,51 @@
                     encoding=serialization.Encoding.DER,
                     format=serialization.PublicFormat.SubjectPublicKeyInfo,
                 )
             )
 
         return self.__public_bytes
 
-    def create_secret_url(self, name):
-        """Create a URL for a specific secret."""
-        return url_join(
-            self._host, "secrets-v1", "workspaces", self._workspace, "secrets", name
-        )
-
-    def create_public_key_url(self):
-        """Create a URL for encryption public key."""
-        return url_join(
-            self._host,
-            "secrets-v1",
-            "workspaces",
-            self._workspace,
-            "secrets",
-            "publicKey",
-        )
-
     def get_secret(self, secret_name: str) -> SecretContainer:
         """Get secret defined with given name from Robocorp Vault.
 
         Args:
             secret_name: Name of secret to fetch
         Returns:
             SecretContainer object
 
         Raises:
             RobocorpVaultError: Error with API request or response payload
         """
-        url = self.create_secret_url(secret_name)
+        params = {
+            "encryptionScheme": self.ENCRYPTION_SCHEME,
+            "publicKey": self._public_bytes,
+        }
 
         try:
-            response = requests.get(url, headers=self.headers, params=self.params)
-            response.raise_for_status()
-
+            response = self._client.get(secret_name, params=params)
             payload = response.json()
             payload = self._decrypt_payload(payload)
-        except InvalidTag as e:
-            self.logger.debug(traceback.format_exc())
-            raise RobocorpVaultError("Failed to validate authentication tag") from e
-        except Exception as exc:
-            self.logger.debug(traceback.format_exc())
-            raise RobocorpVaultError from exc
-
-        return SecretContainer(
-            payload["name"], payload["description"], payload["values"]
-        )
+            return SecretContainer(
+                name=payload["name"],
+                description=payload["description"],
+                values=payload["values"],
+            )
+        except InvalidTag as err:
+            raise RobocorpVaultError("Failed to validate authentication tag") from err
+        except HTTPError as err:
+            if err.status_code == 403:
+                message = "Not authorized to read secret. Is your token valid?"
+            elif err.status_code == 404:
+                message = f"No secret with name '{secret_name}' available"
+            else:
+                message = str(err)
+            raise RobocorpVaultError(message) from err
+        except Exception as err:
+            raise RobocorpVaultError(str(err)) from err
 
     def _decrypt_payload(self, payload):
         payload = copy.deepcopy(payload)
 
         fields = payload.pop("encryption", None)
         if fields is None:
             raise KeyError("Missing encryption fields from response")
@@ -307,50 +295,51 @@
 
         """
         value, aes_iv, aes_key, aes_tag = self._encrypt_secret_value_with_aes(secret)
         pub_key = self.get_publickey()
         aes_enc = self._encrypt_aes_key_with_public_rsa(aes_key, pub_key)
 
         payload = {
-            "description": secret.description,
             "encryption": {
                 "authTag": aes_tag.decode(),
                 "encryptedAES": aes_enc.decode(),
                 "encryptionScheme": self.ENCRYPTION_SCHEME,
                 "iv": aes_iv.decode(),
             },
             "name": secret.name,
             "value": value.decode(),
+            "description": secret.description,
         }
 
-        url = self.create_secret_url(secret.name)
         try:
-            response = requests.put(url, headers=self.headers, json=payload)
-            response.raise_for_status()
-        except Exception as e:
-            self.logger.debug(traceback.format_exc())
-            if response.status_code == 403:
-                raise RobocorpVaultError(
-                    "Failed to set secret value. Does your token have write access?"
-                ) from e
-            raise RobocorpVaultError("Failed to set secret value.") from e
+            self._client.put(secret.name, json=payload)
+        except HTTPError as err:
+            if err.status_code == 403:
+                message = "Not authorized to write secret. Is your token valid?"
+            elif err.status_code == 404:
+                message = f"No secret with name '{secret.name}' available"
+            else:
+                message = str(err)
+            raise RobocorpVaultError(message) from err
+        except Exception as err:
+            raise RobocorpVaultError(str(err)) from err
 
     def get_publickey(self) -> bytes:
         """Get the public key for AES encryption with the existing token."""
-        url = self.create_public_key_url()
         try:
-            response = requests.get(url, headers=self.headers)
-            response.raise_for_status()
-        except Exception as e:
-            self.logger.debug(traceback.format_exc())
-            raise RobocorpVaultError(
-                "Failed to fetch public key. Is your token valid?"
-            ) from e
-
-        return response.content
+            response = self._client.get("publicKey")
+            return response.content
+        except HTTPError as err:
+            if err.status_code == 403:
+                message = "Not authorized to read public key. Is your token valid?"
+            else:
+                message = str(err)
+            raise RobocorpVaultError(message) from err
+        except Exception as err:
+            raise RobocorpVaultError(str(err)) from err
 
     @staticmethod
     def _encrypt_secret_value_with_aes(
         secret: SecretContainer,
     ) -> Tuple[bytes, bytes, bytes, bytes]:
         def generate_aes_key() -> Tuple[bytes, bytes]:
             aes_key = AESGCM.generate_key(bit_length=256)
@@ -393,153 +382,7 @@
                 mgf=padding.MGF1(algorithm=hashes.SHA256()),
                 algorithm=hashes.SHA256(),
                 label=None,
             ),
         )
 
         return base64.b64encode(aes_enc)
-
-
-class Vault:
-    """`Vault` is a library for interacting with secrets stored in the ``Robocorp Control Room Vault``.
-
-    Uses ``Robocorp Control Room Vault`` (by default) or file-based secrets, which can be taken
-    into use by setting some environment variables.
-
-    Robocorp Vault relies on environment variables, which are normally set
-    automatically by the Robocorp Work Agent or Assistant when a run is
-    initialized by the Robocorp Control Room. When developing robots locally
-    in VSCode, you can use the `Robocorp Code Extension`_ to set these
-    variables automatically as well.
-
-    Alternatively, you may set these environment variable manually using
-    `rcc`_ or directly in some other fashion. The specific variables which
-    must exist are:
-
-    - ``RC_API_SECRET_HOST``: URL to Robocorp Vault API
-    - ``RC_API_SECRET_TOKEN``: API Token for Robocorp Vault API
-    - ``RC_WORKSPACE_ID``: Control Room Workspace ID
-
-    .. _Robocorp Control Room Vault: https://robocorp.com/docs/development-guide/variables-and-secrets/vault
-    .. _Robocorp Code Extension: https://robocorp.com/docs/developer-tools/visual-studio-code/extension-features#connecting-to-control-room-vault
-    .. _rcc: https://robocorp.com/docs/rcc/workflow
-
-    File-based secrets can be set by defining two environment variables.
-
-    - ``RC_VAULT_SECRET_MANAGER``: FileSecrets
-    - ``RC_VAULT_SECRET_FILE``: Absolute path to the secrets database file
-
-    Example content of local secrets file:
-
-    .. code-block:: json
-
-        {
-            "swaglabs": {
-                "username": "standard_user",
-                "password": "secret_sauce"
-            }
-        }
-
-    OR
-
-    .. code-block:: YAML
-
-        swaglabs:
-            username: standard_user
-            password: secret_sauce
-
-    Example:
-        .. code-block:: python
-
-            VAULT = Vault()
-
-            def reading_secrets():
-                print(f"My secrets: {VAULT.get_secret('swaglabs')}")
-
-            def modifying_secrets():
-                secret = VAULT.get_secret("swaglabs")
-                secret["username"] = "nobody"
-                VAULT.set_secret(secret)
-
-    """  # noqa: E501
-
-    def __init__(self, *args, **kwargs):
-        """The selected adapter can be set with the environment variable.
-
-        Use the environment variable ``RC_VAULT_SECRET_MANAGER``, or the
-        argument ``default_adapter``.
-        Defaults to Robocorp Vault if not defined.
-
-        All other library arguments are passed to the adapter.
-
-        Args:
-            default_adapter: Override default secret adapter
-
-        """
-        self.logger = logging.getLogger(__name__)
-
-        default = kwargs.pop("default_adapter", RobocorpVault)
-        if "RC_VAULT_SECRET_MANAGER" in os.environ:
-            adapter = required_env("RC_VAULT_SECRET_MANAGER", default)
-        elif "RPA_SECRET_MANAGER" in os.environ:  # Backward-compatibility
-            adapter = required_env("RPA_SECRET_MANAGER", default)
-        else:
-            adapter = default
-
-        self._adapter_factory = self._create_factory(adapter, args, kwargs)
-        self._adapter = None
-
-    @property
-    def adapter(self) -> BaseSecretManager:
-        if self._adapter is None:
-            self._adapter = self._adapter_factory()
-
-        return self._adapter
-
-    def _create_factory(self, adapter, args, kwargs):
-        if isinstance(adapter, str):
-            if adapter in ("FileSecrets", "RPA.Robocorp.Vault.FileSecrets"):
-                adapter = FileSecrets
-            else:
-                try:
-                    adapter = import_by_name(adapter, __name__)
-                except Exception as e:
-                    raise ValueError(
-                        f"RC_VAULT_SECRET_MANAGER environment variable seems to "
-                        f"have a wrong value: {adapter!r}.\n"
-                        f'It should be unset to load from Control Room, "FileSecrets" '
-                        f'to load from a file or the name of the "BaseSecretManager" '
-                        f"implementation class."
-                    ) from e
-
-        if not issubclass(adapter, BaseSecretManager):
-            raise ValueError(
-                f"Adapter '{adapter}' does not inherit from BaseSecretManager"
-            )
-
-        def factory():
-            return adapter(*args, **kwargs)
-
-        return factory
-
-    def get_secret(self, secret_name: str) -> SecretContainer:
-        """Read a secret from the configured source, e.g. Robocorp Vault.
-
-        Args:
-            secret_name: Name of secret.
-
-        Returns:
-            `SecretContainer` object.
-        """
-        return self.adapter.get_secret(secret_name)
-
-    def set_secret(self, secret: SecretContainer) -> None:
-        """Overwrite an existing secret with new values.
-
-        Note:
-            Only allows modifying existing secrets, and replaces
-              all values contained within it.
-
-        Args:
-            secret: `SecretContainer` object, from e.g. `get_secret`.
-        """
-        self.adapter.set_secret(secret)
```

### Comparing `robocorp_vault-1.0.0/PKG-INFO` & `robocorp_vault-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: robocorp-vault
-Version: 1.0.0
+Version: 1.1.0
 Summary: Robocorp Control Room Vault API integration library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # Robocorp Control Room Vault API library
 
 `robocorp-vault` is a library which provides read and write access to the
 `Vault` at `Robocorp Control Room`.
 
-
 ## Usage
 
-
 ```python    
 from robocorp import vault
 from robocorp import log 
 
 def reading_secrets():
     secrets_container = vault.get_secret('secret_name')
     # Shows secret keys available:
@@ -50,7 +49,8 @@
 hidden from `robocorp.log` logs (if `robocorp.log` is available
 in the environment), but care needs to be taken when setting it
 so that secrets don't become exposed before being set into the vault.
 
 i.e.: When setting values into the vault, if such values are sensitive,
 use `with robocorp.log.suppress_variables()` so that such value doesn't
 become logged before it's received by the vault.
+
```

