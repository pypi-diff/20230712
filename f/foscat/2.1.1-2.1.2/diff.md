# Comparing `tmp/foscat-2.1.1.tar.gz` & `tmp/foscat-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-asrlb7_o/foscat-2.1.1.tar", last modified: Wed Jul 12 09:31:43 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-9hvmlekh/foscat-2.1.2.tar", last modified: Wed Jul 12 09:52:28 2023, max compression
```

## Comparing `foscat-2.1.1.tar` & `foscat-2.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:31:43.000000 foscat-2.1.1/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.1.1/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-12 09:31:43.000000 foscat-2.1.1/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-12 09:31:05.000000 foscat-2.1.1/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57613 2023-07-11 14:30:51.000000 foscat-2.1.1/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.1.1/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.1.1/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.1.1/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.1.1/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    14492 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.1.1/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.1.1/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    35784 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.1.1/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    58573 2023-07-12 09:16:16.000000 foscat-2.1.1/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.1.1/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-12 09:31:43.000000 foscat-2.1.1/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:52:28.000000 foscat-2.1.2/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:52:28.000000 foscat-2.1.2/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.1.2/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-12 09:52:28.000000 foscat-2.1.2/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-12 09:51:34.000000 foscat-2.1.2/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:52:28.000000 foscat-2.1.2/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57613 2023-07-11 14:30:51.000000 foscat-2.1.2/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.1.2/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.1.2/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.1.2/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.1.2/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    14492 2023-07-12 09:16:16.000000 foscat-2.1.2/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.1.2/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.1.2/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    39335 2023-07-12 09:51:44.000000 foscat-2.1.2/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.1.2/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    58573 2023-07-12 09:16:16.000000 foscat-2.1.2/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.1.2/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-12 09:52:28.000000 foscat-2.1.2/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.1.1/PKG-INFO` & `foscat-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.1.1
+Version: 2.1.2
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.1.1/README.md` & `foscat-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/setup.py` & `foscat-2.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.1.1',
+    version='2.1.2',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.1.1/src/foscat/FoCUS.py` & `foscat-2.1.2/src/foscat/FoCUS.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/GetGPUinfo.py` & `foscat-2.1.2/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/Rformat.py` & `foscat-2.1.2/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/Synthesis.py` & `foscat-2.1.2/src/foscat/Synthesis.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/backend.py` & `foscat-2.1.2/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/build_demo.py` & `foscat-2.1.2/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/scat.py` & `foscat-2.1.2/src/foscat/scat.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
         self.S2=s2
         self.S2L=s2l
         self.cross=cross
         self.backend=backend
         
     def get_j_idx(self):
         shape=list(self.S1.shape)
-        nscale=shape[2]
+        if len(shape)==3:
+            nscale=shape[1]
+        else:
+            nscale=shape[2]
+
         n=nscale*(nscale+1)//2
         j1=np.zeros([n],dtype='int')
         j2=np.zeros([n],dtype='int')
         n=0
         for i in range(nscale):
             for j in range(i+1):
                 j1[n]=j
@@ -244,38 +248,56 @@
 
         if hold:
             plt.figure(figsize=(16,8))
         
         test=None
         plt.subplot(2, 2, 1)
         tmp=abs(self.get_np(self.S1))
-        for k in range(tmp.shape[3]):
-            for i1 in range(tmp.shape[0]):
-                for i2 in range(tmp.shape[0]):
+        if len(tmp.shape)==4:
+            for k in range(tmp.shape[3]):
+                for i1 in range(tmp.shape[0]):
+                    for i2 in range(tmp.shape[0]):
+                        if test is None:
+                            test=1
+                            plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_{1}$' % (name), lw=lw)
+                        else:
+                            plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+        else:
+            for k in range(tmp.shape[2]):
+                for i1 in range(tmp.shape[0]):
                     if test is None:
                         test=1
-                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_{1}$' % (name), lw=lw)
+                        plt.plot(tmp[i1,:,k],color=color, label=r'%s $S_{1}$' % (name), lw=lw)
                     else:
-                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+                        plt.plot(tmp[i1,:,k],color=color, lw=lw)
         plt.yscale('log')
         plt.ylabel('S1')
         plt.xlabel(r'$j_{1}$')
         plt.legend()
 
         test=None
         plt.subplot(2, 2, 2)
         tmp=abs(self.get_np(self.P00))
-        for k in range(tmp.shape[3]):
-            for i1 in range(tmp.shape[0]):
-                for i2 in range(tmp.shape[0]):
+        if len(tmp.shape)==4:
+            for k in range(tmp.shape[3]):
+                for i1 in range(tmp.shape[0]):
+                    for i2 in range(tmp.shape[0]):
+                        if test is None:
+                            test=1
+                            plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                        else:
+                            plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+        else:
+            for k in range(tmp.shape[2]):
+                for i1 in range(tmp.shape[0]):
                     if test is None:
                         test=1
