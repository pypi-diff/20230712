# Comparing `tmp/gemlog-1.7.1.tar.gz` & `tmp/gemlog-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemlog-1.7.1.tar", last modified: Fri Jun 23 18:55:10 2023, max compression
+gzip compressed data, was "gemlog-1.7.2.tar", last modified: Wed Jul 12 20:01:06 2023, max compression
```

## Comparing `gemlog-1.7.1.tar` & `gemlog-1.7.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 18:55:03.000000 gemlog-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 18:55:03.000000 gemlog-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-23 18:55:10.177071 gemlog-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-23 18:55:03.000000 gemlog-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66266 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/noise/
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/noise/Gem_v0.98_Noise_spec.txt
--rw-r--r--   0 runner    (1001) docker     (123)   118800 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/response/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/gemlog/data/response/datalogger/
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/gemlog/data/response/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gem_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gem_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7020 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemconvert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemconvert_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemlog_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/huddle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/parsers.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/xcorr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:55:10.177071 gemlog-1.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4343 2023-06-23 18:55:06.000000 gemlog-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.522261 gemlog-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 20:00:55.000000 gemlog-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 20:00:55.000000 gemlog-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-12 20:01:06.518261 gemlog-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-12 20:00:55.000000 gemlog-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67080 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/data/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/noise/Gem_v0.98_Noise_spec.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   118800 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/data/response/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/data/response/datalogger/
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog/data/response/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/gem_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/gem_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7020 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/gemconvert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/gemconvert_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/gemlog_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/huddle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/parsers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-07-12 20:00:57.000000 gemlog-1.7.2/gemlog/xcorr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:01:06.518261 gemlog-1.7.2/gemlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 20:01:06.000000 gemlog-1.7.2/gemlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:01:06.522261 gemlog-1.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-07-12 20:00:57.000000 gemlog-1.7.2/setup.py
```

### Comparing `gemlog-1.7.1/LICENSE` & `gemlog-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/PKG-INFO` & `gemlog-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemlog
-Version: 1.7.1
+Version: 1.7.2
 Summary: A set of functions for processing Gem datalogger files.
 Home-page: https://github.com/ajakef/gemlog
 Author: Jake Anderson
 Maintainer-email: ajakef@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gemlog-1.7.1/README.md` & `gemlog-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/__init__.py` & `gemlog-1.7.2/gemlog/__init__.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/core.py` & `gemlog-1.7.2/gemlog/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,15 +605,15 @@
                     'serial_output' : 0}) ## default config: it's fairly safe to use this as the default because any other configuration would require ...
     ## this is ugly but functional. pd.read_csv raises an exception when the number of columns is
     ## wrong, and the number of columns will be wrong for all rows except the C rows
     for j in range(10):
         try:
             line = pd.read_csv(fn, skiprows = j+1, nrows=1, delimiter = ',', dtype = 'str', names = ['na', 'gps_mode','gps_cycle','gps_quota','adc_range','led_shutoff','serial_output'], encoding_errors='ignore', on_bad_lines = 'skip')
             if line.iloc[0,0] == 'C':
-                config = {key:int(line[key]) for key in list(line.keys())[1:]}
+                config = {key:int(line.loc[0,key]) for key in list(line.keys())[1:]}
                 break
         except:
             pass
     return config
 
 
 def _find_nonmissing_files(path, SN, nums):
@@ -717,31 +717,36 @@
     # note that linetype has type bytes here, not str like in the pandas func
     df['linetype'] = types
     df['millis-sawtooth'] = millis
     #return _process_gemlog_data(df, offset)
     return df
 
 
-def _read_0_8_with_pandas(filename, require_gps = True):
+def _read_0_8_pd(filename, require_gps = True):
     ## This procedure is different enough from read_with_pandas that they are not interchangeable.
     # skiprows is important so that the header doesn't force dtype=='object'
     # the C engine for pd.read_csv is fast but crashes sometimes. Use the python engine as a backup.
     try:
-        df = pd.read_csv(filename, names=range(13), low_memory=False, skiprows=6, encoding_errors='ignore')
+        # read 15 columns for 'R,2' lines
+        df = pd.read_csv(filename, names=range(15), low_memory=False, skiprows=6, encoding_errors='ignore')
     except Exception:
         try:
