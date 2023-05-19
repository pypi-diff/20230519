# Comparing `tmp/ever_playground-0.4.2.tar.gz` & `tmp/ever_playground-0.5.0.tar.gz`

## Comparing `ever_playground-0.4.2.tar` & `ever_playground-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 ever_playground-0.4.2/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.4.2/.gitignore
--rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.4.2/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.4.2/README.md
--rw-rw-r--   0     1000     1000     2484 2023-05-17 14:29:51.000000 ever_playground-0.4.2/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     4627 2023-05-17 11:29:17.000000 ever_playground-0.4.2/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     4363 2023-05-16 17:02:44.000000 ever_playground-0.4.2/examples.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.4.2/pyproject.toml
--rw-rw-r--   0     1000     1000    14446 2023-05-17 11:29:09.000000 ever_playground-0.4.2/src/lib.rs
--rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.4.2/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.4.2/src/utils.rs
--rw-rw-r--   0     1000     1000    24701 2023-05-17 14:31:56.000000 ever_playground-0.4.2/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 ever_playground-0.5.0/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.5.0/.gitignore
+-rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.5.0/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.5.0/README.md
+-rw-rw-r--   0     1000     1000     4015 2023-05-19 19:14:08.000000 ever_playground-0.5.0/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     4917 2023-05-19 18:26:44.000000 ever_playground-0.5.0/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2244 2023-05-19 14:55:11.000000 ever_playground-0.5.0/examples/basics.py
+-rw-rw-r--   0     1000     1000     1874 2023-05-19 15:59:34.000000 ever_playground-0.5.0/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     2331 2023-05-19 14:55:00.000000 ever_playground-0.5.0/examples/runvm.py
+-rw-rw-r--   0     1000     1000     2919 2023-05-19 19:15:04.000000 ever_playground-0.5.0/examples/testgiver.py
+-rw-rw-r--   0     1000     1000     3601 2023-05-19 15:12:42.000000 ever_playground-0.5.0/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.5.0/pyproject.toml
+-rw-rw-r--   0     1000     1000    15132 2023-05-19 18:27:17.000000 ever_playground-0.5.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.5.0/src/tests.rs
+-rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.5.0/src/utils.rs
+-rw-rw-r--   0     1000     1000    24701 2023-05-19 19:17:35.000000 ever_playground-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.5.0/PKG-INFO
```

### Comparing `ever_playground-0.4.2/Cargo.toml` & `ever_playground-0.5.0/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ever-playground"
-version = "0.4.2"
+version = "0.5.0"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `ever_playground-0.4.2/README.md` & `ever_playground-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.2/ever_playground/ever_playground.pyi` & `ever_playground-0.5.0/ever_playground/ever_playground.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -68,22 +68,34 @@
     """
 
     def s(self, slice: Slice) -> Builder:
         """
         Appends a Builder with a Slice.
         """
 
+    def b(self, builder: Builder) -> Builder:
+        """
+        Appends a Builder with another Builder.
+        """
+
     def i(self, bits: int, integer: int) -> Builder:
         """
         Appends a Builder with an integer of specified length.
         """
 
+    def ib(self, bin: str) -> Builder:
+        """
+        Appends a Builder with an integer from binary string.
+        """
+
     def x(self, bitstring: str) -> Builder:
         """
         Appends a Builder with a bitstring.
+
+        TODO describe what TVM bitstring is
         """
 
     def r(self, cell: Cell) -> Builder:
         """
         Appends a Builder with a Cell.
         """
```

### Comparing `ever_playground-0.4.2/pyproject.toml` & `ever_playground-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.2/src/lib.rs` & `ever_playground-0.5.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use pyo3::{
     prelude::*,
     basic::CompareOp,
     exceptions::PyRuntimeError,
     types::{PyBytes, PyDict, PyList, PyLong, PyTuple},
 };
 
-use ton_types::{BuilderData, Cell as InternalCell, HashmapE, HashmapType, SliceData};
+use ton_types::{BuilderData, Cell as InternalCell, HashmapE, HashmapType, SliceData, IBitstring};
 use ton_vm::{
     error::tvm_exception_full,
     executor::{Engine, EngineTraceInfo, gas::gas_state::Gas},
     stack::{
         StackItem, Stack,
         integer::{IntegerData, utils::process_value},
         savelist::SaveList,
@@ -154,26 +154,41 @@
         Self::default()
     }
     fn s(mut slf: PyRefMut<Self>, slice: Slice) -> PyResult<PyRefMut<Self>> {
         slf.builder.checked_append_references_and_data(&slice.slice)
             .map_err(runtime_err)?;
         Ok(slf)
     }
+    fn b(mut slf: PyRefMut<Self>, builder: Builder) -> PyResult<PyRefMut<Self>> {
+        slf.builder.append_builder(&builder.builder).map_err(runtime_err)?;
+        Ok(slf)
+    }
     fn i(mut slf: PyRefMut<Self>, bits: usize, integer: BigInt) -> PyResult<PyRefMut<Self>> {
         if bits == 0 {
             return err!("bits must be greater than 0")
         }
         let bytes = if integer.sign() == Sign::Minus {
             signed_int_serialize(integer, bits)?
         }else {
             unsigned_int_serialize(integer, bits)?
         };
         slf.builder.append_raw(&bytes, bits).map_err(runtime_err)?;
         Ok(slf)
     }
+    // TODO consider moving this to Python library (by using superclassing)
+    fn ib(mut slf: PyRefMut<Self>, bin: String) -> PyResult<PyRefMut<Self>> {
+        for digit in bin.chars() {
+            match digit {
+                '0' => { slf.builder.append_bit_zero().map_err(runtime_err)?; }
+                '1' => { slf.builder.append_bit_one().map_err(runtime_err)?; }
+                _ => return err!("Failed to parse binary string {}", bin)
+            }
+        }
+        Ok(slf)
+    }
     fn x(mut slf: PyRefMut<Self>, bitstring: String) -> PyResult<PyRefMut<Self>> {
         let slice = SliceData::from_string(&bitstring)
             .map_err(runtime_err)?;
         slf.builder.checked_append_references_and_data(&slice)
             .map_err(runtime_err)?;
         Ok(slf)
     }
```

### Comparing `ever_playground-0.4.2/src/tests.rs` & `ever_playground-0.5.0/src/tests.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.2/src/utils.rs` & `ever_playground-0.5.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.2/Cargo.lock` & `ever_playground-0.5.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.4.2"
+version = "0.5.0"
 dependencies = [
  "num-bigint",
  "pyo3",
  "ton_block",
  "ton_labs_assembler",
  "ton_types",
  "ton_vm",
```

### Comparing `ever_playground-0.4.2/PKG-INFO` & `ever_playground-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.4.2
+Version: 0.5.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

