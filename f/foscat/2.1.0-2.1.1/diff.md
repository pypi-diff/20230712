# Comparing `tmp/foscat-2.1.0.tar.gz` & `tmp/foscat-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-0uexk0g6/foscat-2.1.0.tar", last modified: Tue Jul 11 15:11:14 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-asrlb7_o/foscat-2.1.1.tar", last modified: Wed Jul 12 09:31:43 2023, max compression
```

## Comparing `foscat-2.1.0.tar` & `foscat-2.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 15:11:14.000000 foscat-2.1.0/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.1.0/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 15:11:14.000000 foscat-2.1.0/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 15:08:52.000000 foscat-2.1.0/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57613 2023-07-11 14:30:51.000000 foscat-2.1.0/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.1.0/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.1.0/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.1.0/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.1.0/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.1.0/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.1.0/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.1.0/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    33367 2023-07-11 15:05:00.000000 foscat-2.1.0/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.1.0/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    54003 2023-07-11 15:05:12.000000 foscat-2.1.0/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.1.0/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:31:43.000000 foscat-2.1.1/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.1.1/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-12 09:31:43.000000 foscat-2.1.1/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-12 09:31:05.000000 foscat-2.1.1/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57613 2023-07-11 14:30:51.000000 foscat-2.1.1/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.1.1/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.1.1/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.1.1/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.1.1/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    14492 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.1.1/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.1.1/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    35784 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.1.1/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    58573 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.1.1/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.1.0/PKG-INFO` & `foscat-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.1.0/README.md` & `foscat-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/setup.py` & `foscat-2.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.1.0',
+    version='2.1.1',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.1.0/src/foscat/FoCUS.py` & `foscat-2.1.1/src/foscat/FoCUS.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/GetGPUinfo.py` & `foscat-2.1.1/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/Rformat.py` & `foscat-2.1.1/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/Synthesis.py` & `foscat-2.1.1/src/foscat/Synthesis.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/backend.py` & `foscat-2.1.1/src/foscat/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,14 +168,34 @@
         else:
             if self.BACKEND==self.TENSORFLOW:
                 return(self.backend.reduce_mean(data,axis=axis))
             if self.BACKEND==self.TORCH:
                 return(self.backend.mean(data,axis))
             if self.BACKEND==self.NUMPY:
                 return(np.mean(data,axis))
+
+    def bk_reduce_std(self,data,axis=None):
+        
+        if isinstance(data,Rformat.Rformat):
+            return self.bk_reduce_std(data.get())
+        
+        if axis is None:
+            if self.BACKEND==self.TENSORFLOW:
+                return(self.backend.math.reduce_std(data))
+            if self.BACKEND==self.TORCH:
+                return(self.backend.std(data))
+            if self.BACKEND==self.NUMPY:
+                return(np.std(data))
+        else:
+            if self.BACKEND==self.TENSORFLOW:
+                return(self.backend.math.reduce_std(data,axis=axis))
+            if self.BACKEND==self.TORCH:
+                return(self.backend.std(data,axis))
+            if self.BACKEND==self.NUMPY:
+                return(np.std(data,axis))
         
     def bk_sqrt(self,data):
         
         if isinstance(data,Rformat.Rformat):
             return Rformat.Rformat(self.bk_sqrt(data.get()),data.off,0,chans=data.chans)
         
         return(self.backend.sqrt(self.backend.abs(data)))
```

### Comparing `foscat-2.1.0/src/foscat/build_demo.py` & `foscat-2.1.1/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/scat.py` & `foscat-2.1.1/src/foscat/scat.py`

 * *Files 8% similar despite different names*

```diff
@@ -426,14 +426,62 @@
     def mean(self):
         return abs(self.get_np(self.S0).mean()+ \
                    self.get_np(self.S1).mean()+ \
                    self.get_np(self.S2).mean()+ \
                    self.get_np(self.S2L).mean()+ \
                    self.get_np(self.P00).mean())/3
 
