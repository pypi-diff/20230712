# Comparing `tmp/efrem_utils-0.0.1.tar.gz` & `tmp/efrem_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.0.1.tar", max compression
+gzip compressed data, was "efrem_utils-0.0.2.tar", max compression
```

## Comparing `efrem_utils-0.0.1.tar` & `efrem_utils-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      924 2023-07-12 18:17:09.186430 efrem_utils-0.0.1/efrem_utils.py
--rw-r--r--   0        0        0      299 2023-07-10 15:45:49.104139 efrem_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 14:35:13.665232 efrem_utils-0.0.1/README.md
--rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 efrem_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      936 2023-07-12 18:37:07.019654 efrem_utils-0.0.2/efrem_utils.py
+-rw-r--r--   0        0        0      299 2023-07-12 18:39:13.218589 efrem_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-07-12 18:35:53.881437 efrem_utils-0.0.2/README.md
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 efrem_utils-0.0.2/PKG-INFO
```

### Comparing `efrem_utils-0.0.1/efrem_utils.py` & `efrem_utils-0.0.2/efrem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, TypeVar, Iterable
 
 T = TypeVar("T")
 
-def get_validated_input(*_, msg: str, validators: Iterable[tuple[Callable[[str], bool], str | Callable[[str], str] | None]], constructor: Callable[[str], T], precomp: Callable[[str], str] | None = None) -> Callable[[], T]:
+def get_validated_input(*_, msg: str, validators: Iterable[tuple[Callable[[str], bool], str | Callable[[str], str] | None]], constructor: Callable[[str], T] = str, precomp: Callable[[str], str] | None = None) -> Callable[[], T]:
     def inner() -> T:
         while 1:
             buffer: str = precomp(input(msg)) if precomp is not None else input(msg)
             for validator, err_msg in validators:
                 result: bool
                 try:
                     result = validator(buffer)
@@ -15,9 +15,9 @@
 
                 if not result:
                     if err_msg is not None:
                         print(err_msg(buffer) if callable(err_msg) else err_msg.format(buffer=buffer))
                     break
 
             else:
-                return constructor(buffer)
+                return constructor(buffer)      
     return inner
```

