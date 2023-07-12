# Comparing `tmp/KDEpy-1.1.3.tar.gz` & `tmp/KDEpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KDEpy-1.1.3.tar", last modified: Tue May 23 15:16:41 2023, max compression
+gzip compressed data, was "KDEpy-1.1.4.tar", last modified: Wed Jul 12 06:26:29 2023, max compression
```

## Comparing `KDEpy-1.1.3.tar` & `KDEpy-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-23 15:16:41.471184 KDEpy-1.1.3/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-23 15:16:41.467193 KDEpy-1.1.3/KDEpy/
--rw-r--r--   0 runner     (501) staff       (20)     8718 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/BaseKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     8259 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/FFTKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     5036 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/NaiveKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     6884 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/TreeKDE.py
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16130 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/binning.py
--rw-r--r--   0 runner     (501) staff       (20)    10045 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/bw_selection.py
--rw-r--r--   0 runner     (501) staff       (20)   894529 2023-05-23 15:13:37.000000 KDEpy-1.1.3/KDEpy/cutils.c
--rw-r--r--   0 runner     (501) staff       (20)    14713 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/cutils.pyx
--rw-r--r--   0 runner     (501) staff       (20)     9817 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/kernel_funcs.py
--rw-r--r--   0 runner     (501) staff       (20)     3809 2023-05-23 15:12:40.000000 KDEpy-1.1.3/KDEpy/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-23 15:16:41.469980 KDEpy-1.1.3/KDEpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     6930 2023-05-23 15:16:41.000000 KDEpy-1.1.3/KDEpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      391 2023-05-23 15:16:41.000000 KDEpy-1.1.3/KDEpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-23 15:16:41.000000 KDEpy-1.1.3/KDEpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      163 2023-05-23 15:16:41.000000 KDEpy-1.1.3/KDEpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-05-23 15:16:41.000000 KDEpy-1.1.3/KDEpy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1499 2023-05-23 15:12:40.000000 KDEpy-1.1.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       48 2023-05-23 15:12:40.000000 KDEpy-1.1.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     6930 2023-05-23 15:16:41.470667 KDEpy-1.1.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4563 2023-05-23 15:12:40.000000 KDEpy-1.1.3/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1034 2023-05-23 15:12:40.000000 KDEpy-1.1.3/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-05-23 15:16:41.471296 KDEpy-1.1.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      575 2023-05-23 15:12:40.000000 KDEpy-1.1.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.206738 KDEpy-1.1.4/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.203098 KDEpy-1.1.4/KDEpy/
+-rw-r--r--   0 runner     (501) staff       (20)     8718 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/BaseKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     8259 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/FFTKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     5036 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/NaiveKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     6884 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/TreeKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16130 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/binning.py
+-rw-r--r--   0 runner     (501) staff       (20)    10045 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/bw_selection.py
+-rw-r--r--   0 runner     (501) staff       (20)   896080 2023-07-12 06:23:43.000000 KDEpy-1.1.4/KDEpy/cutils.c
+-rw-r--r--   0 runner     (501) staff       (20)    14713 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/cutils.pyx
+-rw-r--r--   0 runner     (501) staff       (20)    10297 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/kernel_funcs.py
+-rw-r--r--   0 runner     (501) staff       (20)     3809 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.205568 KDEpy-1.1.4/KDEpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      391 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      163 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1499 2023-07-12 06:22:35.000000 KDEpy-1.1.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       48 2023-07-12 06:22:35.000000 KDEpy-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-12 06:26:29.206322 KDEpy-1.1.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4563 2023-07-12 06:22:35.000000 KDEpy-1.1.4/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1034 2023-07-12 06:22:37.000000 KDEpy-1.1.4/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-12 06:26:29.206846 KDEpy-1.1.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      575 2023-07-12 06:22:37.000000 KDEpy-1.1.4/setup.py
```

### Comparing `KDEpy-1.1.3/KDEpy/BaseKDE.py` & `KDEpy-1.1.4/KDEpy/BaseKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/FFTKDE.py` & `KDEpy-1.1.4/KDEpy/FFTKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/NaiveKDE.py` & `KDEpy-1.1.4/KDEpy/NaiveKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/TreeKDE.py` & `KDEpy-1.1.4/KDEpy/TreeKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/binning.py` & `KDEpy-1.1.4/KDEpy/binning.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/bw_selection.py` & `KDEpy-1.1.4/KDEpy/bw_selection.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/cutils.c` & `KDEpy-1.1.4/KDEpy/cutils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1303,14 +1309,31 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
@@ -4297,15 +4320,15 @@
  * 
  *     # Verify the user input
  *     assert grid.ndim == 2             # <<<<<<<<<<<<<<
  *     n_obs, n_dims = grid.shape[0], grid.shape[1]
  *     assert n_obs > 0
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_grid, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
@@ -4335,15 +4358,15 @@
  *     assert grid.ndim == 2
  *     n_obs, n_dims = grid.shape[0], grid.shape[1]
  *     assert n_obs > 0             # <<<<<<<<<<<<<<
  *     assert n_dims >= 1
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_n_obs > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 356, __pyx_L1_error)
     }
   }
   #endif
 
