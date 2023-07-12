# Comparing `tmp/tagreader-4.2.0.tar.gz` & `tmp/tagreader-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.2.0.tar", max compression
+gzip compressed data, was "tagreader-4.2.1.tar", max compression
```

## Comparing `tagreader-4.2.0.tar` & `tagreader-4.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.0/README.md
--rw-r--r--   0        0        0     1633 2023-06-28 12:51:14.513858 tagreader-4.2.0/pyproject.toml
--rw-r--r--   0        0        0      351 2023-06-14 10:40:53.499388 tagreader-4.2.0/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.0/tagreader/__version__.py
--rw-r--r--   0        0        0    12790 2023-06-28 12:51:14.514876 tagreader-4.2.0/tagreader/cache.py
--rw-r--r--   0        0        0    23557 2023-06-28 12:51:14.515437 tagreader-4.2.0/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.0/tagreader/logger.py
--rw-r--r--   0        0        0    25164 2023-06-21 08:33:16.577206 tagreader-4.2.0/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     8215 2023-06-14 13:05:07.541522 tagreader-4.2.0/tagreader/utils.py
--rw-r--r--   0        0        0    32496 2023-06-28 10:45:36.341065 tagreader-4.2.0/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.1/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.1/README.md
+-rw-r--r--   0        0        0     1633 2023-07-12 07:06:59.568866 tagreader-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0      351 2023-06-14 10:40:53.499388 tagreader-4.2.1/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.1/tagreader/__version__.py
+-rw-r--r--   0        0        0    12661 2023-07-07 07:04:09.639508 tagreader-4.2.1/tagreader/cache.py
+-rw-r--r--   0        0        0    23367 2023-07-07 07:04:09.639974 tagreader-4.2.1/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.1/tagreader/logger.py
+-rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.1/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.1/tagreader/utils.py
+-rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.1/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.1/PKG-INFO
```

### Comparing `tagreader-4.2.0/LICENSE` & `tagreader-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.0/README.md` & `tagreader-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.0/pyproject.toml` & `tagreader-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.2.0"
+version = "4.2.1"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 homepage = "https://github.com/equinor/tagreader-python"
```

### Comparing `tagreader-4.2.0/tagreader/cache.py` & `tagreader-4.2.1/tagreader/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,162 +100,160 @@
 
     def delete_metadata(self, key: str) -> None:
         _key = f"$metadata${key}"
         self.delete(_key)
 
 
 class BucketCache(BaseCache):
+    @staticmethod
     def _key_path(
-        self,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Union[int, timedelta],
         stepped: bool,
-        status: bool,
-        start_time: Optional[datetime] = None,
-        end_time: Optional[datetime] = None,
+        get_status: bool,
+        start: Optional[datetime] = None,
+        end: Optional[datetime] = None,
     ) -> str:
         """Return a string on the form
-        $tagname$readtype[$sample_time][$stepped][$status]$_start_time_end_time
+        $tagname$read_type[$sample_time][$stepped][$get_status]$_start_end
         tagname: safe tagname
         sample_time: integer value. Empty for RAW.
         stepped: "stepped" if value was read as stepped. Empty if not.
-        status: "status" if value contains status. Empty if not.
-        start_time: The start_time of the query that created the bucket.
-        end_time: The end_time of the query that created the bucket.
+        get_status: "status" if value contains status. Empty if not.
+        start: The start of the query that created the bucket.
+        end: The end of the query that created the bucket.
         """
         tagname = safe_tagname(tagname)
 
         ts = (
             int(ts.total_seconds())
-            if readtype != ReaderType.RAW and isinstance(ts, timedelta)
+            if read_type != ReaderType.RAW and isinstance(ts, timedelta)
             else ts
         )
         timespan = ""
-        if start_time is not None:
-            start_time_epoch = timestamp_to_epoch(start_time)
-            end_time_epoch = timestamp_to_epoch(end_time) if end_time else end_time
-            timespan = f"$_{start_time_epoch}_{end_time_epoch}"
+        if start is not None:
+            start_epoch = timestamp_to_epoch(start)
+            end_epoch = timestamp_to_epoch(end) if end else end
+            timespan = f"$_{start_epoch}_{end_epoch}"
 
         keyval = (
             f"${tagname}"
-            f"${readtype.name}"
-            f"{(ts is not None and readtype != ReaderType.RAW) * f'$s{ts}'}"
+            f"${read_type.name}"
+            f"{(ts is not None and read_type != ReaderType.RAW) * f'$s{ts}'}"
             f"{stepped * '$stepped'}"
-            f"{status * '$status'}"
+            f"{get_status * '$get_status'}"
             f"{timespan}"
         )
         return keyval
 
     def store(
         self,
         df: pd.DataFrame,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: timedelta,
         stepped: bool,
-        status: bool,
-        start_time: datetime,
-        end_time: datetime,
+        get_status: bool,
+        start: datetime,
+        end: datetime,
     ) -> None:
         if df.empty:
             return
 
         intersecting = self.get_intersecting_datasets(
             tagname=tagname,
-            readtype=readtype,
+            read_type=read_type,
             ts=ts,
             stepped=stepped,
-            status=status,
-            start_time=start_time,
-            end_time=end_time,
+            get_status=get_status,
+            start=start,
+            end=end,
         )
         if len(intersecting) > 0:
             for dataset in intersecting:
                 this_start, this_end = self._get_intervals_from_dataset_name(dataset)
-                start_time = min(start_time, this_start if this_start else start_time)
-                end_time = max(end_time, this_end if this_end else end_time)
+                start = min(start, this_start if this_start else start)
+                end = max(end, this_end if this_end else end)
                 df2 = self.get(dataset)
                 if df2 is not None:
                     df = pd.concat([df, df2], axis=0)
                 self.delete(dataset)
         key = self._key_path(
             tagname=tagname,
-            readtype=readtype,
+            read_type=read_type,
             ts=ts,
             stepped=stepped,
-            status=status,
-            start_time=start_time,
-            end_time=end_time,
+            get_status=get_status,
+            start=start,
+            end=end,
         )
         self.put(key=key, value=clean_dataframe(df))
 
     @staticmethod
     def _get_intervals_from_dataset_name(
         name: str,
     ) -> Tuple[datetime, datetime]:
         name_with_times = name.split("$")[-1]
         if not name_with_times.count("_") == 2:
-            return (None, None)  # type: ignore[return-value]
-        _, start_time_epoch, end_time_epoch = name_with_times.split("_")
-        start_time = pd.to_datetime(int(start_time_epoch), unit="s").tz_localize("UTC")
-        end_time = pd.to_datetime(int(end_time_epoch), unit="s").tz_localize("UTC")
-        return start_time, end_time
+            return None, None  # type: ignore[return-value]
+        _, start_epoch, end_epoch = name_with_times.split("_")
+        start = pd.to_datetime(int(start_epoch), unit="s").tz_localize("UTC")
+        end = pd.to_datetime(int(end_epoch), unit="s").tz_localize("UTC")
+        return start, end
 
     def get_intersecting_datasets(
         self,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Union[int, timedelta],
         stepped: bool,
-        status: bool,
-        start_time: datetime,
-        end_time: datetime,
+        get_status: bool,
+        start: datetime,
+        end: datetime,
     ) -> List[str]:
         if not len(self) > 0:
             return []
         intersecting_datasets = []
         for dataset in self.iterkeys():
             target_key = self._key_path(
                 tagname=tagname,
-                readtype=readtype,
-                start_time=None,
-                end_time=None,
+                read_type=read_type,
+                start=None,
+                end=None,
                 ts=ts,
                 stepped=stepped,
-                status=status,
+                get_status=get_status,
             )
             if target_key in dataset:
-                start_time_ds, end_time_ds = self._get_intervals_from_dataset_name(
-                    dataset
-                )
-                if end_time_ds >= start_time and end_time >= start_time_ds:
+                start_ds, end_ds = self._get_intervals_from_dataset_name(dataset)
+                if end_ds >= start and end >= start_ds:
                     intersecting_datasets.append(dataset)
         return intersecting_datasets
 
     def get_missing_intervals(
         self,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Union[int, timedelta],
         stepped: bool,
-        status: bool,
-        start_time: datetime,
-        end_time: datetime,
+        get_status: bool,
+        start: datetime,
+        end: datetime,
     ) -> List[Tuple[datetime, datetime]]:
         datasets = self.get_intersecting_datasets(
             tagname=tagname,
-            readtype=readtype,
+            read_type=read_type,
             ts=ts,
             stepped=stepped,
-            status=status,
-            start_time=start_time,
-            end_time=end_time,
+            get_status=get_status,
+            start=start,
+            end=end,
         )
-        missing_intervals = [(start_time, end_time)]
+        missing_intervals = [(start, end)]
         for dataset in datasets:
             b = self._get_intervals_from_dataset_name(dataset)
             for _ in range(0, len(missing_intervals)):
                 r = missing_intervals.pop(0)
                 if b[1] < r[0] or b[0] > r[1]:
                     # No overlap
                     missing_intervals.append(r)
@@ -273,81 +271,83 @@
                     # The bucket chomps the end of the interval
                     missing_intervals.append((r[0], b[0]))
         return missing_intervals
 
     def fetch(
         self,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Union[int, timedelta],
         stepped: bool,
-        status: bool,
-        start_time: datetime,
-        end_time: datetime,
+        get_status: bool,
+        start: datetime,
+        end: datetime,
     ) -> pd.DataFrame:
         df = pd.DataFrame()
         if not len(self) > 0:
             return df
 
         if isinstance(ts, timedelta):
             ts = int(ts.total_seconds())
 
         datasets = self.get_intersecting_datasets(
             tagname=tagname,
-            readtype=readtype,
+            read_type=read_type,
             ts=ts,
             stepped=stepped,
-            status=status,
-            start_time=start_time,
-            end_time=end_time,
+            get_status=get_status,
+            start=start,
+            end=end,
         )
 
         for dataset in datasets:
             df2 = self.get(dataset)
             if df2 is not None:
-                df = pd.concat([df, df2.loc[start_time:end_time]], axis=0)  # type: ignore[call-overload, misc]
+                df = pd.concat([df, df2.loc[start:end]], axis=0)  # type: ignore[call-overload, misc]
 
         return clean_dataframe(df)
 
 
 class SmartCache(BaseCache):
     @staticmethod
     def key_path(
         df: Union[str, pd.DataFrame],
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Optional[Union[int, timedelta]] = None,
+        get_status: bool = False,
     ) -> str:
         """Return a string on the form
         XXX$sYY$ZZZ where XXX is the ReadType, YY is the interval between samples
         (in seconds) and ZZZ is a safe tagname.
         """
         name = str(list(df)[0]) if isinstance(df, pd.DataFrame) else df
         name = safe_tagname(name)
         ts = int(ts.total_seconds()) if isinstance(ts, timedelta) else ts
-        if readtype != ReaderType.RAW:
+        if read_type != ReaderType.RAW:
             if ts is None:
                 # Determine sample time by reading interval between first two
                 # samples of dataframe.
                 if isinstance(df, pd.DataFrame):
                     interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)  # type: ignore[attr-defined]
                 else:
                     raise TypeError
             else:
                 interval = int(ts)
-            return f"{readtype.name}$s{interval}${name}"
+            return f"{read_type.name}$s{interval}${name}"
         else:
-            return f"{readtype.name}${name}"
+            return f"{read_type.name}${name}"
 
     def store(
         self,
         df: pd.DataFrame,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Optional[Union[int, timedelta]] = None,
+        get_status: bool = False,
     ) -> None:
-        key = self.key_path(df=df, readtype=readtype, ts=ts)
+        key = self.key_path(df=df, read_type=read_type, ts=ts, get_status=get_status)
         if df.empty:
             return  # Weirdness ensues when using empty df in select statement below
         if key in self:
             df2 = self.get(key)
             if df2 is not None:
                 df = pd.concat([df, df2], axis=0)
             self.delete(key=key)
