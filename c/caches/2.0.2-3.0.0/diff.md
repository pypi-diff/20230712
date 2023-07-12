# Comparing `tmp/caches-2.0.2.tar.gz` & `tmp/caches-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caches-2.0.2.tar", last modified: Tue Oct 19 21:16:51 2021, max compression
+gzip compressed data, was "caches-3.0.0.tar", last modified: Wed Jul 12 20:33:55 2023, max compression
```

## Comparing `caches-2.0.2.tar` & `caches-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2021-10-19 21:16:51.637472 caches-2.0.2/
--rw-r--r--   0 jaymon     (501) staff       (20)     6358 2021-10-19 21:16:51.637142 caches-2.0.2/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     5637 2021-10-12 23:02:53.000000 caches-2.0.2/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2021-10-19 21:16:51.631794 caches-2.0.2/caches/
--rw-r--r--   0 jaymon     (501) staff       (20)     1162 2021-10-13 22:18:50.000000 caches-2.0.2/caches/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-10-10 20:34:09.000000 caches-2.0.2/caches/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)    20701 2021-10-13 22:16:38.000000 caches-2.0.2/caches/core.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2793 2021-10-10 20:34:09.000000 caches-2.0.2/caches/decorators.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4172 2021-10-10 20:34:09.000000 caches-2.0.2/caches/dsn.py
--rw-r--r--   0 jaymon     (501) staff       (20)      144 2021-10-10 20:34:09.000000 caches-2.0.2/caches/exception.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6625 2021-10-13 22:48:37.000000 caches-2.0.2/caches/interface.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2021-10-19 21:16:51.633702 caches-2.0.2/caches.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     6358 2021-10-19 21:16:51.000000 caches-2.0.2/caches.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      394 2021-10-19 21:16:51.000000 caches-2.0.2/caches.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2021-10-19 21:16:51.000000 caches-2.0.2/caches.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       36 2021-10-19 21:16:51.000000 caches-2.0.2/caches.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       13 2021-10-19 21:16:51.000000 caches-2.0.2/caches.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2021-10-19 21:16:51.637559 caches-2.0.2/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1701 2021-10-10 20:34:09.000000 caches-2.0.2/setup.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2021-10-19 21:16:51.636534 caches-2.0.2/tests/
--rw-r--r--   0 jaymon     (501) staff       (20)      638 2021-10-12 22:50:32.000000 caches-2.0.2/tests/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      615 2021-10-12 22:51:02.000000 caches-2.0.2/tests/caches_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)    17713 2021-10-13 22:17:58.000000 caches-2.0.2/tests/core_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3371 2021-10-10 20:34:09.000000 caches-2.0.2/tests/decorators_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1546 2021-10-10 20:34:09.000000 caches-2.0.2/tests/dsn_test.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:33:55.155574 caches-3.0.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1083 2023-07-08 17:00:16.000000 caches-3.0.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     6115 2023-07-12 20:33:55.155451 caches-3.0.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     5388 2023-07-12 20:27:18.000000 caches-3.0.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:33:55.154114 caches-3.0.0/caches/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1162 2023-07-08 20:12:04.000000 caches-3.0.0/caches/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-10-10 20:34:09.000000 caches-3.0.0/caches/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    20976 2023-07-12 20:32:37.000000 caches-3.0.0/caches/core.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2792 2023-07-08 17:11:07.000000 caches-3.0.0/caches/decorators.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4490 2023-07-08 18:06:46.000000 caches-3.0.0/caches/dsn.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      144 2021-10-10 20:34:09.000000 caches-3.0.0/caches/exception.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6199 2023-07-08 17:51:12.000000 caches-3.0.0/caches/interface.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:33:55.154683 caches-3.0.0/caches.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     6115 2023-07-12 20:33:55.000000 caches-3.0.0/caches.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      406 2023-07-12 20:33:55.000000 caches-3.0.0/caches.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-12 20:33:55.000000 caches-3.0.0/caches.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       25 2023-07-12 20:33:55.000000 caches-3.0.0/caches.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       13 2023-07-12 20:33:55.000000 caches-3.0.0/caches.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-12 20:33:55.155617 caches-3.0.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1687 2023-07-08 17:11:22.000000 caches-3.0.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:33:55.155292 caches-3.0.0/tests/
+-rw-r--r--   0 jaymon     (501) staff       (20)      638 2021-10-12 22:50:32.000000 caches-3.0.0/tests/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      615 2021-10-12 22:51:02.000000 caches-3.0.0/tests/caches_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    17816 2023-07-08 19:50:57.000000 caches-3.0.0/tests/core_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3371 2021-10-10 20:34:09.000000 caches-3.0.0/tests/decorators_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1722 2023-07-08 19:29:19.000000 caches-3.0.0/tests/dsn_test.py
```

### Comparing `caches-2.0.2/PKG-INFO` & `caches-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 Metadata-Version: 2.1
 Name: caches
