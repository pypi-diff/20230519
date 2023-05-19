# Comparing `tmp/sorted_nearest-0.0.8.tar.gz` & `tmp/sorted_nearest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sorted_nearest-0.0.8.tar", last modified: Fri Jun 29 14:54:21 2018, max compression
+gzip compressed data, was "dist/sorted_nearest-0.0.9.tar", last modified: Sun Jul  1 09:52:06 2018, max compression
```

## Comparing `sorted_nearest-0.0.8.tar` & `sorted_nearest-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-06-29 14:54:21.000000 sorted_nearest-0.0.8/
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-06-29 14:54:19.000000 sorted_nearest-0.0.8/sorted_nearest.egg-info/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      360 2018-06-29 14:54:18.000000 sorted_nearest-0.0.8/sorted_nearest.egg-info/SOURCES.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2018-06-29 14:54:18.000000 sorted_nearest-0.0.8/sorted_nearest.egg-info/dependency_links.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       15 2018-06-29 14:54:18.000000 sorted_nearest-0.0.8/sorted_nearest.egg-info/top_level.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      649 2018-06-29 14:54:18.000000 sorted_nearest-0.0.8/sorted_nearest.egg-info/PKG-INFO
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-06-29 14:54:18.000000 sorted_nearest-0.0.8/sorted_nearest/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      289 2018-06-29 12:53:09.000000 sorted_nearest-0.0.8/sorted_nearest/__init__.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-06-29 14:54:20.000000 sorted_nearest-0.0.8/sorted_nearest/src/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   843478 2018-06-29 14:50:10.000000 sorted_nearest-0.0.8/sorted_nearest/src/sorted_nearest.c
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     6279 2018-06-29 14:50:04.000000 sorted_nearest-0.0.8/sorted_nearest/src/sorted_nearest.pyx
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-21 07:58:56.000000 sorted_nearest-0.0.8/sorted_nearest/src/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      441 2018-06-22 08:13:03.000000 sorted_nearest-0.0.8/sorted_nearest/src/csorted_nearest.pxd
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    12981 2018-05-21 07:52:05.000000 sorted_nearest-0.0.8/sorted_nearest/src/utarray.h
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      649 2018-06-29 14:54:21.000000 sorted_nearest-0.0.8/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1467 2018-06-29 14:53:52.000000 sorted_nearest-0.0.8/setup.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       38 2018-06-29 14:54:21.000000 sorted_nearest-0.0.8/setup.cfg
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-07-01 09:52:05.000000 sorted_nearest-0.0.9/
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-07-01 09:51:59.000000 sorted_nearest-0.0.9/sorted_nearest.egg-info/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      360 2018-07-01 09:51:54.000000 sorted_nearest-0.0.9/sorted_nearest.egg-info/SOURCES.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2018-07-01 09:51:54.000000 sorted_nearest-0.0.9/sorted_nearest.egg-info/dependency_links.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       15 2018-07-01 09:51:54.000000 sorted_nearest-0.0.9/sorted_nearest.egg-info/top_level.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      649 2018-07-01 09:51:54.000000 sorted_nearest-0.0.9/sorted_nearest.egg-info/PKG-INFO
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-07-01 09:51:56.000000 sorted_nearest-0.0.9/sorted_nearest/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      289 2018-06-29 12:53:09.000000 sorted_nearest-0.0.9/sorted_nearest/__init__.py
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-07-01 09:52:04.000000 sorted_nearest-0.0.9/sorted_nearest/src/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   827658 2018-07-01 09:14:59.000000 sorted_nearest-0.0.9/sorted_nearest/src/sorted_nearest.c
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4075 2018-07-01 08:41:33.000000 sorted_nearest-0.0.9/sorted_nearest/src/sorted_nearest.pyx
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-21 07:58:56.000000 sorted_nearest-0.0.9/sorted_nearest/src/__init__.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      441 2018-06-22 08:13:03.000000 sorted_nearest-0.0.9/sorted_nearest/src/csorted_nearest.pxd
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    12981 2018-05-21 07:52:05.000000 sorted_nearest-0.0.9/sorted_nearest/src/utarray.h
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      649 2018-07-01 09:52:05.000000 sorted_nearest-0.0.9/PKG-INFO
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1467 2018-07-01 09:51:40.000000 sorted_nearest-0.0.9/setup.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       38 2018-07-01 09:52:05.000000 sorted_nearest-0.0.9/setup.cfg
```

### Comparing `sorted_nearest-0.0.8/sorted_nearest.egg-info/PKG-INFO` & `sorted_nearest-0.0.9/sorted_nearest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sorted-nearest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Find nearest interval.
 Home-page: https://github.com/endrebak/sorted_nearest
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: New BSD License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `sorted_nearest-0.0.8/sorted_nearest/src/sorted_nearest.c` & `sorted_nearest-0.0.9/sorted_nearest/src/sorted_nearest.c`

 * *Files 1% similar despite different names*

