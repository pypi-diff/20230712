# Comparing `tmp/pylib_essentials-0.0.1.tar.gz` & `tmp/pylib_essentials-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib_essentials-0.0.1.tar", last modified: Fri Jun 16 20:55:48 2023, max compression
+gzip compressed data, was "pylib_essentials-0.0.2.tar", last modified: Wed Jul 12 20:47:45 2023, max compression
```

## Comparing `pylib_essentials-0.0.1.tar` & `pylib_essentials-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lcui01   (216616) vims     (50001)        0 2023-06-16 20:55:48.203920 pylib_essentials-0.0.1/
--rw-r--r--   0 lcui01   (216616) vims     (50001)      218 2023-06-16 20:55:48.192920 pylib_essentials-0.0.1/PKG-INFO
--rw-r--r--   0 lcui01   (216616) vims     (50001)      292 2023-06-15 20:52:38.000000 pylib_essentials-0.0.1/README.md
-drwxr-xr-x   0 lcui01   (216616) vims     (50001)        0 2023-06-16 20:55:47.867918 pylib_essentials-0.0.1/pylib_essentials/
--rw-r--r--   0 lcui01   (216616) vims     (50001)        0 2023-06-15 20:52:38.000000 pylib_essentials-0.0.1/pylib_essentials/__init__.py
--rw-r--r--   0 lcui01   (216616) vims     (50001)   157407 2023-06-15 20:52:39.000000 pylib_essentials-0.0.1/pylib_essentials/schism_file.py
-drwxr-xr-x   0 lcui01   (216616) vims     (50001)        0 2023-06-16 20:55:48.176920 pylib_essentials-0.0.1/pylib_essentials.egg-info/
--rw-r--r--   0 lcui01   (216616) vims     (50001)      218 2023-06-16 20:55:46.000000 pylib_essentials-0.0.1/pylib_essentials.egg-info/PKG-INFO
--rw-r--r--   0 lcui01   (216616) vims     (50001)      278 2023-06-16 20:55:46.000000 pylib_essentials-0.0.1/pylib_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 lcui01   (216616) vims     (50001)        1 2023-06-16 20:55:46.000000 pylib_essentials-0.0.1/pylib_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 lcui01   (216616) vims     (50001)       30 2023-06-16 20:55:46.000000 pylib_essentials-0.0.1/pylib_essentials.egg-info/requires.txt
--rw-r--r--   0 lcui01   (216616) vims     (50001)       17 2023-06-16 20:55:46.000000 pylib_essentials-0.0.1/pylib_essentials.egg-info/top_level.txt
--rw-r--r--   0 lcui01   (216616) vims     (50001)       38 2023-06-16 20:55:48.204920 pylib_essentials-0.0.1/setup.cfg
--rw-r--r--   0 lcui01   (216616) vims     (50001)      391 2023-06-15 20:52:39.000000 pylib_essentials-0.0.1/setup.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.840634 pylib_essentials-0.0.2/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 20:47:45.830634 pylib_essentials-0.0.2/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.2/README.md
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.667633 pylib_essentials-0.0.2/pylib_essentials/
+-rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.2/pylib_essentials/__init__.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)   184895 2023-07-11 15:23:30.000000 pylib_essentials-0.0.2/pylib_essentials/schism_file.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.826634 pylib_essentials-0.0.2/pylib_essentials.egg-info/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      278 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       42 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/requires.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/top_level.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-12 20:47:45.840634 pylib_essentials-0.0.2/setup.cfg
+-rw-r--r--   0 feiye    (49086) vims     (50001)      391 2023-07-12 20:47:40.000000 pylib_essentials-0.0.2/setup.py
```

### Comparing `pylib_essentials-0.0.1/pylib_essentials/schism_file.py` & `pylib_essentials-0.0.2/pylib_essentials/schism_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 #/usr/bin/env python3
+import os
+import sys
 from numpy import array, array_equal, argsort, arange, c_, r_, diff,\
   sort, unique, zeros, ones, setdiff1d, fliplr, flipud, tile, nonzero,\