@@ -4351,15 +4374,15 @@
  *     n_obs, n_dims = grid.shape[0], grid.shape[1]
  *     assert n_obs > 0
  *     assert n_dims >= 1             # <<<<<<<<<<<<<<
  * 
  *     # ----------------------------------------------------------------
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_n_dims >= 1) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 357, __pyx_L1_error)
     }
   }
   #endif
 
@@ -12092,15 +12115,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -17819,15 +17842,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -17982,15 +18005,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -18004,15 +18027,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18104,15 +18127,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -18135,15 +18158,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18368,15 +18391,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -18388,15 +18411,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18517,15 +18540,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -19076,14 +19099,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -23010,15 +23038,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23244,15 +23272,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23478,15 +23506,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `KDEpy-1.1.3/KDEpy/cutils.pyx` & `KDEpy-1.1.4/KDEpy/cutils.pyx`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy/kernel_funcs.py` & `KDEpy-1.1.4/KDEpy/kernel_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,25 @@
     >>> np.allclose(ans, 2)
     True
     >>> ans = gauss_integral(4)
     >>> np.allclose(ans, 3.75994)
     True
     """
     factor = np.sqrt(np.pi * 2)
-    if n % 2 == 0:
+
+    # Special case:
+    # factorial2(-1) used to return 1
+    # but now it returns 0
+    # https://github.com/scipy/scipy/pull/15841
+    # https://github.com/tommyod/KDEpy/issues/145
+    if n == 0:
+        return factor * factorial2(n - 0) / 2
+
+    # Normal cases
+    elif n % 2 == 0:
         return factor * factorial2(n - 1) / 2
     elif n % 2 == 1:
         return factor * norm.pdf(0) * factorial2(n - 1)
     else:
         raise ValueError("n must be odd or even.")
 
 
@@ -260,14 +270,22 @@
         # unit variance.
         self.support = support / np.sqrt(self.var)
 
     def practical_support(self, bw, atol=10e-5):
         """
         Return the support for practical purposes. Used to find a support value
         for computations for kernel functions without finite (bounded) support.
+
+        Examples
+        --------
+        >>> kernel = Kernel(gaussian, var=1, support=np.inf)
+        >>> kernel.practical_support(bw=1)
+        3.8994...
+        >>> kernel.practical_support(bw=2)
+        7.4331...
         """
         # If the kernel has finite support, return the support accounting for
         # the bw
         if self.finite_support:
             return self.support * bw
 
         # If the function does not have finite support, find a practical value
@@ -349,12 +367,12 @@
     "tricube": tricube,
     "cosine": cosine,
     # 'logistic': logistic,
     # 'sigmoid': sigmoid
 }
 
 
-if __name__ == "__main__" and False:
+if __name__ == "__main__":
     import pytest
 
     # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v"])
+    pytest.main(args=[__file__, "--doctest-modules", "-v"])
```

### Comparing `KDEpy-1.1.3/KDEpy/utils.py` & `KDEpy-1.1.4/KDEpy/utils.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/KDEpy.egg-info/PKG-INFO` & `KDEpy-1.1.4/KDEpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KDEpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Kernel Density Estimation in Python.
 Author-email: tommyod <tommy.odland@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Tommy Odland
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `KDEpy-1.1.3/LICENSE` & `KDEpy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/PKG-INFO` & `KDEpy-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KDEpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Kernel Density Estimation in Python.
 Author-email: tommyod <tommy.odland@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Tommy Odland
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `KDEpy-1.1.3/README.md` & `KDEpy-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.3/pyproject.toml` & `KDEpy-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "KDEpy"
-version = "1.1.3"
+version = "1.1.4"
 dependencies = [
     "numpy>=1.14.2",
     "scipy>=1.0.1",
     "matplotlib>=2.2.2",
 ]
 description = "Kernel Density Estimation in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
```

### Comparing `KDEpy-1.1.3/setup.py` & `KDEpy-1.1.4/setup.py`

 * *Files identical despite different names*

