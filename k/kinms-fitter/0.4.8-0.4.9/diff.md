# Comparing `tmp/kinms_fitter-0.4.8.tar.gz` & `tmp/kinms_fitter-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinms_fitter-0.4.8.tar", last modified: Wed Apr 12 14:54:11 2023, max compression
+gzip compressed data, was "kinms_fitter-0.4.9.tar", last modified: Wed Jul 12 13:02:42 2023, max compression
```

## Comparing `kinms_fitter-0.4.8.tar` & `kinms_fitter-0.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-12 14:54:11.051556 kinms_fitter-0.4.8/
--rw-r--r--   0 tdavis     (501) staff       (20)    35149 2021-01-07 12:48:31.000000 kinms_fitter-0.4.8/LICENSE
--rw-r--r--   0 tdavis     (501) staff       (20)     2079 2023-04-12 14:54:11.051346 kinms_fitter-0.4.8/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)     1530 2022-08-24 14:57:04.000000 kinms_fitter-0.4.8/README.md
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-12 14:54:11.049847 kinms_fitter-0.4.8/kinms_fitter/
--rwxr--r--   0 tdavis     (501) staff       (20)      291 2022-08-24 14:32:42.000000 kinms_fitter-0.4.8/kinms_fitter/__init__.py
--rwxr--r--   0 tdavis     (501) staff       (20)     9679 2023-04-06 14:09:43.000000 kinms_fitter-0.4.8/kinms_fitter/diskThick_funcs.py
--rwxr--r--   0 tdavis     (501) staff       (20)    41289 2023-04-05 16:30:58.000000 kinms_fitter-0.4.8/kinms_fitter/kinms_fitter.py
--rwxr--r--   0 tdavis     (501) staff       (20)    40353 2023-03-08 15:55:21.000000 kinms_fitter-0.4.8/kinms_fitter/kinms_fitter_old.py
--rwxr--r--   0 tdavis     (501) staff       (20)     1680 2023-02-15 10:57:33.000000 kinms_fitter-0.4.8/kinms_fitter/prior_funcs.py
--rwxr--r--   0 tdavis     (501) staff       (20)    17929 2023-04-06 16:00:06.000000 kinms_fitter-0.4.8/kinms_fitter/sb_profs.py
--rw-r--r--   0 tdavis     (501) staff       (20)     2342 2023-02-21 14:38:07.000000 kinms_fitter-0.4.8/kinms_fitter/transformClouds.py
--rwxr--r--   0 tdavis     (501) staff       (20)    37043 2023-03-31 08:43:11.000000 kinms_fitter-0.4.8/kinms_fitter/velocity_profs.py
--rwxr--r--   0 tdavis     (501) staff       (20)     9608 2023-02-21 14:38:22.000000 kinms_fitter-0.4.8/kinms_fitter/warp_funcs.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-12 14:54:11.050904 kinms_fitter-0.4.8/kinms_fitter.egg-info/
--rw-r--r--   0 tdavis     (501) staff       (20)     2079 2023-04-12 14:54:10.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)      498 2023-04-12 14:54:10.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-04-12 14:54:10.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       82 2023-04-12 14:54:10.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/requires.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       13 2023-04-12 14:54:10.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2021-01-07 12:53:57.000000 kinms_fitter-0.4.8/kinms_fitter.egg-info/zip-safe
--rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-04-12 14:54:11.051605 kinms_fitter-0.4.8/setup.cfg
--rw-r--r--   0 tdavis     (501) staff       (20)     1056 2023-04-12 14:53:44.000000 kinms_fitter-0.4.8/setup.py
+drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.783744 kinms_fitter-0.4.9/
+-rw-r--r--   0 tdavis     (503) staff       (20)        0 2021-01-07 12:48:31.000000 kinms_fitter-0.4.9/LICENSE
+-rw-r--r--   0 tdavis     (503) staff       (20)      575 2023-07-12 13:02:42.783585 kinms_fitter-0.4.9/PKG-INFO
+-rw-r--r--   0 tdavis     (503) staff       (20)        0 2022-08-24 14:57:04.000000 kinms_fitter-0.4.9/README.md
+drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.782609 kinms_fitter-0.4.9/kinms_fitter/
+-rwxr--r--   0 tdavis     (503) staff       (20)      291 2022-08-24 14:32:42.000000 kinms_fitter-0.4.9/kinms_fitter/__init__.py
+-rwxr--r--   0 tdavis     (503) staff       (20)     9679 2023-04-06 14:09:43.000000 kinms_fitter-0.4.9/kinms_fitter/diskThick_funcs.py
+-rwxr--r--   0 tdavis     (503) staff       (20)    41273 2023-07-12 12:58:40.000000 kinms_fitter-0.4.9/kinms_fitter/kinms_fitter.py
+-rwxr--r--   0 tdavis     (503) staff       (20)    40353 2023-03-08 15:55:21.000000 kinms_fitter-0.4.9/kinms_fitter/kinms_fitter_old.py
+-rwxr--r--   0 tdavis     (503) staff       (20)     1680 2023-02-15 10:57:33.000000 kinms_fitter-0.4.9/kinms_fitter/prior_funcs.py
+-rwxr--r--   0 tdavis     (503) staff       (20)    17861 2023-06-01 08:47:13.000000 kinms_fitter-0.4.9/kinms_fitter/sb_profs.py
+-rw-r--r--   0 tdavis     (503) staff       (20)     2342 2023-02-21 14:38:07.000000 kinms_fitter-0.4.9/kinms_fitter/transformClouds.py
+-rwxr--r--   0 tdavis     (503) staff       (20)    37043 2023-03-31 08:43:11.000000 kinms_fitter-0.4.9/kinms_fitter/velocity_profs.py
+-rwxr--r--   0 tdavis     (503) staff       (20)     9608 2023-02-21 14:38:22.000000 kinms_fitter-0.4.9/kinms_fitter/warp_funcs.py
+drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.783410 kinms_fitter-0.4.9/kinms_fitter.egg-info/
+-rw-r--r--   0 tdavis     (503) staff       (20)      575 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (503) staff       (20)      498 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (503) staff       (20)        1 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (503) staff       (20)       82 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (503) staff       (20)       13 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (503) staff       (20)        0 2021-01-07 12:53:57.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/zip-safe
+-rw-r--r--   0 tdavis     (503) staff       (20)       38 2023-07-12 13:02:42.783789 kinms_fitter-0.4.9/setup.cfg
+-rw-r--r--   0 tdavis     (503) staff       (20)     1056 2023-07-12 12:58:53.000000 kinms_fitter-0.4.9/setup.py
```

### Comparing `kinms_fitter-0.4.8/kinms_fitter/diskThick_funcs.py` & `kinms_fitter-0.4.9/kinms_fitter/diskThick_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/kinms_fitter/kinms_fitter.py` & `kinms_fitter-0.4.9/kinms_fitter/kinms_fitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
         phasecen=[xc,yc]
         
         
         pa=warp_funcs.eval(self.pa_profile,self.sbRad,param[5:5+self.n_pavars])
         inc=warp_funcs.eval(self.inc_profile,self.sbRad,param[5+self.n_pavars:5+self.n_pavars+self.n_incvars])
 
         if len(self.skySampClouds) >0:
-            inClouds=transformClouds(self.skySampClouds[:,0:3],posAng = pa,inc = inc,cent = phasecen,sbRad=self.sbRad)
+            inClouds=transformClouds(self.skySampClouds[:,0:3],posAng = pa,inc = inc,sbRad=self.sbRad)
             sbprof=None
             myargs={'vPhaseCent': phasecen,'inClouds': inClouds, 'flux_clouds': self.skySampClouds[:,3]}
         else:
             if np.any([callable(i.thicknessfunc) for i in self.sb_profile]):
                 inClouds=sb_profs.model(self.sb_profile,self.sbRad,param[5+self.n_pavars+self.n_incvars:5+self.n_pavars+self.n_incvars+self.n_sbvars],self.nSamps)
                 myargs={'vPhaseCent': phasecen,'inClouds': inClouds}
                 sbprof=None
```

### Comparing `kinms_fitter-0.4.8/kinms_fitter/kinms_fitter_old.py` & `kinms_fitter-0.4.9/kinms_fitter/kinms_fitter_old.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/kinms_fitter/prior_funcs.py` & `kinms_fitter-0.4.9/kinms_fitter/prior_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/kinms_fitter/sb_profs.py` & `kinms_fitter-0.4.9/kinms_fitter/sb_profs.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,14 @@
                 if len(inClouds)==0:
                     inClouds=theseinClouds.copy()
                 else:
                     inClouds=np.concatenate((inClouds,theseinClouds))
                 
             ilast+=model.freeparams
             
-        
-        if len(inClouds)>5e5:
-            breakpoint()    
         return inClouds    
     
     class expdisk:  
         """
         Creates an exponentially declining surface brightness profile.     
         
         Inputs
```

### Comparing `kinms_fitter-0.4.8/kinms_fitter/transformClouds.py` & `kinms_fitter-0.4.9/kinms_fitter/transformClouds.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/kinms_fitter/velocity_profs.py` & `kinms_fitter-0.4.9/kinms_fitter/velocity_profs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/kinms_fitter/warp_funcs.py` & `kinms_fitter-0.4.9/kinms_fitter/warp_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.8/setup.py` & `kinms_fitter-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='kinms_fitter',
-       version='0.4.8',
+       version='0.4.9',
        description='Wrapper for KinMSpy that automates most common galaxy fitting tasks',
        url='https://github.com/TimothyADavis/KinMS_fitter',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='GNU GPLv3',
```

