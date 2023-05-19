# Comparing `tmp/example_haskell_wheel-0.1.0a5-cp39-cp39-win_amd64.whl.zip` & `tmp/example_haskell_wheel-1.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 2705477 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      437 b- defN 23-Apr-01 18:54 example_haskell_wheel/__init__.py
--rw-rw-rw-  2.0 fat       62 b- defN 23-Apr-01 18:54 example_haskell_wheel/__main__.py
--rw-rw-rw-  2.0 fat 12510720 b- defN 23-Apr-01 18:57 example_haskell_wheel/_binding.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       28 b- defN 23-Apr-01 18:54 example_haskell_wheel/binding.def
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Apr-01 18:54 example_haskell_wheel/binding.i
--rw-rw-rw-  2.0 fat     2282 b- defN 23-Apr-01 18:56 example_haskell_wheel/binding.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1705 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 23-Apr-01 18:57 example_haskell_wheel-0.1.0a5.dist-info/RECORD
-12 files, 12518702 bytes uncompressed, 2703531 bytes compressed:  78.4%
+Zip file size: 2716991 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1590 b- defN 23-May-19 21:06 ExampleHaskellWheel/Binding.hs
+-rw-rw-rw-  2.0 fat      548 b- defN 23-May-19 21:06 example_haskell_wheel/__init__.py
+-rw-rw-rw-  2.0 fat      153 b- defN 23-May-19 21:06 example_haskell_wheel/__main__.py
+-rw-rw-rw-  2.0 fat 12546560 b- defN 23-May-19 21:13 example_haskell_wheel/_binding.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      597 b- defN 23-May-19 21:13 example_haskell_wheel/_binding.py
+-rw-rw-rw-  2.0 fat       28 b- defN 23-May-19 21:06 example_haskell_wheel/binding.def
+-rw-rw-rw-  2.0 fat     1218 b- defN 23-May-19 21:06 example_haskell_wheel/binding.i
+-rw-rw-rw-  2.0 fat     2394 b- defN 23-May-19 21:12 example_haskell_wheel/binding.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1815 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       78 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       42 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-19 21:13 example_haskell_wheel-1.0.0.dist-info/RECORD
+14 files, 12557505 bytes uncompressed, 2714791 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
+Filename: ExampleHaskellWheel/Binding.hs
+Comment: 
+
 Filename: example_haskell_wheel/__init__.py
 Comment: 
 
 Filename: example_haskell_wheel/__main__.py
 Comment: 
 
 Filename: example_haskell_wheel/_binding.cp39-win_amd64.pyd
 Comment: 
 
+Filename: example_haskell_wheel/_binding.py
+Comment: 
+
 Filename: example_haskell_wheel/binding.def
 Comment: 
 
 Filename: example_haskell_wheel/binding.i
 Comment: 
 
 Filename: example_haskell_wheel/binding.py
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/LICENSE
+Filename: example_haskell_wheel-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/METADATA
+Filename: example_haskell_wheel-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/WHEEL
+Filename: example_haskell_wheel-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/entry_points.txt
+Filename: example_haskell_wheel-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/top_level.txt
+Filename: example_haskell_wheel-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: example_haskell_wheel-0.1.0a5.dist-info/RECORD
+Filename: example_haskell_wheel-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## example_haskell_wheel/__init__.py

```diff
@@ -1,20 +1,26 @@
-from example_haskell_wheel._binding import (
-    hs_fib,
-    hs_defaultMain,
-    hs_rts_init,
-    hs_rts_exit,
+from typing import List
+
+from ._binding import (
+    unsafe_hs_example_haskell_wheel_version,
+    unsafe_hs_example_haskell_wheel_main,
+    unsafe_hs_init,
+    unsafe_hs_exit,
 )
 
+VERSION: str = "1.0.0"
+
 
-def fib(n: int) -> int:
-    hs_rts_init(["example-haskell-wheel"])
-    r = hs_fib(n)
-    hs_rts_exit()
-    return r
+def version() -> str:
+    try:
+        unsafe_hs_init([])
+        return str(unsafe_hs_example_haskell_wheel_version())
+    finally:
+        unsafe_hs_exit()
 
 
-def main():
-    print("Let's ask Haskell to compute some Fibonacci numbers:")
-    hs_rts_init(["example-haskell-wheel"])
-    hs_defaultMain(["1", "5", "42", "book"])
-    hs_rts_exit()
+def main(args: List[str]) -> None:
+    try:
+        unsafe_hs_init(args)
+        unsafe_hs_example_haskell_wheel_main()
+    finally:
+        unsafe_hs_exit()
```

