# Comparing `tmp/cachetory-2.6.0.tar.gz` & `tmp/cachetory-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.6.0.tar", max compression
+gzip compressed data, was "cachetory-2.7.0.tar", max compression
```

## Comparing `cachetory-2.6.0.tar` & `cachetory-2.7.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0    11355 2023-07-12 13:13:19.923697 cachetory-2.6.0/LICENSE
--rw-r--r--   0        0        0    13890 2023-07-12 13:13:19.923697 cachetory-2.6.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1711 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2476 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1401 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2333 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2171 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     4241 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     3665 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3618 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3452 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      909 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3168 2023-07-12 13:13:35.068556 cachetory-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    15355 1970-01-01 00:00:00.000000 cachetory-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-12 15:16:14.500930 cachetory-2.7.0/LICENSE
+-rw-r--r--   0        0        0    14352 2023-07-12 15:16:14.500930 cachetory-2.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     2385 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/django.py
+-rw-r--r--   0        0        0     1520 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1718 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2476 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0     1266 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     2220 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/django.py
+-rw-r--r--   0        0        0     1408 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2340 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2201 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     4241 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3665 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3959 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3489 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      481 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3235 2023-07-12 15:16:28.077126 cachetory-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    15899 1970-01-01 00:00:00.000000 cachetory-2.7.0/PKG-INFO
```

### Comparing `cachetory-2.6.0/LICENSE` & `cachetory-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/README.md` & `cachetory-2.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -204,14 +204,24 @@
 | Sync                                    | Async                                     |
 |:----------------------------------------|:------------------------------------------|
 | `cachetory.backends.sync.DummyBackend`  | `cachetory.backends.async_.DummyBackend`  |
 
 Dummy backend that always succeeds but never stores anything. Any values get forgotten immediately,
 and operations behave as if the cache always is empty.
 
