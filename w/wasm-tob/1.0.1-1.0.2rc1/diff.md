# Comparing `tmp/wasm-tob-1.0.1.tar.gz` & `tmp/wasm_tob-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm-tob-1.0.1.tar", last modified: Wed Apr  5 22:33:16 2023, max compression
+gzip compressed data, was "wasm_tob-1.0.2rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wasm-tob-1.0.1.tar` & `wasm_tob-1.0.2rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1162 2023-04-05 22:33:08.356674 wasm-tob-1.0.1/LICENSE
--rw-r--r--   0        0        0     4972 2023-04-05 22:33:08.356674 wasm-tob-1.0.1/README.md
--rw-r--r--   0        0        0     1250 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2144 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/__init__.py
--rw-r--r--   0        0        0     2140 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/__main__.py
--rw-r--r--   0        0        0     2436 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/compat.py
--rw-r--r--   0        0        0     2078 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/decode.py
--rw-r--r--   0        0        0     2881 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/formatter.py
--rw-r--r--   0        0        0     1218 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/immtypes.py
--rw-r--r--   0        0        0     6290 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/modtypes.py
--rw-r--r--   0        0        0    13251 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/opcodes.py
--rw-r--r--   0        0        0    10560 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/types.py
--rw-r--r--   0        0        0     1672 2023-04-05 22:33:08.404673 wasm-tob-1.0.1/wasm_tob/wasmtypes.py
--rw-r--r--   0        0        0     6064 1970-01-01 00:00:00.000000 wasm-tob-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1162 2023-05-19 17:19:44.809245 wasm_tob-1.0.2rc1/LICENSE
+-rw-r--r--   0        0        0     4972 2023-05-19 17:19:44.809245 wasm_tob-1.0.2rc1/README.md
+-rw-r--r--   0        0        0     1250 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2149 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/__init__.py
+-rw-r--r--   0        0        0     2140 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/__main__.py
+-rw-r--r--   0        0        0     2436 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/compat.py
+-rw-r--r--   0        0        0     2078 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/decode.py
+-rw-r--r--   0        0        0     2881 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/formatter.py
+-rw-r--r--   0        0        0     1218 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/immtypes.py
+-rw-r--r--   0        0        0     6290 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/modtypes.py
+-rw-r--r--   0        0        0    13251 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/opcodes.py
+-rw-r--r--   0        0        0    10560 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/types.py
+-rw-r--r--   0        0        0     1672 2023-05-19 17:19:44.853242 wasm_tob-1.0.2rc1/wasm_tob/wasmtypes.py
+-rw-r--r--   0        0        0     6067 1970-01-01 00:00:00.000000 wasm_tob-1.0.2rc1/PKG-INFO
```

### Comparing `wasm-tob-1.0.1/LICENSE` & `wasm_tob-1.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/README.md` & `wasm_tob-1.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/pyproject.toml` & `wasm_tob-1.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/__init__.py` & `wasm_tob-1.0.2rc1/wasm_tob/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import unicode_literals
 
-__version__ = '1.0.1'
+__version__ = "1.0.2.pre1"
 
 from .decode import (
     decode_bytecode,
     decode_module,
 )
 
 from .formatter import (
@@ -71,15 +71,15 @@
     INSN_LEAVE_BLOCK,
     INSN_BRANCH,
     INSN_NO_FLOW,
 )
 
 for cur_op in opcodes.OPCODES:
     globals()[
-        'OP_' + cur_op.mnemonic.upper().replace('.', '_').replace('/', '_')
+        "OP_" + cur_op.mnemonic.upper().replace(".", "_").replace("/", "_")
     ] = cur_op.id
 
 from .wasmtypes import (
     UInt8Field,
     UInt16Field,
     UInt32Field,
     UInt64Field,
```

### Comparing `wasm-tob-1.0.1/wasm_tob/__main__.py` & `wasm_tob-1.0.2rc1/wasm_tob/__main__.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/compat.py` & `wasm_tob-1.0.2rc1/wasm_tob/compat.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/decode.py` & `wasm_tob-1.0.2rc1/wasm_tob/decode.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/formatter.py` & `wasm_tob-1.0.2rc1/wasm_tob/formatter.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/immtypes.py` & `wasm_tob-1.0.2rc1/wasm_tob/immtypes.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/modtypes.py` & `wasm_tob-1.0.2rc1/wasm_tob/modtypes.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/opcodes.py` & `wasm_tob-1.0.2rc1/wasm_tob/opcodes.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/types.py` & `wasm_tob-1.0.2rc1/wasm_tob/types.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/wasm_tob/wasmtypes.py` & `wasm_tob-1.0.2rc1/wasm_tob/wasmtypes.py`

 * *Files identical despite different names*

### Comparing `wasm-tob-1.0.1/PKG-INFO` & `wasm_tob-1.0.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-tob
-Version: 1.0.1
+Version: 1.0.2rc1
 Summary: WebAssembly decoder & disassembler
 Keywords: wasm,disassembler,decoder
 Author-email: Trail of Bits <opensource@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

