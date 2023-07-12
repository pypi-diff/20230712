# Comparing `tmp/aiochris-0.2.2.tar.gz` & `tmp/aiochris-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.2.2.tar", max compression
+gzip compressed data, was "aiochris-0.3.0rc1.tar", max compression
```

## Comparing `aiochris-0.2.2.tar` & `aiochris-0.3.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-12 18:24:29.663271 aiochris-0.2.2/LICENSE
--rw-r--r--   0        0        0     1738 2023-07-12 18:24:29.663271 aiochris-0.2.2/README.md
--rw-r--r--   0        0        0      574 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6173 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/anon.py
--rw-r--r--   0        0        0     9627 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/authed.py
--rw-r--r--   0        0        0     3723 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/base.py
--rw-r--r--   0        0        0     1707 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/normal.py
--rw-r--r--   0        0        0     2284 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/examples.md
--rw-r--r--   0        0        0     4811 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/home.md
--rw-r--r--   0        0        0       97 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     4969 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/http.py
--rw-r--r--   0        0        0     4664 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/__init__.py
--rw-r--r--   0        0        0     1638 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2912 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/data.py
--rw-r--r--   0        0        0      644 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/enums.py
--rw-r--r--   0        0        0     5061 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/logged_in.py
--rw-r--r--   0        0        0     1128 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/public.py
--rw-r--r--   0        0        0     3118 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/types.py
--rw-r--r--   0        0        0       31 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/__init__.py
--rw-r--r--   0        0        0      698 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/errors.py
--rw-r--r--   0        0        0     6920 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/search.py
--rw-r--r--   0        0        0      782 2023-07-12 18:24:29.663271 aiochris-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 aiochris-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/LICENSE
+-rw-r--r--   0        0        0     1738 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/README.md
+-rw-r--r--   0        0        0      594 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9615 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3718 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/base.py
+-rw-r--r--   0        0        0     1695 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/normal.py
+-rw-r--r--   0        0        0      644 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/enums.py
+-rw-r--r--   0        0        0      698 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/errors.py
+-rw-r--r--   0        0        0     2284 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     4969 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/http.py
+-rw-r--r--   0        0        0     4659 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1631 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2898 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/data.py
+-rw-r--r--   0        0        0     5047 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0     1114 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/types.py
+-rw-r--r--   0        0        0       31 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/util/__init__.py
+-rw-r--r--   0        0        0     6900 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/util/search.py
+-rw-r--r--   0        0        0      785 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 aiochris-0.3.0rc1/PKG-INFO
```

### Comparing `aiochris-0.2.2/LICENSE` & `aiochris-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/README.md` & `aiochris-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/__init__.py` & `aiochris-0.3.0rc1/aiochris/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 import aiochris.client
 import aiochris.models
 import aiochris.util
 from aiochris.util.search import Search, acollect
 from aiochris.client.normal import ChrisClient
 from aiochris.client.anon import AnonChrisClient
 from aiochris.client.admin import ChrisAdminClient
-from aiochris.models.enums import Status, ParameterTypeName
+from aiochris.enums import Status, ParameterTypeName
 
 __all__ = [
     "AnonChrisClient",
     "ChrisClient",
     "ChrisAdminClient",
     "Search",
     "acollect",
     "Status",
     "ParameterTypeName",
     "client",
     "models",
     "util",
+    "errors",
+    "types",
 ]
```

### Comparing `aiochris-0.2.2/aiochris/client/admin.py` & `aiochris-0.3.0rc1/aiochris/client/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from aiochris.link.linked import deserialize_linked
 from aiochris.models.collection_links import (
     AdminCollectionLinks,
     AdminApiCollectionLinks,
 )
 from aiochris.models.logged_in import Plugin
 from aiochris.models.public import ComputeResource
-from aiochris.models.types import PluginUrl, ComputeResourceName, PfconUrl
-from aiochris.util.errors import raise_for_status
+from aiochris.types import PluginUrl, ComputeResourceName, PfconUrl
+from aiochris.errors import raise_for_status
 
 
 class _AdminApiClient(CollectionJsonApiClient[AdminApiCollectionLinks]):
     """
     A client to `/chris-admin/api/v1/`
     """
```

### Comparing `aiochris-0.2.2/aiochris/client/anon.py` & `aiochris-0.3.0rc1/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/client/authed.py` & `aiochris-0.3.0rc1/aiochris/client/authed.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from aiochris.client.base import BaseChrisClient
 from aiochris.client.base import L, CSelf
 from aiochris.link import http
 from aiochris.link.linked import deserialize_res
 from aiochris.models.logged_in import Plugin, File, User, PluginInstance, Feed
 from aiochris.models.public import ComputeResource
-from aiochris.models.types import ChrisURL, Username, Password
-from aiochris.util.errors import IncorrectLoginError, raise_for_status
+from aiochris.types import ChrisURL, Username, Password
+from aiochris.errors import IncorrectLoginError, raise_for_status
 from aiochris.util.search import Search, acollect
 
 
 class AuthenticatedClient(BaseChrisClient[L, CSelf], Generic[L, CSelf], abc.ABC):
     """
     An authenticated ChRIS client.
     """
```

### Comparing `aiochris-0.2.2/aiochris/client/base.py` & `aiochris-0.3.0rc1/aiochris/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import aiohttp
 from serde import from_dict
 
 from aiochris import Search
 from aiochris.link.collection_client import L, CollectionJsonApiClient
 from aiochris.models.public import PublicPlugin