-  nan, isnan, loadtxt, savetxt, load, linspace, meshgrid, concatenate
+  nan, isnan, loadtxt, savetxt, load, linspace, meshgrid, concatenate,\
+  squeeze, mod, angle, pi, sign
 from matplotlib.pyplot import figure, show, savefig, tricontour,\
     tricontourf, tripcolor, colorbar, gca, gcf, plot, axis, xlim, ylim,\
     triplot, title, xlabel, ylabel, gca, gcf, setp, getp, close
 import matplotlib.cm as cm
 import matplotlib as mpl
+try:
+    from pylib_utils.utility_functions import proj
+except:
+    print("projection module not found; install pylib_utils")
+
+# for experimental features
+import numpy as np
+import pickle
+import pandas as pd
+import copy
+import scipy
+import unittest
+
 
 class schism_grid:
     def __init__(self, fname=None):
         '''
         Initialize to empty instance if fname is not provided;
         otherwise, read from three supported file format
         '''
@@ -3198,9 +3214,666 @@
         #resize window
         wd.geometry('600x180'); wd.update(); xm=max([i.winfo_width() for i in fms])
         for i in arange(0,100,3):
             L1['text']=' '*i; L2['text']=' '*i; wd.update(); xs=fms[-1].winfo_width()
             if xs>xm: wd.geometry('{}x210'.format(xs)); wd.update(); break
         return wd,w
 