@@ -357,21 +357,24 @@
             )
         else:
             self.put(key, df)
 
     def fetch(
         self,
         tagname: str,
-        readtype: ReaderType,
+        read_type: ReaderType,
         ts: Optional[Union[int, timedelta]] = None,
-        start_time: Optional[datetime] = None,
-        stop_time: Optional[datetime] = None,
+        start: Optional[datetime] = None,
+        end: Optional[datetime] = None,
+        get_status: bool = False,
     ) -> pd.DataFrame:
-        key = self.key_path(df=tagname, readtype=readtype, ts=ts)
+        key = self.key_path(
+            df=tagname, read_type=read_type, ts=ts, get_status=get_status
+        )
         df = cast(Optional[pd.DataFrame], self.get(key=key))
         if df is None:
             return pd.DataFrame()
-        if start_time is not None:
-            df = df.loc[df.index >= start_time]
-        if stop_time is not None:
-            df = df.loc[df.index <= stop_time]
+        if start is not None:
+            df = df.loc[df.index >= start]
+        if end is not None:
+            df = df.loc[df.index <= end]
         return df
```

### Comparing `tagreader-4.2.0/tagreader/clients.py` & `tagreader-4.2.1/tagreader/clients.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,62 +74,62 @@
         if auth is None:
             auth = get_auth_aspen()
         return list_aspenone_sources(url=url, auth=auth, verifySSL=verifySSL)
 
 
 def get_missing_intervals(
     df: pd.DataFrame,
-    start_time: datetime,
-    stop_time: datetime,
+    start: datetime,
+    end: datetime,
     ts: Optional[timedelta],
     read_type: ReaderType,
 ):
     if (
         read_type == ReaderType.RAW
     ):  # Fixme: How to check for completeness for RAW data?
-        return [[start_time, stop_time]]
+        return [[start, end]]
     seconds = int(ts.total_seconds())
-    tvec = pd.date_range(start=start_time, end=stop_time, freq=f"{seconds}s")
+    tvec = pd.date_range(start=start, end=end, freq=f"{seconds}s")
     if len(df) == len(tvec):  # Short-circuit if dataset is complete
         return []
     values_in_df = tvec.isin(df.index)
     missing_intervals = []
     for k, g in groupby(enumerate(values_in_df), lambda ix: ix[1]):
         if not k:
             seq = list(map(itemgetter(0), g))
             missing_intervals.append(
                 (
                     pd.Timestamp(tvec[seq[0]]).to_pydatetime(),
                     pd.Timestamp(tvec[seq[-1]]).to_pydatetime(),
                 )
             )
             # Should be unnecessary to fetch overlapping points since get_next_timeslice
-            # ensures start <= t <= stop
+            # ensures start <= t <= end
             # missingintervals.append((pd.Timestamp(tvec[seq[0]]),
             #                          pd.Timestamp(tvec[min(seq[-1]+1, len(tvec)-1)])))
     return missing_intervals
 
 
 def get_next_timeslice(
-    start_time: datetime,
-    stop_time: datetime,
+    start: datetime,
+    end: datetime,
     ts: Optional[timedelta],
     max_steps: Optional[int],
 ) -> Tuple[datetime, datetime]:
     if max_steps is None:
-        calc_stop_time = stop_time
+        calc_end = end
     else:
-        calc_stop_time = start_time + ts * max_steps
-    calc_stop_time = min(stop_time, calc_stop_time)
+        calc_end = start + ts * max_steps
+    calc_end = min(end, calc_end)
     # Ensure we include the last data point.
     # Discrepancies between Aspen and Pi for +ts
     # Discrepancies between IMS and cache for e.g. ts.