+    def iso_mean(self):
+        shape=list(self.S2.shape)
+        idx=np.zeros([shape[2]*shape[2]],dtype='int')
+        for i in range(shape[2]):
+            idx[i*shape[2]:(i+1)*shape[2]]=(np.arange(shape[2])+i)%shape[2]+np.arange(shape[2])*shape[2]
+
+        S1  = self.backend.bk_reduce_mean(self.S1,2)
+        P00 = self.backend.bk_reduce_mean(self.P00,2)
+        S2=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.S2,[shape[0],shape[1],shape[2]*shape[2]]),idx,2),
+                                      [shape[0],shape[1],shape[2],shape[2]])
+        S2L=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.S2L,[shape[0],shape[1],shape[2]*shape[2]]),idx,2),
+                                       [shape[0],shape[1],shape[2],shape[2]])
+
+        S2  =self.backend.bk_reduce_mean(S2,3)
+        S2L=self.backend.bk_reduce_mean(S2L,3)
+
+        return scat(P00,self.S0,S1,S2,S2L,backend=self.backend)
+
+
+    def iso_std(self,repeat=False):
+        shape=list(self.S2.shape)
+        idx=np.zeros([shape[2]*shape[2]],dtype='int')
+        for i in range(shape[2]):
+            idx[i*shape[2]:(i+1)*shape[2]]=(np.arange(shape[2])+i)%shape[2]+np.arange(shape[2])*shape[2]
+            
+        S1  = self.backend.bk_reduce_std(self.S1,2)
+        if repeat:
+            S1=self.backend.bk_reshape(self.backend.bk_repeat(S1,shape[2]),self.S1.shape)
+        P00 = self.backend.bk_reduce_std(self.P00,2)
+        if repeat:
+            P00=self.backend.bk_reshape(self.backend.bk_repeat(P00,shape[2]),self.S1.shape)
+        S2=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.S2,[shape[0],shape[1],shape[2]*shape[2]]),idx,2),
+                                      [shape[0],shape[1],shape[2],shape[2]])
+        S2L=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.S2L,[shape[0],shape[1],shape[2]*shape[2]]),idx,2),
+                                       [shape[0],shape[1],shape[2],shape[2]])
+
+        S2  =self.backend.bk_reduce_std(S2,3)
+        S2L=self.backend.bk_reduce_std(S2L,3)
+        if repeat:
+            S2=self.backend.bk_reshape(self.backend.bk_repeat(S2,shape[2]),self.S2.shape)
+            S2L=self.backend.bk_reshape(self.backend.bk_repeat(S2L,shape[2]),self.S2.shape)
+
+        return scat(P00,self.backend.bk_abs(self.S0),S1,S2,S2L,backend=self.backend)
+
     # ---------------------------------------------−---------
     def model(self,i__y,add=0,dx=3,dell=2,weigth=None,inverse=False):
 
         if i__y.shape[0]<dx+1:
             l__dx=i__y.shape[0]-1
         else:
             l__dx=dx
```

### Comparing `foscat-2.1.0/src/foscat/scat_cov.old.py` & `foscat-2.1.1/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat/scat_cov.py` & `foscat-2.1.1/src/foscat/scat_cov.py`

 * *Files 9% similar despite different names*

```diff
@@ -452,15 +452,15 @@
                             test=1
                             plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_1$' % (name), lw=lw)
                         else:
                             plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
             plt.yscale('log')
             plt.legend()
             plt.ylabel('S1')
-            plt.xlabel(r'$j_{1},\Theta_{1}$')
+            plt.xlabel(r'$j_{1}$')
 
         test=None
         plt.subplot(2, 2, 2)
         tmp=abs(self.get_np(self.P00))
         for k in range(tmp.shape[3]):
             for i1 in range(tmp.shape[0]):
                 for i2 in range(tmp.shape[0]):
@@ -654,14 +654,111 @@
                     abs(self.get_np(self.P00)).mean()) / 4
         else:  # Cross
             return (abs(self.get_np(self.C01)).mean() +
                     abs(self.get_np(self.C10)).mean() +
                     abs(self.get_np(self.C11)).mean() +
                     abs(self.get_np(self.P00)).mean()) / 4
 