+### Django
+
+![scheme: django](https://img.shields.io/badge/scheme-django://-important)
+
+| Sync                                    | Async                                     |
+|:----------------------------------------|:------------------------------------------|
+| `cachetory.backends.sync.DjangoBackend` | `cachetory.backends.async_.DjangoBackend` |
+
+Adapter for the Django cache framework: allows using a pre-configured Django cache for Cachetory's `Cache`.
+
 ## Supported serializers
 
 ### Pickle
 
 ![scheme: pickle](https://img.shields.io/badge/scheme-pickle://-important)
 
 Serializes using the standard [`pickle`](https://docs.python.org/3/library/pickle.html) module.
```

### Comparing `cachetory-2.6.0/cachetory/backends/async_/__init__.py` & `cachetory-2.7.0/cachetory/backends/sync/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from urllib.parse import urlparse
 
-from cachetory.interfaces.backends.async_ import AsyncBackend
+from cachetory.interfaces.backends.sync import SyncBackend
 
 from .dummy import DummyBackend
 from .memory import MemoryBackend
 
 try:
-    # noinspection PyUnresolvedReferences
     from .redis import RedisBackend
 except ImportError:
-    _is_redis_available = False
-else:
-    _is_redis_available = True
+    RedisBackend = None  # type: ignore[assignment, misc]
+
+try:
+    from .django import DjangoBackend
+except ImportError:
+    DjangoBackend = None  # type: ignore[assignment, misc]
 
 
-def from_url(url: str) -> AsyncBackend:
+def from_url(url: str) -> SyncBackend:
     """
-    Create an asynchronous backend from the given URL.
+    Create a synchronous backend from the given URL.
 
     Examples:
         >>> from_url("redis://localhost:6379")
     """
     parsed_url = urlparse(url)
     scheme = parsed_url.scheme
     if scheme == "memory":
         return MemoryBackend.from_url(url)
     if scheme in ("redis", "rediss", "redis+unix"):
-        if not _is_redis_available:
+        if RedisBackend is None:
             raise ValueError(f"`{scheme}://` requires `cachetory[redis]` extra")  # pragma: no cover
         return RedisBackend.from_url(url)
     if scheme == "dummy":
         return DummyBackend.from_url(url)
+    if scheme == "django":
+        if DjangoBackend is None:
+            raise ValueError(f"`{scheme}://` requires `cachetory[django]` extra")  # pragma: no cover
+        return DjangoBackend.from_url(url)
     raise ValueError(f"`{scheme}://` is not supported")
```

### Comparing `cachetory-2.6.0/cachetory/backends/async_/dummy.py` & `cachetory-2.7.0/cachetory/backends/async_/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cachetory.interfaces.backends.private import WireT
 
 
 class DummyBackend(AsyncBackend[WireT], Generic[WireT]):
     """Dummy backend that stores nothing."""
 
     @classmethod
-    def from_url(cls, url: str) -> DummyBackend:
+    def from_url(cls, url: str) -> DummyBackend[WireT]:
         return DummyBackend()
 
     async def get(self, key: str) -> WireT:  # pragma: no cover
         raise KeyError(key)
 
     async def get_many(self, *keys: str) -> AsyncIterable[tuple[str, WireT]]:
         for _ in ():  # pragma: no cover
```

### Comparing `cachetory-2.6.0/cachetory/backends/async_/memory.py` & `cachetory-2.7.0/cachetory/backends/async_/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class MemoryBackend(AsyncBackend[WireT], Generic[WireT]):
     """Memory backend that stores everything in a local dictionary."""
 
     __slots__ = ("_inner",)
 
     @classmethod
-    def from_url(cls, _url: str) -> MemoryBackend:
+    def from_url(cls, _url: str) -> MemoryBackend[WireT]:
         return MemoryBackend()
 
     def __init__(self) -> None:
         # We'll simply delegate call to the wrapped backend.
         self._inner: SyncMemoryBackend = SyncMemoryBackend()
 
     def get(self, key: str) -> Coroutine[Any, Any, WireT]:
```

### Comparing `cachetory-2.6.0/cachetory/backends/async_/redis.py` & `cachetory-2.7.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/backends/sync/dummy.py` & `cachetory-2.7.0/cachetory/backends/sync/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cachetory.interfaces.backends.sync import SyncBackend
 
 
 class DummyBackend(SyncBackend[WireT], Generic[WireT]):
     """Dummy backend that stores nothing."""
 
     @classmethod
-    def from_url(cls, url: str) -> DummyBackend:
+    def from_url(cls, url: str) -> DummyBackend[WireT]:
         return DummyBackend()
 
     def get(self, key: str) -> WireT:  # pragma: no cover
         raise KeyError(key)
 
     def get_many(self, *keys: str) -> Iterable[tuple[str, WireT]]:  # pragma: no cover
         return []
```

### Comparing `cachetory-2.6.0/cachetory/backends/sync/memory.py` & `cachetory-2.7.0/cachetory/backends/sync/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class MemoryBackend(SyncBackend[WireT], Generic[WireT]):
     """Memory backend that stores everything in a local dictionary."""
 
     __slots__ = ("_entries",)
 
     @classmethod
-    def from_url(cls, _url: str) -> MemoryBackend:
+    def from_url(cls, _url: str) -> MemoryBackend[WireT]:
         return MemoryBackend()
 
     def __init__(self) -> None:
         self._entries: dict[str, _Entry[WireT]] = {}
 
     def get(self, key: str) -> WireT:
         return self._get_entry(key).value
```

### Comparing `cachetory-2.6.0/cachetory/backends/sync/redis.py` & `cachetory-2.7.0/cachetory/backends/sync/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from cachetory.interfaces.backends.sync import SyncBackend
 
 
 class RedisBackend(SyncBackend[bytes]):
     """Synchronous Redis backend."""
 
+    __slots__ = ("_client",)
+
     @classmethod
     def from_url(cls, url: str) -> RedisBackend:
         if url.startswith("redis+"):
             url = url[6:]
         return cls(Redis.from_url(url))
 
     def __init__(self, client: Redis) -> None:
```

### Comparing `cachetory-2.6.0/cachetory/caches/async_.py` & `cachetory-2.7.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/caches/sync.py` & `cachetory-2.7.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/decorators/async_.py` & `cachetory-2.7.0/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/decorators/shared.py` & `cachetory-2.7.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/decorators/sync.py` & `cachetory-2.7.0/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.7.0/cachetory/interfaces/backends/async_.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 Note, that some methods provide reasonable default implementation,
 but implementors SHOULD override them for the sake of performance.
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from contextlib import AbstractAsyncContextManager
+from contextlib import AbstractAsyncContextManager, AbstractContextManager
 from datetime import datetime, timedelta, timezone
 from typing import AsyncIterable, Generic, Iterable
 
-from typing_extensions import Protocol
+from typing_extensions import Never, Protocol
 
 from cachetory.interfaces.backends.private import WireT, WireT_co, WireT_contra
 
 
 class AsyncBackendRead(Protocol[WireT_co]):
     """Describes the read operations of an asynchronous cache."""
 
@@ -71,14 +71,16 @@
         """
         Put the value into the cache.
 
         Returns:
             `True` if the value has been successfully set, `False` when `if_not_exists` is true
             and the key is already existing.
         """
+
+        # TODO: just return `None`.
         raise NotImplementedError
 
     async def set_many(self, items: Iterable[tuple[str, WireT_contra]]) -> None:
         """Put all the specified values to the cache."""
         for key, value in items:
             await self.set(key, value)
 
@@ -93,14 +95,15 @@
 
     async def clear(self) -> None:  # pragma: no cover
         """Clear the backend storage."""
         raise NotImplementedError
 
 
 class AsyncBackend(
+    AbstractContextManager,
     AbstractAsyncContextManager,
     AsyncBackendRead[WireT],
     AsyncBackendWrite[WireT],
     Generic[WireT],
     metaclass=ABCMeta,
 ):
     """Generic asynchronous cache backend."""
@@ -112,9 +115,15 @@
         Create an asynchronous cache backend from the specified URL.
 
         Returns:
             An instance of the specific backend class.
         """
         raise NotImplementedError
 
+    def __enter__(self) -> Never:
+        raise RuntimeError("use async context manager protocol instead")
+
+    def __exit__(self, _exc_type, _exc_val, _exc_tb) -> Never:
+        raise RuntimeError("use async context manager protocol instead")
+
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         return None
```

### Comparing `cachetory-2.6.0/cachetory/interfaces/backends/private.py` & `cachetory-2.7.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.7.0/cachetory/interfaces/backends/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         """
         Put the value into the cache.
 
         Returns:
             `True` if the value has been successfully set, `False` when `if_not_exists` is true
             and the key is already existing.
         """
+
+        # TODO: just return `None`.
         raise NotImplementedError
 
     def set_many(self, items: Iterable[tuple[str, WireT_contra]]) -> None:
         """Put all the specified values to the cache."""
         for key, value in items:
             self.set(key, value)
```

### Comparing `cachetory-2.6.0/cachetory/interfaces/serializers.py` & `cachetory-2.7.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/private/functools.py` & `cachetory-2.7.0/cachetory/private/functools.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/chained.py` & `cachetory-2.7.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.7.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/compressors/zstd.py` & `cachetory-2.7.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/json.py` & `cachetory-2.7.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/msgpack.py` & `cachetory-2.7.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/noop.py` & `cachetory-2.7.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/cachetory/serializers/pickle.py` & `cachetory-2.7.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.6.0/pyproject.toml` & `cachetory-2.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.6.0"
+version = "2.7.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -29,38 +29,40 @@
 ]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
+django = {version = "^4.0.0", optional = true}
+ormsgpack = {version = "^1.2.6", optional = true, markers = "platform_python_implementation == 'CPython'"}
 pydantic = "^1.10.4"
-typing-extensions = "^4.4.0"
+python = "^3.8.0"
 redis = {version = "^4.4.2", optional = true}
+typing-extensions = "^4.4.0"
 zstd = {version = "^1.5.2.6", optional = true}
-ormsgpack = {version = "^1.2.6", optional = true, markers = "platform_python_implementation == 'CPython'"}
 
 [tool.poetry.extras]
+django = ["django"]
+ormsgpack = ["ormsgpack"]
 redis = ["redis"]
 zstd = ["zstd"]
-ormsgpack = ["ormsgpack"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.3.0"
 black = "^23.1.0"
-ruff = "^0.0.275"
+freezegun = "^1.2.2"
+mypy = "^1.3.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.275"
 types-redis = "^4.4.0.4"
-freezegun = "^1.2.2"
 
 [tool.black]
 line-length = 120
 target_version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.ruff]
 line-length = 120
```

### Comparing `cachetory-2.6.0/PKG-INFO` & `cachetory-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.6.0
+Version: 2.7.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -18,17 +18,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
+Provides-Extra: django
 Provides-Extra: ormsgpack
 Provides-Extra: redis
 Provides-Extra: zstd
+Requires-Dist: django (>=4.0.0,<5.0.0) ; extra == "django"
 Requires-Dist: ormsgpack (>=1.2.6,<2.0.0) ; (platform_python_implementation == "CPython") and (extra == "ormsgpack")
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: redis (>=4.4.2,<5.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: zstd (>=1.5.2.6,<2.0.0.0) ; extra == "zstd"
 Project-URL: Repository, https://github.com/kpn/cachetory
 Description-Content-Type: text/markdown
@@ -239,14 +241,24 @@
 | Sync                                    | Async                                     |
 |:----------------------------------------|:------------------------------------------|
 | `cachetory.backends.sync.DummyBackend`  | `cachetory.backends.async_.DummyBackend`  |
 
 Dummy backend that always succeeds but never stores anything. Any values get forgotten immediately,
 and operations behave as if the cache always is empty.
 
+### Django
+
+![scheme: django](https://img.shields.io/badge/scheme-django://-important)
+
+| Sync                                    | Async                                     |
+|:----------------------------------------|:------------------------------------------|
+| `cachetory.backends.sync.DjangoBackend` | `cachetory.backends.async_.DjangoBackend` |
+
+Adapter for the Django cache framework: allows using a pre-configured Django cache for Cachetory's `Cache`.
+
 ## Supported serializers
 
 ### Pickle
 
 ![scheme: pickle](https://img.shields.io/badge/scheme-pickle://-important)
 
 Serializes using the standard [`pickle`](https://docs.python.org/3/library/pickle.html) module.
```

