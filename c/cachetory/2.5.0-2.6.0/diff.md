# Comparing `tmp/cachetory-2.5.0.tar.gz` & `tmp/cachetory-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.5.0.tar", max compression
+gzip compressed data, was "cachetory-2.6.0.tar", max compression
```

## Comparing `cachetory-2.5.0.tar` & `cachetory-2.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11355 2023-07-05 12:56:59.698513 cachetory-2.5.0/LICENSE
--rw-r--r--   0        0        0    13890 2023-07-05 12:56:59.702513 cachetory-2.5.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1711 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2476 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1401 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2333 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2171 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     3835 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     3318 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3618 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3452 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      909 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3168 2023-07-05 12:57:12.926631 cachetory-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    15355 1970-01-01 00:00:00.000000 cachetory-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-12 13:13:19.923697 cachetory-2.6.0/LICENSE
+-rw-r--r--   0        0        0    13890 2023-07-12 13:13:19.923697 cachetory-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1711 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2476 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0      993 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     1401 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2333 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2171 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     4241 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3665 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3618 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3452 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      255 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-07-12 13:13:19.923697 cachetory-2.6.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3168 2023-07-12 13:13:35.068556 cachetory-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    15355 1970-01-01 00:00:00.000000 cachetory-2.6.0/PKG-INFO
```

### Comparing `cachetory-2.5.0/LICENSE` & `cachetory-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/README.md` & `cachetory-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/async_/__init__.py` & `cachetory-2.6.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/async_/dummy.py` & `cachetory-2.6.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/async_/memory.py` & `cachetory-2.6.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/async_/redis.py` & `cachetory-2.6.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/sync/__init__.py` & `cachetory-2.6.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/sync/dummy.py` & `cachetory-2.6.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/sync/memory.py` & `cachetory-2.6.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/backends/sync/redis.py` & `cachetory-2.6.0/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/caches/async_.py` & `cachetory-2.6.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/caches/sync.py` & `cachetory-2.6.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/decorators/async_.py` & `cachetory-2.6.0/cachetory/decorators/async_.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,65 +13,79 @@
 from cachetory.private.functools import into_async_callable
 
 P = ParamSpec("P")
 """Original wrapped function parameter specification."""
 
 
 def cached(
-    cache: Cache[ValueT, WireT] | Callable[..., Cache[ValueT, WireT]] | Callable[..., Awaitable[Cache[ValueT, WireT]]],
+    cache: Cache[ValueT, WireT]
+    | Callable[..., Cache[ValueT, WireT] | None]
+    | Callable[..., Awaitable[Cache[ValueT, WireT] | None]]
+    | None,
     *,
     make_key: Callable[..., str] = shared.make_default_key,  # no way to use `P` here
-    time_to_live: timedelta | Callable[..., timedelta] | Callable[..., Awaitable[timedelta]] | None = None,
+    time_to_live: timedelta | Callable[..., timedelta | None] | Callable[..., Awaitable[timedelta]] | None = None,
     if_not_exists: bool = False,
     exclude: Callable[[str, ValueT], bool] | Callable[[str, ValueT], Awaitable[bool]] | None = None,
 ) -> Callable[[Callable[P, Awaitable[ValueT]]], _CachedCallable[P, Awaitable[ValueT]]]:
     """
     Apply memoization to the wrapped callable.
 
     Args:
         cache:
             `Cache` instance or a callable (sync or async) that returns a `Cache` instance for each function call.
             In the latter case the specific callable gets called with a wrapped function as the first argument,
             and the rest of the arguments next to it.
+            If the callable returns `None`, the cache is skipped.
         make_key: callable to generate a custom cache key per each call.
         time_to_live:
             cached value expiration time or a callable (sync or async) that returns the expiration time.
             The callable needs to accept keyword arguments, and it is given the cache key to
             compute the expiration time.
         if_not_exists: controls concurrent sets: if `True` – avoids overwriting a cached value.
         exclude: Optional callable to prevent a key-value pair from being cached if the callable returns true.
     """
 
     def wrap(callable_: Callable[P, Awaitable[ValueT]]) -> _CachedCallable[P, Awaitable[ValueT]]:
         get_cache = into_async_callable(cache)
         get_time_to_live = into_async_callable(time_to_live)
-        exclude_ = into_async_callable(exclude)  # type: ignore[arg-type]
+        exclude_: None | Callable[[str, ValueT], Awaitable[bool]] = (
+            into_async_callable(exclude) if exclude is not None else None
+        )
 
         @wraps(callable_)
         async def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
             cache_ = await get_cache(callable_, *args, **kwargs)
             key_ = make_key(callable_, *args, **kwargs)
-            time_to_live_ = await get_time_to_live(key=key_)
 
-            value = await cache_.get(key_)
+            if cache_ is not None:
+                value = await cache_.get(key_)
+            else:
+                value = None
+
             if value is None:
                 value = await callable_(*args, **kwargs)
-                if exclude is None or not await exclude_(key_, value):
+                if cache_ is not None and (exclude_ is None or not await exclude_(key_, value)):
+                    time_to_live_ = await get_time_to_live(key=key_)
                     await cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
