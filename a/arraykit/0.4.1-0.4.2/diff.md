# Comparing `tmp/arraykit-0.4.1.tar.gz` & `tmp/arraykit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.1.tar", last modified: Wed May 17 23:06:51 2023, max compression
+gzip compressed data, was "arraykit-0.4.2.tar", last modified: Thu May 18 23:34:04 2023, max compression
```

## Comparing `arraykit-0.4.1.tar` & `arraykit-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-17 23:06:45.000000 arraykit-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-17 23:06:45.000000 arraykit-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-17 23:06:51.449581 arraykit-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-05-17 23:06:45.000000 arraykit-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 23:06:51.449581 arraykit-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-17 23:06:45.000000 arraykit-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-05-17 23:06:45.000000 arraykit-0.4.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   175735 2023-05-17 23:06:45.000000 arraykit-0.4.1/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    18219 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:34:04.074422 arraykit-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-18 23:33:57.000000 arraykit-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 23:33:57.000000 arraykit-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-18 23:34:04.074422 arraykit-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-18 23:33:57.000000 arraykit-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:34:04.074422 arraykit-0.4.2/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-18 23:34:03.000000 arraykit-0.4.2/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-18 23:34:04.000000 arraykit-0.4.2/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:34:03.000000 arraykit-0.4.2/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 23:34:03.000000 arraykit-0.4.2/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 23:34:03.000000 arraykit-0.4.2/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:34:04.074422 arraykit-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-18 23:33:57.000000 arraykit-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:34:04.074422 arraykit-0.4.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-18 23:33:57.000000 arraykit-0.4.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178131 2023-05-18 23:33:57.000000 arraykit-0.4.2/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:34:04.074422 arraykit-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19339 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-05-18 23:33:57.000000 arraykit-0.4.2/test/test_util.py
```

### Comparing `arraykit-0.4.1/LICENSE.txt` & `arraykit-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/PKG-INFO` & `arraykit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.1/README.rst` & `arraykit-0.4.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,24 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.2
+............
+
+Added ``slice_to_ascending_slice()``.
+
+Updated ``BlockIndex.shape`` to internally cache the shape tuple.
+
+Corrected ``BlockIndex.iter_select()`` handling of negative integers in sequences.
+
+
 0.4.1
 ............
 
 Updated ``BlockIndex.register()`` to handle 0-column 2D arrays and return False.
 
 Added ``BlockIndex.rows``, ``BlockIndex.columns`` properties.
```

### Comparing `arraykit-0.4.1/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.2/arraykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.1/setup.py` & `arraykit-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.1'
+AK_VERSION = '0.4.2'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.1/src/__init__.py` & `arraykit-0.4.2/src/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 from ._arraykit import delimited_to_arrays as delimited_to_arrays
 from ._arraykit import iterable_str_to_array_1d as iterable_str_to_array_1d
 from ._arraykit import get_new_indexers_and_screen as get_new_indexers_and_screen
 from ._arraykit import split_after_count as split_after_count
 from ._arraykit import count_iteration as count_iteration
 from ._arraykit import first_true_1d as first_true_1d
 from ._arraykit import first_true_2d as first_true_2d