-    # if calc_stop_time == stop_time:
-    #     calc_stop_time += ts / 2
-    return start_time, calc_stop_time
+    # if calc_end == end:
+    #     calc_end += ts / 2
+    return start, calc_end
 
 
 def get_server_address_aspen(datasource: str) -> Optional[Tuple[str, int]]:
     """Data sources are listed under
     HKEY_CURRENT_USER\\Software\\AspenTech\\ADSA\\Caches\\AspenADSA\\username.
     For each data source there are multiple keys with Host entries. We start by
     identifying the correct key to use by locating the UUID for Aspen SQLplus
@@ -145,25 +145,25 @@
         winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Classes\Wow6432Node\CLSID"
     )
     regkey, _ = find_registry_key_from_name(
         regkey_clsid, "Aspen SQLplus service component"
     )
     regkey_implemented_categories = winreg.OpenKeyEx(regkey, "Implemented Categories")
 
-    _, aspen_UUID = find_registry_key_from_name(
+    _, aspen_uuid = find_registry_key_from_name(
         regkey_implemented_categories, "Aspen SQLplus services"
     )
 
     reg_adsa = winreg.OpenKey(
         winreg.HKEY_CURRENT_USER,
         r"Software\AspenTech\ADSA\Caches\AspenADSA\\" + os.getlogin(),
     )
 
     try:
-        reg_site_key = winreg.OpenKey(reg_adsa, datasource + "\\" + aspen_UUID)
+        reg_site_key = winreg.OpenKey(reg_adsa, datasource + "\\" + aspen_uuid)
         host = winreg.QueryValueEx(reg_site_key, "Host")[0]
         port = int(winreg.QueryValueEx(reg_site_key, "Port")[0])
         return host, port
     except FileNotFoundError:
         return None
 
 
@@ -307,14 +307,15 @@
         url: Optional[str] = None,
         host: Optional[str] = None,
         port: Optional[int] = None,
         handler_options: Dict[str, Union[int, float, str]] = {},  # noqa:
         verifySSL: bool = True,
         auth: Optional[Any] = None,
         cache: Optional[Union[SmartCache, BucketCache]] = None,
+        get_status: bool = False,
     ):
         if isinstance(imstype, str):
             try:
                 imstype = getattr(IMSType, imstype.upper())
             except AttributeError:
                 raise ValueError(
                     f"imstype needs to be one of {', '.join([v for v in IMSType.__members__.values()])}."
@@ -361,91 +362,92 @@
         return self.handler._get_tag_metadata(
             tag
         )  # noqa: Should probably expose this as a public method if needed.
 
     def _read_single_tag(
         self,
         tag: str,
-        start_time: Optional[datetime],
-        stop_time: Optional[datetime],
+        start: Optional[datetime],
+        end: Optional[datetime],
         ts: timedelta,
         read_type: ReaderType,
         get_status: bool,
         cache: Optional[Union[BucketCache, SmartCache]],
     ):
         if read_type == ReaderType.SNAPSHOT:
             metadata = self._get_metadata(tag)
             df = self.handler.read_tag(
                 tag=tag,
-                start_time=start_time,
-                stop_time=stop_time,
+                start=start,
+                end=end,
                 sample_time=ts,
                 read_type=read_type,
                 metadata=metadata,
                 get_status=get_status,
             )
         else:
             stepped = False
-            missing_intervals = [(start_time, stop_time)]
+            missing_intervals = [(start, end)]
             df = pd.DataFrame()
 
             if (
                 isinstance(cache, SmartCache)
                 and read_type != ReaderType.RAW
                 and not get_status
             ):
                 time_slice = get_next_timeslice(
-                    start_time=start_time, stop_time=stop_time, ts=ts, max_steps=None
+                    start=start, end=end, ts=ts, max_steps=None
                 )
                 df = cache.fetch(
                     tagname=tag,
-                    readtype=read_type,
+                    read_type=read_type,
                     ts=ts,
-                    start_time=time_slice[0],
-                    end_time=time_slice[1],
+                    start=time_slice[0],
+                    end=time_slice[1],
+                    get_status=get_status,
                 )
                 missing_intervals = get_missing_intervals(
                     df=df,
-                    start_time=start_time,
-                    stop_time=stop_time,
+                    start=start,
+                    end=end,
                     ts=ts,
                     read_type=read_type,
                 )
                 if not missing_intervals:
                     return df.tz_convert(self.tz).sort_index()
             elif isinstance(cache, BucketCache):
                 df = cache.fetch(
                     tagname=tag,
-                    readtype=read_type,
+                    read_type=read_type,
                     ts=ts,
                     stepped=stepped,
-                    status=get_status,
-                    starttime=start_time,
-                    endtime=stop_time,
+                    get_status=get_status,
+                    start=start,
+                    end=end,
                 )
                 missing_intervals = cache.get_missing_intervals(
                     tagname=tag,
-                    readtype=read_type,
+                    read_type=read_type,
                     ts=ts,
                     stepped=stepped,
-                    status=get_status,
-                    start_time=start_time,
-                    end_time=stop_time,
+                    get_status=get_status,
+                    start=start,
+                    end=end,
                 )
                 if not missing_intervals:
                     return df.tz_convert(self.tz).sort_index()
 
             metadata = self._get_metadata(tag)
             frames = [df]
-            for start, stop in missing_intervals:
+            for start, end in missing_intervals:
                 while True:
                     df = self.handler.read_tag(
                         tag=tag,
-                        start_time=start,
-                        stop_time=stop,
+                        start=start,
+                        end=end,
                         sample_time=ts,
                         read_type=read_type,
                         metadata=metadata,
                         get_status=get_status,
                     )
                     if len(df.index) > 0:
                         if (
@@ -453,24 +455,24 @@
                             and read_type
                             not in [
                                 ReaderType.SNAPSHOT,
                                 ReaderType.RAW,
                             ]
                             and not get_status
                         ):
-                            cache.store(df=df, readtype=read_type, ts=ts)
+                            cache.store(df=df, read_type=read_type, ts=ts)
                     frames.append(df)
                     if len(df) < self.handler._max_rows:
                         break
                     start = df.index[-1]
                 # if read_type != ReaderType.RAW:
                 #     time_slice = [start, start]
-                #     while time_slice[1] < stop:
+                #     while time_slice[1] < end:
                 #         time_slice = get_next_timeslice(
-                #             time_slice[1], stop, ts, self.handler._max_rows
+                #             time_slice[1], end, ts, self.handler._max_rows
                 #         )
                 #         df = self.handler.read_tag(
                 #             tag, time_slice[0], time_slice[1], ts, read_type, metadata
                 #         )
                 #         if len(df.index) > 0:
                 #             if cache is not None and read_type != ReaderType.RAW:
                 #                 cache.store(df, read_type, ts)
@@ -524,24 +526,26 @@
         tags: Union[str, List[str]],
         start_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
         stop_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
         ts: Optional[Union[timedelta, pd.Timedelta]] = timedelta(seconds=60),
         read_type: ReaderType = ReaderType.INT,
         get_status: bool = False,
     ):
+        start = start_time
+        end = stop_time
         logger.warn(
             (
                 "This function has been renamed to read() and is deprecated. "
                 "Please call 'read()' instead"
             )
         )
         return self.read(
             tags=tags,
-            start_time=start_time,
-            end_time=stop_time,
+            start_time=start,
+            end_time=end,
             ts=ts,
             read_type=read_type,
             get_status=get_status,
         )
 
     def read(
         self,
@@ -563,74 +567,76 @@
         All possible values for read_type are defined in the ReaderType class,
         which can be imported as follows:
             from utils import ReaderType
 
         Values for ReaderType.* that should work for all handlers are:
             INT, RAW, MIN, MAX, RNG, AVG, VAR, STD and SNAPSHOT
         """
+        start = start_time
+        end = end_time
         if isinstance(tags, str):
             tags = [tags]
         if isinstance(read_type, str):
             try:
                 read_type = getattr(ReaderType, read_type)
             except AttributeError:
                 ValueError(
-                    "readtype needs to be of type ReaderType.* or a legal value. Please refer to the docstring."
+                    "read_type needs to be of type ReaderType.* or a legal value. Please refer to the docstring."
                 )
         if read_type in [ReaderType.RAW, ReaderType.SNAPSHOT] and len(tags) > 1:
             raise RuntimeError(
                 "Unable to read raw/sampled data for multiple tags since they don't "
                 "share time vector. Read one at a time."
             )
 
         if isinstance(tags, str):
             tags = [tags]
 