## example_haskell_wheel/__main__.py

```diff
@@ -1,3 +1,10 @@
+import sys
 import example_haskell_wheel
 
-example_haskell_wheel.main()
+
+def main() -> None:
+    example_haskell_wheel.main(sys.argv)
+
+
+if __name__ == "__main__":
+    main()
```

## example_haskell_wheel/binding.i

```diff
@@ -1,23 +1,25 @@
 %module binding
 %{
-#include "Fib_stub.h"
+#include "ExampleHaskellWheel/Binding_stub.h"
 
-extern HsInt32 hs_fib(HsInt32 n);
+char * unsafe_hs_example_haskell_wheel_version() {
+  return hs_example_haskell_wheel_version();
+}
 
-extern void hs_defaultMain(HsInt32 argc, HsPtr argv);
+void unsafe_hs_example_haskell_wheel_main() {
+  hs_example_haskell_wheel_main();
+}
 
-void hs_rts_init(int argc, char **argv)
-{
+void unsafe_hs_init(int argc, char **argv) {
   hs_init(&argc, &argv);
 }
 
-void hs_rts_exit()
-{
-  void hs_exit();
+void unsafe_hs_exit() {
+  hs_exit();
 }
 %}
 
 %typemap(in) (int argc, char **argv) {
   /* Check if is a list */
   if (PyList_Check($input)) {
     int i;
@@ -39,11 +41,11 @@
   }
 }
 
 %typemap(freearg) (int argc, char **argv) {
   free((char *) $2);
 }
 
-int hs_fib(int n);
-void hs_defaultMain(int argc, char **argv);
-void hs_rts_init(int argc, char **argv);
-void hs_rts_exit();
+char * unsafe_hs_example_haskell_wheel_version();
+void unsafe_hs_example_haskell_wheel_main();
+void unsafe_hs_init(int argc, char **argv);
+void unsafe_hs_exit();
```

## example_haskell_wheel/binding.py

```diff
@@ -55,19 +55,19 @@
 
 class _SwigNonDynamicMeta(type):
     """Meta class to enforce nondynamic attributes (no new attributes) for a class"""
     __setattr__ = _swig_setattr_nondynamic_class_variable(type.__setattr__)
 
 
 
-def hs_fib(n):
-    return _binding.hs_fib(n)
+def unsafe_hs_example_haskell_wheel_version():
+    return _binding.unsafe_hs_example_haskell_wheel_version()
 
-def hs_defaultMain(argc):
-    return _binding.hs_defaultMain(argc)
+def unsafe_hs_example_haskell_wheel_main():
+    return _binding.unsafe_hs_example_haskell_wheel_main()
 
-def hs_rts_init(argc):
-    return _binding.hs_rts_init(argc)
+def unsafe_hs_init(argc):
+    return _binding.unsafe_hs_init(argc)
 
-def hs_rts_exit():
-    return _binding.hs_rts_exit()
+def unsafe_hs_exit():
+    return _binding.unsafe_hs_exit()
```

## Comparing `example_haskell_wheel-0.1.0a5.dist-info/LICENSE` & `example_haskell_wheel-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `example_haskell_wheel-0.1.0a5.dist-info/METADATA` & `example_haskell_wheel-1.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-haskell-wheel
-Version: 0.1.0a5
+Version: 1.0.0
 Summary: An experiment in publishing a Haskell library as a Python Wheel.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Wen Kokke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Requires-Python: <3.12,>=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: mypy
+Requires-Dist: types-setuptools (>=45) ; extra == 'mypy'
 Provides-Extra: test
 Requires-Dist: pytest (<8,>=7.1) ; extra == 'test'
 
 # example-haskell-wheel
 
 An experiment in publishing a Haskell library as a Python wheel.