+
             return value
 
         async def purge(*args: P.args, **kwargs: P.kwargs) -> bool:
             """
             Delete the value that was cached using the same call arguments.
 
             Returns:
                 whether a cached value existed
             """
-            key = make_key(callable_, *args, **kwargs)
-            return await (await get_cache(callable_, *args, **kwargs)).delete(key)
+            if (cache := await get_cache(callable_, *args, **kwargs)) is not None:
+                key = make_key(callable_, *args, **kwargs)
+                return await cache.delete(key)
+            else:
+                return False
 
         cached_callable.purge = purge  # type: ignore[attr-defined]
         return cached_callable  # type: ignore[return-value]
 
     return wrap
```

### Comparing `cachetory-2.5.0/cachetory/decorators/shared.py` & `cachetory-2.6.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/decorators/sync.py` & `cachetory-2.6.0/cachetory/decorators/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from contextlib import suppress
 from datetime import timedelta
 from functools import wraps
 from typing import Callable
 
 from typing_extensions import ParamSpec, Protocol
 
 from cachetory.caches.sync import Cache
@@ -13,29 +14,30 @@
 from cachetory.private.functools import into_callable
 
 P = ParamSpec("P")
 """Original wrapped function parameter specification."""
 
 
 def cached(
-    cache: Cache[ValueT, WireT] | Callable[..., Cache[ValueT, WireT]],  # no way to use `P` here
+    cache: Cache[ValueT, WireT] | Callable[..., Cache[ValueT, WireT] | None] | None,  # no way to use `P` here
     *,
     make_key: Callable[..., str] = shared.make_default_key,  # no way to use `P` here
-    time_to_live: timedelta | Callable[..., timedelta] | None = None,
+    time_to_live: timedelta | Callable[..., timedelta | None] | None = None,
     if_not_exists: bool = False,
     exclude: Callable[[str, ValueT], bool] | None = None,
 ) -> Callable[[Callable[P, ValueT]], _CachedCallable[P, ValueT]]:
     """
     Apply memoization to the wrapped callable.
 
     Args:
         cache:
             `Cache` instance or a callable tha returns a `Cache` instance for each function call.
             In the latter case the specified callable gets called with a wrapped function as the first argument,
             and the rest of the arguments next to it.
+            If the callable returns `None`, the cache is skipped.
         make_key: callable to generate a custom cache key per each call.
         time_to_live:
             cached value expiration time or callable that returns the expiration time.
             The callable needs to accept keyword arguments, and it is given the cache key to
             compute the expiration time.
         if_not_exists: controls concurrent sets: if `True` – avoids overwriting a cached value.
         exclude: Optional callable to prevent a key-value pair from being cached if the callable returns true.
@@ -45,27 +47,32 @@
         get_cache = into_callable(cache)
         get_time_to_live = into_callable(time_to_live)
 
         @wraps(callable_)
         def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
             cache_ = get_cache(callable_, *args, **kwargs)
             key_ = make_key(callable_, *args, **kwargs)
-            time_to_live_ = get_time_to_live(key=key_)
 
-            try:
-                value = cache_[key_]
-            except KeyError:
-                value = callable_(*args, **kwargs)
-                if exclude is None or not exclude(key_, value):
-                    cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
+            if cache_ is not None:
+                with suppress(KeyError):
+                    # `KeyError` normally means the value is «non-cached».
+                    return cache_[key_]
+
+            value = callable_(*args, **kwargs)
+            if cache_ is not None and (exclude is None or not exclude(key_, value)):
+                time_to_live_ = get_time_to_live(key=key_)
+                cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
             return value
 
         def purge(*args: P.args, **kwargs: P.kwargs) -> bool:
-            key = make_key(callable_, *args, **kwargs)
-            return get_cache(callable_, *args, **kwargs).delete(key)
+            if (cache := get_cache(callable_, *args, **kwargs)) is not None:
+                key = make_key(callable_, *args, **kwargs)
+                return cache.delete(key)
+            else:
+                return False
 
         cached_callable.purge = purge  # type: ignore[attr-defined]
         return cached_callable  # type: ignore[return-value]
 
     return wrap
```

### Comparing `cachetory-2.5.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.6.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/interfaces/backends/private.py` & `cachetory-2.6.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.6.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/interfaces/serializers.py` & `cachetory-2.6.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/private/functools.py` & `cachetory-2.6.0/cachetory/private/functools.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/chained.py` & `cachetory-2.6.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.6.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/compressors/zstd.py` & `cachetory-2.6.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/json.py` & `cachetory-2.6.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/msgpack.py` & `cachetory-2.6.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/noop.py` & `cachetory-2.6.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/cachetory/serializers/pickle.py` & `cachetory-2.6.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.5.0/pyproject.toml` & `cachetory-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.5.0"
+version = "2.6.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `cachetory-2.5.0/PKG-INFO` & `cachetory-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.5.0
+Version: 2.6.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.0,<4.0.0
```