-        if start_time is None:
-            start_time = NONE_START_TIME
-        elif isinstance(start_time, (str, pd.Timestamp)):
+        if start is None:
+            start = NONE_START_TIME
+        elif isinstance(start, (str, pd.Timestamp)):
             try:
-                start_time = convert_to_pydatetime(start_time)
+                start = convert_to_pydatetime(start)
             except ValueError:
-                start_time = convert_to_pydatetime(start_time)
-        if end_time is None:
-            end_time = datetime.utcnow()
-        elif isinstance(end_time, (str, pd.Timestamp)):
-            end_time = convert_to_pydatetime(end_time)
+                start = convert_to_pydatetime(start)
+        if end is None:
+            end = datetime.utcnow()
+        elif isinstance(end, (str, pd.Timestamp)):
+            end = convert_to_pydatetime(end)
 
         if isinstance(ts, pd.Timedelta):
             ts = ts.to_pytimedelta()
         elif isinstance(ts, int):
             ts = timedelta(seconds=ts)
         elif not isinstance(ts, timedelta):
             raise ValueError(
                 "ts needs to be either a None, timedelta or and integer (number of seconds)."
                 f" Given type: {type(ts)}"
             )
 
         if read_type != ReaderType.SNAPSHOT:
-            start_time = ensure_datetime_with_tz(start_time, tz=self.tz)
-        if end_time:
-            end_time = ensure_datetime_with_tz(end_time, tz=self.tz)
+            start = ensure_datetime_with_tz(start, tz=self.tz)
+        if end:
+            end = ensure_datetime_with_tz(end, tz=self.tz)
 
-        oldtags = tags
+        old_tags = tags
         tags = list(dict.fromkeys(tags))
-        if len(oldtags) > len(tags):
-            duplicates = set([x for n, x in enumerate(oldtags) if x in oldtags[:n]])
+        if len(old_tags) > len(tags):
+            duplicates = set([x for n, x in enumerate(old_tags) if x in old_tags[:n]])
             logger.warning(
                 f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}"
             )
 
         results = []
         for i, tag in enumerate(tags):
             results.append(
                 self._read_single_tag(
                     tag=tag,
-                    start_time=start_time,
-                    stop_time=end_time,
+                    start=start,
+                    end=end,
                     ts=ts,
                     read_type=read_type,
                     get_status=get_status,
                     cache=self.cache,
                 )
             )
