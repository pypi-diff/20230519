# Comparing `tmp/algokit_client_generator-0.1.0b2-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 13241 bytes, number of entries: 14
+Zip file size: 13219 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3122 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
 -rw-r--r--  2.0 unx    22444 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     5986 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
--rw-r--r--  2.0 unx     3847 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
+-rw-r--r--  2.0 unx     3913 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx      635 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/WHEEL
--rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1297 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/RECORD
-14 files, 41391 bytes uncompressed, 11025 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      543 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1297 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b3.dist-info/RECORD
+14 files, 41365 bytes uncompressed, 11003 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b2.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b2.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b3.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b2.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b2.dist-info/entry_points.txt
+Filename: algokit_client_generator-0.1.0b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b2.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/utils.py

```diff
@@ -33,14 +33,16 @@
             inner_type = ", ".join([map_abi_type_to_python(abi_type)] * array_size)
             tuple_type = f"tuple[{inner_type}]"
             if abi_type == "byte":
                 return f"bytes | {tuple_type}"
             return tuple_type
         else:
             abi_type = abi_type[:-2]
+            if abi_type == "byte":
+                return "bytes"
             return f"list[{map_abi_type_to_python(abi_type)}]"
     if abi_type.startswith("(") and abi_type.endswith(")"):
         abi_type = abi_type[1:-1]
         inner_types = [map_abi_type_to_python(t) for t in abi_type.split(",")]
         return f"tuple[{', '.join(inner_types)}]"
     # TODO validate or annotate ints
     python_type = {
```

## Comparing `algokit_client_generator-0.1.0b2.dist-info/LICENSE` & `algokit_client_generator-0.1.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b2.dist-info/METADATA` & `algokit_client_generator-0.1.0b3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: algokit-utils (>=1.2.0b2,<2.0.0)
-Requires-Dist: beaker-pyteal (>=1.0.0,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # algokit-client-generator-py
```

## Comparing `algokit_client_generator-0.1.0b2.dist-info/RECORD` & `algokit_client_generator-0.1.0b3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_client_generator/__init__.py,sha256=ikLxrMdPVjpmrVYDdHbunvzUwiXqrCdvp8Qi5x0gC0c,91
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
 algokit_client_generator/cli.py,sha256=F7dcZtmliFiDCZEU5hc2ya9BPxoi7fKx49Azx0tqOrc,1783
 algokit_client_generator/document.py,sha256=-IIw0wXqZ9NesrGGbTXANcQQrggAX-DBcegTq9gOJ3s,3122
 algokit_client_generator/generator.py,sha256=meXSfSB6fzX9kYRu7FFyHcRQcC0AorRieeX2EAgViag,22444
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=LcPiMhvnnscvnACk_YGzweEnzQ7V7kQyDvQ94Uo9Nlo,5986
-algokit_client_generator/utils.py,sha256=iILQJ-KNSPigkH6Hn8-lJUAMf2dU4cvDKsHFuF9vw5M,3847
+algokit_client_generator/utils.py,sha256=HoGDeseuPl0E5b3EVErwiy6q5Q0H8a9nt5DPyMlGqSI,3913
 algokit_client_generator/writer.py,sha256=MF46CQ8q1nW-K66RcKcXYE1uArrNRKHWF-uKQT8eziU,890
-algokit_client_generator-0.1.0b2.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b2.dist-info/METADATA,sha256=P0r-6hVmEFjp2etgM18L5TWl22ysvtfdZ2Vlp1N9E5g,635
-algokit_client_generator-0.1.0b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_client_generator-0.1.0b2.dist-info/entry_points.txt,sha256=Z4YZmQEtOuvNIRYqH_aAJeJymkTBWrOnZW3HLaT7qBc,78
-algokit_client_generator-0.1.0b2.dist-info/RECORD,,
+algokit_client_generator-0.1.0b3.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b3.dist-info/METADATA,sha256=6UqHxMtouGTTLmIZB0lfVBJW2TuWdqrPRBat20ZMr4w,543
+algokit_client_generator-0.1.0b3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_client_generator-0.1.0b3.dist-info/entry_points.txt,sha256=Z4YZmQEtOuvNIRYqH_aAJeJymkTBWrOnZW3HLaT7qBc,78
+algokit_client_generator-0.1.0b3.dist-info/RECORD,,
```