+    def iso_mean(self):
+        shape=list(self.P00.shape)
+        norient=shape[3]
+
+        idx1=np.zeros([norient*norient],dtype='int')
+        for i in range(norient):
+            idx1[i*norient:(i+1)*norient]=(np.arange(norient)+i)%norient+i*norient
+
+        idx2=np.zeros([norient*norient*norient],dtype='int')
+        for i in range(norient):
+            for j in range(norient):
+                idx2[i*norient*norient+j*norient:i*norient*norient+(j+1)*norient]= \
+                    ((np.arange(norient)+i)%norient)*norient \
+                    +(np.arange(norient)+i+j)%norient+np.arange(norient)*norient*norient
+        S1=self.S1
+        if self.S1 is not None:
+            S1  = self.backend.bk_reduce_mean(self.S1,3)
+        P00 = self.backend.bk_reduce_mean(self.P00,3)
+
+        C01=self.C01
+        shape=list(self.C01.shape)
+        if self.C01 is not None:
+            C01=self.backend.bk_reshape(self.backend.bk_gather(
+                self.backend.bk_reshape(self.C01,[shape[0],shape[1],shape[2],norient*norient]),idx1,3),
+                                        [shape[0],shape[1],shape[2],norient,norient])
+            C01=self.backend.bk_reduce_mean(C01,4)
+        C10=self.C10
+        if self.C10 is not None:
+            C10=self.backend.bk_reshape(self.backend.bk_gather(
+                self.backend.bk_reshape(self.C10,[shape[0],shape[1],shape[2],norient*norient]),idx1,3),
+                                        [shape[0],shape[1],shape[2],norient,norient])
+            C10=self.backend.bk_reduce_mean(C10,4)
+
+        print(self.C11)
+        shape=list(self.C11.shape)
+        print(self.C11.shape,shape)
+        C11=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.C11,[shape[0],shape[1],shape[2],norient*norient*norient]),idx2,3),
+                                       [shape[0],shape[1],shape[2],norient,norient,norient])
+
+        C11=self.backend.bk_reduce_mean(C11,5)
+
+        return scat_cov(P00, C01, C11, s1=S1, c10=C10,backend=self.backend)
+
+
+    def iso_std(self,repeat=False):
+        shape=list(self.P00.shape)
+        norient=shape[3]
+
+        idx1=np.zeros([norient*norient],dtype='int')
+        for i in range(norient):
+            idx1[i*norient:(i+1)*norient]=(np.arange(norient)+i)%norient+i*norient
+
+        idx2=np.zeros([norient*norient*norient],dtype='int')
+        for i in range(norient):
+            for j in range(norient):
+                idx2[i*norient*norient+j*norient:i*norient*norient+(j+1)*norient]= \
+                    ((np.arange(norient)+i)%norient)*norient \
+                    +(np.arange(norient)+i+j)%norient+np.arange(norient)*norient*norient
+        S1=self.S1
+        if self.S1 is not None:
+            S1  = self.backend.bk_reduce_mean(self.S1,3)
+            if repeat:
+                S1=self.backend.bk_reshape(self.backend.bk_repeat(S1,norient),self.S1.shape)
+        P00 = self.backend.bk_reduce_mean(self.P00,3)
+        if repeat:
+            P00=self.backend.bk_reshape(self.backend.bk_repeat(P00,norient),self.P00.shape)
+
+        C01=self.C01
+        shape=list(self.C01.shape)
+        if self.C01 is not None:
+            C01=self.backend.bk_reshape(self.backend.bk_gather(
+                self.backend.bk_reshape(self.C01,[shape[0],shape[1],shape[2],norient*norient]),idx1,3),
+                                        [shape[0],shape[1],shape[2],norient,norient])
+            C01=self.backend.bk_reduce_mean(C01,4)
+            if repeat:
+                C01=self.backend.bk_reshape(self.backend.bk_repeat(C01,norient),self.C01.shape)
+        C10=self.C10
+        if self.C10 is not None:
+            C10=self.backend.bk_reshape(self.backend.bk_gather(
+                self.backend.bk_reshape(self.C10,[shape[0],shape[1],shape[2],norient*norient]),idx1,3),
+                                        [shape[0],shape[1],shape[2],norient,norient])
+            C10=self.backend.bk_reduce_mean(C10,4)
+            if repeat:
+                C10=self.backend.bk_reshape(self.backend.bk_repeat(C10,norient),self.C10.shape)
+
+        shape=list(self.C11.shape)
+        C11=self.backend.bk_reshape(self.backend.bk_gather(
+            self.backend.bk_reshape(self.C11,[shape[0],shape[1],shape[2],norient*norient*norient]),idx2,3),
+                                       [shape[0],shape[1],shape[2],norient,norient,norient])
+
+        C11=self.backend.bk_reduce_mean(C11,5)
+        if repeat:
+            C11=self.backend.bk_reshape(self.backend.bk_repeat(C11,norient),self.C11.shape)
+
+        return scat_cov(P00, C01, C11, s1=S1, c10=C10,backend=self.backend)
+
     def get_nscale(self):
         return self.P00.shape[2]
     
     def get_norient(self):
         return self.P00.shape[3]
 
     def add_data_from_log_slope(self,y,n,ds=3):
@@ -901,15 +998,15 @@
                 npix=nside*nside
             else:
                 npix = image1.shape[-1]  # image1 is [Npix] or [Nbatch, Npix]
                 nside = int(np.sqrt(npix / 12))
 
         J = int(np.log(nside) / np.log(2))  # Number of j scales
         Jmax = J - self.OSTEP  # Number of steps for the loop on scales
-
+        
         ### LOCAL VARIABLES (IMAGES and MASK)
         # Check if image1 is [Npix] or [Nbatch, Npix] or Rformat
         if len(image1.shape) == 1 or (len(image1.shape)==2 and self.chans==1) or (len(image1.shape) == 3 and isinstance(image1, Rformat.Rformat)):
             I1 = self.backend.bk_cast(self.backend.bk_expand_dims(image1, 0))  # Local image1 [Nbatch, Npix]
             if cross:
                 I2 = self.backend.bk_cast(self.backend.bk_expand_dims(image2, 0))  # Local image2 [Nbatch, Npix]
         else:
```

### Comparing `foscat-2.1.0/src/foscat/scat_cov_new.py` & `foscat-2.1.1/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.0/src/foscat.egg-info/PKG-INFO` & `foscat-2.1.1/src/foscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