+from ._arraykit import slice_to_ascending_slice as slice_to_ascending_slice
```

### Comparing `arraykit-0.4.1/src/_arraykit.c` & `arraykit-0.4.2/src/_arraykit.c`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 # include "numpy/halffloat.h"
 
 //------------------------------------------------------------------------------
 // Macros
 
 //------------------------------------------------------------------------------
 // Given a PyObject, raise if not an array.
-# define AK_CHECK_NUMPY_ARRAY(O)                                              \
-    if (!PyArray_Check(O)) {                                                  \
-        return PyErr_Format(PyExc_TypeError, "Expected NumPy array (got %s)", \
-                            Py_TYPE(O)->tp_name);                             \
+# define AK_CHECK_NUMPY_ARRAY(O)                 \
+    if (!PyArray_Check(O)) {                     \
+        return PyErr_Format(PyExc_TypeError,     \
+                "Expected NumPy array, not %s.", \
+                Py_TYPE(O)->tp_name);            \
     }
 
 // Given a PyObject, raise if not an array or is not one or two dimensional.
 # define AK_CHECK_NUMPY_ARRAY_1D_2D(O)                    \
     do {                                                  \
         AK_CHECK_NUMPY_ARRAY(O)                           \
         int ndim = PyArray_NDIM((PyArrayObject *)O);      \
         if (ndim != 1 && ndim != 2) {                     \
             return PyErr_Format(PyExc_NotImplementedError,\
-                    "expected 1D or 2D array (got %i)",   \
+                    "Expected 1D or 2D array, not %i.",   \
                     ndim);                                \
         }                                                 \
     } while (0)
 
 // Placeholder of not implemented pathways / debugging.
 # define AK_NOT_IMPLEMENTED(msg)                        \
     do {                                                \
@@ -3318,14 +3319,61 @@
         // NOTE: this will set PyErr if shape is not compatible
         return PyArray_Newshape(array, &shape, NPY_ANYORDER);
     }
     Py_INCREF(a);
     return a;
 }
 
+
+// Convert any slice to an ascending slice that covers the same values.
+static PyObject *
+slice_to_ascending_slice(PyObject *Py_UNUSED(m), PyObject *args) {
+
+    PyObject* slice;
+    PyObject* size;
+    if (!PyArg_ParseTuple(args,
+            "O!O!:slice_to_ascending_slice",
+            &PySlice_Type, &slice,
+            &PyLong_Type, &size)) {
+        return NULL;
+    }
+
+    Py_ssize_t step_count = -1;
+    Py_ssize_t start = 0;
+    Py_ssize_t stop = 0;
+    Py_ssize_t step = 0;
+
+    if (PySlice_Unpack(slice, &start, &stop, &step)) {
+        return NULL;
+    }
+    if (step > 0) {
+        Py_INCREF(slice);
+        return slice;
+    }
+    step_count = PySlice_AdjustIndices(
+            PyLong_AsSsize_t(size),
+            &start,
+            &stop,
+            step);
+
+    PyObject* asc_stop = PyLong_FromSsize_t(start + 1);
+    // step will be negative; shift original start value down to find new start
+    PyObject* asc_start = PyLong_FromSsize_t(start + (step * (step_count - 1)));
+    PyObject* asc_step = PyLong_FromSsize_t(-step);
+
+    // might be NULL, let return
+    PyObject* asc = PySlice_New(asc_start, asc_stop, asc_step);
+
+    Py_DECREF(asc_start);
+    Py_DECREF(asc_stop);
+    Py_DECREF(asc_step);
+
+    return asc;
+}
+
 //------------------------------------------------------------------------------
 // array utility
 
 static char *array_deepcopy_kwarg_names[] = {
     "array",
     "memo",
     NULL
@@ -4126,28 +4174,40 @@
     PyObject_VAR_HEAD
     Py_ssize_t block_count;
     Py_ssize_t row_count;
     Py_ssize_t bir_count;
     Py_ssize_t bir_capacity;
     BlockIndexRecord* bir;
     PyArray_Descr* dtype;
+    int8_t shape_recache;
+    PyObject* shape;
 } BlockIndexObject;
 
 
-// Returns a new reference to tuple. Returns NULL on error.
-static PyObject*
+// Returns a new reference to tuple. Returns NULL on error. Python already wraps negative numbers up to negative length when used in the sequence slot
+static inline PyObject*
 AK_BI_item(BlockIndexObject* self, Py_ssize_t i) {
     if (!((size_t)i < (size_t)self->bir_count)) {
         PyErr_SetString(PyExc_IndexError, "index out of range");
         return NULL;
     }
     BlockIndexRecord* biri = &self->bir[i];
     return Py_BuildValue("nn", biri->block, biri->column); // maybe NULL
 }
 
+// Returns a new reference to tuple. Returns NULL on error. Supports negative numbers up to negative length.
+static inline PyObject*
+AK_BI_item_wraps(BlockIndexObject* self, Py_ssize_t i)
+{
+    if (i < 0) {
+        i = self->bir_count + i;
+    }
+    return AK_BI_item(self, i);
+}
+
 //------------------------------------------------------------------------------
 // BI Iterator
 static PyTypeObject BIIterType;
 
 typedef struct BIIterObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
@@ -4289,27 +4349,27 @@
     }
     // use i to get index from selector
     Py_ssize_t t = 0;
     if (self->is_array) {
         PyArrayObject *a = (PyArrayObject *)self->selector;
         switch (PyArray_TYPE(a)) { // type of passed in array
             case NPY_INT64:
-                t = *(npy_int64*)PyArray_GETPTR1(a, i);
+                t = (Py_ssize_t)*(npy_int64*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_INT32:
                 t = *(npy_int32*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_INT16:
                 t = *(npy_int16*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_INT8:
                 t = *(npy_int8*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_UINT64:
-                t = *(npy_uint64*)PyArray_GETPTR1(a, i);
+                t = (Py_ssize_t)*(npy_uint64*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_UINT32:
                 t = *(npy_uint32*)PyArray_GETPTR1(a, i);
                 break;
             case NPY_UINT16:
                 t = *(npy_uint16*)PyArray_GETPTR1(a, i);
                 break;
@@ -4324,15 +4384,15 @@
             t = PyNumber_AsSsize_t(o, NULL);
         }
         else {
             PyErr_SetString(PyExc_TypeError, "element type not suitable for indexing");
             return NULL;
         }
     }
-    return AK_BI_item(self->bi, t); // return new ref
+    return AK_BI_item_wraps(self->bi, t); // return new ref
 }
 
 static PyObject *
 BIIterSeq_reversed(BIIterSeqObject *self) {
     return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_SEQUENCE);
 }
 
@@ -4503,15 +4563,14 @@
     .tp_dealloc = (destructor) BIIterBoolean_dealloc,
     .tp_iter = (getiterfunc) BIIterBoolean_iter,
     .tp_iternext = (iternextfunc) BIIterBoolean_iternext,
     .tp_methods = BIiterBoolean_methods,
     .tp_name = "arraykit.BlockIndexIteratorBoolean",
 };
 
-
 //------------------------------------------------------------------------------
 
 // NOTE: this constructor returns one of three different PyObject types. We do this to consolidate error reporting and type checks.
 static PyObject *
 BIIterSelector_new(BlockIndexObject *bi,
         PyObject* selector,
         int8_t reversed,
@@ -4574,15 +4633,14 @@
             return NULL;
         }
         len = PySlice_AdjustIndices(bi->bir_count, &pos, &stop, step);
         if (reversed) {
             pos += (step * (len - 1));
             step *= -1;
         }
-        // AK_DEBUG_MSG_OBJ("resolved slice", Py_BuildValue("nnnn", pos, stop, step, len));
     }
     else if (PyList_CheckExact(selector)) {
         if (kind == BIIS_UNKNOWN) {
             kind = BIIS_SEQUENCE;
         }
         else if (kind != BIIS_SEQUENCE) {
             PyErr_SetString(PyExc_TypeError, "Lists cannot be used as for non-sequence iterators");
@@ -4640,16 +4698,14 @@
     Py_INCREF(selector);
     return bii;
 error:
     // nothing shold be increfed when we get here
     return NULL;
 }
 
-
-
 //------------------------------------------------------------------------------
 
 // Returns 0 on succes, -1 on error.
 int
 AK_BI_BIR_new(BlockIndexObject* bi) {
     BlockIndexRecord* bir = (BlockIndexRecord*)PyMem_Malloc(
             sizeof(BlockIndexRecord) * bi->bir_capacity);
@@ -4724,14 +4780,17 @@
     }
     // handle all Py_ssize_t
     bi->block_count = block_count;
     bi->row_count = row_count;
     bi->bir_count = bir_count;
     bi->bir_capacity = bir_capacity;
 
+    bi->shape_recache = 1; // always init to true
+    bi->shape = NULL;
+
     // Load the bi->bir struct array, if defined
     bi->bir = NULL;
     // always set bi to capacity defined at this point
     if (AK_BI_BIR_new(bi)) {
         return -1;
     }
     if (bir_bytes != NULL) {
@@ -4748,25 +4807,26 @@
             bi->dtype = (PyArray_Descr*)dtype;
         }
         else {
             PyErr_SetString(PyExc_TypeError, "dtype argument must be a dtype");
             return -1;
         }
     }
+
     return 0;
 }
 
 static void
 BlockIndex_dealloc(BlockIndexObject *self) {
     if (self->bir != NULL) {
         PyMem_Free(self->bir);
     }
-    if (self->dtype != NULL) {
-        Py_DECREF((PyObject*)self->dtype);
-    }
+    // both dtype and shape might not be set
+    Py_XDECREF((PyObject*)self->dtype);
+    Py_XDECREF(self->shape);
     Py_TYPE(self)->tp_free((PyObject *)self);
 }
 
 static PyObject *
 BlockIndex_repr(BlockIndexObject *self) {
     PyObject* dt = self->dtype == NULL ? Py_None : (PyObject*) self->dtype;
     return PyUnicode_FromFormat("<%s(blocks: %i, rows: %i, columns: %i, dtype: %R)>",
@@ -4789,37 +4849,41 @@
 
     if (ndim < 1 || ndim > 2) {
         PyErr_Format(ErrorInitTypeBlocks, "Array block has invalid dimensions: %i", ndim);
         return NULL;
     }
     Py_ssize_t increment = ndim == 1 ? 1 : PyArray_DIM(a, 1);
 
-    // assign alignment on first observation; otherwise take
+    // assign alignment on first observation; otherwise force alignemnt. We do this regardless of if the array has no columns.
     Py_ssize_t alignment = PyArray_DIM(a, 0);
     if (self->row_count == -1) {
         self->row_count = alignment;
     }
     else if (self->row_count != alignment) {
         PyErr_Format(ErrorInitTypeBlocks,
                 "Array block has unaligned row count: found %i, expected %i",
                 alignment,
                 self->row_count);
         return NULL;
     }
 
+    // if we are not adding columns, we are not adding types, so we are not changing the  dtype or shape
     if (increment == 0) {
         Py_RETURN_FALSE;
     }
 
+
     PyArray_Descr* dt = PyArray_DESCR(a); // borrowed ref
-    if (self->dtype == NULL) {
+    self->shape_recache = 1; // adjusting columns, must recache shape
+
+    if (self->dtype == NULL) { // if not already set
         Py_INCREF((PyObject*)dt);
         self->dtype = dt;
     }
-    else if (!PyDataType_ISOBJECT(self->dtype)) {
+    else if (!PyDataType_ISOBJECT(self->dtype)) { // if object cannot resolve further
         PyArray_Descr* dtr = AK_ResolveDTypes(self->dtype, dt); // new ref
         Py_DECREF((PyObject*)self->dtype);
         self->dtype = dtr;
     }
 
     // create space for increment new records
     if (AK_BI_BIR_resize(self, increment)) {
@@ -4920,14 +4984,17 @@
         return NULL;
     }
     bi->block_count = self->block_count;
     bi->row_count = self->row_count;
     bi->bir_count = self->bir_count;
     bi->bir_capacity = self->bir_capacity;
 
+    bi->shape_recache = 1; // could copy, but do not want to copy a pending cache state
+    bi->shape = NULL;
+
     bi->bir = NULL;
     AK_BI_BIR_new(bi); // do initial alloc to self->bir_capacity
     memcpy(bi->bir,
             self->bir,
             self->bir_count * sizeof(BlockIndexRecord));
 
     bi->dtype = NULL;
@@ -4941,17 +5008,24 @@
 static PyObject*
 BlockIndex_iter(BlockIndexObject* self) {
     return BIIter_new(self, 0);
 }
 
 
 static PyObject *
-BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
-    // NOTE: this could be cached
-    return Py_BuildValue("nn", self->row_count, self->bir_count);
+BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure))
+{
+    if (self->shape == NULL || self->shape_recache) {
+        Py_XDECREF(self->shape); // get rid of old if it exists
+        self->shape = Py_BuildValue("nn", self->row_count, self->bir_count); // new ref
+    }
+    // shape is not null and shape_recache is false
+    Py_INCREF(self->shape); // for caller
+    self->shape_recache = 0;
+    return self->shape;
 }
 
 static PyObject *
 BlockIndex_rows_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
     return PyLong_FromSsize_t(self->row_count);
 }
 
@@ -5344,14 +5418,15 @@
     {"immutable_filter", immutable_filter, METH_O, NULL},
     {"mloc", mloc, METH_O, NULL},
     {"name_filter", name_filter, METH_O, NULL},
     {"shape_filter", shape_filter, METH_O, NULL},
     {"column_2d_filter", column_2d_filter, METH_O, NULL},
     {"column_1d_filter", column_1d_filter, METH_O, NULL},
     {"row_1d_filter", row_1d_filter, METH_O, NULL},
+    {"slice_to_ascending_slice", slice_to_ascending_slice, METH_VARARGS, NULL},
     {"array_deepcopy",
             (PyCFunction)array_deepcopy,
             METH_VARARGS | METH_KEYWORDS,
             NULL},
     {"resolve_dtype", resolve_dtype, METH_VARARGS, NULL},
     {"resolve_dtype_iter", resolve_dtype_iter, METH_O, NULL},
     {"first_true_1d",
```