-Version: 2.0.2
+Version: 3.0.0
 Summary: Python caching backed by Redis
 Home-page: http://github.com/jaymon/caches
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # Caches
 
 A Python caching library that gives a similar interface to standard Python data structures like Dict and Set but is backed by [Redis](https://redis.io).
 
 Caches has been used in production for years across many different products, handling millions of requests.
 
 
 ## How to use
 
-Caches can only use [Redis](http://redis.io).
-
 Caches relies on setting the environment variable `CACHES_DSN`:
 
-    caches.interface.Redis://localhost/0
+    redis://localhost/0
 
-If you want to cache things using more than one redis server, you can actually set multiple environment variables:
+If you want to cache things using more than one Redis server, you can actually set multiple environment variables and specify the `caches.interface.Redis` class you want to use:
 
-    export CACHES_DSN_1=caches.interface.Redis://somedomain.com/0#redis1
-    export CACHES_DSN_2=caches.interface.Redis://someotherdomain.com/0#redis2
+    # redis1 uses the standard Redis interface
+    export CACHES_DSN_1=redis://somedomain.com/0#redis1
+    
+    # redis2 uses a custom interface child class
+    export CACHES_DSN_2=custom.interface.Redis://someotherdomain.com/0#redis2
 
 After you've set the environment variable, then you just need to import caches in your code:
 
 ```python
 import caches
 ```
 
-Caches will take care of parsing the url and creating the redis connection, automatically, so after the import Caches will be ready to use.
+Caches will take care of parsing the and DSN urls and creating the associated Redis connections automatically, so after importing, Caches will be ready to use.
 
 
 ### Interface
 
-All caches caching classes have a similar interface, their constructor takes a key and data:
+All Caches caching classes have a similar interface, their constructor takes a key and data:
 
 ```python
 c = Cache(['foo', 'bar', 'che'])
 print c.key # foo.bar.che
 ```
 
 If you would like to init your cache object with a value, use the `data` `**kwarg`:
 
 ```python
 c = Cache('foo', data="boom!")
 print c.key # foo
 print c # "boom!"
 ```
 
-Each caches base caching class is meant to be extended so you can set some parameters:
+Each Caches base caching class is meant to be extended so you can set some parameters:
 
 * **serialize** -- boolean -- True if you want all values pickled, False if you don't (ie, you're caching ints or strings or something).
 
 * **prefix** -- string -- This will be prepended to the key args you pass into the constructor.
 
 * **ttl** -- integer -- time to live, how many seconds to cache the value. 0 (default) means cache forever.
 
-* **connection_name** -- string -- if you have more than one caches dsn then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a dsn url).
+* **connection_name** -- string -- if you have more than one caches DSN then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a DSN url).
 
 ```python
 class MyIntCache(Cache):
   serialize = False # don't bother to serialize values since we're storing ints
   prefix = "MyIntCache" # every key will have this prefix, change to invalidate all currently cached values
   ttl = 7200 # store each int for 2 hours
 ```