-            df = pd.read_csv(filename, names=range(13), engine='python', skiprows=6,
+            df = pd.read_csv(filename, names=range(15), engine='python', skiprows=6,
                              on_bad_lines = 'skip', # replacement for error/warn_bad_lines, available since pandas 1.3.0
                              encoding_errors='ignore')
-        except:
-            raise CorruptRawFile(filename)
+        except Exception as exception_message:
+            raise CorruptRawFile('_read_0_8_pd; pd.read_csv: ' + str(exception_message))
     if df.shape[0] == 0:
         raise EmptyRawFile(filename)
 
-    df = df.iloc[np.where(~np.isnan(df.iloc[:,1]))[0],:]
+    ## some old data files have lines that are just a single character from a NMEA string. There's
+    ## a risk of an exception if they aren't dropped first.
+    df = df.loc[df.iloc[:,0].isin(['D', 'M', 'G']), :]
+    df[1] = df[1].astype(float) # weirdly, this doesn't work with iloc
+    df = df.iloc[np.where(~np.isnan(df.iloc[:,1]))[0],:] # error-prone if any "Nones" are in df[1]
     df['linetype'] = df.iloc[:,0].copy()
     df = df.iloc[:,1:]
     
     if ('G' not in set(df.loc[:,'linetype'])) and require_gps:
         raise CorruptRawFileNoGPS(filename)
     
     df = df.loc[df.loc[:,'linetype'].isin(['D', 'M', 'G']), :]
@@ -808,37 +813,40 @@
     """
     # Try each of the three file readers in order of decreasing speed but
     # probably increasing likelihood of success.
 
     if version in ['1.1', '0.91', '0.9', '0.85C']:
         readers = [ _read_with_cython, _read_with_pandas]#, _slow__read_single_v0_9 ]
     else:
-        readers = [_read_0_8_with_pandas]
+        readers = [_read_0_8_pd]
 
+    output_message = ''
     for reader in readers:
         try:
             df = reader(filename, require_gps)
             
             output = _process_gemlog_data(df, offset, version = version, require_gps = require_gps)
         except (EmptyRawFile, FileNotFoundError, CorruptRawFileNoGPS, KeyboardInterrupt):
             # If the file is definitely not going to work, exit early and
-            # re-raise the exception that caused the problem
+            # re-raise the exception that caused the problem.
+            # CorruptRawFile might work with a different reader so don't exit early.
             raise
-        except Exception:
+        except Exception as exception_message:
+            output_message = str(exception_message) + ': ' + filename
             pass
         else: # if we're here, the file read worked. it may be invalid though.
             if (len(output['gps'].lat) == 0) and require_gps:
                 raise CorruptRawFile(filename)
 
             # implement a small timing correction (depends on the raw format version)
             output['data'][:,0] += _time_corrections[version] 
             return output
 
 
-    raise CorruptRawFile(filename)
+    raise CorruptRawFile(output_message)
 
 def _process_gemlog_data(df, offset=0, version = '0.9', require_gps = True):
     ## figure out what settings to used according to the raw file format version
     if version in ['0.9', '0.85C']:
         rollover = 2**13
         M_cols = ['millis', 'batt', 'temp', 'A2', 'A3',
                   'maxWriteTime', 'minFifoFree', 'maxFifoUsed',
@@ -1060,16 +1068,18 @@
             
         except KeyboardInterrupt:
             raise
         except CorruptRawFileInadequateGPS:
             print('Insufficient GPS data in ' + fn + ', skipping this file')
         except CorruptRawFileNoGPS:
             print('No GPS data in ' + fn + ', skipping this file')
-        except:
-            print('Failed to read ' + fn + ', skipping this file')
+        except CorruptRawFile as exception_message:
+            print(f'Skipping corrupt raw file {fn}: {exception_message}')
+        except Exception as exception_message:
+            print(f'Failed to read {fn}, skipping this file: {exception_message}')
             _breakpoint()
         else:
             pass
         ## end of fn loop
     #_breakpoint()
     return {'metadata':M, 'gps':G, 'data': D, 'header': header}
```

### Comparing `gemlog-1.7.1/gemlog/data/noise/Gem_v0.98_Noise_spec.txt` & `gemlog-1.7.2/gemlog/data/noise/Gem_v0.98_Noise_spec.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt` & `gemlog-1.7.2/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100` & `gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100` & `gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100` & `gemlog-1.7.2/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005` & `gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016` & `gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023` & `gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022` & `gemlog-1.7.2/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/gem_cat.py` & `gemlog-1.7.2/gemlog/gem_cat.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/gem_network.py` & `gemlog-1.7.2/gemlog/gem_network.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/gemconvert.py` & `gemlog-1.7.2/gemlog/gemconvert.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/gemconvert_single.py` & `gemlog-1.7.2/gemlog/gemconvert_single.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/gemlog_aux.py` & `gemlog-1.7.2/gemlog/gemlog_aux.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/huddle_test.py` & `gemlog-1.7.2/gemlog/huddle_test.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/parsers.pyx` & `gemlog-1.7.2/gemlog/parsers.pyx`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog/version.py` & `gemlog-1.7.2/gemlog/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-__version__ = '1.7.1' # fixed verify_huddle_test bug with Axes.set_ticks 
+__version__ = '1.7.2' # minor improvements to data read functions (not important to most users), and dependency updates (scipy security issue, Python 3.11, build wheels on Ubuntu 22.04) 
+#__version__ = '1.7.1' # fixed verify_huddle_test bug with Axes.set_ticks 
 #__version__ = '1.7.0' # new command-line tool to make sensor network info, including a stationXML file 
 #__version__ = '1.6.9' # added command-line tools to cross-correlate data and invert time lags for slowness and backazimuth, fixed for pypi 
 #__version__ = '1.6.8' # added command-line tools to cross-correlate data and invert time lags for slowness and backazimuth 
 #__version__ = '1.6.7' # bug fix in verify_huddle_test 
 #__version__ = '1.6.6' # version described by JOSS paper 
 #__version__ = '1.6.5' # bug fixes and other minor improvements 
 #__version__ = '1.6.4' # upgrades dependencies due to moderate security issue in numpy: https://github.com/advisories/GHSA-fpfv-jqm9-f5jm 
@@ -59,8 +60,8 @@
 #__version__  = '0.3.2' # added demo with inventory functions
 #__version__  = '0.3.1' #  more helpful logging output
 #__version__  = '0.3.0' # 2020-09-04, cython added
 #__version__  = '0.2.3' # improving testing, including empty/bad files
 #__version__  = '0.2.2' # automated github tests, setup.py improvements, and modelst speed-up
 #__version__  = '0.2.1' # 
 #__version__ = '0.0.5' # added new functions to make network map from gps data and rename mseeds from serial_number.channel to network.station.location.channel codes
-## List of old versions is not comprehensive########################################################
+## List of old versions is not comprehensive#########################################################
```

### Comparing `gemlog-1.7.1/gemlog/xcorr.py` & `gemlog-1.7.2/gemlog/xcorr.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/gemlog.egg-info/PKG-INFO` & `gemlog-1.7.2/gemlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemlog
-Version: 1.7.1
+Version: 1.7.2
 Summary: A set of functions for processing Gem datalogger files.
 Home-page: https://github.com/ajakef/gemlog
 Author: Jake Anderson
 Maintainer-email: ajakef@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gemlog-1.7.1/gemlog.egg-info/SOURCES.txt` & `gemlog-1.7.2/gemlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.1/setup.py` & `gemlog-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,28 @@
 
 VERSION = version_dict['__version__']
 
 ## Dependency notes:
 ## Main version requirements
 # pandas: >= 1.3 (2021-07; earlier versions are incompatible with all gemlog. >=1.4 only works for gemlog >= 1.6.1)
 # numpy: >=1.22 (2022-06-22; earlier versions have security issue https://github.com/advisories/GHSA-fpfv-jqm9-f5jm).
-# scipy: >=1.4 (2022-11-22; 1.3.0 fails to install now, don't know why)
+# scipy: >=1.10 (2023-07-12; security issue)
 
 ## Secondary requirements
 # python: >=3.8 (2022-06-22; >=3.8 is required by numpy 1.22).
 # obspy: >=1.3 (2022-06-22; >=1.3 is required for numpy 1.22 compatibility)
 
 ## example range: pandas>=1.3.0,<1.4.0
 ## example exact: numpy==1.21
 INSTALL_REQUIRES = [
     'setuptools>=18.0', # 18.0 needed to handle cython in installation
     'obspy>=1.3',
     'numpy>=1.22', 
     'pandas>=1.3.0', 
-    'scipy>=1.4.0', # May 2019
+    'scipy>=1.10.0', # 1.10 for a security update in July 2023
     'matplotlib>=3.2.0', # March 2020
     'cython', # used for reading raw files quickly
     'fpdf' # needed for pdf huddle test reports
 ]
 
 TESTS_REQUIRE = ['pytest']
```