### Comparing `arraykit-0.4.1/test/test_array_go.py` & `arraykit-0.4.2/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_block_index.py` & `arraykit-0.4.2/test/test_block_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 
 
 class TestUnit(unittest.TestCase):
 
     def test_block_index_init_a(self) -> None:
         bi1 = BlockIndex()
         self.assertEqual(bi1.dtype, np.dtype(float))
-        # print(bi1)
+        s = bi1.shape
+        self.assertEqual(s, (-1, 0))
+        del bi1
+        self.assertEqual(s, (-1, 0))
+        del s
 
     def test_block_index_init_b1(self) -> None:
         with self.assertRaises(ValueError):
             _ = BlockIndex(3, 2, 10, 2)
 
     def test_block_index_init_b1(self) -> None:
         with self.assertRaises(TypeError):
@@ -161,18 +165,20 @@
 
     #---------------------------------------------------------------------------
 
     def test_block_index_copy_a(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(12).reshape(2,6))
         bi1.register(np.arange(4).reshape(2,2))
-
+        s1 = bi1.shape
         bi2 = bi1.copy()
         self.assertEqual(bi1.to_list(), bi2.to_list())
-
+        self.assertEqual(bi1.dtype, bi2.dtype)
+        del bi1
+        self.assertEqual(bi2.shape, s1)
 
     def test_block_index_copy_b(self) -> None:
         dt1 = np.dtype(np.float64)
         bi1 = BlockIndex(0, 2, 0, 8, b"", dt1)
         bi2 = bi1.copy()
         dt2 = bi1.dtype
         del dt1
