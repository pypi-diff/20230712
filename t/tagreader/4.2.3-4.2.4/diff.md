# Comparing `tmp/tagreader-4.2.3.tar.gz` & `tmp/tagreader-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.2.3.tar", max compression
+gzip compressed data, was "tagreader-4.2.4.tar", max compression
```

## Comparing `tagreader-4.2.3.tar` & `tagreader-4.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.3/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.3/README.md
--rw-r--r--   0        0        0     1633 2023-07-12 11:49:21.921486 tagreader-4.2.3/pyproject.toml
--rw-r--r--   0        0        0      409 2023-07-12 09:12:52.054768 tagreader-4.2.3/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.3/tagreader/__version__.py
--rw-r--r--   0        0        0    11751 2023-07-12 11:49:21.922116 tagreader-4.2.3/tagreader/cache.py
--rw-r--r--   0        0        0    22664 2023-07-12 11:49:21.922743 tagreader-4.2.3/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.3/tagreader/logger.py
--rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.3/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.3/tagreader/utils.py
--rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.3/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.4/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.4/README.md
+-rw-r--r--   0        0        0     1633 2023-07-12 12:06:22.847778 tagreader-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0      409 2023-07-12 09:12:52.054768 tagreader-4.2.4/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.4/tagreader/__version__.py
+-rw-r--r--   0        0        0    11699 2023-07-12 11:59:21.151799 tagreader-4.2.4/tagreader/cache.py
+-rw-r--r--   0        0        0    22878 2023-07-12 12:01:14.138324 tagreader-4.2.4/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.4/tagreader/logger.py
+-rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.4/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.4/tagreader/utils.py
+-rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.4/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.4/PKG-INFO
```

### Comparing `tagreader-4.2.3/LICENSE` & `tagreader-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.3/README.md` & `tagreader-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.3/pyproject.toml` & `tagreader-4.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.2.3"
+version = "4.2.4"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 homepage = "https://github.com/equinor/tagreader-python"
```

### Comparing `tagreader-4.2.3/tagreader/cache.py` & `tagreader-4.2.4/tagreader/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,16 @@
     @staticmethod
     def _key_path(
         tagname: str,
         read_type: ReaderType,
         ts: timedelta,
         stepped: bool,
         get_status: bool,
-        start: Optional[datetime] = None,
-        end: Optional[datetime] = None,
+        start: Optional[datetime],
+        end: Optional[datetime],
     ) -> str:
         """Return a string on the form
         $tagname$read_type[$sample_time][$stepped][$get_status]$_start_end
         tagname: safe tagname
         sample_time: integer value. Empty for RAW.
         stepped: "stepped" if value was read as stepped. Empty if not.
         get_status: "status" if value contains status. Empty if not.
@@ -303,15 +303,15 @@
 class SmartCache(BaseCache):
     @staticmethod
     def _key_path(
         *,
         tagname: str,
         read_type: ReaderType,
         ts: timedelta,
-        get_status: bool = False,
+        get_status: bool,
     ) -> str:
         name = safe_tagname(tagname)
         status = get_status * "$status"
         if read_type != ReaderType.RAW:
             interval = int(ts.total_seconds())
             return f"{read_type.name}$s{interval}${name}{status}"
         else:
@@ -320,15 +320,15 @@
     def store(
         self,
         *,
         df: pd.DataFrame,
         tagname: str,
         read_type: ReaderType,
         ts: timedelta,
-        get_status: bool = False,
+        get_status: bool,
     ) -> None:
         key = self._key_path(
             tagname=tagname, read_type=read_type, ts=ts, get_status=get_status
         )
         if df.empty:
             return  # Weirdness ensues when using empty df in select statement below
         if key in self:
@@ -345,17 +345,17 @@
 
     def fetch(
         self,
         *,
         tagname: str,
         read_type: ReaderType,
         ts: timedelta,
-        start: Optional[datetime] = None,
-        end: Optional[datetime] = None,
-        get_status: bool = False,
+        start: Optional[datetime],
+        end: Optional[datetime],
+        get_status: bool,
     ) -> pd.DataFrame:
         key = self._key_path(
             tagname=tagname, read_type=read_type, ts=ts, get_status=get_status
         )
         df = cast(Optional[pd.DataFrame], self.get(key=key))
         if df is None:
             return pd.DataFrame()
```

### Comparing `tagreader-4.2.3/tagreader/clients.py` & `tagreader-4.2.4/tagreader/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,15 +442,21 @@
                         sample_time=ts,
                         read_type=read_type,
                         metadata=metadata,
                         get_status=get_status,
                     )
                     if not df.empty and read_type != ReaderType.RAW:
                         if isinstance(cache, SmartCache):
-                            cache.store(df=df, tagname=tag, read_type=read_type, ts=ts)
+                            cache.store(
+                                df=df,
+                                tagname=tag,
+                                read_type=read_type,
+                                ts=ts,
+                                get_status=get_status,
+                            )
                         if isinstance(cache, BucketCache):
                             cache.store(
                                 df=df,
                                 tagname=tag,
                                 read_type=read_type,
                                 ts=ts,
                                 stepped=stepped,
```

### Comparing `tagreader-4.2.3/tagreader/odbc_handlers.py` & `tagreader-4.2.4/tagreader/odbc_handlers.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.3/tagreader/utils.py` & `tagreader-4.2.4/tagreader/utils.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.3/tagreader/web_handlers.py` & `tagreader-4.2.4/tagreader/web_handlers.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.3/PKG-INFO` & `tagreader-4.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.2.3
+Version: 4.2.4
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
```