-from aiochris.util.errors import raise_for_status
+from aiochris.errors import raise_for_status
 
 CSelf = TypeVar(
     "CSelf", bound="BaseChrisClient"
 )  # can't wait for `Self` in Python 3.11!
 
 
 class BaseChrisClient(
```

### Comparing `aiochris-0.2.2/aiochris/client/normal.py` & `aiochris-0.3.0rc1/aiochris/client/normal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from contextlib import asynccontextmanager
 from typing import Optional
 
 import aiohttp
 from serde.json import from_json
 
 from aiochris.client.authed import AuthenticatedClient
-from aiochris.util.errors import raise_for_status
+from aiochris.errors import raise_for_status
 from aiochris.models.collection_links import CollectionLinks
 from aiochris.models.data import UserData
-from aiochris.models.types import ChrisURL, Username, Password
+from aiochris.types import ChrisURL, Username, Password
 
 
 class ChrisClient(AuthenticatedClient[CollectionLinks, "ChrisClient"]):
     """
     A normal user *ChRIS* client, who may upload files and create plugin instances.
     """
```

### Comparing `aiochris-0.2.2/aiochris/examples.md` & `aiochris-0.3.0rc1/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/home.md` & `aiochris-0.3.0rc1/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/link/collection_client.py` & `aiochris-0.3.0rc1/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/link/http.py` & `aiochris-0.3.0rc1/aiochris/link/http.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/link/linked.py` & `aiochris-0.3.0rc1/aiochris/link/linked.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AsyncContextManager,
 )
 
 import aiohttp
 import serde
 import yarl
 
-from aiochris.util.errors import raise_for_status, ResponseError
+from aiochris.errors import raise_for_status, ResponseError
 
 T = TypeVar("T")
 
 
 class LinkedMeta(abc.ABCMeta):
     """
     A metaclass for HTTP clients which make requests to URIs
```

### Comparing `aiochris-0.2.2/aiochris/link/metaprog.py` & `aiochris-0.3.0rc1/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/models/collection_links.py` & `aiochris-0.3.0rc1/aiochris/models/collection_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 import functools
 from dataclasses import dataclass
 from typing import Iterator
 
 from serde import deserialize
 
-from aiochris.models.types import ApiUrl, UserUrl, AdminUrl
+from aiochris.types import ApiUrl, UserUrl, AdminUrl
 
 
 @deserialize
 @dataclass(frozen=True)
 class AbstractCollectionLinks:
     @classmethod
     def has_field(cls, field_name: str) -> bool:
```

### Comparing `aiochris-0.2.2/aiochris/models/data.py` & `aiochris-0.3.0rc1/aiochris/models/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from dataclasses import dataclass
 import datetime
 from typing import Optional
 
 from serde import deserialize
 
 from aiochris.link.linked import LinkedModel
-from aiochris.models.enums import PluginType, Status
-from aiochris.models.types import *
+from aiochris.enums import PluginType, Status
+from aiochris.types import *
 
 
 @deserialize
 @dataclass(frozen=True)
 class UserData:
     """A *CUBE* user."""
```

### Comparing `aiochris-0.2.2/aiochris/models/enums.py` & `aiochris-0.3.0rc1/aiochris/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/models/logged_in.py` & `aiochris-0.3.0rc1/aiochris/models/logged_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from typing import Optional
 
 from serde import deserialize
 
 from aiochris.link import http
 from aiochris.link.linked import LinkedModel
 from aiochris.models.data import PluginInstanceData, FeedData, UserData, FeedNoteData
-from aiochris.models.enums import PluginType
+from aiochris.enums import PluginType
 from aiochris.models.public import PublicPlugin
-from aiochris.models.types import *
+from aiochris.types import *
 
 
 @deserialize
 @dataclass(frozen=True)
 class User(UserData, LinkedModel):
     pass  # TODO change_email, change_password
```

### Comparing `aiochris-0.2.2/aiochris/models/public.py` & `aiochris-0.3.0rc1/aiochris/models/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from dataclasses import dataclass
 
 import serde
 from serde import deserialize
 
 from aiochris.link import http
 from aiochris.link.linked import LinkedModel
-from aiochris.models.enums import PluginType
-from aiochris.models.types import *
+from aiochris.enums import PluginType
+from aiochris.types import *
 from aiochris.util.search import Search
 
 
 @deserialize
 @dataclass(frozen=True)
 class ComputeResource:
     url: ApiUrl
```

### Comparing `aiochris-0.2.2/aiochris/models/types.py` & `aiochris-0.3.0rc1/aiochris/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/util/errors.py` & `aiochris-0.3.0rc1/aiochris/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.2/aiochris/util/search.py` & `aiochris-0.3.0rc1/aiochris/util/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,20 @@
     Type,
     AsyncIterable,
     Any,
     Generic,
     AsyncIterator,
 )
 
-import aiohttp
 import yarl
 from serde import deserialize
 from serde.json import from_json
 
 from aiochris.link.linked import deserialize_linked, Linked
-from aiochris.util.errors import (
+from aiochris.errors import (
     BaseClientError,
     raise_for_status,
     NonsenseResponseError,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `aiochris-0.2.2/pyproject.toml` & `aiochris-0.3.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.2.2"
+version = "0.3.0rc1"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aiochris-0.2.2/PKG-INFO` & `aiochris-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.2.2
+Version: 0.3.0rc1
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