```diff
@@ -1144,14 +1144,17 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* None.proto */
+static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1431,17 +1434,14 @@
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
-
-/* None.proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
@@ -1614,17 +1614,17 @@
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_find_clusters(__Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
@@ -1694,15 +1694,14 @@
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
-static const char __pyx_k_l_idx[] = "l_idx";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_r_idx[] = "r_idx";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_encode[] = "encode";
@@ -1721,18 +1720,16 @@
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_next_dist[] = "next_dist";
-static const char __pyx_k_next_lidx[] = "next_lidx";
 static const char __pyx_k_next_ridx[] = "next_ridx";
 static const char __pyx_k_prev_dist[] = "prev_dist";
-static const char __pyx_k_prev_lidx[] = "prev_lidx";
 static const char __pyx_k_prev_ridx[] = "prev_ridx";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
@@ -1818,36 +1815,33 @@
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_l_e;
-static PyObject *__pyx_n_s_l_idx;
 static PyObject *__pyx_n_s_l_s;
 static PyObject *__pyx_n_s_long;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_next_dist;
-static PyObject *__pyx_n_s_next_lidx;
 static PyObject *__pyx_n_s_next_ridx;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_ones;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_prev_dist;
-static PyObject *__pyx_n_s_prev_lidx;
 static PyObject *__pyx_n_s_prev_ridx;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
@@ -1875,17 +1869,17 @@
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx); /* proto */
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx); /* proto */
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_prev_lidx, __Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_lidx, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist); /* proto */
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx); /* proto */
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx); /* proto */
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist); /* proto */
 static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_6find_clusters(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ends); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
@@ -1960,31 +1954,29 @@
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
 /* "sorted_nearest/src/sorted_nearest.pyx":10
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] l_idx, long [::1] r_s, long [::1] r_idx):             # <<<<<<<<<<<<<<
+ * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] r_s, long [::1] r_idx):             # <<<<<<<<<<<<<<
  * 
  *     cdef int j = 0
  */
 
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_1nearest_next_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_j;
   int __pyx_v_i;
   int __pyx_v_len_l;
   int __pyx_v_len_r;
-  PyObject *__pyx_v_arr_lidx = NULL;
   PyObject *__pyx_v_arr_ridx = NULL;
   PyObject *__pyx_v_arr_dist = NULL;
-  __Pyx_memviewslice __pyx_v_lidx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_ridx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dist = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -1997,22 +1989,18 @@
   Py_ssize_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_ssize_t __pyx_t_18;
-  Py_ssize_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
   __Pyx_RefNannySetupContext("nearest_next_nonoverlapping", 0);
 
   /* "sorted_nearest/src/sorted_nearest.pyx":12
- * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] l_idx, long [::1] r_s, long [::1] r_idx):
+ * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] r_s, long [::1] r_idx):
  * 
  *     cdef int j = 0             # <<<<<<<<<<<<<<
  *     cdef int i = 0
  * 
  */
   __pyx_v_j = 0;
 
@@ -2036,25 +2024,25 @@
   __pyx_v_len_l = __pyx_t_1;
 
   /* "sorted_nearest/src/sorted_nearest.pyx":16
  * 
  *     cdef int len_l = len(l_e)
  *     cdef int len_r = len(r_s)             # <<<<<<<<<<<<<<
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_r_s); 
   __pyx_v_len_r = __pyx_t_1;
 
   /* "sorted_nearest/src/sorted_nearest.pyx":18
  *     cdef int len_r = len(r_s)
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  *     arr_dist = np.ones(len_l, dtype=np.long) * -1
+ *     cdef long [::1] ridx
  */
   __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
@@ -2077,23 +2065,23 @@
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyNumber_Multiply(__pyx_t_6, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_arr_lidx = __pyx_t_2;
+  __pyx_v_arr_ridx = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "sorted_nearest/src/sorted_nearest.pyx":19
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     arr_dist = np.ones(len_l, dtype=np.long) * -1
- *     cdef long [::1] lidx
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_dist = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
+ *     cdef long [::1] ridx
+ *     cdef long [::1] dist
  */
   __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
@@ -2116,93 +2104,42 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyNumber_Multiply(__pyx_t_5, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_arr_ridx = __pyx_t_2;
-  __pyx_t_2 = 0;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":20
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
- *     arr_dist = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     cdef long [::1] lidx
- *     cdef long [::1] ridx
- */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_long); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_arr_dist = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":25
+  /* "sorted_nearest/src/sorted_nearest.pyx":23
  *     cdef long [::1] dist
  * 
- *     lidx = arr_lidx             # <<<<<<<<<<<<<<
- *     ridx = arr_ridx
- *     dist = arr_dist
- */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_lidx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_v_lidx = __pyx_t_7;
-  __pyx_t_7.memview = NULL;
-  __pyx_t_7.data = NULL;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":26
- * 
- *     lidx = arr_lidx
  *     ridx = arr_ridx             # <<<<<<<<<<<<<<
  *     dist = arr_dist
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_v_ridx = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":27
- *     lidx = arr_lidx
+  /* "sorted_nearest/src/sorted_nearest.pyx":24
+ * 
  *     ridx = arr_ridx
  *     dist = arr_dist             # <<<<<<<<<<<<<<
  * 
  *     # print("l_e", list(l_e))
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_v_dist = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":31
+  /* "sorted_nearest/src/sorted_nearest.pyx":28
  *     # print("l_e", list(l_e))
  *     # print("r_s", list(r_s))
  *     while i < len_l and j < len_r:             # <<<<<<<<<<<<<<
  *         # print("l_e[i]", l_e[i])
  *         # print("r_s[j]", r_s[j])
  */
   while (1) {
@@ -2213,130 +2150,105 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_9 = ((__pyx_v_j < __pyx_v_len_r) != 0);
     __pyx_t_8 = __pyx_t_9;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_8) break;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":34
+    /* "sorted_nearest/src/sorted_nearest.pyx":31
  *         # print("l_e[i]", l_e[i])
  *         # print("r_s[j]", r_s[j])
  *         if l_e[i] >= r_s[j]:             # <<<<<<<<<<<<<<
  *             # print("in if")
  *             j += 1
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_j;
     __pyx_t_8 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_e.data) + __pyx_t_10)) ))) >= (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_s.data) + __pyx_t_11)) )))) != 0);
     if (__pyx_t_8) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":36
+      /* "sorted_nearest/src/sorted_nearest.pyx":33
  *         if l_e[i] >= r_s[j]:
  *             # print("in if")
  *             j += 1             # <<<<<<<<<<<<<<
- *             lidx[i] = l_idx[i]
- *         else:
- */
-      __pyx_v_j = (__pyx_v_j + 1);
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":37
- *             # print("in if")
- *             j += 1
- *             lidx[i] = l_idx[i]             # <<<<<<<<<<<<<<
  *         else:
  *             # print("in else")
  */
-      __pyx_t_12 = __pyx_v_i;
-      __pyx_t_13 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_lidx.data) + __pyx_t_13)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_idx.data) + __pyx_t_12)) )));
+      __pyx_v_j = (__pyx_v_j + 1);
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":34
+      /* "sorted_nearest/src/sorted_nearest.pyx":31
  *         # print("l_e[i]", l_e[i])
  *         # print("r_s[j]", r_s[j])
  *         if l_e[i] >= r_s[j]:             # <<<<<<<<<<<<<<
  *             # print("in if")
  *             j += 1
  */
       goto __pyx_L7;
     }
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":40
+    /* "sorted_nearest/src/sorted_nearest.pyx":36
  *         else:
  *             # print("in else")
  *             dist[i] = r_s[j] - l_e[i]             # <<<<<<<<<<<<<<
  *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]
+ *             i += 1
  */
     /*else*/ {
-      __pyx_t_14 = __pyx_v_j;
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_16 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_dist.data) + __pyx_t_16)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_s.data) + __pyx_t_14)) ))) - (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_e.data) + __pyx_t_15)) ))));
+      __pyx_t_12 = __pyx_v_j;
+      __pyx_t_13 = __pyx_v_i;
+      __pyx_t_14 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_dist.data) + __pyx_t_14)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_s.data) + __pyx_t_12)) ))) - (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_e.data) + __pyx_t_13)) ))));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":41
+      /* "sorted_nearest/src/sorted_nearest.pyx":37
  *             # print("in else")
  *             dist[i] = r_s[j] - l_e[i]
  *             ridx[i] = r_idx[j]             # <<<<<<<<<<<<<<
- *             lidx[i] = l_idx[i]
- *             i += 1
- */
-      __pyx_t_17 = __pyx_v_j;
-      __pyx_t_18 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ridx.data) + __pyx_t_18)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_idx.data) + __pyx_t_17)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":42
- *             dist[i] = r_s[j] - l_e[i]
- *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]             # <<<<<<<<<<<<<<
  *             i += 1
  *         # print("dist", list(dist))
  */
-      __pyx_t_19 = __pyx_v_i;
-      __pyx_t_20 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_lidx.data) + __pyx_t_20)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_idx.data) + __pyx_t_19)) )));
+      __pyx_t_15 = __pyx_v_j;
+      __pyx_t_16 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ridx.data) + __pyx_t_16)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_idx.data) + __pyx_t_15)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":43
+      /* "sorted_nearest/src/sorted_nearest.pyx":38
+ *             dist[i] = r_s[j] - l_e[i]
  *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]
  *             i += 1             # <<<<<<<<<<<<<<
  *         # print("dist", list(dist))
  *         # print("ridx", list(ridx))
  */
       __pyx_v_i = (__pyx_v_i + 1);
     }
     __pyx_L7:;
   }
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":47
+  /* "sorted_nearest/src/sorted_nearest.pyx":42
  *         # print("ridx", list(ridx))
  * 
- *     return arr_lidx, arr_ridx, arr_dist             # <<<<<<<<<<<<<<
+ *     return arr_ridx, arr_dist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_arr_lidx);
-  __Pyx_GIVEREF(__pyx_v_arr_lidx);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_arr_lidx);
   __Pyx_INCREF(__pyx_v_arr_ridx);
   __Pyx_GIVEREF(__pyx_v_arr_ridx);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_arr_ridx);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_arr_ridx);
   __Pyx_INCREF(__pyx_v_arr_dist);
   __Pyx_GIVEREF(__pyx_v_arr_dist);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_arr_dist);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_arr_dist);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "sorted_nearest/src/sorted_nearest.pyx":10
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] l_idx, long [::1] r_s, long [::1] r_idx):             # <<<<<<<<<<<<<<
+ * cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] r_s, long [::1] r_idx):             # <<<<<<<<<<<<<<
  * 
  *     cdef int j = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -2344,44 +2256,39 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_next_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_arr_lidx);
   __Pyx_XDECREF(__pyx_v_arr_ridx);
   __Pyx_XDECREF(__pyx_v_arr_dist);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_lidx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_ridx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_dist, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_1nearest_next_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_1nearest_next_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_l_e = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __Pyx_memviewslice __pyx_v_l_idx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_r_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_r_idx = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("nearest_next_nonoverlapping (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_l_e,&__pyx_n_s_l_idx,&__pyx_n_s_r_s,&__pyx_n_s_r_idx,0};
-    PyObject* values[4] = {0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_l_e,&__pyx_n_s_r_s,&__pyx_n_s_r_idx,0};
+    PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -2390,107 +2297,99 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_l_e)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_l_idx)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 4, 4, 1); __PYX_ERR(0, 10, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 3, 3, 1); __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_s)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_idx)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 4, 4, 2); __PYX_ERR(0, 10, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_idx)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 4, 4, 3); __PYX_ERR(0, 10, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 3, 3, 2); __PYX_ERR(0, 10, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest_next_nonoverlapping") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_l_e = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_e.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
-    __pyx_v_l_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_idx.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
-    __pyx_v_r_s = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_s.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
-    __pyx_v_r_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_idx.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
+    __pyx_v_r_s = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_s.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
+    __pyx_v_r_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_idx.memview)) __PYX_ERR(0, 10, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 10, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("nearest_next_nonoverlapping", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 10, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_next_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__pyx_self, __pyx_v_l_e, __pyx_v_l_idx, __pyx_v_r_s, __pyx_v_r_idx);
+  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__pyx_self, __pyx_v_l_e, __pyx_v_r_s, __pyx_v_r_idx);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx) {
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_e, __Pyx_memviewslice __pyx_v_r_s, __Pyx_memviewslice __pyx_v_r_idx) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("nearest_next_nonoverlapping", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__pyx_v_l_e, __pyx_v_l_idx, __pyx_v_r_s, __pyx_v_r_idx, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (unlikely(!__pyx_v_l_e.memview)) { __Pyx_RaiseUnboundLocalError("l_e"); __PYX_ERR(0, 10, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_r_s.memview)) { __Pyx_RaiseUnboundLocalError("r_s"); __PYX_ERR(0, 10, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_r_idx.memview)) { __Pyx_RaiseUnboundLocalError("r_idx"); __PYX_ERR(0, 10, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_next_nonoverlapping(__pyx_v_l_e, __pyx_v_r_s, __pyx_v_r_idx, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_next_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_l_e, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_l_idx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_r_s, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_r_idx, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sorted_nearest/src/sorted_nearest.pyx":54
+/* "sorted_nearest/src/sorted_nearest.pyx":48
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] l_idx, long [::1] r_e, long [::1] r_idx):             # <<<<<<<<<<<<<<
+ * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] r_e, long [::1] r_idx):             # <<<<<<<<<<<<<<
  * 
  *     cdef int len_l = len(l_s)
  */
 
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_3nearest_previous_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_len_l;
   int __pyx_v_len_r;
   int __pyx_v_j;
   int __pyx_v_i;
-  PyObject *__pyx_v_arr_lidx = NULL;
   PyObject *__pyx_v_arr_ridx = NULL;
   PyObject *__pyx_v_arr_dist = NULL;
-  __Pyx_memviewslice __pyx_v_lidx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_ridx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dist = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2503,346 +2402,266 @@
   Py_ssize_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_ssize_t __pyx_t_18;
-  Py_ssize_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
   __Pyx_RefNannySetupContext("nearest_previous_nonoverlapping", 0);
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":56
- * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] l_idx, long [::1] r_e, long [::1] r_idx):
+  /* "sorted_nearest/src/sorted_nearest.pyx":50
+ * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] r_e, long [::1] r_idx):
  * 
  *     cdef int len_l = len(l_s)             # <<<<<<<<<<<<<<
  *     cdef int len_r = len(r_e)
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_l_s); 
   __pyx_v_len_l = __pyx_t_1;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":57
+  /* "sorted_nearest/src/sorted_nearest.pyx":51
  * 
  *     cdef int len_l = len(l_s)
  *     cdef int len_r = len(r_e)             # <<<<<<<<<<<<<<
  * 
  *     cdef int j = len_r - 1
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_r_e); 
   __pyx_v_len_r = __pyx_t_1;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":59
+  /* "sorted_nearest/src/sorted_nearest.pyx":53
  *     cdef int len_r = len(r_e)
  * 
  *     cdef int j = len_r - 1             # <<<<<<<<<<<<<<
  *     cdef int i = len_l - 1
  * 
  */
   __pyx_v_j = (__pyx_v_len_r - 1);
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":60
+  /* "sorted_nearest/src/sorted_nearest.pyx":54
  * 
  *     cdef int j = len_r - 1
  *     cdef int i = len_l - 1             # <<<<<<<<<<<<<<
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
  */
   __pyx_v_i = (__pyx_v_len_l - 1);
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":62
+  /* "sorted_nearest/src/sorted_nearest.pyx":56
  *     cdef int i = len_l - 1
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  *     arr_dist = np.ones(len_l, dtype=np.long) * -1
+ *     cdef long [::1] ridx
  */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_6, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_6, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_arr_lidx = __pyx_t_2;
+  __pyx_v_arr_ridx = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":63
+  /* "sorted_nearest/src/sorted_nearest.pyx":57
  * 
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     arr_dist = np.ones(len_l, dtype=np.long) * -1
- *     cdef long [::1] lidx
+ *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
+ *     arr_dist = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
+ *     cdef long [::1] ridx
+ *     cdef long [::1] dist
  */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_long); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_long); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_5, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_arr_ridx = __pyx_t_2;
-  __pyx_t_2 = 0;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":64
- *     arr_lidx = np.ones(len_l, dtype=np.long) * -1
- *     arr_ridx = np.ones(len_l, dtype=np.long) * -1
- *     arr_dist = np.ones(len_l, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     cdef long [::1] lidx
- *     cdef long [::1] ridx
- */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_len_l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_5, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_long); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_arr_dist = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":69
+  /* "sorted_nearest/src/sorted_nearest.pyx":61
  *     cdef long [::1] dist
  * 
- *     lidx = arr_lidx             # <<<<<<<<<<<<<<
- *     ridx = arr_ridx
- *     dist = arr_dist
- */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_lidx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __pyx_v_lidx = __pyx_t_7;
-  __pyx_t_7.memview = NULL;
-  __pyx_t_7.data = NULL;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":70
- * 
- *     lidx = arr_lidx
  *     ridx = arr_ridx             # <<<<<<<<<<<<<<
  *     dist = arr_dist
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 61, __pyx_L1_error)
   __pyx_v_ridx = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":71
- *     lidx = arr_lidx
+  /* "sorted_nearest/src/sorted_nearest.pyx":62
+ * 
  *     ridx = arr_ridx
  *     dist = arr_dist             # <<<<<<<<<<<<<<
  * 
- * 
+ *     while -1 < i and -1 < j:
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 62, __pyx_L1_error)
   __pyx_v_dist = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":74
- * 
+  /* "sorted_nearest/src/sorted_nearest.pyx":64
+ *     dist = arr_dist
  * 
  *     while -1 < i and -1 < j:             # <<<<<<<<<<<<<<
  *         if l_s[i] <= r_e[j]:
- *             j -= 1
+ *             # print("in if")
  */
   while (1) {
     __pyx_t_9 = ((-1L < __pyx_v_i) != 0);
     if (__pyx_t_9) {
     } else {
       __pyx_t_8 = __pyx_t_9;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_9 = ((-1L < __pyx_v_j) != 0);
     __pyx_t_8 = __pyx_t_9;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_8) break;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":75
+    /* "sorted_nearest/src/sorted_nearest.pyx":65
  * 
  *     while -1 < i and -1 < j:
  *         if l_s[i] <= r_e[j]:             # <<<<<<<<<<<<<<
+ *             # print("in if")
  *             j -= 1
- *             lidx[i] = l_idx[i]
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_j;
     __pyx_t_8 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_s.data) + __pyx_t_10)) ))) <= (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_e.data) + __pyx_t_11)) )))) != 0);
     if (__pyx_t_8) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":76
- *     while -1 < i and -1 < j:
+      /* "sorted_nearest/src/sorted_nearest.pyx":67
  *         if l_s[i] <= r_e[j]:
+ *             # print("in if")
  *             j -= 1             # <<<<<<<<<<<<<<
- *             lidx[i] = l_idx[i]
  *         else:
+ *             # print("in else")
  */
       __pyx_v_j = (__pyx_v_j - 1);
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":77
- *         if l_s[i] <= r_e[j]:
- *             j -= 1
- *             lidx[i] = l_idx[i]             # <<<<<<<<<<<<<<
- *         else:
- *             dist[i] = l_s[i] - r_e[j]
- */
-      __pyx_t_12 = __pyx_v_i;
-      __pyx_t_13 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_lidx.data) + __pyx_t_13)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_idx.data) + __pyx_t_12)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":75
+      /* "sorted_nearest/src/sorted_nearest.pyx":65
  * 
  *     while -1 < i and -1 < j:
  *         if l_s[i] <= r_e[j]:             # <<<<<<<<<<<<<<
+ *             # print("in if")
  *             j -= 1
- *             lidx[i] = l_idx[i]
  */
       goto __pyx_L7;
     }
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":79
- *             lidx[i] = l_idx[i]
- *         else:
+    /* "sorted_nearest/src/sorted_nearest.pyx":72
+ *             # print("l_s[i]", l_s[i])
+ *             # print("r_e[j]", r_e[j])
  *             dist[i] = l_s[i] - r_e[j]             # <<<<<<<<<<<<<<
  *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]
+ *             i -= 1
  */
     /*else*/ {
+      __pyx_t_12 = __pyx_v_i;
+      __pyx_t_13 = __pyx_v_j;
       __pyx_t_14 = __pyx_v_i;
-      __pyx_t_15 = __pyx_v_j;
-      __pyx_t_16 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_dist.data) + __pyx_t_16)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_s.data) + __pyx_t_14)) ))) - (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_e.data) + __pyx_t_15)) ))));
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_dist.data) + __pyx_t_14)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_s.data) + __pyx_t_12)) ))) - (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_e.data) + __pyx_t_13)) ))));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":80
- *         else:
+      /* "sorted_nearest/src/sorted_nearest.pyx":73
+ *             # print("r_e[j]", r_e[j])
  *             dist[i] = l_s[i] - r_e[j]
  *             ridx[i] = r_idx[j]             # <<<<<<<<<<<<<<
- *             lidx[i] = l_idx[i]
  *             i -= 1
+ *         # print("dist", list(dist))
  */
-      __pyx_t_17 = __pyx_v_j;
-      __pyx_t_18 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ridx.data) + __pyx_t_18)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_idx.data) + __pyx_t_17)) )));
+      __pyx_t_15 = __pyx_v_j;
+      __pyx_t_16 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ridx.data) + __pyx_t_16)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_r_idx.data) + __pyx_t_15)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":81
+      /* "sorted_nearest/src/sorted_nearest.pyx":74
  *             dist[i] = l_s[i] - r_e[j]
  *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]             # <<<<<<<<<<<<<<
- *             i -= 1
- * 
- */
-      __pyx_t_19 = __pyx_v_i;
-      __pyx_t_20 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_lidx.data) + __pyx_t_20)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_l_idx.data) + __pyx_t_19)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":82
- *             ridx[i] = r_idx[j]
- *             lidx[i] = l_idx[i]
  *             i -= 1             # <<<<<<<<<<<<<<
- * 
- *     return arr_lidx, arr_ridx, arr_dist
+ *         # print("dist", list(dist))
+ *         # print("ridx", list(ridx))
  */
       __pyx_v_i = (__pyx_v_i - 1);
     }
     __pyx_L7:;
   }
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":84
- *             i -= 1
+  /* "sorted_nearest/src/sorted_nearest.pyx":81
+ *     # print("final ridx", list(ridx))
  * 
- *     return arr_lidx, arr_ridx, arr_dist             # <<<<<<<<<<<<<<
+ *     return arr_ridx, arr_dist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_arr_lidx);
-  __Pyx_GIVEREF(__pyx_v_arr_lidx);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_arr_lidx);
   __Pyx_INCREF(__pyx_v_arr_ridx);
   __Pyx_GIVEREF(__pyx_v_arr_ridx);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_arr_ridx);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_arr_ridx);
   __Pyx_INCREF(__pyx_v_arr_dist);
   __Pyx_GIVEREF(__pyx_v_arr_dist);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_arr_dist);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_arr_dist);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":54
+  /* "sorted_nearest/src/sorted_nearest.pyx":48
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] l_idx, long [::1] r_e, long [::1] r_idx):             # <<<<<<<<<<<<<<
+ * cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] r_e, long [::1] r_idx):             # <<<<<<<<<<<<<<
  * 
  *     cdef int len_l = len(l_s)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -2850,44 +2669,39 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_previous_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_arr_lidx);
   __Pyx_XDECREF(__pyx_v_arr_ridx);
   __Pyx_XDECREF(__pyx_v_arr_dist);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_lidx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_ridx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_dist, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_3nearest_previous_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_3nearest_previous_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_l_s = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __Pyx_memviewslice __pyx_v_l_idx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_r_e = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_r_idx = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("nearest_previous_nonoverlapping (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_l_s,&__pyx_n_s_l_idx,&__pyx_n_s_r_e,&__pyx_n_s_r_idx,0};
-    PyObject* values[4] = {0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_l_s,&__pyx_n_s_r_e,&__pyx_n_s_r_idx,0};
+    PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -2896,105 +2710,97 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_l_s)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_l_idx)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_e)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 4, 4, 1); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 3, 3, 1); __PYX_ERR(0, 48, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_e)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 4, 4, 2); __PYX_ERR(0, 54, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_idx)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_r_idx)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 4, 4, 3); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 3, 3, 2); __PYX_ERR(0, 48, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest_previous_nonoverlapping") < 0)) __PYX_ERR(0, 54, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest_previous_nonoverlapping") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_l_s = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_s.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
-    __pyx_v_l_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_idx.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
-    __pyx_v_r_e = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_e.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
-    __pyx_v_r_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_idx.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
+    __pyx_v_l_s = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_s.memview)) __PYX_ERR(0, 48, __pyx_L3_error)
+    __pyx_v_r_e = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_e.memview)) __PYX_ERR(0, 48, __pyx_L3_error)
+    __pyx_v_r_idx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_r_idx.memview)) __PYX_ERR(0, 48, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 54, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("nearest_previous_nonoverlapping", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 48, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_previous_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(__pyx_self, __pyx_v_l_s, __pyx_v_l_idx, __pyx_v_r_e, __pyx_v_r_idx);
+  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(__pyx_self, __pyx_v_l_s, __pyx_v_r_e, __pyx_v_r_idx);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_l_idx, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx) {
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_2nearest_previous_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_l_s, __Pyx_memviewslice __pyx_v_r_e, __Pyx_memviewslice __pyx_v_r_idx) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("nearest_previous_nonoverlapping", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__pyx_v_l_s, __pyx_v_l_idx, __pyx_v_r_e, __pyx_v_r_idx, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (unlikely(!__pyx_v_l_s.memview)) { __Pyx_RaiseUnboundLocalError("l_s"); __PYX_ERR(0, 48, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_r_e.memview)) { __Pyx_RaiseUnboundLocalError("r_e"); __PYX_ERR(0, 48, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_r_idx.memview)) { __Pyx_RaiseUnboundLocalError("r_idx"); __PYX_ERR(0, 48, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_previous_nonoverlapping(__pyx_v_l_s, __pyx_v_r_e, __pyx_v_r_idx, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_previous_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_l_s, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_l_idx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_r_e, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_r_idx, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sorted_nearest/src/sorted_nearest.pyx":90
+/* "sorted_nearest/src/sorted_nearest.pyx":86
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_nonoverlapping(long [::1] prev_lidx, long [::1] prev_ridx, long [::1] prev_dist,             # <<<<<<<<<<<<<<
- *                              long [::1] next_lidx, long [::1] next_ridx, long [::1] next_dist):
+ * cpdef nearest_nonoverlapping(long [::1] prev_ridx, long [::1] prev_dist,             # <<<<<<<<<<<<<<
+ *                              long [::1] next_ridx, long [::1] next_dist):
  * 
  */
 
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_5nearest_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__Pyx_memviewslice __pyx_v_prev_lidx, __Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_lidx, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_i;
   int __pyx_v_length;
-  PyObject *__pyx_v_output_arr_lidx = NULL;
   PyObject *__pyx_v_output_arr_ridx = NULL;
   PyObject *__pyx_v_output_arr_dist = NULL;
-  __Pyx_memviewslice __pyx_v_output_lidx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_output_ridx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_output_dist = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -3022,583 +2828,468 @@
   Py_ssize_t __pyx_t_25;
   Py_ssize_t __pyx_t_26;
   Py_ssize_t __pyx_t_27;
   Py_ssize_t __pyx_t_28;
   Py_ssize_t __pyx_t_29;
   Py_ssize_t __pyx_t_30;
   Py_ssize_t __pyx_t_31;
-  Py_ssize_t __pyx_t_32;
-  Py_ssize_t __pyx_t_33;
-  Py_ssize_t __pyx_t_34;
-  Py_ssize_t __pyx_t_35;
-  Py_ssize_t __pyx_t_36;
-  Py_ssize_t __pyx_t_37;
   __Pyx_RefNannySetupContext("nearest_nonoverlapping", 0);
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":97
- *     # gr2 = pr.PyRanges(df2)
- *     # gr2 = pr.PyRanges(df2)
+  /* "sorted_nearest/src/sorted_nearest.pyx":89
+ *                              long [::1] next_ridx, long [::1] next_dist):
+ * 
  *     cdef int i = 0             # <<<<<<<<<<<<<<
  * 
  *     cdef int length = len(prev_ridx)
  */
   __pyx_v_i = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":99
+  /* "sorted_nearest/src/sorted_nearest.pyx":91
  *     cdef int i = 0
  * 
  *     cdef int length = len(prev_ridx)             # <<<<<<<<<<<<<<
  * 
- *     output_arr_lidx = np.ones(length, dtype=np.long) * -1
+ *     output_arr_ridx = np.ones(length, dtype=np.long) * -1
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_prev_ridx); 
   __pyx_v_length = __pyx_t_1;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":101
+  /* "sorted_nearest/src/sorted_nearest.pyx":93
  *     cdef int length = len(prev_ridx)
  * 
- *     output_arr_lidx = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     output_arr_ridx = np.ones(length, dtype=np.long) * -1
+ *     output_arr_ridx = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  *     output_arr_dist = np.ones(length, dtype=np.long) * -1
+ * 
  */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_6, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_6, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_output_arr_lidx = __pyx_t_2;
+  __pyx_v_output_arr_ridx = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":102
+  /* "sorted_nearest/src/sorted_nearest.pyx":94
  * 
- *     output_arr_lidx = np.ones(length, dtype=np.long) * -1
- *     output_arr_ridx = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- *     output_arr_dist = np.ones(length, dtype=np.long) * -1
+ *     output_arr_ridx = np.ones(length, dtype=np.long) * -1
+ *     output_arr_dist = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  * 
+ *     cdef long [::1] output_ridx
  */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_long); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_long); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_5, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_output_arr_ridx = __pyx_t_2;
-  __pyx_t_2 = 0;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":103
- *     output_arr_lidx = np.ones(length, dtype=np.long) * -1
- *     output_arr_ridx = np.ones(length, dtype=np.long) * -1
- *     output_arr_dist = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
- * 
- *     cdef long [::1] output_lidx
- */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_5, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_long); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_output_arr_dist = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":109
+  /* "sorted_nearest/src/sorted_nearest.pyx":99
  *     cdef long [::1] output_dist
  * 
- *     output_lidx = output_arr_lidx             # <<<<<<<<<<<<<<
- *     output_ridx = output_arr_ridx
- *     output_dist = output_arr_dist
- */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_lidx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_v_output_lidx = __pyx_t_7;
-  __pyx_t_7.memview = NULL;
-  __pyx_t_7.data = NULL;
-
-  /* "sorted_nearest/src/sorted_nearest.pyx":110
- * 
- *     output_lidx = output_arr_lidx
  *     output_ridx = output_arr_ridx             # <<<<<<<<<<<<<<
  *     output_dist = output_arr_dist
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_ridx, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 99, __pyx_L1_error)
   __pyx_v_output_ridx = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":111
- *     output_lidx = output_arr_lidx
+  /* "sorted_nearest/src/sorted_nearest.pyx":100
+ * 
  *     output_ridx = output_arr_ridx
  *     output_dist = output_arr_dist             # <<<<<<<<<<<<<<
  * 
  *     for i in range(length):
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_dist, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 100, __pyx_L1_error)
   __pyx_v_output_dist = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":113
+  /* "sorted_nearest/src/sorted_nearest.pyx":102
  *     output_dist = output_arr_dist
  * 
  *     for i in range(length):             # <<<<<<<<<<<<<<
  *         if next_ridx[i] == -1 and prev_ridx[i] > -1:
- *             output_lidx[i] = prev_lidx[i]
+ *             output_ridx[i] = prev_ridx[i]
  */
   __pyx_t_8 = __pyx_v_length;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":114
+    /* "sorted_nearest/src/sorted_nearest.pyx":103
  * 
  *     for i in range(length):
  *         if next_ridx[i] == -1 and prev_ridx[i] > -1:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]
+ *             output_dist[i] = prev_dist[i]
  */
     __pyx_t_12 = __pyx_v_i;
     __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_ridx.data) + __pyx_t_12)) ))) == -1L) != 0);
     if (__pyx_t_13) {
     } else {
       __pyx_t_11 = __pyx_t_13;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_14 = __pyx_v_i;
     __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_14)) ))) > -1L) != 0);
     __pyx_t_11 = __pyx_t_13;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_11) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":115
+      /* "sorted_nearest/src/sorted_nearest.pyx":104
  *     for i in range(length):
  *         if next_ridx[i] == -1 and prev_ridx[i] > -1:
- *             output_lidx[i] = prev_lidx[i]             # <<<<<<<<<<<<<<
- *             output_ridx[i] = prev_ridx[i]
+ *             output_ridx[i] = prev_ridx[i]             # <<<<<<<<<<<<<<
  *             output_dist[i] = prev_dist[i]
+ *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
  */
       __pyx_t_15 = __pyx_v_i;
       __pyx_t_16 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_lidx.data) + __pyx_t_16)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_lidx.data) + __pyx_t_15)) )));
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_16)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_15)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":116
+      /* "sorted_nearest/src/sorted_nearest.pyx":105
  *         if next_ridx[i] == -1 and prev_ridx[i] > -1:
- *             output_lidx[i] = prev_lidx[i]
- *             output_ridx[i] = prev_ridx[i]             # <<<<<<<<<<<<<<
- *             output_dist[i] = prev_dist[i]
- *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
- */
-      __pyx_t_17 = __pyx_v_i;
-      __pyx_t_18 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_18)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_17)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":117
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]             # <<<<<<<<<<<<<<
  *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
- *             output_lidx[i] = prev_lidx[i]
+ *             output_ridx[i] = prev_ridx[i]
  */
-      __pyx_t_19 = __pyx_v_i;
-      __pyx_t_20 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_20)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_19)) )));
+      __pyx_t_17 = __pyx_v_i;
+      __pyx_t_18 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_18)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_17)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":114
+      /* "sorted_nearest/src/sorted_nearest.pyx":103
  * 
  *     for i in range(length):
  *         if next_ridx[i] == -1 and prev_ridx[i] > -1:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]
+ *             output_dist[i] = prev_dist[i]
  */
       goto __pyx_L5;
     }
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":118
+    /* "sorted_nearest/src/sorted_nearest.pyx":106
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]
  *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]
+ *             output_dist[i] = prev_dist[i]
  */
-    __pyx_t_21 = __pyx_v_i;
-    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_21)) ))) > -1L) != 0);
+    __pyx_t_19 = __pyx_v_i;
+    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_19)) ))) > -1L) != 0);
     if (__pyx_t_13) {
     } else {
       __pyx_t_11 = __pyx_t_13;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_22 = __pyx_v_i;
-    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_ridx.data) + __pyx_t_22)) ))) > -1L) != 0);
+    __pyx_t_20 = __pyx_v_i;
+    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_ridx.data) + __pyx_t_20)) ))) > -1L) != 0);
     if (__pyx_t_13) {
     } else {
       __pyx_t_11 = __pyx_t_13;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_23 = __pyx_v_i;
-    __pyx_t_24 = __pyx_v_i;
-    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_23)) ))) <= (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_24)) )))) != 0);
+    __pyx_t_21 = __pyx_v_i;
+    __pyx_t_22 = __pyx_v_i;
+    __pyx_t_13 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_21)) ))) <= (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_22)) )))) != 0);
     __pyx_t_11 = __pyx_t_13;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_11) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":119
+      /* "sorted_nearest/src/sorted_nearest.pyx":107
  *             output_dist[i] = prev_dist[i]
  *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
- *             output_lidx[i] = prev_lidx[i]             # <<<<<<<<<<<<<<
- *             output_ridx[i] = prev_ridx[i]
- *             output_dist[i] = prev_dist[i]
- */
-      __pyx_t_25 = __pyx_v_i;
-      __pyx_t_26 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_lidx.data) + __pyx_t_26)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_lidx.data) + __pyx_t_25)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":120
- *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]             # <<<<<<<<<<<<<<
  *             output_dist[i] = prev_dist[i]
  *         elif next_dist[i] > -1:
  */
-      __pyx_t_27 = __pyx_v_i;
-      __pyx_t_28 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_28)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_27)) )));
+      __pyx_t_23 = __pyx_v_i;
+      __pyx_t_24 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_24)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_ridx.data) + __pyx_t_23)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":121
- *             output_lidx[i] = prev_lidx[i]
+      /* "sorted_nearest/src/sorted_nearest.pyx":108
+ *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]             # <<<<<<<<<<<<<<
  *         elif next_dist[i] > -1:
- *             output_lidx[i] = next_lidx[i]
+ *             output_ridx[i] = next_ridx[i]
  */
-      __pyx_t_29 = __pyx_v_i;
-      __pyx_t_30 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_30)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_29)) )));
+      __pyx_t_25 = __pyx_v_i;
+      __pyx_t_26 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_26)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_prev_dist.data) + __pyx_t_25)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":118
+      /* "sorted_nearest/src/sorted_nearest.pyx":106
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]
  *         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = prev_lidx[i]
  *             output_ridx[i] = prev_ridx[i]
+ *             output_dist[i] = prev_dist[i]
  */
       goto __pyx_L5;
     }
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":122
+    /* "sorted_nearest/src/sorted_nearest.pyx":109
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]
  *         elif next_dist[i] > -1:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = next_lidx[i]
  *             output_ridx[i] = next_ridx[i]
+ *             output_dist[i] = next_dist[i]
  */
-    __pyx_t_31 = __pyx_v_i;
-    __pyx_t_11 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_31)) ))) > -1L) != 0);
+    __pyx_t_27 = __pyx_v_i;
+    __pyx_t_11 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_27)) ))) > -1L) != 0);
     if (__pyx_t_11) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":123
+      /* "sorted_nearest/src/sorted_nearest.pyx":110
  *             output_dist[i] = prev_dist[i]
  *         elif next_dist[i] > -1:
- *             output_lidx[i] = next_lidx[i]             # <<<<<<<<<<<<<<
- *             output_ridx[i] = next_ridx[i]
- *             output_dist[i] = next_dist[i]
- */
-      __pyx_t_32 = __pyx_v_i;
-      __pyx_t_33 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_lidx.data) + __pyx_t_33)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_lidx.data) + __pyx_t_32)) )));
-
-      /* "sorted_nearest/src/sorted_nearest.pyx":124
- *         elif next_dist[i] > -1:
- *             output_lidx[i] = next_lidx[i]
  *             output_ridx[i] = next_ridx[i]             # <<<<<<<<<<<<<<
  *             output_dist[i] = next_dist[i]
  * 
  */
-      __pyx_t_34 = __pyx_v_i;
-      __pyx_t_35 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_35)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_ridx.data) + __pyx_t_34)) )));
+      __pyx_t_28 = __pyx_v_i;
+      __pyx_t_29 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_ridx.data) + __pyx_t_29)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_ridx.data) + __pyx_t_28)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":125
- *             output_lidx[i] = next_lidx[i]
+      /* "sorted_nearest/src/sorted_nearest.pyx":111
+ *         elif next_dist[i] > -1:
  *             output_ridx[i] = next_ridx[i]
  *             output_dist[i] = next_dist[i]             # <<<<<<<<<<<<<<
  * 
- *     return output_arr_lidx, output_arr_ridx, output_arr_dist
+ *     return output_arr_ridx, output_arr_dist
  */
-      __pyx_t_36 = __pyx_v_i;
-      __pyx_t_37 = __pyx_v_i;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_37)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_36)) )));
+      __pyx_t_30 = __pyx_v_i;
+      __pyx_t_31 = __pyx_v_i;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_dist.data) + __pyx_t_31)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_next_dist.data) + __pyx_t_30)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":122
+      /* "sorted_nearest/src/sorted_nearest.pyx":109
  *             output_ridx[i] = prev_ridx[i]
  *             output_dist[i] = prev_dist[i]
  *         elif next_dist[i] > -1:             # <<<<<<<<<<<<<<
- *             output_lidx[i] = next_lidx[i]
  *             output_ridx[i] = next_ridx[i]
+ *             output_dist[i] = next_dist[i]
  */
     }
     __pyx_L5:;
   }
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":127
+  /* "sorted_nearest/src/sorted_nearest.pyx":113
  *             output_dist[i] = next_dist[i]
  * 
- *     return output_arr_lidx, output_arr_ridx, output_arr_dist             # <<<<<<<<<<<<<<
+ *     return output_arr_ridx, output_arr_dist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_output_arr_lidx);
-  __Pyx_GIVEREF(__pyx_v_output_arr_lidx);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_output_arr_lidx);
   __Pyx_INCREF(__pyx_v_output_arr_ridx);
   __Pyx_GIVEREF(__pyx_v_output_arr_ridx);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_output_arr_ridx);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_output_arr_ridx);
   __Pyx_INCREF(__pyx_v_output_arr_dist);
   __Pyx_GIVEREF(__pyx_v_output_arr_dist);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_output_arr_dist);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_output_arr_dist);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":90
+  /* "sorted_nearest/src/sorted_nearest.pyx":86
+ * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * @cython.initializedcheck(False)
- * cpdef nearest_nonoverlapping(long [::1] prev_lidx, long [::1] prev_ridx, long [::1] prev_dist,             # <<<<<<<<<<<<<<
- *                              long [::1] next_lidx, long [::1] next_ridx, long [::1] next_dist):
+ * cpdef nearest_nonoverlapping(long [::1] prev_ridx, long [::1] prev_dist,             # <<<<<<<<<<<<<<
+ *                              long [::1] next_ridx, long [::1] next_dist):
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_output_arr_lidx);
   __Pyx_XDECREF(__pyx_v_output_arr_ridx);
   __Pyx_XDECREF(__pyx_v_output_arr_dist);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_output_lidx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_output_ridx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_output_dist, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_5nearest_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_14sorted_nearest_3src_14sorted_nearest_5nearest_nonoverlapping(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  __Pyx_memviewslice __pyx_v_prev_lidx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_prev_ridx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_prev_dist = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __Pyx_memviewslice __pyx_v_next_lidx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_next_ridx = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_next_dist = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("nearest_nonoverlapping (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_prev_lidx,&__pyx_n_s_prev_ridx,&__pyx_n_s_prev_dist,&__pyx_n_s_next_lidx,&__pyx_n_s_next_ridx,&__pyx_n_s_next_dist,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_prev_ridx,&__pyx_n_s_prev_dist,&__pyx_n_s_next_ridx,&__pyx_n_s_next_dist,0};
+    PyObject* values[4] = {0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_prev_lidx)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_prev_ridx)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_prev_ridx)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_prev_dist)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, 1); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 4, 4, 1); __PYX_ERR(0, 86, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_prev_dist)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_next_ridx)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, 2); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 4, 4, 2); __PYX_ERR(0, 86, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_next_lidx)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, 3); __PYX_ERR(0, 90, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_next_ridx)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_next_dist)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, 4); __PYX_ERR(0, 90, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_next_dist)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, 5); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 4, 4, 3); __PYX_ERR(0, 86, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest_nonoverlapping") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest_nonoverlapping") < 0)) __PYX_ERR(0, 86, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_prev_lidx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_prev_lidx.memview)) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_prev_ridx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_prev_ridx.memview)) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_prev_dist = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_prev_dist.memview)) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_next_lidx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_next_lidx.memview)) __PYX_ERR(0, 91, __pyx_L3_error)
-    __pyx_v_next_ridx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_next_ridx.memview)) __PYX_ERR(0, 91, __pyx_L3_error)
-    __pyx_v_next_dist = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_next_dist.memview)) __PYX_ERR(0, 91, __pyx_L3_error)
+    __pyx_v_prev_ridx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_prev_ridx.memview)) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_prev_dist = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_prev_dist.memview)) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_next_ridx = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_next_ridx.memview)) __PYX_ERR(0, 87, __pyx_L3_error)
+    __pyx_v_next_dist = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_next_dist.memview)) __PYX_ERR(0, 87, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("nearest_nonoverlapping", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 86, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(__pyx_self, __pyx_v_prev_lidx, __pyx_v_prev_ridx, __pyx_v_prev_dist, __pyx_v_next_lidx, __pyx_v_next_ridx, __pyx_v_next_dist);
+  __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(__pyx_self, __pyx_v_prev_ridx, __pyx_v_prev_dist, __pyx_v_next_ridx, __pyx_v_next_dist);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_prev_lidx, __Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_lidx, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist) {
+static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_4nearest_nonoverlapping(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_prev_ridx, __Pyx_memviewslice __pyx_v_prev_dist, __Pyx_memviewslice __pyx_v_next_ridx, __Pyx_memviewslice __pyx_v_next_dist) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("nearest_nonoverlapping", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__pyx_v_prev_lidx, __pyx_v_prev_ridx, __pyx_v_prev_dist, __pyx_v_next_lidx, __pyx_v_next_ridx, __pyx_v_next_dist, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (unlikely(!__pyx_v_prev_ridx.memview)) { __Pyx_RaiseUnboundLocalError("prev_ridx"); __PYX_ERR(0, 86, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_prev_dist.memview)) { __Pyx_RaiseUnboundLocalError("prev_dist"); __PYX_ERR(0, 86, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_next_ridx.memview)) { __Pyx_RaiseUnboundLocalError("next_ridx"); __PYX_ERR(0, 86, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_next_dist.memview)) { __Pyx_RaiseUnboundLocalError("next_dist"); __PYX_ERR(0, 86, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_nearest_nonoverlapping(__pyx_v_prev_ridx, __pyx_v_prev_dist, __pyx_v_next_ridx, __pyx_v_next_dist, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.nearest_nonoverlapping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_prev_lidx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_prev_ridx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_prev_dist, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_next_lidx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_next_ridx, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_next_dist, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sorted_nearest/src/sorted_nearest.pyx":192
+/* "sorted_nearest/src/sorted_nearest.pyx":119
  * @cython.wraparound(False)
  * @cython.initializedcheck(False)
  * cpdef find_clusters(long [::1] starts, long [::1] ends):             # <<<<<<<<<<<<<<
  * 
  *     cpdef int min_start = starts[0]
  */
 
@@ -3633,363 +3324,363 @@
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   Py_ssize_t __pyx_t_20;
   __Pyx_RefNannySetupContext("find_clusters", 0);
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":194
+  /* "sorted_nearest/src/sorted_nearest.pyx":121
  * cpdef find_clusters(long [::1] starts, long [::1] ends):
  * 
  *     cpdef int min_start = starts[0]             # <<<<<<<<<<<<<<
  *     cpdef int max_end = ends[0]
  *     cpdef int i = 0
  */
   __pyx_t_1 = 0;
   __pyx_v_min_start = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_starts.data) + __pyx_t_1)) )));
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":195
+  /* "sorted_nearest/src/sorted_nearest.pyx":122
  * 
  *     cpdef int min_start = starts[0]
  *     cpdef int max_end = ends[0]             # <<<<<<<<<<<<<<
  *     cpdef int i = 0
  *     cpdef int n_clusters = 0
  */
   __pyx_t_2 = 0;
   __pyx_v_max_end = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ends.data) + __pyx_t_2)) )));
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":196
+  /* "sorted_nearest/src/sorted_nearest.pyx":123
  *     cpdef int min_start = starts[0]
  *     cpdef int max_end = ends[0]
  *     cpdef int i = 0             # <<<<<<<<<<<<<<
  *     cpdef int n_clusters = 0
  *     cpdef int length = len(starts)
  */
   __pyx_v_i = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":197
+  /* "sorted_nearest/src/sorted_nearest.pyx":124
  *     cpdef int max_end = ends[0]
  *     cpdef int i = 0
  *     cpdef int n_clusters = 0             # <<<<<<<<<<<<<<
  *     cpdef int length = len(starts)
  * 
  */
   __pyx_v_n_clusters = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":198
+  /* "sorted_nearest/src/sorted_nearest.pyx":125
  *     cpdef int i = 0
  *     cpdef int n_clusters = 0
  *     cpdef int length = len(starts)             # <<<<<<<<<<<<<<
  * 
  *     output_arr_start = np.ones(length, dtype=np.long) * -1
  */
   __pyx_t_3 = __Pyx_MemoryView_Len(__pyx_v_starts); 
   __pyx_v_length = __pyx_t_3;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":200
+  /* "sorted_nearest/src/sorted_nearest.pyx":127
  *     cpdef int length = len(starts)
  * 
  *     output_arr_start = np.ones(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  *     output_arr_end = np.zeros(length, dtype=np.long) * -1
  * 
  */
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ones); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ones); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_long); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_long); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_8, __pyx_int_neg_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_8, __pyx_int_neg_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_output_arr_start = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":201
+  /* "sorted_nearest/src/sorted_nearest.pyx":128
  * 
  *     output_arr_start = np.ones(length, dtype=np.long) * -1
  *     output_arr_end = np.zeros(length, dtype=np.long) * -1             # <<<<<<<<<<<<<<
  * 
  *     cdef long [::1] output_start
  */
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_long); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_7, __pyx_int_neg_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_7, __pyx_int_neg_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_output_arr_end = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":206
+  /* "sorted_nearest/src/sorted_nearest.pyx":133
  *     cdef long [::1] output_end
  * 
  *     output_start = output_arr_start             # <<<<<<<<<<<<<<
  *     output_end = output_arr_end
  * 
  */
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_start, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_start, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 133, __pyx_L1_error)
   __pyx_v_output_start = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":207
+  /* "sorted_nearest/src/sorted_nearest.pyx":134
  * 
  *     output_start = output_arr_start
  *     output_end = output_arr_end             # <<<<<<<<<<<<<<
  * 
  *     for i in range(length):
  */
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_end, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_output_arr_end, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 134, __pyx_L1_error)
   __pyx_v_output_end = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":209
+  /* "sorted_nearest/src/sorted_nearest.pyx":136
  *     output_end = output_arr_end
  * 
  *     for i in range(length):             # <<<<<<<<<<<<<<
  *         if not starts[i] <= max_end:
  *             output_start[n_clusters] = min_start
  */
   __pyx_t_10 = __pyx_v_length;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_i = __pyx_t_12;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":210
+    /* "sorted_nearest/src/sorted_nearest.pyx":137
  * 
  *     for i in range(length):
  *         if not starts[i] <= max_end:             # <<<<<<<<<<<<<<
  *             output_start[n_clusters] = min_start
  *             output_end[n_clusters] = max_end
  */
     __pyx_t_13 = __pyx_v_i;
     __pyx_t_14 = ((!(((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_starts.data) + __pyx_t_13)) ))) <= __pyx_v_max_end) != 0)) != 0);
     if (__pyx_t_14) {
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":211
+      /* "sorted_nearest/src/sorted_nearest.pyx":138
  *     for i in range(length):
  *         if not starts[i] <= max_end:
  *             output_start[n_clusters] = min_start             # <<<<<<<<<<<<<<
  *             output_end[n_clusters] = max_end
  *             min_start = starts[i]
  */
       __pyx_t_15 = __pyx_v_n_clusters;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_start.data) + __pyx_t_15)) )) = __pyx_v_min_start;
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":212
+      /* "sorted_nearest/src/sorted_nearest.pyx":139
  *         if not starts[i] <= max_end:
  *             output_start[n_clusters] = min_start
  *             output_end[n_clusters] = max_end             # <<<<<<<<<<<<<<
  *             min_start = starts[i]
  *             max_end = ends[i]
  */
       __pyx_t_16 = __pyx_v_n_clusters;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_output_end.data) + __pyx_t_16)) )) = __pyx_v_max_end;
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":213
+      /* "sorted_nearest/src/sorted_nearest.pyx":140
  *             output_start[n_clusters] = min_start
  *             output_end[n_clusters] = max_end
  *             min_start = starts[i]             # <<<<<<<<<<<<<<
  *             max_end = ends[i]
  *             n_clusters += 1
  */
       __pyx_t_17 = __pyx_v_i;
       __pyx_v_min_start = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_starts.data) + __pyx_t_17)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":214
+      /* "sorted_nearest/src/sorted_nearest.pyx":141
  *             output_end[n_clusters] = max_end
  *             min_start = starts[i]
  *             max_end = ends[i]             # <<<<<<<<<<<<<<
  *             n_clusters += 1
  *         else:
  */
       __pyx_t_18 = __pyx_v_i;
       __pyx_v_max_end = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ends.data) + __pyx_t_18)) )));
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":215
+      /* "sorted_nearest/src/sorted_nearest.pyx":142
  *             min_start = starts[i]
  *             max_end = ends[i]
  *             n_clusters += 1             # <<<<<<<<<<<<<<
  *         else:
  *             if ends[i] > max_end:
  */
       __pyx_v_n_clusters = (__pyx_v_n_clusters + 1);
 
-      /* "sorted_nearest/src/sorted_nearest.pyx":210
+      /* "sorted_nearest/src/sorted_nearest.pyx":137
  * 
  *     for i in range(length):
  *         if not starts[i] <= max_end:             # <<<<<<<<<<<<<<
  *             output_start[n_clusters] = min_start
  *             output_end[n_clusters] = max_end
  */
       goto __pyx_L5;
     }
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":217
+    /* "sorted_nearest/src/sorted_nearest.pyx":144
  *             n_clusters += 1
  *         else:
  *             if ends[i] > max_end:             # <<<<<<<<<<<<<<
  *                 max_end = ends[i]
  * 
  */
     /*else*/ {
       __pyx_t_19 = __pyx_v_i;
       __pyx_t_14 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ends.data) + __pyx_t_19)) ))) > __pyx_v_max_end) != 0);
       if (__pyx_t_14) {
 
-        /* "sorted_nearest/src/sorted_nearest.pyx":218
+        /* "sorted_nearest/src/sorted_nearest.pyx":145
  *         else:
  *             if ends[i] > max_end:
  *                 max_end = ends[i]             # <<<<<<<<<<<<<<
  * 
  *     if output_arr_start[n_clusters] != min_start:
  */
         __pyx_t_20 = __pyx_v_i;
         __pyx_v_max_end = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ends.data) + __pyx_t_20)) )));
 
-        /* "sorted_nearest/src/sorted_nearest.pyx":217
+        /* "sorted_nearest/src/sorted_nearest.pyx":144
  *             n_clusters += 1
  *         else:
  *             if ends[i] > max_end:             # <<<<<<<<<<<<<<
  *                 max_end = ends[i]
  * 
  */
       }
     }
     __pyx_L5:;
   }
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":220
+  /* "sorted_nearest/src/sorted_nearest.pyx":147
  *                 max_end = ends[i]
  * 
  *     if output_arr_start[n_clusters] != min_start:             # <<<<<<<<<<<<<<
  *         output_arr_start[n_clusters] = min_start
  *         output_arr_end[n_clusters] = max_end
  */
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_output_arr_start, __pyx_v_n_clusters, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_output_arr_start, __pyx_v_n_clusters, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_min_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_min_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_7, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_7, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_14) {
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":221
+    /* "sorted_nearest/src/sorted_nearest.pyx":148
  * 
  *     if output_arr_start[n_clusters] != min_start:
  *         output_arr_start[n_clusters] = min_start             # <<<<<<<<<<<<<<
  *         output_arr_end[n_clusters] = max_end
  *         n_clusters += 1
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_min_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_min_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_output_arr_start, __pyx_v_n_clusters, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 0, 0) < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_output_arr_start, __pyx_v_n_clusters, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 0, 0) < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":222
+    /* "sorted_nearest/src/sorted_nearest.pyx":149
  *     if output_arr_start[n_clusters] != min_start:
  *         output_arr_start[n_clusters] = min_start
  *         output_arr_end[n_clusters] = max_end             # <<<<<<<<<<<<<<
  *         n_clusters += 1
  * 
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_max_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_max_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_output_arr_end, __pyx_v_n_clusters, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 0, 0) < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_output_arr_end, __pyx_v_n_clusters, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 0, 0) < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":223
+    /* "sorted_nearest/src/sorted_nearest.pyx":150
  *         output_arr_start[n_clusters] = min_start
  *         output_arr_end[n_clusters] = max_end
  *         n_clusters += 1             # <<<<<<<<<<<<<<
  * 
  *     return output_arr_start[:n_clusters], output_arr_end[:n_clusters]
  */
     __pyx_v_n_clusters = (__pyx_v_n_clusters + 1);
 
-    /* "sorted_nearest/src/sorted_nearest.pyx":220
+    /* "sorted_nearest/src/sorted_nearest.pyx":147
  *                 max_end = ends[i]
  * 
  *     if output_arr_start[n_clusters] != min_start:             # <<<<<<<<<<<<<<
  *         output_arr_start[n_clusters] = min_start
  *         output_arr_end[n_clusters] = max_end
  */
   }
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":225
+  /* "sorted_nearest/src/sorted_nearest.pyx":152
  *         n_clusters += 1
  * 
  *     return output_arr_start[:n_clusters], output_arr_end[:n_clusters]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetSlice(__pyx_v_output_arr_start, 0, __pyx_v_n_clusters, NULL, NULL, NULL, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetSlice(__pyx_v_output_arr_start, 0, __pyx_v_n_clusters, NULL, NULL, NULL, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetSlice(__pyx_v_output_arr_end, 0, __pyx_v_n_clusters, NULL, NULL, NULL, 0, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetSlice(__pyx_v_output_arr_end, 0, __pyx_v_n_clusters, NULL, NULL, NULL, 0, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "sorted_nearest/src/sorted_nearest.pyx":192
+  /* "sorted_nearest/src/sorted_nearest.pyx":119
  * @cython.wraparound(False)
  * @cython.initializedcheck(False)
  * cpdef find_clusters(long [::1] starts, long [::1] ends):             # <<<<<<<<<<<<<<
  * 
  *     cpdef int min_start = starts[0]
  */
 
@@ -4040,32 +3731,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_starts)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ends)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("find_clusters", 1, 2, 2, 1); __PYX_ERR(0, 192, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("find_clusters", 1, 2, 2, 1); __PYX_ERR(0, 119, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "find_clusters") < 0)) __PYX_ERR(0, 192, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "find_clusters") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_starts = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_starts.memview)) __PYX_ERR(0, 192, __pyx_L3_error)
-    __pyx_v_ends = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ends.memview)) __PYX_ERR(0, 192, __pyx_L3_error)
+    __pyx_v_starts = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_starts.memview)) __PYX_ERR(0, 119, __pyx_L3_error)
+    __pyx_v_ends = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ends.memview)) __PYX_ERR(0, 119, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("find_clusters", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 192, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("find_clusters", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("sorted_nearest.src.sorted_nearest.find_clusters", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_14sorted_nearest_3src_14sorted_nearest_6find_clusters(__pyx_self, __pyx_v_starts, __pyx_v_ends);
 
@@ -4076,15 +3767,15 @@
 
 static PyObject *__pyx_pf_14sorted_nearest_3src_14sorted_nearest_6find_clusters(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ends) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("find_clusters", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_find_clusters(__pyx_v_starts, __pyx_v_ends, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_14sorted_nearest_3src_14sorted_nearest_find_clusters(__pyx_v_starts, __pyx_v_ends, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17772,36 +17463,33 @@
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_l_e, __pyx_k_l_e, sizeof(__pyx_k_l_e), 0, 0, 1, 1},
-  {&__pyx_n_s_l_idx, __pyx_k_l_idx, sizeof(__pyx_k_l_idx), 0, 0, 1, 1},
   {&__pyx_n_s_l_s, __pyx_k_l_s, sizeof(__pyx_k_l_s), 0, 0, 1, 1},
   {&__pyx_n_s_long, __pyx_k_long, sizeof(__pyx_k_long), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_next_dist, __pyx_k_next_dist, sizeof(__pyx_k_next_dist), 0, 0, 1, 1},
-  {&__pyx_n_s_next_lidx, __pyx_k_next_lidx, sizeof(__pyx_k_next_lidx), 0, 0, 1, 1},
   {&__pyx_n_s_next_ridx, __pyx_k_next_ridx, sizeof(__pyx_k_next_ridx), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_ones, __pyx_k_ones, sizeof(__pyx_k_ones), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_prev_dist, __pyx_k_prev_dist, sizeof(__pyx_k_prev_dist), 0, 0, 1, 1},
-  {&__pyx_n_s_prev_lidx, __pyx_k_prev_lidx, sizeof(__pyx_k_prev_lidx), 0, 0, 1, 1},
   {&__pyx_n_s_prev_ridx, __pyx_k_prev_ridx, sizeof(__pyx_k_prev_ridx), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
@@ -17832,15 +17520,15 @@
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 102, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 132, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 147, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 150, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 399, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 608, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 827, __pyx_L1_error)
@@ -18450,15 +18138,15 @@
   #endif
 
   /* "sorted_nearest/src/sorted_nearest.pyx":5
  * cimport cython
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
- * @cython.boundscheck(False)
+ * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "sorted_nearest/src/sorted_nearest.pyx":1
@@ -19017,14 +18705,19 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* None */
+    static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
+    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
+}
+
 /* GetItemInt */
     static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -20359,19 +20052,14 @@
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* None */
-        static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
-}
-
-/* None */
         static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
```