```

## Comparing `example_haskell_wheel-0.1.0a5.dist-info/RECORD` & `example_haskell_wheel-1.0.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-example_haskell_wheel/__init__.py,sha256=b7qACylND8KOqPEDezFGvX5dzBbv5RUL0xWI1jjmj4A,437
-example_haskell_wheel/__main__.py,sha256=qLd7cZMuknWFeXfJxYT4tHdGs7DOA4EOX0U96-IMqxk,62
-example_haskell_wheel/_binding.cp39-win_amd64.pyd,sha256=GxvAlQhEUFaHb93iW2YhvSeGEZzWG-8yqwie93CpsZo,12510720
+ExampleHaskellWheel/Binding.hs,sha256=pjk_n2MtuNQ5SI2sDXRzb2BvIOLNN0pflxWO_VLxKwU,1590
+example_haskell_wheel/__init__.py,sha256=nrVo6qJM8eN_WcBIIFUaWFWCjbGZeBfbNAgKpL9JoWQ,548
+example_haskell_wheel/__main__.py,sha256=3sFeRZWHzXve3lnhVUOKgQYiDkq8X52V6pNX1EsB9f0,153
+example_haskell_wheel/_binding.cp39-win_amd64.pyd,sha256=bH_a4J9EJ2D3_RO6putAMypuIXSSrc7pmFXixHilGao,12546560
+example_haskell_wheel/_binding.py,sha256=ICqyFEFXpHDWkon209MQAx5_nMldz1ZzZQh8gBm2lyw,597
 example_haskell_wheel/binding.def,sha256=1LCHNMrMeviho0mKw0r4-Kf9GrPIty34P12yAUyuovw,28
-example_haskell_wheel/binding.i,sha256=U9XKRXZ0JouyPuU2CAmyfG1yS9qeSnMnkJuBIdjlspk,1060
-example_haskell_wheel/binding.py,sha256=PdKpbK2TG6XPwqjwugVFOBNAoVXNfcKgFTdAKK2jYvI,2282
-example_haskell_wheel-0.1.0a5.dist-info/LICENSE,sha256=OwSA4A7mUJqR-q9SajMzNwUeJtBDpSz5iSX9IV_f_gs,1087
-example_haskell_wheel-0.1.0a5.dist-info/METADATA,sha256=9JJHL6OsBiJTnrXYFqkq8lflfGj0bndnNPUfdDJSEJk,1705
-example_haskell_wheel-0.1.0a5.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-example_haskell_wheel-0.1.0a5.dist-info/entry_points.txt,sha256=QoIbCqp40lMZppzeTM4ySwFHA4K0X3ofkNZyKyOvpxU,69
-example_haskell_wheel-0.1.0a5.dist-info/top_level.txt,sha256=M2LIGfQenD623rwokg021qLPdgBM6eUVKvg2_-HgSRQ,22
-example_haskell_wheel-0.1.0a5.dist-info/RECORD,,
+example_haskell_wheel/binding.i,sha256=7BzeIx2ODMUgIEa0hGEuXTzqvDWcETurMpS6she8F24,1218
+example_haskell_wheel/binding.py,sha256=JU8N1uZ5iipbGjQ1PLbioxt_fFAL_6bv3YkwSfGFskM,2394
+example_haskell_wheel-1.0.0.dist-info/LICENSE,sha256=OwSA4A7mUJqR-q9SajMzNwUeJtBDpSz5iSX9IV_f_gs,1087
+example_haskell_wheel-1.0.0.dist-info/METADATA,sha256=tCFOziRmjW-RLes9b2qkMgBtsl-GBZminIZmIVqple8,1815
+example_haskell_wheel-1.0.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+example_haskell_wheel-1.0.0.dist-info/entry_points.txt,sha256=gaWDiPzFGI34Cit7U2p4C5KYPSr4yLDunG49C9w3AKc,78
+example_haskell_wheel-1.0.0.dist-info/top_level.txt,sha256=XgRwAoCA0cncXocSk5s7nErBioiIGC8bIMUx8t425Z0,42
+example_haskell_wheel-1.0.0.dist-info/RECORD,,
```