-if __name__=="__main__":
-    pass
+# -------------------------------------experimental-------------------------------------
+def combine_dataframes(A, B, weights=[1.0, 1.0]):
+    import numbers
+
+    AB = copy.deepcopy(A)
+
+    # warn if B's time period does not contain A's time
+    if B.index[0] > A.index[0] or B.index[-1] < A.index[-1]:
+        print('Warning: B\'s time period does not contain A\'s time period')
+        print('In the interpolated B, NaN will be filled for the time period that is not covered by B')
+        print('and the NaN in the interpolated B will be treated as 0 when summing up')
+
+    # Interpolate B to A's index 
+    B_interpolated = B.reindex(A.index).interpolate(method='time')
+
+    # Find the columns that are in B but not in A
+    new_columns = B_interpolated.columns.difference(A.columns)
+
+    # append these columns to A
+    AB = pd.concat([A, B_interpolated[new_columns]], axis=1)
+
+    # Find the common columns in A and B
+    common_columns = A.columns.intersection(B_interpolated.columns)
+
+    # Sum the values from both dataframes for the common columns
+    if isinstance(weights[0], numbers.Number):
+        AB[common_columns] = weights[0] * A[common_columns] + weights[1] * B_interpolated[common_columns]
+    elif isinstance(weights[0], TimeHistory):
+        vs_A = weights[0].df[common_columns]
+        vs_B = weights[1].df[common_columns]
+        vs_B = vs_B.reindex(vs_A.index).interpolate(method='time')
+        weights_A = vs_A / (vs_A + vs_B)
+        weights_B = vs_B / (vs_A + vs_B)
+        AB[common_columns] = weights_A * A[common_columns] + weights_B * B_interpolated[common_columns]
+    else:
+        raise ValueError('weights must be a list of two numbers or two TimeHistory objects')
+
+    return AB
+
+class TimeHistory():
+    """Class for handling SCHISM's *.th file format.
+    A *.th file is a simple ascii file containing time series data,
+    the 1st column is time in seconds or days,
+    the 2nd to last column is data, so each column is a time series.
+    However, the *.th file itself lacks information about the time units and start time
+    and this class is to bind those information in a dataframe.
+    The class also sets the time column as the index of the dataframe
+    and assign each data column with a name (e.g., station name)
+    to facilitate data queries and processing.
+    """
+    @property
+    def time(self):
+        # original time in *th's format
+        seconds = (self.df.index - self.df.index[0]).total_seconds().values
+        t = seconds / self.sec_per_time_unit
+        return t
+
+    @property
+    def n_time(self):
+        return self.df.shape[0]
+    
+    @property
+    def n_station(self):
+        return self.df.shape[1]
+    
+    @property
+    def data(self):
+        # original data excluding time
+        return self.df.values
+
+    def __init__(self, start_time_str="2000-01-01 00:00:00", data_array=None, columns=None, th_unit='seconds'):
+        """
+        Initialize a TimeHistory object from a data array,
+        assuming the first column is time, and the rest are data.
+        Note that you need to provide the start time and the time unit.
+        """
+
+        # list of main attributes
+        self.df = pd.DataFrame(data_array)
+        self.sec_per_time_unit = None
+        self.meaningful_columns = False  # some functions only work when column names are meaningful,
+                                         # e.g., station names or element ids, but not datetime + column numbers
+
+        # set time unit
+        unit_dict = {'seconds': 1, 'minutes': 60, 'hours': 3600, 'days': 86400, 'weeks': 604800, 'years': 31536000}
+        self.sec_per_time_unit = unit_dict[th_unit]  # only related to the time column of a *.th file
+
+        # set column names, which usually are datetime + station ids
+        if type(columns) is list:  # from a user-specified list
+            if len(columns) == self.df.shape[1]:
+                self.df.columns = [str(x) for x in columns]
+                self.meaningful_columns = True
+            elif len(columns) == self.df.shape[1]-1:
+                print('number of column labels does not match the data array, assuming the first column of the data is time')
+                self.df.columns = [str(x) for x in ['datetime'] + columns]
+                self.meaningful_columns = True
+            else:
+                raise Exception('number of columns does not match')
+        elif columns is None:  # first col is time and the rest are column numbers
+            self.df.columns = ['datetime'] + [str(x) for x in range(1, self.df.shape[1])]
+            self.meaningful_columns = False
+        else:
+            raise Exception('unknown columns type')
+
+        # Lay some ground rules
+        # force the first column's name to "datetime"
+        self.df.rename(columns={0: 'datetime'}, inplace=True)
+        second_series = self.df['datetime'].values * self.sec_per_time_unit
+        # convert the first column to pandas DatetimeIndex
+        time_stamps = pd.to_timedelta(second_series, unit='s') + pd.to_datetime(start_time_str)
+        self.df['datetime'] = time_stamps
+        # set datetime as index
+        self.df.set_index('datetime', inplace=True)
+        # force column names to be string
+        self.df.columns = self.df.columns.map(str)
+
+    @classmethod
+    def from_file(cls, file_name, start_time_str="2000-01-01 00:00:00", th_unit='seconds', columns=None):
+        """
+        Initialize from a file.
+        Note that the *.th file doen't have information about the time units and start time,
+        and columns names, so you need to provide them.
+        """
+        data = np.loadtxt(file_name)
+        return cls(data_array=data, th_unit=th_unit, start_time_str=start_time_str, columns=columns)
+    
+    def __add__(self, other, weights=[1.0, 1.0]):
+        """
+        Add two TimeHistory objects together
+        Interpolate other to self's time stamps;
+        other attributes also inherit from self.
+        When combining columns with the same name,
+        the default weights are 1.0 for both self and other,
+        meaning that the values are summed up.
+        if you want to average the values, set weights=[0.5, 0.5]
+        You can also specify two TimeHistory objects as the surrogates of the weights,
+        e.g., when combining two sets of msource, you can set weights=[vsource1, vsource2],
+        i.e., a weighted average based on the volume of the two sources,
+        """
+
+        A = copy.deepcopy(self)
+        B = other
+
+        A.df = combine_dataframes(A.df, B.df, weights=weights)
+
+        return A
+    
+    def __eq__(self, other) -> bool:
+        """Check if two TimeHistory objects are equal"""
+        for att in ['sec_per_time_unit']:
+            if getattr(self, att) != getattr(other, att):
+                print(f'{att} is not equal')
+                return False
+
+        # dataframes, strict test
+        # return self.df.equals(other.df)
+
+        # test if the data are equal within a tolerance
+        if np.any(self.df.columns != other.df.columns):
+            print('column labels are not equal')
+            return False
+        return np.allclose(self.df, other.df, rtol=0.001, atol=0.0001)
+    
+    def writer(self, file_name, np_savetxt_args={'fmt':'%.4f', 'delimiter':' ', 'newline':'\n'}):
+        # assemble data array in *.th format and write to file
+        np.savetxt(file_name, np.c_[self.time, self.data], **np_savetxt_args)
+
+
+class SourceSinkIn():
+    def __init__(self, ele_groups=[[], []]):
+        self.ele_groups = ele_groups  # 0: source; 1: sink
+    
+    @property
+    def n_group(self):
+        return len(self.ele_groups)
+
+    @property
+    def np_group(self):
+        return [len(x) for x in self.ele_groups]
+
+    @property
+    def ip_group(self):
+        return [np.array(x) for x in self.ele_groups]
+    
+    @property
+    def n_source(self):
+        return self.np_group[0]
+    
+    @property
+    def n_sink(self):
+        return self.np_group[1]
+
+    @classmethod
+    def from_file(cls, filename):
+        ele_groups = [[], []]
+        with open(filename, 'r') as file:
+            for k in range(0, 2):  # 0: source; 1: sink
+                num_points = int(file.readline().strip().split()[0])
+                for _ in range(num_points):
+                    ele_groups[k].append(int(file.readline().strip().split()[0]))
+                # blank line between groups
+                if k == 0:
+                    file.readline()
+        source_sink_in = cls(ele_groups=ele_groups)
+        source_sink_in.print_info()
+
+        return source_sink_in
+    
+    def print_info(self):
+        print(f"nsource: {self.n_source}")
+        if self.n_source > 0:
+            print(f"first and last ele: {self.ele_groups[0][0]}, {self.ele_groups[0][-1]}")
+
+        print(f"nsink: {self.n_sink}")
+        if self.n_sink > 0:
+            print(f"first and last ele: {self.ele_groups[1][0]}, {self.ele_groups[1][-1]}")
+
+    def writer(self, filename=None):
+        with open(filename, 'w') as fout:
+            for k in range(0, self.n_group):
+                print("Points in Group " + str(k+1) + ": " + str(self.np_group[k]))
+                fout.write(f"{self.np_group[k]}\n")
+                for i in range(0, self.np_group[k]):
+                    fout.write(f"{self.ele_groups[k][i]}\n")
+                fout.write("\n")  # empty line
+
+    def __eq__(self, other) -> bool:
+        for g1, g2 in zip(self.ele_groups, other.ele_groups):
+            if g1.tolist() != g2.tolist():
+                return False
+        return True
+
+
+class source_sink():
+    """
+    Class for handling all source/sink inputs:
+
+    source_sink.in,
+    vsource.th,
+    vsink.th,
+    msource.th
+
+    These files are always used together,
+    so a class is created to bind and process them,
+    for example, adding or comparing two source_sink objects
+
+    In addition, there are no complete time info in the *.th files,
+    so the TimeHistory class is also used to bind the time info and
+    provide additional functions.
+    """
+    @property
+    def source_eles(self):
+        return self.source_sink_in.ele_groups[0]
+    
+    @property
+    def sink_eles(self):
+        return self.source_sink_in.ele_groups[1]
+    
+    @property
+    def nsource(self):
+        return self.source_sink_in.n_source
+    
+    @property
+    def nsink(self):
+        return self.source_sink_in.n_sink
+
+    def __init__(self, vsource:TimeHistory, vsink:TimeHistory, msource:list):
+        """initialize from TimeHistory objects,
+        vsource: TimeHistory object for volume source
+        vsink: TimeHistory object for volume sink
+        msource: list of TimeHistory objects for mass source
+        
+        Note that msource is different from SCHISM's native msource.th
+        because saving all tracers in one array is not convenient for 
+        subsequent processing; instead, each tracer is saved in a separate 
+        TimeHistory object in a list
+        """
+
+        # list of main attributes
+        self.vsource = vsource
+        self.vsink = vsink
+        self.msource = msource
+        self.ntracers = None
+        self.source_sink_in = None
+                        
+        # if vsource, vsink, and msources are properly set,
+        # then ntracers and source_sink_in will be automatically set
+        if vsource is not None:
+            self.ntracers = len(msource)
+            source_eles = vsource.df.columns.astype(int).values
+        else:
+            self.ntracers = 0
+            source_eles = []
+        if vsink is not None:
+            sink_eles = vsink.df.columns.astype(int).values
+        else:
+            sink_eles = []
+
+        self.source_sink_in = SourceSinkIn(ele_groups=[source_eles, sink_eles])
+
+    @classmethod
+    def dummy(cls, start_time_str='2000-01-01 00:00:00', timedeltas=[0.0, 86400.0*365*100],
+                 source_eles=[], sink_eles=[], ntracers=2):
+        """create a dummy source_sink object for testing purpose"""
+
+        # Sanity check
+        if vsource_data is None:
+            vsource_data = np.zeros([nt, nsources])
+        else:
+            if len(source_eles) != vsource_data.shape[1] + 1:
+                raise ValueError("source_eles and vsource_data must have the same number of elements")
+        if vsink_data is None:
+            vsink_data = np.zeros([nt, nsinks])
+        else:
+            if len(sink_eles) != vsink_data.shape[1] + 1:
+                raise ValueError("sink_eles and vsink_data must have the same number of elements")  
+
+        # initialize a set of source/sink files from scratch
+        nt = len(timedeltas)
+        nsources = len(source_eles)
+        nsinks = len(sink_eles)
+        vsource = None
+        vsink = None
+        msource = [None] * ntracers
+
+        if nsources > 0:
+            vsource = TimeHistory(file_name=None, start_time_str=start_time_str,
+                                  data_array=np.c_[np.array(timedeltas), vsource_data],
+                                  columns=source_eles)
+            # dummy temperature, set to -9999, i.e., ambient temperature
+            msource[0] = TimeHistory(file_name=None, start_time_str=start_time_str,
+                                     data_array=np.c_[np.array(timedeltas), -9999*np.ones([nt, nsources])],
+                                     columns=source_eles)
+            # dummy salinity, set to 0
+            msource[1] = TimeHistory(file_name=None, start_time_str=start_time_str,
+                                     data_array=np.c_[np.array(timedeltas), np.zeros([nt, nsources])],
+                                     columns=source_eles)
+
+        if nsinks > 0:
+            vsink = TimeHistory(file_name=None, start_time_str=start_time_str,
+                               data_array=np.c_[np.array(timedeltas), vsink_data],
+                               columns=sink_eles)
+
+        return cls(vsource, vsink, msource)
+
+    @classmethod
+    def from_files(cls, source_dir, start_time_str='2000-01-01 00:00:00'):
+        '''
+        Initialize from existing source/sink files under the source_dir.
+        Note that these files don't have start time information,
+        and you need to provide it.
+        '''
+        vsource = None
+        msource = None
+        vsink = None
+
+        # ele_groups are defined in source_sink.in
+        source_sink_in = SourceSinkIn.from_file(filename=f"{source_dir}/source_sink.in")
+
+        if source_sink_in.n_source > 0:
+            print('reading vsource\n')
+            vsource = TimeHistory.from_file(
+                f"{source_dir}/vsource.th",
+                start_time_str=start_time_str,
+                columns=source_sink_in.ele_groups[0],  # source_eles, index starts from 1
+            )
+
+            print('reading msource\n')
+            msource_total = loadtxt(f"{source_dir}/msource.th")
+            msource_t = msource_total[:, 0]
+            ntracers = (msource_total.shape[1] - 1) / vsource.n_station
+            if (int(ntracers) != ntracers):
+                raise ValueError("Number of tracers must be an integer, vsource and msource don't match")
+            else:
+                ntracers = int(ntracers)
+
+            # Split msource_total into separate TimeHistory objects,
+            # one for each tracer. This facilitates subsequent processing.
+            msource = [None] * ntracers
+            for i in range(ntracers):
+                idx1 = i * vsource.n_station + 1
+                idx2 = (i + 1) * vsource.n_station + 1
+                msource[i] = TimeHistory(
+                    data_array=np.c_[msource_t, msource_total[:, idx1:idx2]],
+                    start_time_str=start_time_str,
+                    columns=source_sink_in.ele_groups[0]
+                )
+
+        if source_sink_in.n_sink > 0:
+            print('reading vsink\n')
+            vsink = TimeHistory.from_file(
+                f"{source_dir}/vsink.th",
+                start_time_str=start_time_str,
+                columns=source_sink_in.ele_groups[1]
+            )
+        
+        source_sink = cls(vsource, vsink, msource)
+        source_sink.check_consistency()
+        return source_sink
+    
+    def writer(self, source_dir):
+        '''
+        Write source/sink files to the source_dir.
+        '''
+        if not os.path.exists(source_dir):
+            os.makedirs(source_dir)
+
+        self.source_sink_in.writer(f"{source_dir}/source_sink.in")
+        if self.vsource is not None:
+            self.vsource.writer(f"{source_dir}/vsource.th")
+
+            msource_total = self.msource[0].time
+            for i in range(self.ntracers):
+                msource_total = np.c_[msource_total, self.msource[i].df.values]
+            np.savetxt(f"{source_dir}/msource.th", msource_total)
+
+        if self.vsink is not None:
+            self.vsink.writer(f"{source_dir}/vsink.th")
+        
+    def check_consistency(self):
+        # check consistency of source_sink_in and vsource/vsink/msource
+        if self.nsource == 0:
+            if self.vsource is not None:
+                raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
+        else:
+            if len(self.msource) != self.ntracers:
+                raise Exception('inconsistent number of sources in source_sink.in and msource.th')
+            if self.nsource != self.msource[0].n_station:
+                raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
+            if self.nsource != self.vsource.n_station:
+                raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
+            if np.min(self.vsource.df.values, axis=None) < 0:
+                raise Exception('vsource must be positive')
+        
+        if self.nsink == 0:
+            if self.vsink is not None:
+                raise Exception('inconsistent number of sinks in source_sink.in and vsink.th')
+        else:
+            if self.nsink != self.vsink.n_station:
+                raise Exception('inconsistent number of sinks in source_sink.in and vsink.th')  
+            if np.max(self.vsink.df.values, axis=None) > 0:
+                raise Exception('vsink must be negative')
+    
+    def __add__(self, other):
+        '''
+        Add source/sink other to source/sink self,
+        retaining self's time stamps.
+        '''
+        A = self
+        B = other
+
+        # sanity check
+        if A.nsource == 0 and B.nsource == 0 and A.nsink == 0 and B.nsink == 0:
+            raise Exception('both source and sink are empty')
+
+        # most cases are trivial unless both A and B have source
+        if A.nsource == 0 and B.nsource == 0:  # neither has source
+            vsource = None
+            msource = None
+        elif A.nsource == 0:  # only B has source
+            vsource = B.vsource
+            msource = B.msource
+        elif B.nsource == 0:  # only A has source
+            vsource = A.vsource
+            msource = A.msource
+        else:  # both have source
+            vsource = A.vsource + B.vsource  # using TimeHistory.__add__
+            msource = [None] * A.ntracers
+            for i in range(A.ntracers):  # also using TimeHistory.__add__, but with weights
+                msource[i] = A.msource[i].__add__(B.msource[i], weights=[A.vsource, B.vsource])
+        
+        # most cases are trivial unless both A and B have sink
+        if A.nsink == 0 and B.nsink == 0:  # neither has sink
+            vsink = None
+        elif A.nsink == 0:  # only B has sink
+            vsink = B.vsink
+        elif B.nsink == 0:  # only A has sink
+            vsink = A.vsink
+        else:  # both have sink
+            vsink = A.vsink + B.vsink  # using TimeHistory.__add__
+
+        return type(self)(vsource=vsource, vsink=vsink, msource=msource)
+
+    def __eq__(self, other):
+        for att in ['source_sink_in', 'vsource', 'vsink']:
+            if getattr(self, att) != getattr(other, att):
+                print(f'{att} not equal')
+                return False
+        for i, [ms_A, ms_B] in enumerate(zip(self.msource, other.msource)):
+            if ms_A != ms_B:
+                print('msource {i} not equal')
+                return False
+        return True
+
+# -------------------------------------temporarily copied from other files in pylib-------------------------------------
+def signa(x,y):
+    '''
+        compute signed area for triangles along the last dimension (x[...,0:3],y[...,0:3])
+    '''
+    if x.ndim==1:
+        area=((x[0]-x[2])*(y[1]-y[2])-(x[1]-x[2])*(y[0]-y[2]))/2
+    elif x.ndim==2:
+        # area=((x[:,0]-x[:,2])*(y[:,1]-y[:,2])-(x[:,1]-x[:,2])*(y[:,0]-y[:,2]))/2
+        area=((x[...,0]-x[...,2])*(y[...,1]-y[...,2])-(x[...,1]-x[...,2])*(y[...,0]-y[...,2]))/2
+    area=squeeze(area)
+    return area
+
+class zdata:
+    '''
+    self-defined data structure by Zhengui Wang.  Attributes are used to store data
+    '''
+    def __init__(self):
+        pass
+
+    @property
+    def VINFO(self):
+        return get_VINFO(self)
+
+def savez(fname,data,fmt=0):
+    '''
+    save data as self-defined python format
+       fmt=0: save data as *.npz (small filesize, reads slower)
+       fmt=1: save data as *.pkl (large filesize, reads faster)
+    if fname endswith *.npz or *.pkl, then fmt is reset to match fname
+    '''
+
+    #determine format
+    if fname.endswith('.npz'): fmt=0; fname=fname[:-4]
+    if fname.endswith('.pkl'): fmt=1; fname=fname[:-4]
+    if fmt==1: fname=fname+'.pkl'
+
+    #save data
+    if fmt==0:
+       #get all attribute
+       svars=list(data.__dict__.keys())
+       if 'VINFO' in svars: svars.remove('VINFO')
+
+       #check whether there are functions. If yes, change function to string
+       rvars=[]
+       for svar in svars:
+           if hasattr(data.__dict__[svar], '__call__'):
+              import cloudpickle
+              try:
+                 data.__dict__[svar]=cloudpickle.dumps(data.__dict__[svar])
+              except:
+                 print('function {} not saved'.format(svar))
+                 rvars.append(svar)
+       svars=setdiff1d(svars,rvars)
+
+       #check variable types for list,string,int and float
+       lvars=[]; tvars=[]; ivars=[]; fvars=[]
+       for svar in svars:
+           if isinstance(data.__dict__[svar],int): ivars.append(svar)
+           if isinstance(data.__dict__[svar],float): fvars.append(svar)
+           if isinstance(data.__dict__[svar],str): tvars.append(svar)
+           if isinstance(data.__dict__[svar],list):
+              lvars.append(svar)
+              data.__dict__[svar]=array(data.__dict__[svar],dtype='O')
+
+       #constrcut save_string
+       save_str='savez_compressed("{}" '.format(fname)
+       for svar in svars: save_str=save_str+',{}=data.{}'.format(svar,svar)
+       save_str=save_str+',_list_variables=lvars,_str_variables=tvars,_int_variables=ivars,_float_variables=fvars)'
+       exec(save_str)
+    elif fmt==1:
+       fid=open(fname,'wb'); pickle.dump(data,fid,pickle.HIGHEST_PROTOCOL); fid.close()
+
+def loadz(fname,svars=None):
+    '''
+    load self-defined data "fname.npz" or "fname.pkl"
+         svars: list of variables to be read
+    '''
+
+    if fname.endswith('.npz'):
+       #get data info
+       data0=load(fname,allow_pickle=True)
+       keys0=data0.keys() if svars is None else svars
+       ivars=list(data0['_int_variables']) if ('_int_variables' in keys0) else []
+       fvars=list(data0['_float_variables']) if ('_float_variables' in keys0) else []
+       tvars=list(data0['_str_variables']) if ('_str_variables' in keys0) else []
+       lvars=list(data0['_list_variables']) if ('_list_variables' in keys0) else []
+
+       #extract data
+       vdata=zdata()
+       for keyi in keys0:
+           if keyi in ['_list_variables','_str_variables','_int_variables','_float_variables']: continue
+
+           #get variable
+           datai=data0[keyi]
+           if datai.dtype==dtype('O'): datai=datai[()] #restore object
+           if keyi in ivars: datai=int(datai)          #restore int variable
+           if keyi in fvars: datai=float(datai)        #restore int variable
+           if keyi in tvars: datai=str(datai)          #restore str variable
+           if keyi in lvars: datai=datai.tolist()      #restore list variable
+
+           #if value is a function
+           if 'cloudpickle.cloudpickle' in str(datai):
+              import pickle
+              try:
+                 datai=pickle.loads(datai)
+              except:
+                 continue
+           vdata.__dict__[keyi]=datai
+    elif fname.endswith('.pkl'):
+       import pickle
+       vdata=zdata(); fid=open(fname,'rb')
+       data=pickle.load(fid)
+       vdata.__dict__=dcopy(data).__dict__.copy()
+       fid.close()
+    else:
+       sys.exit('unknown format: {}'.format(fname))
+    return vdata
+
+# ---------------------------- unit test ----------------------------
+class test_add_source_sink(unittest.TestCase):
+    def test_add_source_sink(self):
+        print('*************** test_add_source_sink ****************')
+        # read from prepared sample files
+        A = source_sink.from_files('/sciclone/data10/feiye/SCHISM_REPOSITORY/schism/src/Utility/Pre-Processing/STOFS-3D-Atl-shadow-VIMS/Pre_processing/Source_sink/Test_data/source_sink_sample1')
+        B = source_sink.from_files('/sciclone/data10/feiye/SCHISM_REPOSITORY/schism/src/Utility/Pre-Processing/STOFS-3D-Atl-shadow-VIMS/Pre_processing/Source_sink/Test_data/source_sink_sample2')
+        AB = source_sink.from_files('/sciclone/data10/feiye/SCHISM_REPOSITORY/schism/src/Utility/Pre-Processing/STOFS-3D-Atl-shadow-VIMS/Pre_processing/Source_sink/Test_data/source_sink_sample12')
+
+        A_add_B = A + B
+
+        self.assertEqual(A_add_B, AB)
+
+class test_combine_dataframes(unittest.TestCase):
+    def setUp(self):
+        # create some random time series for test
+        index_A = pd.date_range(start='2023-01-01', end='2023-12-31', freq='D')
+        index_B = pd.date_range(start='2023-01-01', end='2023-10-31', freq='3D')  # lower frequency
+        self.df_A = pd.DataFrame(np.random.rand(len(index_A), 3), index=index_A, columns=['A', 'B', 'C'])
+        self.df_B = pd.DataFrame(np.random.rand(len(index_B), 3), index=index_B, columns=['B', 'C', 'D'])
+
+    def test_combine_dataframes(self):
+        print('*************** test combine dataframes ****************')
+        df_combined = combine_dataframes(self.df_A, self.df_B)
+
+        print("First few rows of DataFrame A:")
+        print(self.df_A.head())
+        print("First few rows of DataFrame B:")
+        print(self.df_B.head())
+        print("First few rows of Combined DataFrame:")
+        print(df_combined.head())
+
+        # Check the shape of the resulting dataframe
+        self.assertEqual(df_combined.shape[0], self.df_A.shape[0])  # check row number
+        self.assertEqual(df_combined.shape[1], 4)  # check column number
+
+        # Check the column names of the resulting dataframe
+        self.assertTrue(all(np.isin(['A', 'B', 'C', 'D'], df_combined.columns)))  # check column names
+
+        # Check that the values of the resulting dataframe are correct
+        common_columns = self.df_A.columns.intersection(self.df_B.columns)
+        for col in common_columns:
+            self.assertTrue(all(np.isclose(df_combined[col].loc[self.df_B.index], self.df_A[col].loc[self.df_B.index] + self.df_B[col], atol=1e-5)))
+
+if __name__ == "__main__":
+    unittest.main()
```