### Comparing `sorted_nearest-0.0.8/sorted_nearest/src/sorted_nearest.pyx` & `sorted_nearest-0.0.9/sorted_nearest/src/sorted_nearest.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,120 @@
 cimport sorted_nearest.src.csorted_nearest as cn
 
 cimport cython
 
 import numpy as np
 
+
 @cython.boundscheck(False)
 @cython.wraparound(False)
-@cython.initializedcheck(False)
-cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] l_idx, long [::1] r_s, long [::1] r_idx):
+cpdef nearest_next_nonoverlapping(long [::1] l_e, long [::1] r_s, long [::1] r_idx):
 
     cdef int j = 0
     cdef int i = 0
 
     cdef int len_l = len(l_e)
     cdef int len_r = len(r_s)
 
-    arr_lidx = np.ones(len_l, dtype=np.long) * -1
     arr_ridx = np.ones(len_l, dtype=np.long) * -1
     arr_dist = np.ones(len_l, dtype=np.long) * -1
-    cdef long [::1] lidx
     cdef long [::1] ridx
     cdef long [::1] dist
 
-    lidx = arr_lidx
     ridx = arr_ridx
     dist = arr_dist
 
     # print("l_e", list(l_e))
     # print("r_s", list(r_s))
     while i < len_l and j < len_r:
         # print("l_e[i]", l_e[i])
         # print("r_s[j]", r_s[j])
         if l_e[i] >= r_s[j]:
             # print("in if")
             j += 1