-                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                        plt.plot(tmp[i1,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
                     else:
-                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+                        plt.plot(tmp[i1,:,k],color=color, lw=lw)
         plt.yscale('log')
         plt.ylabel('P00')
         plt.xlabel(r'$j_{1}$')
         plt.legend()
         
         ax1=plt.subplot(2, 2, 3)
         ax2 = ax1.twiny()
@@ -284,28 +306,51 @@
         lname=r'%s $S_{2}$' % (name)
         ax1.set_ylabel(r'$S_{2}$ [L1 norm]')
         test=None
         tabx=[]
         tabnx=[]
         tab2x=[]
         tab2nx=[]
-        for i0 in range(tmp.shape[0]):
-            for i1 in range(tmp.shape[1]):
+        if len(tmp.shape)==5:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        for i3 in range(tmp.shape[3]):
+                            for i4 in range(tmp.shape[4]):
+                                if j2[j1==i2].shape[0]==1:
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                                 color=color, lw=lw)
+                                else:
+                                    if legend and test is None:
+                                        ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                                 color=color, label=lname, lw=lw)
+                                        test=1
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                             color=color, lw=lw)
+                        tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                        tabx=tabx+[k+n for k in j2[j1==i2]]
+                        tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                        n=n+j2[j1==i2].shape[0]-1
+        else:
+            print(tmp.shape)
+            for i0 in range(tmp.shape[0]):
                 for i2 in range(j1.max()+1):
-                    for i3 in range(tmp.shape[3]):
-                        for i4 in range(tmp.shape[4]):
+                    for i3 in range(tmp.shape[2]):
+                        for i4 in range(tmp.shape[3]):
                             if j2[j1==i2].shape[0]==1:
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
-                                             color=color, lw=lw)
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4],'.', \
+                                         color=color, lw=lw)
                             else:
                                 if legend and test is None:
-                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4], \
                                              color=color, label=lname, lw=lw)
                                     test=1
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4], \
                                          color=color, lw=lw)
                     tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
                     tabx=tabx+[k+n for k in j2[j1==i2]]
                     tab2x=tab2x+[(j2[j1==i2]+n).mean()]
                     tab2nx=tab2nx+['%d'%(i2)]
                     ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
                     n=n+j2[j1==i2].shape[0]-1
@@ -343,28 +388,50 @@
         lname=r'%s $S2_{2}$' % (name)
         ax1.set_ylabel(r'$S_{2}$ [L2 norm]')
         test=None
         tabx=[]
         tabnx=[]
         tab2x=[]
         tab2nx=[]
-        for i0 in range(tmp.shape[0]):
-            for i1 in range(tmp.shape[1]):
+        if len(tmp.shape)==5:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        for i3 in range(tmp.shape[3]):
+                            for i4 in range(tmp.shape[4]):
+                                if j2[j1==i2].shape[0]==1:
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                                 color=color, lw=lw)
+                                else:
+                                    if legend and test is None:
+                                        ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                                 color=color, label=lname, lw=lw)
+                                        test=1
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                             color=color, lw=lw)
+                        tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                        tabx=tabx+[k+n for k in j2[j1==i2]]
+                        tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                        n=n+j2[j1==i2].shape[0]-1
+        else:
+            for i0 in range(tmp.shape[0]):
                 for i2 in range(j1.max()+1):
-                    for i3 in range(tmp.shape[3]):
-                        for i4 in range(tmp.shape[4]):
+                    for i3 in range(tmp.shape[2]):
+                        for i4 in range(tmp.shape[3]):
                             if j2[j1==i2].shape[0]==1:
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4],'.', \
                                              color=color, lw=lw)
                             else:
                                 if legend and test is None:
-                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4], \
                                              color=color, label=lname, lw=lw)
                                     test=1
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,j1==i2,i3,i4], \
                                          color=color, lw=lw)
                     tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
                     tabx=tabx+[k+n for k in j2[j1==i2]]
                     tab2x=tab2x+[(j2[j1==i2]+n).mean()]
                     tab2nx=tab2nx+['%d'%(i2)]
                     ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
                     n=n+j2[j1==i2].shape[0]-1
```

### Comparing `foscat-2.1.1/src/foscat/scat_cov.old.py` & `foscat-2.1.2/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/scat_cov.py` & `foscat-2.1.2/src/foscat/scat_cov.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat/scat_cov_new.py` & `foscat-2.1.2/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.1.1/src/foscat.egg-info/PKG-INFO` & `foscat-2.1.2/src/foscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.1.1
+Version: 2.1.2
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