```

### Comparing `tagreader-4.2.0/tagreader/odbc_handlers.py` & `tagreader-4.2.1/tagreader/odbc_handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         else:
             return self._connection_string
 
     @staticmethod
     def generate_read_query(
         tag: str,
         mapdef: Optional[Dict[str, str]],
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         get_status: bool = False,
     ):
         if mapdef is None:
             mapdef = {}
         if read_type in [
@@ -108,33 +108,33 @@
 
         # TODO: How to interpret ip_input_quality and ip_value_quality
         # which use a different numeric schema (e.g. -1) than status from
         # history table (0, 1, 2, 4, 5, 6)
         if get_status and read_type == ReaderType.SNAPSHOT:
             raise NotImplementedError
 
-        if read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            stop_time = None
+        if read_type == ReaderType.SNAPSHOT and end is not None:
+            end = None
             logger.warning(
                 "End time is not supported for Aspen ODBC connection using 'SNAPSHOT'."
                 "Try the web API 'piwebapi' instead."
             )
 
         seconds = 0
         if read_type != ReaderType.SNAPSHOT:
-            start_time = start_time.astimezone(pytz.UTC)
-            if stop_time:
-                stop_time = stop_time.astimezone(pytz.UTC)
+            start = start.astimezone(pytz.UTC)
+            if end:
+                end = end.astimezone(pytz.UTC)
             seconds = int(sample_time.total_seconds())
             if read_type == ReaderType.SAMPLED:
                 seconds = 0
             else:
                 if seconds <= 0:
                     raise NotImplementedError
-                    # sample_time = (stop_time-start_time).totalseconds
+                    # sample_time = (end-start).totalseconds
 
         timecast_format_query = "%Y-%m-%dT%H:%M:%SZ"  # 05-jan-18 14:00:00
 
         request_num = {
             ReaderType.SAMPLED: 4,  # VALUES request (actual recorded data), history
             ReaderType.SHAPEPRESERVING: 3,  # FITS request, history
             ReaderType.INT: 7,  # TIMES2_EXTENDED request, history
@@ -150,15 +150,16 @@
         from_column = {
             ReaderType.SAMPLED: "history",
             ReaderType.SHAPEPRESERVING: "history",
             ReaderType.INT: "history",
             ReaderType.SNAPSHOT: '"' + str(tag) + '"',
         }.get(read_type, "aggregates")
         # For RAW: historyevent?
-        # Ref https://help.sap.com/saphelp_pco151/helpdata/en/4c/72e34ee631469ee10000000a15822d/content.htm?no_cache=true
+        # Ref:
+        #  https://help.sap.com/saphelp_pco151/helpdata/en/4c/72e34ee631469ee10000000a15822d/content.htm?no_cache=true
 
         ts = "ts"
         if from_column == "aggregates":
             ts = "ts_start"
         elif read_type == ReaderType.SNAPSHOT:
             ts = mapdef.get("MAP_CurrentTimeStamp", "IP_INPUT_TIME")
 
@@ -183,25 +184,25 @@
         query = [f'SELECT ISO8601({ts}) AS "time", {value} AS "value"']
         if get_status:
             # status is returned/interpreted as char regardless if cast to INT
             query.extend([f', {status} AS "status"'])
         query.extend([f"FROM {from_column}"])
 
         if ReaderType.SNAPSHOT != read_type:
-            start = start_time.strftime(timecast_format_query)
-            stop = stop_time.strftime(timecast_format_query)
+            start = start.strftime(timecast_format_query)
+            end = end.strftime(timecast_format_query)
             query.extend([f"WHERE name = {tag!r}"])
             if mapdef:
                 query.extend([f'AND FIELD_ID = FT({mapdef["MAP_HistoryValue"]!r})'])
             if ReaderType.RAW != read_type:
                 query.extend([f"AND (period = {seconds*10})"])
             query.extend(
                 [
                     f"AND (request = {request_num})",
-                    f"AND (ts BETWEEN {start!r} AND {stop!r})",
+                    f"AND (ts BETWEEN {start!r} AND {end!r})",
                     "ORDER BY ts",
                 ]
             )
 
         return " ".join(query)
 
     def set_options(self, options):
@@ -353,31 +354,31 @@
         if not res.description:
             res.description = ""
         return res.description
 
     def read_tag(
         self,
         tag: str,
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         (cleantag, mapping) = tag.split(";") if ";" in tag else (tag, None)
         mapdef = dict()
 
         if isinstance(mapping, str):
             mapdef = self._get_specific_mapdef(tagname=cleantag, mapping=mapping)
         query = self.generate_read_query(
             tag=cleantag,
             mapdef=mapdef,
-            start_time=start_time,
-            stop_time=stop_time,
+            start=start,
+            end=end,
             sample_time=sample_time,
             read_type=read_type,
             get_status=get_status,
         )
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
@@ -455,16 +456,16 @@
                 ["descriptor LIKE '{desc}'".format(desc=desc.replace("*", "%"))]
             )
         return " ".join(query)
 
     def generate_read_query(
         self,
         tag: str,
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if read_type in [
             ReaderType.COUNT,
@@ -472,33 +473,33 @@
             ReaderType.BAD,
             ReaderType.TOTAL,
             ReaderType.SUM,
             ReaderType.SHAPEPRESERVING,
         ]:
             raise NotImplementedError
 
-        if read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            stop_time = None
+        if read_type == ReaderType.SNAPSHOT and end is not None:
+            end = None
             logger.warning(
                 "End time is not supported for PI ODBC connection using 'SNAPSHOT'."
                 "Try the web API 'piwebapi' instead."
             )
 
         seconds = 0
         if read_type != ReaderType.SNAPSHOT:
-            start_time = start_time.astimezone(pytz.UTC)
-            if stop_time:
-                stop_time = stop_time.astimezone(pytz.UTC)
+            start = start.astimezone(pytz.UTC)
+            if end:
+                end = end.astimezone(pytz.UTC)
             seconds = int(sample_time.total_seconds())
             if ReaderType.SAMPLED == read_type:
                 seconds = 0
             else:
                 if seconds <= 0:
                     pass  # Fixme: Not implemented
-                    # sample_time = (stop_time-start_time).totalseconds
+                    # sample_time = (end-start).totalseconds
 
         timecast_format_query = "%d-%b-%y %H:%M:%S"  # 05-jan-18 14:00:00
         # timecast_format_output = "yyyy-MM-dd HH:mm:ss"
 
         source = {
             ReaderType.INT: "[piarchive]..[piinterp2]",
             ReaderType.MIN: "[piarchive]..[pimin]",
@@ -523,35 +524,37 @@
         elif ReaderType.BAD == read_type:
             query = ["SELECT 100-CAST(pctgood as FLOAT32)"]
         elif ReaderType.RAW == read_type:
             query = [f"SELECT TOP {self._max_rows} CAST(value as FLOAT32)"]
         else:
             query = ["SELECT CAST(value as FLOAT32)"]
 
-        # query.extend([f"AS value, FORMAT(time, '{timecast_format_output}') AS timestamp FROM {source} WHERE tag='{tag}'"])
+        # query.extend(
+        #   [f"AS value, FORMAT(time, '{timecast_format_output}') AS timestamp FROM {source} WHERE tag='{tag}'"]
+        # )
         query.extend(["AS value,"])
 
         if get_status:
             query.extend(["status, questionable, substituted,"])
 
         query.extend([f"time FROM {source} WHERE tag='{tag}'"])  # __utctime also works
 
         if ReaderType.SNAPSHOT != read_type:
-            start = start_time.strftime(timecast_format_query)
-            stop = stop_time.strftime(timecast_format_query)
-            query.extend([f"AND (time BETWEEN '{start}' AND '{stop}')"])
+            start = start.strftime(timecast_format_query)
+            end = end.strftime(timecast_format_query)
+            query.extend([f"AND (time BETWEEN '{start}' AND '{end}')"])
 
         if ReaderType.GOOD == read_type:
             query.extend(["AND questionable = FALSE"])
         elif ReaderType.NOTGOOD == read_type:
             query.extend(["AND questionable = TRUE"])
         elif ReaderType.SHAPEPRESERVING == read_type:
             query.extend(
                 [
-                    f"AND (intervalcount = {int((stop_time - start_time).total_seconds() / seconds)})"
+                    f"AND (intervalcount = {int((end - start).total_seconds() / seconds)})"
                 ]
             )
         elif ReaderType.RAW == read_type:
             pass
         elif read_type not in [ReaderType.SNAPSHOT, ReaderType.RAW]:
             query.extend([f"AND (timestep = '{seconds}s')"])
 
@@ -611,30 +614,30 @@
         ]:
             return True
         return False
 
     def read_tag(
         self,
         tag: str,
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if metadata is None:
             # Tag not found
             # TODO: Handle better and similarly across all handlers.
             return pd.DataFrame()
 
         query = self.generate_read_query(
             tag=tag,
-            start_time=start_time,
-            stop_time=stop_time,
+            start=start,
+            end=end,
             sample_time=sample_time,
             read_type=read_type,
             get_status=get_status,
             metadata=None,
         )
 
         with warnings.catch_warnings():
```

### Comparing `tagreader-4.2.0/tagreader/utils.py` & `tagreader-4.2.1/tagreader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,18 @@
     if not date_stamp.tzinfo:
         date_stamp = tz.localize(date_stamp)
 
     return date_stamp
 
 
 def urljoin(*args) -> str:
-    """Joins components of URL. Ensures slashes are inserted or removed where
+    """
+    Joins components of URL. Ensures slashes are inserted or removed where
     needed, and does not strip trailing slash of last element.
 
-    Arguments:
-        str
     Returns:
         str -- Generated URL
     """
     trailing_slash = "/" if args[-1].endswith("/") else ""
     return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
```

### Comparing `tagreader-4.2.0/tagreader/web_handlers.py` & `tagreader-4.2.1/tagreader/web_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from requests_kerberos import OPTIONAL, HTTPKerberosAuth
 
 from tagreader.cache import BaseCache
 from tagreader.logger import logger
 from tagreader.utils import ReaderType, is_mac, is_windows, urljoin
 
 
-def get_verifySSL() -> Union[bool, str]:
+def get_verify_ssl() -> Union[bool, str]:
     if is_windows() or is_mac():
         return True
     return "/etc/ssl/certs/ca-bundle.trust.crt"
 
 
 def get_auth_pi() -> HTTPKerberosAuth:
     return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
@@ -52,15 +52,15 @@
 
     if auth is None:
         auth = get_auth_aspen()
 
     if verifySSL is False:
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     elif verifySSL is None:
-        verifySSL = get_verifySSL()
+        verifySSL = get_verify_ssl()
 
     url_ = urljoin(url, "DataSources")
     params = {"service": "ProcessData", "allQuotes": 1}
 
     res = requests.get(url_, params=params, auth=auth, verify=verifySSL)
     res.raise_for_status()
     try:
@@ -80,15 +80,15 @@
 
     if auth is None:
         auth = get_auth_pi()
 
     if verifySSL is False:
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     elif verifySSL is None:
-        verifySSL = get_verifySSL()
+        verifySSL = get_verify_ssl()
 
     url_ = urljoin(url, "dataservers")
     res = requests.get(url_, auth=auth, verify=verifySSL)
 
     res.raise_for_status()
     try:
         source_list = [r["Name"] for r in res.json()["Items"]]
@@ -107,15 +107,15 @@
     ):
         self.datasource = datasource
         self.base_url = url
         self.session = requests.Session()
         self.session.auth = auth if auth is not None else get_auth_aspen()
         if verifySSL is False:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
+        self.session.verify = verifySSL if verifySSL is not None else get_verify_ssl()
 
     def fetch(self, url, params: Optional[Union[str, Dict[str, str]]] = None) -> Dict:
         res = self.session.get(url, params=params)
         res.raise_for_status()
 
         if len(res.text) == 0:
             logger.warning(f"No data found for {url} {params}")
@@ -191,16 +191,16 @@
         params = {"datasource": datasource, "tag": tag, "max": 100, "getTrendable": 0}
         return params
 
     def generate_read_query(
         self,
         tagname: str,
         mapname: Optional[str],
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         metadata: Any,
     ):
         # Maxpoints is used for Actual (raw) and Bestfit (shapepreserving).
         # Probably need to handle this in another way at some point
         maxpoints = self._max_rows
@@ -222,22 +222,22 @@
             ReaderType.BAD: 10,
             ReaderType.TOTAL: -1,
             ReaderType.SUM: 16,
             ReaderType.SNAPSHOT: -1,
         }.get(read_type, -1)
 
         if read_type == ReaderType.SNAPSHOT:
-            if stop_time is not None:
+            if end is not None:
                 use_current = 0
-                end_time = int(stop_time.timestamp()) * 1000
+                end = int(end.timestamp()) * 1000
             else:
                 use_current = 1
-                end_time = 0
+                end = 0
 
-            query = f'<Q f="d" allQuotes="1" rt="{end_time}" uc="{use_current}">'
+            query = f'<Q f="d" allQuotes="1" rt="{end}" uc="{use_current}">'
         else:
             query = '<Q f="d" allQuotes="1">'
 
         query += "<Tag>" f"<N><![CDATA[{tagname}]]></N>"
 
         if mapname:
             query += f"<M><![CDATA[{mapname}]]></M>"
@@ -245,16 +245,16 @@
         query += f"<D><![CDATA[{self.datasource}]]></D>" "<F><![CDATA[VAL]]></F>"
 
         if read_type == ReaderType.SNAPSHOT:
             query += "<VS>1</VS>"
         else:
             query += (
                 "<HF>0</HF>"  # History format: 0=Raw, 1=RecordAsString
-                f"<St>{int(start_time.timestamp()) * 1000}</St>"
-                f"<Et>{int(stop_time.timestamp()) * 1000}</Et>"
+                f"<St>{int(start.timestamp()) * 1000}</St>"
+                f"<Et>{int(end.timestamp()) * 1000}</Et>"
                 f"<RT>{rt}</RT>"
             )
         if read_type in [ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
             query += f"<X>{maxpoints}</X>"
         if read_type not in [ReaderType.INT, ReaderType.SNAPSHOT]:
             query += f"<O>{outsiders}</O>"
         if read_type not in [ReaderType.RAW]:
@@ -439,23 +439,23 @@
 
     def _get_tag_description(self, tag: str):
         query = self.generate_get_description_query(tag)
         url = urljoin(self.base_url, "TagInfo")
         data = self.fetch(url, params=query)
         try:
             desc = data["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
-        except Exception:
+        except KeyError:
             desc = ""
         return desc
 
     def read_tag(
         self,
         tag: str,
-        start_time: Optional[datetime],
-        stop_time: Optional[datetime],
+        start: Optional[datetime],
+        end: Optional[datetime],
         sample_time: Optional[timedelta],
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if read_type not in [
             ReaderType.INT,
@@ -474,28 +474,28 @@
             url = urljoin(self.base_url, "Attribute")
         else:
             url = urljoin(self.base_url, "History")
 
         # Actual and bestfit read types allow specifying maxpoints.
         # Aggregate reads limit to 10 000 points and issue a moredata-token.
         # TODO: May need to look into using this later - most likely more
-        # efficient than creating new query starting at previous stoptime.
+        # efficient than creating new query starting at previous end time.
         # Interpolated reads return error message if more than 100 000 points,
         # so we need to limit the range. Note -1 because INT normally includes
         # both start and end time.
         if read_type == ReaderType.INT:
-            stop_time = min(stop_time, start_time + sample_time * (self._max_rows - 1))
+            end = min(end, start + sample_time * (self._max_rows - 1))
 
         tagname, mapname = self.split_tagmap(tag)
 
         params = self.generate_read_query(
             tagname=tagname,
             mapname=mapname,
-            start_time=start_time,
-            stop_time=stop_time,
+            start=start,
+            end=end,
             sample_time=sample_time,
             read_type=read_type,
             metadata={},
         )
 
         data = self.fetch(url, params=params)
 
@@ -665,16 +665,16 @@
             params["scope"] = f"pi:{datasource}"
 
         return params
 
     def generate_read_query(
         self,
         tag: str,
-        start_time: datetime,
-        stop_time: datetime,
+        start: datetime,
+        end: datetime,
         sample_time: timedelta,
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ) -> Tuple[str, Dict[str, str]]:
         if read_type in [
             ReaderType.COUNT,
@@ -699,19 +699,19 @@
             ReaderType.SHAPEPRESERVING: "plot",
         }.get(read_type, "summary")
 
         url = f"streams/{webid}/{get_action}"
         params = {}
 
         if read_type != ReaderType.SNAPSHOT:
-            params["startTime"] = self._time_to_UTC_string(start_time)
-            params["endTime"] = self._time_to_UTC_string(stop_time)
+            params["startTime"] = self._time_to_UTC_string(start)
+            params["endTime"] = self._time_to_UTC_string(end)
             params["timeZone"] = "UTC"
-        elif read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            params["time"] = self._time_to_UTC_string(stop_time)
+        elif read_type == ReaderType.SNAPSHOT and end is not None:
+            params["time"] = self._time_to_UTC_string(end)
             params["timeZone"] = "UTC"
 
         summary_type = {
             ReaderType.MIN: "Minimum",
             ReaderType.MAX: "Maximum",
             ReaderType.AVG: "Average",
             ReaderType.VAR: "StdDev",
@@ -778,15 +778,15 @@
             data = self.fetch(url, params=params)
 
             for item in data["Items"]:
                 description = item["Description"] if "Description" in item else ""
                 ret.append((item["Name"], description))
             next_start = int(data["Links"]["Next"].split("=")[-1])
             if int(data["Links"]["Last"].split("=")[-1]) >= next_start:
-                params["start"] = next_start
+                params["start"] = next_start  # noqa
             else:
                 done = True
         return ret
 
     def _get_tag_metadata(self, tag: str) -> Dict[str, str]:
         return {}  # FIXME
 
@@ -857,29 +857,29 @@
         ]:
             return True
         return False
 
     def read_tag(
         self,
         tag: str,
-        start_time: Optional[datetime],
-        stop_time: Optional[datetime],
+        start: Optional[datetime],
+        end: Optional[datetime],
         sample_time: timedelta,
         read_type: ReaderType,
         metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         webid = self.tag_to_webid(tag)
         if not webid:
             return pd.DataFrame()
 
         (url, params) = self.generate_read_query(
             tag=webid,
-            start_time=start_time,
-            stop_time=stop_time,
+            start=start,
+            end=end,
             sample_time=sample_time,
             read_type=read_type,
             metadata={},
             get_status=get_status,
         )
         url = urljoin(self.base_url, url)
         data = self.fetch(url, params=params)
@@ -914,38 +914,46 @@
                     "Value.Substituted": "Substituted",
                 }
             )
 
         df = df.filter(["Timestamp", "Value", "Good", "Questionable", "Substituted"])
 
         try:
+            # Could call this here, to support mixed format, but have not checked performance
+            # df["Timestamp"] = pd.to_datetime(df["Timestamp"], format='ISO8601', utc=True)
             if read_type == ReaderType.RAW or read_type == ReaderType.SNAPSHOT:
                 # Sub-second timestamps are common
                 df["Timestamp"] = pd.to_datetime(
                     df["Timestamp"], format="%Y-%m-%dT%H:%M:%S.%fZ", utc=True
                 )
             else:
                 # Sub-second timestamps are uncommon
                 df["Timestamp"] = pd.to_datetime(
                     df["Timestamp"], format="%Y-%m-%dT%H:%M:%SZ", utc=True
                 )
         except ValueError:
-            df["Timestamp"] = pd.to_datetime(df["Timestamp"], utc=True)
+            try:
+                df["Timestamp"] = pd.to_datetime(df["Timestamp"], utc=True)
+            except ValueError:
+                #  Handle when both second and sub-second data is returned
+                df["Timestamp"] = pd.to_datetime(
+                    df["Timestamp"], format="ISO8601", utc=True
+                )
 
         if read_type == ReaderType.VAR:
             df["Value"] = df["Value"] ** 2
 
         df = df.set_index("Timestamp", drop=True)
         df.index.name = "time"
         # df = df.tz_localize("UTC")
 
         # Correct weird bug in PI Web API where MAX timestamps end of interval while
         # all the other summaries stamp start of interval by shifting all timestamps
         # one interval down.
-        if read_type == ReaderType.MAX and df.index[0] > start_time:
+        if read_type == ReaderType.MAX and df.index[0] > start:
             df.index = df.index - sample_time
 
         if get_status:
             df["Status"] = (
                 # Values are boolean, but no need to do .astype(int)
                 df["Questionable"]
                 + 2 * (1 - df["Good"])
```

### Comparing `tagreader-4.2.0/PKG-INFO` & `tagreader-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.2.0
+Version: 4.2.1
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
```