-            lidx[i] = l_idx[i]
         else:
             # print("in else")
             dist[i] = r_s[j] - l_e[i]
             ridx[i] = r_idx[j]
-            lidx[i] = l_idx[i]
             i += 1
         # print("dist", list(dist))
         # print("ridx", list(ridx))
 
-    return arr_lidx, arr_ridx, arr_dist
+    return arr_ridx, arr_dist
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-@cython.initializedcheck(False)
-cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] l_idx, long [::1] r_e, long [::1] r_idx):
+cpdef nearest_previous_nonoverlapping(long [::1] l_s, long [::1] r_e, long [::1] r_idx):
 
     cdef int len_l = len(l_s)
     cdef int len_r = len(r_e)
 
     cdef int j = len_r - 1
     cdef int i = len_l - 1
 
-    arr_lidx = np.ones(len_l, dtype=np.long) * -1
     arr_ridx = np.ones(len_l, dtype=np.long) * -1
     arr_dist = np.ones(len_l, dtype=np.long) * -1
-    cdef long [::1] lidx
     cdef long [::1] ridx
     cdef long [::1] dist
 
-    lidx = arr_lidx
     ridx = arr_ridx
     dist = arr_dist
 
-
     while -1 < i and -1 < j:
         if l_s[i] <= r_e[j]:
+            # print("in if")
             j -= 1
-            lidx[i] = l_idx[i]
         else:
+            # print("in else")
+            # print("l_s[i]", l_s[i])
+            # print("r_e[j]", r_e[j])
             dist[i] = l_s[i] - r_e[j]
             ridx[i] = r_idx[j]
-            lidx[i] = l_idx[i]
             i -= 1
+        # print("dist", list(dist))
+        # print("ridx", list(ridx))
+
+    # print("final dist", list(dist))
+    # print("final ridx", list(ridx))
 
-    return arr_lidx, arr_ridx, arr_dist
+    return arr_ridx, arr_dist
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-@cython.initializedcheck(False)
-cpdef nearest_nonoverlapping(long [::1] prev_lidx, long [::1] prev_ridx, long [::1] prev_dist,
-                             long [::1] next_lidx, long [::1] next_ridx, long [::1] next_dist):
+cpdef nearest_nonoverlapping(long [::1] prev_ridx, long [::1] prev_dist,
+                             long [::1] next_ridx, long [::1] next_dist):
 
-    # gr = pr.PyRanges(df)
-    # gr = pr.PyRanges(df)
-    # gr2 = pr.PyRanges(df2)
-    # gr2 = pr.PyRanges(df2)
     cdef int i = 0
 
     cdef int length = len(prev_ridx)
 