@@ -91,40 +92,40 @@
 
 ```python
 c = Cache('foo')
 c.data = 5 # cache 5
 c += 10 # increment 5 by 10, store 15 in the cache
 
 c.clear()
-print c # None
+print(c) # None
 ```
 
 
 #### DictCache
 
 This caching object acts more or less like a Python [dictionary](http://docs.python.org/3/library/stdtypes.html#mapping-types-dict):
 
 ```python
 c = DictCache('foo')
 c['bar'] = 'b'
 c['che'] = 'c'
 for key, val in c.items():
-  print key, val # will print "bar b" and then "che c"
+  print(key, val) # will print "bar b" and then "che c"
 ```
 
 
 #### SetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set):
 
 ```python
 c = SetCache('foo')
 c.add('bar')
 c.add('che')
-print 'che' in c # True
+print('che' in c) # True
 ```
 
 
 #### SortedSetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set) but has some changes:
 
@@ -133,16 +134,16 @@
 * An `rpop()` method allows you to pop the highest score from the set.
 * Iterating through the set results in tuples of `(score, elem)`, not just elem like in a normal set or the `SetCache`.
 
 ```python
 c = SortedSetCache('foo')
 c.add((1, 'bar'))
 c.add((10, 'che'))
-print 'che' in c # True
-print c.pop() # (1, bar)
+print('che' in c) # True
+print(c.pop()) # (1, bar)
 ```
 
 
 #### SentinelCache
 
 Handy for gated access:
 
@@ -205,21 +206,7 @@
 Use pip from pypi:
 
     pip install caches
 
 or from source using pip:
 
     pip install -U "git+https://github.com/jaymon/caches#egg=caches"
-
-
-
-## License
-
-MIT
-
-## Other links
-
-* [redis_collections module](https://github.com/redis-collections/redis-collections) - If you need broader/deeper support for python standard types like dict and set then check out this project. Prior to 2.0.0 Caches had a dependency on this module.
-* [Dogpile](http://dogpilecache.readthedocs.org/en/latest/usage.html)
-
-
-
```

### Comparing `caches-2.0.2/README.md` & `caches-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,60 +3,61 @@
 A Python caching library that gives a similar interface to standard Python data structures like Dict and Set but is backed by [Redis](https://redis.io).
 
 Caches has been used in production for years across many different products, handling millions of requests.
 
 
 ## How to use
 
-Caches can only use [Redis](http://redis.io).
-
 Caches relies on setting the environment variable `CACHES_DSN`:
 
-    caches.interface.Redis://localhost/0
+    redis://localhost/0
 
-If you want to cache things using more than one redis server, you can actually set multiple environment variables:
+If you want to cache things using more than one Redis server, you can actually set multiple environment variables and specify the `caches.interface.Redis` class you want to use:
 
-    export CACHES_DSN_1=caches.interface.Redis://somedomain.com/0#redis1
-    export CACHES_DSN_2=caches.interface.Redis://someotherdomain.com/0#redis2
+    # redis1 uses the standard Redis interface
+    export CACHES_DSN_1=redis://somedomain.com/0#redis1
+    
+    # redis2 uses a custom interface child class
+    export CACHES_DSN_2=custom.interface.Redis://someotherdomain.com/0#redis2
 
 After you've set the environment variable, then you just need to import caches in your code:
 
 ```python
 import caches
 ```
 
-Caches will take care of parsing the url and creating the redis connection, automatically, so after the import Caches will be ready to use.
+Caches will take care of parsing the and DSN urls and creating the associated Redis connections automatically, so after importing, Caches will be ready to use.
 
 
 ### Interface
 
-All caches caching classes have a similar interface, their constructor takes a key and data:
+All Caches caching classes have a similar interface, their constructor takes a key and data:
 
 ```python
 c = Cache(['foo', 'bar', 'che'])
 print c.key # foo.bar.che
 ```
 
 If you would like to init your cache object with a value, use the `data` `**kwarg`:
 
 ```python
 c = Cache('foo', data="boom!")
 print c.key # foo
 print c # "boom!"
 ```
 
-Each caches base caching class is meant to be extended so you can set some parameters:
+Each Caches base caching class is meant to be extended so you can set some parameters:
 
 * **serialize** -- boolean -- True if you want all values pickled, False if you don't (ie, you're caching ints or strings or something).
 
 * **prefix** -- string -- This will be prepended to the key args you pass into the constructor.
 
 * **ttl** -- integer -- time to live, how many seconds to cache the value. 0 (default) means cache forever.
 
-* **connection_name** -- string -- if you have more than one caches dsn then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a dsn url).
+* **connection_name** -- string -- if you have more than one caches DSN then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a DSN url).
 
 ```python
 class MyIntCache(Cache):
   serialize = False # don't bother to serialize values since we're storing ints
   prefix = "MyIntCache" # every key will have this prefix, change to invalidate all currently cached values
   ttl = 7200 # store each int for 2 hours
 ```
@@ -70,40 +71,40 @@
 
 ```python
 c = Cache('foo')
 c.data = 5 # cache 5
 c += 10 # increment 5 by 10, store 15 in the cache
 
 c.clear()
-print c # None
+print(c) # None
 ```
 
 
 #### DictCache
 
 This caching object acts more or less like a Python [dictionary](http://docs.python.org/3/library/stdtypes.html#mapping-types-dict):
 
 ```python
 c = DictCache('foo')
 c['bar'] = 'b'
 c['che'] = 'c'
 for key, val in c.items():
-  print key, val # will print "bar b" and then "che c"
+  print(key, val) # will print "bar b" and then "che c"
 ```
 
 
 #### SetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set):
 
 ```python
 c = SetCache('foo')
 c.add('bar')
 c.add('che')
-print 'che' in c # True
+print('che' in c) # True
 ```
 
 
 #### SortedSetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set) but has some changes:
 
@@ -112,16 +113,16 @@
 * An `rpop()` method allows you to pop the highest score from the set.
 * Iterating through the set results in tuples of `(score, elem)`, not just elem like in a normal set or the `SetCache`.
 
 ```python
 c = SortedSetCache('foo')
 c.add((1, 'bar'))
 c.add((10, 'che'))
-print 'che' in c # True
-print c.pop() # (1, bar)
+print('che' in c) # True
+print(c.pop()) # (1, bar)
 ```
 
 
 #### SentinelCache
 
 Handy for gated access:
 
@@ -184,19 +185,7 @@
 Use pip from pypi:
 
     pip install caches
 
 or from source using pip:
 
     pip install -U "git+https://github.com/jaymon/caches#egg=caches"
-
-
-
-## License
-
-MIT
-
-## Other links
-
-* [redis_collections module](https://github.com/redis-collections/redis-collections) - If you need broader/deeper support for python standard types like dict and set then check out this project. Prior to 2.0.0 Caches had a dependency on this module.
-* [Dogpile](http://dogpilecache.readthedocs.org/en/latest/usage.html)
-
```

### Comparing `caches-2.0.2/caches/__init__.py` & `caches-3.0.0/caches/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SentinelCache,
 )
 from .interface import get_interfaces, get_interface, set_interface
 from .dsn import configure, configure_environ
 from .decorators import cached
 
 
-__version__ = '2.0.2'
+__version__ = '3.0.0'
 
 
 logger = logging.getLogger(__name__)
 
 
 def unsafe_clear(pattern):
     """Clear the keys matching pattern
```

### Comparing `caches-2.0.2/caches/core.py` & `caches-3.0.0/caches/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,27 +41,34 @@
     @classmethod
     def cached(cls, *args, **kwargs):
         """very similar to the generic decorator, except this one you don't have
         to specify the caching class, it will use the class whose method you called"""
         dec = cached(cls, *args, **kwargs)
         return dec
 
-    def __init__(self, key, data=None, **kwargs):
+    def __init__(self, key="", data=None, **kwargs):
         # allow for overriding class value with passed in values
         for k, v in kwargs.items():
             setattr(self, k, v)
 
         self.key = self.normalize_key(key)
         self.update(data)
 
     def normalize_key(self, key):
         if isinstance(key, (basestring, int)):
             key = [key]
         prefixes = [self.normalize_prefix(self.prefix)]
-        return '.'.join(map(String, itertools.chain(prefixes, key)))
+        nkey = '.'.join(
+            map(String, filter(None, itertools.chain(prefixes, key)))
+        )
+
+        if not nkey:
+            raise ValueError("No key")
+
+        return nkey
 
     def normalize_data(self, data):
         return data
 
     def normalize_ttl(self, ttl):
         return int(self.ttl)
 
@@ -91,26 +98,17 @@
         self.interface.delete(self.key)
 
     def update(self, data):
         raise NotImplementedError()
 
     @contextmanager
     def pipeline(self, **kwargs):
-        pipeinfo = getattr(self, "_pipeinfo", {"counter": 0, "pipe": None})
-        pipeinfo["counter"] += 1
-        if not pipeinfo["pipe"]:
-            pipeinfo["pipe"] = self.interface.pipeline()
-            self._pipeinfo = pipeinfo
-
-        yield pipeinfo["pipe"]
-        pipeinfo["counter"] -= 1
-
-        if pipeinfo["counter"] <= 0:
-            pipeinfo["pipe"].execute()
-            del self._pipeinfo
+        with self.interface.pipeline() as pipe:
+            yield pipe
+            r = pipe.execute()
 
 
 class Cache(BaseCache):
     """
     When you think of a traditional caching class, this is the class you most likely
     think of, this will cache a value at a key.
 
@@ -169,14 +167,23 @@
                 pipe.expire(self.key, self.normalize_ttl(self.ttl))
             res = pipe.execute()[0]
 
         res = int(res)
         self._data = res
         return res
 
+    def get(self, *default):
+        data = self.data
+        if data is None and default:
+            data = default[0]
+        return data
+
+    def set(self, data):
+        self.data = data
+
     def __iadd__(self, other):
         self.increment(other)
         return self
 
     def __isub__(self, other):
         self.increment(-other)
         return self
@@ -303,29 +310,41 @@
 
     def setdefault(self, k, default=None):
         if k not in self:
             self[k] = default
 
     def pop(self, k, *default):
         try:
-            # TODO -- I think this could be piped to one request
-            v = self[k]
-            del self[k]
+            with self.pipeline() as pipe:
+                pipe.hget(self.key, k)
+                pipe.hdel(self.key, k)
+                ret = pipe.execute()
+                data = ret[0]
+                if data is None:
+                    if ret[1] == 0:
+                        raise KeyError(k)
+
+                v = self.normalize_data(self.from_interface(data))
 
         except KeyError:
             if default:
                 v = default[0]
             else:
                 raise
         return v
 
     def popitem(self):
-        """unlike the actual dict.popitem, this pops a random item"""
+        """unlike the actual dict.popitem of python >=3.7, this pops a random
+        item
+
+        https://docs.python.org/3/library/stdtypes.html#dict.popitem
+        """
         k = self.interface.hrandfield(self.key, 1)
         if k:
+            k = k[0]
             v = self.pop(k)
             return (String(k), v)
 
         else:
             raise KeyError()
 
     def copy(self):
@@ -335,27 +354,31 @@
 
 class SetCache(BaseCache, set):
     """Membership set backed by redis
 
     https://docs.python.org/3/library/stdtypes.html#set
     https://redis.io/commands#set
     """
-    def add(self, elem):
+    def add(self, elem, **kwargs):
         data = self.to_interface(self.normalize_data(elem))
         with self.pipeline() as pipe:
-            pipe.sadd(self.key, data)
-            if self.ttl:
-                pipe.expire(self.key, self.normalize_ttl(self.ttl))
+            self._add(elem, pipe, **kwargs)
+
+    def _add(self, elem, pipe, **kwargs):
+        data = self.to_interface(self.normalize_data(elem))
+        pipe.sadd(self.key, data)
+        if self.ttl:
+            pipe.expire(self.key, self.normalize_ttl(self.ttl))
 
     def update(self, *data):
-        with self.pipeline():
+        with self.pipeline() as pipe:
             for iterator in data:
                 if iterator:
                     for elem in iterator:
-                        self.add(elem)
+                        self._add(elem, pipe)
 
     def remove(self, elem):
         """Remove element elem from the set. Raises KeyError if elem is not contained in the set."""
         data = self.to_interface(self.normalize_data(elem))
         res = self.interface.srem(self.key, data) # 1 (success) or 0 (failure)
         if not res:
             raise KeyError(elem)
@@ -433,53 +456,55 @@
     http://docs.python.org/2/library/stdtypes.html#set
     http://code.activestate.com/recipes/576694/
     """
     def normalize_score(self, score):
         """normalize the score, this method is called anytime score is added/retrieved"""
         return int(score)
 
-    def add(self, item: tuple, **kwargs):
+    def _add(self, item: tuple, pipe, **kwargs):
         """add an item tuple of (score, elem) to the set
 
         https://redis.io/commands/zadd
 
         :param item: tuple (score, elem)
         :param **kwargs: these are passed to the interface
             xx -- bool, only update elements that already exist. Don't add new elements
             nx -- bool, only add new elements. Don't update aleady existing elements
             lt -- bool, only update existing elem if new score is less than current score
             gt -- bool, only update existing elem if new score is greater than current score
         """
         if isinstance(item, tuple):
             if len(item) != 2:
                 raise ValueError(
-                    "SortedSetCache only accepts (score, elem) tuples, got tuple with {} values".format(
-                        len(item),
-                    )
+                    " ".join([
+                        "SortedSetCache only accepts (score, elem) tuples,",
+                        "got tuple with {} values".format(
+                            len(item),
+                        )
+                    ])
                 )
 
         else:
             raise TypeError(
                 "SortedSetCache only accepts (score, elem) tuples, got {}".format(
                     type(item),
                 )
             )
 
         score, elem = item
         args = [self.key]
         score = self.normalize_score(score)
         data = self.to_interface(self.normalize_data(elem))
-        with self.pipeline() as pipe:
-            # https://github.com/andymccurdy/redis-py/issues/625
-            # https://github.com/redis/redis/pull/1132
-            # https://github.com/redis/redis/issues/1128
-            # https://redis.io/commands/zadd
-            pipe.zadd(self.key, {data: score}, **kwargs)
-            if self.ttl:
-                pipe.expire(self.key, self.normalize_ttl(self.ttl))
+        # https://github.com/andymccurdy/redis-py/issues/625
+        # https://github.com/redis/redis/pull/1132
+        # https://github.com/redis/redis/issues/1128
+        # https://redis.io/commands/zadd
+        pipe.zadd(self.key, {data: score}, **kwargs)
+        if self.ttl:
+            pipe.expire(self.key, self.normalize_ttl(self.ttl))
 
     def remove(self, elem):
         """Remove element elem from the set. Raises KeyError if elem is not contained in the set."""
         data = self.to_interface(self.normalize_data(elem))
         res = self.interface.zrem(self.key, data) # 1 (success) or 0 (failure)
         if not res:
             raise KeyError(elem)
@@ -488,37 +513,29 @@
         """Remove and return an element from the front or back of the set.
         Raises KeyError if the set is empty.
 
         :param desc: bool, False, then return an item from front of set, True then
             return an item from the back of the set
         :returns: tuple (score, elem)
         """
+        if desc:
+            # https://redis.io/commands/zpopmax/
+            ret = self.interface.zpopmax(self.key, 1)
 
-        # redis >=5.0.0
-        #if desc:
-        #    res = self.interface.zpopmax(self.key, 1)
-        #
-        #else:
-        #    res = self.interface.zpopmin(self.key, 1)
-        with self.interface.pipeline() as pipe:
-            pipe.zrange(self.key, 0, 1, desc=desc, withscores=True, score_cast_func=self.normalize_score)
-            if desc:
-                pipe.zremrangebyrank(self.key, -1, -1)
-
-            else:
-                pipe.zremrangebyrank(self.key, 0, 0)
+        else:
+            # https://redis.io/commands/zpopmin/
+            ret = self.interface.zpopmin(self.key, 1)
 
-            ret = pipe.execute()[0]
-            if ret:
-                ret = ret[0]
-                elem = self.normalize_data(self.from_interface(ret[0]))
-                ret = (ret[1], elem)
+        if ret:
+            ret = ret[0]
+            elem = self.normalize_data(self.from_interface(ret[0]))
+            ret = (ret[1], elem)
 
-            else:
-                raise KeyError()
+        else:
+            raise KeyError()
 
         return ret
 
     def rpop(self):
         """convenience method for pop(desc=True), pops from the end of the set instead of the front"""
         return self.pop(desc=True)
```

### Comparing `caches-2.0.2/caches/decorators.py` & `caches-3.0.0/caches/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, division, print_function, absolute_import
 
-from decorators import FuncDecorator, classproperty
+from datatypes import FuncDecorator, classproperty
 
 from .compat import *
 
 
 class cached(FuncDecorator):
     """make caching the return value of a function extremely easy
```

### Comparing `caches-2.0.2/caches/dsn.py` & `caches-3.0.0/caches/dsn.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,34 +24,41 @@
         return self.interface_class(**self.connection_config())
 
     def connection_config(self):
         connection_config = dict(
             host=self.host,
             port=self.port,
             password=self.password,
-            **self.query
+            **self.query_params
         )
         paths = self.paths
         if paths:
             connection_config['db'] = paths[0]
         return connection_config
 
     def configure(self):
+        # https://redis.readthedocs.io/en/stable/examples/ssl_connection_examples.html#Connecting-to-a-Redis-instance-via-SSL.
+        if "rediss" in self.scheme:
+            self.query_params["ssl"] = True
+            #self.query_params["ssl_cert_reqs"] = "none"
+
         self.scheme = self.configure_scheme(self.scheme)
         self.password = self.configure_password(self.username, self.password)
 
         if not self.port:
             self.port = 6379
 
-        self.query["socket_timeout"] = float(self.query.get("socket_timeout", 1.0))
+        self.query_params["socket_timeout"] = float(
+            self.query_params.get("socket_timeout", 1.0)
+        )
 
     def configure_scheme(self, v):
         ret = v
         d = {
-            "caches.interface.Redis": set(["redis"]),
+            "caches.interface.Redis": set(["redis", "rediss"]),
         }
 
         kv = v.lower()
         for interface_name, vals in d.items():
             if kv in vals:
                 ret = interface_name
                 break
```

### Comparing `caches-2.0.2/caches/interface.py` & `caches-3.0.0/caches/interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, division, print_function, absolute_import
 import logging
 
 import redis
-from redis.client import Pipeline, Script
+from redis.client import Pipeline
+from redis.commands.core import Script
+from datatypes import LogMixin
 
 from .compat import *
 from .exception import CacheError
 
 
 logger = logging.getLogger(__name__)
 
@@ -35,54 +37,51 @@
     """
     don't want to bother with a dsn? Use this method to make an interface available
     """
     if not interface:
         raise ValueError('interface is empty')
 
     global interfaces
-    logger.debug('connection_name: "{}" -> {}.{}'.format(name, interface.__module__, interface.__class__.__name__))
+    logger.debug('connection_name: "{}" -> {}.{}'.format(
+        name,
+        interface.__module__,
+        interface.__class__.__name__
+    ))
     interfaces[name] = interface
 
 
-class RedisMixin(object):
-    log_key = set(['DEL', 'DUMP', 'EXISTS', 'EXPIRE', 'EXPIREAT', 'MOVE', 'PERSIST',
-                'PEXPIRE', 'PEXPIREAT', 'PTTL', 'RENAME', 'RENAMENX', 'RESTORE',
-                'SORT', 'TTL', 'TYPE', 'HGETALL', 'HKEYS', 'HLEN', 'HVALS', 'SADD',
-                'SCARD', 'SISMEMBER', 'SMEMBERS', 'SPOP', 'SRANDMEMBER', 'SREM', 'ZADD',
-                'ZCARD', 'ZCOUNT', 'ZINCRBY', 'ZRANGE', 'ZRANGEBYSCORE', 'ZRANK', 'ZREM',
-                'ZREMRANGEBYRANK', 'ZREMRANGEBYSCORE', 'ZREVRANGE', 'ZREVRANGEBYSCORE', 
-                'ZREVRANK', 'ZSCORE', 'APPEND', 'BITCOUNT', 'BITOP', 'DECR', 'DECRBY', 
-                'GET', 'GETBIT', 'GETRANGE', 'GETSET', 'INCR', 'INCRBY', 'INCRBYFLOAT',
-                'MGET', 'MSET', 'MSETNX', 'PSETEX', 'SET', 'SETBIT', 'SETEX', 'SETNX',
-                'SETRANGE', 'STRLEN'
-              ])
-
-    log_key_field = set(['HDEL', 'HEXISTS', 'HGET', 'HINCRBY', 'HINCRBYFLOAT', 'HSET', 'HSETNX'])
+class RedisMixin(LogMixin):
+    log_key = set([
+        'DEL', 'DUMP', 'EXISTS', 'EXPIRE', 'EXPIREAT', 'MOVE', 'PERSIST',
+        'PEXPIRE', 'PEXPIREAT', 'PTTL', 'RENAME', 'RENAMENX', 'RESTORE',
+        'SORT', 'TTL', 'TYPE', 'HGETALL', 'HKEYS', 'HLEN', 'HVALS', 'SADD',
+        'SCARD', 'SISMEMBER', 'SMEMBERS', 'SPOP', 'SRANDMEMBER', 'SREM',
+        'ZADD', 'ZCARD', 'ZCOUNT', 'ZINCRBY', 'ZRANGE', 'ZRANGEBYSCORE',
+        'ZRANK', 'ZREM', 'ZREMRANGEBYRANK', 'ZREMRANGEBYSCORE', 'ZREVRANGE',
+        'ZREVRANGEBYSCORE', 'ZREVRANK', 'ZSCORE', 'APPEND', 'BITCOUNT', 'BITOP',
+        'DECR', 'DECRBY', 'GET', 'GETBIT', 'GETRANGE', 'GETSET', 'INCR',
+        'INCRBY', 'INCRBYFLOAT', 'MGET', 'MSET', 'MSETNX', 'PSETEX', 'SET',
+        'SETBIT', 'SETEX', 'SETNX', 'SETRANGE', 'STRLEN',
+    ])
+
+    log_key_field = set(['HDEL',
+        'HEXISTS',
+        'HGET',
+        'HINCRBY',
+        'HINCRBYFLOAT',
+        'HSET',
+        'HSETNX'
+    ])
 
     log_script = set(['EVALSHA'])
 
-    def log(self, format_str, *format_args, **log_options):
-        """
-        wrapper around the module's logger
-
-        format_str -- string -- the message to log
-        *format_args -- list -- if format_str is a string containing {}, then format_str.format(*format_args) is ran
-        **log_options --
-            level -- something like logging.DEBUG
-        """
-        log_level = log_options.get('level', logging.DEBUG)
-        if logger.isEnabledFor(log_level):
-            if format_args:
-                logger.log(log_level, format_str.format(*format_args))
-            else:
-                logger.log(log_level, format_str)
-
     def log_call(self, args, res, is_pipe=False, **log_options):
         log_level = log_options.get('level', logging.DEBUG)
-        if not logger.isEnabledFor(log_level): return
+        if not self.is_logging(log_level): return
+        #if not logger.isEnabledFor(log_level): return
 
         format_log = '{} QUEUED' if is_pipe else '{}'
         format_args = []
 
         if args[0] in self.log_key:
             format_log += ' - {}'
             format_args.append(args[0])
@@ -145,20 +144,28 @@
 
         return pipeline
 
 
 class RedisPipeline(RedisMixin, Pipeline):
     def _execute_pipeline(self, connection, commands, raise_on_error):
         self.log('Execute {} Pipeline commands', len(commands))
-        res = super(RedisPipeline, self)._execute_pipeline(connection, commands, raise_on_error)
+        res = super(RedisPipeline, self)._execute_pipeline(
+            connection,
+            commands,
+            raise_on_error
+        )
         return res
 
     def _execute_transaction(self, connection, commands, raise_on_error):
         self.log('Execute {} Transaction commands', len(commands))
-        res = super(RedisPipeline, self)._execute_transaction(connection, commands, raise_on_error)
+        res = super(RedisPipeline, self)._execute_transaction(
+            connection,
+            commands,
+            raise_on_error
+        )
         return res
 
     def execute_command(self, *args, **kwargs):
         res = super(RedisPipeline, self).execute_command(*args, **kwargs)
         self.log_call(args, res, is_pipe=True)
         return res
```

### Comparing `caches-2.0.2/caches.egg-info/PKG-INFO` & `caches-3.0.0/caches.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 Metadata-Version: 2.1
 Name: caches
-Version: 2.0.2
+Version: 3.0.0
 Summary: Python caching backed by Redis
 Home-page: http://github.com/jaymon/caches
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # Caches
 
 A Python caching library that gives a similar interface to standard Python data structures like Dict and Set but is backed by [Redis](https://redis.io).
 
 Caches has been used in production for years across many different products, handling millions of requests.
 
 
 ## How to use
 
-Caches can only use [Redis](http://redis.io).
-
 Caches relies on setting the environment variable `CACHES_DSN`:
 
-    caches.interface.Redis://localhost/0
+    redis://localhost/0
 
-If you want to cache things using more than one redis server, you can actually set multiple environment variables:
+If you want to cache things using more than one Redis server, you can actually set multiple environment variables and specify the `caches.interface.Redis` class you want to use:
 
-    export CACHES_DSN_1=caches.interface.Redis://somedomain.com/0#redis1
-    export CACHES_DSN_2=caches.interface.Redis://someotherdomain.com/0#redis2
+    # redis1 uses the standard Redis interface
+    export CACHES_DSN_1=redis://somedomain.com/0#redis1
+    
+    # redis2 uses a custom interface child class
+    export CACHES_DSN_2=custom.interface.Redis://someotherdomain.com/0#redis2
 
 After you've set the environment variable, then you just need to import caches in your code:
 
 ```python
 import caches
 ```
 
-Caches will take care of parsing the url and creating the redis connection, automatically, so after the import Caches will be ready to use.
+Caches will take care of parsing the and DSN urls and creating the associated Redis connections automatically, so after importing, Caches will be ready to use.
 
 
 ### Interface
 
-All caches caching classes have a similar interface, their constructor takes a key and data:
+All Caches caching classes have a similar interface, their constructor takes a key and data:
 
 ```python
 c = Cache(['foo', 'bar', 'che'])
 print c.key # foo.bar.che
 ```
 
 If you would like to init your cache object with a value, use the `data` `**kwarg`:
 
 ```python
 c = Cache('foo', data="boom!")
 print c.key # foo
 print c # "boom!"
 ```
 
-Each caches base caching class is meant to be extended so you can set some parameters:
+Each Caches base caching class is meant to be extended so you can set some parameters:
 
 * **serialize** -- boolean -- True if you want all values pickled, False if you don't (ie, you're caching ints or strings or something).
 
 * **prefix** -- string -- This will be prepended to the key args you pass into the constructor.
 
 * **ttl** -- integer -- time to live, how many seconds to cache the value. 0 (default) means cache forever.
 
-* **connection_name** -- string -- if you have more than one caches dsn then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a dsn url).
+* **connection_name** -- string -- if you have more than one caches DSN then you can use this to set the name of the connection you want (the name of the connection is the `#connection_name` fragment of a DSN url).
 
 ```python
 class MyIntCache(Cache):
   serialize = False # don't bother to serialize values since we're storing ints
   prefix = "MyIntCache" # every key will have this prefix, change to invalidate all currently cached values
   ttl = 7200 # store each int for 2 hours
 ```
@@ -91,40 +92,40 @@
 
 ```python
 c = Cache('foo')
 c.data = 5 # cache 5
 c += 10 # increment 5 by 10, store 15 in the cache
 
 c.clear()
-print c # None
+print(c) # None
 ```
 
 
 #### DictCache
 
 This caching object acts more or less like a Python [dictionary](http://docs.python.org/3/library/stdtypes.html#mapping-types-dict):
 
 ```python
 c = DictCache('foo')
 c['bar'] = 'b'
 c['che'] = 'c'
 for key, val in c.items():
-  print key, val # will print "bar b" and then "che c"
+  print(key, val) # will print "bar b" and then "che c"
 ```
 
 
 #### SetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set):
 
 ```python
 c = SetCache('foo')
 c.add('bar')
 c.add('che')
-print 'che' in c # True
+print('che' in c) # True
 ```
 
 
 #### SortedSetCache
 
 This caching object acts more or less like a Python [set](http://docs.python.org/2/library/stdtypes.html#set) but has some changes:
 
@@ -133,16 +134,16 @@
 * An `rpop()` method allows you to pop the highest score from the set.
 * Iterating through the set results in tuples of `(score, elem)`, not just elem like in a normal set or the `SetCache`.
 
 ```python
 c = SortedSetCache('foo')
 c.add((1, 'bar'))
 c.add((10, 'che'))
-print 'che' in c # True
-print c.pop() # (1, bar)
+print('che' in c) # True
+print(c.pop()) # (1, bar)
 ```
 
 
 #### SentinelCache
 
 Handy for gated access:
 
@@ -205,21 +206,7 @@
 Use pip from pypi:
 
     pip install caches
 
 or from source using pip:
 
     pip install -U "git+https://github.com/jaymon/caches#egg=caches"
-
-
-
-## License
-
-MIT
-
-## Other links
-
-* [redis_collections module](https://github.com/redis-collections/redis-collections) - If you need broader/deeper support for python standard types like dict and set then check out this project. Prior to 2.0.0 Caches had a dependency on this module.
-* [Dogpile](http://dogpilecache.readthedocs.org/en/latest/usage.html)
-
-
-
```

### Comparing `caches-2.0.2/setup.py` & `caches-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 setup(
     version=version,
     description='Python caching backed by Redis',
     author='Jay Marcyes',
     author_email='jay@marcyes.com',
     url='http://github.com/jaymon/{}'.format(name),
     license="MIT",
-    install_requires=['redis', 'dsnparse', 'decorators', 'datatypes'],
+    install_requires=['redis', 'dsnparse', 'datatypes'],
     #tests_require=['testdata'],
     classifiers=[ # https://pypi.python.org/pypi?:action=list_classifiers
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `caches-2.0.2/tests/__init__.py` & `caches-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caches-2.0.2/tests/caches_test.py` & `caches-3.0.0/tests/caches_test.py`

 * *Files identical despite different names*

### Comparing `caches-2.0.2/tests/core_test.py` & `caches-3.0.0/tests/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, division, print_function, absolute_import
 import sys
 import time
 import random
 
-from . import TestCase
+from datatypes import Version
 
 import caches
 from caches.compat import *
 from caches.core import (
     Cache,
     DictCache,
     SetCache,
     SortedSetCache,
     SentinelCache,
 )
 
+from . import TestCase
+
 
 class CacheTest(TestCase):
     def test_lifecycle(self):
         key = "c.lifecycle"
         c = Cache(key)
         self.assertIsNone(c.data)
 
@@ -262,31 +264,33 @@
 
         self.assertIsNone(d.get("foo"))
         self.assertEqual(1, d.get("foo", 1))
 
         d["foo"] = 2
         self.assertEqual(2, d.get("foo", 1))
 
-    def test_pop(self):
+    def test_pop_1(self):
         d = DictCache("pop")
 
         with self.assertRaises(KeyError):
             d.pop("foo")
 
         self.assertIsNone(d.pop("foo", None))
         self.assertEqual(1, d.pop("foo", 1))
 
         d["foo"] = 2
         self.assertEqual(2, d.pop("foo", 1))
         self.assertFalse("foo" in d)
 
     def test_popitem(self):
-        self.skip_test("This only works on Redis >=6.2")
         d = DictCache("popitem")
 
+        if Version(d.interface.info()["redis_version"]) < "6.2":
+            self.skip_test("This only works on Redis >=6.2")
+
         with self.assertRaises(KeyError):
             d.popitem()
 
         d["foo"] = 2
         self.assertEqual(("foo", 2), d.popitem())
         self.assertFalse("foo" in d)
```

### Comparing `caches-2.0.2/tests/decorators_test.py` & `caches-3.0.0/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `caches-2.0.2/tests/dsn_test.py` & `caches-3.0.0/tests/dsn_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 
 class DSNTest(TestCase):
     def test_scheme(self):
         dsn = DSN('redis://host:1234/dbname#connection_name')
         self.assertFalse("redis" in dsn.scheme)
 
+        dsn = DSN('rediss://host:1234/dbname#connection_name')
+        self.assertFalse("rediss" in dsn.scheme)
+        self.assertTrue(dsn.connection_config()["ssl"])
+
     def test_password(self):
         dsn = DSN('redis://password@host:1234/dbname')
         self.assertTrue("password", dsn.password)
 
         dsn = DSN('redis://username:password@host:1234/dbname')
         self.assertTrue("password", dsn.password)
 
@@ -31,15 +35,15 @@
 
         i = dsn.interface()
         self.assertTrue(i)
 
     def test_defaults(self):
         dsn = DSN("redis://localhost?socket_timeout=1")
         self.assertEqual(6379, dsn.port)
-        self.assertEqual(1.0, dsn.query["socket_timeout"])
+        self.assertEqual(1.0, dsn.query_params["socket_timeout"])
 
 
 class ConfigureTest(TestCase):
     def test_configure(self):
         with self.assertRaises(KeyError):
             i = caches.get_interface('connection_name')
```