@@ -518,8 +524,31 @@
         bi1.register(np.arange(4).reshape(2,2))
         bi1.register(np.arange(2))
         self.assertEqual(list(bi1.iter_select(np.full(len(bi1), False))),
                 []
                 )
         self.assertEqual(list(bi1.iter_select(np.full(len(bi1), True))),
                 [(0, 0), (0, 1), (1, 0)]
-                )
+                )
+
+    #---------------------------------------------------------------------------
+    def test_block_index_iter_select_sequence_a(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(4).reshape(2,2))
+        bi1.register(np.arange(2))
+        bi1.register(np.arange(10).reshape(2,5))
+
+        self.assertEqual(list(bi1.iter_select([0, -1, -2, -8])),
+                [(0, 0), (2, 4), (2, 3), (0, 0)]
+                )
+        self.assertEqual(list(bi1.iter_select(np.array([0, -1, -2, -8]))),
+                [(0, 0), (2, 4), (2, 3), (0, 0)]
+                )
+
+    def test_block_index_iter_select_sequence_b(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(4).reshape(2,2))
+        bi1.register(np.arange(2))
+        bi1.register(np.arange(10).reshape(2,5))
+
+        with self.assertRaises(IndexError):
+            _ = list(bi1.iter_select([-9]))
```

### Comparing `arraykit-0.4.1/test/test_delimited_to_arrays.py` & `arraykit-0.4.2/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.2/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.2/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_pyi.py` & `arraykit-0.4.2/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_split_after_count.py` & `arraykit-0.4.2/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_type_discovery.py` & `arraykit-0.4.2/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.1/test/test_util.py` & `arraykit-0.4.2/test/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 from arraykit import column_1d_filter
 from arraykit import row_1d_filter
 from arraykit import mloc
 from arraykit import immutable_filter
 from arraykit import array_deepcopy
 from arraykit import isna_element
 from arraykit import dtype_from_element