-    output_arr_lidx = np.ones(length, dtype=np.long) * -1
     output_arr_ridx = np.ones(length, dtype=np.long) * -1
     output_arr_dist = np.ones(length, dtype=np.long) * -1
 
-    cdef long [::1] output_lidx
     cdef long [::1] output_ridx
     cdef long [::1] output_dist
 
-    output_lidx = output_arr_lidx
     output_ridx = output_arr_ridx
     output_dist = output_arr_dist
 
     for i in range(length):
         if next_ridx[i] == -1 and prev_ridx[i] > -1:
-            output_lidx[i] = prev_lidx[i]
             output_ridx[i] = prev_ridx[i]
             output_dist[i] = prev_dist[i]
         elif prev_ridx[i] > -1 and next_ridx[i] > -1 and prev_dist[i] <= next_dist[i]:
-            output_lidx[i] = prev_lidx[i]
             output_ridx[i] = prev_ridx[i]
             output_dist[i] = prev_dist[i]
         elif next_dist[i] > -1:
-            output_lidx[i] = next_lidx[i]
             output_ridx[i] = next_ridx[i]
             output_dist[i] = next_dist[i]
 
-    return output_arr_lidx, output_arr_ridx, output_arr_dist
-
-
-# @cython.boundscheck(False)
-# @cython.wraparound(False)
-# @cython.initializedcheck(False)
-# cpdef merge_sort_overlapping_and_nearest(long [::1] o_lidx, long [::1] o_ridx,
-#                                          long [::1] n_lidx, long [::1] n_ridx, long[::1] n_dist):
-
-#     cpdef int nc = 0
-#     cpdef int oc = 0
-#     cpdef int i = 0
-#     cpdef int nlen = len(n_lidx)
-#     cpdef int olen = len(o_lidx)
-#     cpdef int total_len = nlen + olen
-
-#     output_arr_lidx = np.ones(total_len, dtype=np.long) * -1
-#     output_arr_ridx = np.ones(total_len, dtype=np.long) * -1
-#     output_arr_dist = np.zeros(total_len, dtype=np.long)
-
-#     cdef long [::1] output_lidx
-#     cdef long [::1] output_ridx
-#     cdef long [::1] output_dist
-
-#     output_lidx = output_arr_lidx
-#     output_ridx = output_arr_ridx
-#     output_dist = output_arr_dist
-
-#     while nc < nlen and oc < olen:
-
-#         if n_lidx[nc] == i:
-#             output_lidx[i] = n_lidx[nc]
-#             output_ridx[i] = n_ridx[nc]
-#             output_dist[i] = n_dist[nc]
-#             nc += 1
-#         elif o_lidx[oc] == i:
-#             output_lidx[i] = o_lidx[oc]
-#             output_ridx[i] = o_ridx[oc]
-#             oc += 1
-
-#         i += 1
-
-#     while nc < nlen:
-#         output_lidx[i] = n_lidx[nc]
-#         output_ridx[i] = n_ridx[nc]
-#         output_dist[i] = n_dist[nc]
-#         nc += 1
-#         i += 1
-
-#     while oc < olen:
-#         output_lidx[i] = o_lidx[oc]
-#         output_ridx[i] = o_ridx[oc]
-#         oc += 1
-#         i += 1
-
-#     return output_arr_lidx, output_arr_ridx, output_arr_dist
-
-
-
-
+    return output_arr_ridx, output_arr_dist
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.initializedcheck(False)
 cpdef find_clusters(long [::1] starts, long [::1] ends):
```

### Comparing `sorted_nearest-0.0.8/sorted_nearest/src/utarray.h` & `sorted_nearest-0.0.9/sorted_nearest/src/utarray.h`

 * *Files identical despite different names*

### Comparing `sorted_nearest-0.0.8/PKG-INFO` & `sorted_nearest-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sorted_nearest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Find nearest interval.
 Home-page: https://github.com/endrebak/sorted_nearest
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: New BSD License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `sorted_nearest-0.0.8/setup.py` & `sorted_nearest-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 extensions = [Extension("sorted_nearest.src.sorted_nearest", ["sorted_nearest/src/sorted_nearest.pyx"],
                         define_macros=macros)]
 
 
 setup(
     name = "sorted_nearest",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     ext_modules = cythonize(extensions),
     description = \
     'Find nearest interval.',
     long_description = __doc__,
     author = "Endre Bakken Stovner",
     author_email='endrebak85@gmail.com',
```