-from arraykit import split_after_count
 from arraykit import count_iteration
 from arraykit import first_true_1d
 from arraykit import first_true_2d
+from arraykit import slice_to_ascending_slice
 
 from performance.reference.util import get_new_indexers_and_screen_ak as get_new_indexers_and_screen_full
 from arraykit import get_new_indexers_and_screen
 
 from performance.reference.util import mloc as mloc_ref
+from performance.reference.util import slice_to_ascending_slice as slice_to_ascending_slice_ref
 
 
 class TestUnit(unittest.TestCase):
 
     def test_mloc_a(self) -> None:
         a1 = np.arange(10)
         self.assertEqual(mloc(a1), mloc_ref(a1))
@@ -699,13 +700,50 @@
                 [1, 3, 2])
         self.assertEqual(first_true_2d(a1, axis=1, forward=True).tolist(),
                 [1, 0, 1, 1])
         self.assertEqual(first_true_2d(a1, axis=1, forward=False).tolist(),
                 [1, 0, 2, 1])
 
 
+    #---------------------------------------------------------------------------
+    def test_slice_to_ascending_slice_a(self) -> None:
+        self.assertEqual(slice_to_ascending_slice(
+                slice(5, 2, -1), 6),
+                slice(3, 6, 1),
+                )
+
+    def test_slice_to_ascending_slice_b(self) -> None:
+        self.assertEqual(slice_to_ascending_slice(
+                slice(2, 5, 1), 6),
+                slice(2, 5, 1),
+                )
 
+    def test_slice_to_ascending_slice_c(self) -> None:
+        with self.assertRaises(TypeError):
+            _ = slice_to_ascending_slice('a', 6)
+
+        with self.assertRaises(TypeError):
+            _ = slice_to_ascending_slice(slice(1, 4), 'x')
 
+    def test_slice_to_ascending_slice_d(self) -> None:
+        self.assertEqual(slice_to_ascending_slice(
+                slice(10, 2, -2), 12),
+                slice(4, 11, 2),
+                )
+
+    def test_slice_to_ascending_slice_e(self) -> None:
+        for slc, size in (
+                (slice(10, 2, -2), 12),
+                (slice(12, 2, -3), 12),
+                (slice(12, None, -4), 12),
+                (slice(76, 12, -8), 100),
+                (slice(81, 33, -12), 100),
+                (slice(97, 6, -7), 101),
+                ):
+            self.assertEqual(
+                slice_to_ascending_slice(slc, size),
+                slice_to_ascending_slice_ref(slc, size),
+                )
 
 
 if __name__ == '__main__':
     unittest.main()
```

